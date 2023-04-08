# Comparing `tmp/essentials_configuration-2.0.0.tar.gz` & `tmp/essentials_configuration-2.0.1.tar.gz`

## Comparing `essentials_configuration-2.0.0.tar` & `essentials_configuration-2.0.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/MANIFEST.in
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/example.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/summary-ex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/cli/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/cli/main.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/py.typed
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/env/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/env/py.typed
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/errors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/errors/py.typed
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/ini/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/ini/py.typed
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/json/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/json/py.typed
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/py.typed
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/toml/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/toml/py.typed
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/yaml/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/yaml/py.typed
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/LICENSE
--rw-r--r--   0        0        0    12981 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/README.md
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/example.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/summary-ex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/py.typed
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/py.typed
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/env/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/env/py.typed
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/errors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/errors/py.typed
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/ini/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/ini/py.typed
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/json/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/json/py.typed
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/py.typed
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/toml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/toml/py.typed
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/yaml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/yaml/py.typed
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/LICENSE
+-rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/README.md
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/PKG-INFO
```

### Comparing `essentials_configuration-2.0.0/CHANGELOG.md` & `essentials_configuration-2.0.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.0.1] - 2023-04-08 :egg:
+- Fix missing `py.typed` files in the distribution package.
+
 ## [2.0.0] - 2023-04-08 :egg:
 - Renames the main namespace to `config`.
 - Adds a method to obtain type checked configuration items (e.g. with `pydantic`
   or custom classes).
 - Adds support to read secrets stored in the user folder, for development purpose.
 - Adds a CLI to administer local secrets stored in the user folder.
 - Adds a `FileConfigurationSource` base class.
```

### Comparing `essentials_configuration-2.0.0/summary-ex.py` & `essentials_configuration-2.0.1/summary-ex.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/common/__init__.py` & `essentials_configuration-2.0.1/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/common/files.py` & `essentials_configuration-2.0.1/config/common/files.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/env/__init__.py` & `essentials_configuration-2.0.1/config/env/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/ini/__init__.py` & `essentials_configuration-2.0.1/config/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/secrets/__init__.py` & `essentials_configuration-2.0.1/config/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/secrets/cli.py` & `essentials_configuration-2.0.1/config/secrets/cli.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/toml/__init__.py` & `essentials_configuration-2.0.1/config/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/config/yaml/__init__.py` & `essentials_configuration-2.0.1/config/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/.gitignore` & `essentials_configuration-2.0.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -101,8 +101,9 @@
 .mypy_cache/
 
 .idea/
 
 test-cov.xml
 test-output.xml
 *.py,cover
-venv*
+venv*
+.vscode
```

### Comparing `essentials_configuration-2.0.0/LICENSE` & `essentials_configuration-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.0/README.md` & `essentials_configuration-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - support for nested structures and lists, using attribute notation
 - strategy to use environment specific settings
 - features to handle secrets and values stored in the user folder, for local
   development
 - features to support validation of configuration items, for example using
   `pydantic`, or user defined classes
 
-This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1).
+This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1), [Microsoft Extensions Configuration Deep Dive](https://www.paraesthesia.com/archive/2018/06/20/microsoft-extensions-configuration-deep-dive/)_).
 
 The main class is influenced by Luciano Ramalho`s example of
 JSON structure explorer using attribute notation, in his book [Fluent Python](http://shop.oreilly.com/product/0636920032519.do).
 
 ## Overview
 
 `essentials-configuration` provides a way to handle configuration roots
```

### Comparing `essentials_configuration-2.0.0/pyproject.toml` & `essentials_configuration-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "essentials-configuration"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
 description = "Implementation of key-value pair based configuration for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `essentials_configuration-2.0.0/PKG-INFO` & `essentials_configuration-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: essentials-configuration
-Version: 2.0.0
+Version: 2.0.1
 Summary: Implementation of key-value pair based configuration for Python applications.
 Project-URL: Homepage, https://github.com/Neoteroi/essentials-configuration
 Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-configuration/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: configuration,management,root,strategy
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,15 +40,15 @@
 - support for nested structures and lists, using attribute notation
 - strategy to use environment specific settings
 - features to handle secrets and values stored in the user folder, for local
   development
 - features to support validation of configuration items, for example using
   `pydantic`, or user defined classes
 
-This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1).
+This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1), [Microsoft Extensions Configuration Deep Dive](https://www.paraesthesia.com/archive/2018/06/20/microsoft-extensions-configuration-deep-dive/)_).
 
 The main class is influenced by Luciano Ramalho`s example of
 JSON structure explorer using attribute notation, in his book [Fluent Python](http://shop.oreilly.com/product/0636920032519.do).
 
 ## Overview
 
 `essentials-configuration` provides a way to handle configuration roots
```

