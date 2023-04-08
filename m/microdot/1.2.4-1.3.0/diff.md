# Comparing `tmp/microdot-1.2.4.tar.gz` & `tmp/microdot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdot-1.2.4.tar", last modified: Fri Mar  3 08:40:21 2023, max compression
+gzip compressed data, was "microdot-1.3.0.tar", last modified: Sat Apr  8 16:21:30 2023, max compression
```

## Comparing `microdot-1.2.4.tar` & `microdot-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2023-03-03 08:40:21.898353 microdot-1.2.4/
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1072 2022-08-15 19:57:22.000000 microdot-1.2.4/LICENSE
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1525 2023-03-03 08:40:21.899352 microdot-1.2.4/PKG-INFO
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      847 2022-08-15 19:57:22.000000 microdot-1.2.4/README.md
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      104 2022-08-15 19:57:22.000000 microdot-1.2.4/pyproject.toml
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1035 2023-03-03 08:40:21.901352 microdot-1.2.4/setup.cfg
--rwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)       38 2022-08-15 19:57:22.000000 microdot-1.2.4/setup.py
-drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2023-03-03 08:40:21.870367 microdot-1.2.4/src/
-drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2023-03-03 08:40:21.876364 microdot-1.2.4/src/microdot.egg-info/
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1525 2023-03-03 08:40:21.000000 microdot-1.2.4/src/microdot.egg-info/PKG-INFO
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      999 2023-03-03 08:40:21.000000 microdot-1.2.4/src/microdot.egg-info/SOURCES.txt
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        1 2023-03-03 08:40:21.000000 microdot-1.2.4/src/microdot.egg-info/dependency_links.txt
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        1 2022-08-15 19:58:01.000000 microdot-1.2.4/src/microdot.egg-info/not-zip-safe
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      248 2023-03-03 08:40:21.000000 microdot-1.2.4/src/microdot.egg-info/top_level.txt
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    43265 2023-02-28 18:30:11.000000 microdot-1.2.4/src/microdot.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     4912 2023-03-03 08:14:41.000000 microdot-1.2.4/src/microdot_asgi.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2855 2022-09-04 12:32:37.000000 microdot-1.2.4/src/microdot_asgi_websocket.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    17172 2023-02-21 18:54:48.000000 microdot-1.2.4/src/microdot_asyncio.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     7828 2022-09-17 19:45:12.000000 microdot-1.2.4/src/microdot_asyncio_test_client.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     3780 2022-09-04 12:32:37.000000 microdot-1.2.4/src/microdot_asyncio_websocket.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1128 2022-08-15 19:57:22.000000 microdot-1.2.4/src/microdot_jinja.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2966 2022-12-10 23:31:08.000000 microdot-1.2.4/src/microdot_session.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    10779 2022-12-10 23:31:08.000000 microdot-1.2.4/src/microdot_test_client.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1331 2022-08-15 19:57:22.000000 microdot-1.2.4/src/microdot_utemplate.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     5935 2022-12-10 23:31:08.000000 microdot-1.2.4/src/microdot_websocket.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     3486 2022-09-17 19:40:02.000000 microdot-1.2.4/src/microdot_websocket_alt.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2364 2022-12-10 23:31:08.000000 microdot-1.2.4/src/microdot_wsgi.py
-drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2023-03-03 08:40:21.897354 microdot-1.2.4/tests/
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1818 2022-09-04 12:32:37.000000 microdot-1.2.4/tests/test_jinja.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    22691 2023-02-21 18:54:48.000000 microdot-1.2.4/tests/test_microdot.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     5072 2023-03-03 08:14:41.000000 microdot-1.2.4/tests/test_microdot_asgi.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    22819 2023-02-21 18:54:48.000000 microdot-1.2.4/tests/test_microdot_asyncio.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2087 2022-09-04 12:32:37.000000 microdot-1.2.4/tests/test_microdot_asyncio_websocket.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2670 2022-09-04 12:32:37.000000 microdot-1.2.4/tests/test_microdot_websocket.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     3449 2022-09-17 19:40:02.000000 microdot-1.2.4/tests/test_microdot_wsgi.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2083 2022-12-10 23:31:08.000000 microdot-1.2.4/tests/test_multidict.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     5454 2022-08-15 19:57:22.000000 microdot-1.2.4/tests/test_request.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     5272 2022-09-04 12:32:37.000000 microdot-1.2.4/tests/test_request_asyncio.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    10455 2022-09-17 19:44:15.000000 microdot-1.2.4/tests/test_response.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     5784 2022-09-17 19:40:02.000000 microdot-1.2.4/tests/test_response_asyncio.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     3855 2022-12-10 23:31:08.000000 microdot-1.2.4/tests/test_session.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     4050 2022-08-15 19:57:22.000000 microdot-1.2.4/tests/test_url_pattern.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      403 2022-12-10 23:31:08.000000 microdot-1.2.4/tests/test_urlencode.py
--rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1752 2022-09-04 12:32:37.000000 microdot-1.2.4/tests/test_utemplate.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.021456 microdot-1.3.0/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.0/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-04-08 16:21:30.021861 microdot-1.3.0/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.0/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.0/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-04-08 16:21:30.023421 microdot-1.3.0/setup.cfg
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.0/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.000315 microdot-1.3.0/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.004421 microdot-1.3.0/src/microdot.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.0/src/microdot.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/top_level.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    46220 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4912 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asgi_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_utemplate.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_websocket_alt.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_wsgi.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.020610 microdot-1.3.0/tests/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_cors.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5072 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_wsgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-03-23 00:04:52.000000 microdot-1.3.0/tests/test_multidict.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-04-08 16:16:17.000000 microdot-1.3.0/tests/test_request.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_request_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-03-21 00:28:33.000000 microdot-1.3.0/tests/test_response.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_response_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4050 2020-02-18 23:41:59.000000 microdot-1.3.0/tests/test_url_pattern.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2022-09-24 18:55:50.000000 microdot-1.3.0/tests/test_urlencode.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_utemplate.py
```

### Comparing `microdot-1.2.4/LICENSE` & `microdot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/PKG-INFO` & `microdot-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.2.4
+Version: 1.3.0
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.2.4/README.md` & `microdot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/setup.cfg` & `microdot-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = microdot
-version = 1.2.4
+version = 1.3.0
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = The impossibly small web framework for MicroPython
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/microdot
 project_urls =
