# Comparing `tmp/advent-of-code-hhoppe-1.0.1.tar.gz` & `tmp/advent-of-code-hhoppe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advent-of-code-hhoppe-1.0.1.tar", last modified: Fri Apr  7 14:04:12 2023, max compression
+gzip compressed data, was "advent-of-code-hhoppe-1.0.2.tar", last modified: Fri Apr  7 23:19:39 2023, max compression
```

## Comparing `advent-of-code-hhoppe-1.0.1.tar` & `advent-of-code-hhoppe-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/LICENSE
--rw-r--r--   0        0        0     2367 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/README.md
--rw-r--r--   0        0        0     7737 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/advent_of_code_hhoppe/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/advent_of_code_hhoppe/py.typed
--rw-r--r--   0        0        0      907 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/advent_of_code_hhoppe/setup.cfg
--rw-r--r--   0        0        0     2017 2023-04-07 14:04:01.110678 advent-of-code-hhoppe-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 advent-of-code-hhoppe-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2367 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/README.md
+-rw-r--r--   0        0        0     7737 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/py.typed
+-rw-r--r--   0        0        0      907 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/setup.cfg
+-rw-r--r--   0        0        0     2017 2023-04-07 23:19:31.652335 advent-of-code-hhoppe-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 advent-of-code-hhoppe-1.0.2/PKG-INFO
```

### Comparing `advent-of-code-hhoppe-1.0.1/LICENSE` & `advent-of-code-hhoppe-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.1/README.md` & `advent-of-code-hhoppe-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.1/advent_of_code_hhoppe/__init__.py` & `advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """Library for Advent of Code -- Hugues Hoppe."""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 from collections.abc import Callable
 import contextlib
 import dataclasses
 import numbers
 import pathlib
```

### Comparing `advent-of-code-hhoppe-1.0.1/advent_of_code_hhoppe/setup.cfg` & `advent-of-code-hhoppe-1.0.2/advent_of_code_hhoppe/setup.cfg`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.1/pyproject.toml` & `advent-of-code-hhoppe-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "advent-of-code-hhoppe"
 description = "Library for Advent of Code -- Hugues Hoppe."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "Hugues Hoppe", email="hhoppe@gmail.com"}]
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
 ]
```

### Comparing `advent-of-code-hhoppe-1.0.1/PKG-INFO` & `advent-of-code-hhoppe-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: advent-of-code-hhoppe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for Advent of Code -- Hugues Hoppe.
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: IPython
 Project-URL: homepage, https://github.com/hhoppe/advent-of-code-hhoppe
 Project-URL: repository, https://github.com/hhoppe/advent-of-code-hhoppe
```

