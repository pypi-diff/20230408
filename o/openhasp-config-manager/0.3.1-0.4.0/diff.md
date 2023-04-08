# Comparing `tmp/openhasp_config_manager-0.3.1.tar.gz` & `tmp/openhasp_config_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhasp_config_manager-0.3.1.tar", max compression
+gzip compressed data, was "openhasp_config_manager-0.4.0.tar", max compression
```

## Comparing `openhasp_config_manager-0.3.1.tar` & `openhasp_config_manager-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,56 @@
--rw-r--r--   0        0        0    34523 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/LICENSE
--rw-r--r--   0        0        0    12701 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/__init__.py
--rw-r--r--   0        0        0     8422 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/__init__.py
--rw-r--r--   0        0        0      734 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/cmd.py
--rw-r--r--   0        0        0     3306 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/common.py
--rw-r--r--   0        0        0     1219 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/deploy.py
--rw-r--r--   0        0        0     1032 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/generate.py
--rw-r--r--   0        0        0     1286 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/screenshot.py
--rw-r--r--   0        0        0     1060 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/upload.py
--rw-r--r--   0        0        0     1247 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli/vars.py
--rw-r--r--   0        0        0      257 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/cli.py
--rw-r--r--   0        0        0      122 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/const.py
--rw-r--r--   0        0        0    15019 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/manager.py
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/__init__.py
--rw-r--r--   0        0        0      229 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/component.py
--rw-r--r--   0        0        0      640 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/config.py
--rw-r--r--   0        0        0      362 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/device.py
--rw-r--r--   0        0        0      190 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/device_config.py
--rw-r--r--   0        0        0      224 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/gui_config.py
--rw-r--r--   0        0        0      178 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/hasp_config.py
--rw-r--r--   0        0        0      111 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/http_config.py
--rw-r--r--   0        0        0      154 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/mqtt_config.py
--rw-r--r--   0        0        0      193 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
--rw-r--r--   0        0        0       98 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/screen_config.py
--rw-r--r--   0        0        0       85 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/website_config.py
--rw-r--r--   0        0        0     1141 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/mqtt_client.py
--rw-r--r--   0        0        0     9589 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/openhasp.py
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/__init__.py
--rw-r--r--   0        0        0     6089 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/device_processor.py
--rw-r--r--   0        0        0      369 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/jsonl/__init__.py
--rw-r--r--   0        0        0     2198 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/jsonl/jsonl.py
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/preprocessor/__init__.py
--rw-r--r--   0        0        0     2348 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
--rw-r--r--   0        0        0     5401 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/template_rendering.py
--rw-r--r--   0        0        0     5464 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/processing/variables.py
--rw-r--r--   0        0        0        0 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/ui/__init__.py
--rw-r--r--   0        0        0     1427 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/ui/util.py
--rw-r--r--   0        0        0     5080 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/uploader.py
--rw-r--r--   0        0        0     1798 2023-03-30 19:35:33.047199 openhasp_config_manager-0.3.1/openhasp_config_manager/util.py
--rw-r--r--   0        0        0      565 2023-03-30 19:35:33.051200 openhasp_config_manager-0.3.1/openhasp_config_manager/validation/__init__.py
--rw-r--r--   0        0        0      649 2023-03-30 19:35:33.051200 openhasp_config_manager-0.3.1/openhasp_config_manager/validation/cmd.py
--rw-r--r--   0        0        0     1140 2023-03-30 19:35:33.051200 openhasp_config_manager-0.3.1/openhasp_config_manager/validation/device_validator.py
--rw-r--r--   0        0        0     2111 2023-03-30 19:35:33.051200 openhasp_config_manager-0.3.1/openhasp_config_manager/validation/jsonl.py
--rw-r--r--   0        0        0     1235 2023-03-30 19:35:33.051200 openhasp_config_manager-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    13816 1970-01-01 00:00:00.000000 openhasp_config_manager-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/LICENSE
+-rw-r--r--   0        0        0    13491 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/cmd.py
+-rw-r--r--   0        0        0     3562 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/common.py
+-rw-r--r--   0        0        0     1231 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/deploy.py
+-rw-r--r--   0        0        0     1044 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/generate.py
+-rw-r--r--   0        0        0     1152 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/listen.py
+-rw-r--r--   0        0        0     1024 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/logs.py
+-rw-r--r--   0        0        0     1292 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/screenshot.py
+-rw-r--r--   0        0        0     1023 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/shell.py
+-rw-r--r--   0        0        0     1056 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/state.py
+-rw-r--r--   0        0        0     1072 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/upload.py
+-rw-r--r--   0        0        0     1265 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli/vars.py
+-rw-r--r--   0        0        0      257 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/cli.py
+-rw-r--r--   0        0        0      122 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/const.py
+-rw-r--r--   0        0        0    16151 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/component.py
+-rw-r--r--   0        0        0      958 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/config.py
+-rw-r--r--   0        0        0      164 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/debug_config.py
+-rw-r--r--   0        0        0      362 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/device.py
+-rw-r--r--   0        0        0      190 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/device_config.py
+-rw-r--r--   0        0        0      224 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/gui_config.py
+-rw-r--r--   0        0        0      178 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/hasp_config.py
+-rw-r--r--   0        0        0      111 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/http_config.py
+-rw-r--r--   0        0        0      154 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/mqtt_config.py
+-rw-r--r--   0        0        0      193 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
+-rw-r--r--   0        0        0       98 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/screen_config.py
+-rw-r--r--   0        0        0       97 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/telnet_config.py
+-rw-r--r--   0        0        0       85 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/website_config.py
+-rw-r--r--   0        0        0       97 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/wifi_config.py
+-rw-r--r--   0        0        0     1420 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/mqtt_client.py
+-rw-r--r--   0        0        0     8518 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/openhasp.py
+-rw-r--r--   0        0        0     4822 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/telnet_client.py
+-rw-r--r--   0        0        0     8705 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/webservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/device_processor.py
+-rw-r--r--   0        0        0      369 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
+-rw-r--r--   0        0        0     5401 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/template_rendering.py
+-rw-r--r--   0        0        0     5464 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/processing/variables.py
+-rw-r--r--   0        0        0        0 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/ui/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/ui/util.py
+-rw-r--r--   0        0        0     6051 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/uploader.py
+-rw-r--r--   0        0        0     1798 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/util.py
+-rw-r--r--   0        0        0      565 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/cmd.py
+-rw-r--r--   0        0        0     1140 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/device_validator.py
+-rw-r--r--   0        0        0     2111 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/openhasp_config_manager/validation/jsonl.py
+-rw-r--r--   0        0        0     1255 2023-04-07 23:45:02.731626 openhasp_config_manager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14635 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.0/PKG-INFO
```

### Comparing `openhasp_config_manager-0.3.1/LICENSE` & `openhasp_config_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/README.md` & `openhasp_config_manager-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,39 @@
     * [x] local and globally scoped variables
 * [x] validation of common mistakes for
     * [x] jsonl objects
     * [x] cmd files
 * [x] simple configuration upload to the device(s)
     * [x] automatic diffing to only update changed configuration files
     * [x] git-style diff output for changed lines
