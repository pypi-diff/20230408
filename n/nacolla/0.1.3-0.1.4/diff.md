# Comparing `tmp/nacolla-0.1.3.tar.gz` & `tmp/nacolla-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacolla-0.1.3.tar", max compression
+gzip compressed data, was "nacolla-0.1.4.tar", max compression
```

## Comparing `nacolla-0.1.3.tar` & `nacolla-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1072 2023-01-14 19:40:53.512633 nacolla-0.1.3/LICENSE
--rw-r--r--   0        0        0      125 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-08 15:06:51.780387 nacolla-0.1.3/nacolla/flow.py
--rw-r--r--   0        0        0      876 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/models.py
--rw-r--r--   0        0        0       21 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__init__.py
--rw-r--r--   0        0        0      199 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      170 2023-01-17 12:26:39.565399 nacolla-0.1.3/nacolla/operations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      878 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/add_self_loop.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0        0        0      908 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/add_self_loop.cpython-39.pyc
--rw-r--r--   0        0        0      828 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/concatenate.cpython-38.pyc
--rw-r--r--   0        0        0      824 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/concatenate.cpython-39.pyc
--rw-r--r--   0        0        0     1730 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/merge.cpython-38.pyc
--rw-r--r--   0        0        0     1650 2023-01-17 12:26:39.565399 nacolla-0.1.3/nacolla/operations/__pycache__/merge.cpython-39.pyc
--rw-r--r--   0        0        0      505 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/__pycache__/rename.cpython-39.pyc
--rw-r--r--   0        0        0     1512 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/operations/merge.py
--rw-r--r--   0        0        0      122 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__init__.py
--rw-r--r--   0        0        0      227 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      221 2023-01-17 12:26:39.562066 nacolla-0.1.3/nacolla/parsing/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1787 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-38.pyc
--rw-r--r--   0        0        0     2590 2023-01-17 12:26:39.565399 nacolla-0.1.3/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-39.pyc
--rw-r--r--   0        0        0     3730 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_flow.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     3492 2023-01-17 12:26:39.572066 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_flow.cpython-39.pyc
--rw-r--r--   0        0        0     2519 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation.cpython-38.pyc
--rw-r--r--   0        0        0     2989 2023-04-08 15:09:58.966026 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation.cpython-39.pyc
--rw-r--r--   0        0        0     2845 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation_map.cpython-38.pyc
--rw-r--r--   0        0        0     3151 2023-01-17 12:26:39.562066 nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation_map.cpython-39.pyc
--rw-r--r--   0        0        0     1499 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/flow_file_specification.py
--rw-r--r--   0        0        0     2134 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/implementation_map_file_specification.py
--rw-r--r--   0        0        0     4486 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/parse_flow.py
--rw-r--r--   0        0        0     2979 2023-04-08 15:09:53.836054 nacolla-0.1.3/nacolla/parsing/parse_implementation.py
--rw-r--r--   0        0        0     3568 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/parsing/parse_implementation_map.py
--rw-r--r--   0        0        0     3558 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/stateful_callable.py
--rw-r--r--   0        0        0     8089 2023-04-08 15:05:14.054256 nacolla-0.1.3/nacolla/step.py
--rw-r--r--   0        0        0       67 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__init__.py
--rw-r--r--   0        0        0      217 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      211 2023-01-17 12:26:39.555399 nacolla-0.1.3/nacolla/utilities/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1113 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     1114 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     1118 2023-01-17 12:26:39.555399 nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39.pyc
--rw-r--r--   0        0        0      364 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__pycache__/generics.cpython-38.pyc
--rw-r--r--   0        0        0      395 2023-01-17 12:26:39.555399 nacolla-0.1.3/nacolla/utilities/__pycache__/generics.cpython-39.pyc
--rw-r--r--   0        0        0     2696 2023-01-14 19:40:53.512633 nacolla-0.1.3/nacolla/utilities/__pycache__/nacallable.cpython-38-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     2583 2023-01-14 19:40:53.515966 nacolla-0.1.3/nacolla/utilities/__pycache__/nacallable.cpython-38.pyc
--rw-r--r--   0        0        0     1255 2023-01-14 19:40:53.515966 nacolla-0.1.3/nacolla/utilities/__pycache__/type_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     1315 2023-01-17 12:26:39.555399 nacolla-0.1.3/nacolla/utilities/__pycache__/type_utilities.cpython-39.pyc
--rw-r--r--   0        0        0      962 2023-01-14 19:40:53.515966 nacolla-0.1.3/nacolla/utilities/dispatching_utilities.py
--rw-r--r--   0        0        0      299 2023-01-14 19:40:53.515966 nacolla-0.1.3/nacolla/utilities/generics.py
--rw-r--r--   0        0        0     1289 2023-01-14 19:40:53.515966 nacolla-0.1.3/nacolla/utilities/type_utilities.py
--rw-r--r--   0        0        0      443 2023-04-08 15:10:39.499137 nacolla-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 nacolla-0.1.3/setup.py
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 nacolla-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-14 19:40:53.512633 nacolla-0.1.4/LICENSE
+-rw-r--r--   0        0        0      125 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-08 16:34:58.931374 nacolla-0.1.4/nacolla/flow.py
+-rw-r--r--   0        0        0      876 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/models.py
+-rw-r--r--   0        0        0       21 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__init__.py
+-rw-r--r--   0        0        0      199 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      170 2023-01-17 12:26:39.565399 nacolla-0.1.4/nacolla/operations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      878 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/add_self_loop.cpython-39-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      908 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/add_self_loop.cpython-39.pyc
+-rw-r--r--   0        0        0      828 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/concatenate.cpython-38.pyc
+-rw-r--r--   0        0        0      824 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/concatenate.cpython-39.pyc
+-rw-r--r--   0        0        0     1730 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/merge.cpython-38.pyc
+-rw-r--r--   0        0        0     1650 2023-01-17 12:26:39.565399 nacolla-0.1.4/nacolla/operations/__pycache__/merge.cpython-39.pyc
+-rw-r--r--   0        0        0      505 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/__pycache__/rename.cpython-39.pyc
+-rw-r--r--   0        0        0     1512 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/operations/merge.py
+-rw-r--r--   0        0        0      122 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__init__.py
+-rw-r--r--   0        0        0      227 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      221 2023-01-17 12:26:39.562066 nacolla-0.1.4/nacolla/parsing/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1787 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-38.pyc
+-rw-r--r--   0        0        0     2590 2023-01-17 12:26:39.565399 nacolla-0.1.4/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-39.pyc
+-rw-r--r--   0        0        0     3730 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_flow.cpython-39-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     3492 2023-01-17 12:26:39.572066 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_flow.cpython-39.pyc
+-rw-r--r--   0        0        0     2519 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation.cpython-38.pyc
+-rw-r--r--   0        0        0     2989 2023-04-08 15:09:58.966026 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation.cpython-39.pyc
+-rw-r--r--   0        0        0     2845 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation_map.cpython-38.pyc
+-rw-r--r--   0        0        0     3151 2023-01-17 12:26:39.562066 nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation_map.cpython-39.pyc
+-rw-r--r--   0        0        0     1499 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/flow_file_specification.py
+-rw-r--r--   0        0        0     2134 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/implementation_map_file_specification.py
+-rw-r--r--   0        0        0     4486 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/parse_flow.py
+-rw-r--r--   0        0        0     2979 2023-04-08 15:09:53.836054 nacolla-0.1.4/nacolla/parsing/parse_implementation.py
+-rw-r--r--   0        0        0     3568 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/parsing/parse_implementation_map.py
+-rw-r--r--   0        0        0     3558 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/stateful_callable.py
+-rw-r--r--   0        0        0     8606 2023-04-08 16:34:54.911396 nacolla-0.1.4/nacolla/step.py
+-rw-r--r--   0        0        0       67 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__init__.py
+-rw-r--r--   0        0        0      217 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      211 2023-01-17 12:26:39.555399 nacolla-0.1.4/nacolla/utilities/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1113 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0     1114 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     1118 2023-01-17 12:26:39.555399 nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39.pyc
+-rw-r--r--   0        0        0      364 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__pycache__/generics.cpython-38.pyc
+-rw-r--r--   0        0        0      395 2023-01-17 12:26:39.555399 nacolla-0.1.4/nacolla/utilities/__pycache__/generics.cpython-39.pyc
+-rw-r--r--   0        0        0     2696 2023-01-14 19:40:53.512633 nacolla-0.1.4/nacolla/utilities/__pycache__/nacallable.cpython-38-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     2583 2023-01-14 19:40:53.515966 nacolla-0.1.4/nacolla/utilities/__pycache__/nacallable.cpython-38.pyc
+-rw-r--r--   0        0        0     1255 2023-01-14 19:40:53.515966 nacolla-0.1.4/nacolla/utilities/__pycache__/type_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0     1315 2023-01-17 12:26:39.555399 nacolla-0.1.4/nacolla/utilities/__pycache__/type_utilities.cpython-39.pyc
+-rw-r--r--   0        0        0      962 2023-01-14 19:40:53.515966 nacolla-0.1.4/nacolla/utilities/dispatching_utilities.py
+-rw-r--r--   0        0        0      299 2023-01-14 19:40:53.515966 nacolla-0.1.4/nacolla/utilities/generics.py
+-rw-r--r--   0        0        0     1289 2023-01-14 19:40:53.515966 nacolla-0.1.4/nacolla/utilities/type_utilities.py
+-rw-r--r--   0        0        0      500 2023-04-08 16:35:54.081071 nacolla-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 nacolla-0.1.4/setup.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 nacolla-0.1.4/PKG-INFO
```

### Comparing `nacolla-0.1.3/LICENSE` & `nacolla-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/flow.py` & `nacolla-0.1.4/nacolla/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     @property
     def current_step(self):
         return self.__current_step
 
     def __next__(self) -> Step[ImmutableModel, ImmutableModel]:
         self.__current_message = self.__current_step(self.__current_message)
         self.__current_step = self._stop(
-            self.__current_step.next_step(self.__current_message)
+            self.__current_step.next_step(type(self.__current_message))
         )
         return self.__current_step
 
     def __iter__(self) -> Iterator[Step[ImmutableModel, ImmutableModel]]:
         return self
 
     def _stop(
```

### Comparing `nacolla-0.1.3/nacolla/models.py` & `nacolla-0.1.4/nacolla/models.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/add_self_loop.cpython-39-pytest-7.2.0.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/add_self_loop.cpython-39-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/add_self_loop.cpython-39.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/add_self_loop.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/concatenate.cpython-38.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/concatenate.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/concatenate.cpython-39.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/concatenate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/merge.cpython-38.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/merge.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/__pycache__/merge.cpython-39.pyc` & `nacolla-0.1.4/nacolla/operations/__pycache__/merge.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/operations/merge.py` & `nacolla-0.1.4/nacolla/operations/merge.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-38.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-39.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/implementation_map_file_specification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_flow.cpython-39-pytest-7.2.0.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_flow.cpython-39-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_flow.cpython-39.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_flow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation.cpython-38.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation.cpython-39.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation_map.cpython-38.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation_map.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/__pycache__/parse_implementation_map.cpython-39.pyc` & `nacolla-0.1.4/nacolla/parsing/__pycache__/parse_implementation_map.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/flow_file_specification.py` & `nacolla-0.1.4/nacolla/parsing/flow_file_specification.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/implementation_map_file_specification.py` & `nacolla-0.1.4/nacolla/parsing/implementation_map_file_specification.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/parse_flow.py` & `nacolla-0.1.4/nacolla/parsing/parse_flow.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/parse_implementation.py` & `nacolla-0.1.4/nacolla/parsing/parse_implementation.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/parsing/parse_implementation_map.py` & `nacolla-0.1.4/nacolla/parsing/parse_implementation_map.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/stateful_callable.py` & `nacolla-0.1.4/nacolla/stateful_callable.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/step.py` & `nacolla-0.1.4/nacolla/step.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,31 @@
         # to check if the port is among the outputs of this step
         # and the inputs of the destination step
 
         if self.next is None:
             raise ValueError("None next found, cannot concatenate")
         if self._is_concatenation_compatible(port, destination_step):
             self.next[port] = destination_step
+            return
+
+        raise ValueError(
+            "Concatenation between '"
+            + str(self)
+            + " ["
+            + str(self.output)
+            + "] "
+            + "' and '"
+            + str(destination_step)
+            + " ["
+            + str(destination_step.input)
+            + "]"
+            + "' along '"
+            + str(port)
+            + "' is incompatible"
+        )
 
     def __eq__(self, other: object) -> bool:
         """Compute equality between two steps.
         Steps with the same name are always equal"""
 
         if not isinstance(other, Step):
             return False
@@ -88,42 +105,47 @@
     def __str__(
         self,
     ):
         """A step is fully represented by its name"""
         return self.name
 
     def next_step(
-        self, out: ImmutableModel
+        self, port: type[ImmutableModel]
     ) -> "Union[Step[ImmutableModel, ImmutableModel], End]":
         next_mapping = next(self)
-        output_type = cast(type[OUTPUT_INTERFACE], type(out))
 
-        if output_type in next_mapping.keys():
-            return next_mapping[output_type]
+        if port in next_mapping.keys():
+            return next_mapping[cast(type[OUTPUT_INTERFACE], port)]
 
         for available_out, step in next_mapping.items():
-            if issubclass(output_type, available_out):
+            if issubclass(port, available_out):
                 return step
 
         raise ValueError(
             "Could not find "
-            + str(type(out))
+            + str(type(port))
             + " among available output types: "
             + str(next_mapping)
         )
 
     def _is_concatenation_compatible(
         self, port: type, destination_step: Self
     ) -> TypeGuard[type[OUTPUT_INTERFACE]]:
-        if (
-            not next(self).get(cast(type[OUTPUT_INTERFACE], port))
-            or port not in destination_step.input
-        ):
+        try:
+            self.next_step(port)
+            if port in destination_step.input:
+                return True
+
+            for destination_input in destination_step.input:
+                if issubclass(destination_input, port):
+                    return True
+
+            return False
+        except:
             return False
-        return True
 
     @property
     def input(self) -> set[type[INPUT_INTERFACE]]:
         """Input interface"""
 
         return cast(set[type[INPUT_INTERFACE]], self.input_interface)
```

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-38.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39-pytest-7.2.0.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/dispatching_utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/nacallable.cpython-38-pytest-7.1.3.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/nacallable.cpython-38-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/nacallable.cpython-38.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/nacallable.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/type_utilities.cpython-38.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/type_utilities.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/__pycache__/type_utilities.cpython-39.pyc` & `nacolla-0.1.4/nacolla/utilities/__pycache__/type_utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/dispatching_utilities.py` & `nacolla-0.1.4/nacolla/utilities/dispatching_utilities.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/nacolla/utilities/type_utilities.py` & `nacolla-0.1.4/nacolla/utilities/type_utilities.py`

 * *Files identical despite different names*

### Comparing `nacolla-0.1.3/setup.py` & `nacolla-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['pydantic>=1.10.2,<2.0.0',
  'toml>=0.10.2,<0.11.0',
  'typing-extensions>=4.3.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'nacolla',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Declarative flow based programming',
     'long_description': 'None',
     'author': 'DPaletti',
     'author_email': 'danielepaletti98@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nacolla-0.1.3/PKG-INFO` & `nacolla-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacolla
-Version: 0.1.3
+Version: 0.1.4
 Summary: Declarative flow based programming
 License: MIT
 Author: DPaletti
 Author-email: danielepaletti98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

