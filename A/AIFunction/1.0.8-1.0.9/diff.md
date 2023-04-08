# Comparing `tmp/AIFunction-1.0.8.tar.gz` & `tmp/AIFunction-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFunction-1.0.8.tar", last modified: Sat Apr  8 19:01:25 2023, max compression
+gzip compressed data, was "AIFunction-1.0.9.tar", last modified: Sat Apr  8 19:06:15 2023, max compression
```

## Comparing `AIFunction-1.0.8.tar` & `AIFunction-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.578300 AIFunction-1.0.8/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 19:01:25.577597 AIFunction-1.0.8/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.8/README.md
--rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.8/pyproject.toml
--rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 19:01:25.579189 AIFunction-1.0.8/setup.cfg
--rw-r--r--   0 nekumelon   (501) staff       (20)      818 2023-04-08 19:01:15.000000 AIFunction-1.0.8/setup.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.560708 AIFunction-1.0.8/src/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.565593 AIFunction-1.0.8/src/AIFunction/
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:42:58.000000 AIFunction-1.0.8/src/AIFunction/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.8/src/AIFunction/main.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.574356 AIFunction-1.0.8/src/AIFunction/modules/
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:24.000000 AIFunction-1.0.8/src/AIFunction/modules/__init__.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.574793 AIFunction-1.0.8/src/AIFunction/modules/web/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.577098 AIFunction-1.0.8/src/AIFunction/modules/web/OpenAI/
--rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.8/src/AIFunction/modules/web/OpenAI/OpenAI.py
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:31.000000 AIFunction-1.0.8/src/AIFunction/modules/web/OpenAI/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:28.000000 AIFunction-1.0.8/src/AIFunction/modules/web/__init__.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:01:25.572310 AIFunction-1.0.8/src/AIFunction.egg-info/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 19:01:25.000000 AIFunction-1.0.8/src/AIFunction.egg-info/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      399 2023-04-08 19:01:25.000000 AIFunction-1.0.8/src/AIFunction.egg-info/SOURCES.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 19:01:25.000000 AIFunction-1.0.8/src/AIFunction.egg-info/dependency_links.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)       83 2023-04-08 19:01:25.000000 AIFunction-1.0.8/src/AIFunction.egg-info/top_level.txt
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.216069 AIFunction-1.0.9/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 19:06:15.215392 AIFunction-1.0.9/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1150 2023-04-08 17:57:38.000000 AIFunction-1.0.9/README.md
+-rw-r--r--   0 nekumelon   (501) staff       (20)       84 2023-04-08 01:58:13.000000 AIFunction-1.0.9/pyproject.toml
+-rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-08 19:06:15.216274 AIFunction-1.0.9/setup.cfg
+-rw-r--r--   0 nekumelon   (501) staff       (20)      802 2023-04-08 19:05:53.000000 AIFunction-1.0.9/setup.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.203551 AIFunction-1.0.9/src/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.207922 AIFunction-1.0.9/src/AIFunction/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:42:58.000000 AIFunction-1.0.9/src/AIFunction/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)     2498 2023-04-08 03:05:28.000000 AIFunction-1.0.9/src/AIFunction/main.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.212141 AIFunction-1.0.9/src/AIFunction/modules/
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:24.000000 AIFunction-1.0.9/src/AIFunction/modules/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.212593 AIFunction-1.0.9/src/AIFunction/modules/web/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.214778 AIFunction-1.0.9/src/AIFunction/modules/web/OpenAI/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-1.0.9/src/AIFunction/modules/web/OpenAI/OpenAI.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:31.000000 AIFunction-1.0.9/src/AIFunction/modules/web/OpenAI/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-08 18:23:28.000000 AIFunction-1.0.9/src/AIFunction/modules/web/__init__.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-08 19:06:15.211259 AIFunction-1.0.9/src/AIFunction.egg-info/
+-rw-r--r--   0 nekumelon   (501) staff       (20)     1558 2023-04-08 19:06:15.000000 AIFunction-1.0.9/src/AIFunction.egg-info/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      399 2023-04-08 19:06:15.000000 AIFunction-1.0.9/src/AIFunction.egg-info/SOURCES.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-08 19:06:15.000000 AIFunction-1.0.9/src/AIFunction.egg-info/dependency_links.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)       11 2023-04-08 19:06:15.000000 AIFunction-1.0.9/src/AIFunction.egg-info/top_level.txt
```

### Comparing `AIFunction-1.0.8/PKG-INFO` & `AIFunction-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIFunction-1.0.8/README.md` & `AIFunction-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.8/src/AIFunction/main.py` & `AIFunction-1.0.9/src/AIFunction/main.py`

 * *Files identical despite different names*

### Comparing `AIFunction-1.0.8/src/AIFunction.egg-info/PKG-INFO` & `AIFunction-1.0.9/src/AIFunction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIFunction
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate realtime AI Functions!
 Home-page: https://github.com/nekumelon/AIFunction
 Author: nekumelon
 Author-email: nekumelon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

