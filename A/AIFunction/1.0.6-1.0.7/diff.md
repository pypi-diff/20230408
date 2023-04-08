# Comparing `tmp/AIFunction-1.0.6.tar.gz` & `tmp/AIFunction-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFunction-1.0.6.tar", last modified: Sat Apr  8 18:50:50 2023, max compression
+gzip compressed data, was "AIFunction-1.0.7.tar", last modified: Sat Apr  8 18:52:17 2023, max compression
```

## Comparing `AIFunction-1.0.6.tar` & `AIFunction-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.122104 AIFunction-1.0.6/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:50:50.121563 AIFunction-1.0.6/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.6/README.md
--rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.6/pyproject.toml
--rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 18:50:50.122282 AIFunction-1.0.6/setup.cfg
--rw-r--r--   0 nekumelon   (501) staff       (20)      746 2023-04-08 18:50:37.000000 AIFunction-1.0.6/setup.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.109361 AIFunction-1.0.6/src/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.112486 AIFunction-1.0.6/src/AIFunction/
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:42:58.000000 AIFunction-1.0.6/src/AIFunction/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.6/src/AIFunction/main.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.117056 AIFunction-1.0.6/src/AIFunction/modules/
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:24.000000 AIFunction-1.0.6/src/AIFunction/modules/__init__.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.117650 AIFunction-1.0.6/src/AIFunction/modules/web/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.119996 AIFunction-1.0.6/src/AIFunction/modules/web/OpenAI/
--rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.6/src/AIFunction/modules/web/OpenAI/OpenAI.py
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:31.000000 AIFunction-1.0.6/src/AIFunction/modules/web/OpenAI/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:28.000000 AIFunction-1.0.6/src/AIFunction/modules/web/__init__.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:50:50.116320 AIFunction-1.0.6/src/AIFunction.egg-info/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:50:50.000000 AIFunction-1.0.6/src/AIFunction.egg-info/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      399 2023-04-08 18:50:50.000000 AIFunction-1.0.6/src/AIFunction.egg-info/SOURCES.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:50:50.000000 AIFunction-1.0.6/src/AIFunction.egg-info/dependency_links.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:50:50.000000 AIFunction-1.0.6/src/AIFunction.egg-info/top_level.txt
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.586409 AIFunction-1.0.7/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:52:17.586019 AIFunction-1.0.7/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.7/README.md
+-rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.7/pyproject.toml
+-rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 18:52:17.587678 AIFunction-1.0.7/setup.cfg
+-rw-r--r--   0 nekumelon   (501) staff       (20)      746 2023-04-08 18:52:05.000000 AIFunction-1.0.7/setup.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.523742 AIFunction-1.0.7/src/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.551768 AIFunction-1.0.7/src/AIFunction/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:42:58.000000 AIFunction-1.0.7/src/AIFunction/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.7/src/AIFunction/main.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.567775 AIFunction-1.0.7/src/AIFunction/modules/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:24.000000 AIFunction-1.0.7/src/AIFunction/modules/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.578977 AIFunction-1.0.7/src/AIFunction/modules/web/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.585052 AIFunction-1.0.7/src/AIFunction/modules/web/OpenAI/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.7/src/AIFunction/modules/web/OpenAI/OpenAI.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:31.000000 AIFunction-1.0.7/src/AIFunction/modules/web/OpenAI/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:28.000000 AIFunction-1.0.7/src/AIFunction/modules/web/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:52:17.563389 AIFunction-1.0.7/src/AIFunction.egg-info/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:52:17.000000 AIFunction-1.0.7/src/AIFunction.egg-info/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      399 2023-04-08 18:52:17.000000 AIFunction-1.0.7/src/AIFunction.egg-info/SOURCES.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:52:17.000000 AIFunction-1.0.7/src/AIFunction.egg-info/dependency_links.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:52:17.000000 AIFunction-1.0.7/src/AIFunction.egg-info/top_level.txt
```

### Comparing `AIFunction-1.0.6/PKG-INFO` & `AIFunction-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIFunction-1.0.6/README.md` & `AIFunction-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.6/setup.py` & `AIFunction-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "AIFunction",
-    version = "1.0.6",
+    version = "1.0.7",
     author = "nekumelon",
     author_email = "nekumelon@gmail.com",
     description = "Generate realtime AI Functions!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nekumelon/AIFunction",
     project_urls = {
```

### Comparing `AIFunction-1.0.6/src/AIFunction/main.py` & `AIFunction-1.0.7/src/AIFunction/main.py`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.6/src/AIFunction.egg-info/PKG-INFO` & `AIFunction-1.0.7/src/AIFunction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

