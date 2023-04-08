# Comparing `tmp/har_toolkit-0.2.0.tar.gz` & `tmp/har_toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har_toolkit-0.2.0.tar", last modified: Mon Sep 19 04:35:18 2022, max compression
+gzip compressed data, was "har_toolkit-0.3.0.tar", last modified: Sat Apr  8 20:54:54 2023, max compression
```

## Comparing `har_toolkit-0.2.0.tar` & `har_toolkit-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2022-09-19 04:35:18.088748 har_toolkit-0.2.0/
--rw-r--r--   0 mason     (1000) mason     (1000)    35150 2022-09-17 20:44:16.000000 har_toolkit-0.2.0/LICENSE
--rw-r--r--   0 mason     (1000) mason     (1000)     1205 2022-09-19 04:35:18.088748 har_toolkit-0.2.0/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)      630 2022-09-19 03:01:05.000000 har_toolkit-0.2.0/README.md
--rw-r--r--   0 mason     (1000) mason     (1000)      666 2022-09-19 04:34:47.000000 har_toolkit-0.2.0/pyproject.toml
--rw-r--r--   0 mason     (1000) mason     (1000)       38 2022-09-19 04:35:18.088748 har_toolkit-0.2.0/setup.cfg
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2022-09-19 04:35:18.085414 har_toolkit-0.2.0/src/
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2022-09-19 04:35:18.085414 har_toolkit-0.2.0/src/har_toolkit/
--rw-r--r--   0 mason     (1000) mason     (1000)       95 2022-09-19 02:52:22.000000 har_toolkit-0.2.0/src/har_toolkit/__init__.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2022-09-19 04:35:18.088748 har_toolkit-0.2.0/src/har_toolkit/har_objects/
--rw-r--r--   0 mason     (1000) mason     (1000)      206 2022-09-18 05:47:14.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      857 2022-09-18 05:17:26.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/bases.py
--rw-r--r--   0 mason     (1000) mason     (1000)       99 2022-09-18 05:31:52.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/browser.py
--rw-r--r--   0 mason     (1000) mason     (1000)      411 2022-09-18 05:44:26.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/cache.py
--rw-r--r--   0 mason     (1000) mason     (1000)      303 2022-09-18 05:44:55.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/cache_state.py
--rw-r--r--   0 mason     (1000) mason     (1000)      847 2022-09-19 04:14:08.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/content.py
--rw-r--r--   0 mason     (1000) mason     (1000)      412 2022-09-18 05:34:54.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/cookie.py
--rw-r--r--   0 mason     (1000) mason     (1000)       99 2022-09-18 05:35:26.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/creator.py
--rw-r--r--   0 mason     (1000) mason     (1000)      746 2022-09-18 05:36:18.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/entry.py
--rw-r--r--   0 mason     (1000) mason     (1000)      117 2022-09-19 02:38:55.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/exceptions.py
--rw-r--r--   0 mason     (1000) mason     (1000)       96 2022-09-18 05:36:54.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/header.py
--rw-r--r--   0 mason     (1000) mason     (1000)      542 2022-09-18 05:37:27.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/page.py
--rw-r--r--   0 mason     (1000) mason     (1000)      246 2022-09-18 05:37:44.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/page_timings.py
--rw-r--r--   0 mason     (1000) mason     (1000)      305 2022-09-18 05:38:02.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/params.py
--rw-r--r--   0 mason     (1000) mason     (1000)      407 2022-09-18 05:38:39.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/post_data.py
--rw-r--r--   0 mason     (1000) mason     (1000)      101 2022-09-18 05:39:04.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/query_string.py
--rw-r--r--   0 mason     (1000) mason     (1000)     1170 2022-09-19 02:52:59.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/request.py
--rw-r--r--   0 mason     (1000) mason     (1000)      803 2022-09-18 05:40:19.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/response.py
--rw-r--r--   0 mason     (1000) mason     (1000)      415 2022-09-18 05:40:34.000000 har_toolkit-0.2.0/src/har_toolkit/har_objects/timings.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2689 2022-09-19 03:54:33.000000 har_toolkit-0.2.0/src/har_toolkit/parser.py
--rw-r--r--   0 mason     (1000) mason     (1000)      345 2022-09-19 02:59:09.000000 har_toolkit-0.2.0/src/har_toolkit/utils.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2022-09-19 04:35:18.085414 har_toolkit-0.2.0/src/har_toolkit.egg-info/
--rw-r--r--   0 mason     (1000) mason     (1000)     1205 2022-09-19 04:35:18.000000 har_toolkit-0.2.0/src/har_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)     1017 2022-09-19 04:35:18.000000 har_toolkit-0.2.0/src/har_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 mason     (1000) mason     (1000)        1 2022-09-19 04:35:18.000000 har_toolkit-0.2.0/src/har_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 mason     (1000) mason     (1000)       12 2022-09-19 04:35:18.000000 har_toolkit-0.2.0/src/har_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/
+-rw-r--r--   0 mason     (1000) mason     (1000)    35150 2022-09-17 20:44:16.000000 har_toolkit-0.3.0/LICENSE
+-rw-r--r--   0 mason     (1000) mason     (1000)     1199 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)      624 2022-09-20 22:43:28.000000 har_toolkit-0.3.0/README.md
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/har_toolkit/
+-rw-r--r--   0 mason     (1000) mason     (1000)       95 2022-09-19 02:52:22.000000 har_toolkit-0.3.0/har_toolkit/__init__.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/har_toolkit/har_browser/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2022-10-04 22:54:50.000000 har_toolkit-0.3.0/har_toolkit/har_browser/harbrowser.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/har_toolkit/har_objects/
+-rw-r--r--   0 mason     (1000) mason     (1000)      206 2022-09-18 05:47:14.000000 har_toolkit-0.3.0/har_toolkit/har_objects/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      974 2023-04-08 19:20:59.000000 har_toolkit-0.3.0/har_toolkit/har_objects/bases.py
+-rw-r--r--   0 mason     (1000) mason     (1000)       99 2022-09-18 05:31:52.000000 har_toolkit-0.3.0/har_toolkit/har_objects/browser.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      411 2022-09-18 05:44:26.000000 har_toolkit-0.3.0/har_toolkit/har_objects/cache.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      303 2022-09-18 05:44:55.000000 har_toolkit-0.3.0/har_toolkit/har_objects/cache_state.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1163 2023-04-08 19:34:06.000000 har_toolkit-0.3.0/har_toolkit/har_objects/content.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      412 2022-09-18 05:34:54.000000 har_toolkit-0.3.0/har_toolkit/har_objects/cookie.py
+-rw-r--r--   0 mason     (1000) mason     (1000)       99 2022-09-18 05:35:26.000000 har_toolkit-0.3.0/har_toolkit/har_objects/creator.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      801 2023-04-08 18:28:00.000000 har_toolkit-0.3.0/har_toolkit/har_objects/entry.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      117 2022-09-19 02:38:55.000000 har_toolkit-0.3.0/har_toolkit/har_objects/exceptions.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      181 2023-04-08 19:37:26.000000 har_toolkit-0.3.0/har_toolkit/har_objects/header.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      542 2022-09-18 05:37:27.000000 har_toolkit-0.3.0/har_toolkit/har_objects/page.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      246 2022-09-18 05:37:44.000000 har_toolkit-0.3.0/har_toolkit/har_objects/page_timings.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      305 2022-09-18 05:38:02.000000 har_toolkit-0.3.0/har_toolkit/har_objects/params.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      407 2022-09-18 05:38:39.000000 har_toolkit-0.3.0/har_toolkit/har_objects/post_data.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      101 2022-09-18 05:39:04.000000 har_toolkit-0.3.0/har_toolkit/har_objects/query_string.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1170 2022-09-19 02:52:59.000000 har_toolkit-0.3.0/har_toolkit/har_objects/request.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      858 2023-04-08 19:16:42.000000 har_toolkit-0.3.0/har_toolkit/har_objects/response.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      415 2022-09-18 05:40:34.000000 har_toolkit-0.3.0/har_toolkit/har_objects/timings.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/har_toolkit/media/
+-rw-r--r--   0 mason     (1000) mason     (1000)      840 2023-04-08 20:46:52.000000 har_toolkit-0.3.0/har_toolkit/media/image.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2869 2023-04-08 20:46:51.000000 har_toolkit-0.3.0/har_toolkit/parser.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      357 2022-09-22 03:48:27.000000 har_toolkit-0.3.0/har_toolkit/utils.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/har_toolkit.egg-info/
+-rw-r--r--   0 mason     (1000) mason     (1000)     1199 2023-04-08 20:54:54.000000 har_toolkit-0.3.0/har_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)      978 2023-04-08 20:54:54.000000 har_toolkit-0.3.0/har_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)        1 2023-04-08 20:54:54.000000 har_toolkit-0.3.0/har_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)       12 2023-04-08 20:54:54.000000 har_toolkit-0.3.0/har_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)      666 2023-04-08 20:54:41.000000 har_toolkit-0.3.0/pyproject.toml
+-rw-r--r--   0 mason     (1000) mason     (1000)       38 2023-04-08 20:54:54.295357 har_toolkit-0.3.0/setup.cfg
```

### Comparing `har_toolkit-0.2.0/LICENSE` & `har_toolkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `har_toolkit-0.2.0/PKG-INFO` & `har_toolkit-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har_toolkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: A module to work with HAR (HTTP Archive) files.
 Author-email: Mason Weaver <mason@swingproxy.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Otach/Har-Toolkit.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -29,11 +29,11 @@
 ```
 
 To read and parse a HAR file:
 ```
 import har_toolkit
 har = har_toolkit.read_har_file("<path/to/har_file>")
 ```
