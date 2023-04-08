# Comparing `tmp/dependatool-0.2.0.tar.gz` & `tmp/dependatool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dependatool-0.2.0.tar", last modified: Sat Apr  8 09:40:08 2023, max compression
+gzip compressed data, was "dependatool-0.2.1.tar", last modified: Sat Apr  8 17:01:31 2023, max compression
```

## Comparing `dependatool-0.2.0.tar` & `dependatool-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:40:08.004696 dependatool-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 09:40:07.000000 dependatool-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 09:40:08.004696 dependatool-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-08 09:40:07.000000 dependatool-0.2.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:40:08.004696 dependatool-0.2.0/dependatool/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:40:08.004696 dependatool-0.2.0/dependatool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-08 09:40:08.000000 dependatool-0.2.0/dependatool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 09:40:07.000000 dependatool-0.2.0/dependatool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 09:40:08.004696 dependatool-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-08 09:40:07.000000 dependatool-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.823561 dependatool-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 17:01:31.000000 dependatool-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 17:01:31.823561 dependatool-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-08 17:01:31.000000 dependatool-0.2.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.819561 dependatool-0.2.1/dependatool/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.819561 dependatool-0.2.1/dependatool/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/abstract/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.819561 dependatool-0.2.1/dependatool/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/docker/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/docker/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.819561 dependatool-0.2.1/dependatool/gomod/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/gomod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/gomod/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/gomod/check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.823561 dependatool-0.2.1/dependatool/pip/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/pip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/pip/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/pip/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:01:31.819561 dependatool-0.2.1/dependatool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 17:01:31.000000 dependatool-0.2.1/dependatool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 17:01:31.823561 dependatool-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-08 17:01:31.000000 dependatool-0.2.1/setup.py
```

### Comparing `dependatool-0.2.0/backend_shim.py` & `dependatool-0.2.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `dependatool-0.2.0/setup.py` & `dependatool-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,12 +33,16 @@
     'package_data': {
         'dependatool': (
             'py.typed',
         ),
     },
     'packages': (
         'dependatool',
+        'dependatool.abstract',
+        'dependatool.docker',
+        'dependatool.gomod',
+        'dependatool.pip',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/dependatool',
-    'version': '0.2.0',
+    'version': '0.2.1',
 })
```