```

### Comparing `microdot-1.2.4/src/microdot.egg-info/PKG-INFO` & `microdot-1.3.0/src/microdot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.2.4
+Version: 1.3.0
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.2.4/src/microdot.egg-info/SOURCES.txt` & `microdot-1.3.0/src/microdot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/microdot_websocket_alt.py
 src/microdot_wsgi.py
 src/microdot.egg-info/PKG-INFO
 src/microdot.egg-info/SOURCES.txt
 src/microdot.egg-info/dependency_links.txt
 src/microdot.egg-info/not-zip-safe
 src/microdot.egg-info/top_level.txt
+tests/test_cors.py
 tests/test_jinja.py
 tests/test_microdot.py
 tests/test_microdot_asgi.py
 tests/test_microdot_asyncio.py
 tests/test_microdot_asyncio_websocket.py
 tests/test_microdot_websocket.py
 tests/test_microdot_wsgi.py
```

### Comparing `microdot-1.2.4/src/microdot.py` & `microdot-1.3.0/src/microdot.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,18 @@
         kl = key.lower()
         return self.keymap.get(kl, kl) in self.keys()
 
     def get(self, key, default=None):
         kl = key.lower()
         return super().get(self.keymap.get(kl, kl), default)
 
+    def update(self, other_dict):
+        for key, value in other_dict.items():
+            self[key] = value
+
 
 def mro(cls):  # pragma: no cover
     """Return the method resolution order of a class.
 
     This is a helper function that returns the method resolution order of a
     class. It is used by Microdot to find the best error handler to invoke for
     the raised exception.
@@ -396,19 +400,19 @@
                        stream=client_stream, sock=client_sock)
 
     def _parse_urlencoded(self, urlencoded):
         data = MultiDict()
         if len(urlencoded) > 0:
             if isinstance(urlencoded, str):
                 for k, v in [pair.split('=', 1)
-                             for pair in urlencoded.split('&')]:
+                             for pair in urlencoded.split('&') if pair]:
                     data[urldecode_str(k)] = urldecode_str(v)
             elif isinstance(urlencoded, bytes):  # pragma: no branch
                 for k, v in [pair.split(b'=', 1)
-                             for pair in urlencoded.split(b'&')]:
+                             for pair in urlencoded.split(b'&') if pair]:
                     data[urldecode_bytes(k)] = urldecode_bytes(v)
         return data
 
     @property
     def body(self):
         """The body of the request, as bytes."""
         if self.stream_used:
@@ -521,14 +525,18 @@
     }
     send_file_buffer_size = 1024
 
     #: The content type to use for responses that do not explicitly define a
     #: ``Content-Type`` header.
     default_content_type = 'text/plain'
 
+    #: The default cache control max age used by :meth:`send_file`. A value
+    #: of ``None`` means that no ``Cache-Control`` header is added.
+    default_send_file_max_age = None
+
     #: Special response used to signal that a response does not need to be
     #: written to the client. Used to exit WebSocket connections cleanly.
     already_handled = None
 
     def __init__(self, body='', status_code=200, headers=None, reason=None):
         if body is None and status_code == 200:
             body = ''
@@ -540,14 +548,15 @@
             self.body = json.dumps(body).encode()
             self.headers['Content-Type'] = 'application/json; charset=UTF-8'
         elif isinstance(body, str):
             self.body = body.encode()
         else:
             # this applies to bytes, file-like objects or generators
             self.body = body
+        self.is_head = False
 
     def set_cookie(self, cookie, value, path=None, domain=None, expires=None,
                    max_age=None, secure=False, http_only=False):
         """Add a cookie to the response.
 
         :param cookie: The cookie's name.
         :param value: The cookie's value.
