# Comparing `tmp/pymwp-0.2.1.tar.gz` & `tmp/pymwp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymwp-0.2.1.tar", last modified: Tue Oct  4 16:38:51 2022, max compression
+gzip compressed data, was "pymwp-0.3.0.tar", last modified: Sat Apr  8 21:13:10 2023, max compression
```

## Comparing `pymwp-0.2.1.tar` & `pymwp-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:38:51.240587 pymwp-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)    17837 2022-10-04 16:38:24.000000 pymwp-0.2.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-04 16:38:24.000000 pymwp-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-10-04 16:38:51.240587 pymwp-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-10-04 16:38:24.000000 pymwp-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:38:51.240587 pymwp-0.2.1/pymwp/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18948 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    11277 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/choice.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11916 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/delta_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/file_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     7858 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/monomial.py
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    18152 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (121)    11348 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7142 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/relation_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-10-04 16:38:24.000000 pymwp-0.2.1/pymwp/semiring.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:38:51.240587 pymwp-0.2.1/pymwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-04 16:38:51.000000 pymwp-0.2.1/pymwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-04 16:38:24.000000 pymwp-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 16:38:51.240587 pymwp-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-04 16:38:24.000000 pymwp-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:38:51.240587 pymwp-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 16:38:51.240587 pymwp-0.2.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)    19851 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/mocks/ast_mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4794 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_delta_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     6668 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_monomial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-10-04 16:38:24.000000 pymwp-0.2.1/tests/test_relation_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 21:12:38.000000 pymwp-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-08 21:12:38.000000 pymwp-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-08 21:13:10.935534 pymwp-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-08 21:12:38.000000 pymwp-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.927534 pymwp-0.3.0/pymwp/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/delta_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/relation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/semiring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.931534 pymwp-0.3.0/pymwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-08 21:12:38.000000 pymwp-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:13:10.935534 pymwp-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-08 21:12:38.000000 pymwp-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/mocks/ast_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_delta_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_relation_list.py
```

### Comparing `pymwp-0.2.1/PKG-INFO` & `pymwp-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.2.1
+Version: 0.3.0
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
+License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENCE.md
+License-File: LICENSE
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/statycc/pymwp/branch/main/graph/badge.svg?token=4v3zRbkAjM)](https://codecov.io/gh/statycc/pymwp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymwp)](https://pypi.org/project/pymwp/)
 [![PyPI](https://img.shields.io/pypi/v/pymwp)](https://pypi.org/project/pymwp/)
@@ -36,24 +38,26 @@
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
-pymwp is a tool for automatically performing static analysis on programs written in C, inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
+pymwp is a tool for automatically performing static analysis on programs written in C.
+It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
-You can run our [many examples](https://statycc.github.io/pymwp/examples/) on-line [in our demo](https://statycc.github.io/pymwp/demo/) before [installing it](https://statycc.github.io/pymwp/), consult our list of [supported C language features](https://statycc.github.io/pymwp/features/),
-or review latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting metrics. 
+Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
+For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
+See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
-Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation of our modules, an [on-line demo](https://statycc.github.io/pymwp/demo/) as well as a presentation of [our examples](https://statycc.github.io/pymwp/examples/).
+Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
 <!--include-start-->
 
 ## Installation
 
 Install the latest release from PyPI
 
@@ -72,15 +76,15 @@
 For all available options and help, run:
 
 ```
 pymwp --help
 ```
 
 
-You can also use pymwp in a Python script:
+You can also use pymwp by importing it in a Python script:
 
 ```python
 from pymwp import Polynomial
 from pymwp.matrix import identity_matrix, show
 
 matrix = identity_matrix(3)
 matrix[0][1] = Polynomial('m')
```

### Comparing `pymwp-0.2.1/README.md` & `pymwp-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,26 @@
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
-pymwp is a tool for automatically performing static analysis on programs written in C, inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
+pymwp is a tool for automatically performing static analysis on programs written in C.
+It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
-You can run our [many examples](https://statycc.github.io/pymwp/examples/) on-line [in our demo](https://statycc.github.io/pymwp/demo/) before [installing it](https://statycc.github.io/pymwp/), consult our list of [supported C language features](https://statycc.github.io/pymwp/features/),
-or review latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting metrics. 
+Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
+For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
+See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
-Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation of our modules, an [on-line demo](https://statycc.github.io/pymwp/demo/) as well as a presentation of [our examples](https://statycc.github.io/pymwp/examples/).
+Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
 <!--include-start-->
 
 ## Installation
 
 Install the latest release from PyPI
 
@@ -45,15 +47,15 @@
 For all available options and help, run:
 
 ```
 pymwp --help
 ```
 
 
-You can also use pymwp in a Python script:
+You can also use pymwp by importing it in a Python script:
 
 ```python
 from pymwp import Polynomial
 from pymwp.matrix import identity_matrix, show
 
 matrix = identity_matrix(3)
 matrix[0][1] = Polynomial('m')
```

### Comparing `pymwp-0.2.1/pymwp/__init__.py` & `pymwp-0.3.0/pymwp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 """
 pymwp: implementation of MWP analysis on C code in Python.
 """
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
-__license__ = "CC BY-NC 4.0"
-__version__ = "0.2.1"
+__license__ = "GPLv3"
+__version__ = "0.3.0"
 
 from pymwp.parser import Parser
 from pymwp.delta_graphs import DeltaGraph
 from pymwp.choice import Choices
 from pymwp.relation_list import RelationList
 from pymwp.relation import Relation
 from pymwp.polynomial import Polynomial
 from pymwp.monomial import Monomial
+from pymwp.result import Result
 from pymwp.analysis import Analysis
+
```

### Comparing `pymwp-0.2.1/pymwp/__main__.py` & `pymwp-0.3.0/pymwp/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 """
 
 import argparse
 import logging
 import sys
 from typing import List, Optional
 
-from pymwp import Parser, Analysis, __version__, __title__ as pymwp
-from .file_io import default_file_out
+from pymwp import Parser, Result, Analysis, __version__, __title__ as pymwp
+from .file_io import default_file_out, loc
 
 
 def main():
     """Implementation of MWP analysis on C code in Python."""
     parser = argparse.ArgumentParser(prog=pymwp, description=main.__doc__)
     args = __parse_args(parser)
 
@@ -36,26 +36,32 @@
         parser.print_help()
         sys.exit(1)
 
     # setup logger
     log_level = logging.FATAL - (0 if args.silent else 40)
     __setup_logger(log_level, args.logfile)
 
+    # capture results
+    result = Result()
+
     # get parser args then get AST
     parser_kwargs = {'use_cpp': not args.no_cpp}
-    # these options only apply when use_cpp is set to True
+    # these options apply only when use_cpp is True
     if not args.no_cpp:
         parser_kwargs['cpp_path'] = args.cpp_path
         parser_kwargs['cpp_args'] = args.cpp_args
     c_headers = args.headers.split(',') if args.headers else None
     ast = Parser.parse(args.input_file, c_headers, **(parser_kwargs or {}))
+    result.program.program_path = args.input_file
+    result.program.n_lines = loc(args.input_file)
 
     # run analysis
     Analysis.run(
         ast=ast,
+        result=result,
         file_out=args.out or default_file_out(args.input_file),
         no_save=args.no_save,
         no_eval=args.no_eval,
         fin=args.fin
     )
```

### Comparing `pymwp-0.2.1/pymwp/analysis.py` & `pymwp-0.3.0/pymwp/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 # noinspection DuplicatedCode
 import logging
-import time
 from typing import List, Tuple, Optional, Union, Dict
 
 from .file_io import save_relation
 # noinspection PyPep8Naming
 from .parser import Parser as pr
-from pymwp import DeltaGraph, Monomial, Polynomial, Relation, RelationList
+from pymwp import DeltaGraph, Monomial, Polynomial, RelationList, Result
+from pymwp.result import FUNC_RESULT
 
 logger = logging.getLogger(__name__)
 
 
 class Analysis:
     """MWP analysis implementation."""
 
     @staticmethod
-    def run(ast: pr.AST, **kwargs) \
-            -> Union[Dict, Tuple[Relation, List[List[int]], bool]]:
+    def run(ast: pr.AST, result: Result = None, **kwargs) \
+            -> Union[Dict[str, FUNC_RESULT], FUNC_RESULT]:
         """Run MWP analysis on specified input file.
 
         Arguments:
             ast: parsed C source code AST
+            result: (optional) result object
 
         Returns:
-              - Computed relation,
-              - list of non-infinity choices
-              - infinite/not infinite (boolean flag)
+            Computed relation, list of non-infinity choices, and
+                infinite/not infinite (boolean flag)
         """
         file_out: str = kwargs['file_out'] if 'file_out' in kwargs else None
         save: bool = 'no_save' not in kwargs or kwargs['no_save'] is False
         stop_early: bool = 'fin' not in kwargs or kwargs['fin'] is False
         skip_eval: bool = 'no_eval' in kwargs and kwargs['no_eval'] is True
+        result__: Result = result or Result()
 
-        logger.debug("starting analysis")
-        start_time = time.time_ns()
-        single_function = len(ast.ext) == 1
-        result, function_name = {}, ''
-        functions = [f for f in ast if pr.is_func(f)]
-
-        if len(functions) == 0:
-            logger.warning("C file contains no analyzable functions")
-
-        for ast_ext in functions:
+        logger.debug("started analysis")
+        result__.on_start()
+        for ast_ext in [f for f in ast if pr.is_func(f)]:
             choices = [0, 1, 2]
             index, combinations = 0, []
             function_name = ast_ext.decl.name
             function_body = ast_ext.body
             args = ast_ext.decl.type.args
             variables = Analysis.find_variables(function_body, args)
             logger.debug(f"variables of {function_name}: {variables}")
@@ -72,40 +66,29 @@
 
             # the evaluation is infinite when either of these conditions holds:
             infinite = delta_infty or (
                     relations.first.variables and index > 0 and
                     evaluated and not combinations.valid)
 
             # record and display results
+            outcome = function_name,
             if infinite and stop_early:
-                result[function_name] = None, None, True
-                logger.info(f'RESULT: {function_name} is infinite')
+                outcome += (None, None, True)
             elif infinite:
-                result[function_name] = relations.first, [], True
-                logger.info(f'\nMATRIX{relations}')
-                logger.info(f'RESULT: {function_name} is infinite')
+                outcome += (relations.first, None, True)
             else:
-                result[function_name] = relations.first, combinations, False
-                logger.info(f'\nMATRIX{relations}')
-                if not evaluated:
-                    logger.info('Skipped evaluation')
-                else:
-                    logger.info(f'CHOICES: {combinations.valid}')
-
-        # save result to file unless explicitly disabled
-        if save:
-            save_relation(file_out, result)
+                outcome += (relations.first, combinations, False)
+            result__.add_relation(*outcome)
 
-        end_time = time.time_ns()
-        dur_s = round((end_time - start_time) / 1e9, 1)
-        dur_ms = int((end_time - start_time) / 1e6)
-        logger.info(f'Total time: {dur_s} s ({dur_ms} ms)')
+        result__.on_end()
+        result__.log_result()
 
-        # return results to caller
-        return result[function_name] if single_function else result
+        if save:
+            save_relation(file_out, result__.relations)
+        return result__.get_result()
 
     @staticmethod
     def find_variables(
             function_body: pr.Compound, param_list: Optional[pr.ParamList]
     ) -> List[str]:
         """Finds all local variable declarations in function body and
         parameter list.
@@ -261,22 +244,22 @@
         rel_list.replace_column(vector, x.name)
 
         return index, rel_list, False
 
     @staticmethod
     def constant(index: int, variable_name: str) \
             -> Tuple[int, RelationList, bool]:
-        """Analyze a constant assignment of form: x = c where x is some
+        """Analyze a constant assignment of form `x = c` where x is some
         variable and c is constant.
 
-        From MWP paper:
+        !!! quote "From MWP paper:"
 
-        > To deal with constants, just replace the program’s constants by
-          variables and regard the replaced constants as input to these
-          variables.
+            To deal with constants, just replace the program’s constants by
+            variables and regard the replaced constants as input to these
+            variables.
 
         Arguments:
             index: delta index
             variable_name: name of variable to which constant is being assigned
 
         Returns:
             Updated index value, relation list, and an exit flag.
@@ -294,16 +277,14 @@
             node: unary operator node
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
         logger.debug('Computing Relation (third case / unary)')
         var_name = node.lvalue.name
-        # list_var = None  # list_var(exp)
-        # variables = [var_name] + list_var
         variables = [var_name]
         return index, RelationList.identity(variables), False
 
     @staticmethod
     def if_(index: int, node: pr.If, dg: DeltaGraph) \
             -> Tuple[int, RelationList, bool]:
         """Analyze an if statement.
@@ -394,15 +375,14 @@
             if exit_:
                 return index, rel_list, exit_
             relations.composition(rel_list)
 
         logger.debug('while loop fixpoint')
         relations.fixpoint()
         relations.while_correction(dg)
-
         dg.fusion()
 
         exit_ = False
         if 0 in dg.graph_dict:
             if dg.graph_dict[0] == {(): {}}:
                 logger.info('delta_graphs: infinite -> Exit now')
                 exit_ = True
```

### Comparing `pymwp-0.2.1/pymwp/choice.py` & `pymwp-0.3.0/pymwp/choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         This works in two steps: 1. simplify delta sequences 2. build
         choice vectors.
 
         Arguments:
             choices: list of valid choices for one index, e.g. [0,1,2]
             index: the length of the vector, e.g. 10. This is the same as
-               number of assignments in the analyzed function.
+                number of assignments in the analyzed function.
             inf: set of deltas that lead to infinity
 
         Returns:
             Generated choice object.
         """
         # simplify the set of infinities
         sequences = Choices.simplify(choices, inf)
```

### Comparing `pymwp-0.2.1/pymwp/delta_graphs.py` & `pymwp-0.3.0/pymwp/delta_graphs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,221 +1,237 @@
 from __future__ import annotations
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
-from .monomial import Monomial
+from .monomial import Monomial, DELTA
+
+NODE = Tuple[DELTA, ...]
+"""Graph node type is a variable-length tuple of deltas."""
 
 
 class DeltaGraph:
     """
-    DeltaGraph is a dictionary representing a weighted graph of tuple of
-    deltas (also referenced here as monomial_list aka: a monomial without
-    its scalar).
-
-    We use tuple here instead of list because we want them to be hashable (
-    as key in dictionary).
-
-    We will often refer to tuple of deltas as simple node. But a node with
-    length!
+    Delta Graph is a dictionary representing a weighted graph of tuples of
+    deltas (also referenced here as a _monomial_list_, a
+    [`Monomials`](monomial.md) without its scalar). We will often refer to
+    tuple of deltas as simple node, but a node with length!
 
     Nodes are "sorted" by this length in order to be compared by chunks of
     same size.
 
     Weight of edge represents the index where the nodes differ.
 
-    example:
+    We use tuple because we want them to be hashable (as key in dictionary).
+
+
+    Example:
 
     ```
-                                 ↓
-        n1 = ( (0,1) , (0,2) , (0,3), (0,4) )
-        n2 = ( (0,1) , (0,2) , (1,3), (0,4) )
+                             ↓
+    n1 = ( (0,1) , (0,2) , (0,3), (0,4) )
+    n2 = ( (0,1) , (0,2) , (1,3), (0,4) )
     ```
 
     in our graph will have:
 
     ```
-        n1 <---- 3 ----> n2
+    n1 <---- 3 ----> n2
     ```
 
     or
 
     ```python
     size = 4   ↓
 
     graph_dict[4][n1][n2] = 3
     ```
 
-    Note: yes it also means it's symetric :
+    The graph is symmetric:
 
     ```python
     graph_dict[4][n2][n1] = 3
     ```
 
     This representation will help us simplify the evaluation by
     removing redundant/irrelevant choices/paths.
     """
 
-    def __init__(self, monomials: Optional[List[Monomial]] = None):
-        """Create DeltaGraph
-            fill with empty dictionary all monomial_list of monomials given
+    def __init__(
+            self, *init_nodes: Optional[Union[Monomial, NODE]], degree: int = 3
+    ):
+        """Creates a Delta Graph.
+
+        Fills a dictionary with nodes of all given initial nodes.
+
+        Example:
+
+        Create an empty delta graph
+
+        ```python
+        dg = DeltaGraph()
+        ```
+
+        Create delta graph with some initial nodes from monomials.
+
+        ```python
+        dg = DeltaGraph(mono1, mono2)
+        ```
+
+        Arguments:
+            init_nodes: initial list of monomials or nodes (optional).
+            degree: degree of a full node [default: 3].
         """
+        self.degree = degree
         self.graph_dict = {}
-        if monomials:
-            for ml in monomials:
-                self.import_monomial(ml)
+        if init_nodes:
+            for node in init_nodes:
+                if isinstance(node, Monomial):
+                    self.from_monomial(node)
+                if isinstance(node, Tuple):
+                    self.insert_node(node)
+
+    def __str__(self):
+        return "".join(
+            [f'{n} {self.graph_dict[n]}\n{26 * "--"}\n' for n in
+             self.graph_dict])
 
-    def import_monomial(self, m: Monomial) -> None:
-        """import monomial
+    def from_monomial(self, monomial: Monomial) -> None:
+        """Add monomial's deltas to the delta graph.
 
         Arguments:
-            m: monomial
+            monomial: monomial
         """
-        self.insert_tuple(tuple(m.deltas))
+        self.insert_node(tuple(monomial.deltas))
 
-    def add_edge(self, node1, node2, label) -> None:
+    def insert_edge(self, node1: NODE, node2: NODE, label: int) -> None:
         """Add an edge of label `label` between `node1` and `node2`
         If one node does not exist, it's created
 
-        Symmetry is also added in the graph
-
-        Note:
-            node2 should always exist if add_edge is always called
-            from insert_tuple
+        Symmetry is also added in the graph.
 
         Arguments:
             node1: first node
             node2: second node
             label: label over the edge
 
         """
-        # add_edge is called only when len(node1) = len(node2)
         size = len(node1)
         if node1 not in self.graph_dict[size]:
             self.graph_dict[size][node1] = {}
 
-        # self.graph_dict[size][node1]=[(node2,label)]
         self.graph_dict[size][node1][node2] = label
 
-        # If add_edge is always called from insert_tuple
-        # node2 should always be in self.graph_dict[size]
+        # node2 should always exist if add_edge is always called
+        # from insert_tuple
         if node2 not in self.graph_dict[size]:
             self.graph_dict[size][node2] = {}
         self.graph_dict[size][node2][node1] = label
 
-    # monomial_list : Tuple[Tuple[int,int]]
-    def insert_tuple(self, monomial_list, simplification=False) -> None:
-        """Insert tuple in the graph
-
-        it may exists cases where we need to perform simplification
-        over monomials, this is why we added simplification boolean
-
-        if monomial_list is already in the graph do nothing
-        else compare it with all monomial_list of same size with
-        mono_diff
-
-        <!--
-        Note:
-            Is it possible that we've already computed that diff in
-            the other way ? (symmetry)
-            Answer:
-                AFA it's called now, NO
-        -->
+    def insert_node(self, node: NODE) -> None:
+        """Insert a node into the graph.
+
+        If a node is already in the graph do nothing.
+        Else compare it with all nodes of same size with `node_diff`.
 
         Arguments:
-            monomial_list: tuple to insert in the graph
-            simplification: boolean to inform if simplification is
-                necessary
+            node: tuple to insert in the graph
         """
-        n = len(monomial_list)
-
-        if n not in self.graph_dict:
-            self.graph_dict[n] = {}
-            self.graph_dict[n][monomial_list] = {}
+        size = len(node)
+        # Is it possible that we've already computed that diff in
+        # the other way ? (symmetry)
+        # Answer: AFA it's called now, NO
+        if size not in self.graph_dict:
+            self.graph_dict[size] = {}
+            self.graph_dict[size][node] = {}
         else:
-            # if simplification:
-            # Add here the simplification
-
+            # TODO: Case may exist where we need to perform simplification
+            #    over monomials -> Add here the simplification
             inserted = False
-            if monomial_list not in self.graph_dict[n]:
-                for listi in list(self.graph_dict[n]):
-                    # Already tested when listi[listi][monomial_list] exists
+            if node not in self.graph_dict[size]:
+                for node2 in list(self.graph_dict[size].keys()):
+                    # Already tested when node2[node2][monomial_list] exists
                     # FIXME is it possible ?
-                    # if monomial_list not in listi[listi]:
-                    (diff, i) = self.mono_diff(monomial_list, listi)
+                    # if monomial_list not in node2[node2]:
+                    diff, i = self.node_diff(node, node2)
                     if diff:
                         inserted = True
-                        self.add_edge(monomial_list, listi, i)
+                        self.insert_edge(node, node2, i)
                 if not inserted:
-                    self.graph_dict[n][monomial_list] = {}
+                    self.graph_dict[size][node] = {}
 
     @staticmethod
-    def remove_index(ml: List[Monomial], index: int) -> Tuple:
-        """Remove delta with given index
+    def remove_index(node: NODE, index: int) -> NODE:
+        """Remove delta with given index.
+
+        Example:
+
+        ```
+        remove index 4:
+        ((0, 2), (1, 3), (2, 4))  ->  ((0, 2), (1, 3))
+        ```
+
         Arguments:
-            ml: monomial_list as tuple
+            node: monomial list
             index: index to remove
 
         Returns:
-            a new tuple without detlas with index `index`
+            a new tuple without deltas with index `index`
         """
-        return tuple(filter(lambda x: x[1] != index, list(ml)))
+        return tuple(filter(lambda x: x[1] != index, node))
 
-    # Remove tuple from graph and related edges
-    #: Tuple[Tuple[int,int]]
-    def remove_tuple(self, ml: List[Monomial], index: int):
-        """Remove given tuple and neighbors connected with same label
+    def remove_node(self, node: NODE, index: int) -> None:
+        """Remove given node and neighbors connected with same label.
 
-        Removes also edge/labels connected to that node
-        (which no longer exists)
+        Also removes edges/labels connected to the node (they no longer exist).
         """
-        size = len(ml)
+        size = len(node)
 
         # Keep track of neighbors before removing node
-        neighbos = list(self.graph_dict[size][ml])
+        neighbors = list(self.graph_dict[size][node])
 
         # Remove node
-        del self.graph_dict[size][ml]
+        del self.graph_dict[size][node]
 
         # For each neighbour
-        for ml_nb in neighbos:
-            if ml_nb in self.graph_dict[size]:
-                labl = self.graph_dict[size][ml_nb][ml]
+        for neighbor in neighbors:
+            if neighbor in self.graph_dict[size]:
+                label = self.graph_dict[size][neighbor][node]
                 # If same label then recursively remove neighbour
-                if labl == index:
-                    self.remove_tuple(ml_nb, index)
+                if label == index:
+                    self.remove_node(neighbor, index)
                 # if not just remove the edge
                 else:
-                    del self.graph_dict[size][ml_nb][ml]
+                    del self.graph_dict[size][neighbor][node]
 
     @staticmethod
-    def mono_diff(
-            ml1: List[Monomial], ml2: List[Monomial],
-            index: Optional[int] = None
-    ) -> Tuple[bool, Union[int, Monomial]]:
-        """Compares two nodes
-
-        Compares two lists of monomials (of the same length) and returns (
-        diff, i) where diff is True if and only if both lists differ only on
-        one element regarding the same index and i is the index of the
-        corresponding delta.
+    def node_diff(
+            node1: NODE, node2: NODE, index: Optional[int] = None
+    ) -> Tuple[bool, int]:
+        """Compares two nodes of the same length.
+
+        The return value is a tuple representing the result of comparison
+        (boolean) and an index.
+
+        The result is True, if and only if both lists differ only on one
+        element regarding the same index. The second return value is the index
+        of the corresponding delta.
 
         Arguments:
-            ml1: first monomial_list
-            ml2: second monomial_list
+            node1: first monomial list
+            node2: second monomial list
             index: index with to check number of diff
 
         Returns:
-            Tuple (diff, i)
             diff: boolean True if the lists differ of one element
             i: the index of the delta which differs
         """
         diff_found = False
         i = 0
-        while i < len(ml1):
-            if ml1[i] not in ml2:
-                i1 = ml1[i][1]
+        while i < len(node1):
+            if node1[i] not in node2:
+                i1 = node1[i][1]
                 # We've already recorded one so two diff
                 if diff_found:
                     return False, i1
                 # Case recursive call, we've not found yet
                 # But index is defined by arguments
                 if index is not None:
                     # If the diff has different index than expected
@@ -224,171 +240,92 @@
                     else:
                         # We've found one but still searching more
                         diff_found = True
                 # Found first diff without init of index
                 else:
                     # Search in other monomial if it has only one diff
                     # Of same index `i1`
-                    (diff, _) = DeltaGraph.mono_diff(ml2, ml1, i1)
+                    (diff, _) = DeltaGraph.node_diff(node2, node1, i1)
                     if diff:
                         index = i1
                         # Continue searching see if there are more diff
                         diff_found = True
                     else:
                         return False, i1
             i += 1
         return diff_found, index
 
-    def is_full(self, n: int, mono: Monomial, index: int,
-                max_choices: Optional[int] = 3) -> bool:
-        """Check for cliques of same label
+    def is_full(self, node: NODE, size: int, index: int) -> bool:
+        """Check for cliques of same label.
 
-        example :
+        Example:
 
         ```Python
-        m3 = ((0, 1), (2, 2), (0, 3))
-        m4 = ((0, 1), (2, 2), (1, 3))
-        m5 = ((0, 1), (2, 2), (2, 3))
+        n3 = ((0, 1), (2, 2), (0, 3))
+        n4 = ((0, 1), (2, 2), (1, 3))
+        n5 = ((0, 1), (2, 2), (2, 3))
 
-        mono = m4
+        node = n4
+        size = 3
         index = 3
-        max_choices = 3
-
-        # m3 --3-- m4
-        #   \\       |
-        #    \\      |
-        #     3     3
-        #      \\    |
-        #       \\   |
-        #         m5
+        degree = 3
 
+        '''
+        n3 -- 3 -- n4
+         ⟍         |
+            3       3
+              ⟍    |
+                ⟍  |
+                  n5
+        '''
         return True
         ```
 
         Arguments:
-            n: size of nodes or "level"
-            mono: around that node
-            index: index with to find clique
-            max_choices: optional
+            node: check for clique around that graph node
+            size: size of nodes or graph "level"
+            index: index where to find clique
 
         Returns:
             True if there is a clique
         """
-        i = 0
-        for mono2 in self.graph_dict[n][mono]:
-            j = self.graph_dict[n][mono][mono2]
-            if j == index:
-                i = i + 1
-                if i == max_choices - 1:
-                    return True
-        return False
+        src = self.graph_dict[size][node]
+        adjacent = sum([1 for n2 in src if src[n2] == index])
+        return adjacent == (self.degree - 1)
 
-    @staticmethod
-    def get_indexes(lm: List[Monomial]) -> List[int]:
-        """Given a list of monomials, get only its indices
+    def fusion(self) -> None:
+        """Eliminates cliques of same label in a delta graph.
 
-        Arguments:
-            lm: list of monomials
+        Example:
 
-        Returns:
-            list of indices.
-        """
-        _, listi = zip(*lm)
-        return listi
-
-    # def fusion(self, list_of_max, max_i=None):
-    def fusion(self, max_i: Optional[int] = 3) -> None:
-        """Eliminate clique of same label in delta_graph
-
-        example :
-        ```
+        ```python
         m1 = ((0, 1), (0, 2))
         m2 = ((0, 1), (1, 2))
         m3 = ((0, 1), (2, 2), (0, 3))
         m4 = ((0, 1), (2, 2), (1, 3))
         m5 = ((0, 1), (2, 2), (2, 3))
-        ```
 
-
-        with list_of_max = [3,3,3,3]
-        look for cliques of size 3 for each index
-
-        delta graph :
-
-        ```
-         m1 --2-- m2
-         m3 --3-- m4
-           \\       |
-            \\      |
-             3     3
-              \\    |
-               \\   |
-                 m5
+        '''
+          delta graph:
+          m1 -- 2 -- m2
+          m3 -- 3 -- m4
+           ⟍         |
+              3      3
+                ⟍    |
+                  ⟍  |
+                    m5
+
+        Looks for cliques (size default 3) at each index.
+        => Graph will simplify to: ((0,1)).
+        '''
         ```
-
-        will simplify to :
-
-        ```
-        m0 = ((0,1))
-        ```
-
-        Arguments:
-            max_i: size of clique we want to eliminate regarding to index
-                of deltas
-
-        Returns:
-            eliminates corresponding clique in the delta_graph
         """
-        # Start from the longest monomial list to the shortest
-        for n in sorted(self.graph_dict, reverse=True):
-            # For all monomial list of size n
-            for lm in list(self.graph_dict[n]):
-                # For all indexes in deltas of that monomial
-                for index in self.get_indexes(lm):
+        # Start from the longest node to the shortest
+        for size in sorted(self.graph_dict, reverse=True):
+            for node in list(self.graph_dict[size]):
+                # For all indexes in deltas of that node
+                for index in (list(zip(*node))[1]):
                     # Check if it's full of same index
-                    if lm in self.graph_dict[n] and self.is_full(
-                            n, lm, index, max_i):
-                        self.remove_tuple(lm, index)
-                        self.insert_tuple(DeltaGraph.remove_index(lm, index))
-
-    @staticmethod
-    def combination_matches_tuple(
-            c: List, lm: Tuple[Tuple[int, int]]
-    ) -> bool:
-        """(description)
-
-        Arguments:
-            c: list
-            lm: tuple
-
-        Returns:
-            true/false
-        """
-        for t in lm:
-            if c[t[1]] != t[0]:
-                return False
-        return True
-
-    def contains_combination(self, combination: List) -> bool:
-        """If we have (0,1) in our graph remove all combinations where
-        combinations[1] = 0 then for size 2 (0,2)(1,3) remove all combinations
-        where we have combinations[2] = 0 and combinations[3] = 1 etc…
-
-        Arguments:
-            combination:  list
-
-        Returns:
-            true/false
-        """
-        for n in sorted(self.graph_dict):
-            # For all monomial list of size n starting with n = 1
-            for lm in list(self.graph_dict[n].keys()):
-                if DeltaGraph.combination_matches_tuple(combination, lm):
-                    return True
-        return False
-
-    def __str__(self):
-        res = ""
-        for n in self.graph_dict:
-            res += str(n) + ":" + \
-                   str(self.graph_dict[n]) + "\n" + 26 * "-- " + "\n"
-        return res
+                    if node in self.graph_dict[size] and \
+                            self.is_full(node, size, index):
+                        self.remove_node(node, index)
+                        self.insert_node(DeltaGraph.remove_index(node, index))
```

### Comparing `pymwp-0.2.1/pymwp/file_io.py` & `pymwp-0.3.0/pymwp/file_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from .matrix import decode
 from .relation import Relation
 
 logger = logging.getLogger(__name__)
 RESULT_TYPE = Tuple[Optional[Relation], Optional[Choices], bool]
 
 
+def loc(input_file: str) -> int:
+    """Get number of lines is a file"""
+    with open(input_file, 'r') as fp:
+        return len(fp.readlines())
+
+
 def default_file_out(input_file: str) -> str:
     """Generates default output file.
 
     Arguments:
         input_file: input filename (with or without path)
 
     Returns:
@@ -48,15 +54,14 @@
                 - `[2]`: `True` when function does not have polynomial bounds
     """
 
     file_content = {}
 
     for function_name, result in analysis_result.items():
         relation, choices, infinity = result
-
         file_content[function_name] = {
             "relation": relation.to_dict() if relation else None,
             "choices": choices.valid if choices else None,
             "infinity": infinity
         }
 
     # ensure directory path exists
```

### Comparing `pymwp-0.2.1/pymwp/matrix.py` & `pymwp-0.3.0/pymwp/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,18 +224,19 @@
     # ['  +m', '  +o', '  +o']
     # ['  +o', '  +m', '  +o']
     # ['  +o', '  +o', '  +m']
     ```
 
     Arguments:
         matrix: the matrix to display.
-        **kwargs: keyword arguments
 
-            - `prefix` (`str`): display some text before displaying matrix
-            - `postfix` (`str`): display some text after displaying matrix
+    Kwargs:
+
+    - `prefix` (`str`): display some text before displaying matrix
+    - `postfix` (`str`): display some text after displaying matrix
 
     Raises:
         TypeError: If the matrix is not iterable (type list of lists)
     """
     if 'prefix' in kwargs:
         print(kwargs['prefix'])
     for row in matrix:
```

### Comparing `pymwp-0.2.1/pymwp/monomial.py` & `pymwp-0.3.0/pymwp/monomial.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     A monomial is a pair made of:
 
     1. `scalar` - a value in the semi-ring
     2. a sorted list of `deltas`, where an index occurs at most once.
 
     Deltas are coded as pairs $(i,j)$ with:
 
-     - $i$ the value and
-     - $j$ the index in the domain (infinite product)
+    - $i$ the value and
+    - $j$ the index in the domain (infinite product)
 
     We will have that $(i,j)$ will be equal to the unit of the semi-ring
     iff the $j^{th}$ input is equal to $i$ (so, the $j^{th}$ choice is $i$).
 
     We will make the assumption that the deltas of delta is sorted
     and no two deltas can have the same index.
     """
@@ -54,15 +54,15 @@
         ```python
         mono = Monomial('w', (0, 0), (1, 1))
         ```
 
         Arguments:
             scalar: monomial scalar
             deltas: list of deltas - either a syntactic list,
-              or sequence of tuples that represent deltas.
+                or sequence of tuples that represent deltas.
         """
         self.deltas = []
         self.scalar = scalar
 
         if deltas is not None:
             if isinstance(deltas, list):
                 Monomial.insert_deltas(self, deltas)
```

### Comparing `pymwp-0.2.1/pymwp/parser.py` & `pymwp-0.3.0/pymwp/parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/pymwp/polynomial.py` & `pymwp-0.3.0/pymwp/polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/pymwp/relation.py` & `pymwp-0.3.0/pymwp/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             dg: DeltaGraph instance
         """
         for i, vector in enumerate(self.matrix):
             for j, poly in enumerate(vector):
                 for mon in poly.list:
                     if mon.scalar == "p" or (mon.scalar == "w" and i == j):
                         mon.scalar = "i"
-                        dg.import_monomial(mon)
+                        dg.from_monomial(mon)
 
     def sum(self, other: Relation) -> Relation:
         """Sum two relations.
 
         Calling this method is equivalent to syntax `relation + relation`.
 
         Arguments:
@@ -336,15 +336,15 @@
         # fill the resized matrix with values from original matrix
         for mj, rj, mi, ri in index_map:
             matrix2[mi][mj] = r2.matrix[ri][rj]
 
         return Relation(extended_vars, matrix1), Relation(extended_vars,
                                                           matrix2)
 
-    def eval(self, choices: List[int], index: int):
+    def eval(self, choices: List[int], index: int) -> Choices:
         """Eval experiment: returns a choice object."""
 
         infinity_deltas = set()
 
         # get all choices leading to infinity
         for row in self.matrix:
             for poly in row:
```

### Comparing `pymwp-0.2.1/pymwp/relation_list.py` & `pymwp-0.3.0/pymwp/relation_list.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/pymwp/semiring.py` & `pymwp-0.3.0/pymwp/semiring.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/pymwp.egg-info/PKG-INFO` & `pymwp-0.3.0/pymwp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.2.1
+Version: 0.3.0
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
+License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENCE.md
+License-File: LICENSE
 
 # pymwp: MWP analysis in Python
 
 [![build](https://github.com/statycc/pymwp/actions/workflows/build.yaml/badge.svg)](https://github.com/statycc/pymwp/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/statycc/pymwp/branch/main/graph/badge.svg?token=4v3zRbkAjM)](https://codecov.io/gh/statycc/pymwp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymwp)](https://pypi.org/project/pymwp/)
 [![PyPI](https://img.shields.io/pypi/v/pymwp)](https://pypi.org/project/pymwp/)
@@ -36,24 +38,26 @@
     do not remove start and end comments (e.g. "include-start", "include-end").
     They are markers for what to include in the docs, but feel free to edit 
     the inner content.
 -->
 
 <!--desc-start-->
 
-pymwp is a tool for automatically performing static analysis on programs written in C, inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
+pymwp is a tool for automatically performing static analysis on programs written in C.
+It is inspired by [_"A Flow Calculus of mwp-Bounds for Complexity Analysis"_](https://doi.org/10.1145/1555746.1555752).
 It analyzes resource usage and determines if a program's variables growth rates are no more than polynomially related to their inputs sizes.
-You can run our [many examples](https://statycc.github.io/pymwp/examples/) on-line [in our demo](https://statycc.github.io/pymwp/demo/) before [installing it](https://statycc.github.io/pymwp/), consult our list of [supported C language features](https://statycc.github.io/pymwp/features/),
-or review latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting metrics. 
+Try our online [demo](https://statycc.github.io/pymwp/demo/) to see it action.
+For more details on usage and behavior, see pymwp [documentation](https://statycc.github.io/pymwp/), particularly [supported C language features](https://statycc.github.io/pymwp/features/).
+See latest [profiling results](https://github.com/statycc/pymwp/releases/tag/profile-latest) for interesting performance metrics. 
 
 <!--desc-end--> 
 
 ## Documentation and Demo
 
-Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation of our modules, an [on-line demo](https://statycc.github.io/pymwp/demo/) as well as a presentation of [our examples](https://statycc.github.io/pymwp/examples/).
+Refer to **[statycc.github.io/pymwp](https://statycc.github.io/pymwp/)** for a documentation, an [online demo](https://statycc.github.io/pymwp/demo/), and a presentation of [examples](https://statycc.github.io/pymwp/examples/).
 
 <!--include-start-->
 
 ## Installation
 
 Install the latest release from PyPI
 
@@ -72,15 +76,15 @@
 For all available options and help, run:
 
 ```
 pymwp --help
 ```
 
 
-You can also use pymwp in a Python script:
+You can also use pymwp by importing it in a Python script:
 
 ```python
 from pymwp import Polynomial
 from pymwp.matrix import identity_matrix, show
 
 matrix = identity_matrix(3)
 matrix[0][1] = Polynomial('m')
```

### Comparing `pymwp-0.2.1/pymwp.egg-info/SOURCES.txt` & `pymwp-0.3.0/pymwp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENCE.md
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pymwp/__init__.py
 pymwp/__main__.py
 pymwp/analysis.py
@@ -12,14 +12,15 @@
 pymwp/file_io.py
 pymwp/matrix.py
 pymwp/monomial.py
 pymwp/parser.py
 pymwp/polynomial.py
 pymwp/relation.py
 pymwp/relation_list.py
+pymwp/result.py
 pymwp/semiring.py
 pymwp.egg-info/PKG-INFO
 pymwp.egg-info/SOURCES.txt
 pymwp.egg-info/dependency_links.txt
 pymwp.egg-info/entry_points.txt
 pymwp.egg-info/requires.txt
 pymwp.egg-info/top_level.txt
```

### Comparing `pymwp-0.2.1/setup.py` & `pymwp-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __desc__ = "Implementation of MWP analysis on C code in Python."
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=__title__,
     version=__version__,
     author=__author__,
     author_email='nrusch@augusta.edu',
     packages=['pymwp'],
     entry_points={'console_scripts': ['pymwp = pymwp.__main__:main'], },
+    license='GPLv3',
     description=__desc__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/statycc/pymwp',
     project_urls={
         'Bug Tracker': 'https://github.com/statycc/pymwp/issues',
         'Documentation': 'https://statycc.github.io/pymwp/',
@@ -31,19 +32,20 @@
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
         'Environment :: Console',
         'Typing :: Typed',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
     ],
     python_requires=">=3.7",
     install_requires=[
         'pycparser',
         'pycparser-fake-libc'
     ]
-)
+)
```

### Comparing `pymwp-0.2.1/tests/test_analysis.py` & `pymwp-0.3.0/tests/test_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from pymwp import Analysis, Polynomial
 from .mocks.ast_mocks import \
-    INFINITE_2C, NOT_INFINITE_2C, IF_WO_BRACES, IF_WITH_BRACES, \
-    VARIABLE_IGNORED, BRACES_ISSUES, PARAMS, FUNCTION_CALL, INFINITE_8C
+    INFINITE_2C, INFINITE_8C, NOT_INFINITE_2C, NOT_INFINITE_3C, \
+    IF_WO_BRACES, IF_WITH_BRACES, VARIABLE_IGNORED, BRACES_ISSUES, \
+    PARAMS, FUNCTION_CALL, EMPTY
 
 
 def test_analyze_infinite2():
     """Check analysis result for infinite/infinite_2.c"""
     relation, combinations, infty = Analysis.run(INFINITE_2C, no_save=True)
 
     assert infty  # result should be infinite
     assert combinations is None  # no combinations since it is infinite
     assert relation is None  # no relation since infinite
 
 
+def test_analyze_infinite_8():
+    """Check analysis result for infinite/infinite_8.c"""
+    _, _, infty = Analysis.run(INFINITE_8C, no_save=True)
+    assert infty
+
+
 def test_analyze_non_infinite_2():
     """Check analysis result for not_infinite/notinfinite_2.c"""
     relation, combinations, infty = Analysis.run(NOT_INFINITE_2C, no_save=True)
 
     assert not infty
 
     # match expected choices and variables
@@ -33,18 +40,27 @@
 
     # match *some* deltas from the matrix
     assert str(relation.matrix[0][0].list[0]) == 'w.delta(0,0)'
     assert str(relation.matrix[0][0].list[1]) == 'w.delta(1,0)'
     assert str(relation.matrix[0][0].list[2]) == 'w.delta(2,0)'
 
 
-def test_analyze_infinite_8():
-    """Check analysis result for infinite/infinite_8.c"""
-    _, _, infty = Analysis.run(INFINITE_8C, no_save=True)
-    assert infty
+def test_analyze_non_infinite_3():
+    """Check analysis result for not_infinite/notinfinite_3.c"""
+    _, combinations, infty = Analysis.run(NOT_INFINITE_3C, no_save=True)
+
+    assert not infty
+    assert len(combinations.valid) == 1
+    assert combinations.valid[0] == [[0, 1, 2], [0, 1, 2], [2]]
+
+
+def test_analyze_infinite_to_completion():
+    """Check analysis completion for infinite program"""
+    matrix, _, _ = Analysis.run(INFINITE_2C, no_save=True, fin=True)
+    assert matrix
 
 
 def test_analyze_if_braces_do_not_matter():
     """If...else block with single-statement, with or without curly braces,
      should give the same analysis result."""
     rel_with, choices_with = Analysis.run(IF_WITH_BRACES, no_save=True)[:2]
     rel_wo, choices_wo = Analysis.run(IF_WO_BRACES, no_save=True)[:2]
@@ -124,7 +140,12 @@
     """
     result = Analysis.run(FUNCTION_CALL, no_save=True)
     _, _, f_infty = result['f']
     foo, _, _ = result['foo']
 
     assert not f_infty
     assert set(foo.variables) == {'X1', 'X2'}
+
+
+def test_analysis_handles_empty_program():
+    relation = Analysis.run(EMPTY, no_save=True)
+    assert relation == {}
```

### Comparing `pymwp-0.2.1/tests/test_choices.py` & `pymwp-0.3.0/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_compare.py` & `pymwp-0.3.0/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_delta_graph.py` & `pymwp-0.3.0/tests/test_delta_graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,177 +1,163 @@
-from itertools import product
 from pymwp.delta_graphs import DeltaGraph
-from pytest import raises
+from pymwp.monomial import Monomial
+
+
+def test_insert_mono():
+    m1 = Monomial('m', (0, 0), (0, 1), (1, 2), (2, 3))
+    m2 = Monomial('m', (1, 0), (2, 1))
+    m3 = Monomial('m', (1, 0), (1, 1))
+    dg = DeltaGraph(m1, m2, m3)
+
+    assert ((1, 0), (2, 1)) in dg.graph_dict[2]
+    assert ((1, 0), (1, 1)) in dg.graph_dict[2]
+    assert ((0, 0), (0, 1), (1, 2), (2, 3)) in dg.graph_dict[4]
+
 
 def test_insert_tuple():
     m1 = ((0, 0), (0, 1))
     m2 = ((0, 1), (1, 2))
     m3 = ((0, 2), (1, 3), (2, 4))
     m4 = ((0, 2), (1, 3), (3, 4))
     m5 = ((0, 2), (1, 3), (3, 4))
     m6 = ((0, 2), (2, 3), (2, 4))
 
-    lm = [m1,m2,m3,m4,m5,m6]
+    lm = [m1, m2, m3, m4, m5, m6]
 
     dg = DeltaGraph()
-    # dg.import_monomials(lm)
 
     for m in lm:
-        dg.insert_tuple(m)
-
+        dg.insert_node(m)
 
-    try:
-        assert dg.mono_diff(m3,m4) == (True,4)
-        assert dg.graph_dict[3][m3][m4] == 4
-        assert dg.graph_dict[3][m4][m3] == 4
-        with raises(KeyError):
-            dg.graph_dict[3][m4][m5]
-        assert dg.graph_dict[3][m3][m6] == 3
-    except AssertionError:
-        print(dg.graph_dict[3][m4])
-        raise
+    assert dg.node_diff(m3, m4) == (True, 4)
+    assert dg.graph_dict[3][m3][m4] == 4
+    assert dg.graph_dict[3][m4][m3] == 4
+    assert dg.graph_dict[3][m3][m6] == 3
 
 
 def test_remove_index():
     m1 = ((0, 0), (0, 1))
     m1_ = ((0, 1),)
     m2 = ((0, 1), (1, 2))
     m2_ = ((0, 1),)
     m3 = ((0, 2), (1, 3), (2, 4))
     m3_ = ((0, 2), (1, 3))
     m4 = ((0, 2), (1, 3), (2, 3))
-    # FIXME Should remove all deltas with index 3 ?
     m4_ = ((0, 2),)
 
-    try:
-        assert DeltaGraph.remove_index(m1,0) == m1_
-        assert DeltaGraph.remove_index(m2,2) == m2_
-        assert DeltaGraph.remove_index(m3,4) == m3_
-        assert DeltaGraph.remove_index(m4,3) == m4_
-    except AssertionError:
-        raise
+    assert DeltaGraph.remove_index(m1, 0) == m1_
+    assert DeltaGraph.remove_index(m2, 2) == m2_
+    assert DeltaGraph.remove_index(m3, 4) == m3_
+    assert DeltaGraph.remove_index(m4, 3) == m4_
+
 
 def test_remove_tuple():
     m1 = ((0, 0), (0, 1))
     m2 = ((0, 1), (1, 2))
     m3 = ((0, 2), (1, 3), (2, 4))
     m4 = ((0, 2), (1, 3), (3, 4))
     m5 = ((0, 2), (2, 3), (3, 4))
     m6 = ((0, 2), (2, 3), (2, 4))
 
-    # m1 --1-- m2
+    # m1 --1--m2
     # m3 --4--m4--3-- m5
     #   \           /
     #    \         /
     #     3       4
     #      \     /
     #       \   /
     #         m6
-    lm = [m1,m2,m3,m4,m5,m6]
+    lm = [m1, m2, m3, m4, m5, m6]
 
     dg = DeltaGraph()
 
     for m in lm:
-        dg.insert_tuple(m)
+        dg.insert_node(m)
 
-    try:
+    assert dg.graph_dict[2][m1] == {}
+    assert dg.graph_dict[2][m2] == {}
+    assert dg.graph_dict[3][m3][m4] == 4
+    assert dg.graph_dict[3][m4][m3] == 4
+    assert dg.graph_dict[3][m4][m5] == 3
+    assert dg.graph_dict[3][m3][m6] == 3
+    assert dg.graph_dict[3][m5][m6] == 4
+    assert dg.graph_dict[3][m6][m5] == 4
 
-        assert dg.graph_dict[2][m1] == {}
-        assert dg.graph_dict[2][m2] == {}
+    # Should remove m6 and m5
+    dg.remove_node(m6, 4)
 
-        assert dg.graph_dict[3][m3][m4] == 4
-        assert dg.graph_dict[3][m4][m3] == 4
-        assert dg.graph_dict[3][m4][m5] == 3
-        assert dg.graph_dict[3][m3][m6] == 3
-        assert dg.graph_dict[3][m5][m6] == 4
-        assert dg.graph_dict[3][m6][m5] == 4
-    except AssertionError:
-        raise
+    assert dg.graph_dict[2][m1] == {}
+    assert dg.graph_dict[2][m2] == {}
 
-    # Should remove m6 and m5
-    dg.remove_tuple(m6,4)
+    assert dg.graph_dict[3][m3][m4] == 4
+    assert dg.graph_dict[3][m4][m3] == 4
+    assert m5 not in dg.graph_dict[3]
+    assert m5 not in dg.graph_dict[3][m4]
+    assert m6 not in dg.graph_dict[3]
+    assert m6 not in dg.graph_dict[3][m3]
 
-    try:
-        assert dg.graph_dict[2][m1] == {}
-        assert dg.graph_dict[2][m2] == {}
-
-        assert dg.graph_dict[3][m3][m4] == 4
-        assert dg.graph_dict[3][m4][m3] == 4
-        assert m5 not in dg.graph_dict[3]
-        assert m5 not in dg.graph_dict[3][m4]
-        assert m6 not in dg.graph_dict[3]
-        assert m6 not in dg.graph_dict[3][m3]
-    except AssertionError:
-        raise
 
-def test_mono_diff():
+def test_diff():
     m1 = ((0, 0), (0, 2))
     m2 = ((0, 1), (1, 2))
     m3 = ((0, 2), (1, 3), (2, 4))
     m4 = ((0, 2), (1, 3), (3, 4))
     m5 = ((0, 2), (2, 3), (3, 4))
 
+    assert DeltaGraph.node_diff(m3, m4) == (True, 4)
+    assert DeltaGraph.node_diff(m4, m3) == (True, 4)
+    assert DeltaGraph.node_diff(m1, m2) == (False, 0)
+    assert DeltaGraph.node_diff(m2, m1) == (False, 1)
+    assert DeltaGraph.node_diff(m3, m5) == (False, 3)
 
-    assert DeltaGraph.mono_diff(m3,m4) == (True,4)
-    assert DeltaGraph.mono_diff(m4,m3) == (True,4)
-    assert DeltaGraph.mono_diff(m1,m2) == (False,0)
-    assert DeltaGraph.mono_diff(m2,m1) == (False,1)
-    assert DeltaGraph.mono_diff(m3,m5) == (False,3)
 
-def test_isfull():
+def test_is_full2():
     m1 = ((0, 1), (0, 2))
     m2 = ((0, 1), (1, 2))
+    dg2 = DeltaGraph(m1, m2, degree=2)
+    dg3 = DeltaGraph(m1, m2, degree=3)
+
+    # m1 --2-- m2
+    assert dg3.is_full(m1, 2, 2) is False
+    assert dg3.is_full(m2, 2, 2) is False
+    assert dg2.is_full(m1, 2, 2) is True
+    assert dg2.is_full(m2, 2, 2) is True
+
+
+def test_is_full3():
     m3 = ((0, 1), (2, 2), (0, 3))
     m4 = ((0, 1), (2, 2), (1, 3))
     m5 = ((0, 1), (2, 2), (2, 3))
+    dg = DeltaGraph(m3, m4, m5, degree=3)
 
-    # m1 --2-- m2
     # m3 --3-- m4
     #   \       |
     #    \      |
     #     3     3
     #      \    |
     #       \   |
     #         m5
 
-    lm = (m1,m2,m3,m4,m5)
+    assert dg.is_full(m3, 3, 3) is True
+    assert dg.is_full(m4, 3, 3) is True
+    assert dg.is_full(m5, 3, 3) is True
 
-    dg = DeltaGraph()
-
-    for m in lm:
-        dg.insert_tuple(m)
-
-    try:
-        assert dg.is_full(3, m3, 3, 3) == True
-        assert dg.is_full(3, m4, 3, 3) == True
-        assert dg.is_full(3, m5, 3, 3) == True
-        assert dg.is_full(2, m1, 2, 3) == False
-        assert dg.is_full(2, m2, 2, 3) == False
-        assert dg.is_full(2, m1, 2, 2) == True
-        assert dg.is_full(2, m2, 2, 2) == True
-    except AssertionError:
-        raise
 
 def test_fusion():
     m1 = ((0, 1), (0, 2))
     m2 = ((0, 1), (1, 2))
     m3 = ((0, 1), (2, 2), (0, 3))
     m4 = ((0, 1), (2, 2), (1, 3))
     m5 = ((0, 1), (2, 2), (2, 3))
 
-    lm = (m1,m2,m3,m4,m5)
+    lm = (m1, m2, m3, m4, m5)
 
     dg = DeltaGraph()
 
     for m in lm:
-        dg.insert_tuple(m)
-
-    # list_of_max = [3,3,3,3]
+        dg.insert_node(m)
 
     dg.fusion()
 
-    try:
-        assert dg.graph_dict[3] == {}
-        assert dg.graph_dict[2] == {}
-        assert dg.graph_dict[1] == {((0,1),):{}}
-    except AssertionError:
-        raise
+    assert dg.graph_dict[3] == {}
+    assert dg.graph_dict[2] == {}
+    assert dg.graph_dict[1] == {((0, 1),): {}}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymwp-0.2.1/tests/test_file_io.py` & `pymwp-0.3.0/tests/test_file_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import json
 
-from pymwp.file_io import default_file_out, save_relation, load_relation
+from pymwp.file_io import default_file_out, save_relation, load_relation, loc
 from pymwp import Relation, Choices
 
 
 def test_file_out_name_wo_path():
     """Generating output filename from just a filename without path returns
     result with output directory path."""
     input_file = "my_c_file.c"
@@ -67,7 +67,17 @@
 
     # # now check that composed relation matches expectation
     assert combinations.valid == [[0, 1], [0]]
     assert relation.variables == ["x", "y"]
     assert first_poly.scalar == "m"
     assert first_poly.deltas == [(0, 0)]
     assert not infinity
+
+
+def test_read_loc(mocker):
+    """Returns expected number of lines"""
+    mocker.patch('builtins.open',
+                 new_callable=mocker.mock_open,
+                 read_data="1\n2\n3\n4")
+    result = loc("some_file.c")
+
+    assert result == 4
```

### Comparing `pymwp-0.2.1/tests/test_matrix.py` & `pymwp-0.3.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_monomial.py` & `pymwp-0.3.0/tests/test_monomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_parser.py` & `pymwp-0.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_polynomial.py` & `pymwp-0.3.0/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_relation.py` & `pymwp-0.3.0/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.2.1/tests/test_relation_list.py` & `pymwp-0.3.0/tests/test_relation_list.py`

 * *Files identical despite different names*

