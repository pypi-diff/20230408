# Comparing `tmp/acr122u-websocket-1.0.0.tar.gz` & `tmp/acr122u-websocket-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acr122u-websocket-1.0.0.tar", last modified: Sat Apr  8 19:08:50 2023, max compression
+gzip compressed data, was "acr122u-websocket-1.0.1.tar", last modified: Sat Apr  8 19:21:48 2023, max compression
```

## Comparing `acr122u-websocket-1.0.0.tar` & `acr122u-websocket-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:08:50.917678 acr122u-websocket-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-08 19:08:50.917678 acr122u-websocket-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:08:50.913678 acr122u-websocket-1.0.0/acr122u_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/acr122u_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/acr122u_websocket/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/acr122u_websocket/my_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/acr122u_websocket/reader_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:08:50.917678 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-08 19:08:50.000000 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-08 19:08:50.000000 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:08:50.000000 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 19:08:50.000000 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 19:08:50.000000 acr122u-websocket-1.0.0/acr122u_websocket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-08 19:08:38.000000 acr122u-websocket-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:08:50.917678 acr122u-websocket-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/acr122u_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/my_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/reader_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/setup.cfg
```

### Comparing `acr122u-websocket-1.0.0/LICENSE` & `acr122u-websocket-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.0.0/PKG-INFO` & `acr122u-websocket-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acr122u-websocket
-Version: 1.0.0
+Version: 1.0.1
 Summary: A webserver that connects to a acr122u and exposes it over websocket
 Author-email: Robert van Dijk <contact@robertvandijk.nl>
 Project-URL: Homepage, https://github.com/robertdijk/acr122u-websocket
 Keywords: nfc,acr,acr122u,websocket,web
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,7 +40,9 @@
 ## Usage
 
 1. Connect the ACR122U reader to the computer
 2. Run the app
     ```shell
     python -m acr122u_websocket.app
     ```
+
+## API
```

### Comparing `acr122u-websocket-1.0.0/README.md` & `acr122u-websocket-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 
 ## Usage
 
 1. Connect the ACR122U reader to the computer
 2. Run the app
     ```shell
     python -m acr122u_websocket.app
-    ```
+    ```
+
+## API
```

### Comparing `acr122u-websocket-1.0.0/acr122u_websocket/app.py` & `acr122u-websocket-1.0.1/acr122u_websocket/app.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.0.0/acr122u_websocket/my_reader.py` & `acr122u-websocket-1.0.1/acr122u_websocket/my_reader.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.0.0/acr122u_websocket/reader_helpers.py` & `acr122u-websocket-1.0.1/acr122u_websocket/reader_helpers.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.0.0/acr122u_websocket.egg-info/PKG-INFO` & `acr122u-websocket-1.0.1/acr122u_websocket.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acr122u-websocket
-Version: 1.0.0
+Version: 1.0.1
 Summary: A webserver that connects to a acr122u and exposes it over websocket
 Author-email: Robert van Dijk <contact@robertvandijk.nl>
 Project-URL: Homepage, https://github.com/robertdijk/acr122u-websocket
 Keywords: nfc,acr,acr122u,websocket,web
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,7 +40,9 @@
 ## Usage
 
 1. Connect the ACR122U reader to the computer
 2. Run the app
     ```shell
     python -m acr122u_websocket.app
     ```
+
+## API
```

### Comparing `acr122u-websocket-1.0.0/pyproject.toml` & `acr122u-websocket-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acr122u-websocket"
-version = "1.0.0"
+version = "1.0.1"
 description = "A webserver that connects to a acr122u and exposes it over websocket"
 readme = "README.md"
 authors = [{ name = "Robert van Dijk", email = "contact@robertvandijk.nl" }]
 license = { file = "pb" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
     "bumpver",
 ]
 
 [project.urls]
 Homepage = "https://github.com/robertdijk/acr122u-websocket"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

