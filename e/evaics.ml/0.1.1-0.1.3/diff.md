# Comparing `tmp/evaics.ml-0.1.1.tar.gz` & `tmp/evaics.ml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics.ml-0.1.1.tar", last modified: Tue Apr  4 20:54:03 2023, max compression
+gzip compressed data, was "evaics.ml-0.1.3.tar", last modified: Sat Apr  8 21:46:35 2023, max compression
```

## Comparing `evaics.ml-0.1.1.tar` & `evaics.ml-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/
--rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.1/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      693 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      118 2023-03-29 17:24:22.000000 evaics.ml-0.1.1/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/evaics/
--rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-04 20:53:59.000000 evaics.ml-0.1.1/evaics/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/evaics/ml/
--rw-r--r--   0 divisor   (1000) root         (0)    15989 2023-04-04 20:53:59.000000 evaics.ml-0.1.1/evaics/ml/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-04 20:53:59.000000 evaics.ml-0.1.1/evaics/ml/learning.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/evaics.ml.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      693 2023-04-04 20:54:03.000000 evaics.ml-0.1.1/evaics.ml.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-04 20:54:03.000000 evaics.ml-0.1.1/evaics.ml.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-04 20:54:03.000000 evaics.ml-0.1.1/evaics.ml.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-04 20:54:03.000000 evaics.ml-0.1.1/evaics.ml.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-04 20:54:03.000000 evaics.ml-0.1.1/evaics.ml.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-04 20:54:03.796081 evaics.ml-0.1.1/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-04 20:53:59.000000 evaics.ml-0.1.1/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/
+-rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.3/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      136 2023-04-08 21:45:24.000000 evaics.ml-0.1.3/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics/
+-rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics/ml/
+-rw-r--r--   0 divisor   (1000) root         (0)    15819 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/ml/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/evaics/ml/learning.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/evaics.ml.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-08 21:46:35.000000 evaics.ml-0.1.3/evaics.ml.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-08 21:46:35.173111 evaics.ml-0.1.3/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-08 21:46:28.000000 evaics.ml-0.1.3/setup.py
```

### Comparing `evaics.ml-0.1.1/LICENSE` & `evaics.ml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.1/evaics/ml/__init__.py` & `evaics.ml-0.1.3/evaics/ml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.1'
+__version__ = '0.1.3'
 
 import sys
 import requests
 import gzip
 import logging
 import time
 import json
@@ -34,24 +34,21 @@
     automatically added to evaics.client.HttpClient
     """
 
     def __init__(self, client, params_csv: str = None):
         """
         Create HistoryDF object instance
 
+        All configuration methods of the class can be used in chains.
+
         Args:
             client: HTTP client object
 
         Optional:
             params_csv: CSV file or stream to read parameters from
-
-        All configuration methods of the class can be used in chains, e.g.
-        HistoryDF(client).oid(
-            'sensor:s1', status=False, value='s1').oid(
-            'sensor:s2', status=False, value='s2').fill('1T').fetch()
         """
         self.client = client
         self.mlkit = None
         self.params = {'fill': '1S'}
         self.oid_map = []
         if params_csv is not None:
             self.read_params_csv(params_csv)
@@ -386,17 +383,17 @@
               strict_col_order=False):
         """
         Fetch data
 
         Optional:
             output: output format (arrow, pandas or polars)
             t_col: time column processing, "keep" - keep the column, "drop" -
-                drop the time column
+            drop the time column
             tz: time zone (local, custom or None to keep time column as UNIX
-                timestamp), the default is "local"
+            timestamp), the default is "local"
             strict_col_order: force strict column ordering
 
 
         Returns:
             a prepared Pandas DataFrame object
         """
         if t_col not in ['keep', 'drop']:
```

### Comparing `evaics.ml-0.1.1/evaics/ml/learning.py` & `evaics.ml-0.1.3/evaics/ml/learning.py`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.1/setup.py` & `evaics.ml-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.1'
+__version__ = '0.1.3'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