-This will return a HarReader object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
+This will return a Har object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
 
 The different sections of the format can be accessed by calling that section attribute on the parent class. Example: `har.browser` or `har.entries`
```

### Comparing `har_toolkit-0.2.0/README.md` & `har_toolkit-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 ```
 
 To read and parse a HAR file:
 ```
 import har_toolkit
 har = har_toolkit.read_har_file("<path/to/har_file>")
 ```
-This will return a HarReader object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
+This will return a Har object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
 
 The different sections of the format can be accessed by calling that section attribute on the parent class. Example: `har.browser` or `har.entries`
```

### Comparing `har_toolkit-0.2.0/pyproject.toml` & `har_toolkit-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "har_toolkit"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     { name="Mason Weaver", email="mason@swingproxy.com" },
 ]
 description = "A module to work with HAR (HTTP Archive) files."
 readme = "README.md"
 license = { text="GNU General Public License v3 (GPLv3)" }
 requires-python = ">=3.6"
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/bases.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/bases.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,7 +30,10 @@
     def __init__(self, data):
         super().__init__(data)
         self.name = data["name"]
         self.value = data["value"]
 
     def __str__(self):
         return f"{type(self).__name__}\n\t{self.name=}\n\t{self.value=}\n\t{self.comment=}"
+
+    def __repr__(self):
+        return f"{type(self).__name__}\n\t{self.name=}\n\t{self.value=}\n\t{self.comment=}"
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/content.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/content.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,21 +11,34 @@
         self.compression = data.get("compression")
         self.mimeType = data.get("mimeType")
         self.text = data.get("text")
         self.encoding = data.get("encoding")
         self.charset = self._extract_charset()
 
     def _extract_charset(self):
