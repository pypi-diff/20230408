# Comparing `tmp/pynarrator-0.0.1.6.tar.gz` & `tmp/pynarrator-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynarrator-0.0.1.6.tar", last modified: Sat Apr  8 18:47:57 2023, max compression
+gzip compressed data, was "pynarrator-0.0.1.7.tar", last modified: Sat Apr  8 19:49:25 2023, max compression
```

## Comparing `pynarrator-0.0.1.6.tar` & `pynarrator-0.0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.693501 pynarrator-0.0.1.6/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.6/LICENSE
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1684 2023-04-08 18:47:57.693376 pynarrator-0.0.1.6/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      968 2023-04-08 18:46:26.000000 pynarrator-0.0.1.6/README.md
--rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-08 18:47:57.693537 pynarrator-0.0.1.6/setup.cfg
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-08 18:47:16.000000 pynarrator-0.0.1.6/setup.py
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.691683 pynarrator-0.0.1.6/src/
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.692869 pynarrator-0.0.1.6/src/pynarrator.egg-info/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1684 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/SOURCES.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/dependency_links.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/requires.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/top_level.txt
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.692989 pynarrator-0.0.1.6/tests/
--rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.6/tests/test_narrate_descriptive.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.333199 pynarrator-0.0.1.7/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.7/LICENSE
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-08 19:49:25.333073 pynarrator-0.0.1.7/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      968 2023-04-08 18:46:26.000000 pynarrator-0.0.1.7/README.md
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-08 19:49:25.333234 pynarrator-0.0.1.7/setup.cfg
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-08 19:49:19.000000 pynarrator-0.0.1.7/setup.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.331831 pynarrator-0.0.1.7/src/
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.332806 pynarrator-0.0.1.7/src/pynarrator.egg-info/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1740 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/SOURCES.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/dependency_links.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/requires.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-08 19:49:25.000000 pynarrator-0.0.1.7/src/pynarrator.egg-info/top_level.txt
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 19:49:25.332910 pynarrator-0.0.1.7/tests/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.7/tests/test_narrate_descriptive.py
```

### Comparing `pynarrator-0.0.1.6/LICENSE` & `pynarrator-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynarrator-0.0.1.6/PKG-INFO` & `pynarrator-0.0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Template-based NLG framework for creating text narratives out of data
+Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
+License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -57,7 +60,9 @@
 ```
 
 ```python
 summarize_narrative(narrative)
 ```
 
 Complete documentation is available at the [narrator](https://denisabd.github.io/narrator/) package website
+
+
```

### Comparing `pynarrator-0.0.1.6/README.md` & `pynarrator-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pynarrator-0.0.1.6/setup.py` & `pynarrator-0.0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open('README.md', 'r') as fh:
    long_description = fh.read()
   
 setup(
   name = 'pynarrator',
-  version = '0.0.1.6',
+  version = '0.0.1.7',
   author = 'Denis Abdullin',
   author_email = 'denisabdullincz@gmail.com',
   description = 'Template-based NLG framework for creating text narratives out of data',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   py_modules = [
     'narrate_descriptive',
```

### Comparing `pynarrator-0.0.1.6/src/pynarrator.egg-info/PKG-INFO` & `pynarrator-0.0.1.7/src/pynarrator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: Template-based NLG framework for creating text narratives out of data
+Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
+License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -57,7 +60,9 @@
 ```
 
 ```python
 summarize_narrative(narrative)
 ```
 
 Complete documentation is available at the [narrator](https://denisabd.github.io/narrator/) package website
+
+
```

