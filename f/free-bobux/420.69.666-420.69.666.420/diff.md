# Comparing `tmp/free-bobux-420.69.666.tar.gz` & `tmp/free-bobux-420.69.666.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free-bobux-420.69.666.tar", last modified: Sat Apr  8 16:46:27 2023, max compression
+gzip compressed data, was "free-bobux-420.69.666.420.tar", last modified: Sat Apr  8 16:59:54 2023, max compression
```

## Comparing `free-bobux-420.69.666.tar` & `free-bobux-420.69.666.420.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:46:27.302482 free-bobux-420.69.666/
--rw-r--r--   0 adam      (1003) adam      (1003)      250 2023-04-08 16:46:27.302482 free-bobux-420.69.666/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     1908 2023-04-06 16:18:02.000000 free-bobux-420.69.666/README.md
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:46:27.302482 free-bobux-420.69.666/free_bobux.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)      250 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      262 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       48 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        9 2023-04-08 16:46:27.000000 free-bobux-420.69.666/free_bobux.egg-info/top_level.txt
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:46:27.302482 free-bobux-420.69.666/rickroll/
--rw-r--r--   0 adam      (1003) adam      (1003)       33 2023-04-06 16:25:00.000000 free-bobux-420.69.666/rickroll/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      268 2023-04-06 16:28:01.000000 free-bobux-420.69.666/rickroll/rick.py
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:46:27.302482 free-bobux-420.69.666/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)      968 2023-04-08 16:46:11.000000 free-bobux-420.69.666/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:59:54.366689 free-bobux-420.69.666.420/
+-rw-r--r--   0 adam      (1003) adam      (1003)      254 2023-04-08 16:59:54.366689 free-bobux-420.69.666.420/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     1908 2023-04-06 16:18:02.000000 free-bobux-420.69.666.420/README.md
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:59:54.366689 free-bobux-420.69.666.420/free_bobux.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)      254 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      262 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       48 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        9 2023-04-08 16:59:54.000000 free-bobux-420.69.666.420/free_bobux.egg-info/top_level.txt
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:59:54.366689 free-bobux-420.69.666.420/rickroll/
+-rw-r--r--   0 adam      (1003) adam      (1003)       33 2023-04-06 16:25:00.000000 free-bobux-420.69.666.420/rickroll/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      268 2023-04-06 16:28:01.000000 free-bobux-420.69.666.420/rickroll/rick.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:59:54.366689 free-bobux-420.69.666.420/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     1172 2023-04-08 16:50:44.000000 free-bobux-420.69.666.420/setup.py
```

### Comparing `free-bobux-420.69.666/README.md` & `free-bobux-420.69.666.420/README.md`

 * *Files identical despite different names*

