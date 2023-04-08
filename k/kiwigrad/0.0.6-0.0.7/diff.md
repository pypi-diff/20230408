# Comparing `tmp/kiwigrad-0.0.6.tar.gz` & `tmp/kiwigrad-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.0.6.tar", last modified: Sat Apr  8 16:32:15 2023, max compression
+gzip compressed data, was "kiwigrad-0.0.7.tar", last modified: Sat Apr  8 16:36:18 2023, max compression
```

## Comparing `kiwigrad-0.0.6.tar` & `kiwigrad-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:32:15.038666 kiwigrad-0.0.6/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.0.6/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.0.6/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-08 16:32:15.038319 kiwigrad-0.0.6/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.0.6/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:32:15.035762 kiwigrad-0.0.6/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      173 2023-04-08 16:31:35.000000 kiwigrad-0.0.6/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.0.6/kiwigrad/engine.pyx
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.0.6/kiwigrad/graph.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:32:15.037885 kiwigrad-0.0.6/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-08 16:32:15.000000 kiwigrad-0.0.6/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      262 2023-04-08 16:32:15.000000 kiwigrad-0.0.6/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-08 16:32:15.000000 kiwigrad-0.0.6/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-08 16:32:15.000000 kiwigrad-0.0.6/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-08 16:32:15.000000 kiwigrad-0.0.6/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      667 2023-04-08 16:31:39.000000 kiwigrad-0.0.6/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-08 16:32:15.038783 kiwigrad-0.0.6/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:36:18.787791 kiwigrad-0.0.7/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.0.7/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.0.7/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-08 16:36:18.787429 kiwigrad-0.0.7/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.0.7/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:36:18.785017 kiwigrad-0.0.7/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      222 2023-04-08 16:35:37.000000 kiwigrad-0.0.7/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.0.7/kiwigrad/engine.pyx
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.0.7/kiwigrad/graph.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 16:36:18.786983 kiwigrad-0.0.7/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-08 16:36:18.000000 kiwigrad-0.0.7/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      262 2023-04-08 16:36:18.000000 kiwigrad-0.0.7/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-08 16:36:18.000000 kiwigrad-0.0.7/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-08 16:36:18.000000 kiwigrad-0.0.7/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-08 16:36:18.000000 kiwigrad-0.0.7/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      667 2023-04-08 16:35:41.000000 kiwigrad-0.0.7/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-08 16:36:18.787908 kiwigrad-0.0.7/setup.cfg
```

### Comparing `kiwigrad-0.0.6/LICENSE` & `kiwigrad-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.6/PKG-INFO` & `kiwigrad-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.0.6/kiwigrad/engine.pyx` & `kiwigrad-0.0.7/kiwigrad/engine.pyx`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.6/kiwigrad/graph.py` & `kiwigrad-0.0.7/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.6/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.0.7/kiwigrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.0.6/pyproject.toml` & `kiwigrad-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

