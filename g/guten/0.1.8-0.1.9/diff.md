# Comparing `tmp/guten-0.1.8.tar.gz` & `tmp/guten-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guten-0.1.8.tar", max compression
+gzip compressed data, was "guten-0.1.9.tar", max compression
```

## Comparing `guten-0.1.8.tar` & `guten-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       54 2022-12-25 18:53:57.314870 guten-0.1.8/README.md
--rw-r--r--   0        0        0        0 2022-12-24 11:32:16.552571 guten-0.1.8/guten/__init__.py
--rw-r--r--   0        0        0      876 2022-12-26 05:13:17.812880 guten-0.1.8/guten/__main__.py
--rw-r--r--   0        0        0     1207 2022-12-26 04:57:45.933337 guten-0.1.8/guten/backend.py
--rw-r--r--   0        0        0     3844 2022-12-27 06:29:19.860678 guten-0.1.8/guten/backends/html.py
--rw-r--r--   0        0        0     2443 2022-12-27 06:42:31.641999 guten-0.1.8/guten/backends/text.py
--rw-r--r--   0        0        0     3272 2022-12-26 05:15:30.047264 guten-0.1.8/guten/config.py
--rw-r--r--   0        0        0     3236 2023-01-02 04:55:36.341134 guten-0.1.8/guten/press.py
--rw-r--r--   0        0        0      184 2022-12-25 03:46:23.026388 guten-0.1.8/guten/source.py
--rw-r--r--   0        0        0      362 2022-12-25 18:33:08.012285 guten-0.1.8/guten/utils.py
--rw-r--r--   0        0        0      376 2023-01-02 04:57:16.978234 guten-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 guten-0.1.8/setup.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 guten-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       54 2022-12-25 18:53:57.314870 guten-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-12-24 11:32:16.552571 guten-0.1.9/guten/__init__.py
+-rw-r--r--   0        0        0      876 2022-12-26 05:13:17.812880 guten-0.1.9/guten/__main__.py
+-rw-r--r--   0        0        0     1207 2022-12-26 04:57:45.933337 guten-0.1.9/guten/backend.py
+-rw-r--r--   0        0        0     4930 2023-04-08 17:27:57.778085 guten-0.1.9/guten/backends/html.py
+-rw-r--r--   0        0        0     2443 2022-12-27 06:42:31.641999 guten-0.1.9/guten/backends/text.py
+-rw-r--r--   0        0        0     3272 2022-12-26 05:15:30.047264 guten-0.1.9/guten/config.py
+-rw-r--r--   0        0        0     3383 2023-04-08 16:56:06.506470 guten-0.1.9/guten/press.py
+-rw-r--r--   0        0        0      184 2022-12-25 03:46:23.026388 guten-0.1.9/guten/source.py
+-rw-r--r--   0        0        0      362 2022-12-25 18:33:08.012285 guten-0.1.9/guten/utils.py
+-rw-r--r--   0        0        0      376 2023-04-08 17:33:39.210665 guten-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 guten-0.1.9/setup.py
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 guten-0.1.9/PKG-INFO
```

### Comparing `guten-0.1.8/guten/__main__.py` & `guten-0.1.9/guten/__main__.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.8/guten/backend.py` & `guten-0.1.9/guten/backend.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.8/guten/backends/html.py` & `guten-0.1.9/guten/backends/html.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List
 from pathlib import Path
 from datetime import datetime, timedelta, timezone
 from dateutil.parser import parse as date_parse
 
 from guten.backend import Backend
 from guten.press import FetchedSourceGroup
+from guten.utils import eprint
 
 
 METADATA_FILE = ".metadata"
 
 def begin_document():
     return "<html>"
 
@@ -79,29 +80,51 @@
     return f"""
         <details>
             <summary><a href='{data['link']}'>{data['title']}</a></summary>
             {data['summary']}
         </details>
     """
 
+def DEFAULT_HIST(today):
+    return today - timedelta(days=5)
+
+
+def parse_metadata(data, today):
+    dates = [date_parse(d.strip()) for d in data.split(";")]
+
+    if len(dates) == 0:
+        return DEFAULT_HIST(today), DEFAULT_HIST(today)
+    elif len(dates) == 1:
+        return dates[0], DEFAULT_HIST(today)
+    else:
+        return dates[0], dates[1]
+    
+
 class HTMLBackend(Backend):
     async def run(self, groups: List[FetchedSourceGroup], output_dir: Path) -> Path:
         today = datetime.now(timezone.utc)
         output_file = output_dir / f"{today.year}-{today.month}-{today.day}.html"
         metadata_file = output_dir / METADATA_FILE
 
-        previous_run_date = today - timedelta(days=5)
+        hist0, hist1 = None, None
         if metadata_file.exists():
             with open(metadata_file, "r") as f:
                 data = f.read()
-            temp = date_parse(data)
-            if temp.date() != today.date():
-                previous_run_date = temp
-            else:
-                previous_run_date = today - timedelta(days=1)
+                hist0, hist1 = parse_metadata(data, today)
+        else:
+            hist0, hist1 = DEFAULT_HIST(today), DEFAULT_HIST(today)
+
+        # Now, hist0 and hist1 have been set
+
+        # If guten is run more than once, we use hist1 as the previous run
+        # date. This approximates a fresh re-run of guten for that day.
+        if hist0.date() == today.date():
+            previous_run_date = hist1
+
+        eprint(f"Showing entries published after {previous_run_date}")
 
         with open(output_file, "w") as f:
             f.write(begin_document())
             f.write(preamble())
 
             f.write(begin_body())
 
@@ -137,14 +160,25 @@
 
             f.write(small(f"Generated at: {today.isoformat()}"))
 
             f.write(end_body())
             f.write(end_document())
 
         with open(metadata_file, "w") as f:
-            f.write(today.isoformat())
+            # If hist0.date() == today.date(), set metadate file to:
+            # <hist0>;<hist1>
+            # Otherwise, set metadata file to:
+            # <today>;<hist0>
+            if hist0.date() == today.date():
+                f.write(hist0.isoformat())
+                f.write(";")
+                f.write(hist1.isoformat())
+            else:
+                f.write(today.isoformat())
+                f.write(";")
+                f.write(hist0.isoformat())
 
         return output_file
 
 
 
 __backend__ = HTMLBackend
```

### Comparing `guten-0.1.8/guten/backends/text.py` & `guten-0.1.9/guten/backends/text.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.8/guten/config.py` & `guten-0.1.9/guten/config.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.8/guten/press.py` & `guten-0.1.9/guten/press.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
             # Parse feed
             data = feedparser.parse(feed)
 
             # Convert to data frame
             df = pd.DataFrame(data["entries"])
 
+            if "published" not in df:
+                if "updated" in data["feed"]:
+                    df["published"] = data["feed"]["updated"]
+
             eprint(f"Fetched '{source}'")
 
             return (source, df)
         except Exception as e:
             raise PressException(f"Failed to fetch source '{source}'", e)
 
     async def fetch_source_group(self, client: httpx.AsyncClient, source_group: SourceGroup) -> FetchedSourceGroup:
```

### Comparing `guten-0.1.8/setup.py` & `guten-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pandas>=1.5.2,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'pytz>=2022.7,<2023.0',
  'toml==0.10.2']
 
 setup_kwargs = {
     'name': 'guten',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# guten\n\nCompile RSS/Atom feeds into a combined feed.\n',
     'author': 'Elton',
     'author_email': 'eltonp3103@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `guten-0.1.8/PKG-INFO` & `guten-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guten
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Elton
 Author-email: eltonp3103@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

