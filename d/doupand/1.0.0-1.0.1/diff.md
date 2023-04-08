# Comparing `tmp/doupand-1.0.0.tar.gz` & `tmp/doupand-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/doupand-1.0.0.tar", last modified: Fri Apr  7 19:18:13 2023, max compression
+gzip compressed data, was "dist/doupand-1.0.1.tar", last modified: Sat Apr  8 17:46:46 2023, max compression
```

## Comparing `doupand-1.0.0.tar` & `doupand-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-07 19:18:13.000000 doupand-1.0.0/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-07 19:18:13.000000 doupand-1.0.0/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.0/LICENSE
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-07 14:44:45.000000 doupand-1.0.0/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.0/doupand/utils/userauth.py
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.0/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      232 2023-04-07 14:52:04.000000 doupand-1.0.0/doupand/utils/cons.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)     1839 2023-04-07 19:12:44.000000 doupand-1.0.0/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.0/doupand/api/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-07 19:18:13.000000 doupand-1.0.0/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)     2427 2023-04-07 19:13:54.000000 doupand-1.0.0/setup.py
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-07 19:18:13.000000 doupand-1.0.0/setup.cfg
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-08 17:46:46.000000 doupand-1.0.1/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.1/LICENSE
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.1/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.1/doupand/utils/userauth.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.1/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.1/doupand/utils/cons.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)     3182 2023-04-08 17:45:25.000000 doupand-1.0.1/doupand/api/client.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.1/doupand/api/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)     2427 2023-04-07 19:13:54.000000 doupand-1.0.1/setup.py
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-08 17:46:46.000000 doupand-1.0.1/setup.cfg
```

### Comparing `doupand-1.0.0/PKG-INFO` & `doupand-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.0/LICENSE` & `doupand-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.0/doupand/utils/userauth.py` & `doupand-1.0.1/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.0/doupand.egg-info/PKG-INFO` & `doupand-1.0.1/doupand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.0/setup.py` & `doupand-1.0.1/setup.py`

 * *Files identical despite different names*

