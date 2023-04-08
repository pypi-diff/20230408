# Comparing `tmp/backend_sqlalchemy-0.1.1.tar.gz` & `tmp/backend_sqlalchemy-0.1.2.dev1680974524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.1.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.2.dev1680974524.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.1.tar` & `backend_sqlalchemy-0.1.2.dev1680974524.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       21 2023-04-08 16:39:26.858898 backend_sqlalchemy-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-08 16:39:26.858898 backend_sqlalchemy-0.1.1/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      188 2023-04-08 16:39:26.858898 backend_sqlalchemy-0.1.1/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0     1400 2023-04-08 16:39:48.795119 backend_sqlalchemy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      197 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-08 17:21:45.684613 backend_sqlalchemy-0.1.2.dev1680974524/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0     1415 2023-04-08 17:22:04.944725 backend_sqlalchemy-0.1.2.dev1680974524/pyproject.toml
+-rw-r--r--   0        0        0     1426 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.2.dev1680974524/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.1/pyproject.toml` & `backend_sqlalchemy-0.1.2.dev1680974524/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.1"
+version = "0.1.2.dev.1680974524"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
```

### Comparing `backend_sqlalchemy-0.1.1/PKG-INFO` & `backend_sqlalchemy-0.1.2.dev1680974524/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.1
+Version: 0.1.2.dev1680974524
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -24,7 +24,10 @@
 Project-URL: Sponsor on GitHub, https://github.com/sponsors/example123
 Project-URL: Sponsor on Open Collective, https://opencollective.com/example123
 Project-URL: Twitter, https://twitter.com/example123
 Description-Content-Type: text/markdown
 
 # Backend SQLAlchemy
 
+
+[![codecov](https://codecov.io/gh/martinmore-team/backend-sqlalchemy/branch/main/graph/badge.svg?token=XJER9LZAZV)](https://codecov.io/gh/martinmore-team/backend-sqlalchemy)
+
```

