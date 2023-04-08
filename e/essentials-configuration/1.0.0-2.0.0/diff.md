# Comparing `tmp/essentials-configuration-1.0.0.tar.gz` & `tmp/essentials_configuration-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "essentials-configuration-1.0.0.tar", last modified: Sat Nov  5 20:17:50 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `essentials-configuration-1.0.0.tar` & `essentials_configuration-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.565878 essentials-configuration-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10266 2022-11-05 20:17:50.565878 essentials-configuration-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9442 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/common/
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/env/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/env/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/errors/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/ini/
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/ini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/ini/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/json/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/json/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/toml/
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/toml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/toml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.561878 essentials-configuration-1.0.0/configuration/yaml/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/configuration/yaml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 20:17:50.565878 essentials-configuration-1.0.0/essentials_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10266 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-05 20:17:50.000000 essentials-configuration-1.0.0/essentials_configuration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-05 20:17:50.565878 essentials-configuration-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-11-05 20:17:32.000000 essentials-configuration-1.0.0/setup.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/example.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/summary-ex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/cli/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/cli/main.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/common/py.typed
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/env/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/env/py.typed
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/errors/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/errors/py.typed
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/ini/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/ini/py.typed
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/json/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/json/py.typed
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/secrets/py.typed
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/toml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/toml/py.typed
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/yaml/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/config/yaml/py.typed
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/LICENSE
+-rw-r--r--   0        0        0    12981 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/README.md
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 essentials_configuration-2.0.0/PKG-INFO
```

### Comparing `essentials-configuration-1.0.0/LICENSE` & `essentials_configuration-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials-configuration-1.0.0/PKG-INFO` & `essentials_configuration-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,107 @@
-Metadata-Version: 2.1
-Name: essentials-configuration
-Version: 1.0.0
-Summary: Implementation of key-value pair based configuration for Python applications.
-Home-page: https://github.com/Neoteroi/essentials-configuration
-Author: RobertoPrevato
-Author-email: roberto.prevato@gmail.com
-License: MIT
-Keywords: configuration root environment
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: yaml
-License-File: LICENSE
-
 ![Build](https://github.com/Neoteroi/essentials-configuration/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/essentials-configuration.svg)](https://pypi.python.org/pypi/essentials-configuration)
 [![versions](https://img.shields.io/pypi/pyversions/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration)
 [![codecov](https://codecov.io/gh/Neoteroi/essentials-configuration/branch/main/graph/badge.svg?token=VzAnusWIZt)](https://codecov.io/gh/Neoteroi/essentials-configuration)
 [![license](https://img.shields.io/github/license/Neoteroi/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration/blob/main/LICENSE)
 
 # Python configuration utilities
 Implementation of key-value pair based configuration for Python applications.
 
 **Features:**
-* support for most common sources of application settings
-* support for overriding settings in sequence
-* support for nested structures and lists, using attribute notation
-* strategy to use environment specific settings
+- support for most common sources of application settings
+- support for overriding settings in sequence
+- support for nested structures and lists, using attribute notation
+- strategy to use environment specific settings
+- features to handle secrets and values stored in the user folder, for local
+  development
+- features to support validation of configuration items, for example using
+  `pydantic`, or user defined classes
 
-This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1), [Microsoft Extensions Configuration Deep Dive](https://www.paraesthesia.com/archive/2018/06/20/microsoft-extensions-configuration-deep-dive/)_).
+This library is freely inspired by .NET Core `Microsoft.Extensions.Configuration` (_ref. [MSDN documentation](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-2.1).
 
 The main class is influenced by Luciano Ramalho`s example of
 JSON structure explorer using attribute notation, in his book [Fluent Python](http://shop.oreilly.com/product/0636920032519.do).
 
 ## Overview
 
 `essentials-configuration` provides a way to handle configuration roots
-composed of different layers, such as configuration files and environment
+composed of several layers, such as configuration files and environment
 variables. Layers are applied in order and can override each others' values,
 enabling different scenarios like configuration by environment and system
 instance.
 
 ## Supported sources:
-* **toml** files
-* **yaml** files
-* **json** files
-* **ini** files
-* environment variables
-* dictionaries
-* keys and values
-* [Azure Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/basic-concepts), using [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault)
-* custom sources, implementing the `ConfigurationSource` interface
+- **toml** files
+- **yaml** files
+- **json** files
+- **ini** files
+- environment variables
+- secrets stored in the user folder, for development purpose
+- dictionaries
+- keys and values
+- [Azure Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/basic-concepts), using [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault)
+- custom sources, implementing the `ConfigurationSource` interface
 
 ## Installation
 
 ```bash
 pip install essentials-configuration
 ```
 
 To install with support for `YAML` configuration files:
 
 ```
 pip install essentials-configuration[yaml]
 ```
 
+To install with support for `YAML` configuration files and the `CLI` to handle
+user secrets:
+
+```
+pip install essentials-configuration[full]
+```
+
 ## Extensions
 
 * Azure Key Vault secrets configuration source:
   [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault)
 
-
 # Examples
 
+Please read the list of examples in the [examples folder](./examples). Below
+are reported some of the examples that are tested in this repository.
+
 ### TOML file
 
 ```python
-from configuration.common import ConfigurationBuilder
-from configuration.toml import TOMLFile
-from configuration.env import EnvVars
+from config.common import ConfigurationBuilder
+from config.env import EnvVars
+from config.toml import TOMLFile
+
 
 builder = ConfigurationBuilder(
     TOMLFile("settings.toml"),
     EnvVars(prefix="APP_")
 )
 
 config = builder.build()
 ```
 
 For example, if the TOML file contains the following contents:
 
-```json
+```toml
 title = "TOML Example"
 
 [owner]
 name = "Tom Preston-Werner"
 ```
 
-And the environment has a variable named `APP_OWNER__NAME=AAA`:
+And the environment has a variable such as `APP_OWNER__NAME=AAA`, the owner
+name from the TOML file gets overridden by the env variable:
 
 ```python
 >>> config
 <Configuration {'title': '...', 'owner': '...'}>
 >>> config.title
 'TOML Example'
 >>> config.owner.name
@@ -117,17 +112,17 @@
 
 In the following example, configuration values will include the structure
 inside the file `settings.json` and environment variables whose name starts
 with "APP_". Settings are applied in order, so environment variables with
 matching name override values from the `json` file.
 
 ```python
-from configuration.common import ConfigurationBuilder
-from configuration.json import JSONFile
-from configuration.env import EnvVars
+from config.common import ConfigurationBuilder
+from config.json import JSONFile
+from config.env import EnvVars
 
 builder = ConfigurationBuilder(
     JSONFile("settings.json"),
     EnvVars(prefix="APP_")
 )
 
 config = builder.build()
@@ -161,17 +156,17 @@
 In this example, configuration will include anything inside a file
 `settings.yaml` and environment variables. Settings are applied in order, so
 environment variables with matching name override values from the `yaml` file
 (using the `yaml` source requires also `PyYAML` package).
 
 
 ```python
-from configuration.common import ConfigurationBuilder
-from configuration.env import EnvVars
-from configuration.yaml import YAMLFile
+from config.common import ConfigurationBuilder
+from config.env import EnvVars
+from config.yaml import YAMLFile
 
 builder = ConfigurationBuilder()
 
 builder.add_source(YAMLFile("settings.yaml"))
 builder.add_source(EnvVars())
 
 config = builder.build()
@@ -182,64 +177,61 @@
 In this example, if an environment variable with name `APP_ENVIRONMENT` and
 value `dev` exists, and a configuration file with name `settings.dev.yaml` is
 present, it is read to override values configured in `settings.yaml` file.
 
 ```python
 import os
 
-from configuration.common import ConfigurationBuilder
-from configuration.env import EnvVars
-from configuration.yaml import YAMLFile
+from config.common import ConfigurationBuilder
+from config.env import EnvVars
+from config.yaml import YAMLFile
 
 environment_name = os.environ["APP_ENVIRONMENT"]
 
-builder = ConfigurationBuilder()
-
-builder.add_source(YAMLFile("settings.yaml"))
-
-builder.add_source(YAMLFile(f"settings.{environment_name}.yaml", optional=True))
-
-builder.add_source(EnvVars(prefix="APP_"))
+builder = ConfigurationBuilder(
+    YAMLFile("settings.yaml"),
+    YAMLFile(f"settings.{environment_name}.yaml", optional=True)
+)
 
 config = builder.build()
 ```
 
 ### Filtering environment variables by prefix
 
 ```python
-from configuration.common import ConfigurationBuilder
-from configuration.env import EnvVars
+from config.common import ConfigurationBuilder
+from config.env import EnvVars
 
 builder = ConfigurationBuilder()
 
 builder.add_source(EnvVars(prefix="APP_"))
 
 config = builder.build()
 ```
 
 ### INI files
 
 INI files are parsed using the built-in `configparser` module, therefore
 support `[DEFAULT]` section; all values are kept as strings.
 
 ```python
-from configuration.common import ConfigurationBuilder
-from configuration.ini import INIFile
+from config.common import ConfigurationBuilder
+from config.ini import INIFile
 
 builder = ConfigurationBuilder()
 
 builder.add_source(INIFile("settings.ini"))
 
 config = builder.build()
 ```
 
 ### Dictionaries
 
 ```python
-from configuration.common import ConfigurationBuilder
+from config.common import ConfigurationBuilder
 
 builder = ConfigurationBuilder()
 
 builder.add_map({"host": "localhost", "port": 8080})
 
 builder.add_map({"hello": "world", "example": [{"id": 1}, {"id": 2}]})
 
@@ -251,38 +243,104 @@
 assert config.example[0].id == 1
 assert config.example[1].id == 2
 ```
 
 ### Keys and values
 
 ```python
-from configuration.common import ConfigurationBuilder
+from config.common import ConfigurationBuilder
 
 builder = ConfigurationBuilder()
 
 builder.add_map({"host": "localhost", "port": 8080})
 
 builder.add_value("port", 44555)
 
 config = builder.build()
 
 assert config.host == "localhost"
 assert config.port == 44555
 ```
 
+### User secrets
+
+The library provides a strategy to handle secrets during local development,
+storing them into the user folder.
+
+The following example shows how secrets can be configured for a project:
+
+```bash
+config secrets init
+config secrets set "Foo" "Some secret value"
+```
+
+Secrets are organized by project, and the project information is obtained from
+`pyproject.toml` files (from the `project.name` property). If `pyproject.toml`
+file does not exist, one is generated automatically with a random name.
+
+---
+
+Then, from a Python app, it's possible to load the secrets from the user folder:
+
+```python
+from config.common import ConfigurationBuilder
+from config.json import JSONFile
+from config.secrets import UserSecrets
+
+builder = ConfigurationBuilder(JSONFile("settings.json"), UserSecrets())
+
+config = builder.build()
+
+print(config)
+# config contains both values from `settings.json`, and secrets read from the user
+# folder
+```
+
+Secrets are optional and should be used only for local development, they are
+stored in unencrypted form in the user's folder.
+
+Production apps should use dedicated services to handle secrets, like
+[Azure Key Vault](https://docs.microsoft.com/en-us/azure/key-vault/general/basic-concepts),
+[AWS Secrets Manager](https://aws.amazon.com/secrets-manager/), or similar services.
+For Azure Key Vault, an implementation is provided in [essentials-configuration-keyvault](https://github.com/Neoteroi/essentials-configuration-keyvault).
+
+## Handling user secrets
+
+User secrets can be handled using the provided `config` CLI.
+
+```
+config secrets
+Usage: config secrets [OPTIONS] COMMAND [ARGS]...
+
+  Commands to handle user secrets, for local development.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  del       Delete a secret for a project, by key.
+  get       Get a secret in a user file by key.
+  info      Show information about secrets for a project.
+  init      Initialize user secrets for the current folder.
+  list      List all projects configured for secrets stored in the user...
+  set       Set a secret in a user file by key and value.
+  set-many  Set many secrets read from a JSON file passed through stdin.
+  show      Show the local secrets for a project.
+```
+
 ### Overriding nested values
 
 It is possible to override nested values by environment variables or
 dictionary keys using the following notation for sub properties:
 
 * keys separated by colon ":", such as `a:d:e`
 * keys separated by "__", such as `a__d__e`
 
 ```python
-from configuration.common import ConfigurationBuilder, MapSource
+from config.common import ConfigurationBuilder, MapSource
 
 
 builder = ConfigurationBuilder(
     MapSource(
         {
             "a": {
                 "b": 1,
@@ -312,18 +370,21 @@
 ```
 
 ### Overriding nested values using env variables
 
 ```python
 import os
 
+from config.common import ConfigurationBuilder, MapSource
+from config.env import EnvVars
+
 builder = ConfigurationBuilder(
     MapSource(
         {
-            "a": {Env
+            "a": {
                 "b": 1,
                 "c": 2,
                 "d": {
                     "e": 3,
                     "f": 4,
                 },
             }
@@ -352,34 +413,78 @@
 
 assert config.a.d.e == "5"
 ```
 
 ### Overriding values in list items using env variables
 
 ```python
+import os
+
+from config.common import ConfigurationBuilder, MapSource
+from config.env import EnvVars
+
 builder = ConfigurationBuilder(
     MapSource(
         {
             "b2c": [
                 {"tenant": "1"},
                 {"tenant": "2"},
                 {"tenant": "3"},
             ]
         }
-    )
+    ),
+    EnvVars(),
 )
 
-builder.add_value("b2c:1:tenant", "4")
+os.environ["b2c__0__tenant"] = "5"
 
 config = builder.build()
 
-assert config.b2c[0].tenant == "1"
-assert config.b2c[1].tenant == "4"
+assert config.b2c[0].tenant == "5"
+assert config.b2c[1].tenant == "2"
 assert config.b2c[2].tenant == "3"
+```
+
+### Typed config
+
+To bind configuration sections with types checking, for example to use `pydantic` to
+validate application settings, use the `config.bind` method like in
+the following example:
+
+```yaml
+# example-01.yaml
+foo:
+  value: "foo"
+  x: 100
+```
+
+```python
+# example
+from pydantic import BaseModel
+
+from config.common import ConfigurationBuilder
+from config.yaml import YAMLFile
+
+
+class FooSettings(BaseModel):
+    value: str
+    x: int
+
+
+builder = ConfigurationBuilder(YAMLFile("example-01.yaml"))
+
+config = builder.build()
+
+# the bind method accepts a variable number of fragments to
+# obtain the configuration section that should be used to instantiate the given type
+foo_settings = config.bind(FooSettings, "foo")
 
+assert isinstance(foo_settings, FooSettings)
+assert foo_settings.value == "foo"
+assert foo_settings.x == 100
 ```
 
 ### Goal and non-goals
 
 The goal of this package is to provide a way to handle configuration roots,
 fetching and composing settings from different sources, usually happening
 once at application's start.
```

### Comparing `essentials-configuration-1.0.0/configuration/common/__init__.py` & `essentials_configuration-2.0.0/config/common/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from abc import ABC, abstractmethod
 from collections import abc
-from typing import Any, Dict, List, Mapping, Optional
+from typing import Any, Dict, List, Mapping, Optional, Type, TypeVar
 
-from configuration.errors import ConfigurationOverrideError
+from config.errors import ConfigurationOverrideError
+
+T = TypeVar("T")
 
 
 def apply_key_value(obj, key, value):
     key = key.strip("_:")  # remove special characters from both ends
     for token in (":", "__"):
         if token in key:
             parts = key.split(token)
 
             sub_property = obj
             last_part = parts[-1]
             for part in parts[:-1]:
-
                 if isinstance(sub_property, abc.MutableSequence):
                     try:
                         index = int(part)
                     except ValueError:
                         raise ConfigurationOverrideError(
                             f"{part} was supposed to be a numeric index in {key}"
                         )
@@ -149,14 +150,24 @@
     @property
     def values(self) -> Dict[str, Any]:
         """
         Returns a copy of the dictionary of current settings.
         """
         return self._data.copy()
 
+    def bind(self, cls: Type[T], *path: str) -> T:
+        """
+        Returns an instance of the given type, using the current values as input.
+        This enables validation of configuration sections.
+        """
+        values = self.values
+        for fragment in path:
+            values = values[fragment]
+        return cls(**values)
+
 
 class ConfigurationBuilder:
     def __init__(self, *sources: ConfigurationSource) -> None:
         """
         Creates a new instance of ConfigurationBuilder, that can obtain a Configuration
         object from different sources. Sources are applied in the given order and can
         override each other's settings.
```

### Comparing `essentials-configuration-1.0.0/configuration/env/__init__.py` & `essentials_configuration-2.0.0/config/env/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import os
 from typing import Any, Dict, Optional
 
-from configuration.common import ConfigurationSource
+from dotenv import load_dotenv
+
+from config.common import ConfigurationSource
+from config.common.files import PathType
 
 
 class EnvironmentVariables(ConfigurationSource):
-    def __init__(self, prefix: Optional[str] = None, strip_prefix: bool = True) -> None:
+    def __init__(
+        self,
+        prefix: Optional[str] = None,
+        strip_prefix: bool = True,
+        file: Optional[PathType] = None,
+    ) -> None:
         super().__init__()
         self.prefix = prefix
         self.strip_prefix = strip_prefix
+        self._file = file
 
     def get_values(self) -> Dict[str, Any]:
+        if self._file:
+            load_dotenv(self._file)
+
         values = {}
         prefix = self.prefix
         strip_prefix = self.strip_prefix
         if prefix:
             prefix = prefix.lower()
         for key, value in os.environ.items():
             key_lower = key.lower()
```

### Comparing `essentials-configuration-1.0.0/configuration/json/__init__.py` & `essentials_configuration-2.0.0/config/common/files.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import json
-import os
-from typing import Any, Dict
-
-from configuration.common import ConfigurationSource
-from configuration.errors import MissingConfigurationFileError
+from abc import abstractmethod
+from pathlib import Path
+from typing import Any, Dict, Union
 
+from config.common import ConfigurationSource
+from config.errors import MissingConfigurationFileError
 
-class JSONFile(ConfigurationSource):
-    def __init__(
-        self, file_path: str, optional: bool = False, safe_load: bool = True
-    ) -> None:
+PathType = Union[Path, str]
+
+
+class FileConfigurationSource(ConfigurationSource):
+    def __init__(self, file_path: PathType, optional: bool = False) -> None:
         super().__init__()
-        self.file_path = file_path
+        self.file_path = Path(file_path)
         self.optional = optional
-        self.safe_load = safe_load
+
+    @abstractmethod
+    def read_source(self) -> Dict[str, Any]:
+        """
+        Reads values from the source file path. This method is not
+        used if the file does not exist.
+        """
 
     def get_values(self) -> Dict[str, Any]:
-        if not os.path.exists(self.file_path):
+        if not self.file_path.exists():
             if self.optional:
                 return {}
             raise MissingConfigurationFileError(self.file_path)
-
-        with open(self.file_path, "rt", encoding="utf-8") as source:
-            return json.load(source)
+        return self.read_source()
```

### Comparing `essentials-configuration-1.0.0/configuration/toml/__init__.py` & `essentials_configuration-2.0.0/config/toml/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-import os
 from typing import Any, Callable, Dict
 
+from config.common.files import FileConfigurationSource, PathType
+
 try:
     # Python 3.11
     import tomllib
 except ImportError:  # pragma: no cover
     # older Python
     import tomli as tomllib  # noqa
 
-from configuration.common import ConfigurationSource
-from configuration.errors import MissingConfigurationFileError
-
 
-class TOMLFile(ConfigurationSource):
+class TOMLFile(FileConfigurationSource):
     def __init__(
         self,
-        file_path: str,
+        file_path: PathType,
         optional: bool = False,
         parse_float: Callable[[str], Any] = float,
     ) -> None:
-        super().__init__()
-        self.file_path = file_path
-        self.optional = optional
+        super().__init__(file_path, optional)
         self.parse_float = parse_float
 
-    def get_values(self) -> Dict[str, Any]:
-        if not os.path.exists(self.file_path):
-            if self.optional:
-                return {}
-            raise MissingConfigurationFileError(self.file_path)
-
+    def read_source(self) -> Dict[str, Any]:
         with open(self.file_path, "rb") as source:
             return tomllib.load(source, parse_float=self.parse_float)
```