-        if "; charset=" in self.mimeType:
+        if self.mimeType is not None and "; charset=" in self.mimeType:
             return self.mimeType.split("=")[-1]
         else:
             return None
 
     def decode(self):
         if self.encoding == "base64":
             self.text = b64decode(self.text)
 
         # Convert the text to utf8 bytes
         if isinstance(self.text, str):
             self.text = self.text.encode('utf8')
 
         return self
+
+    def __str__(self):
+        return str(dict(
+            size=self.size,
+            compression=self.compression,
+            mimeType=self.mimeType,
+            encoding=self.encoding,
+            charset=self.charset
+        ))
+
+    def __repr__(self):
+        return str(self)
+
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/entry.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,10 @@
         self.time = data["time"]
         self.request = Request(data["request"])
         self.response = Response(data["response"])
         self.cache = Cache(data["cache"]) if data["cache"] != {} else None
         self.timings = Timings(data["timings"]) if data["timings"] != {} else None
         self.serverIPAddress = data.get("serverIPAddress")
         self.connection = data.get("connection")
+
+    def __str__(self):
+        return str(vars(self))
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/page.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/page.py`

 * *Files identical despite different names*

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/request.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/request.py`

 * *Files identical despite different names*

### Comparing `har_toolkit-0.2.0/src/har_toolkit/har_objects/response.py` & `har_toolkit-0.3.0/har_toolkit/har_objects/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,10 @@
         self.headers = []
         for header in data["headers"]:
             self.headers.append(Header(header))
         self.content = Content(data["content"]) if data["content"] != {} else None
         self.redirectURL = data["redirectURL"]
         self.headersSize = data.get("headersSize", -1)
         self.bodySize = data["bodySize"]