-* [x] device command execution directly from the CLI (still needs a connection to the MQTT broker)
+* [x] API client (Web + MQTT)
+    * [x] execute commands on a plate
+    * [x] listen to events and state updates
+
+```shell
+> openhasp-config-manager -h
+Usage: openhasp-config-manager [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version   Show the version and exit.
+  -h, --help  Show this message and exit.
+
+Commands:
+  cmd         Sends a command request to a device.
+  deploy      Combines the generation and upload of a configuration.
+  generate    Generates the output files for all devices in the given...
+  help        Show this message and exit.
+  listen      Sends a state update request to a device.
+  logs        Prints the logs of a device.
+  screenshot  Requests a screenshot from the given device and stores it...
+  shell       Connects to the telnet server of a device.
+  state       Sends a state update request to a device.
+  upload      Uploads the previously generated configuration to their...
+  vars        Prints the variables accessible in a given path.
+```
 
 # Disclaimer
 
 **TL;DR: This project is still experimental.**
 
 I do use openhasp-config-manager exclusively to configure all of my openHASP devices. I am in the
 process of adding tests to everything to make it more reliable and have also added lots of features along the way.
@@ -341,30 +365,20 @@
 ...
 header.title: Home
 ```
 
 ## Deployment
 
 To deploy your configurations to the already connected openHASP devices, simply use the
-command line tool `openhasp-config-manager`:
-
-```shell
-> openhasp-config-manager                                                         0 (0.604s) < 02:11:38
-Usage: openhasp-config-manager [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --version   Show the version and exit.
-  -h, --help  Show this message and exit.
+`generate`, `upload` or `deploy` commands of `openhasp-config-manager`.
 
-Commands:
-  cmd       Sends a command request to a device.
-  deploy    Combines the generation and upload of a configuration.
-  generate  Generates the output files for all devices in the given...
-  upload    Uploads the previously generated configuration to their...
-```
+> **Note**
+> openhasp-config-manager needs direct IP access as well as an enabled webservice on the plate
+> to be able to deploy files to the device. To enable the webservice
+> try: `openhasp-config-manager cmd -d plate35 -C service -p "start http"`
 
 ## Run commands
 
 While openhasp-config-manager is first and foremost a config management system,
 it also allows you to run commands on a device by issuing MQTT messages without the need to install a separate
 MQTT client first. Note that the MQTT _server_ still needs to be running and also has to
 be reachable from your local machine for this to work.
@@ -376,15 +390,21 @@
 > openhasp-config-manager cmd -c ./openhasp-configs -d plate35 -C backlight -p "{\"state\":\"on\",\"brightness\":128}"
 ```
 
 # FAQ
 
 ## How do I see device logs?
 
-With the device connected via USB cable, open a terminal and run:
+Try the `logs` command (this does require network access to the device):
+
+```shell
+> openhasp-config-manager logs -d plate35
+```
+
+If that doesn't work, open a terminal and run the following command with the device connected via USB cable:
 
 ```shell
 bash -c "screen -q -L -Logfile device.log /dev/ttyUSB0 115200 &> /dev/null; tail -F device.log; killall screen"
 ```
 
 ## Output file name length must not exceed 30 characters
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/__init__.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,36 @@
+import asyncio
 import pathlib
 from pathlib import Path
 
 import click
 
 from openhasp_config_manager.cli.cmd import c_cmd
 from openhasp_config_manager.cli.deploy import c_deploy
 from openhasp_config_manager.cli.generate import c_generate
+from openhasp_config_manager.cli.listen import c_listen
+from openhasp_config_manager.cli.logs import c_logs
 from openhasp_config_manager.cli.screenshot import c_screenshot
+from openhasp_config_manager.cli.shell import c_shell
+from openhasp_config_manager.cli.state import c_state
 from openhasp_config_manager.cli.upload import c_upload
 from openhasp_config_manager.cli.vars import c_vars
 from openhasp_config_manager.ui.util import echo
 
 PARAM_CFG_DIR = "cfg_dir"
 PARAM_OUTPUT_DIR = "output_dir"
 PARAM_DEVICE = "device"
 PARAM_PURGE = "purge"
 PARAM_SHOW_DIFF = "diff"
 PARAM_CMD = "cmd"
 PARAM_PAYLOAD = "payload"
 PARAM_PATH = "path"
+PARAM_OBJECT = "object"
+PARAM_STATE = "state"
+PARAM_MQTT_PATH = "mqtt_path"
 
 DEFAULT_CONFIG_PATH = Path("./openhasp-configs")
 DEFAULT_OUTPUT_PATH = Path("./output")
 DEFAULT_SCREENSHOT_OUTPUT_PATH = Path("./")
 
 CMD_OPTION_NAMES = {
     PARAM_CFG_DIR: {
@@ -55,14 +63,26 @@
     PARAM_SHOW_DIFF: {
         "names": ["--diff", "-D"],
         "help": """Whether to show a diff for files uploaded to the target device.""",
     },
     PARAM_PATH: {
         "names": ["--path", "-p"],
         "help": """The subpath inside the configuration directory"""
+    },
+    PARAM_OBJECT: {
+        "names": ["--object", "-o"],
+        "help": """The object identifier, f.ex. p1b15"""
+    },
+    PARAM_STATE: {
+        "names": ["--state", "-s"],
+        "help": """The state to set. Can also be a json object to set multiple properties in one go."""
+    },
+    PARAM_MQTT_PATH: {
+        "names": ["--path", "-p"],
+        "help": """The MQTT sub-path (hasp/<device>/<path>) to listen to."""
     }
 }
 
 
 def get_option_names(parameter: str) -> list:
     """
     Returns a list of all valid console parameter names for a given parameter
@@ -112,15 +132,17 @@
               help=get_option_help(PARAM_OUTPUT_DIR))
 @click.option(*get_option_names(PARAM_DEVICE), required=False, default=None,
               help=get_option_help(PARAM_DEVICE))
 def generate(config_dir: Path, output_dir: Path, device: str):
     """
     Generates the output files for all devices in the given config directory.
     """
-    c_generate(config_dir, output_dir, device)
+    asyncio.run(
+        c_generate(config_dir, output_dir, device)
+    )
 
 
 @cli.command(name="deploy")
 @click.option(*get_option_names(PARAM_CFG_DIR),
               required=False,
               default=DEFAULT_CONFIG_PATH,
               type=click.Path(exists=True, path_type=Path),
@@ -136,15 +158,17 @@
               help=get_option_help(PARAM_PURGE))
 @click.option(*get_option_names(PARAM_SHOW_DIFF), is_flag=True,
               help=get_option_help(PARAM_SHOW_DIFF))
 def deploy(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
     """
     Combines the generation and upload of a configuration.
     """
-    c_deploy(config_dir, output_dir, device, purge, diff)
+    asyncio.run(
+        c_deploy(config_dir, output_dir, device, purge, diff)
+    )
 
 
 @cli.command(name="upload")
 @click.option(*get_option_names(PARAM_CFG_DIR),
               required=False,
               default=DEFAULT_CONFIG_PATH,
               type=click.Path(exists=True, path_type=Path),
@@ -160,25 +184,82 @@
               help=get_option_help(PARAM_PURGE))
 @click.option(*get_option_names(PARAM_SHOW_DIFF), is_flag=True,
               help=get_option_help(PARAM_SHOW_DIFF))
 def upload(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
     """
     Uploads the previously generated configuration to their corresponding devices.
     """
-    c_upload(config_dir, output_dir, device, purge, diff)
+    asyncio.run(
+        c_upload(config_dir, output_dir, device, purge, diff)
+    )
 
 
-@cli.command(name="cmd")
+@cli.command(name="logs")
+@click.option(*get_option_names(PARAM_CFG_DIR),
+              required=False,
+              default=DEFAULT_CONFIG_PATH,
+              type=click.Path(exists=True, path_type=Path),
+              help=get_option_help(PARAM_CFG_DIR))
+@click.option(*get_option_names(PARAM_DEVICE), required=True, default=None,
+              help=get_option_help(PARAM_DEVICE))
+def logs(config_dir: Path, device: str):
+    """
+    Prints the logs of a device.
+    """
+    asyncio.run(
+        c_logs(config_dir, device)
+    )
+
+
+@cli.command(name="shell")
+@click.option(*get_option_names(PARAM_CFG_DIR),
+              required=False,
+              default=DEFAULT_CONFIG_PATH,
+              type=click.Path(exists=True, path_type=Path),
+              help=get_option_help(PARAM_CFG_DIR))
+@click.option(*get_option_names(PARAM_DEVICE), required=True, default=None,
+              help=get_option_help(PARAM_DEVICE))
+def shell(config_dir: Path, device: str):
+    """
+    Connects to the telnet server of a device.
+    """
+    asyncio.run(
+        c_shell(config_dir, device)
+    )
+
+
+@cli.command(name="listen")
 @click.option(*get_option_names(PARAM_CFG_DIR),
               required=False,
               default=DEFAULT_CONFIG_PATH,
               type=click.Path(exists=True, path_type=Path),
               help=get_option_help(PARAM_CFG_DIR))
 @click.option(*get_option_names(PARAM_DEVICE),
+              required=False,
+              help=get_option_help(PARAM_DEVICE))
+@click.option(*get_option_names(PARAM_MQTT_PATH),
               required=True,
+              help=get_option_help(PARAM_MQTT_PATH))
+def listen(config_dir: Path, device: str, path: str):
+    """
+    Sends a state update request to a device.
+    """
+    asyncio.run(
+        c_listen(config_dir, device, path)
+    )
+
+
+@cli.command(name="cmd")
+@click.option(*get_option_names(PARAM_CFG_DIR),
+              required=False,
+              default=DEFAULT_CONFIG_PATH,
+              type=click.Path(exists=True, path_type=Path),
+              help=get_option_help(PARAM_CFG_DIR))
+@click.option(*get_option_names(PARAM_DEVICE),
+              required=False,
               help=get_option_help(PARAM_DEVICE))
 @click.option(*get_option_names(PARAM_CMD),
               required=True,
               help=get_option_help(PARAM_CMD))
 @click.option(*get_option_names(PARAM_PAYLOAD),
               required=False,
               default="",
@@ -186,15 +267,41 @@
 def cmd(config_dir: Path, device: str, command: str, payload: str):
     """
     Sends a command request to a device.
 
     The list of possible commands can be found on the official openHASP
     documentation: https://www.openhasp.com/latest/commands
     """
-    c_cmd(config_dir, device, command, payload)
+    asyncio.run(
+        c_cmd(config_dir, device, command, payload)
+    )
+
+
+@cli.command(name="state")
+@click.option(*get_option_names(PARAM_CFG_DIR),
+              required=False,
+              default=DEFAULT_CONFIG_PATH,
+              type=click.Path(exists=True, path_type=Path),
+              help=get_option_help(PARAM_CFG_DIR))
+@click.option(*get_option_names(PARAM_DEVICE),
+              required=False,
+              help=get_option_help(PARAM_DEVICE))
+@click.option(*get_option_names(PARAM_OBJECT),
+              required=True,
+              help=get_option_help(PARAM_OBJECT))
+@click.option(*get_option_names(PARAM_STATE),
+              required=True,
+              help=get_option_help(PARAM_STATE))
+def state(config_dir: Path, device: str, object: str, state: str):
+    """
+    Sends a state update request to a device.
+    """
+    asyncio.run(
+        c_state(config_dir, device, object, state)
+    )
 
 
 @cli.command(name="vars")
 @click.option(*get_option_names(PARAM_CFG_DIR),
               required=False,
               default=DEFAULT_CONFIG_PATH,
               type=click.Path(exists=True, path_type=Path),
@@ -203,15 +310,17 @@
               required=False,
               default="",
               help=get_option_help(PARAM_PATH))
 def vars(config_dir: Path, path: str):
     """
     Prints the variables accessible in a given path.
     """
-    c_vars(config_dir, path)
+    asyncio.run(
+        c_vars(config_dir, path)
+    )
 
 
 @cli.command(name="screenshot")
 @click.option(*get_option_names(PARAM_CFG_DIR),
               required=False,
               default=DEFAULT_CONFIG_PATH,
               type=click.Path(exists=True, path_type=Path),
@@ -228,8 +337,10 @@
               default=DEFAULT_SCREENSHOT_OUTPUT_PATH,
               type=click.Path(path_type=Path),
               help=get_option_help(PARAM_OUTPUT_DIR))
 def screenshot(config_dir: Path, device: str, output_dir: Path):
     """
     Requests a screenshot from the given device and stores it to the given output directory.
     """
-    c_screenshot(config_dir, device, output_dir)
+    asyncio.run(
+        c_screenshot(config_dir, device, output_dir)
+    )
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/cmd.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 
 from openhasp_config_manager.cli.common import _create_config_manager, _analyze_and_filter, _cmd
 from openhasp_config_manager.ui.util import success, error
 
 
-def c_cmd(config_dir: Path, device: str, command: str, payload: str):
+async def c_cmd(config_dir: Path, device: str, command: str, payload: str):
     try:
         config_manager = _create_config_manager(config_dir, Path("./nonexistent"))
         filtered_devices, ignored_devices = _analyze_and_filter(config_manager=config_manager, device_filter=device)
 
         if len(filtered_devices) <= 0:
             raise Exception(f"No device matches the filter: {device}")
 
         for device in filtered_devices:
-            _cmd(device, command, payload)
+            await _cmd(device, command, payload)
         success("Done!")
     except Exception as ex:
         error(str(ex))
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/common.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,65 +3,69 @@
 
 from openhasp_config_manager.manager import ConfigManager
 from openhasp_config_manager.openhasp_client.model.device import Device
 from openhasp_config_manager.processing.variables import VariableManager
 from openhasp_config_manager.ui.util import info
 
 
-def _generate(config_manager: ConfigManager, device: Device):
+async def _generate(config_manager: ConfigManager, device: Device):
     info(f"Generating output for '{device.name}'...")
     try:
         config_manager.process(device)
     except Exception as ex:
         raise Exception(f"Error generating output for {device.name}: {ex}")
 
 
-def _upload(device: Device, output_dir: Path, purge: bool, show_diff: bool):
+async def _upload(device: Device, output_dir: Path, purge: bool, show_diff: bool):
     from openhasp_config_manager.openhasp_client.openhasp import OpenHaspClient
     from openhasp_config_manager.uploader import ConfigUploader
 
     client = OpenHaspClient(device)
     uploader = ConfigUploader(output_dir, client)
     try:
         info(f"Uploading files to device '{device.name}'...")
-        uploader.upload(device, purge, show_diff)
+        return uploader.upload(device, purge, show_diff)
     except Exception as ex:
         raise Exception(f"Error uploading files to '{device.name}': {ex}")
 
 
-def _deploy(config_manager: ConfigManager, device: Device, output_dir: Path, purge: bool, show_diff: bool):
-    _generate(config_manager, device)
-    _upload(device, output_dir, purge, show_diff)
+async def _deploy(config_manager: ConfigManager, device: Device, output_dir: Path, purge: bool, show_diff: bool):
+    await _generate(config_manager, device)
+    changed = _upload(device, output_dir, purge, show_diff)
     # _cmd(config_dir, device="touch_down_1", command="reboot", payload="")
     # _reload(config_dir, device)
-    _reboot(device)
+    if changed:
+        info(f"Rebooting {device.name} to apply changes")
+        await _reboot(device)
+    else:
+        info(f"No changes detected for {device.name}, device is already up-to-date")
 
 
-def _reload(device: Device):
+async def _reload(device: Device):
     from openhasp_config_manager.openhasp_client.openhasp import OpenHaspClient
 
     client = OpenHaspClient(device)
-    client.command("clearpage", "all")
-    client.command("run", "L:/boot.cmd")
+    await client.command("clearpage", "all")
+    await client.command("run", "L:/boot.cmd")
 
 
-def _reboot(device: Device):
+async def _reboot(device: Device):
     from openhasp_config_manager.openhasp_client.openhasp import OpenHaspClient
 
     client = OpenHaspClient(device)
     info(f"Rebooting {device.name}...")
     client.reboot()
 
 
-def _cmd(device: Device, command: str, payload: str):
+async def _cmd(device: Device, command: str, payload: str):
     from openhasp_config_manager.openhasp_client.openhasp import OpenHaspClient
 
     client = OpenHaspClient(device)
     info(f"Sending command {command} to {device.name}...")
-    client.command(command, payload)
+    await client.command(command, payload)
 
 
 def _create_config_manager(config_dir, output_dir) -> ConfigManager:
     variable_manager = VariableManager(cfg_root=config_dir)
     config_manager = ConfigManager(
         cfg_root=config_dir,
         output_root=output_dir,
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/deploy.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from openhasp_config_manager.cli.common import _create_config_manager, _analyze_and_filter, _deploy
 from openhasp_config_manager.ui.util import warn, success, error
 
 
-def c_deploy(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
+async def c_deploy(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
     try:
         config_manager = _create_config_manager(config_dir, output_dir)
         filtered_devices, ignored_devices = _analyze_and_filter(config_manager=config_manager, device_filter=device)
 
         if len(filtered_devices) <= 0:
             if device is None:
                 raise Exception("No devices found.")
@@ -16,15 +16,15 @@
                 raise Exception(f"No device matches the filter: {device}")
 
         if len(ignored_devices) > 0:
             ignored_devices_names = list(map(lambda x: x.name, ignored_devices))
             warn(f"Skipping devices: {', '.join(ignored_devices_names)}")
 
         for device in filtered_devices:
-            _deploy(
+            await _deploy(
                 config_manager=config_manager,
                 device=device,
                 output_dir=output_dir,
                 purge=purge,
                 show_diff=diff
             )
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/generate.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from openhasp_config_manager.cli.common import _create_config_manager, _analyze_and_filter, _generate
 from openhasp_config_manager.ui.util import warn, success, error
 
 
-def c_generate(config_dir: Path, output_dir: Path, device: str):
+async def c_generate(config_dir: Path, output_dir: Path, device: str):
     try:
         config_manager = _create_config_manager(config_dir, output_dir)
         filtered_devices, ignored_devices = _analyze_and_filter(config_manager=config_manager, device_filter=device)
 
         if len(filtered_devices) <= 0:
             if device is None:
                 raise Exception("No devices found.")
@@ -16,12 +16,12 @@
                 raise Exception(f"No device matches the filter: {device}")
 
         if len(ignored_devices) > 0:
             ignored_devices_names = list(map(lambda x: x.name, ignored_devices))
             warn(f"Skipping devices: {', '.join(ignored_devices_names)}")
 
         for device in filtered_devices:
-            _generate(config_manager, device)
+            await _generate(config_manager, device)
 
         success("Done!")
     except Exception as ex:
         error(str(ex))
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/screenshot.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from openhasp_config_manager.cli.common import _create_config_manager, _analyze_and_filter
 from openhasp_config_manager.ui.util import error, success, info
 
 
-def c_screenshot(config_dir: Path, device: str, output: Path):
+async def c_screenshot(config_dir: Path, device: str, output: Path):
     try:
         config_manager = _create_config_manager(config_dir, Path("./nonexistent"))
         filtered_devices, ignored_devices = _analyze_and_filter(config_manager=config_manager, device_filter=device)
 
         if len(filtered_devices) <= 0:
             raise Exception(f"No device matches the filter: {device}")
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/upload.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from openhasp_config_manager.cli.common import _create_config_manager, _analyze_and_filter, _upload
 from openhasp_config_manager.ui.util import warn, success, error
 
 
-def c_upload(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
+async def c_upload(config_dir: Path, output_dir: Path, device: str, purge: bool, diff: bool):
     try:
         config_manager = _create_config_manager(config_dir, output_dir)
         filtered_devices, ignored_devices = _analyze_and_filter(config_manager=config_manager, device_filter=device)
 
         if len(filtered_devices) <= 0:
             if device is None:
                 raise Exception("No devices found.")
@@ -16,12 +16,12 @@
                 raise Exception(f"No device matches the filter: {device}")
 
         if len(ignored_devices) > 0:
             ignored_devices_names = list(map(lambda x: x.name, ignored_devices))
             warn(f"Skipping devices: {', '.join(ignored_devices_names)}")
 
         for device in filtered_devices:
-            _upload(device, output_dir, purge, diff)
+            await _upload(device, output_dir, purge, diff)
 
         success("Done!")
     except Exception as ex:
         error(str(ex))
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/cli/vars.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/cli/vars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Dict, List
 
 from openhasp_config_manager.processing.variables import VariableManager
 from openhasp_config_manager.ui.util import error, echo
 
 
-def _format_variables(variables: Dict) -> str:
+async def _format_variables(variables: Dict) -> str:
     def get_dict_contents(d: Dict, parent_key: str = '', result: List[str] = []):
         for k in sorted(d.keys()):
             v = d[k]
             if isinstance(v, dict):
                 get_dict_contents(v, parent_key + k + '.', result)
             elif isinstance(v, list):
                 for i in range(len(v)):
@@ -20,15 +20,15 @@
             else:
                 result.append(f"{parent_key}{k}: {v}")
         return result
 
     return "\n".join(get_dict_contents(variables))
 
 
-def c_vars(config_dir: Path, path: str):
+async def c_vars(config_dir: Path, path: str):
     try:
         variable_manager = VariableManager(cfg_root=config_dir)
         variables = variable_manager.get_vars(Path(config_dir, path))
-        formatted = _format_variables(variables)
+        formatted = await _format_variables(variables)
         echo(formatted)
     except Exception as ex:
         error(str(ex))
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/manager.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 from typing import List, Set
 
 import orjson
 
 from openhasp_config_manager.const import COMMON_FOLDER_NAME, DEVICES_FOLDER_NAME, SYSTEM_SCRIPTS
 from openhasp_config_manager.openhasp_client.model.component import Component
 from openhasp_config_manager.openhasp_client.model.config import Config
+from openhasp_config_manager.openhasp_client.model.debug_config import DebugConfig
 from openhasp_config_manager.openhasp_client.model.device import Device
 from openhasp_config_manager.openhasp_client.model.device_config import DeviceConfig
 from openhasp_config_manager.openhasp_client.model.gui_config import GuiConfig
 from openhasp_config_manager.openhasp_client.model.hasp_config import HaspConfig
 from openhasp_config_manager.openhasp_client.model.http_config import HttpConfig
 from openhasp_config_manager.openhasp_client.model.mqtt_config import MqttConfig
 from openhasp_config_manager.openhasp_client.model.openhasp_config_manager_config import OpenhaspConfigManagerConfig
 from openhasp_config_manager.openhasp_client.model.screen_config import ScreenConfig
+from openhasp_config_manager.openhasp_client.model.telnet_config import TelnetConfig
+from openhasp_config_manager.openhasp_client.model.wifi_config import WifiConfig
 from openhasp_config_manager.processing.device_processor import DeviceProcessor
 from openhasp_config_manager.processing.jsonl.jsonl import ObjectDimensionsProcessor
 from openhasp_config_manager.processing.variables import VariableManager
 from openhasp_config_manager.ui.util import warn
 from openhasp_config_manager.validation.cmd import CmdFileValidator
 from openhasp_config_manager.validation.device_validator import DeviceValidator
 from openhasp_config_manager.validation.jsonl import JsonlObjectValidator
@@ -159,18 +162,21 @@
             is_screen_rotated = gui_config.rotate % 2 == 1
 
             config = Config(
                 openhasp_config_manager=self._parse_openhasp_config_manager_config(
                     data=loaded["openhasp_config_manager"],
                     swap_width_and_height=is_screen_rotated
                 ),
+                wifi=self._parse_wifi_config(loaded["wifi"]),
                 mqtt=self._parse_mqtt_config(loaded["mqtt"]),
                 http=self._parse_http_config(loaded["http"]),
                 gui=self._parse_gui_config(loaded["gui"]),
-                hasp=self._parse_hasp_config(loaded["hasp"])
+                hasp=self._parse_hasp_config(loaded["hasp"]),
+                debug=self._parse_debug_config(loaded["debug"]),
+                telnet=self._parse_telnet_config(loaded["telnet"])
             )
 
             return config
 
     @staticmethod
     def _parse_openhasp_config_manager_config(data: dict, swap_width_and_height: bool) -> OpenhaspConfigManagerConfig:
         screen_width_key = "width"
@@ -189,14 +195,21 @@
                     width=data["device"]["screen"][screen_width_key],
                     height=data["device"]["screen"][screen_height_key]
                 )
             )
         )
 
     @staticmethod
+    def _parse_wifi_config(data: dict) -> WifiConfig:
+        return WifiConfig(
+            ssid=data["ssid"],
+            password=data["pass"],
+        )
+
+    @staticmethod
     def _parse_mqtt_config(data: dict) -> MqttConfig:
         return MqttConfig(
             name=data["name"],
             group=data["group"],
             host=data["host"],
             port=data["port"],
             user=data["user"],
@@ -232,14 +245,33 @@
             theme=data["theme"],
             color1=data["color1"],
             color2=data["color2"],
             font=data["font"],
             pages=data["pages"],
         )
 
+    @staticmethod
+    def _parse_debug_config(data: dict) -> DebugConfig:
+        return DebugConfig(
+            ansi=data["ansi"],
+            baud=data["baud"],
+            tele=data["tele"],
+            host=data["host"],
+            port=data["port"],
+            proto=data["proto"],
+            log=data["log"],
+        )
+
+    @staticmethod
+    def _parse_telnet_config(data: dict) -> TelnetConfig:
+        return TelnetConfig(
+            enable=data["enable"],
+            port=data["port"],
+        )
+
     def process(self, device: Device):
         """
         Process the configuration and generate the corresponding output
         """
         self._generate_output(device)
 
     def _generate_output(self, device: Device):
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/model/config.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/model/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from dataclasses import dataclass
 
+from openhasp_config_manager.openhasp_client.model.debug_config import DebugConfig
 from openhasp_config_manager.openhasp_client.model.gui_config import GuiConfig
 from openhasp_config_manager.openhasp_client.model.hasp_config import HaspConfig
 from openhasp_config_manager.openhasp_client.model.http_config import HttpConfig
 from openhasp_config_manager.openhasp_client.model.mqtt_config import MqttConfig
 from openhasp_config_manager.openhasp_client.model.openhasp_config_manager_config import OpenhaspConfigManagerConfig
+from openhasp_config_manager.openhasp_client.model.telnet_config import TelnetConfig
+from openhasp_config_manager.openhasp_client.model.wifi_config import WifiConfig
 
 
 @dataclass
 class Config:
     openhasp_config_manager: OpenhaspConfigManagerConfig
+    wifi: WifiConfig
     mqtt: MqttConfig
     http: HttpConfig
     gui: GuiConfig
     hasp: HaspConfig
+    debug: DebugConfig
+    telnet: TelnetConfig
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/mqtt_client.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/mqtt_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-import paho.mqtt.client as paho
+import asyncio
+from typing import Callable
 
-from openhasp_config_manager.openhasp_client.model.device import Device
+from asyncio_mqtt import Client, MqttError
 
 
 class MqttClient:
 
     def __init__(self, host: str, port: int, mqtt_user: str, mqtt_password: str):
         self._mqtt_client_id = 'openhasp-config-manager'
         self._host = host
         self._port = port
         self._mqtt_user = mqtt_user
         self._mqtt_password = mqtt_password
+        self._reconnect_interval_seconds = 5
 
-    def publish(self, topic: str, payload: str):
+    async def publish(self, topic: str, payload: str):
+        async with self._create_mqtt_client() as client:
+            await client.publish(topic, payload=payload)
+
+    async def subscribe(self, topic: str, callback: Callable):
         try:
-            self._connect()
-            result = self._client.publish(topic=topic, payload=payload)
-            result.wait_for_publish()
-
-            if not result.rc == paho.MQTT_ERR_SUCCESS:
-                raise Exception(f'Code {result.rc} while sending message {result.mid}: {paho.error_string(result.rc)})')
-        finally:
-            self._client.disconnect()
-
-    def watch(self, device: Device):
-        pass
-
-    def _connect(self):
-        self._client = paho.Client(client_id=self._mqtt_client_id, protocol=paho.MQTTv5)
-        self._client.username_pw_set(username=self._mqtt_user, password=self._mqtt_password)
-        self._client.connect(self._host, self._port)
+            async with self._create_mqtt_client() as client:
+                async with client.messages() as messages:
+                    await client.subscribe(topic)
+                    async for message in messages:
+                        await callback(message.topic, message.payload)
+        except MqttError:
+            print(f'Connection lost; Reconnecting in {self._reconnect_interval_seconds} seconds ...')
+            await asyncio.sleep(self._reconnect_interval_seconds)
+
+    def _create_mqtt_client(self) -> Client:
+        return Client(
+            hostname=self._host,
+            port=self._port,
+            username=self._mqtt_user,
+            password=self._mqtt_password,
+            client_id=self._mqtt_client_id
+        )
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/openhasp_client/openhasp.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/openhasp_client/openhasp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,312 +1,263 @@
-from typing import Dict, List
-
-import orjson
-import requests as requests
+import json
+from typing import Dict, List, Any, Callable
 
 from openhasp_config_manager.openhasp_client.model.device import Device
 from openhasp_config_manager.openhasp_client.model.gui_config import GuiConfig
 from openhasp_config_manager.openhasp_client.model.hasp_config import HaspConfig
 from openhasp_config_manager.openhasp_client.model.http_config import HttpConfig
 from openhasp_config_manager.openhasp_client.model.mqtt_config import MqttConfig
 from openhasp_config_manager.openhasp_client.mqtt_client import MqttClient
+from openhasp_config_manager.openhasp_client.telnet_client import OpenHaspTelnetClient
+from openhasp_config_manager.openhasp_client.webservice_client import WebserviceClient
 from openhasp_config_manager.ui.util import info
 
-GET = "GET"
-POST = "POST"
-DELETE = "DELETE"
-
 
 class OpenHaspClient:
 
     def __init__(self, device: Device):
         """
         :param device: the device this client can communicate with
         """
         self._device = device
-        self._base_url = self._compute_base_url(self._device)
+
+        self._webservice_client = WebserviceClient(
+            url=device.config.openhasp_config_manager.device.ip,
+            username=self._device.config.http.user,
+            password=self._device.config.http.password
+        )
 
         self._mqtt_client = MqttClient(
             host=device.config.mqtt.host,
             port=device.config.mqtt.port,
             mqtt_user=device.config.mqtt.user,
             mqtt_password=device.config.mqtt.password
         )
 
-    def get_files(self) -> List[str]:
+        self._telnet_client = OpenHaspTelnetClient(
+            host=device.config.openhasp_config_manager.device.ip,
+            port=device.config.telnet.port,
+            baudrate=device.config.debug.baud,
+            user=device.config.http.user,
+            password=device.config.http.password,
+        )
+
+    async def send_image(self, image: any, page: int, object_id: int):
         """
-        Retrieve a list of all file on the device
-        :return: a list of all files on the device
+        Send an image to the device
+        :param image: the image to send
+        :param page: the page to send the image to
+        :param object_id: the object id to send the image to
         """
-        username = self._device.config.http.user
-        password = self._device.config.http.password
+        pass
 
-        response = self._do_request(
-            method=GET,
-            url=self._base_url + "list?dir=/",
-            username=username, password=password
+    async def set_text(self, obj: str, text: str):
+        """
+        Set the text of an object
+        :param obj: the object to set the text for
+        :param text: the text to set
+        """
+        await self.set_object_properties(obj, {"text": text})
+
+    async def set_object_properties(self, obj: str, properties: Dict[str, Any]):
+        """
+        Set the state of a plate
+        :param obj: object to set a state for
+        :param properties: properties to set
+        """
+        for prop, value in properties.items():
+            await self.command(
+                name=f"{obj}.{prop}",
+                params=value,
+            )
+
+    async def set_idle_state(self, state: str):
+        """
+        Forces the given idle state
+        :param state: one of "off", "short", "long"
+        """
+        return await self.command(
+            name="idle",
+            params=state
         )
-        response_data = orjson.loads(response.decode('utf-8'))
 
-        files = list(filter(lambda x: x["type"] == "file", response_data))
-        file_names = list(map(lambda x: x["name"], files))
-        return file_names
+    async def set_backlight(self, state: bool, brightness: int):
+        """
+        Sets the backlight state and brightness
+        :param state: True to turn on, False to turn off
+        :param brightness: the brightness level in 0..255
+        """
+        return await self.command(
+            name="backlight",
+            params=json.dumps({
+                "state": state,
+                "brightness": brightness,
+            })
+        )
 
-    def get_file_content(self, file_name: str) -> str or None:
-        username = self._device.config.http.user
-        password = self._device.config.http.password
+    async def wakeup(self):
+        """
+        Wakes up the display
+        """
+        return await self.set_idle_state(state="off")
 
-        try:
-            response = self._do_request(
-                method=GET,
-                url=self._base_url + file_name,
-                username=username, password=password
-            )
-            response_data = response.decode('utf-8')
-            return response_data
-        except Exception as ex:
-            return None
+    async def set_page(self, index: int):
+        """
+        Set the current page
+        :param index: the index of the page to set
+        """
+        return await self.command(
+            name="page",
+            params=f"{index}"
+        )
 
-    def delete_file(self, file_name: str):
+    async def set_hidden(self, obj: str, hidden: bool):
         """
-        Delete a file on the device
-        :param file_name: the name of the file
+        Set the "hidden" property of an object
+        :param obj: the object to set the property for
+        :param hidden: True to hide the object, False to show it
+        """
+        return await self.set_object_properties(
+            obj=obj,
+            properties={
+                "hidden": "1" if hidden else "0",
+            }
+        )
+
+    async def listen_state(
+            self,
+            callback: Callable,
+            state: str,
+    ):
+        """
+        Listen to OpenHASP state events
+        :param callback: callback to call when a matching event is received
+        :param state: state to listen for
+        :return: A handle that can be used to cancel the callback.
         """
-        username = self._device.config.http.user
-        password = self._device.config.http.password
+        plate = self._device.config.mqtt.name
 
-        self._do_request(
-            method=DELETE,
-            url=self._base_url + "edit",
-            data={
-                "path": "/" + file_name
-            },
-            username=username, password=password
+        async def _callback(event_topic: str, event_payload: bytes):
+            event_topic_segments = event_topic.split('/')
+
+            if len(event_topic_segments) != 4 or event_topic_segments[2] != "state":
+                return
+
+            event_plate = event_topic_segments[1]
+            event_state_name = event_topic_segments[3]
+
+            if (event_plate == plate) and event_state_name == state:
+                await callback(event_topic, event_plate, event_state_name, event_payload)
+
+        await self.listen_event(
+            path=f"hasp/{plate}/state/{state}",
+            callback=_callback,
         )
 
-    def watch(self):
-        self._mqtt_client.watch(self._device)
+    async def listen_event(self, path: str, callback: Callable):
+        """
+        Listen for an event
+        :param path:
+        :param callback:
+        :return:
+        """
+
+        async def _on_message(topic: str, payload: bytes):
+            await callback(topic, payload)
+
+        topic = f"hasp/{self._device.config.mqtt.name}/{path}"
+        await self._mqtt_client.subscribe(topic, _on_message)
 
-    def command(self, name: str, params: str):
+    async def command(self, name: str, params: str):
         """
         Execute a command on a device
         :param name: the name of the command
         :param params: parameters for the command
         """
         topic = f"hasp/{self._device.config.mqtt.name}/command/{name}"
-
         data = params.strip('"')
-        self._mqtt_client.publish(topic=topic, payload=data)
+        await self._mqtt_client.publish(topic=topic, payload=data)
+
+    def get_files(self) -> List[str]:
+        """
+        Retrieve a list of all file on the device
+        :return: a list of all files on the device
+        """
+        return self._webservice_client.get_files()
+
+    def get_file_content(self, file_name: str) -> str or None:
+        return self._webservice_client.get_file_content(file_name)
+
+    def delete_file(self, file_name: str):
+        """
+        Delete a file on the device
+        :param file_name: the name of the file
+        """
+        self._webservice_client.delete_file(file_name)
 
     def reboot(self):
         """
         Request a reboot
         """
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-        self._do_request(
-            method=GET,
-            url=self._base_url + "reboot",
-            username=username, password=password
-        )
+        self._webservice_client.reboot()
 
     def set_hasp_config(self, config: HaspConfig):
         """
         Set the "HASP" configuration
         :param config: the configuration to set
         """
-        data = {
-            "startpage": config.startpage,
-            "startdim": config.startdim,
-            "theme": config.theme,
-            "color1": config.color1,
-            "color2": config.color2,
-            "font": config.font,
-            "pages": config.pages,
-            "save": "hasp"
-        }
-
-        # ignore keys with None value
-        data = {k: v for k, v in data.items() if v is not None}
-
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-
-        self._do_request(
-            method=POST,
-            url=self._base_url + "config",
-            data=data,
-            username=username, password=password
-        )
+        self._webservice_client.set_hasp_config(config)
 
     def set_http_config(self, config: HttpConfig):
         """
         Set the HTTP configuration
         :param config: the configuration to set
         """
-        data = {
-            "user": config.user,
-            "pass": config.password,
-            "save": "http"
-        }
-
-        # ignore keys with None value
-        data = {k: v for k, v in data.items() if v is not None}
-
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-
-        self._do_request(
-            method=POST,
-            url=self._base_url + "config",
-            data=data,
-            username=username, password=password
-        )
+        self._webservice_client.set_http_config(config)
+
+    def get_mqtt_config(self) -> MqttConfig:
+        return self._webservice_client.get_mqtt_config()
 
     def set_mqtt_config(self, config: MqttConfig):
         """
         Set the MQTT configuration
         :param config: the configuration to set
         :return:
         """
-        data = {
-            "name": config.name,
-            "group": config.group,
-            "host": config.host,
-            "port": config.port,
-            "user": config.user,
-            "pass": config.password,
-            "save": "mqtt"
-        }
-
-        # ignore keys with None value
-        data = {k: v for k, v in data.items() if v is not None}
-
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-
-        self._do_request(
-            method=POST,
-            url=self._base_url + "config",
-            data=data,
-            username=username, password=password
-        )
+        self._webservice_client.set_mqtt_config(config)
 
     def set_gui_config(self, config: GuiConfig):
         """
         Set the GUI configuration
         :param config: the configuration to set
         :return:
         """
-        data = {
-            "idle1": config.idle1,
-            "idle2": config.idle2,
-            "rotate": config.rotate,
-            "cursor": config.cursor,
-            "bckl": config.bckl,
-            "save": "gui"
-        }
-
-        # ignore keys with None value
-        data = {k: v for k, v in data.items() if v is not None}
-
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-
-        self._do_request(
-            method=POST,
-            url=self._base_url + "config",
-            data=data,
-            username=username, password=password
-        )
+        self._webservice_client.set_gui_config(config)
 
     def upload_files(self, files: Dict[str, str]):
         """
         Upload a collection of files
         :param files: "target file name"->"file content" mapping
         """
-        for name, content in files.items():
-            self.upload_file(name, content)
+        self._webservice_client.upload_files(files)
 
     def upload_file(self, name: str, content: str):
         """
         Upload a single file
         :param name: the target name of the file on the device
         :param content: the file content
         """
         info(f"Uploading '{name}'...")
-
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-        self._do_request(
-            method=POST,
-            url=self._base_url + "edit",
-            files={
-                f"{name}": content
-            },
-            username=username, password=password
-        )
+        self._webservice_client.upload_file(name, content)
 
     def take_screenshot(self) -> bytes:
         """
         Requests a screenshot from the device.
         :return:
         """
-        username = self._device.config.http.user
-        password = self._device.config.http.password
-
-        return self._do_request(
-            method=GET,
-            url=self._base_url + "screenshot",
-            params={
-                "q": "0"
-            },
-            stream=True,
-            username=username, password=password
-        )
+        return self._webservice_client.take_screenshot()
 
-    @staticmethod
-    def _do_request(method: str = GET, url: str = "/", params: dict = None,
-                    json: any = None, files: any = None, data: any = None,
-                    headers: dict = None,
-                    username: str = None, password: str = None,
-                    stream: bool = None) -> list or dict or None:
-        """
-        Executes a http request based on the given parameters
-
-        :param method: the method to use (GET, POST)
-        :param url: the url to use
-        :param params: query parameters that will be appended to the url
-        :param json: request body
-        :param headers: custom headers
-        :return: the response parsed as a json
-        """
-        _headers = {
-        }
-        if headers is not None:
-            _headers.update(headers)
-
-        response = requests.request(
-            method, url, headers=_headers,
-            params=params,
-            json=json, files=files,
-            data=data,
-            auth=(username, password),
-            timeout=5,
-            stream=stream,
-        )
+    async def shell(self):
+        await self._telnet_client.shell()
 
-        response.raise_for_status()
-        if len(response.content) > 0:
-            if "application/json" in response.headers.get("Content-Type", ""):
-                return response.json()
-            else:
-                return response.content
-
-    @staticmethod
-    def _compute_base_url(device: Device) -> str:
-        url = device.config.openhasp_config_manager.device.ip
-        if not url.startswith("http://"):
-            url = "http://" + url
-        if not url.endswith("/"):
-            url += "/"
-        return url
+    async def logs(self):
+        await self._telnet_client.logs()
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/processing/device_processor.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/device_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/processing/jsonl/jsonl.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/processing/template_rendering.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/template_rendering.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/processing/variables.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/processing/variables.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/ui/util.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/ui/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/uploader.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/uploader.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,23 +10,36 @@
 class ConfigUploader:
 
     def __init__(self, output_root: Path, openhasp_client: OpenHaspClient):
         self._api_client = openhasp_client
         self._output_root = output_root
         self._cache_dir = Path(self._output_root, ".cache")
 
-    def upload(self, device: Device, purge: bool = False, print_diff: bool = False):
+    def upload(self, device: Device, purge: bool = False, print_diff: bool = False) -> bool:
+        """
+        Uploads configuration files and config properties to a device.
+        :param device: The device to upload to.
+        :param purge: If True, removes files from the device, which are not present in the generated output.
+        :param print_diff: If true, a diff will be printed to the console for each file that has changed.
+        :return: True if any files have changed, false otherwise.
+        """
+        result = False
+
         if purge:
-            self.cleanup_device(device)
-        self._upload_files(device, print_diff)
-        self._update_config(device)
+            result |= self.cleanup_device(device)
 
-    def _upload_files(self, device: Device, print_diff: bool):
+        result |= self._upload_files(device, print_diff)
+        result |= self._update_config(device)
+        return result
+
+    def _upload_files(self, device: Device, print_diff: bool) -> bool:
         existing_files = self._api_client.get_files()
 
+        result = False
+
         for file in device.output_dir.iterdir():
             info(f"Preparing '{file.name}' for upload...")
 
             content = file.read_text()
 
             if len(content) <= 0:
                 warn(f"File is empty, skipping upload: {file}")
@@ -43,14 +56,15 @@
             new_checksum = self._check_if_checksum_will_change(
                 file=file,
                 original_checksum=device_file_content_checksum,
                 new_content=content
             )
 
             if new_checksum is not None:
+                result = True
                 if print_diff:
                     diff_output = self._calculate_diff(
                         file_name=file.name,
                         string1=file_content_on_device,
                         string2=content
                     )
                     print_diff_to_console(diff_output)
@@ -60,29 +74,36 @@
                     checksum_file.parent.mkdir(parents=True, exist_ok=True)
                     checksum_file.write_text(new_checksum)
                 except Exception as ex:
                     raise Exception(f"Error uploading file '{file.name}' to '{device.name}': {ex}")
             else:
                 info(f"Skipping {file} because it hasn't changed.")
 
-    def cleanup_device(self, device: Device):
+        return result
+
+    def cleanup_device(self, device: Device) -> bool:
         """
         Delete files from the device, which are not present in the currently generated output
         :param device: the target device
+        :return: True if any files have been deleted, false otherwise
         """
+        result = False
+
         file_names = ["config.json"]
         for file in device.output_dir.iterdir():
             file_names.append(file.name)
 
         # cleanup files which are on the device, but not present in the generated output
         files_on_device = self._api_client.get_files()
         for f in files_on_device:
             if f not in file_names:
+                result = True
                 info(f"Deleting file '{f}' from device '{device.name}'")
                 self._api_client.delete_file(f)
+        return result
 
     def _check_if_checksum_will_change(self, file: Path, original_checksum: str, new_content: str) -> str | None:
         """
         Checks if the checksum for the given file has changed since it was last uploaded.
         :param file: the path of the file to check
         :param original_checksum: expected checksum of the original content
         :param new_content: the content of the new file
@@ -108,18 +129,24 @@
         return Path(
             self._cache_dir,
             *file.relative_to(self._output_root).parts[:-1],
             file.name + ".md5"
         )
 
     def _update_config(self, device: Device):
+        current_mqtt_config = self._api_client.get_mqtt_config()
+        # TODO: compare existing config with new config and only update if necessary
+
         self._api_client.set_mqtt_config(device.config.mqtt)
         self._api_client.set_http_config(device.config.http)
         self._api_client.set_gui_config(device.config.gui)
 
+        # TODO: return True if config has changed
+        return False
+
     @staticmethod
     def _calculate_diff(file_name: str, string1: str, string2: str) -> str:
         diff = difflib.unified_diff(
             string1.splitlines(),
             string2.splitlines(),
             lineterm="\n",
             fromfile=f"${file_name}",
```

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/util.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/validation/__init__.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/validation/cmd.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/validation/device_validator.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/device_validator.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/openhasp_config_manager/validation/jsonl.py` & `openhasp_config_manager-0.4.0/openhasp_config_manager/validation/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.3.1/pyproject.toml` & `openhasp_config_manager-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openhasp-config-manager"
-version = "0.3.1"
+version = "0.4.0"
 description = "A tool to manage all of your openHASP device configs in a centralized place."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
@@ -29,19 +29,20 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.10"  # Compatible python versions must be declared here
 
 click = "*"
 requests = "*"
-paho-mqtt = "*"
 Jinja2 = "*"
 py-range-parse = "*"
 pyyaml = "*"
 orjson = "*"
+asyncio-mqtt = "*"
+telnetlib3 = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
```

### Comparing `openhasp_config_manager-0.3.1/PKG-INFO` & `openhasp_config_manager-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhasp-config-manager
-Version: 0.3.1
+Version: 0.4.0
 Summary: A tool to manage all of your openHASP device configs in a centralized place.
 Home-page: https://github.com/markusressel/openhasp-config-manager
 License: AGPL-3.0-or-later
 Keywords: openhasp,config,management
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
@@ -13,20 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2
+Requires-Dist: asyncio-mqtt
 Requires-Dist: click
 Requires-Dist: orjson
-Requires-Dist: paho-mqtt
 Requires-Dist: py-range-parse
 Requires-Dist: pyyaml
 Requires-Dist: requests
+Requires-Dist: telnetlib3
 Project-URL: Repository, https://github.com/markusressel/openhasp-config-manager
 Description-Content-Type: text/markdown
 
 # openhasp-config-manager
 
 A cli tool to manage all of your [openHASP](https://github.com/HASwitchPlate/openHASP) device configs in a centralized
 place.
@@ -42,15 +43,39 @@
     * [x] local and globally scoped variables
 * [x] validation of common mistakes for
     * [x] jsonl objects
     * [x] cmd files
 * [x] simple configuration upload to the device(s)
     * [x] automatic diffing to only update changed configuration files
     * [x] git-style diff output for changed lines
-* [x] device command execution directly from the CLI (still needs a connection to the MQTT broker)
+* [x] API client (Web + MQTT)
+    * [x] execute commands on a plate
+    * [x] listen to events and state updates
+
+```shell
+> openhasp-config-manager -h
+Usage: openhasp-config-manager [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version   Show the version and exit.
+  -h, --help  Show this message and exit.
+
+Commands:
+  cmd         Sends a command request to a device.
+  deploy      Combines the generation and upload of a configuration.
+  generate    Generates the output files for all devices in the given...
+  help        Show this message and exit.
+  listen      Sends a state update request to a device.
+  logs        Prints the logs of a device.
+  screenshot  Requests a screenshot from the given device and stores it...
+  shell       Connects to the telnet server of a device.
+  state       Sends a state update request to a device.
+  upload      Uploads the previously generated configuration to their...
+  vars        Prints the variables accessible in a given path.
+```
 
 # Disclaimer
 
 **TL;DR: This project is still experimental.**
 
 I do use openhasp-config-manager exclusively to configure all of my openHASP devices. I am in the
 process of adding tests to everything to make it more reliable and have also added lots of features along the way.
@@ -369,30 +394,20 @@
 ...
 header.title: Home
 ```
 
 ## Deployment
 
 To deploy your configurations to the already connected openHASP devices, simply use the
-command line tool `openhasp-config-manager`:
-
-```shell
-> openhasp-config-manager                                                         0 (0.604s) < 02:11:38
-Usage: openhasp-config-manager [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --version   Show the version and exit.
-  -h, --help  Show this message and exit.
+`generate`, `upload` or `deploy` commands of `openhasp-config-manager`.
 
-Commands:
-  cmd       Sends a command request to a device.
-  deploy    Combines the generation and upload of a configuration.
-  generate  Generates the output files for all devices in the given...
-  upload    Uploads the previously generated configuration to their...
-```
+> **Note**
+> openhasp-config-manager needs direct IP access as well as an enabled webservice on the plate
+> to be able to deploy files to the device. To enable the webservice
+> try: `openhasp-config-manager cmd -d plate35 -C service -p "start http"`
 
 ## Run commands
 
 While openhasp-config-manager is first and foremost a config management system,
 it also allows you to run commands on a device by issuing MQTT messages without the need to install a separate
 MQTT client first. Note that the MQTT _server_ still needs to be running and also has to
 be reachable from your local machine for this to work.
@@ -404,15 +419,21 @@
 > openhasp-config-manager cmd -c ./openhasp-configs -d plate35 -C backlight -p "{\"state\":\"on\",\"brightness\":128}"
 ```
 
 # FAQ
 
 ## How do I see device logs?
 
-With the device connected via USB cable, open a terminal and run:
+Try the `logs` command (this does require network access to the device):
+
+```shell
+> openhasp-config-manager logs -d plate35
+```
+
+If that doesn't work, open a terminal and run the following command with the device connected via USB cable:
 
 ```shell
 bash -c "screen -q -L -Logfile device.log /dev/ttyUSB0 115200 &> /dev/null; tail -F device.log; killall screen"
 ```
 
 ## Output file name length must not exceed 30 characters
```

