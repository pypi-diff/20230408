# Comparing `tmp/pcdscalc-0.4.0.tar.gz` & `tmp/pcdscalc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdscalc-0.4.0.tar", last modified: Mon Nov 21 18:12:50 2022, max compression
+gzip compressed data, was "pcdscalc-0.4.1.tar", last modified: Tue Apr  4 19:25:56 2023, max compression
```

## Comparing `pcdscalc-0.4.0.tar` & `pcdscalc-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,58 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3027 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1047 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.131549 pcdscalc-0.4.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      626 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/make.bat
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.135551 pcdscalc-0.4.0/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2376 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/source/be_lens_calcs.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5589 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/docs/source/pmps.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/pcdscalc/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/pcdscalc/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37755 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/be_lens_calcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2683 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9458 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3504 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/diffraction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10288 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/pmps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/pcdscalc/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19199 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/test_be_lens_calcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3698 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2498 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/test_diffraction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4408 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/pcdscalc/tests/test_pmps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-21 18:12:50.135551 pcdscalc-0.4.0/pcdscalc.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1047 2022-11-21 18:12:50.000000 pcdscalc-0.4.0/pcdscalc.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      723 2022-11-21 18:12:50.000000 pcdscalc-0.4.0/pcdscalc.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-11-21 18:12:50.000000 pcdscalc-0.4.0/pcdscalc.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2022-11-21 18:12:50.000000 pcdscalc-0.4.0/pcdscalc.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-11-21 18:12:50.000000 pcdscalc-0.4.0/pcdscalc.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2022-11-21 18:12:50.139553 pcdscalc-0.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80045 2022-11-21 18:12:33.000000 pcdscalc-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/be_lens_calcs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5592 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/pmps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37830 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/diffraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10268 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/pmps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19199 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_diffraction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_lens_sets/lens_set
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_pmps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/setup.cfg
```

### Comparing `pcdscalc-0.4.0/CONTRIBUTING.rst` & `pcdscalc-0.4.1/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -59,31 +59,32 @@
 1. Fork the `pcdscalc` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/pcdscalc.git
 
 3. Install your local copy into a new conda environment. Assuming you have conda installed, this is how you set up your fork for local development::
 
-    $ conda create -n pcdscalc python=3.7
+    $ conda create -n pcdscalc python=3.9 pip
     $ cd pcdscalc/
     $ pip install -e .
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-5. When you're done making changes, check that your changes pass flake8::
+5. Install and enable ``pre-commit`` for this repository::
 
-    $ flake8 pcdscalc
+    $ pip install pre-commit
+    $ pre-commit install
 
 6. Add new tests for any additional functionality or bugs you may have discovered.  And, of course, be sure that all previous tests still pass by running::
 
-    $ python run_tests.py -v
+    $ pytest -v
 
 7. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
@@ -94,10 +95,9 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put your
    new functionality into a function with a docstring, and add the feature to
    the list in README.rst.
-3. The pull request should work for Python 3.5 and up. Check
-   https://travis-ci.org/pcdshub/pcdscalc/pull_requests
+3. The pull request should work for Python 3.9 and up. Check the GitHub Actions status
    and make sure that the tests pass for all supported Python versions.
```

### Comparing `pcdscalc-0.4.0/LICENSE` & `pcdscalc-0.4.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `pcdscalc-0.4.0/README.rst` & `pcdscalc-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/docs/Makefile` & `pcdscalc-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/docs/make.bat` & `pcdscalc-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/docs/source/be_lens_calcs.rst` & `pcdscalc-0.4.1/docs/source/be_lens_calcs.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/docs/source/conf.py` & `pcdscalc-0.4.1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
@@ -41,24 +40,25 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
+    "docs_versions_menu",
+    "numpydoc",
+    "recommonmark",
     "sphinx.ext.autodoc",
-    "sphinx.ext.todo",
     "sphinx.ext.coverage",
+    "sphinx.ext.githubpages",
     "sphinx.ext.mathjax",
+    "sphinx.ext.todo",
     "sphinx.ext.viewcode",
-    "sphinx.ext.githubpages",
-    "numpydoc",
-    "recommonmark",
-    "doctr_versions_menu",
     "sphinx_rtd_theme",
+    "sphinxcontrib.jquery",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 autosummary_generate = True
 
@@ -73,15 +73,15 @@
 master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `pcdscalc-0.4.0/docs/source/index.rst` & `pcdscalc-0.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/be_lens_calcs.py` & `pcdscalc-0.4.1/pcdscalc/be_lens_calcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1047,35 +1047,44 @@
         size_fwhm=size_calc_1,
         distance=z_offset,
         n_max=max_tot_number_of_lenses,
         max_each=max_each,
         lens_radii=LENS_RADII,
     )
 
