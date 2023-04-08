# Comparing `tmp/hhoppe-tools-1.2.7.tar.gz` & `tmp/hhoppe-tools-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhoppe-tools-1.2.7.tar", last modified: Fri Apr  7 23:19:53 2023, max compression
+gzip compressed data, was "hhoppe-tools-1.2.8.tar", last modified: Sat Apr  8 04:13:37 2023, max compression
```

## Comparing `hhoppe-tools-1.2.7.tar` & `hhoppe-tools-1.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-07 23:19:44.987891 hhoppe-tools-1.2.7/LICENSE
--rw-r--r--   0        0        0      147 2023-04-07 23:19:44.987891 hhoppe-tools-1.2.7/README.md
--rw-r--r--   0        0        0    76405 2023-04-07 23:19:44.987891 hhoppe-tools-1.2.7/hhoppe_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 23:19:44.987891 hhoppe-tools-1.2.7/hhoppe_tools/py.typed
--rw-r--r--   0        0        0     2569 2023-04-07 23:19:44.987891 hhoppe-tools-1.2.7/pyproject.toml
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/LICENSE
+-rw-r--r--   0        0        0      147 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/README.md
+-rw-r--r--   0        0        0    76399 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/hhoppe_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/hhoppe_tools/py.typed
+-rw-r--r--   0        0        0     2569 2023-04-08 04:13:29.845101 hhoppe-tools-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 hhoppe-tools-1.2.8/PKG-INFO
```

### Comparing `hhoppe-tools-1.2.7/LICENSE` & `hhoppe-tools-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hhoppe-tools-1.2.7/hhoppe_tools/__init__.py` & `hhoppe-tools-1.2.8/hhoppe_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 env python3 -m doctest -v __init__.py | perl -ne 'print if /had no tests/../passed all/' | tail -n +2 | head -n -1
 ```
 ."""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.2.7'
+__version__ = '1.2.8'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import ast
 import collections.abc
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import cProfile
@@ -279,27 +279,27 @@
   ...   s = m.getvalue()
   >>> s
   'a = <string>, literal_string, s, a * 2 = <string><string>, 34 // 3 = 11\n'
   """
   print(_dump_vars(*args), flush=True)
 
 
-def analyze_lru_caches(variables: Mapping[str, Any], /) -> None:
+def analyze_functools_caches(variables: Mapping[str, Any], /) -> None:
   """Report on usage and efficiency of memoization caches.
 
   Args:
     variables: Dictionary, which is usually `globals()`.
 
-  >>> @functools.lru_cache(maxsize=None)
+  >>> @functools.cache
   ... def func(i: int) -> int:
   ...   return i**2
 
   >>> [func(i) for i in [1, 2, 1, 3, 1]]
   [1, 4, 1, 9, 1]
-  >>> analyze_lru_caches(globals())
+  >>> analyze_functools_caches(globals())
   ...  # doctest:+ELLIPSIS
   # func ...  3/inf        0.400 hit=            2 miss=            3
   """
   for name, value in variables.items():
     try:
       info = value.cache_info()
     except AttributeError:
@@ -310,37 +310,37 @@
     name2 = f'{name:31}' if len(name) <= 31 else f'{name[:15]}..{name[-14:]}'
     print(
         f'# {name2} {info.currsize:11_}/{s_max_size:<10}'
         f' {hit_ratio:5.3f} hit={info.hits:13_} miss={info.misses:13_}'
     )
 
 
-def clear_lru_caches(variables: Mapping[str, Any], /, *, verbose: bool = False) -> None:
+def clear_functools_caches(variables: Mapping[str, Any], /, *, verbose: bool = False) -> None:
   """Clear all the function memoization caches.
 
   Args:
     variables: Dictionary, which is usually `globals()`.
     verbose: If True, show names of cleared caches.
 
-  >>> @functools.lru_cache(maxsize=None)
+  >>> @functools.cache
   ... def func(i: int) -> int:
   ...   return i**2
 
   >>> [func(i) for i in [1, 2, 1, 3, 1]]
   [1, 4, 1, 9, 1]
   >>> check_eq(func.cache_info().currsize, 3)
 
-  >>> clear_lru_caches(globals())
+  >>> clear_functools_caches(globals())
   >>> check_eq(func.cache_info().hits, 0)
   """
   for name, value in variables.items():
     with contextlib.suppress(AttributeError):
       value.cache_clear()
       if verbose:
-        print(f'Cleared lru_cache for {name}().')
+        print(f'Cleared functools.cache for {name}().')
 
 
 # ** Jupyter/IPython notebook functionality
 
 
 def _get_ipython() -> Any:
   import IPython
```

### Comparing `hhoppe-tools-1.2.7/pyproject.toml` & `hhoppe-tools-1.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hhoppe-tools-1.2.7/PKG-INFO` & `hhoppe-tools-1.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhoppe-tools
-Version: 1.2.7
+Version: 1.2.8
 Summary: Library of Python tools by Hugues Hoppe
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

