# Comparing `tmp/afplay-py-0.1.0.tar.gz` & `tmp/afplay-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afplay-py-0.1.0.tar", last modified: Sat Apr  8 16:16:12 2023, max compression
+gzip compressed data, was "afplay-py-0.2.0.tar", last modified: Sat Apr  8 18:17:25 2023, max compression
```

## Comparing `afplay-py-0.1.0.tar` & `afplay-py-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.622890 afplay-py-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.618890 afplay-py-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.618890 afplay-py-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-08 16:15:58.000000 afplay-py-0.1.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-08 16:15:58.000000 afplay-py-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-08 16:15:58.000000 afplay-py-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-08 16:15:58.000000 afplay-py-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 16:15:58.000000 afplay-py-0.1.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 16:15:58.000000 afplay-py-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-08 16:16:12.626891 afplay-py-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-08 16:15:58.000000 afplay-py-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.618890 afplay-py-0.1.0/afplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-08 16:15:58.000000 afplay-py-0.1.0/afplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:15:58.000000 afplay-py-0.1.0/afplay/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.622890 afplay-py-0.1.0/afplay_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 16:16:12.000000 afplay-py-0.1.0/afplay_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-08 16:15:58.000000 afplay-py-0.1.0/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 16:15:58.000000 afplay-py-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 16:16:12.626891 afplay-py-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-08 16:15:58.000000 afplay-py-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:16:12.622890 afplay-py-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:15:58.000000 afplay-py-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-08 16:15:58.000000 afplay-py-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)  2370476 2023-04-08 16:15:58.000000 afplay-py-0.1.0/tests/foo.wav
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-08 16:15:58.000000 afplay-py-0.1.0/tests/test_afplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.046641 afplay-py-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.042641 afplay-py-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.042641 afplay-py-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-08 18:17:08.000000 afplay-py-0.2.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-08 18:17:08.000000 afplay-py-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-08 18:17:08.000000 afplay-py-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-08 18:17:08.000000 afplay-py-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 18:17:08.000000 afplay-py-0.2.0/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 18:17:08.000000 afplay-py-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-08 18:17:25.046641 afplay-py-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-08 18:17:08.000000 afplay-py-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.042641 afplay-py-0.2.0/afplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-08 18:17:08.000000 afplay-py-0.2.0/afplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:08.000000 afplay-py-0.2.0/afplay/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.042641 afplay-py-0.2.0/afplay_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 18:17:24.000000 afplay-py-0.2.0/afplay_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-08 18:17:08.000000 afplay-py-0.2.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 18:17:08.000000 afplay-py-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 18:17:25.046641 afplay-py-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-08 18:17:08.000000 afplay-py-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:25.046641 afplay-py-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:17:08.000000 afplay-py-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-08 18:17:08.000000 afplay-py-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2370476 2023-04-08 18:17:08.000000 afplay-py-0.2.0/tests/foo.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-08 18:17:08.000000 afplay-py-0.2.0/tests/test_afplay.py
```

### Comparing `afplay-py-0.1.0/.github/workflows/lint.yaml` & `afplay-py-0.2.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/.github/workflows/publish.yaml` & `afplay-py-0.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/.github/workflows/test.yaml` & `afplay-py-0.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/.gitignore` & `afplay-py-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/LICENSE` & `afplay-py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/PKG-INFO` & `afplay-py-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afplay-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: A wrapper around macOS afplay
 Home-page: https://github.com/unparalleled-js/afplay-py
 Author: Juliya Smith <juliya@juliyasmith.com>
 Author-email: juliya@juliyasmith.com
 License: Apache-2.0
 Keywords: afplay,macos
 Platform: UNKNOWN
@@ -43,14 +43,24 @@
 
 ```shell
 pip install .
 ```
 
 ## Quick Usage
 
+Play an audio file:
+
 ```python
 from afplay import afplay
 
-afplay("path/to/file.mp3")
+afplay("path/to/file.mp3", volume=2, time=100, leaks=True)
+```
+
+Check if `afplay` is installed:
+
+```python
+from afplay import is_installed
+
+print(is_installed())
 ```
```

### Comparing `afplay-py-0.1.0/afplay_py.egg-info/PKG-INFO` & `afplay-py-0.2.0/afplay_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afplay-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: A wrapper around macOS afplay
 Home-page: https://github.com/unparalleled-js/afplay-py
 Author: Juliya Smith <juliya@juliyasmith.com>
 Author-email: juliya@juliyasmith.com
 License: Apache-2.0
 Keywords: afplay,macos
 Platform: UNKNOWN
@@ -43,14 +43,24 @@
 
 ```shell
 pip install .
 ```
 
 ## Quick Usage
 
+Play an audio file:
+
 ```python
 from afplay import afplay
 
-afplay("path/to/file.mp3")
+afplay("path/to/file.mp3", volume=2, time=100, leaks=True)
+```
+
+Check if `afplay` is installed:
+
+```python
+from afplay import is_installed
+
+print(is_installed())
 ```
```

### Comparing `afplay-py-0.1.0/afplay_py.egg-info/requires.txt` & `afplay-py-0.2.0/afplay_py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/setup.py` & `afplay-py-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `afplay-py-0.1.0/tests/conftest.py` & `afplay-py-0.2.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import subprocess
+import sys
 from pathlib import Path
 
 import pytest
 
 BASE_PATH = Path(__file__).parent
 
 
 @pytest.fixture(autouse=True)
 def mock_player(mocker, devnull):
     class MockPlayer:
         _run = mocker.patch("afplay.run")
         _popen = mocker.patch("afplay.Popen")
 
-        def assert_played(self, _file):
-            self._popen.assert_called_once_with(
-                ["afplay", str(_file)], stdout=devnull, stderr=devnull
-            )
+        def assert_played(self, _file, **kwargs):
+            cmd = ["afplay", str(_file)]
+            for key, val in kwargs.items():
+                opt_str = f"--{key}"
+                if key in ("leaks",):
+                    cmd.append(opt_str)  # is_flag
+                else:
+                    cmd.extend((opt_str, str(val)))
+
+            self._popen.assert_called_once_with(cmd, stdout=sys.stdout, stderr=sys.stderr)
+
+        def assert_checked(self):
+            self._run.assert_called_once_with(["afplay"], stdout=devnull, stderr=devnull)
 
     return MockPlayer()
 
 
 @pytest.fixture
 def audio_file_path():
     return BASE_PATH / "foo.wav"
```

### Comparing `afplay-py-0.1.0/tests/foo.wav` & `afplay-py-0.2.0/tests/foo.wav`

 * *Files identical despite different names*