-    distances = np.asarray([
+    distances = np.asarray(
+        [
             calc_distance_for_size(
                 size_calc_1,
                 list(chain(*list(zip(set, t_lens_radii)))),
                 energy=energy,
                 fwhm_unfocused=beam_size_unfocused,
-            )[focus_before_sample] for set in sets])
+            )[focus_before_sample]
+            for set in sets
+        ]
+    )
 
     good_sets = np.logical_and(
         distances > np.min(z_offset + np.asarray(z_range)),
-        distances < np.max(z_offset + np.asarray(z_range)))
+        distances < np.max(z_offset + np.asarray(z_range))
+    )
 
     sets = sets[good_sets]
-    size_range_min = np.asarray([
+    size_range_min = np.asarray(
+        [
             calc_beam_fwhm(
                 energy,
                 list(chain(*list(zip(set, t_lens_radii)))),
                 distance=z_offset - min(z_range),
                 fwhm_unfocused=beam_size_unfocused,
                 printsummary=False,
-            ) for set in sets])
+            )
+            for set in sets
+        ]
+    )
 
     size_range_max = np.asarray([
         calc_beam_fwhm(
             energy,
             list(chain(*list(zip(set, t_lens_radii)))),
             distance=z_offset - max(z_range),
             fwhm_unfocused=beam_size_unfocused,
```

### Comparing `pcdscalc-0.4.0/pcdscalc/common.py` & `pcdscalc-0.4.1/pcdscalc/common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/constants.py` & `pcdscalc-0.4.1/pcdscalc/constants.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/diffraction.py` & `pcdscalc-0.4.1/pcdscalc/diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/pmps.py` & `pcdscalc-0.4.1/pcdscalc/pmps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Calculation utilities related to the LCLS PMPS system.
 
 Here you will find functions related to eV bitmasks.
 """
 import math
-from typing import List, Optional, Tuple
+from typing import Optional
 
 # Source for these values:
 # lcls-twincat-pmps/PMPS/GVLs/PMPS_GVL.TcGVL
 LFE = [
     1.0E3,
     1.7E3,
     2.1E3,
@@ -37,15 +37,16 @@
     27.0E3,
     28.0E3,
     28.5E3,
     29.0E3,
     30.0E3,
     60.0E3,
     90.0E3,
-    ]
+]
+
 KFE = [
     100,
     250,
     270,
     350,
     400,
     450,
@@ -71,18 +72,18 @@
     2.80E3,
     3.00E3,
     3.15E3,
     3.50E3,
     4.00E3,
     5.30E3,
     7.00E3
-    ]
+]
 
 
-def select_bitmask_boundaries(line: str) -> List[float]:
+def select_bitmask_boundaries(line: str) -> list[float]:
     """
     Given a line, select the bitmask boundaries to use.
 
     These are hard-coded for now but in theory this could be loaded from
     a database, an EPICS PV, or some other source.
 
     Parameters
@@ -106,15 +107,15 @@
 
 
 def get_bitmask(
     lower: float,
     upper: float,
     allow: bool,
     line: str,
-    bounds: Optional[List[float]] = None,
+    bounds: Optional[list[float]] = None,
 ) -> int:
     """
     Given a range of eV values, calculate the appropriate pmps bitmask.
 
     This saves you the effort of checking up on the eV ranges and
     remembering how the bitmask is assembled.
 
@@ -191,15 +192,15 @@
         return lower_range | upper_range
 
 
 def check_bitmask(
     energy: float,
     bitmask: int,
     line: str,
-    bounds: Optional[List[float]] = None,
+    bounds: Optional[list[float]] = None,
 ) -> bool:
     """
     Given an energy and a bitmask, tell us if our energy is allowed.
 
     This is the same calculation the PMPS is doing internally to determine
     if it is safe for beam to proceed.
 
@@ -246,16 +247,16 @@
 
 
 def check_actual_range(
     lower: float,
     upper: float,
     allow: bool,
     line: str,
-    bounds: Optional[List[float]] = None,
-) -> Tuple[float, float]:
+    bounds: Optional[list[float]] = None,
+) -> tuple[float, float]:
     """
     Returns the actual effective range given bitmask precision.
 
     Because of the granularity of the bitmask, most range specifications
     exclude more energy values than requested.
 
     Parameters
@@ -309,15 +310,15 @@
         # The range is empty: return an empty range instead of inf inf.
         return (lower, lower)
 
 
 def describe_bitmask(
     bitmask: int,
     line: str,
-    bounds: Optional[List[float]] = None,
+    bounds: Optional[list[float]] = None,
 ) -> None:
     """
     Print a text description of a bitmask.
 
     This will describe what the bitmask means.
 
     Parameters
@@ -339,16 +340,16 @@
     lines = get_bitmask_desc(bitmask=bitmask, line=line, bounds=bounds)
     print('\n'.join(lines))
 
 
 def get_bitmask_desc(
     bitmask: int,
     line: str,
-    bounds: Optional[List[float]] = None,
-) -> List[str]:
+    bounds: Optional[list[float]] = None,
+) -> list[str]:
     """
     Return a text description of a bitmask.
 
     This will describe what the bitmask means.
 
     Parameters
     ----------
```

### Comparing `pcdscalc-0.4.0/pcdscalc/tests/test_be_lens_calcs.py` & `pcdscalc-0.4.1/pcdscalc/tests/test_be_lens_calcs.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/tests/test_common.py` & `pcdscalc-0.4.1/pcdscalc/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/tests/test_diffraction.py` & `pcdscalc-0.4.1/pcdscalc/tests/test_diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.0/pcdscalc/tests/test_pmps.py` & `pcdscalc-0.4.1/pcdscalc/tests/test_pmps.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,32 @@
 bm4 = 0b1111_1111_1111_1110_1111_1111_1111_1111
 
 
 @pytest.mark.parametrize(
     "test_input,expected",
     [('k', KFE), ('kfe', KFE), ('sxr', KFE),
      ('L', LFE), ('LFE', LFE), ('HXR', LFE)]
-    )
+)
 def test_select_bounds(test_input, expected):
     logger.debug(f'test_select_bounds({test_input}, {expected})')
     assert select_bitmask_boundaries(test_input) is expected
 
 
 @pytest.mark.parametrize(
     "lower,upper,allow,expected",
     [(0, 100, True, allow_all),
      (0, 100, False, allow_none),
-     (0, 15.5, True,     0b0000_0000_0000_0000_0111_1111_1111_1111),
-     (15.5, 100, True,   0b1111_1111_1111_1111_0000_0000_0000_0000),
-     (14.5, 21.5, True,  0b0000_0000_0001_1111_1000_0000_0000_0000),
-     (14.5, 21.5, False, 0b1111_1111_1100_0000_0011_1111_1111_1111),
-     (15, 20, True,      0b0000_0000_0000_1111_1000_0000_0000_0000),
-     (15, 20, False,     0b1111_1111_1111_0000_0111_1111_1111_1111)])
+     (0, 15.5, True,     0b0000_0000_0000_0000_0111_1111_1111_1111),  # noqa: E241
+     (15.5, 100, True,   0b1111_1111_1111_1111_0000_0000_0000_0000),  # noqa: E241
+     (14.5, 21.5, True,  0b0000_0000_0001_1111_1000_0000_0000_0000),  # noqa: E241
+     (14.5, 21.5, False, 0b1111_1111_1100_0000_0011_1111_1111_1111),  # noqa: E241
+     (15, 20, True,      0b0000_0000_0000_1111_1000_0000_0000_0000),  # noqa: E241
+     (15, 20, False,     0b1111_1111_1111_0000_0111_1111_1111_1111),  # noqa: E241
+     ]
+)
 def test_get_bitmask(lower, upper, allow, expected):
     """
     Test that the correct bitmask is created.
 
     Explanation of test cases 3 to 8 (first two are obvious):
     3. Allow between 0 and 15, exclude the 15.5 point because we can't allow
        points like 15.6 and they share a range. Therefore, enable bits 1
```

