# Comparing `tmp/openhasp_config_manager-0.4.0.tar.gz` & `tmp/openhasp_config_manager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhasp_config_manager-0.4.0.tar", max compression
+gzip compressed data, was "openhasp_config_manager-0.4.1.tar", max compression
```

## Comparing `openhasp_config_manager-0.4.0.tar` & `openhasp_config_manager-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    34523 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/LICENSE
--rw-r--r--   0        0        0    13491 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/__init__.py
--rw-r--r--   0        0        0      746 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/cmd.py
--rw-r--r--   0        0        0     3562 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/common.py
--rw-r--r--   0        0        0     1231 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/deploy.py
--rw-r--r--   0        0        0     1044 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/generate.py
--rw-r--r--   0        0        0     1152 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/listen.py
--rw-r--r--   0        0        0     1024 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/logs.py
--rw-r--r--   0        0        0     1292 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/screenshot.py
--rw-r--r--   0        0        0     1023 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/shell.py
--rw-r--r--   0        0        0     1056 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/state.py
--rw-r--r--   0        0        0     1072 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/upload.py
--rw-r--r--   0        0        0     1265 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/vars.py
--rw-r--r--   0        0        0      257 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli.py
--rw-r--r--   0        0        0      122 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/const.py
--rw-r--r--   0        0        0    16151 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/manager.py
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/__init__.py
--rw-r--r--   0        0        0      229 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/component.py
--rw-r--r--   0        0        0      958 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/config.py
--rw-r--r--   0        0        0      164 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/debug_config.py
--rw-r--r--   0        0        0      362 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/device.py
--rw-r--r--   0        0        0      190 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/device_config.py
--rw-r--r--   0        0        0      224 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/gui_config.py
--rw-r--r--   0        0        0      178 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/hasp_config.py
--rw-r--r--   0        0        0      111 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/http_config.py
--rw-r--r--   0        0        0      154 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/mqtt_config.py
--rw-r--r--   0        0        0      193 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
--rw-r--r--   0        0        0       98 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/screen_config.py
--rw-r--r--   0        0        0       97 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/telnet_config.py
--rw-r--r--   0        0        0       85 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/website_config.py
--rw-r--r--   0        0        0       97 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/wifi_config.py
--rw-r--r--   0        0        0     1420 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/mqtt_client.py
--rw-r--r--   0        0        0     8518 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/openhasp.py
--rw-r--r--   0        0        0     4822 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/telnet_client.py
--rw-r--r--   0        0        0     8705 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/webservice_client.py
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/device_processor.py
--rw-r--r--   0        0        0      369 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/__init__.py
--rw-r--r--   0        0        0     2198 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/jsonl.py
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/__init__.py
--rw-r--r--   0        0        0     2348 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
--rw-r--r--   0        0        0     5401 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/template_rendering.py
--rw-r--r--   0        0        0     5464 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/variables.py
--rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/ui/__init__.py
--rw-r--r--   0        0        0     1427 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/ui/util.py
--rw-r--r--   0        0        0     6051 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/uploader.py
--rw-r--r--   0        0        0     1798 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/util.py
--rw-r--r--   0        0        0      565 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/__init__.py
--rw-r--r--   0        0        0      649 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/cmd.py
--rw-r--r--   0        0        0     1140 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/device_validator.py
--rw-r--r--   0        0        0     2111 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/jsonl.py
--rw-r--r--   0        0        0     1255 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    14635 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/LICENSE
+-rw-r--r--   0        0        0    13491 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/cmd.py
+-rw-r--r--   0        0        0     3473 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/common.py
+-rw-r--r--   0        0        0     1231 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/deploy.py
+-rw-r--r--   0        0        0     1044 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/generate.py
+-rw-r--r--   0        0        0     1152 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/listen.py
+-rw-r--r--   0        0        0     1024 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/logs.py
+-rw-r--r--   0        0        0     1292 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/screenshot.py
+-rw-r--r--   0        0        0     1023 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/shell.py
+-rw-r--r--   0        0        0     1056 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/state.py
+-rw-r--r--   0        0        0     1072 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/upload.py
+-rw-r--r--   0        0        0     1265 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli/vars.py
+-rw-r--r--   0        0        0      257 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/cli.py
+-rw-r--r--   0        0        0      122 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/const.py
+-rw-r--r--   0        0        0    16151 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/component.py
+-rw-r--r--   0        0        0      958 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/config.py
+-rw-r--r--   0        0        0      164 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/debug_config.py
+-rw-r--r--   0        0        0      362 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/device.py
+-rw-r--r--   0        0        0      190 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/device_config.py
+-rw-r--r--   0        0        0      224 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/gui_config.py
+-rw-r--r--   0        0        0      178 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/hasp_config.py
+-rw-r--r--   0        0        0      111 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/http_config.py
+-rw-r--r--   0        0        0      154 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/mqtt_config.py
+-rw-r--r--   0        0        0      193 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
+-rw-r--r--   0        0        0       98 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/screen_config.py
+-rw-r--r--   0        0        0       97 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/telnet_config.py
+-rw-r--r--   0        0        0       85 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/website_config.py
+-rw-r--r--   0        0        0       97 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/wifi_config.py
+-rw-r--r--   0        0        0     1420 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/mqtt_client.py
+-rw-r--r--   0        0        0     8518 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/openhasp.py
+-rw-r--r--   0        0        0     4822 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/telnet_client.py
+-rw-r--r--   0        0        0     8705 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/webservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/device_processor.py
+-rw-r--r--   0        0        0      369 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/jsonl/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/jsonl/jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2479 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
+-rw-r--r--   0        0        0     5401 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/template_rendering.py
+-rw-r--r--   0        0        0     5464 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/processing/variables.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/ui/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/ui/util.py
+-rw-r--r--   0        0        0     6053 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/uploader.py
+-rw-r--r--   0        0        0     1798 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/util.py
+-rw-r--r--   0        0        0      565 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/validation/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/validation/cmd.py
+-rw-r--r--   0        0        0     1140 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/validation/device_validator.py
+-rw-r--r--   0        0        0     2111 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/openhasp_config_manager/validation/jsonl.py
+-rw-r--r--   0        0        0     1255 2023-04-08 16:33:48.684636 openhasp_config_manager-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    14635 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.1/PKG-INFO
```

### Comparing `openhasp_config_manager-0.4.0/LICENSE` & `openhasp_config_manager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/README.md` & `openhasp_config_manager-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/__init__.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/cmd.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/common.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,31 @@
 
 
 async def _generate(config_manager: ConfigManager, device: Device):
     info(f"Generating output for '{device.name}'...")
     try:
         config_manager.process(device)
     except Exception as ex:
