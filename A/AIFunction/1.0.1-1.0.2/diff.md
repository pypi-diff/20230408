# Comparing `tmp/AIFunction-1.0.1.tar.gz` & `tmp/AIFunction-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFunction-1.0.1.tar", last modified: Sat Apr  8 17:54:07 2023, max compression
+gzip compressed data, was "AIFunction-1.0.2.tar", last modified: Sat Apr  8 17:58:05 2023, max compression
```

## Comparing `AIFunction-1.0.1.tar` & `AIFunction-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:54:07.530195 AIFunction-1.0.1/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1605 2023-04-08 17:54:07.529609 AIFunction-1.0.1/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)     1197 2023-04-08 17:53:14.000000 AIFunction-1.0.1/README.md
--rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.1/pyproject.toml
--rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 17:54:07.537565 AIFunction-1.0.1/setup.cfg
--rw-r--r--   0 nekumelon   (501) staff       (20)      757 2023-04-08 17:53:49.000000 AIFunction-1.0.1/setup.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:54:07.514991 AIFunction-1.0.1/src/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:54:07.528082 AIFunction-1.0.1/src/AIFunction.egg-info/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1605 2023-04-08 17:54:07.000000 AIFunction-1.0.1/src/AIFunction.egg-info/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      185 2023-04-08 17:54:07.000000 AIFunction-1.0.1/src/AIFunction.egg-info/SOURCES.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 17:54:07.000000 AIFunction-1.0.1/src/AIFunction.egg-info/dependency_links.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 17:54:07.000000 AIFunction-1.0.1/src/AIFunction.egg-info/top_level.txt
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:58:05.524244 AIFunction-1.0.2/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 17:58:05.518428 AIFunction-1.0.2/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.2/README.md
+-rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.2/pyproject.toml
+-rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 17:58:05.524454 AIFunction-1.0.2/setup.cfg
+-rw-r--r--   0 nekumelon   (501) staff       (20)      757 2023-04-08 17:57:47.000000 AIFunction-1.0.2/setup.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:58:05.500792 AIFunction-1.0.2/src/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 17:58:05.517345 AIFunction-1.0.2/src/AIFunction.egg-info/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 17:58:05.000000 AIFunction-1.0.2/src/AIFunction.egg-info/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      185 2023-04-08 17:58:05.000000 AIFunction-1.0.2/src/AIFunction.egg-info/SOURCES.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 17:58:05.000000 AIFunction-1.0.2/src/AIFunction.egg-info/dependency_links.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 17:58:05.000000 AIFunction-1.0.2/src/AIFunction.egg-info/top_level.txt
```

### Comparing `AIFunction-1.0.1/PKG-INFO` & `AIFunction-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # AI Function
 
-<img width=200 src='./assets/logo.png'></img>
-
 Generate realtime AI Functions!
 
 ## Installation
 
 To install AI Function, run:
 
 ```bash
```

### Comparing `AIFunction-1.0.1/README.md` & `AIFunction-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # AI Function
 
-<img width=200 src='./assets/logo.png'></img>
-
 Generate realtime AI Functions!
 
 ## Installation
 
 To install AI Function, run:
 
 ```bash
```

### Comparing `AIFunction-1.0.1/setup.py` & `AIFunction-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "AIFunction",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "nekumelon",
     author_email = "nekumelon@gmail.com",
     description = "Generate realtime AI Functions!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nekumelon/AIFunction",
     project_urls = {
```

### Comparing `AIFunction-1.0.1/src/AIFunction.egg-info/PKG-INFO` & `AIFunction-1.0.2/src/AIFunction.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # AI Function
 
-<img width=200 src='./assets/logo.png'></img>
-
 Generate realtime AI Functions!
 
 ## Installation
 
 To install AI Function, run:
 
 ```bash
```

