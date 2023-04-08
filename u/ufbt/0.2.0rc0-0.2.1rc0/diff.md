# Comparing `tmp/ufbt-0.2.0rc0.tar.gz` & `tmp/ufbt-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.0rc0.tar", last modified: Thu Apr  6 14:07:44 2023, max compression
+gzip compressed data, was "ufbt-0.2.1rc0.tar", last modified: Sat Apr  8 20:13:55 2023, max compression
```

## Comparing `ufbt-0.2.0rc0.tar` & `ufbt-0.2.1rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:07:44.991598 ufbt-0.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-06 14:07:44.991598 ufbt-0.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-06 14:07:33.000000 ufbt-0.2.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-06 14:07:33.000000 ufbt-0.2.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 14:07:44.991598 ufbt-0.2.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:07:44.991598 ufbt-0.2.0rc0/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-06 14:07:33.000000 ufbt-0.2.0rc0/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-06 14:07:33.000000 ufbt-0.2.0rc0/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23426 2023-04-06 14:07:33.000000 ufbt-0.2.0rc0/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:07:44.991598 ufbt-0.2.0rc0/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-06 14:07:44.000000 ufbt-0.2.0rc0/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-06 14:07:44.000000 ufbt-0.2.0rc0/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:07:44.000000 ufbt-0.2.0rc0/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 14:07:44.000000 ufbt-0.2.0rc0/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 14:07:44.000000 ufbt-0.2.0rc0/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25056 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.0rc0/PKG-INFO` & `ufbt-0.2.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.0rc0
+Version: 0.2.1rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.0rc0/README.md` & `ufbt-0.2.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.0rc0/pyproject.toml` & `ufbt-0.2.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.0rc0/ufbt/__init__.py` & `ufbt-0.2.1rc0/ufbt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import pathlib
 import platform
 import sys
 
-from .bootstrap import bootstrap_cli, bootstrap_subcommands
+from .bootstrap import bootstrap_cli, bootstrap_subcommands, get_ufbt_package_version
+
+__version__ = get_ufbt_package_version()
 
 
 def ufbt_cli():
     if not os.environ.get("UFBT_STATE_DIR"):
         os.environ["UFBT_STATE_DIR"] = os.path.expanduser("~/.ufbt")
     if not os.environ.get("FBT_TOOLCHAIN_PATH"):
         os.environ["FBT_TOOLCHAIN_PATH"] = os.environ["UFBT_STATE_DIR"]
```

### Comparing `ufbt-0.2.0rc0/ufbt/bootstrap.py` & `ufbt-0.2.1rc0/ufbt/bootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,34 @@
 from dataclasses import dataclass, field
 from html.parser import HTMLParser
 from pathlib import Path, PurePosixPath
 from typing import ClassVar, Dict, Optional
 from urllib.parse import unquote, urlparse
 from urllib.request import Request, urlopen
 from zipfile import ZipFile
+from importlib.metadata import version
 
 logging.basicConfig(
     format="%(asctime)s.%(msecs)03d [%(levelname).1s] %(message)s",
     level=logging.INFO,
     datefmt="%H:%M:%S",
 )
 log = logging.getLogger(__name__)
 
 ##############################################################################
 
 
+def get_ufbt_package_version():
+    try:
+        return version("ufbt")
+    except Exception as e:
+        log.debug(f"Failed to get ufbt version: {e}")
+        return "unknown"
+
+
 class FileType(enum.Enum):
     SDK_ZIP = "sdk_zip"
     LIB_ZIP = "lib_zip"
     CORE2_FIRMWARE_TGZ = "core2_firmware_tgz"
     RESOURCES_TGZ = "resources_tgz"
     SCRIPTS_TGZ = "scripts_tgz"
     UPDATE_TGZ = "update_tgz"
@@ -240,15 +249,14 @@
 
         log.info(f"Using version: {versions[0]['version']}")
         log.debug(f"Changelog: {versions[0].get('changelog', 'None')}")
         return versions[0]
 
     @staticmethod
     def _get_file_info(version_data: dict, file_type: FileType, file_target: str):
