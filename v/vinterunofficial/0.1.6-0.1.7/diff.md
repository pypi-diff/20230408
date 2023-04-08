# Comparing `tmp/vinterunofficial-0.1.6.tar.gz` & `tmp/vinterunofficial-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinterunofficial-0.1.6.tar", last modified: Thu Mar 30 13:04:03 2023, max compression
+gzip compressed data, was "vinterunofficial-0.1.7.tar", last modified: Sat Apr  8 20:46:58 2023, max compression
```

## Comparing `vinterunofficial-0.1.6.tar` & `vinterunofficial-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:04:03.895061 vinterunofficial-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-30 13:04:03.895061 vinterunofficial-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 13:04:03.895061 vinterunofficial-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:04:03.891061 vinterunofficial-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/tests/test_async_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/tests/test_vinter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/tests/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:04:03.891061 vinterunofficial-0.1.6/vinterunofficial/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/vinter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/vinter_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/vinter_sdk_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-30 13:03:41.000000 vinterunofficial-0.1.6/vinterunofficial/vinter_sdk_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:04:03.895061 vinterunofficial-0.1.6/vinterunofficial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-30 13:04:03.000000 vinterunofficial-0.1.6/vinterunofficial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-30 13:04:03.000000 vinterunofficial-0.1.6/vinterunofficial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:04:03.000000 vinterunofficial-0.1.6/vinterunofficial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 13:04:03.000000 vinterunofficial-0.1.6/vinterunofficial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 13:04:03.000000 vinterunofficial-0.1.6/vinterunofficial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.393491 vinterunofficial-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_async_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_vinter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/vinterunofficial/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/vinterunofficial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/top_level.txt
```

### Comparing `vinterunofficial-0.1.6/PKG-INFO` & `vinterunofficial-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinterunofficial
-Version: 0.1.6
+Version: 0.1.7
 Project-URL: homepage, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: documentation, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: repository, https://github.com/rahulmistri1997/vinterunofficial-pypi
 Description-Content-Type: text/markdown
 
 # Unofficial Wrapper for the Vinter API
 ![Code Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen.svg)
@@ -238,15 +238,15 @@
 
 def on_open(ws):
     print("### open ###")
 
 vinter_ws = VinterAPIWS(
     symbol="btc-usd-p-r",
     token="<APIKey>",
-    asset_type="singleassets",
+    asset_type="single_assets",
     on_message=on_message,
     on_error=on_error,
     on_close=on_close,
     on_open=on_open,
 )
 vinter_ws.open()
```

### Comparing `vinterunofficial-0.1.6/README.md` & `vinterunofficial-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -230,16 +230,16 @@
 
 def on_open(ws):
     print("### open ###")
 
 vinter_ws = VinterAPIWS(
     symbol="btc-usd-p-r",
     token="<APIKey>",
-    asset_type="singleassets",
+    asset_type="single_assets",
     on_message=on_message,
     on_error=on_error,
     on_close=on_close,
     on_open=on_open,
 )
 vinter_ws.open()
 
-```
+```
```

### Comparing `vinterunofficial-0.1.6/pyproject.toml` & `vinterunofficial-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=38.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vinterunofficial"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = ["httpx==0.23.3", "websocket-client==1.5.1"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [metadata]
```

### Comparing `vinterunofficial-0.1.6/tests/test_api.py` & `vinterunofficial-0.1.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/tests/test_async_api.py` & `vinterunofficial-0.1.7/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/tests/test_vinter_utils.py` & `vinterunofficial-0.1.7/tests/test_vinter_utils.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/tests/test_ws.py` & `vinterunofficial-0.1.7/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/config.py` & `vinterunofficial-0.1.7/vinterunofficial/config.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/utils.py` & `vinterunofficial-0.1.7/vinterunofficial/utils.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/vinter_abc.py` & `vinterunofficial-0.1.7/vinterunofficial/vinter_abc.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/vinter_sdk.py` & `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/vinter_sdk_async.py` & `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_async.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial/vinter_sdk_ws.py` & `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_ws.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.6/vinterunofficial.egg-info/PKG-INFO` & `vinterunofficial-0.1.7/vinterunofficial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinterunofficial
-Version: 0.1.6
+Version: 0.1.7
 Project-URL: homepage, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: documentation, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: repository, https://github.com/rahulmistri1997/vinterunofficial-pypi
 Description-Content-Type: text/markdown
 
 # Unofficial Wrapper for the Vinter API
 ![Code Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen.svg)
@@ -238,15 +238,15 @@
 
 def on_open(ws):
     print("### open ###")
 
 vinter_ws = VinterAPIWS(
     symbol="btc-usd-p-r",
     token="<APIKey>",
-    asset_type="singleassets",
+    asset_type="single_assets",
     on_message=on_message,
     on_error=on_error,
     on_close=on_close,
     on_open=on_open,
 )
 vinter_ws.open()
```

### Comparing `vinterunofficial-0.1.6/vinterunofficial.egg-info/SOURCES.txt` & `vinterunofficial-0.1.7/vinterunofficial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

