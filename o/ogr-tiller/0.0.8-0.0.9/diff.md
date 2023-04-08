# Comparing `tmp/ogr_tiller-0.0.8.tar.gz` & `tmp/ogr_tiller-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogr_tiller-0.0.8.tar", last modified: Sun Mar 26 17:18:19 2023, max compression
+gzip compressed data, was "ogr_tiller-0.0.9.tar", last modified: Sun Mar 26 17:21:08 2023, max compression
```

## Comparing `ogr_tiller-0.0.8.tar` & `ogr_tiller-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:19.477563 ogr_tiller-0.0.8/ogr_tiller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/ogr_tiller/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/entities/job_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/ogr_tiller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/ogr_tiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/utils/fast_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/utils/ogr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/utils/sqlite_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/ogr_tiller/utils/tile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/ogr_tiller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-26 17:18:19.000000 ogr_tiller-0.0.8/ogr_tiller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-26 17:18:19.481563 ogr_tiller-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-26 17:18:08.000000 ogr_tiller-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:21:08.062029 ogr_tiller-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-26 17:21:08.062029 ogr_tiller-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:21:08.058029 ogr_tiller-0.0.9/ogr_tiller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:21:08.058029 ogr_tiller-0.0.9/ogr_tiller/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/entities/job_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/ogr_tiller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:21:08.062029 ogr_tiller-0.0.9/ogr_tiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/utils/fast_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/utils/ogr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/utils/sqlite_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/ogr_tiller/utils/tile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:21:08.058029 ogr_tiller-0.0.9/ogr_tiller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:21:07.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-26 17:21:08.000000 ogr_tiller-0.0.9/ogr_tiller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-26 17:21:08.062029 ogr_tiller-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-26 17:20:59.000000 ogr_tiller-0.0.9/setup.py
```

### Comparing `ogr_tiller-0.0.8/PKG-INFO` & `ogr_tiller-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogr_tiller
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates vector tiles on the fly from local geopackage files
 Home-page: https://github.com/geoyogesh/ogr_tiller
 Author: Yogesh Dhanapal
 Author-email: geoyogesh@gmail.com
 License: GNU-GPL
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ogr_tiller-0.0.8/ogr_tiller/main.py` & `ogr_tiller-0.0.9/ogr_tiller/main.py`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/ogr_tiller/ogr_tiller.py` & `ogr_tiller-0.0.9/ogr_tiller/ogr_tiller.py`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/ogr_tiller/utils/fast_api_utils.py` & `ogr_tiller-0.0.9/ogr_tiller/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/ogr_tiller/utils/ogr_utils.py` & `ogr_tiller-0.0.9/ogr_tiller/utils/ogr_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return result
 
 
 def setup_ogr_cache(data_folder):
     # update global variablea
     global data_location, tilesets
     data_location = data_folder
-    tilesets = get_tilesets(data_location)
+    tilesets = get_tilesets()
 
 
 def format_layer_name(name: str):
     return name.lower()
 
 
 def format_field_name(name: str):
```

### Comparing `ogr_tiller-0.0.8/ogr_tiller/utils/sqlite_utils.py` & `ogr_tiller-0.0.9/ogr_tiller/utils/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/ogr_tiller/utils/tile_utils.py` & `ogr_tiller-0.0.9/ogr_tiller/utils/tile_utils.py`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/ogr_tiller.egg-info/PKG-INFO` & `ogr_tiller-0.0.9/ogr_tiller.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogr-tiller
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates vector tiles on the fly from local geopackage files
 Home-page: https://github.com/geoyogesh/ogr_tiller
 Author: Yogesh Dhanapal
 Author-email: geoyogesh@gmail.com
 License: GNU-GPL
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ogr_tiller-0.0.8/ogr_tiller.egg-info/SOURCES.txt` & `ogr_tiller-0.0.9/ogr_tiller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogr_tiller-0.0.8/setup.py` & `ogr_tiller-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 setup(name='ogr_tiller',
-      version='0.0.8',
+      version='0.0.9',
       url='https://github.com/geoyogesh/ogr_tiller',
       license='GNU-GPL',
       author='Yogesh Dhanapal',
       author_email='geoyogesh@gmail.com',
       entry_points={"console_scripts": ["ogr_tiller = ogr_tiller.main:cli"]},
       description='Creates vector tiles on the fly from local geopackage files',
       packages=find_packages(),
```

