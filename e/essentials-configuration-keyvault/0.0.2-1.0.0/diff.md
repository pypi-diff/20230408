# Comparing `tmp/essentials-configuration-keyvault-0.0.2.tar.gz` & `tmp/essentials_configuration_keyvault-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "essentials-configuration-keyvault-0.0.2.tar", last modified: Wed Aug 11 22:17:33 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `essentials-configuration-keyvault-0.0.2.tar` & `essentials_configuration_keyvault-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-11 22:17:33.805393 essentials-configuration-keyvault-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1065 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3728 2021-08-11 22:17:33.805393 essentials-configuration-keyvault-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2845 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-11 22:17:33.801393 essentials-configuration-keyvault-0.0.2/configuration/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-11 22:17:33.805393 essentials-configuration-keyvault-0.0.2/configuration/keyvault/
--rw-r--r--   0 runner    (1001) docker     (116)      983 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/configuration/keyvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/configuration/keyvault/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-11 22:17:33.805393 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3728 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      445 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2021-08-11 22:17:33.000000 essentials-configuration-keyvault-0.0.2/essentials_configuration_keyvault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-08-11 22:17:33.805393 essentials-configuration-keyvault-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1276 2021-08-11 22:17:12.000000 essentials-configuration-keyvault-0.0.2/setup.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/config/keyvault/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/config/keyvault/py.typed
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/README.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 essentials_configuration_keyvault-1.0.0/PKG-INFO
```

### Comparing `essentials-configuration-keyvault-0.0.2/LICENSE` & `essentials_configuration_keyvault-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials-configuration-keyvault-0.0.2/PKG-INFO` & `essentials_configuration_keyvault-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: essentials-configuration-keyvault
-Version: 0.0.2
-Summary: Azure Key Vault source for essentials-configuration
-Home-page: https://github.com/Neoteroi/essentials-configuration-keyvault
-Author: RobertoPrevato
-Author-email: roberto.prevato@gmail.com
-License: MIT
-Keywords: Azure Key Vault secrets configuration environment
-Platform: UNKNOWN
+Version: 1.0.0
+Summary: Azure Key Vault source for essentials-configuration.
+Project-URL: Homepage, https://github.com/Neoteroi/essentials-configuration-keyvault
+Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-configuration-keyvault/issues
+Author-email: Roberto Prevato <roberto.prevato@gmail.com>
+License-File: LICENSE
+Keywords: Azure Key Vault,configuration,environment,secrets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Requires-Dist: azure-identity~=1.12.0
+Requires-Dist: azure-keyvault-secrets~=4.7.0
+Requires-Dist: essentials-configuration~=2.0.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ![Build](https://github.com/Neoteroi/essentials-configuration-keyvault/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/essentials-configuration-keyvault.svg)](https://pypi.python.org/pypi/essentials-configuration-keyvault)
 [![versions](https://img.shields.io/pypi/pyversions/essentials-configuration-keyvault.svg)](https://github.com/Neoteroi/essentials-configuration-keyvault)
 [![codecov](https://codecov.io/gh/Neoteroi/essentials-configuration-keyvault/branch/main/graph/badge.svg)](https://codecov.io/gh/Neoteroi/essentials-configuration-keyvault)
 [![license](https://img.shields.io/github/license/Neoteroi/essentials-configuration-keyvault.svg)](https://github.com/Neoteroi/essentials-configuration-keyvault/blob/main/LICENSE)
 
@@ -46,16 +47,16 @@
 in Azure Key Vault into configuration objects.
 
 Example:
 
 ```python
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
-from configuration.common import ConfigurationBuilder
-from configuration.keyvault import KeyVaultSource
+from config.common import ConfigurationBuilder
+from config.keyvault import KeyVaultSource
 
 key_vault_name = "example-keyvault-name"
 
 secrets_client = SecretClient(
     vault_url=f"https://{key_vault_name}.vault.azure.net",
     credential=DefaultAzureCredential(),
 )
@@ -68,19 +69,19 @@
 config = builder.build()
 ```
 
 > Refer to the [official Key Vault documentation for more
 > information about its Python client library.](https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python).
 
 ## How to run the tests using a real Key Vault
-The provided tests can either use a mocked `SecretClient`, or use a real Key Vault. 
+
+The provided tests can either use a mocked `SecretClient`, or use a real Key Vault.
 To use a real Key Vault service:
 
 1. create a Key Vault ([ref.](https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python))
-2. sign-in using any way supported by `azure.identity.DefaultAzureCredential` (e.g. VS Code or `az login`)
+2. sign-in using any way supported by `azure.identity.DefaultAzureCredential` 3
+   (e.g. VS Code or `az login`)
 3. run the tests with the following command:
 
 ```bash
 KEYVAULT_NAME="<YOUR_KEYVAULT_NAME>" pytest -s
 ```
-
-
```

### Comparing `essentials-configuration-keyvault-0.0.2/README.md` & `essentials_configuration_keyvault-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 in Azure Key Vault into configuration objects.
 
 Example:
 
 ```python
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
-from configuration.common import ConfigurationBuilder
-from configuration.keyvault import KeyVaultSource
+from config.common import ConfigurationBuilder
+from config.keyvault import KeyVaultSource
 
 key_vault_name = "example-keyvault-name"
 
 secrets_client = SecretClient(
     vault_url=f"https://{key_vault_name}.vault.azure.net",
     credential=DefaultAzureCredential(),
 )
@@ -46,17 +46,19 @@
 config = builder.build()
 ```
 
 > Refer to the [official Key Vault documentation for more
 > information about its Python client library.](https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python).
 
 ## How to run the tests using a real Key Vault
-The provided tests can either use a mocked `SecretClient`, or use a real Key Vault. 
+
+The provided tests can either use a mocked `SecretClient`, or use a real Key Vault.
 To use a real Key Vault service:
 
 1. create a Key Vault ([ref.](https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python))
-2. sign-in using any way supported by `azure.identity.DefaultAzureCredential` (e.g. VS Code or `az login`)
+2. sign-in using any way supported by `azure.identity.DefaultAzureCredential` 3
+   (e.g. VS Code or `az login`)
 3. run the tests with the following command:
 
 ```bash
 KEYVAULT_NAME="<YOUR_KEYVAULT_NAME>" pytest -s
 ```
```

### Comparing `essentials-configuration-keyvault-0.0.2/configuration/keyvault/__init__.py` & `essentials_configuration_keyvault-1.0.0/config/keyvault/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, Iterable, Tuple
 
 from azure.keyvault.secrets import SecretClient
-from configuration.common import ConfigurationSource
+from config.common import ConfigurationSource
 
 
 class KeyVaultSource(ConfigurationSource):
     def __init__(self, client: SecretClient) -> None:
         """
         Creates a ConfigurationSource object that reads all secrets in a
         Azure Key Vault, using the given SecretClient.
```

### Comparing `essentials-configuration-keyvault-0.0.2/setup.py` & `essentials_configuration_keyvault-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-from setuptools import setup
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
+[project]
+name = "essentials-configuration-keyvault"
+version = "1.0.0"
+authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
+description = "Azure Key Vault source for essentials-configuration."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+]
+keywords = ["Azure Key Vault", "secrets", "configuration", "environment"]
 
-def readme():
-    with open("README.md") as f:
-        return f.read()
+dependencies = ["essentials-configuration~=2.0.0", "azure-identity~=1.12.0", "azure-keyvault-secrets~=4.7.0"]
 
+[tool.hatch.build.targets.sdist]
+exclude = [
+    "/.github",
+    "/docs",
+    "/deps",
+    "/htmlcov",
+    "/tests",
+    "Makefile",
+    "CODE_OF_CONDUCT.md",
+    ".isort.cfg",
+    ".gitignore",
+    ".flake8",
+    "junit",
+    "requirements.txt",
+    "mypy.ini",
+    "pytest.ini",
+    "venv",
+]
 
-setup(
-    name="essentials-configuration-keyvault",
-    version="0.0.2",
-    description=("Azure Key Vault source for essentials-configuration"),
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Operating System :: OS Independent",
-    ],
-    url="https://github.com/Neoteroi/essentials-configuration-keyvault",
-    author="RobertoPrevato",
-    author_email="roberto.prevato@gmail.com",
-    keywords="Azure Key Vault secrets configuration environment",
-    license="MIT",
-    packages=["configuration.keyvault"],
-    install_requires=[
-        "azure-identity==1.6.0",
-        "azure-keyvault-secrets==4.3.0",
-        "essentials-configuration>=0.0.2",
-    ],
-    include_package_data=True,
-    zip_safe=False,
-)
+[project.urls]
+"Homepage" = "https://github.com/Neoteroi/essentials-configuration-keyvault"
+"Bug Tracker" = "https://github.com/Neoteroi/essentials-configuration-keyvault/issues"
```

