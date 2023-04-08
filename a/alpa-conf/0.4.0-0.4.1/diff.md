# Comparing `tmp/alpa_conf-0.4.0.tar.gz` & `tmp/alpa_conf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpa_conf-0.4.0.tar", max compression
+gzip compressed data, was "alpa_conf-0.4.1.tar", max compression
```

## Comparing `alpa_conf-0.4.0.tar` & `alpa_conf-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-07 22:05:51.672398 alpa_conf-0.4.0/LICENSE
--rw-r--r--   0        0        0       70 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/README.md
--rw-r--r--   0        0        0      151 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/__init__.py
--rw-r--r--   0        0        0     2198 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/alpa.py
--rw-r--r--   0        0        0     1210 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/config_base.py
--rw-r--r--   0        0        0      229 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/constants.py
--rw-r--r--   0        0        0       45 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/exceptions.py
--rw-r--r--   0        0        0     2725 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/alpa_conf/metadata.py
--rw-r--r--   0        0        0      723 2023-04-07 22:05:51.676398 alpa_conf-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 alpa_conf-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 22:26:38.822468 alpa_conf-0.4.1/LICENSE
+-rw-r--r--   0        0        0       70 2023-04-07 22:26:38.822468 alpa_conf-0.4.1/README.md
+-rw-r--r--   0        0        0      151 2023-04-07 22:26:38.822468 alpa_conf-0.4.1/alpa_conf/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-07 22:26:38.822468 alpa_conf-0.4.1/alpa_conf/alpa.py
+-rw-r--r--   0        0        0     1210 2023-04-07 22:26:38.822468 alpa_conf-0.4.1/alpa_conf/config_base.py
+-rw-r--r--   0        0        0      229 2023-04-07 22:26:38.826468 alpa_conf-0.4.1/alpa_conf/constants.py
+-rw-r--r--   0        0        0       45 2023-04-07 22:26:38.826468 alpa_conf-0.4.1/alpa_conf/exceptions.py
+-rw-r--r--   0        0        0     2725 2023-04-07 22:26:38.826468 alpa_conf-0.4.1/alpa_conf/metadata.py
+-rw-r--r--   0        0        0      723 2023-04-07 22:26:38.826468 alpa_conf-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 alpa_conf-0.4.1/PKG-INFO
```

### Comparing `alpa_conf-0.4.0/LICENSE` & `alpa_conf-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpa_conf-0.4.0/alpa_conf/alpa.py` & `alpa_conf-0.4.1/alpa_conf/alpa.py`

 * *Files identical despite different names*

### Comparing `alpa_conf-0.4.0/alpa_conf/config_base.py` & `alpa_conf-0.4.1/alpa_conf/config_base.py`

 * *Files identical despite different names*

### Comparing `alpa_conf-0.4.0/alpa_conf/metadata.py` & `alpa_conf-0.4.1/alpa_conf/metadata.py`

 * *Files identical despite different names*

### Comparing `alpa_conf-0.4.0/pyproject.toml` & `alpa_conf-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "alpa-conf"
-version = "0.4.0"
+version = "0.4.1"
 description = "Wrapper around configuration files for packit and alpa"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa-conf"
 repository = "https://github.com/alpa-team/alpa-conf"
 exclude = ["test/"]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 pyyaml = ">=5.0"
 pydantic = ">=1.8"
 email-validator = ">=1.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
```

### Comparing `alpa_conf-0.4.0/PKG-INFO` & `alpa_conf-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: alpa-conf
-Version: 0.4.0
+Version: 0.4.1
 Summary: Wrapper around configuration files for packit and alpa
 Home-page: https://github.com/alpa-team/alpa-conf
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: email-validator (>=1.0)
 Requires-Dist: pydantic (>=1.8)
 Requires-Dist: pyyaml (>=5.0)
 Project-URL: Repository, https://github.com/alpa-team/alpa-conf
```

