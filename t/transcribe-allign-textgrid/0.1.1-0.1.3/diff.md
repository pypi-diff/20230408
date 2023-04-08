# Comparing `tmp/transcribe_allign_textgrid-0.1.1.tar.gz` & `tmp/transcribe_allign_textgrid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe_allign_textgrid-0.1.1.tar", last modified: Mon Mar 27 20:37:49 2023, max compression
+gzip compressed data, was "transcribe_allign_textgrid-0.1.3.tar", last modified: Sat Apr  8 19:03:43 2023, max compression
```

## Comparing `transcribe_allign_textgrid-0.1.1.tar` & `transcribe_allign_textgrid-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-03-27 20:37:49.914716 transcribe_allign_textgrid-0.1.1/
--rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-27 13:19:36.000000 transcribe_allign_textgrid-0.1.1/LICENCE
--rw-r--r--   0 jjw       (1000) jjw       (1000)     6456 2023-03-27 20:37:49.914716 transcribe_allign_textgrid-0.1.1/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     5814 2023-03-27 20:20:22.000000 transcribe_allign_textgrid-0.1.1/README.md
--rw-r--r--   0 jjw       (1000) jjw       (1000)      926 2023-03-27 20:31:14.000000 transcribe_allign_textgrid-0.1.1/pyproject.toml
--rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-03-26 22:09:15.000000 transcribe_allign_textgrid-0.1.1/requirements.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-03-27 20:37:49.914716 transcribe_allign_textgrid-0.1.1/setup.cfg
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-03-27 20:37:49.912716 transcribe_allign_textgrid-0.1.1/src/
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-03-27 20:37:49.913716 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      380 2023-03-27 20:31:26.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)       79 2023-03-26 12:28:00.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/__main__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3461 2023-03-27 19:24:44.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/adapter.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3824 2023-03-27 20:29:37.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/cli.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1994 2023-03-27 18:59:40.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/whisper_schema.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-03-27 20:37:49.914716 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     6456 2023-03-27 20:37:49.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)      576 2023-03-27 20:37:49.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/SOURCES.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-03-27 20:37:49.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/dependency_links.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-03-27 20:37:49.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/requires.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       27 2023-03-27 20:37:49.000000 transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/top_level.txt
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-03-27 20:37:49.914716 transcribe_allign_textgrid-0.1.1/tests/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      795 2023-03-27 18:58:28.000000 transcribe_allign_textgrid-0.1.1/tests/test_adapter.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      225 2023-03-27 15:09:04.000000 transcribe_allign_textgrid-0.1.1/tests/test_schema.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/LICENCE
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6587 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     5814 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/README.md
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1047 2023-04-08 19:02:07.000000 transcribe_allign_textgrid-0.1.3/pyproject.toml
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/requirements.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/setup.cfg
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.456562 transcribe_allign_textgrid-0.1.3/src/
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.457562 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1001 2023-04-08 19:02:26.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       79 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/__main__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3315 2023-04-08 18:57:03.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/adapter.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3846 2023-04-08 18:58:22.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/cli.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1994 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/whisper_schema.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6587 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      576 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/requires.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       27 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/top_level.txt
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/tests/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      795 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/tests/test_adapter.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      225 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/tests/test_schema.py
```

### Comparing `transcribe_allign_textgrid-0.1.1/LICENCE` & `transcribe_allign_textgrid-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.1/PKG-INFO` & `transcribe_allign_textgrid-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: transcribe_allign_textgrid
-Version: 0.1.1
+Version: 0.1.3
 Summary: Create for-alligned transcription TextGrids from Audio
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/transcribe_allign_textgrid
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/transcribe_allign_textgrid/issues
 Keywords: praat,whisper,force-allign,TextGrid
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Transcribe Allign TextGrid
```

### Comparing `transcribe_allign_textgrid-0.1.1/README.md` & `transcribe_allign_textgrid-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.1/pyproject.toml` & `transcribe_allign_textgrid-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "transcribe_allign_textgrid"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="JJWRoeloffs", email="jelleroeloffs@gmail.com" },
 ]
 description = "Create for-alligned transcription TextGrids from Audio"
 keywords = ["praat", "whisper", "force-allign", "TextGrid"]
 readme = "README.md"
 requires-python = ">=3.7, <3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/adapter.py` & `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def fill_if_empty(entries: List[Interval]) -> List[Interval]:
     return entries if entries else [Interval(start=0.0, end=0.1, label="")]
 
 
 class WhisperWord:
-    def __init__(self, whisper_word) -> None:
+    def __init__(self, whisper_word: Dict) -> None:
         self.text = str(whisper_word["text"])
         self.start = float(whisper_word["start"])
         self.end = float(whisper_word["end"])
         self.confidence = float(whisper_word["confidence"])
 
     def to_text_interval(self) -> Interval:
         return Interval(start=self.start, end=self.end, label=self.text)
@@ -40,19 +40,14 @@
 
     def to_confidence_interval(self) -> Interval:
         return Interval(start=self.start, end=self.end, label=str(self.confidence))
 
 
 class WhisperObject:
     def __init__(self, wt_output: Dict) -> None:
-        try:
-            self.language = str(wt_output["language"])
-        except TypeError:
-            print(wt_output)
-            raise ValueError
         self.text = str(wt_output["text"])
         self.segments = [WhisperSegment(x) for x in wt_output["segments"]]
 
     def to_segment_text_tier(self) -> IntervalTier:
         entries = [x.to_text_interval() for x in self.segments]
         return IntervalTier("segments_text", fill_if_empty(entries))
```

### Comparing `transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/cli.py` & `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class Args:
     paths: List[Path]
     model: str
     language: Optional[str]
 
 
 def get_files(path: Path) -> List[Path]:
-    return [path] if path.is_file() else list(path.iterdir())
+    return [path] if path.is_file() else [x for x in path.iterdir() if x.is_file()]
 
 
 def parse_args(args: List[str]) -> Args:
     parser = argparse.ArgumentParser(
         prog="transcribe_allign_textgrid",
         description="""
             A small wrapper cli around whisper-timestamped.
```

### Comparing `transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid/whisper_schema.py` & `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/whisper_schema.py`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/PKG-INFO` & `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: transcribe-allign-textgrid
-Version: 0.1.1
+Version: 0.1.3
 Summary: Create for-alligned transcription TextGrids from Audio
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/transcribe_allign_textgrid
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/transcribe_allign_textgrid/issues
 Keywords: praat,whisper,force-allign,TextGrid
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Transcribe Allign TextGrid
```

### Comparing `transcribe_allign_textgrid-0.1.1/src/transcribe_allign_textgrid.egg-info/SOURCES.txt` & `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.1/tests/test_adapter.py` & `transcribe_allign_textgrid-0.1.3/tests/test_adapter.py`

 * *Files identical despite different names*

