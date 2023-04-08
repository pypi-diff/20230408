# Comparing `tmp/permuted_brunnermunzel-0.0.1.tar.gz` & `tmp/permuted_brunnermunzel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permuted_brunnermunzel-0.0.1.tar", last modified: Sat Apr  8 16:19:43 2023, max compression
+gzip compressed data, was "permuted_brunnermunzel-0.0.2.tar", last modified: Sat Apr  8 17:54:28 2023, max compression
```

## Comparing `permuted_brunnermunzel-0.0.1.tar` & `permuted_brunnermunzel-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 16:19:43.731446 permuted_brunnermunzel-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-08 16:04:09.000000 permuted_brunnermunzel-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2677 2023-04-08 16:19:43.730458 permuted_brunnermunzel-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1997 2023-04-08 15:34:08.000000 permuted_brunnermunzel-0.0.1/README.md
--rw-rw-rw-   0        0        0      675 2023-04-08 16:06:06.000000 permuted_brunnermunzel-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 16:19:43.731446 permuted_brunnermunzel-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      564 2023-04-08 16:13:31.000000 permuted_brunnermunzel-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:19:43.691446 permuted_brunnermunzel-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 16:19:43.714461 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel/
--rw-rw-rw-   0        0        0        0 2023-04-08 15:59:55.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel/__init__.py
--rw-rw-rw-   0        0        0    13392 2023-04-08 15:12:59.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel/brunnermunzel_test.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:19:43.726462 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/
--rw-rw-rw-   0        0        0     2677 2023-04-08 16:19:43.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-08 16:19:43.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 16:19:43.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-08 16:13:55.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-08 16:19:43.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-08 16:19:43.000000 permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 16:19:43.728462 permuted_brunnermunzel-0.0.1/tests/
--rw-rw-rw-   0        0        0     5800 2023-04-08 15:02:26.000000 permuted_brunnermunzel-0.0.1/tests/test_permuted_brunnermunzel.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:28.107292 permuted_brunnermunzel-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-08 16:04:09.000000 permuted_brunnermunzel-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2725 2023-04-08 17:54:28.106296 permuted_brunnermunzel-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2023-04-08 17:46:57.000000 permuted_brunnermunzel-0.0.2/README.md
+-rw-rw-rw-   0        0        0      675 2023-04-08 17:48:58.000000 permuted_brunnermunzel-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:54:28.108309 permuted_brunnermunzel-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-04-08 17:49:45.000000 permuted_brunnermunzel-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:28.080287 permuted_brunnermunzel-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:28.091298 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel/
+-rw-rw-rw-   0        0        0        0 2023-04-08 17:06:11.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel/__init__.py
+-rw-rw-rw-   0        0        0    13392 2023-04-08 15:12:59.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel/brunnermunzel_test.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:28.103298 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/
+-rw-rw-rw-   0        0        0     2725 2023-04-08 17:54:27.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-08 17:54:27.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:54:27.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-08 16:13:55.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-08 17:54:27.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-08 17:54:27.000000 permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:28.104297 permuted_brunnermunzel-0.0.2/tests/
+-rw-rw-rw-   0        0        0     5800 2023-04-08 15:02:26.000000 permuted_brunnermunzel-0.0.2/tests/test_permuted_brunnermunzel.py
```

### Comparing `permuted_brunnermunzel-0.0.1/LICENSE` & `permuted_brunnermunzel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permuted_brunnermunzel-0.0.1/PKG-INFO` & `permuted_brunnermunzel-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: permuted_brunnermunzel
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of the permuted brunner munzel
 Home-page: https://github.com/MatthewCorney
 Author: Matthew Corney
 Author-email: Matthew Corney <matthew_corney@yahoo.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthewCorney/permuted_brunner_munzel
 Project-URL: Bug Tracker, https://github.com/MatthewCorney/permuted_brunner_munzel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#Introduction
+# Introduction
 This package is an implementation of the permuted version of the Brunner-Munzel test is a nonparametric test.
 The Permuted Brunner-Munzel is best suited to cases where the number of observations in one of the groups is below 10 and
 ideally above 7
 
 This is a reimplementation of the R/Fortran implementation found here https://cran.r-project.org/web/packages/brunnermunzel/index.html . This is for cases where is it not possible or complicated to call R from python
 
-#Dependencies
+# Dependencies
 The function requires the following Python packages:
 
 - numpy
 - scipy
 - math
 
 # Usage
