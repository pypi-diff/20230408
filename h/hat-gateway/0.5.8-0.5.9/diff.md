# Comparing `tmp/hat_gateway-0.5.8-cp38.cp39-none-any.whl.zip` & `tmp/hat_gateway-0.5.9-cp38.cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 21752 bytes, number of entries: 19
+Zip file size: 21806 bytes, number of entries: 19
 -rw-r--r--  2.0 unx       14 b- defN 21-Feb-19 20:16 hat/gateway/__init__.py
 -rw-r--r--  2.0 unx      128 b- defN 21-Apr-08 11:27 hat/gateway/__main__.py
 -rw-r--r--  2.0 unx     2615 b- defN 21-Feb-22 22:26 hat/gateway/common.py
 -rw-r--r--  2.0 unx     7801 b- defN 21-Nov-13 00:02 hat/gateway/engine.py
 -rw-r--r--  2.0 unx     4801 b- defN 21-Nov-29 22:12 hat/gateway/json_schema_repo.json
 -rw-r--r--  2.0 unx     3728 b- defN 21-Nov-10 14:31 hat/gateway/main.py
 -rw-r--r--  2.0 unx       22 b- defN 21-Feb-19 20:16 hat/gateway/devices/__init__.py
 -rw-r--r--  2.0 unx       21 b- defN 21-May-19 00:33 hat/gateway/devices/modbus/__init__.py
 -rw-r--r--  2.0 unx      353 b- defN 21-Aug-10 11:19 hat/gateway/devices/modbus/master/__init__.py
 -rw-r--r--  2.0 unx     5843 b- defN 21-May-25 14:28 hat/gateway/devices/modbus/master/connection.py
 -rw-r--r--  2.0 unx     8408 b- defN 21-Dec-02 20:31 hat/gateway/devices/modbus/master/device.py
 -rw-r--r--  2.0 unx     5007 b- defN 21-May-26 23:27 hat/gateway/devices/modbus/master/event_client.py
--rw-r--r--  2.0 unx    12606 b- defN 21-Dec-06 13:24 hat/gateway/devices/modbus/master/remote_device.py
--rw-r--r--  2.0 unx    11358 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2232 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1683 b- defN 21-Dec-06 13:32 hat_gateway-0.5.8.dist-info/RECORD
-19 files, 66807 bytes uncompressed, 18954 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx    12777 b- defN 21-Dec-16 17:48 hat/gateway/devices/modbus/master/remote_device.py
+-rw-r--r--  2.0 unx    11358 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2232 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1683 b- defN 21-Dec-16 17:50 hat_gateway-0.5.9.dist-info/RECORD
+19 files, 66978 bytes uncompressed, 19008 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: hat/gateway/devices/modbus/master/event_client.py
 Comment: 
 
 Filename: hat/gateway/devices/modbus/master/remote_device.py
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/LICENSE
+Filename: hat_gateway-0.5.9.dist-info/LICENSE
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/METADATA
+Filename: hat_gateway-0.5.9.dist-info/METADATA
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/WHEEL
+Filename: hat_gateway-0.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/entry_points.txt
+Filename: hat_gateway-0.5.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/top_level.txt
+Filename: hat_gateway-0.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_gateway-0.5.8.dist-info/RECORD
+Filename: hat_gateway-0.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/gateway/devices/modbus/master/remote_device.py

```diff
@@ -237,41 +237,47 @@
         self._data = data
         self._device_id = device_id
         self._data_type = data_type
         self._start_address = start_address
         self._quantity = quantity
         self._interval = interval
         self._response_cb = response_cb
-        self._last_response = None
+        self._is_connected = False
 
         async_group.spawn(self._read_loop)
 
     @property
     def async_group(self):
         return self._async_group
 
     @property
     def is_connected(self):
-        return bool(self._last_response and
-                    self._last_response.result != 'TIMEOUT')
+        return self._is_connected
 
     async def _read_loop(self):
         try:
             mlog.debug('starting read loop')
+            last_responses = {data: None for data in self._data}
+
             while True:
                 mlog.debug('reading data')
                 result = await self._conn.read(
                     self._device_id, self._data_type, self._start_address,
                     self._quantity)
                 mlog.debug('received response (device_id: %s; data_type: %s; '
                            'start_address: %s; quantity: %s): %s',
                            self._device_id, self._data_type,
                            self._start_address, self._quantity, result)
 
+                self._is_connected = not (isinstance(result, Error) and
+                                          result.name == 'TIMEOUT')
+
                 for data in self._data:
+                    last_response = last_responses[data]
+
                     if isinstance(result, Error):
                         value = None
 
                     else:
                         offset = data.start_address - self._start_address
                         value = _get_registers_value(
                             data.register_size, data.bit_offset,
@@ -281,36 +287,36 @@
                     if isinstance(result, Error):
                         mlog.debug('received error response (device_id: %s; '
                                    'data_name: %s): %s',
                                    data.device_id, data.name, result)
                         response = _create_read_response(
                             data, result.name, None, None)
 
-                    elif (self._last_response is None or
-                            self._last_response.result != 'SUCCESS'):
+                    elif (last_response is None or
+                            last_response.result != 'SUCCESS'):
                         mlog.debug('received initial value (device_id: %s; '
                                    'data_name: %s): %s',
                                    data.device_id, data.name, value)
                         response = _create_read_response(
                             data, 'SUCCESS', value, 'INTERROGATE')
 
-                    elif self._last_response.value != value:
+                    elif last_response.value != value:
                         mlog.debug('data value change value (device_id: %s; '
                                    'data_name: %s): %s -> %s',
                                    data.device_id, data.name,
-                                   self._last_response.value, value)
+                                   last_response.value, value)
                         response = _create_read_response(
                             data, 'SUCCESS', value, 'CHANGE')
 
                     else:
                         mlog.debug('no data change')
                         response = None
 
                     if response:
-                        self._last_response = response
+                        last_responses[data] = response
                         self._response_cb(response)
 
                 mlog.debug('waiting poll interval: %s', self._interval)
                 await asyncio.sleep(self._interval)
 
         except ConnectionError:
             mlog.debug('connection closed')
```

