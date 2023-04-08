# Comparing `tmp/griptape_tools-0.1.0.tar.gz` & `tmp/griptape_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.1.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.2.0.tar", max compression
```

## Comparing `griptape_tools-0.1.0.tar` & `griptape_tools-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.1.0/README.md
--rw-r--r--   0        0        0      293 2023-04-06 22:25:01.134218 griptape_tools-0.1.0/griptape_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.1.0/griptape_tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.1.0/griptape_tools/calculator/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-06 22:52:37.057420 griptape_tools-0.1.0/griptape_tools/calculator/requirements.txt
--rw-r--r--   0        0        0     1326 2023-04-06 22:34:53.142788 griptape_tools-0.1.0/griptape_tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.1.0/griptape_tools/google_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-06 19:20:02.787519 griptape_tools-0.1.0/griptape_tools/google_search/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-06 22:52:37.055868 griptape_tools-0.1.0/griptape_tools/google_search/requirements.txt
--rw-r--r--   0        0        0     2273 2023-04-06 19:20:02.787754 griptape_tools-0.1.0/griptape_tools/google_search/tool.py
--rw-r--r--   0        0        0      482 2023-04-06 22:52:46.957135 griptape_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.2.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.2.0/griptape/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.2.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.2.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.2.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-07 16:15:03.210825 griptape_tools-0.2.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0     1331 2023-04-07 15:55:43.987046 griptape_tools-0.2.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.2.0/griptape/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-06 19:20:02.787519 griptape_tools-0.2.0/griptape/tools/google_search/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-07 16:15:03.213519 griptape_tools-0.2.0/griptape/tools/google_search/requirements.txt
+-rw-r--r--   0        0        0     2278 2023-04-07 15:55:50.567434 griptape_tools-0.2.0/griptape/tools/google_search/tool.py
+-rw-r--r--   0        0        0      525 2023-04-07 16:17:26.380989 griptape_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.2.0/PKG-INFO
```

### Comparing `griptape_tools-0.1.0/LICENSE` & `griptape_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.1.0/README.md` & `griptape_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.1.0/griptape_tools/calculator/tool.py` & `griptape_tools-0.2.0/griptape/tools/calculator/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import sys
 from io import StringIO
 from schema import Schema, Literal
-from griptape import BaseTool, action
+from griptape.core import BaseTool, action
 
 
 class Calculator(BaseTool):
     schemas = {
         "calculate": Schema({
             Literal(
                 "action_input",
```

### Comparing `griptape_tools-0.1.0/griptape_tools/google_search/tool.py` & `griptape_tools-0.2.0/griptape/tools/google_search/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 import requests
 from attr import define, field
 from schema import Schema, Literal
-from griptape import BaseTool, action
+from griptape.core import BaseTool, action
 
 
 @define
 class GoogleSearch(BaseTool):
     schemas = {
         "search": Schema({
             Literal(
```

### Comparing `griptape_tools-0.1.0/PKG-INFO` & `griptape_tools-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.1.3)
+Requires-Dist: griptape-core (>=0.2.1)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
```