-        raise Exception(f"Error generating output for {device.name}: {ex}")
+        raise Exception(f"Error generating output for {device.name}: {ex.__class__.__name__} {ex}")
 
 
 async def _upload(device: Device, output_dir: Path, purge: bool, show_diff: bool):
     from openhasp_config_manager.openhasp_client.openhasp import OpenHaspClient
     from openhasp_config_manager.uploader import ConfigUploader
 
     client = OpenHaspClient(device)
     uploader = ConfigUploader(output_dir, client)
-    try:
-        info(f"Uploading files to device '{device.name}'...")
-        return uploader.upload(device, purge, show_diff)
-    except Exception as ex:
-        raise Exception(f"Error uploading files to '{device.name}': {ex}")
+
+    info(f"Uploading files to device '{device.name}'...")
+    return uploader.upload(device, purge, show_diff)
 
 
 async def _deploy(config_manager: ConfigManager, device: Device, output_dir: Path, purge: bool, show_diff: bool):
     await _generate(config_manager, device)
-    changed = _upload(device, output_dir, purge, show_diff)
+    changed = await _upload(device, output_dir, purge, show_diff)
     # _cmd(config_dir, device="touch_down_1", command="reboot", payload="")
     # _reload(config_dir, device)
     if changed:
         info(f"Rebooting {device.name} to apply changes")
         await _reboot(device)
     else:
         info(f"No changes detected for {device.name}, device is already up-to-date")
