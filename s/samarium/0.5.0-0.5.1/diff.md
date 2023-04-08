# Comparing `tmp/samarium-0.5.0.tar.gz` & `tmp/samarium-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samarium-0.5.0.tar", max compression
+gzip compressed data, was "samarium-0.5.1.tar", max compression
```

## Comparing `samarium-0.5.0.tar` & `samarium-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1059 2023-01-19 17:08:27.046007 samarium-0.5.0/LICENSE
--rw-r--r--   0        0        0     2386 2023-03-22 09:50:27.399407 samarium-0.5.0/README.md
--rw-r--r--   0        0        0      681 2023-04-02 14:38:04.866073 samarium-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1424 2023-03-30 22:15:01.906597 samarium-0.5.0/src/samarium/__init__.py
--rw-r--r--   0        0        0       70 2023-01-19 17:08:28.384405 samarium-0.5.0/src/samarium/__main__.py
--rw-r--r--   0        0        0     2852 2023-03-30 23:35:39.650960 samarium-0.5.0/src/samarium/builtins.py
--rw-r--r--   0        0        0      674 2023-03-29 13:29:57.068736 samarium-0.5.0/src/samarium/classes/__init__.py
--rw-r--r--   0        0        0    33150 2023-04-02 20:11:50.255842 samarium-0.5.0/src/samarium/classes/base.py
--rw-r--r--   0        0        0     6092 2023-02-10 03:22:08.381843 samarium-0.5.0/src/samarium/classes/fileio.py
--rw-r--r--   0        0        0     2883 2023-03-30 22:29:22.782907 samarium-0.5.0/src/samarium/core.py
--rw-r--r--   0        0        0     4142 2023-03-30 23:03:58.879893 samarium-0.5.0/src/samarium/exceptions.py
--rw-r--r--   0        0        0     3471 2023-03-30 22:50:48.434960 samarium-0.5.0/src/samarium/imports.py
--rw-r--r--   0        0        0     6354 2023-03-27 10:14:46.925465 samarium-0.5.0/src/samarium/modules/collections.sm
--rw-r--r--   0        0        0     4198 2023-03-31 00:38:33.996282 samarium-0.5.0/src/samarium/modules/datetime.sm
--rw-r--r--   0        0        0     1618 2023-01-19 17:08:28.380937 samarium-0.5.0/src/samarium/modules/io.sm
--rw-r--r--   0        0        0     3925 2023-03-28 16:37:23.322980 samarium-0.5.0/src/samarium/modules/iter.sm
--rw-r--r--   0        0        0     2123 2023-04-01 06:19:49.080123 samarium-0.5.0/src/samarium/modules/math.sm
--rw-r--r--   0        0        0      646 2023-01-19 17:08:28.381214 samarium-0.5.0/src/samarium/modules/operator.sm
--rw-r--r--   0        0        0      169 2023-03-31 13:25:15.747449 samarium-0.5.0/src/samarium/modules/pystd.py
--rw-r--r--   0        0        0      711 2023-03-24 10:18:27.814974 samarium-0.5.0/src/samarium/modules/random.sm
--rw-r--r--   0        0        0     6975 2023-03-24 10:20:22.049342 samarium-0.5.0/src/samarium/modules/string.sm
--rw-r--r--   0        0        0     2378 2023-03-30 19:26:59.802168 samarium-0.5.0/src/samarium/modules/types.sm
--rw-r--r--   0        0        0     3157 2023-03-30 23:35:39.672893 samarium-0.5.0/src/samarium/python.py
--rw-r--r--   0        0        0       40 2023-01-19 17:08:28.377552 samarium-0.5.0/src/samarium/runtime.py
--rw-r--r--   0        0        0     1174 2023-03-30 23:35:30.418689 samarium-0.5.0/src/samarium/shell.py
--rw-r--r--   0        0        0      492 2023-03-30 23:36:03.110649 samarium-0.5.0/src/samarium/template.py
--rw-r--r--   0        0        0     1285 2023-03-30 23:35:30.487593 samarium-0.5.0/src/samarium/tokenizer.py
--rw-r--r--   0        0        0     2180 2023-01-19 17:08:28.373894 samarium-0.5.0/src/samarium/tokens.py
--rw-r--r--   0        0        0    27143 2023-03-30 23:55:54.968285 samarium-0.5.0/src/samarium/transpiler.py
--rw-r--r--   0        0        0     3050 2023-04-01 07:35:30.592325 samarium-0.5.0/src/samarium/utils.py
--rw-r--r--   0        0        0     3136 1970-01-01 00:00:00.000000 samarium-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-02 20:20:07.460871 samarium-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2304 2023-04-02 22:14:04.461419 samarium-0.5.1/README.md
+-rw-r--r--   0        0        0      681 2023-04-07 22:18:25.805970 samarium-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-04-02 20:20:07.478242 samarium-0.5.1/src/samarium/__init__.py
+-rw-r--r--   0        0        0       70 2023-01-19 17:08:28.384405 samarium-0.5.1/src/samarium/__main__.py
+-rw-r--r--   0        0        0     2852 2023-04-02 20:20:07.478578 samarium-0.5.1/src/samarium/builtins.py
+-rw-r--r--   0        0        0      674 2023-04-02 20:20:07.478901 samarium-0.5.1/src/samarium/classes/__init__.py
+-rw-r--r--   0        0        0    33210 2023-04-07 21:00:46.672638 samarium-0.5.1/src/samarium/classes/base.py
+-rw-r--r--   0        0        0     6092 2023-04-02 20:20:07.479723 samarium-0.5.1/src/samarium/classes/fileio.py
+-rw-r--r--   0        0        0     2883 2023-04-02 20:20:07.480066 samarium-0.5.1/src/samarium/core.py
+-rw-r--r--   0        0        0     4142 2023-04-02 20:20:07.480371 samarium-0.5.1/src/samarium/exceptions.py
+-rw-r--r--   0        0        0     3471 2023-04-02 20:20:07.480686 samarium-0.5.1/src/samarium/imports.py
+-rw-r--r--   0        0        0     6354 2023-04-02 20:20:07.481371 samarium-0.5.1/src/samarium/modules/collections.sm
+-rw-r--r--   0        0        0     4198 2023-04-02 20:20:07.481761 samarium-0.5.1/src/samarium/modules/datetime.sm
+-rw-r--r--   0        0        0     1618 2023-04-02 20:20:07.482061 samarium-0.5.1/src/samarium/modules/io.sm
+-rw-r--r--   0        0        0     3925 2023-04-02 20:20:07.482459 samarium-0.5.1/src/samarium/modules/iter.sm
+-rw-r--r--   0        0        0     2123 2023-04-02 20:20:07.482978 samarium-0.5.1/src/samarium/modules/math.sm
+-rw-r--r--   0        0        0      646 2023-01-19 17:08:28.381214 samarium-0.5.1/src/samarium/modules/operator.sm
+-rw-r--r--   0        0        0      169 2023-04-02 20:20:07.483436 samarium-0.5.1/src/samarium/modules/pystd.py
+-rw-r--r--   0        0        0      711 2023-04-02 20:20:07.483957 samarium-0.5.1/src/samarium/modules/random.sm
+-rw-r--r--   0        0        0     6975 2023-04-02 20:20:07.484269 samarium-0.5.1/src/samarium/modules/string.sm
+-rw-r--r--   0        0        0     2378 2023-04-02 20:20:07.484856 samarium-0.5.1/src/samarium/modules/types.sm
+-rw-r--r--   0        0        0     3157 2023-04-02 20:20:07.485169 samarium-0.5.1/src/samarium/python.py
+-rw-r--r--   0        0        0       40 2023-01-19 17:08:28.377552 samarium-0.5.1/src/samarium/runtime.py
+-rw-r--r--   0        0        0     1174 2023-04-02 20:20:07.485455 samarium-0.5.1/src/samarium/shell.py
+-rw-r--r--   0        0        0      492 2023-04-02 20:20:07.485672 samarium-0.5.1/src/samarium/template.py
+-rw-r--r--   0        0        0     1285 2023-04-02 20:20:07.485907 samarium-0.5.1/src/samarium/tokenizer.py
+-rw-r--r--   0        0        0     2180 2023-01-19 17:08:28.373894 samarium-0.5.1/src/samarium/tokens.py
+-rw-r--r--   0        0        0    27167 2023-04-07 21:19:04.255490 samarium-0.5.1/src/samarium/transpiler.py
+-rw-r--r--   0        0        0     3050 2023-04-07 22:18:24.791295 samarium-0.5.1/src/samarium/utils.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 samarium-0.5.1/PKG-INFO
```

### Comparing `samarium-0.5.0/LICENSE` & `samarium-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/README.md` & `samarium-0.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Samarium
 
 Samarium is a dynamic interpreted language transpiled to Python.
 Samarium, in its most basic form, doesn't use any digits or letters.
 
 Here's a `Hello, World!` program written in Samarium:
 
