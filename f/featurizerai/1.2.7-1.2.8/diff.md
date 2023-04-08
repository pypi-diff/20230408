# Comparing `tmp/featurizerai-1.2.7.tar.gz` & `tmp/featurizerai-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.2.7.tar", last modified: Sat Apr  8 16:19:41 2023, max compression
+gzip compressed data, was "featurizerai-1.2.8.tar", last modified: Sat Apr  8 16:21:20 2023, max compression
```

## Comparing `featurizerai-1.2.7.tar` & `featurizerai-1.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.330403 featurizerai-1.2.7/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.2.7/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.2.7/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:19:41.330485 featurizerai-1.2.7/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.2.7/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-08 16:19:41.330717 featurizerai-1.2.7/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-08 16:19:37.000000 featurizerai-1.2.7/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.326617 featurizerai-1.2.7/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.327990 featurizerai-1.2.7/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)       23 2023-03-30 14:54:55.000000 featurizerai-1.2.7/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.329347 featurizerai-1.2.7/src/featurizerai/datasource/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:04.000000 featurizerai-1.2.7/src/featurizerai/datasource/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      573 2023-03-30 14:51:50.000000 featurizerai-1.2.7/src/featurizerai/datasource/create_batch_source.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      858 2023-03-30 14:35:45.000000 featurizerai-1.2.7/src/featurizerai/datasource/create_parquet_sample_file.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.329762 featurizerai-1.2.7/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.2.7/src/featurizerai/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4539 2023-04-08 15:20:31.000000 featurizerai-1.2.7/src/featurizerai/features/featureview.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.328829 featurizerai-1.2.7/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:19:41.000000 featurizerai-1.2.7/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      531 2023-04-08 16:19:41.000000 featurizerai-1.2.7/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-08 16:19:41.000000 featurizerai-1.2.7/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-08 16:19:41.000000 featurizerai-1.2.7/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-08 16:19:41.000000 featurizerai-1.2.7/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:19:41.330125 featurizerai-1.2.7/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      815 2023-04-08 16:04:55.000000 featurizerai-1.2.7/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.533523 featurizerai-1.2.8/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.2.8/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.2.8/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:21:20.533615 featurizerai-1.2.8/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.2.8/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-08 16:21:20.533849 featurizerai-1.2.8/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-08 16:21:17.000000 featurizerai-1.2.8/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.529840 featurizerai-1.2.8/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.531138 featurizerai-1.2.8/src/featurizerai/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.2.8/src/featurizerai/__init__.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.532457 featurizerai-1.2.8/src/featurizerai/datasource/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:04.000000 featurizerai-1.2.8/src/featurizerai/datasource/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      573 2023-03-30 14:51:50.000000 featurizerai-1.2.8/src/featurizerai/datasource/create_batch_source.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      858 2023-03-30 14:35:45.000000 featurizerai-1.2.8/src/featurizerai/datasource/create_parquet_sample_file.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.532943 featurizerai-1.2.8/src/featurizerai/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.2.8/src/featurizerai/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4539 2023-04-08 15:20:31.000000 featurizerai-1.2.8/src/featurizerai/features/featureview.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.531841 featurizerai-1.2.8/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      531 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-08 16:21:20.000000 featurizerai-1.2.8/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:20.533268 featurizerai-1.2.8/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      815 2023-04-08 16:04:55.000000 featurizerai-1.2.8/tests/test_module1.py
```

### Comparing `featurizerai-1.2.7/LICENSE` & `featurizerai-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.7/PKG-INFO` & `featurizerai-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.2.7/setup.py` & `featurizerai-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.2.7',
+    version='1.2.8',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakgloba/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.2.7/src/featurizerai/datasource/create_batch_source.py` & `featurizerai-1.2.8/src/featurizerai/datasource/create_batch_source.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.7/src/featurizerai/datasource/create_parquet_sample_file.py` & `featurizerai-1.2.8/src/featurizerai/datasource/create_parquet_sample_file.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.7/src/featurizerai/features/featureview.py` & `featurizerai-1.2.8/src/featurizerai/features/featureview.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.7/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.2.8/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakgloba/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.2.7/src/featurizerai.egg-info/SOURCES.txt` & `featurizerai-1.2.8/src/featurizerai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featurizerai-1.2.7/tests/test_module1.py` & `featurizerai-1.2.8/tests/test_module1.py`

 * *Files identical despite different names*