@@ -604,27 +613,28 @@
             values = value if isinstance(value, list) else [value]
             for value in values:
                 stream.write('{header}: {value}\r\n'.format(
                     header=header, value=value).encode())
         stream.write(b'\r\n')
 
         # body
-        can_flush = hasattr(stream, 'flush')
-        try:
-            for body in self.body_iter():
-                if isinstance(body, str):  # pragma: no cover
-                    body = body.encode()
-                stream.write(body)
-                if can_flush:  # pragma: no cover
-                    stream.flush()
-        except OSError as exc:  # pragma: no cover
-            if exc.errno in MUTED_SOCKET_ERRORS:
-                pass
-            else:
-                raise
+        if not self.is_head:
+            can_flush = hasattr(stream, 'flush')
+            try:
+                for body in self.body_iter():
+                    if isinstance(body, str):  # pragma: no cover
+                        body = body.encode()
+                    stream.write(body)
+                    if can_flush:  # pragma: no cover
+                        stream.flush()
+            except OSError as exc:  # pragma: no cover
+                if exc.errno in MUTED_SOCKET_ERRORS:
+                    pass
+                else:
+                    raise
 
     def body_iter(self):
         if self.body:
             if hasattr(self.body, 'read'):
                 while True:
                     buf = self.body.read(self.send_file_buffer_size)
                     if len(buf):
@@ -647,37 +657,67 @@
                             default is 302.
         """
         if '\x0d' in location or '\x0a' in location:
             raise ValueError('invalid redirect URL')
         return cls(status_code=status_code, headers={'Location': location})
 
     @classmethod
-    def send_file(cls, filename, status_code=200, content_type=None):
+    def send_file(cls, filename, status_code=200, content_type=None,
+                  stream=None, max_age=None, compressed=False,
+                  file_extension=''):
         """Send file contents in a response.
 
         :param filename: The filename of the file.
         :param status_code: The 3xx status code to use for the redirect. The
                             default is 302.
         :param content_type: The ``Content-Type`` header to use in the
                              response. If omitted, it is generated
