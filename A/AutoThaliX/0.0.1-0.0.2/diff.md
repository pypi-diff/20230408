# Comparing `tmp/AutoThaliX-0.0.1.tar.gz` & `tmp/AutoThaliX-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoThaliX-0.0.1.tar", last modified: Sat Apr  8 17:17:19 2023, max compression
+gzip compressed data, was "AutoThaliX-0.0.2.tar", last modified: Sat Apr  8 21:18:52 2023, max compression
```

## Comparing `AutoThaliX-0.0.1.tar` & `AutoThaliX-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 arkadiymirzabbekyan   (501) staff       (20)        0 2023-04-08 17:17:19.064628 AutoThaliX-0.0.1/
-drwxr-xr-x   0 arkadiymirzabbekyan   (501) staff       (20)        0 2023-04-08 17:17:19.061946 AutoThaliX-0.0.1/AutoThaliX.egg-info/
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     1440 2023-04-08 17:17:19.000000 AutoThaliX-0.0.1/AutoThaliX.egg-info/PKG-INFO
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)      376 2023-04-08 17:17:19.000000 AutoThaliX-0.0.1/AutoThaliX.egg-info/SOURCES.txt
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)        1 2023-04-08 17:17:19.000000 AutoThaliX-0.0.1/AutoThaliX.egg-info/dependency_links.txt
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)       33 2023-04-08 17:17:19.000000 AutoThaliX-0.0.1/AutoThaliX.egg-info/requires.txt
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)       17 2023-04-08 17:17:19.000000 AutoThaliX-0.0.1/AutoThaliX.egg-info/top_level.txt
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     1064 2023-04-06 19:58:11.000000 AutoThaliX-0.0.1/LICENSE
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     1440 2023-04-08 17:17:19.064489 AutoThaliX-0.0.1/PKG-INFO
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)      977 2023-04-07 19:10:49.000000 AutoThaliX-0.0.1/README.md
-drwxr-xr-x   0 arkadiymirzabbekyan   (501) staff       (20)        0 2023-04-08 17:17:19.062884 AutoThaliX-0.0.1/autothalix/
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)      101 2023-04-08 17:05:37.000000 AutoThaliX-0.0.1/autothalix/__init__.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)      486 2023-03-25 10:23:36.000000 AutoThaliX-0.0.1/autothalix/logging.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)    13553 2023-04-08 16:53:46.000000 AutoThaliX-0.0.1/autothalix/measurements.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     1913 2023-04-08 16:18:27.000000 AutoThaliX-0.0.1/autothalix/utils.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)       38 2023-04-08 17:17:19.064669 AutoThaliX-0.0.1/setup.cfg
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)      869 2023-04-07 19:38:06.000000 AutoThaliX-0.0.1/setup.py
-drwxr-xr-x   0 arkadiymirzabbekyan   (501) staff       (20)        0 2023-04-08 17:17:19.064140 AutoThaliX-0.0.1/tests/
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)        0 2023-03-25 10:23:36.000000 AutoThaliX-0.0.1/tests/__init__.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     4453 2023-04-06 20:24:53.000000 AutoThaliX-0.0.1/tests/test_cv.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     3481 2023-04-06 20:24:53.000000 AutoThaliX-0.0.1/tests/test_imp.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     5699 2023-04-06 20:24:53.000000 AutoThaliX-0.0.1/tests/test_lsv.py
--rw-r--r--   0 arkadiymirzabbekyan   (501) staff       (20)     3128 2023-04-06 20:24:53.000000 AutoThaliX-0.0.1/tests/test_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.409480 AutoThaliX-0.0.2/AutoThaliX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.409480 AutoThaliX-0.0.2/autothalix/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-08 21:18:04.000000 AutoThaliX-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_lsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_ocp.py
```

### Comparing `AutoThaliX-0.0.1/AutoThaliX.egg-info/PKG-INFO` & `AutoThaliX-0.0.2/AutoThaliX.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,51 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![AutoThalix](logo.png)
 
 Repository that contains a toolkit to coduct complex operations on potentiostat.
 
