# Comparing `tmp/flux_led-0.28.8.tar.gz` & `tmp/flux_led-0.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux_led-0.28.8.tar", last modified: Sat Jan 22 02:30:34 2022, max compression
+gzip compressed data, was "flux_led-0.28.9.tar", last modified: Mon Jan 24 01:29:29 2022, max compression
```

## Comparing `flux_led-0.28.8.tar` & `flux_led-0.28.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 02:30:34.387658 flux_led-0.28.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-01-22 02:30:25.000000 flux_led-0.28.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-22 02:30:34.387658 flux_led-0.28.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13139 2022-01-22 02:30:25.000000 flux_led-0.28.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 02:30:34.387658 flux_led-0.28.8/flux_led/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/aio.py
--rw-r--r--   0 runner    (1001) docker     (121)    32092 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/aiodevice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/aioprotocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     6837 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/aioscanner.py
--rw-r--r--   0 runner    (1001) docker     (121)    45513 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/base_device.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3468 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/const.py
--rw-r--r--   0 runner    (1001) docker     (121)    13046 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/device.py
--rw-r--r--   0 runner    (1001) docker     (121)    27473 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/fluxled.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    46698 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/models_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    39488 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/pattern.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    82977 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/sock.py
--rw-r--r--   0 runner    (1001) docker     (121)    11406 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11242 2022-01-22 02:30:25.000000 flux_led-0.28.8/flux_led/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 02:30:34.387658 flux_led-0.28.8/flux_led.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-22 02:30:34.000000 flux_led-0.28.8/flux_led.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-01-22 02:30:34.391658 flux_led-0.28.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-01-22 02:30:25.000000 flux_led-0.28.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 01:29:29.258152 flux_led-0.28.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-01-24 01:29:13.000000 flux_led-0.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-24 01:29:29.258152 flux_led-0.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13139 2022-01-24 01:29:13.000000 flux_led-0.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 01:29:29.258152 flux_led-0.28.9/flux_led/
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/aio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32125 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/aiodevice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/aioprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6837 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/aioscanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45551 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/base_device.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3468 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13046 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27473 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/fluxled.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    46704 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/models_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39488 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/pattern.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    82977 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/sock.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11406 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/timer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11242 2022-01-24 01:29:13.000000 flux_led-0.28.9/flux_led/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 01:29:29.258152 flux_led-0.28.9/flux_led.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-24 01:29:29.000000 flux_led-0.28.9/flux_led.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-01-24 01:29:29.258152 flux_led-0.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-01-24 01:29:13.000000 flux_led-0.28.9/setup.py
```

### Comparing `flux_led-0.28.8/LICENSE` & `flux_led-0.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/PKG-INFO` & `flux_led-0.28.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux_led
-Version: 0.28.8
+Version: 0.28.9
 Summary: A Python library to communicate with the flux_led smart bulbs
 Home-page: https://github.com/Danielhiversen/flux_led
 Author: Daniel Hjelseth Høyer
 Author-email: mail@dahoiv.net
 License: LGPLv3+
 Keywords: flux_led,smart bulbs,light
 Platform: UNKNOWN
```

### Comparing `flux_led-0.28.8/README.md` & `flux_led-0.28.9/README.md`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/aiodevice.py` & `flux_led-0.28.9/flux_led/aiodevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,15 @@
         await self._async_turn_on()
 
     async def async_turn_on(self) -> bool:
         """Turn on the device."""
         calls = (
             self._async_turn_on,
             self._async_turn_on,
+            self._async_turn_on,
             self._async_turn_off_on,
             self._async_turn_on,
             self._async_turn_on,
         )
         for idx, call in enumerate(calls):
             if (
                 await self._async_execute_and_wait_for(self._on_futures, call)
```

### Comparing `flux_led-0.28.8/flux_led/aioprotocol.py` & `flux_led-0.28.9/flux_led/aioprotocol.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/aioscanner.py` & `flux_led-0.28.9/flux_led/aioscanner.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/base_device.py` & `flux_led-0.28.9/flux_led/base_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         """Return the preset pattern number."""
         assert self.raw_state is not None
         return self.raw_state.preset_pattern
 
     @property
     def rgbwprotocol(self) -> bool:
         """Devices that don't require a separate rgb/w bit."""
-        return self.model_data.always_writes_white_and_colors
+        return self.rgbwcapable or self.model_data.always_writes_white_and_colors
 
     @property
     def microphone(self) -> bool:
         """Devices that have a microphone built in."""
         return self.model_data.microphone
 
     @property