-                             automatically from the file extension.
+                             automatically from the file extension of the
+                             ``filename`` parameter.
+        :param stream: A file-like object to read the file contents from. If
+                       a stream is given, the ``filename`` parameter is only
+                       used when generating the ``Content-Type`` header.
+        :param max_age: The ``Cache-Control`` header's ``max-age`` value in
+                        seconds. If omitted, the value of the
+                        :attr:`Response.default_send_file_max_age` attribute is
+                        used.
+        :param compressed: Whether the file is compressed. If ``True``, the
+                           ``Content-Encoding`` header is set to ``gzip``. A
+                           string with the header value can also be passed.
+                           Note that when using this option the file must have
+                           been compressed beforehand. This option only sets
+                           the header.
+        :param file_extension: A file extension to append to the ``filename``
+                               parameter when opening the file, including the
+                               dot. The extension given here is not considered
+                               when generating the ``Content-Type`` header.
 
         Security note: The filename is assumed to be trusted. Never pass
         filenames provided by the user without validating and sanitizing them
         first.
         """
         if content_type is None:
             ext = filename.split('.')[-1]
             if ext in Response.types_map:
                 content_type = Response.types_map[ext]
             else:
                 content_type = 'application/octet-stream'
-        f = open(filename, 'rb')
-        return cls(body=f, status_code=status_code,
-                   headers={'Content-Type': content_type})
+        headers = {'Content-Type': content_type}
+
+        if max_age is None:
+            max_age = cls.default_send_file_max_age
+        if max_age is not None:
+            headers['Cache-Control'] = 'max-age={}'.format(max_age)
+
+        if compressed:
+            headers['Content-Encoding'] = compressed \
+                if isinstance(compressed, str) else 'gzip'
+
+        f = stream or open(filename + file_extension, 'rb')
+        return cls(body=f, status_code=status_code, headers=headers)
 
 
 class URLPattern():
     def __init__(self, url_pattern):
         self.url_pattern = url_pattern
         self.pattern = ''
         self.args = []
@@ -755,14 +795,15 @@
     def __init__(self):
         self.url_map = []
         self.before_request_handlers = []
         self.after_request_handlers = []
         self.after_error_request_handlers = []
         self.error_handlers = {}
         self.shutdown_requested = False
+        self.options_handler = self.default_options_handler
         self.debug = False
         self.server = None
 
     def route(self, url_pattern, methods=None):
         """Decorator that is used to register a function as a request handler
         for a given URL.
 
@@ -790,15 +831,16 @@
 
             @app.route('/')
             def index(request):
                 return 'Hello, world!'
         """
         def decorated(f):
             self.url_map.append(
-                (methods or ['GET'], URLPattern(url_pattern), f))
+                ([m.upper() for m in (methods or ['GET'])],
+                 URLPattern(url_pattern), f))
             return f
         return decorated
 
     def get(self, url_pattern):
         """Decorator that is used to register a function as a ``GET`` request
         handler for a given URL.
 
