# Comparing `tmp/backend_sqlalchemy-0.1.2.tar.gz` & `tmp/backend_sqlalchemy-0.1.2.dev1680974524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.2.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.2.dev1680974524.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.2.tar` & `backend_sqlalchemy-0.1.2.dev1680974524.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      197 2023-04-08 17:32:25.635464 backend_sqlalchemy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-08 17:32:25.635464 backend_sqlalchemy-0.1.2/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      240 2023-04-08 17:32:25.635464 backend_sqlalchemy-0.1.2/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0     1400 2023-04-08 17:32:47.659814 backend_sqlalchemy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0     1415 2023-04-08 17:22:04.944725 backend_sqlalchemy-0.1.2.dev1680974524/pyproject.toml
+-rw-r--r--   0        0        0     1426 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.2.dev1680974524/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.2/pyproject.toml` & `backend_sqlalchemy-0.1.2.dev1680974524/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.2"
+version = "0.1.2.dev.1680974524"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
```

### Comparing `backend_sqlalchemy-0.1.2/PKG-INFO` & `backend_sqlalchemy-0.1.2.dev1680974524/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.2
+Version: 0.1.2.dev1680974524
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
```