```

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/deploy.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/generate.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/generate.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/listen.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/listen.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/logs.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/logs.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/screenshot.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/screenshot.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/shell.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/shell.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/state.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/state.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/upload.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/upload.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/vars.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/cli/vars.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/manager.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/manager.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/config.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/model/config.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/mqtt_client.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/openhasp.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/openhasp.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/telnet_client.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/telnet_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/webservice_client.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/openhasp_client/webservice_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/device_processor.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/processing/device_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/jsonl.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/processing/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,29 +38,31 @@
 
     def _remove_comments(self, content: str) -> str:
         """
         Removes comments indicated by "//"
         :param content: original content
         :return: modified content without comments
         """
-        result_lines1 = [line for line in content.splitlines() if not line.strip().startswith("//")]
-
-        result_lines2 = []
-        for line in result_lines1:
-            if line.strip().startswith("//"):
-                continue
-
-            parts = re.split("(?!,)(\s*//.*)$", line)
-            parts = [part.strip() for part in parts if len(part.strip()) > 0]
-            keep = parts[0:max(1, len(parts) - 1)]
-
-            line = "".join(keep)
-            result_lines2.append(line)
-
-        result = "\n".join(result_lines2)
+        result_lines = []
+        for line in content.splitlines():
+            quote_count = 0
+            new_line = []
+            i = 0
+            while i < len(line):
+                char = line[i]
+                if char == '"':
+                    quote_count += 1
+                if char == '/' and i + 1 < len(line) and line[i + 1] == '/' and quote_count % 2 == 0:
+                    break
+                new_line.append(char)
+                i += 1
+            cleaned_line = "".join(new_line).strip()
+            if cleaned_line:  # Only append non-empty lines
+                result_lines.append(cleaned_line)
+        result = "\n".join(result_lines)
         return result.strip()
 
     def _remove_trailing_comma_of_last_property(self, content: str) -> str:
         """
         Removes the "," of the last property within the object.
         :param content: original content
         :return: modified content
```

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/template_rendering.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/processing/template_rendering.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/variables.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/processing/variables.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/ui/util.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/ui/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/uploader.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         return Path(
             self._cache_dir,
             *file.relative_to(self._output_root).parts[:-1],
             file.name + ".md5"
         )
 
     def _update_config(self, device: Device):
-        current_mqtt_config = self._api_client.get_mqtt_config()
+        # current_mqtt_config = self._api_client.get_mqtt_config()
         # TODO: compare existing config with new config and only update if necessary
 
         self._api_client.set_mqtt_config(device.config.mqtt)
         self._api_client.set_http_config(device.config.http)
         self._api_client.set_gui_config(device.config.gui)
 
         # TODO: return True if config has changed
```

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/util.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/__init__.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/cmd.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/validation/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/device_validator.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/validation/device_validator.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/jsonl.py` & `openhasp_config_manager-0.4.1/openhasp_config_manager/validation/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.0/pyproject.toml` & `openhasp_config_manager-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openhasp-config-manager"
-version = "0.4.0"
+version = "0.4.1"
 description = "A tool to manage all of your openHASP device configs in a centralized place."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
```

### Comparing `openhasp_config_manager-0.4.0/PKG-INFO` & `openhasp_config_manager-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhasp-config-manager
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool to manage all of your openHASP device configs in a centralized place.
 Home-page: https://github.com/markusressel/openhasp-config-manager
 License: AGPL-3.0-or-later
 Keywords: openhasp,config,management
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
```

