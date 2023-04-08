# Comparing `tmp/sidetrek-0.0.6.tar.gz` & `tmp/sidetrek-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.6.tar", max compression
+gzip compressed data, was "sidetrek-0.0.7.tar", max compression
```

## Comparing `sidetrek-0.0.6.tar` & `sidetrek-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.6/README.md
--rw-r--r--   0        0        0      689 2023-04-08 21:54:07.116613 sidetrek-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      534 2023-04-02 20:02:40.835617 sidetrek-0.0.6/sidetrek/__init__.py
--rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.6/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.6/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.6/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.6/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.6/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.6/sidetrek/constants.py
--rw-r--r--   0        0        0      473 2023-04-08 21:54:00.392244 sidetrek-0.0.6/sidetrek/global_fns.py
--rw-r--r--   0        0        0      661 2023-03-16 01:49:43.511125 sidetrek-0.0.6/sidetrek/loggers.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.7/README.md
+-rw-r--r--   0        0        0      689 2023-04-08 21:59:54.185051 sidetrek-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      534 2023-04-02 20:02:40.835617 sidetrek-0.0.7/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.7/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.7/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.7/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.7/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.7/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.7/sidetrek/constants.py
+-rw-r--r--   0        0        0      473 2023-04-08 21:59:47.447114 sidetrek-0.0.7/sidetrek/global_fns.py
+-rw-r--r--   0        0        0      661 2023-03-16 01:49:43.511125 sidetrek-0.0.7/sidetrek/loggers.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.7/PKG-INFO
```

### Comparing `sidetrek-0.0.6/pyproject.toml` & `sidetrek-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
```

### Comparing `sidetrek-0.0.6/sidetrek/__init__.py` & `sidetrek-0.0.7/sidetrek/__init__.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/cli.py` & `sidetrek-0.0.7/sidetrek/cli.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc` & `sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.7/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.7/sidetrek/cli_commands/helpers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.7/sidetrek/cli_commands/workflow.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/sidetrek/loggers.py` & `sidetrek-0.0.7/sidetrek/loggers.py`

 * *Files identical despite different names*

### Comparing `sidetrek-0.0.6/PKG-INFO` & `sidetrek-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidetrek
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Seungchan Lee
 Author-email: seunggs@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: flytekit (<=1.4.2)
```