-
         if not (files := version_data.get("files", [])):
             raise ValueError(f"Empty files list")
 
         if not (
             file_info := next(
                 (
                     f
@@ -635,32 +643,80 @@
 class StatusSubcommand(CliSubcommand):
     COMMAND = "status"
 
     def __init__(self):
         super().__init__(self.COMMAND, "Show uFBT SDK status")
 
     def _add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        pass
+        parser.add_argument(
+            "--json",
+            help="Print status in JSON format",
+            action="store_true",
+            default=False,
+        )
+
+        parser.add_argument(
+            "status_key",
+            help="Print only specific status key",
+            nargs="?",
+        )
 
     def _func(self, args) -> int:
+        fields = {
+            "ufbt_version": "uFBT version",
+            "state_dir": "State dir",
+            "download_dir": "Download dir",
+            "sdk_dir": "SDK dir",
+            "target": "Target",
+            "mode": "Mode",
+            "version": "Version",
+            "details": "Details",
+            "error": "Error",
+        }
+
+        ufbt_version = self.get_ufbt_package_version()
+
         sdk_deployer = UfbtSdkDeployer(args.ufbt_home)
-        log.info(f"State dir     {sdk_deployer.ufbt_state_dir}")
-        log.info(f"Download dir  {sdk_deployer.download_dir}")
-        log.info(f"SDK dir       {sdk_deployer.current_sdk_dir}")
+        state_data = {
+            "ufbt_version": ufbt_version,
+            "state_dir": str(sdk_deployer.ufbt_state_dir.absolute()),
+            "download_dir": str(sdk_deployer.download_dir.absolute()),
+            "sdk_dir": str(sdk_deployer.current_sdk_dir.absolute()),
+        }
+
         if previous_task := sdk_deployer.get_previous_task():
-            log.info(f"Target        {previous_task.hw_target}")
-            log.info(f"Mode          {previous_task.mode}")
-            log.info(
-                f"Version       {previous_task.all_params.get('version', BaseSdkLoader.VERSION_UNKNOWN)}"
+            state_data.update(
+                {
+                    "target": previous_task.hw_target,
+                    "mode": previous_task.mode,
+                    "version": previous_task.all_params.get(
+                        "version", BaseSdkLoader.VERSION_UNKNOWN
+                    ),
+                    "details": previous_task.all_params,
+                }
             )
-            log.info(f"Details       {previous_task.all_params}")
-            return 0
         else:
-            log.error("SDK is not deployed")
-            return 1
+            state_data.update({"error": "SDK is not deployed"})
+
+        if key := args.status_key:
+            if key not in state_data:
+                log.error(f"Unknown status key {key}")
+                return 1
+            if args.json:
+                print(json.dumps(state_data[key], indent=4))
+            else:
+                print(state_data.get(key, ""))
+        else:
+            if args.json:
+                print(json.dumps(state_data, indent=4))
+            else:
+                for key, value in state_data.items():
+                    log.info(f"{fields[key]:<15} {value}")
+
+        return 1 if state_data.get("error") else 0
 
 
 bootstrap_subcommand_classes = (UpdateSubcommand, CleanSubcommand, StatusSubcommand)
 
 bootstrap_subcommands = (
     subcommand_cls.COMMAND for subcommand_cls in bootstrap_subcommand_classes
 )
@@ -705,15 +761,15 @@
     if args.no_check_certificate:
         # Temporary fix for SSL negotiation failure on Mac
         import ssl
 
         _ssl_context = ssl.create_default_context()
         _ssl_context.check_hostname = False
         _ssl_context.verify_mode = ssl.CERT_NONE
-        BaseSdkLoader.SSL_CONTEXT = _ssl_context
+        BaseSdkLoader._SSL_CONTEXT = _ssl_context
 
     if "func" not in args:
         root_parser.print_help()
         return 1
 
     try:
         return args.func(args)
```

### Comparing `ufbt-0.2.0rc0/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.1rc0/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.0rc0
+Version: 0.2.1rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