## Comparing `hat_gateway-0.5.8.dist-info/LICENSE` & `hat_gateway-0.5.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_gateway-0.5.8.dist-info/METADATA` & `hat_gateway-0.5.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hat-gateway
-Version: 0.5.8
+Version: 0.5.9
 Summary: Hat gateway
 Home-page: https://github.com/hat-open/hat-gateway
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
```

## Comparing `hat_gateway-0.5.8.dist-info/RECORD` & `hat_gateway-0.5.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 hat/gateway/main.py,sha256=IOSd4_5TPRmVQuMZlwMGjnrCC_BAVPm7A8jTk0E-VYM,3728
 hat/gateway/devices/__init__.py,sha256=bUTqbQdM8I9F9P-5OeD47kNlvVgC0zG27UYJPYg3srw,22
 hat/gateway/devices/modbus/__init__.py,sha256=uONGhCvVvD1gP07Vf2KLqLNbDWsaGaHm9SZRL241_Dc,21
 hat/gateway/devices/modbus/master/__init__.py,sha256=LNuZz0hSI9F5jLQwKzSB41xJZcb7gVV_NcpOeOe5xMU,353
 hat/gateway/devices/modbus/master/connection.py,sha256=jywuNeRwUbRBcRr3lRJ5Wuc9ZNI5TzuI6m7JYHxN6fA,5843
 hat/gateway/devices/modbus/master/device.py,sha256=gQ8Lmw_-vLGtwQwzGTkfSSQoZ7LNYraqRloAT17WB5A,8408
 hat/gateway/devices/modbus/master/event_client.py,sha256=vEQXJ0R5OCwrLs5C8ulM8xsAOm60UffuiZtGnrGosEI,5007
-hat/gateway/devices/modbus/master/remote_device.py,sha256=pewQnOXd3Ccx45wKmbFEkmssxvOPtSbIn2M-oUTOBUU,12606
-hat_gateway-0.5.8.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_gateway-0.5.8.dist-info/METADATA,sha256=4-o1iISpRDNQi7Mub27kkkrt1ow0EcVqpj0bL1i7xAE,2232
-hat_gateway-0.5.8.dist-info/WHEEL,sha256=0r8MCP1NVHT-mKGu5LgjJWwiuNvYPN3jw2sVhuFc1nc,112
-hat_gateway-0.5.8.dist-info/entry_points.txt,sha256=79AsAZGTl0THv4jP9B7uKVdhXNFh76ILoyaXfG1wvE8,71
-hat_gateway-0.5.8.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_gateway-0.5.8.dist-info/RECORD,,
+hat/gateway/devices/modbus/master/remote_device.py,sha256=5IiNwDkms4mV9nwkmLIYM-bbWJ1raZ1_a-I2ikMKfzs,12777
+hat_gateway-0.5.9.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_gateway-0.5.9.dist-info/METADATA,sha256=dGIGi7jjS5gWwIxEeoX578zr5h-Uw1gn9oJy76pZsIk,2232
+hat_gateway-0.5.9.dist-info/WHEEL,sha256=0r8MCP1NVHT-mKGu5LgjJWwiuNvYPN3jw2sVhuFc1nc,112
+hat_gateway-0.5.9.dist-info/entry_points.txt,sha256=79AsAZGTl0THv4jP9B7uKVdhXNFh76ILoyaXfG1wvE8,71
+hat_gateway-0.5.9.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_gateway-0.5.9.dist-info/RECORD,,
```

