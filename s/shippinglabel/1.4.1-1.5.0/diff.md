# Comparing `tmp/shippinglabel-1.4.1.tar.gz` & `tmp/shippinglabel-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippinglabel-1.4.1.tar", last modified: Mon Aug 15 11:30:25 2022, max compression
+gzip compressed data, was "shippinglabel-1.5.0.tar", last modified: Sat Apr  8 21:52:40 2023, max compression
```

## Comparing `shippinglabel-1.4.1.tar` & `shippinglabel-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8239 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-08-15 11:30:25.691675 shippinglabel-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/shippinglabel/
--rw-r--r--   0 runner    (1001) docker     (121)     4991 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/shippinglabel/_vendor/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    38727 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4851 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8539 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10753 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)    21891 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-08-15 11:29:52.000000 shippinglabel-1.4.1/shippinglabel/sdist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 11:30:25.687675 shippinglabel-1.4.1/shippinglabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8239 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-15 11:30:25.000000 shippinglabel-1.4.1/shippinglabel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8157 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-08 21:52:40.604191 shippinglabel-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.596191 shippinglabel-1.5.0/shippinglabel/
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/shippinglabel/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    38727 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4929 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8539 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/conda.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10753 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22077 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/shippinglabel/sdist.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/shippinglabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8157 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-08 21:52:40.000000 shippinglabel-1.5.0/shippinglabel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 21:52:40.600191 shippinglabel-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3219 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_conda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12774 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19625 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_requirements_win.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_sdist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3300 2023-04-08 21:52:03.000000 shippinglabel-1.5.0/tests/test_shippinglabel.py
```

### Comparing `shippinglabel-1.4.1/LICENSE` & `shippinglabel-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/PKG-INFO` & `shippinglabel-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippinglabel
-Version: 1.4.1
+Version: 1.5.0
 Summary: Utilities for handling packages.
 Home-page: https://github.com/domdfcoding/shippinglabel
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -108,16 +109,16 @@
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/shippinglabel/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/shippinglabel/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/shippinglabel?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/shippinglabel?logo=codefactor
@@ -151,23 +152,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.4.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.5.0
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/shippinglabel
 	:target: https://pypi.org/project/shippinglabel/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -183,23 +184,15 @@
 
 .. code-block:: bash
 
 	$ python -m pip install shippinglabel
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install shippinglabel
+	$ conda install -c conda-forge shippinglabel
 
 .. end installation
 
 ``shippinglabel`` includes a vendored copy of `trove-classifiers <https://pypi.org/project/trove-classifiers/>`_.
 If you install a newer version of ``trove-classifiers`` with pip ``shippinglabel`` will use that version instead.
```

### Comparing `shippinglabel-1.4.1/README.rst` & `shippinglabel-1.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/shippinglabel/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/shippinglabel/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/shippinglabel?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/shippinglabel?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.4.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.5.0
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/shippinglabel
 	:target: https://pypi.org/project/shippinglabel/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -128,23 +128,15 @@
 
 .. code-block:: bash
 
 	$ python -m pip install shippinglabel
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install shippinglabel
+	$ conda install -c conda-forge shippinglabel
 
 .. end installation
 
 ``shippinglabel`` includes a vendored copy of `trove-classifiers <https://pypi.org/project/trove-classifiers/>`_.
 If you install a newer version of ``trove-classifiers`` with pip ``shippinglabel`` will use that version instead.
```

### Comparing `shippinglabel-1.4.1/pyproject.toml` & `shippinglabel-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shippinglabel"
-version = "1.4.1"
+version = "1.5.0"
 description = "Utilities for handling packages."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "conda", "packaging", "pypi", "requirements",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
@@ -135,22 +136,22 @@
 base-classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 additional-files = [ "recursive-include shippinglabel/_vendor *", "prune **/__pycache__",]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `shippinglabel-1.4.1/setup.cfg` & `shippinglabel-1.5.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shippinglabel
-version = 1.4.1
+version = 1.5.0
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = packaging, requirements, pypi, conda
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -21,14 +21,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 	Typing :: Typed
 
 [options]
```