@@ -40,14 +40,17 @@
 
 The function returns a tuple of two float values:
 
 - The first value is the estimated location shift between the two distributions (i.e., the P-value).
 - The second value is the P-value of the test.
 
 # Example
+```
+pip install permuted_brunnermunzel
+```
 
 ```
 from permuted_brunnermunzel import permuted_brunnermunzel
 
 x = [0, 0, 0, 1, 1, 1, 0]
 y = [30, 20, 19, 18, 15, 10, ]
```

### Comparing `permuted_brunnermunzel-0.0.1/README.md` & `permuted_brunnermunzel-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#Introduction
+# Introduction
 This package is an implementation of the permuted version of the Brunner-Munzel test is a nonparametric test.
 The Permuted Brunner-Munzel is best suited to cases where the number of observations in one of the groups is below 10 and
 ideally above 7
 
 This is a reimplementation of the R/Fortran implementation found here https://cran.r-project.org/web/packages/brunnermunzel/index.html . This is for cases where is it not possible or complicated to call R from python
 
-#Dependencies
+# Dependencies
 The function requires the following Python packages:
 
 - numpy
 - scipy
 - math
 
 # Usage
@@ -23,14 +23,17 @@
 
 The function returns a tuple of two float values:
 
 - The first value is the estimated location shift between the two distributions (i.e., the P-value).
 - The second value is the P-value of the test.
 
 # Example
+```
+pip install permuted_brunnermunzel
+```
 
 ```
 from permuted_brunnermunzel import permuted_brunnermunzel
 
 x = [0, 0, 0, 1, 1, 1, 0]
 y = [30, 20, 19, 18, 15, 10, ]
```

### Comparing `permuted_brunnermunzel-0.0.1/pyproject.toml` & `permuted_brunnermunzel-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "permuted_brunnermunzel"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matthew Corney", email="matthew_corney@yahoo.co.uk" },
 ]
 description = "Python implementation of the permuted brunner munzel"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `permuted_brunnermunzel-0.0.1/setup.py` & `permuted_brunnermunzel-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='permuted_brunnermunzel',
-      version='0.1',
+      version='0.0.2',
       description='Python implementation of the permuted brunner munzel',
       url='https://github.com/MatthewCorney',
       author='Matthew Corney',
       author_email='matthew_corney@yahoo.co.uk',
       license='MIT',
       package_dir={'':"src"},
       packages=find_packages("src"),
```

### Comparing `permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel/brunnermunzel_test.py` & `permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel/brunnermunzel_test.py`

 * *Files identical despite different names*

### Comparing `permuted_brunnermunzel-0.0.1/src/permuted_brunnermunzel.egg-info/PKG-INFO` & `permuted_brunnermunzel-0.0.2/src/permuted_brunnermunzel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: permuted-brunnermunzel
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of the permuted brunner munzel
 Home-page: https://github.com/MatthewCorney
 Author: Matthew Corney
 Author-email: Matthew Corney <matthew_corney@yahoo.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthewCorney/permuted_brunner_munzel
 Project-URL: Bug Tracker, https://github.com/MatthewCorney/permuted_brunner_munzel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#Introduction
+# Introduction
 This package is an implementation of the permuted version of the Brunner-Munzel test is a nonparametric test.
 The Permuted Brunner-Munzel is best suited to cases where the number of observations in one of the groups is below 10 and
 ideally above 7
 
 This is a reimplementation of the R/Fortran implementation found here https://cran.r-project.org/web/packages/brunnermunzel/index.html . This is for cases where is it not possible or complicated to call R from python
 
-#Dependencies
+# Dependencies
 The function requires the following Python packages:
 
 - numpy
 - scipy
 - math
 
 # Usage
@@ -40,14 +40,17 @@
 
 The function returns a tuple of two float values:
 
 - The first value is the estimated location shift between the two distributions (i.e., the P-value).
 - The second value is the P-value of the test.
 
 # Example
+```
+pip install permuted_brunnermunzel
+```
 
 ```
 from permuted_brunnermunzel import permuted_brunnermunzel
 
 x = [0, 0, 0, 1, 1, 1, 0]
 y = [30, 20, 19, 18, 15, 10, ]
```

### Comparing `permuted_brunnermunzel-0.0.1/tests/test_permuted_brunnermunzel.py` & `permuted_brunnermunzel-0.0.2/tests/test_permuted_brunnermunzel.py`

 * *Files identical despite different names*

