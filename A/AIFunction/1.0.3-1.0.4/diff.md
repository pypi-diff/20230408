# Comparing `tmp/AIFunction-1.0.3.tar.gz` & `tmp/AIFunction-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFunction-1.0.3.tar", last modified: Sat Apr  8 18:13:53 2023, max compression
+gzip compressed data, was "AIFunction-1.0.4.tar", last modified: Sat Apr  8 18:25:07 2023, max compression
```

## Comparing `AIFunction-1.0.3.tar` & `AIFunction-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.696108 AIFunction-1.0.3/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:13:53.695495 AIFunction-1.0.3/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.3/README.md
--rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.3/pyproject.toml
--rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 18:13:53.696317 AIFunction-1.0.3/setup.cfg
--rw-r--r--   0 nekumelon   (501) staff       (20)      757 2023-04-08 18:11:57.000000 AIFunction-1.0.3/setup.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.679625 AIFunction-1.0.3/src/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.683985 AIFunction-1.0.3/src/AIFunction/
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:23:33.000000 AIFunction-1.0.3/src/AIFunction/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.3/src/AIFunction/main.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.680059 AIFunction-1.0.3/src/AIFunction/modules/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.680272 AIFunction-1.0.3/src/AIFunction/modules/web/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.694056 AIFunction-1.0.3/src/AIFunction/modules/web/OpenAI/
--rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.3/src/AIFunction/modules/web/OpenAI/OpenAI.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:13:53.693257 AIFunction-1.0.3/src/AIFunction.egg-info/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:13:53.000000 AIFunction-1.0.3/src/AIFunction.egg-info/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      279 2023-04-08 18:13:53.000000 AIFunction-1.0.3/src/AIFunction.egg-info/SOURCES.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:13:53.000000 AIFunction-1.0.3/src/AIFunction.egg-info/dependency_links.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)       11 2023-04-08 18:13:53.000000 AIFunction-1.0.3/src/AIFunction.egg-info/top_level.txt
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.034957 AIFunction-1.0.4/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:25:07.034151 AIFunction-1.0.4/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.4/README.md
+-rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.4/pyproject.toml
+-rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 18:25:07.035169 AIFunction-1.0.4/setup.cfg
+-rw-r--r--   0 nekumelon   (501) staff       (20)      757 2023-04-08 18:24:51.000000 AIFunction-1.0.4/setup.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.012713 AIFunction-1.0.4/src/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.022446 AIFunction-1.0.4/src/AIFunction/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:23:33.000000 AIFunction-1.0.4/src/AIFunction/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.4/src/AIFunction/main.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.031502 AIFunction-1.0.4/src/AIFunction/modules/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:24.000000 AIFunction-1.0.4/src/AIFunction/modules/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.032081 AIFunction-1.0.4/src/AIFunction/modules/web/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.033602 AIFunction-1.0.4/src/AIFunction/modules/web/OpenAI/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.4/src/AIFunction/modules/web/OpenAI/OpenAI.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:31.000000 AIFunction-1.0.4/src/AIFunction/modules/web/OpenAI/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:28.000000 AIFunction-1.0.4/src/AIFunction/modules/web/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:25:07.030832 AIFunction-1.0.4/src/AIFunction.egg-info/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 18:25:06.000000 AIFunction-1.0.4/src/AIFunction.egg-info/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      399 2023-04-08 18:25:07.000000 AIFunction-1.0.4/src/AIFunction.egg-info/SOURCES.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 18:25:06.000000 AIFunction-1.0.4/src/AIFunction.egg-info/dependency_links.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)       11 2023-04-08 18:25:06.000000 AIFunction-1.0.4/src/AIFunction.egg-info/top_level.txt
```

### Comparing `AIFunction-1.0.3/PKG-INFO` & `AIFunction-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIFunction-1.0.3/README.md` & `AIFunction-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.3/setup.py` & `AIFunction-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "AIFunction",
-    version = "1.0.3",
+    version = "1.0.4",
     author = "nekumelon",
     author_email = "nekumelon@gmail.com",
     description = "Generate realtime AI Functions!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nekumelon/AIFunction",
     project_urls = {
```

### Comparing `AIFunction-1.0.3/src/AIFunction/main.py` & `AIFunction-1.0.4/src/AIFunction/main.py`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.3/src/AIFunction.egg-info/PKG-INFO` & `AIFunction-1.0.4/src/AIFunction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