### Comparing `shippinglabel-1.4.1/setup.py` & `shippinglabel-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/__init__.py` & `shippinglabel-1.5.0/shippinglabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 		"read_pyvenv",
 		"get_project_links",
 		]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.4.1"
+__version__: str = "1.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 
 def no_dev_versions(versions: Iterable[str]) -> List[str]:
 	"""
 	Returns the subset of ``versions`` which does not end with ``-dev``.
```

### Comparing `shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/LICENSE` & `shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/LICENSE`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/_vendor/trove_classifiers/__init__.py` & `shippinglabel-1.5.0/shippinglabel/_vendor/trove_classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/checksum.py` & `shippinglabel-1.5.0/shippinglabel/checksum.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/classifiers.py` & `shippinglabel-1.5.0/shippinglabel/classifiers.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/conda.py` & `shippinglabel-1.5.0/shippinglabel/conda.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/pypi.py` & `shippinglabel-1.5.0/shippinglabel/pypi.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel/requirements.py` & `shippinglabel-1.5.0/shippinglabel/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 # stdlib
 import warnings
 from abc import ABC
 from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Set, Tuple, Union, cast, overload
 
 # 3rd party
+import dist_meta
 import dom_toml
 from domdf_python_tools.compat import importlib_metadata
 from domdf_python_tools.doctools import prettify_docstrings
 from domdf_python_tools.iterative import natmax, natmin
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.stringlist import DelimitedList, StringList
 from domdf_python_tools.typing import PathLike
@@ -88,15 +89,15 @@
 	def _check_marker_equality(left: Optional[Any], right: Optional[Any]) -> bool:
 		if left is not None and right is not None:
 			for left_mark, right_mark in zip(left._markers, right._markers):
 				if str(left_mark) != str(right_mark):
 					return False
 		return True
 
-	def __eq__(self, other) -> bool:
+	def __eq__(self, other) -> bool:  # noqa: MAN001
 
 		if isinstance(other, str):
 			try:
 				other = Requirement(other)
 			except InvalidRequirement:
 				return NotImplemented
 
@@ -109,44 +110,44 @@
 					self._check_equal_not_none(self.extras, other.extras),
 					self._check_equal_not_none(self.specifier, other.specifier),
 					self._check_marker_equality(self.marker, other.marker),
 					))
 		else:  # pragma: no cover
 			return NotImplemented
 
-	def __lt__(self, other) -> bool:
+	def __lt__(self, other) -> bool:  # noqa: MAN001
 		if isinstance(other, Requirement):
 			if self.name != other.name:
 				return self.name < other.name
 			else:
 				if str(self.specifier or '') != str(other.specifier or ''):
 					return str(self.specifier or '') > str(other.specifier or '')
 				else:
 					return str(self.marker or '') > str(other.marker or '')
 
 		elif isinstance(other, str):
 			return self.name < other
 		else:  # pragma: no cover
 			return NotImplemented
 
-	def __le__(self, other) -> bool:
+	def __le__(self, other) -> bool:  # noqa: MAN001
 		if not isinstance(other, (Requirement, str)):  # pragma: no cover
 			return NotImplemented
 		if self < other or self == other:
 			return True
 		return False
 
-	def __ge__(self, other) -> bool:
+	def __ge__(self, other) -> bool:  # noqa: MAN001
 		if not isinstance(other, (Requirement, str)):  # pragma: no cover
 			return NotImplemented
 		if self > other or self == other:
 			return True
 		return False
 
-	def __gt__(self, other) -> bool:
+	def __gt__(self, other) -> bool:  # noqa: MAN001
 		if isinstance(other, Requirement):
 			if self.name != other.name:
 				return self.name > other.name
 			else:
 				if str(self.specifier or '') != str(other.specifier or ''):
 					return str(self.specifier or '') < str(other.specifier or '')
 				else:
@@ -600,18 +601,20 @@
 
 	.. versionchanged:: 0.8.2  The requirements are now sorted alphabetically.
 	"""
 
 	req = ComparableRequirement(name)
 
 	try:
-		raw_deps = importlib_metadata.requires(req.name) or []
-	except importlib_metadata.PackageNotFoundError:
+		distro = dist_meta.distributions.get_distribution(req.name)
+	except dist_meta.distributions.DistributionNotFoundError:
 		return
 
+	raw_deps = distro.get_metadata().get_all("Requires-Dist") or []
+
 	for requirement in [ComparableRequirement(r) for r in sorted(raw_deps)]:
 		if requirement.marker:
 			if req.extras:
 				extras = list(req.extras)[0]
 			else:
 				extras = ''
 
@@ -739,11 +742,11 @@
 	return {
 			k: parse_requirements(v, include_invalid=True, normalize_func=normalize_func)[0]
 			for k,
 			v in dependencies.items()
 			}
 
 
-def _denormalize_ruamel(req: Requirement):
+def _denormalize_ruamel(req: Requirement) -> None:
 	if req.name in {"ruamel-yaml", "ruamel_yaml"}:
 		# Special case to work around issue with Poetry
 		req.name = "ruamel.yaml"
```

### Comparing `shippinglabel-1.4.1/shippinglabel/sdist.py` & `shippinglabel-1.5.0/shippinglabel/sdist.py`

 * *Files identical despite different names*

### Comparing `shippinglabel-1.4.1/shippinglabel.egg-info/PKG-INFO` & `shippinglabel-1.5.0/shippinglabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippinglabel
-Version: 1.4.1
+Version: 1.5.0
 Summary: Utilities for handling packages.
 Home-page: https://github.com/domdfcoding/shippinglabel
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -108,16 +109,16 @@
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/shippinglabel/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/shippinglabel/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/shippinglabel/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/shippinglabel/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/shippinglabel/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/shippinglabel?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/shippinglabel?logo=codefactor
@@ -151,23 +152,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/shippinglabel
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.4.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/shippinglabel/v1.5.0
 	:target: https://github.com/domdfcoding/shippinglabel/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/shippinglabel
 	:target: https://github.com/domdfcoding/shippinglabel/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/shippinglabel
 	:target: https://pypi.org/project/shippinglabel/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -183,23 +184,15 @@
 
 .. code-block:: bash
 
 	$ python -m pip install shippinglabel
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install shippinglabel
+	$ conda install -c conda-forge shippinglabel
 
 .. end installation
 
 ``shippinglabel`` includes a vendored copy of `trove-classifiers <https://pypi.org/project/trove-classifiers/>`_.
 If you install a newer version of ``trove-classifiers`` with pip ``shippinglabel`` will use that version instead.
```

### Comparing `shippinglabel-1.4.1/shippinglabel.egg-info/SOURCES.txt` & `shippinglabel-1.5.0/shippinglabel.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,17 @@
 shippinglabel.egg-info/requires.txt
 shippinglabel.egg-info/top_level.txt
 shippinglabel/_vendor/__init__.py
 shippinglabel/_vendor/requirements.txt
 shippinglabel/_vendor/trove_classifiers/LICENSE
 shippinglabel/_vendor/trove_classifiers/__init__.py
 shippinglabel/_vendor/trove_classifiers/__main__.py
-shippinglabel/_vendor/trove_classifiers/py.typed
+shippinglabel/_vendor/trove_classifiers/py.typed
+tests/test_checksum.py
+tests/test_classifiers.py
+tests/test_conda.py
+tests/test_pypi.py
+tests/test_requirements.py
+tests/test_requirements_manager.py
+tests/test_requirements_win.py
+tests/test_sdist.py
+tests/test_shippinglabel.py
```

