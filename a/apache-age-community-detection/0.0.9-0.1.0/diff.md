# Comparing `tmp/apache-age-community-detection-0.0.9.tar.gz` & `tmp/apache-age-community-detection-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-age-community-detection-0.0.9.tar", last modified: Sat Apr  8 16:01:34 2023, max compression
+gzip compressed data, was "apache-age-community-detection-0.1.0.tar", last modified: Sat Apr  8 16:45:45 2023, max compression
```

## Comparing `apache-age-community-detection-0.0.9.tar` & `apache-age-community-detection-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:01:34.148661 apache-age-community-detection-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:01:34.148661 apache-age-community-detection-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:01:34.148661 apache-age-community-detection-0.0.9/age_community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/age_community_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:01:34.148661 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:01:34.000000 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-08 16:01:34.000000 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:01:34.000000 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 16:01:34.000000 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 16:01:34.000000 apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:01:34.152662 apache-age-community-detection-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 16:01:25.000000 apache-age-community-detection-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/age_community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/age_community_detection/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/lib/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/setup.py
```

### Comparing `apache-age-community-detection-0.0.9/LICENSE` & `apache-age-community-detection-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.0.9/PKG-INFO` & `apache-age-community-detection-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.0.9
+Version: 0.1.0
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.0.9/README.md` & `apache-age-community-detection-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.0.9/age_community_detection/Check.py` & `apache-age-community-detection-0.1.0/age_community_detection/Check.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.0.9/age_community_detection/Exception.py` & `apache-age-community-detection-0.1.0/age_community_detection/Exception.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.0.9/age_community_detection/Graph.py` & `apache-age-community-detection-0.1.0/age_community_detection/Graph.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.0.9/age_community_detection/Lib.py` & `apache-age-community-detection-0.1.0/age_community_detection/Lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import ctypes
 import os
 
 absolute_path = os.path.dirname(__file__)
-absolute_path += "lib/library.so"
+absolute_path += "/lib/library.so"
 
 # # Load the shared library
 lib = ctypes.CDLL(absolute_path)
 
 def get_community(nodes, edges):
     # Create a 2D NumPy array
     a = np.array(edges, dtype=np.int32)
```

### Comparing `apache-age-community-detection-0.0.9/apache_age_community_detection.egg-info/PKG-INFO` & `apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.0.9
+Version: 0.1.0
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.0.9/setup.py` & `apache-age-community-detection-0.1.0/setup.py`

 * *Files identical despite different names*