@@ -1070,15 +1070,15 @@
 
         r_value = None if r is None else int(r)
         g_value = None if g is None else int(g)
         b_value = None if b is None else int(b)
         w_value = None if w is None else int(w)
         # ProtocolLEDENET9Byte devices support two white outputs for cold and warm.
         if w2 is None:
-            if self.color_mode in {COLOR_MODE_CCT, COLOR_MODE_RGBWW}:
+            if w is not None and self.color_mode in {COLOR_MODE_CCT, COLOR_MODE_RGBWW}:
                 # If we're only setting a single white value, we preserve the cold white value
                 w2_value: Optional[int] = self.cold_white
             else:
                 # If we're only setting a single white value, we set the second output to be the same as the first
                 w2_value = w_value
         else:
             w2_value = int(w2)
```

### Comparing `flux_led-0.28.8/flux_led/const.py` & `flux_led-0.28.9/flux_led/const.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/device.py` & `flux_led-0.28.9/flux_led/device.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/fluxled.py` & `flux_led-0.28.9/flux_led/fluxled.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/models_db.py` & `flux_led-0.28.9/flux_led/models_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,15 +919,15 @@
         device_config=IMMUTABLE_DEVICE_CONFIG,
     ),
     LEDENETModel(
         model_num=0x25,
         # 'AK001-ZJ200' == v2 - some devices have RF remote support (the mini ones)
         models=["HF-LPB100-ZJ200", "AK001-ZJ200"],
         description="Controller RGB/WW/CW",
-        always_writes_white_and_colors=False,  # Formerly rgbwprotocol
+        always_writes_white_and_colors=True,  # Formerly rgbwprotocol
         protocols=[MinVersionProtocol(0, PROTOCOL_LEDENET_9BYTE)],
         mode_to_color_mode=BASE_MODE_MAP,
         color_modes={COLOR_MODE_RGBWW},  # Formerly rgbwcapable
         channel_map={},
         microphone=False,
         device_config=MULTI_MODE_DEVICE_CONFIG,
     ),
@@ -1177,15 +1177,15 @@
         color_modes=COLOR_MODES_ADDRESSABLE,
         channel_map={},
         microphone=True,
         device_config=A2_DEVICE_CONFIG,
     ),
     LEDENETModel(
         model_num=0xA3,
-        # AK001-ZJ2147 v1.19 has RF remote support
+        # AK001-ZJ2147 v1.17, v1.19 has RF remote support
         # AK001-ZJ2148 v1.26, v1.27 has RF remote support, confirmed to be able to change 2.4G remote settings
         models=["AK001-ZJ2147", "AK001-ZJ2148"],
         description="Addressable v3",
         always_writes_white_and_colors=False,
         protocols=[MinVersionProtocol(0, PROTOCOL_LEDENET_ADDRESSABLE_A3)],
         mode_to_color_mode={},
         color_modes=COLOR_MODES_ADDRESSABLE,
```

### Comparing `flux_led-0.28.8/flux_led/pattern.py` & `flux_led-0.28.9/flux_led/pattern.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/protocol.py` & `flux_led-0.28.9/flux_led/protocol.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/scanner.py` & `flux_led-0.28.9/flux_led/scanner.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/sock.py` & `flux_led-0.28.9/flux_led/sock.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/timer.py` & `flux_led-0.28.9/flux_led/timer.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led/utils.py` & `flux_led-0.28.9/flux_led/utils.py`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led.egg-info/PKG-INFO` & `flux_led-0.28.9/flux_led.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-led
-Version: 0.28.8
+Version: 0.28.9
 Summary: A Python library to communicate with the flux_led smart bulbs
 Home-page: https://github.com/Danielhiversen/flux_led
 Author: Daniel Hjelseth Høyer
 Author-email: mail@dahoiv.net
 License: LGPLv3+
 Keywords: flux_led,smart bulbs,light
 Platform: UNKNOWN
```

### Comparing `flux_led-0.28.8/flux_led.egg-info/SOURCES.txt` & `flux_led-0.28.9/flux_led.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/flux_led.egg-info/requires.txt` & `flux_led-0.28.9/flux_led.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flux_led-0.28.8/setup.py` & `flux_led-0.28.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ],
 }
 
 
 setup(
     name="flux_led",
     packages=["flux_led"],
-    version="0.28.8",
+    version="0.28.9",
     description="A Python library to communicate with the flux_led smart bulbs",
     author="Daniel Hjelseth Høyer",
     author_email="mail@dahoiv.net",
     url="https://github.com/Danielhiversen/flux_led",
     license="LGPLv3+",
     include_package_data=True,
     package_data={"flux_led": ["py.typed"]},
```

