# Comparing `tmp/wg_utilities-3.0.1.tar.gz` & `tmp/wg_utilities-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.0.1.tar", max compression
+gzip compressed data, was "wg_utilities-3.1.0.tar", max compression
```

## Comparing `wg_utilities-3.0.1.tar` & `wg_utilities-3.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-08 12:17:58.653261 wg_utilities-3.0.1/LICENSE
--rw-r--r--   0        0        0     1024 2023-04-08 12:17:58.653261 wg_utilities-3.0.1/README.md
--rw-r--r--   0        0        0     4830 2023-04-08 12:17:58.657261 wg_utilities-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      560 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4962 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10359 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24659 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56685 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7142 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    14065 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    16193 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    24945 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49741 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21403 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6589 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     5993 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    35904 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8851 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-08 12:17:58.725262 wg_utilities-3.0.1/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 wg_utilities-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-08 17:47:26.186761 wg_utilities-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1520 2023-04-08 17:47:26.186761 wg_utilities-3.1.0/README.md
+-rw-r--r--   0        0        0     4830 2023-04-08 17:47:26.190761 wg_utilities-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-08 17:47:26.254762 wg_utilities-3.1.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      560 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4962 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10359 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24659 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56685 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7142 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    14065 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    16193 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    24945 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49741 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    21403 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6589 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     5993 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36226 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8851 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.1.0/PKG-INFO
```

### Comparing `wg_utilities-3.0.1/LICENSE` & `wg_utilities-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/pyproject.toml` & `wg_utilities-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.0.1"
+version = "3.1.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.0.1/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.1.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/__init__.py` & `wg_utilities-3.1.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/_google.py` & `wg_utilities-3.1.0/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.1.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.1.0/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/google_drive.py` & `wg_utilities-3.1.0/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/google_fit.py` & `wg_utilities-3.1.0/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/google_photos.py` & `wg_utilities-3.1.0/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/monzo.py` & `wg_utilities-3.1.0/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.1.0/wg_utilities/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/spotify.py` & `wg_utilities-3.1.0/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/clients/truelayer.py` & `wg_utilities-3.1.0/wg_utilities/clients/truelayer.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.1.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.1.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.1.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.1.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,14 +556,16 @@
             to None.
         logging (bool, optional): whether to log events. Defaults to False.
         listen_ip (str, optional): the IP address to listen on. Defaults to
             None.
         listen_port (int, optional): the port to listen on. Defaults to None.
         source_port (int, optional): the port to use for the source. Defaults
             to None.
+        resubscribe_seconds (int, optional): the number of seconds between each
+            resubscription. Defaults to 2 minutes.
     """
 
     SUBSCRIPTION_SERVICES = (
         Yas209Service.AVT.service_id,
         Yas209Service.RC.service_id,
     )
 
@@ -590,14 +592,15 @@
         on_volume_update: Callable[[float], None] | None = None,
         on_track_update: Callable[[CurrentTrack.Info], None] | None = None,
         on_state_update: Callable[[str], None] | None = None,
         logging: bool = True,
         listen_ip: str | None = None,
         listen_port: int | None = None,
         source_port: int | None = None,
+        resubscribe_seconds: int = 120,
     ):
         self.ip = ip
         self.on_event = on_event
 
         # noinspection HttpUrlsUsage
         self.description_url = f"http://{ip}:49152/description.xml"
 
@@ -614,14 +617,16 @@
         self.device: UpnpDevice
 
         self._logging = logging
         self._listen_ip = listen_ip
         self._listen_port = listen_port
         self._source_port = source_port or 0
 
+        self.resubscribe_seconds = resubscribe_seconds
+
         self._active_service_ids: list[str] = []
 
         if self._listen_ip is not None and self._listen_port is None:
             raise ValueError(
                 "Argument `listen_port` cannot be None when `listen_ip` is not None:"
                 f" {self._listen_ip!r}"
             )
@@ -775,15 +780,15 @@
                     )
                 failed_subscriptions.append(service)
 
         self._listening = True
 
         # keep the webservice running (force resubscribe)
         while self._listening:
-            for _ in range(120):
+            for _ in range(self.resubscribe_seconds):
                 if not self._listening:
                     if self._logging:
                         LOGGER.debug("Exiting listener loop")
                     break
                 await async_sleep(1)
 
             # The break above only covers the for loop, this is for the while loop
@@ -971,15 +976,18 @@
     def stop(self) -> None:
         """Stop whatever is currently playing."""
         self._call_service_action(Yas209Service.AVT, "Stop", InstanceID=0, Speed="1")
 
     def stop_listening(self) -> None:
         """Stop the event listener."""
         if self._logging:
-            LOGGER.debug("Stopping event listener (will take <= 2 minutes)")
+            LOGGER.debug(
+                "Stopping event listener (will take <= %i seconds)",
+                self.resubscribe_seconds,
+            )
 
         self._listening = False
 
     def unmute(self) -> None:
         """Unmute."""
         self._call_service_action(
             Yas209Service.RC,
```

### Comparing `wg_utilities-3.0.1/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.1.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/__init__.py` & `wg_utilities-3.1.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/_functions.py` & `wg_utilities-3.1.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.1.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/file_management.py` & `wg_utilities-3.1.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/json.py` & `wg_utilities-3.1.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/processes.py` & `wg_utilities-3.1.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.1.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/functions/xml.py` & `wg_utilities-3.1.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/loggers/__init__.py` & `wg_utilities-3.1.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.1.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.0.1/PKG-INFO` & `wg_utilities-3.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.0.1
+Version: 3.1.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
@@ -41,18 +41,22 @@
 
 # WG Utilities
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/worgarside/wg-utilities)
 [![codecov](https://codecov.io/gh/worgarside/wg-utilities/branch/develop/graph/badge.svg?token=5IJW9KBSV6)](https://codecov.io/gh/worgarside/wg-utilities)
 [![GitHub](https://img.shields.io/github/v/tag/worgarside/wg-utilities?logo=github&sort=semver)](https://github.com/worgarside/wg-utilities)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/worgarside/wg-utilities/develop.svg)](https://results.pre-commit.ci/latest/github/worgarside/wg-utilities/develop)
 [![PyPI](https://img.shields.io/pypi/v/wg-utilities.svg?logo=python)](https://pypi.python.org/pypi/wg-utilities)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![image](https://img.shields.io/pypi/pyversions/wg-utilities.svg)](https://pypi.python.org/pypi/wg-utilities)
+[![Python Unit Tests](https://github.com/worgarside/wg-utilities/actions/workflows/python_unit_tests.yml/badge.svg)](https://github.com/worgarside/wg-utilities/actions/workflows/python_unit_tests.yml)
 
 Loads of useful stuff for the things I do :)
 
 ### To-Do List
  - [ ] Finish README
  - [x] Add Coverage Badge
+ - [ ] Sphinx docs
 
 ### Unit Test Coverage
 
 [![Fancy coverage chart](https://codecov.io/gh/worgarside/wg-utilities/branch/develop/graphs/tree.svg?token=5IJW9KBSV6)](https://codecov.io/gh/worgarside/wg-utilities)
```