-<span style="display: inline-block" align="left">
-    <img src="docs/assets/example.png" width="50%">
-</span>
+```kt
+"Hello, World!"!;
+```
 
 Documentation on how to program in Samarium can be found [here](https://samarium-lang.github.io/Samarium/).
 
 
 # Installation
 
 ## [pip](https://pypi.org/project/pip/)
```

### Comparing `samarium-0.5.0/pyproject.toml` & `samarium-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "samarium"
-version = "0.5.0"
+version = "0.5.1"
 description = "The Samarium Programming Language"
 authors = ["trag1c <trag1cdev@yahoo.com>"]
 license = "MIT"
 documentation = "https://samarium-lang.github.io/Samarium/"
 repository = "https://github.com/samarium-lang/Samarium"
 readme = "README.md"
```

### Comparing `samarium-0.5.0/src/samarium/__init__.py` & `samarium-0.5.1/src/samarium/__init__.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/builtins.py` & `samarium-0.5.1/src/samarium/builtins.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/classes/__init__.py` & `samarium-0.5.1/src/samarium/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/classes/base.py` & `samarium-0.5.1/src/samarium/classes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,14 +827,17 @@
 
     def __hash__(self) -> int:
         return cast(int, self.hash().val)
 
     def hash(self) -> Number:
         return Num(hash(self.val))
 
+    def __invert__(self) -> Number:
+        return Num(-1)
+
     def __floordiv__(self, other: Any) -> Number:
         return Num(not other)
 
 
 I64_MAX = 9223372036854775807
 NULL = Null()
```

### Comparing `samarium-0.5.0/src/samarium/classes/fileio.py` & `samarium-0.5.1/src/samarium/classes/fileio.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/core.py` & `samarium-0.5.1/src/samarium/core.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/exceptions.py` & `samarium-0.5.1/src/samarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/imports.py` & `samarium-0.5.1/src/samarium/imports.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/collections.sm` & `samarium-0.5.1/src/samarium/modules/collections.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/datetime.sm` & `samarium-0.5.1/src/samarium/modules/datetime.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/io.sm` & `samarium-0.5.1/src/samarium/modules/io.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/iter.sm` & `samarium-0.5.1/src/samarium/modules/iter.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/math.sm` & `samarium-0.5.1/src/samarium/modules/math.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/operator.sm` & `samarium-0.5.1/src/samarium/modules/operator.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/random.sm` & `samarium-0.5.1/src/samarium/modules/random.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/string.sm` & `samarium-0.5.1/src/samarium/modules/string.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/modules/types.sm` & `samarium-0.5.1/src/samarium/modules/types.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/python.py` & `samarium-0.5.1/src/samarium/python.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/shell.py` & `samarium-0.5.1/src/samarium/shell.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/tokenizer.py` & `samarium-0.5.1/src/samarium/tokenizer.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/tokens.py` & `samarium-0.5.1/src/samarium/tokens.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.0/src/samarium/transpiler.py` & `samarium-0.5.1/src/samarium/transpiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,16 @@
                 "".join(quick_template).format(token_name.split("_")[-1]),
             ]
 
     def _operators(self, token: Token, push: Callable) -> None:
         if token is Token.IN and self._prev is Token.NOT:
             pass
         elif (
-            token in Group.operators - {Token.NOT, Token.IN, Token.SUB, Token.ADD}
+            token
+            in Group.operators - {Token.BNOT, Token.NOT, Token.IN, Token.SUB, Token.ADD}
             and self._prev in Group.operators
             or (
                 self._prev
                 in Group.operators
                 | {
                     Token.PAREN_OPEN,
                     Token.BRACKET_OPEN,
```

### Comparing `samarium-0.5.0/src/samarium/utils.py` & `samarium-0.5.1/src/samarium/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Callable
 from re import sub
 from typing import Any, TypeVar
 
 from .exceptions import SamariumTypeError, SamariumValueError
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 T = TypeVar("T")
 
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
```

### Comparing `samarium-0.5.0/PKG-INFO` & `samarium-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium
-Version: 0.5.0
+Version: 0.5.1
 Summary: The Samarium Programming Language
 Home-page: https://github.com/samarium-lang/Samarium
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,17 +21,17 @@
 # Samarium
 
 Samarium is a dynamic interpreted language transpiled to Python.
 Samarium, in its most basic form, doesn't use any digits or letters.
 
 Here's a `Hello, World!` program written in Samarium:
 
-<span style="display: inline-block" align="left">
-    <img src="docs/assets/example.png" width="50%">
-</span>
+```kt
+"Hello, World!"!;
+```
 
 Documentation on how to program in Samarium can be found [here](https://samarium-lang.github.io/Samarium/).
 
 
 # Installation
 
 ## [pip](https://pypi.org/project/pip/)
```

