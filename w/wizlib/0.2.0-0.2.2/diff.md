# Comparing `tmp/wizlib-0.2.0.tar.gz` & `tmp/wizlib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.2.0.tar", last modified: Thu Apr  6 16:30:47 2023, max compression
+gzip compressed data, was "wizlib-0.2.2.tar", last modified: Sat Apr  8 20:46:25 2023, max compression
```

## Comparing `wizlib-0.2.0.tar` & `wizlib-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-06 16:30:47.567392 wizlib-0.2.0/
--rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-06 16:30:47.566998 wizlib-0.2.0/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1506 2023-04-06 16:26:14.000000 wizlib-0.2.0/README.md
--rw-r--r--   0 francispotter   (501) staff       (20)      466 2023-04-06 16:17:22.000000 wizlib-0.2.0/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-06 16:30:47.567499 wizlib-0.2.0/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-06 16:26:33.000000 wizlib-0.2.0/version
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-06 16:30:47.562908 wizlib-0.2.0/wizlib/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-06 04:54:28.000000 wizlib-0.2.0/wizlib/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1246 2023-04-05 23:35:32.000000 wizlib-0.2.0/wizlib/rlinput.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-06 16:30:47.566341 wizlib-0.2.0/wizlib.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-06 16:30:47.000000 wizlib-0.2.0/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      218 2023-04-06 16:30:47.000000 wizlib-0.2.0/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-06 16:30:47.000000 wizlib-0.2.0/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       12 2023-04-06 16:30:47.000000 wizlib-0.2.0/wizlib.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-04-06 16:30:47.000000 wizlib-0.2.0/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.179970 wizlib-0.2.2/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-08 20:46:25.179190 wizlib-0.2.2/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1506 2023-04-06 16:26:14.000000 wizlib-0.2.2/README.md
+-rw-r--r--   0 francispotter   (501) staff       (20)      540 2023-04-08 05:14:05.000000 wizlib-0.2.2/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-08 20:46:25.180263 wizlib-0.2.2/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-08 20:46:06.000000 wizlib-0.2.2/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.173927 wizlib-0.2.2/wizlib/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-06 04:54:28.000000 wizlib-0.2.2/wizlib/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1750 2023-04-08 20:06:29.000000 wizlib-0.2.2/wizlib/rlinput.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-08 20:46:25.178398 wizlib-0.2.2/wizlib.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1771 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      218 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       89 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-04-08 20:46:25.000000 wizlib-0.2.2/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.2.0/PKG-INFO` & `wizlib-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.0
+Version: 0.2.2
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.2.0/README.md` & `wizlib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.0/wizlib.egg-info/PKG-INFO` & `wizlib-0.2.2/wizlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.0
+Version: 0.2.2
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