@@ -1076,25 +1118,40 @@
             def shutdown(request):
                 request.app.shutdown()
                 return 'The server is shutting down...'
         """
         self.shutdown_requested = True
 
     def find_route(self, req):
+        method = req.method.upper()
+        if method == 'OPTIONS' and self.options_handler:
+            return self.options_handler(req)
+        if method == 'HEAD':
+            method = 'GET'
         f = 404
         for route_methods, route_pattern, route_handler in self.url_map:
             req.url_args = route_pattern.match(req.path)
             if req.url_args is not None:
-                if req.method in route_methods:
+                if method in route_methods:
                     f = route_handler
                     break
                 else:
                     f = 405
         return f
 
+    def default_options_handler(self, req):
+        allow = []
+        for route_methods, route_pattern, route_handler in self.url_map:
+            if route_pattern.match(req.path) is not None:
+                allow.extend(route_methods)
+        if 'GET' in allow:
+            allow.append('HEAD')
+        allow.append('OPTIONS')
+        return {'Allow': ', '.join(allow)}
+
     def handle_request(self, sock, addr):
         if Request.socket_read_timeout and \
                 hasattr(sock, 'settimeout'):  # pragma: no cover
             sock.settimeout(Request.socket_read_timeout)
         if not hasattr(sock, 'readline'):  # pragma: no cover
             stream = sock.makefile("rwb")
         else:
@@ -1161,14 +1218,16 @@
                         elif not isinstance(res, Response):
                             res = Response(res)
                         for handler in self.after_request_handlers:
                             res = handler(req, res) or res
                         for handler in req.after_request_handlers:
                             res = handler(req, res) or res
                         after_request_handled = True
+                    elif isinstance(f, dict):
+                        res = Response(headers=f)
                     elif f in self.error_handlers:
                         res = self.error_handlers[f](req)
                     else:
                         res = 'Not found', f
                 except HTTPException as exc:
                     if exc.status_code in self.error_handlers:
                         res = self.error_handlers[exc.status_code](req)
@@ -1204,14 +1263,15 @@
         if isinstance(res, tuple):
             res = Response(*res)
         elif not isinstance(res, Response):
             res = Response(res)
         if not after_request_handled:
             for handler in self.after_error_request_handlers:
                 res = handler(req, res) or res
+        res.is_head = (req and req.method == 'HEAD')
         return res
 
 
 abort = Microdot.abort
 Response.already_handled = Response()
 redirect = Response.redirect
 send_file = Response.send_file
```

### Comparing `microdot-1.2.4/src/microdot_asgi.py` & `microdot-1.3.0/src/microdot_asgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_asgi_websocket.py` & `microdot-1.3.0/src/microdot_asgi_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_asyncio.py` & `microdot-1.3.0/src/microdot_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,18 +147,19 @@
                 values = value if isinstance(value, list) else [value]
                 for value in values:
                     await stream.awrite('{header}: {value}\r\n'.format(
                         header=header, value=value).encode())
             await stream.awrite(b'\r\n')
 
             # body
-            async for body in self.body_iter():
-                if isinstance(body, str):  # pragma: no cover
-                    body = body.encode()
-                await stream.awrite(body)
+            if not self.is_head:
+                async for body in self.body_iter():
+                    if isinstance(body, str):  # pragma: no cover
+                        body = body.encode()
+                    await stream.awrite(body)
         except OSError as exc:  # pragma: no cover
             if exc.errno in MUTED_SOCKET_ERRORS or \
                     exc.args[0] == 'Connection lost':
                 pass
             else:
                 raise
 
@@ -381,14 +382,16 @@
                         for handler in self.after_request_handlers:
                             res = await self._invoke_handler(
                                 handler, req, res) or res
                         for handler in req.after_request_handlers:
                             res = await self._invoke_handler(
                                 handler, req, res) or res
                         after_request_handled = True
+                    elif isinstance(f, dict):
+                        res = Response(headers=f)
                     elif f in self.error_handlers:
                         res = await self._invoke_handler(
                             self.error_handlers[f], req)
                     else:
                         res = 'Not found', f
                 except HTTPException as exc:
                     if exc.status_code in self.error_handlers:
@@ -427,14 +430,15 @@
             res = Response(*res)
         elif not isinstance(res, Response):
             res = Response(res)
         if not after_request_handled:
             for handler in self.after_error_request_handlers:
                 res = await self._invoke_handler(
                     handler, req, res) or res
+        res.is_head = (req and req.method == 'HEAD')
         return res
 
     async def _invoke_handler(self, f_or_coro, *args, **kwargs):
         ret = f_or_coro(*args, **kwargs)
         if _iscoroutine(ret):
             ret = await ret
         return ret
```

### Comparing `microdot-1.2.4/src/microdot_asyncio_test_client.py` & `microdot-1.3.0/src/microdot_asyncio_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_asyncio_websocket.py` & `microdot-1.3.0/src/microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_jinja.py` & `microdot-1.3.0/src/microdot_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_session.py` & `microdot-1.3.0/src/microdot_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_test_client.py` & `microdot-1.3.0/src/microdot_test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     @classmethod
     def create(cls, res):
         test_res = cls()
         test_res._initialize_response(res)
         test_res._initialize_body(res)
         test_res._process_text_body()
         test_res._process_json_body()
+        test_res.is_head = res.is_head
         return test_res
 
 
 class TestClient:
     """A test client for Microdot.
 
     :param app: The Microdot application instance.
```

### Comparing `microdot-1.2.4/src/microdot_utemplate.py` & `microdot-1.3.0/src/microdot_utemplate.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_websocket.py` & `microdot-1.3.0/src/microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_websocket_alt.py` & `microdot-1.3.0/src/microdot_websocket_alt.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/src/microdot_wsgi.py` & `microdot-1.3.0/src/microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_jinja.py` & `microdot-1.3.0/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_microdot.py` & `microdot-1.3.0/tests/test_microdot.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,60 @@
         res = client.post('/')
         self.assertEqual(res.status_code, 200)
         self.assertEqual(res.headers['Content-Type'],
                          'text/plain; charset=UTF-8')
         self.assertEqual(res.headers['Content-Length'], '3')
         self.assertEqual(res.text, 'bar')
 
