# Comparing `tmp/atprototools-0.0.1.tar.gz` & `tmp/atprototools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.1.tar", last modified: Sat Apr  8 19:50:19 2023, max compression
+gzip compressed data, was "atprototools-0.0.2.tar", last modified: Sat Apr  8 20:26:16 2023, max compression
```

## Comparing `atprototools-0.0.1.tar` & `atprototools-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 19:50:19.739061 atprototools-0.0.1/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 19:50:19.739061 atprototools-0.0.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 18:50:48.000000 atprototools-0.0.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 19:50:19.739061 atprototools-0.0.1/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 19:50:19.000000 atprototools-0.0.1/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      197 2023-04-08 19:50:19.000000 atprototools-0.0.1/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 19:50:19.000000 atprototools-0.0.1/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 19:50:19.000000 atprototools-0.0.1/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 19:50:19.000000 atprototools-0.0.1/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 19:50:19.739061 atprototools-0.0.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 19:49:42.000000 atprototools-0.0.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:26:16.628705 atprototools-0.0.2/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:26:16.618705 atprototools-0.0.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:26:16.618705 atprototools-0.0.2/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:26:16.000000 atprototools-0.0.2/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      197 2023-04-08 20:26:16.000000 atprototools-0.0.2/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 20:26:16.000000 atprototools-0.0.2/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 20:26:16.000000 atprototools-0.0.2/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 20:26:16.000000 atprototools-0.0.2/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 20:26:16.628705 atprototools-0.0.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 20:25:26.000000 atprototools-0.0.2/setup.py
```

### Comparing `atprototools-0.0.1/PKG-INFO` & `atprototools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.1
+Version: 0.0.2
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.1/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.2/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.1
+Version: 0.0.2
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.1/setup.py` & `atprototools-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.1',
+    version='0.0.2',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```

