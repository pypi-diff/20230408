# Comparing `tmp/bayanpy-0.4.tar.gz` & `tmp/bayanpy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.4.tar", last modified: Sat Apr  8 14:15:56 2023, max compression
+gzip compressed data, was "bayanpy-0.5.tar", last modified: Sat Apr  8 16:18:10 2023, max compression
```

## Comparing `bayanpy-0.4.tar` & `bayanpy-0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 14:15:56.753889 bayanpy-0.4/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.4/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 14:15:56.753889 bayanpy-0.4/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5061 2023-04-08 05:40:21.000000 bayanpy-0.4/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 14:15:56.753889 bayanpy-0.4/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       28 2023-04-08 06:28:10.000000 bayanpy-0.4/bayanpy/__init__.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    44347 2023-04-08 03:05:45.000000 bayanpy-0.4/bayanpy/bayanpy.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 14:15:56.753889 bayanpy-0.4/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 14:15:56.000000 bayanpy-0.4/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      219 2023-04-08 14:15:56.000000 bayanpy-0.4/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-08 14:15:56.000000 bayanpy-0.4/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       46 2023-04-08 14:15:56.000000 bayanpy-0.4/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-08 14:15:56.000000 bayanpy-0.4/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-08 14:15:56.753889 bayanpy-0.4/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      548 2023-04-08 14:09:07.000000 bayanpy-0.4/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.5/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 16:18:10.947248 bayanpy-0.5/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5077 2023-04-08 16:17:15.000000 bayanpy-0.5/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-08 16:13:17.000000 bayanpy-0.5/bayanpy/__init__.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52003 2023-04-08 16:14:58.000000 bayanpy-0.5/bayanpy/bayanimplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    44347 2023-04-08 03:05:45.000000 bayanpy-0.5/bayanpy/bayanpy.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      243 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-08 16:18:10.947248 bayanpy-0.5/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      559 2023-04-08 16:17:39.000000 bayanpy-0.5/setup.py
```

### Comparing `bayanpy-0.4/LICENSE` & `bayanpy-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.4/README.md` & `bayanpy-0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 - requests>=2.25.1
 - pandas>=1.3.0
 - networkx>=2.6.3
 - numpy>=1.21.0
 - gurobipy>=9.5
 - cdlib>=0.2.6
+- joblib>=1.1.0
 
 These packages will be automatically installed when you install Bayanpy using pip.
 
 
 
 ### Gurobi Installation with Free Academic License
```

### Comparing `bayanpy-0.4/bayanpy/bayanpy.py` & `bayanpy-0.5/bayanpy/bayanpy.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.4/setup.py` & `bayanpy-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.4", 
+    version="0.5", 
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
-        "cdlib"
+        "cdlib",
+	"joblib"
     ],
 )
```