+    def test_head_request(self):
+        self._mock()
+
+        app = Microdot()
+
+        @app.route('/foo')
+        def index(req):
+            return 'foo'
+
+        mock_socket.clear_requests()
+        fd = mock_socket.add_request('HEAD', '/foo')
+        self._add_shutdown(app)
+        app.run()
+
+        self.assertTrue(fd.response.startswith(b'HTTP/1.0 200 OK\r\n'))
+        self.assertIn(b'Content-Length: 3\r\n', fd.response)
+        self.assertIn(b'Content-Type: text/plain; charset=UTF-8\r\n',
+                      fd.response)
+        self.assertTrue(fd.response.endswith(b'\r\n\r\n'))
+
+        self._unmock()
+
+    def test_options_request(self):
+        app = Microdot()
+
+        @app.route('/', methods=['GET', 'DELETE'])
+        def index(req):
+            return 'foo'
+
+        @app.post('/')
+        def index_post(req):
+            return 'bar'
+
+        @app.route('/foo', methods=['POST', 'PUT'])
+        def foo(req):
+            return 'baz'
+
+        client = TestClient(app)
+        res = client.request('OPTIONS', '/')
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Allow'],
+                         'GET, DELETE, POST, HEAD, OPTIONS')
+        res = client.request('OPTIONS', '/foo')
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Allow'], 'POST, PUT, OPTIONS')
+
     def test_empty_request(self):
         self._mock()
 
         app = Microdot()
 
         mock_socket.clear_requests()
         fd = mock_socket.FakeStream(b'\n')
```

### Comparing `microdot-1.2.4/tests/test_microdot_asgi.py` & `microdot-1.3.0/tests/test_microdot_asgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_microdot_asyncio.py` & `microdot-1.3.0/tests/test_microdot_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,56 @@
         self.assertEqual(res.headers['Content-Type'],
                          'text/plain; charset=UTF-8')
         self.assertEqual(res.headers['Content-Length'], '9')
         self.assertEqual(res.text, 'bar-async')
         self.assertEqual(res.body, b'bar-async')
         self.assertEqual(res.json, None)
 
+    def test_head_request(self):
+        app = Microdot()
+
+        @app.route('/foo')
+        def index(req):
+            return 'foo'
+
+        mock_socket.clear_requests()
+        fd = mock_socket.add_request('HEAD', '/foo')
+        self._add_shutdown(app)
+        app.run()
+
+        self.assertTrue(fd.response.startswith(b'HTTP/1.0 200 OK\r\n'))
+        self.assertIn(b'Content-Length: 3\r\n', fd.response)
+        self.assertIn(b'Content-Type: text/plain; charset=UTF-8\r\n',
+                      fd.response)
+        self.assertTrue(fd.response.endswith(b'\r\n\r\n'))
+
+    def test_options_request(self):
+        app = Microdot()
+
+        @app.route('/', methods=['GET', 'DELETE'])
+        async def index(req):
+            return 'foo'
+
+        @app.post('/')
+        async def index_post(req):
+            return 'bar'
+
+        @app.route('/foo', methods=['POST', 'PUT'])
+        async def foo(req):
+            return 'baz'
+
+        client = TestClient(app)
+        res = self._run(client.request('OPTIONS', '/'))
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Allow'],
+                         'GET, DELETE, POST, HEAD, OPTIONS')
+        res = self._run(client.request('OPTIONS', '/foo'))
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Allow'], 'POST, PUT, OPTIONS')
+
     def test_empty_request(self):
         app = Microdot()
 
         mock_socket.clear_requests()
         fd = mock_socket.FakeStream(b'\n')
         mock_socket._requests.append(fd)
         self._add_shutdown(app)
```

### Comparing `microdot-1.2.4/tests/test_microdot_asyncio_websocket.py` & `microdot-1.3.0/tests/test_microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_microdot_websocket.py` & `microdot-1.3.0/tests/test_microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_microdot_wsgi.py` & `microdot-1.3.0/tests/test_microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_multidict.py` & `microdot-1.3.0/tests/test_multidict.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,7 +54,15 @@
         self.assertIn(('two', 5), list(d.items()))
         self.assertIn(4, list(d.values()))
         self.assertIn(5, list(d.values()))
 
         del d['oNE']
         self.assertEqual(list(d.items()), [('two', 5)])
         self.assertEqual(list(d.values()), [5])
