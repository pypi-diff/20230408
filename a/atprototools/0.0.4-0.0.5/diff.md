# Comparing `tmp/atprototools-0.0.4.tar.gz` & `tmp/atprototools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.4.tar", last modified: Sat Apr  8 20:40:52 2023, max compression
+gzip compressed data, was "atprototools-0.0.5.tar", last modified: Sat Apr  8 20:43:40 2023, max compression
```

## Comparing `atprototools-0.0.4.tar` & `atprototools-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:40:52.728567 atprototools-0.0.4/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:40:52.728567 atprototools-0.0.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:40:52.728567 atprototools-0.0.4/atprototools/
--rw-r--r--   0 user      (1000) user      (1000)       62 2023-04-08 20:40:32.000000 atprototools-0.0.4/atprototools/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1274 2023-04-08 18:50:48.000000 atprototools-0.0.4/atprototools/main.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:40:52.728567 atprototools-0.0.4/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:40:52.000000 atprototools-0.0.4/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      243 2023-04-08 20:40:52.000000 atprototools-0.0.4/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 20:40:52.000000 atprototools-0.0.4/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 20:40:52.000000 atprototools-0.0.4/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-08 20:40:52.000000 atprototools-0.0.4/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 20:40:52.728567 atprototools-0.0.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 20:40:47.000000 atprototools-0.0.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:43:40.478540 atprototools-0.0.5/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/atprototools/
+-rw-r--r--   0 user      (1000) user      (1000)     1274 2023-04-08 18:50:48.000000 atprototools-0.0.5/atprototools/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 20:43:40.478540 atprototools-0.0.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 20:43:23.000000 atprototools-0.0.5/setup.py
```

### Comparing `atprototools-0.0.4/PKG-INFO` & `atprototools-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.4
+Version: 0.0.5
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.4/atprototools/main.py` & `atprototools-0.0.5/atprototools/__init__.py`

 * *Files identical despite different names*

### Comparing `atprototools-0.0.4/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.5/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.4
+Version: 0.0.5
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.4/setup.py` & `atprototools-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.4',
+    version='0.0.5',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```