+Documentation: https://autothalix.readthedocs.io/en/latest/
+
 ## How to use
 
 Usage of this package is demonstrated in [this repository](https://github.com/Arkady-A/AutoThalix_experiments). You can fork or clone it and start using it.
 
+## Communication
+### Report an issue or bug:
+
+- Go to the repository's main page and click on the "Issues" tab.
+- Click the "New Issue" button.
+- Enter a descriptive title and a description of the issue.
+- Add any relevant labels, milestones, or assignees.
+- Click "Submit new issue."
+ 
+### Request a new feature or enhancement:
+
+- Go to the repository's main page and click on the "Issues" tab.
+- Click the "New Issue" button.
+- Enter a descriptive title and a detailed description of the feature or enhancement.
+- Add the "enhancement" label.
+- Add any relevant labels, milestones, or assignees.
+- Click "Submit new issue."
+
 
 ## Participate in development
 
 Run this command to create virtual environment:
 
 ````
 python -m venv venv
@@ -59,7 +81,9 @@
 
 Run this command to run all tests with coverage and open coverage report in browser:
 
 ````
 pytest --cov=thales --cov-report=html && open htmlcov/index.html
 ````
 
+
+
```

### Comparing `AutoThaliX-0.0.1/LICENSE` & `AutoThaliX-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/PKG-INFO` & `AutoThaliX-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,51 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![AutoThalix](logo.png)
 
 Repository that contains a toolkit to coduct complex operations on potentiostat.
 
+Documentation: https://autothalix.readthedocs.io/en/latest/
+
 ## How to use
 
 Usage of this package is demonstrated in [this repository](https://github.com/Arkady-A/AutoThalix_experiments). You can fork or clone it and start using it.
 
+## Communication
+### Report an issue or bug:
+
+- Go to the repository's main page and click on the "Issues" tab.
+- Click the "New Issue" button.
+- Enter a descriptive title and a description of the issue.
+- Add any relevant labels, milestones, or assignees.
+- Click "Submit new issue."
+ 
+### Request a new feature or enhancement:
+
+- Go to the repository's main page and click on the "Issues" tab.
+- Click the "New Issue" button.
+- Enter a descriptive title and a detailed description of the feature or enhancement.
+- Add the "enhancement" label.
+- Add any relevant labels, milestones, or assignees.
+- Click "Submit new issue."
+
 
 ## Participate in development
 
 Run this command to create virtual environment:
 
 ````
 python -m venv venv
@@ -59,7 +81,9 @@
 
 Run this command to run all tests with coverage and open coverage report in browser:
 
 ````
 pytest --cov=thales --cov-report=html && open htmlcov/index.html
 ````
 
+
+
```

### Comparing `AutoThaliX-0.0.1/autothalix/measurements.py` & `AutoThaliX-0.0.2/autothalix/measurements.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/autothalix/utils.py` & `AutoThaliX-0.0.2/autothalix/utils.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/setup.py` & `AutoThaliX-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 install_requires = [req.strip() for req in requirements]
 
 setuptools.setup(
     name="AutoThaliX",
-    version="0.0.1",
+    version="0.0.2",
     author="ArkadyA",
     author_email="arkadymirz@gmail.com",
     description="A set of tools to work with tales potentiostats. Uses tales_remote",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arkady-A/autothalix",
     packages=setuptools.find_packages(),
```

### Comparing `AutoThaliX-0.0.1/tests/test_cv.py` & `AutoThaliX-0.0.2/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/tests/test_imp.py` & `AutoThaliX-0.0.2/tests/test_imp.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/tests/test_lsv.py` & `AutoThaliX-0.0.2/tests/test_lsv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.1/tests/test_ocp.py` & `AutoThaliX-0.0.2/tests/test_ocp.py`

 * *Files identical despite different names*