+
+        d.update({'oNe': 1, 'two': 2, 'three': 3})
+        self.assertEqual(d['one'], 1)
+        self.assertEqual(d['ONE'], 1)
+        self.assertEqual(d['two'], 2)
+        self.assertEqual(d['TWO'], 2)
+        self.assertEqual(d['three'], 3)
+        self.assertEqual(d['THREE'], 3)
```

### Comparing `microdot-1.2.4/tests/test_request.py` & `microdot-1.3.0/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,21 @@
     def test_args(self):
         fd = get_request_fd('GET', '/?foo=bar&abc=def&x=%2f%%')
         req = Request.create('app', fd, 'addr')
         self.assertEqual(req.query_string, 'foo=bar&abc=def&x=%2f%%')
         self.assertEqual(req.args, MultiDict(
             {'foo': 'bar', 'abc': 'def', 'x': '/%%'}))
 
+    def test_badly_formatted_args(self):
+        fd = get_request_fd('GET', '/?&foo=bar&abc=def&&&x=%2f%%')
+        req = Request.create('app', fd, 'addr')
+        self.assertEqual(req.query_string, '&foo=bar&abc=def&&&x=%2f%%')
+        self.assertEqual(req.args, MultiDict(
+            {'foo': 'bar', 'abc': 'def', 'x': '/%%'}))
+
     def test_json(self):
         fd = get_request_fd('GET', '/foo', headers={
             'Content-Type': 'application/json'}, body='{"foo":"bar"}')
         req = Request.create('app', fd, 'addr')
         json = req.json
         self.assertEqual(json, {'foo': 'bar'})
         self.assertTrue(req.json is json)
```

### Comparing `microdot-1.2.4/tests/test_request_asyncio.py` & `microdot-1.3.0/tests/test_request_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_response.py` & `microdot-1.3.0/tests/test_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -231,14 +231,47 @@
         res.write(fd)
         response = fd.getvalue()
         self.assertEqual(
             response,
             b'HTTP/1.0 200 OK\r\nContent-Type: text/html\r\n\r\nfoo\n')
         Response.send_file_buffer_size = original_buffer_size
 
+    def test_send_file_max_age(self):
+        res = Response.send_file('tests/files/test.txt', max_age=123)
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Cache-Control'], 'max-age=123')
+
+        Response.default_send_file_max_age = 456
+        res = Response.send_file('tests/files/test.txt')
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Cache-Control'], 'max-age=456')
+        res = Response.send_file('tests/files/test.txt', max_age=123)
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Cache-Control'], 'max-age=123')
+
+        Response.default_send_file_max_age = None
+
+    def test_send_file_compressed(self):
+        res = Response.send_file('tests/files/test.txt', compressed=True)
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Content-Type'], 'text/plain')
+        self.assertEqual(res.headers['Content-Encoding'], 'gzip')
+
+        res = Response.send_file('tests/files/test.txt', compressed='foo')
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Content-Type'], 'text/plain')
+        self.assertEqual(res.headers['Content-Encoding'], 'foo')
+
+        res = Response.send_file('tests/files/test', compressed=True,
+                                 file_extension='.gz')
+        self.assertEqual(res.status_code, 200)
+        self.assertEqual(res.headers['Content-Type'],
+                         'application/octet-stream')
+        self.assertEqual(res.headers['Content-Encoding'], 'gzip')
+
     def test_default_content_type(self):
         original_content_type = Response.default_content_type
         res = Response('foo')
         res.complete()
         self.assertEqual(res.headers['Content-Type'],
                          'text/plain; charset=UTF-8')
         Response.default_content_type = 'text/html'
```

### Comparing `microdot-1.2.4/tests/test_response_asyncio.py` & `microdot-1.3.0/tests/test_response_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_session.py` & `microdot-1.3.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_url_pattern.py` & `microdot-1.3.0/tests/test_url_pattern.py`

 * *Files identical despite different names*

### Comparing `microdot-1.2.4/tests/test_utemplate.py` & `microdot-1.3.0/tests/test_utemplate.py`

 * *Files identical despite different names*