+
+    def __str__(self):
+        return str(vars(self))
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit.egg-info/PKG-INFO` & `har_toolkit-0.3.0/har_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har-toolkit
-Version: 0.2.0
+Version: 0.3.0
 Summary: A module to work with HAR (HTTP Archive) files.
 Author-email: Mason Weaver <mason@swingproxy.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Otach/Har-Toolkit.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -29,11 +29,11 @@
 ```
 
 To read and parse a HAR file:
 ```
 import har_toolkit
 har = har_toolkit.read_har_file("<path/to/har_file>")
 ```
-This will return a HarReader object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
+This will return a Har object with the contents of the file parsed according to [this W3C document](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
 
 The different sections of the format can be accessed by calling that section attribute on the parent class. Example: `har.browser` or `har.entries`
```

### Comparing `har_toolkit-0.2.0/src/har_toolkit.egg-info/SOURCES.txt` & `har_toolkit-0.3.0/har_toolkit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
-src/har_toolkit/__init__.py
-src/har_toolkit/parser.py
-src/har_toolkit/utils.py
-src/har_toolkit.egg-info/PKG-INFO
-src/har_toolkit.egg-info/SOURCES.txt
-src/har_toolkit.egg-info/dependency_links.txt
-src/har_toolkit.egg-info/top_level.txt
-src/har_toolkit/har_objects/__init__.py
-src/har_toolkit/har_objects/bases.py
-src/har_toolkit/har_objects/browser.py
-src/har_toolkit/har_objects/cache.py
-src/har_toolkit/har_objects/cache_state.py
-src/har_toolkit/har_objects/content.py
-src/har_toolkit/har_objects/cookie.py
-src/har_toolkit/har_objects/creator.py
-src/har_toolkit/har_objects/entry.py
-src/har_toolkit/har_objects/exceptions.py
-src/har_toolkit/har_objects/header.py
-src/har_toolkit/har_objects/page.py
-src/har_toolkit/har_objects/page_timings.py
-src/har_toolkit/har_objects/params.py
-src/har_toolkit/har_objects/post_data.py
-src/har_toolkit/har_objects/query_string.py
-src/har_toolkit/har_objects/request.py
-src/har_toolkit/har_objects/response.py
-src/har_toolkit/har_objects/timings.py
+har_toolkit/__init__.py
+har_toolkit/parser.py
+har_toolkit/utils.py
+har_toolkit.egg-info/PKG-INFO
+har_toolkit.egg-info/SOURCES.txt
+har_toolkit.egg-info/dependency_links.txt
+har_toolkit.egg-info/top_level.txt
+har_toolkit/har_browser/harbrowser.py
+har_toolkit/har_objects/__init__.py
+har_toolkit/har_objects/bases.py
+har_toolkit/har_objects/browser.py
+har_toolkit/har_objects/cache.py
+har_toolkit/har_objects/cache_state.py
+har_toolkit/har_objects/content.py
+har_toolkit/har_objects/cookie.py
+har_toolkit/har_objects/creator.py
+har_toolkit/har_objects/entry.py
+har_toolkit/har_objects/exceptions.py
+har_toolkit/har_objects/header.py
+har_toolkit/har_objects/page.py
+har_toolkit/har_objects/page_timings.py
+har_toolkit/har_objects/params.py
+har_toolkit/har_objects/post_data.py
+har_toolkit/har_objects/query_string.py
+har_toolkit/har_objects/request.py
+har_toolkit/har_objects/response.py
+har_toolkit/har_objects/timings.py
+har_toolkit/media/image.py
```

