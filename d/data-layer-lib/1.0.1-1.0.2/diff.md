# Comparing `tmp/data_layer_lib-1.0.1.tar.gz` & `tmp/data_layer_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_layer_lib-1.0.1.tar", max compression
+gzip compressed data, was "data_layer_lib-1.0.2.tar", max compression
```

## Comparing `data_layer_lib-1.0.1.tar` & `data_layer_lib-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      640 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/README.md
--rw-r--r--   0        0        0     1214 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/src/libdata/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/src/libdata/models/__init__.py
--rw-r--r--   0        0        0      870 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/src/libdata/models/tables.py
--rw-r--r--   0        0        0      894 2023-04-08 16:37:50.960015 data_layer_lib-1.0.1/src/libdata/settings.py
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 data_layer_lib-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      640 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/README.md
+-rw-r--r--   0        0        0     1214 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/src/libdata/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/src/libdata/models/__init__.py
+-rw-r--r--   0        0        0      870 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/src/libdata/models/tables.py
+-rw-r--r--   0        0        0      877 2023-04-08 17:00:05.958299 data_layer_lib-1.0.2/src/libdata/settings.py
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 data_layer_lib-1.0.2/PKG-INFO
```

### Comparing `data_layer_lib-1.0.1/README.md` & `data_layer_lib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `data_layer_lib-1.0.1/pyproject.toml` & `data_layer_lib-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-layer-lib"
-version = "1.0.1"
+version = "1.0.2"
 description = "Database layer library"
 authors = ["Arif Nawaz"]
 readme = "README.md"
 packages = [{include = "libdata", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `data_layer_lib-1.0.1/src/libdata/models/tables.py` & `data_layer_lib-1.0.2/src/libdata/models/tables.py`

 * *Files identical despite different names*

### Comparing `data_layer_lib-1.0.1/src/libdata/settings.py` & `data_layer_lib-1.0.2/src/libdata/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         except AssertionError as error:
             print(error)
         return None
 
     @staticmethod
     def get_session(db_engine):
         return scoped_session(
-            sessionmaker(autocommit=True, autoflush=False, bind=db_engine)
+            sessionmaker(autoflush=False, bind=db_engine)
         )
 
 
 settings = Settings()
 engine = settings.get_engine()
 db_session = Settings.get_session(engine)
```

### Comparing `data_layer_lib-1.0.1/PKG-INFO` & `data_layer_lib-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-layer-lib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Database layer library
 Author: Arif Nawaz
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

