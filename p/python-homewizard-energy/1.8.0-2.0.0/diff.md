# Comparing `tmp/python_homewizard_energy-1.8.0.tar.gz` & `tmp/python_homewizard_energy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_homewizard_energy-1.8.0.tar", max compression
+gzip compressed data, was "python_homewizard_energy-2.0.0.tar", max compression
```

## Comparing `python_homewizard_energy-1.8.0.tar` & `python_homewizard_energy-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11346 2023-01-25 16:10:24.616600 python_homewizard_energy-1.8.0/LICENSE
--rw-r--r--   0        0        0      936 2023-01-25 16:10:24.616600 python_homewizard_energy-1.8.0/README.md
--rw-r--r--   0        0        0      515 2023-01-25 16:10:24.616600 python_homewizard_energy-1.8.0/homewizard_energy/__init__.py
--rw-r--r--   0        0        0       69 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/const.py
--rw-r--r--   0        0        0      640 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/errors.py
--rw-r--r--   0        0        0     1994 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/features.py
--rw-r--r--   0        0        0     8953 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/homewizard_energy.py
--rw-r--r--   0        0        0    11246 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/models.py
--rw-r--r--   0        0        0        0 2023-01-25 16:10:24.620600 python_homewizard_energy-1.8.0/homewizard_energy/py.typed
--rw-r--r--   0        0        0     2383 2023-01-25 16:11:33.647929 python_homewizard_energy-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_homewizard_energy-1.8.0/setup.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/LICENSE
+-rw-r--r--   0        0        0      936 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/README.md
+-rw-r--r--   0        0        0      468 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/const.py
+-rw-r--r--   0        0        0      765 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/errors.py
+-rw-r--r--   0        0        0     8412 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/homewizard_energy.py
+-rw-r--r--   0        0        0    11246 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/models.py
+-rw-r--r--   0        0        0        0 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/py.typed
+-rw-r--r--   0        0        0     2383 2023-04-08 18:32:26.890309 python_homewizard_energy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.0/setup.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.0/PKG-INFO
```

### Comparing `python_homewizard_energy-1.8.0/LICENSE` & `python_homewizard_energy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-1.8.0/README.md` & `python_homewizard_energy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-1.8.0/homewizard_energy/errors.py` & `python_homewizard_energy-2.0.0/homewizard_energy/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 class RequestError(HomeWizardEnergyException):
     """Unable to fulfill request.
 
     Raised when host or API cannot be reached.
     """
 
 
+class NotFoundError(HomeWizardEnergyException):
+    """Request not found.
+
+    Raised when API responds with '404'
+    """
+
+
 class InvalidStateError(HomeWizardEnergyException):
     """Raised when the device is not in the correct state."""
 
 
 class UnsupportedError(HomeWizardEnergyException):
     """Raised when the device is not supported from this library."""
```

### Comparing `python_homewizard_energy-1.8.0/homewizard_energy/homewizard_energy.py` & `python_homewizard_energy-2.0.0/homewizard_energy/homewizard_energy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 """Representation of a HomeWizard Energy device."""
 from __future__ import annotations
 
 import asyncio
 import logging
 import string
+from collections.abc import Callable, Coroutine
 from http import HTTPStatus
-from typing import Any, cast
+from typing import Any
 
 import async_timeout
 from aiohttp.client import ClientError, ClientResponseError, ClientSession
 from aiohttp.hdrs import METH_DELETE, METH_GET, METH_PUT
 
 from .const import SUPPORTED_API_VERSION
-from .errors import DisabledError, RequestError, UnsupportedError
-from .features import Features
+from .errors import DisabledError, NotFoundError, RequestError, UnsupportedError
 from .models import Data, Decryption, Device, State, System
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def optional_method(
+    func: Callable[..., Coroutine[Any, Any, None]]
+) -> Callable[..., Coroutine[Any, Any, None]]:
+    """Check if method is supported."""
+
+    async def wrapper(self, *args, **kwargs):
+        try:
+            return await func(self, *args, **kwargs)
+        except NotFoundError as ex:
+            raise UnsupportedError(f"{func.__name__} is not supported") from ex
+
+    return wrapper
+
+
 class HomeWizardEnergy:
     """Communicate with a HomeWizard Energy device."""
 
     _session: ClientSession | None
     _close_session: bool = False
     _request_timeout: int = 10
 
-    _features: Features | None = None
-
     def __init__(
         self, host: str, clientsession: ClientSession = None, timeout: int = 10
     ):
         """Create a HomeWizard Energy object.
 
         Args:
             host: IP or URL for device.
@@ -49,60 +61,46 @@
 
         Returns:
             host: The used host
 
         """
         return self._host
 
-    async def features(self) -> Features:
-        """Create or return Features object."""
-        if self.features is None:
-            await self.device()
-
-        return cast(Features, self._features)
-
     async def device(self) -> Device:
         """Return the device object."""
         response = await self.request("api")
         device = Device.from_dict(response)
 
-        self._features = Features(device.product_type, device.firmware_version)
-
         if device.api_version != SUPPORTED_API_VERSION:
             raise UnsupportedError(
                 f"Unsupported API version, expected version '{SUPPORTED_API_VERSION}'"
             )
 
         return device
 
     async def data(self) -> Data:
         """Return the data object."""
         response = await self.request("api/v1/data")
         return Data.from_dict(response)
 
+    @optional_method
     async def state(self) -> State | None:
         """Return the state object."""
-        features = await self.features()
-        if not features.has_state:
-            return None
-
         response = await self.request("api/v1/state")
         return State.from_dict(response)
 
+    @optional_method
     async def state_set(
         self,
         power_on: bool | None = None,
         switch_lock: bool | None = None,
         brightness: int | None = None,
     ) -> bool:
         """Set state of device."""
         state: dict[str, bool | str] = {}
-        features = await self.features()
-        if not features.has_state:
-            raise UnsupportedError("Setting state is not supported with this device")
 
         if power_on is not None:
             state["power_on"] = power_on
         if switch_lock is not None:
             state["switch_lock"] = switch_lock
         if brightness is not None:
             state["brightness"] = brightness
@@ -110,67 +108,59 @@
         if not state:
             _LOGGER.error("At least one state update is required")
             return False
 
         await self.request("api/v1/state", method=METH_PUT, data=state)
         return True
 
+    @optional_method
     async def system(self) -> System:
         """Return the system object."""
         response = await self.request("api/v1/system")
         return System.from_dict(response)
 
+    @optional_method
     async def system_set(
         self,
         cloud_enabled: bool | None = None,
     ) -> bool:
         """Set state of device."""
         state = {}
-        features = await self.features()
-        if not features.has_system:
-            raise UnsupportedError("Setting system is not supported with this device")
-
         if cloud_enabled is not None:
             state["cloud_enabled"] = cloud_enabled
 
         if not state:
             _LOGGER.error("At least one state update is required")
             return False
 
         await self.request("api/v1/system", method=METH_PUT, data=state)
         return True
 
+    @optional_method
     async def identify(
         self,
     ) -> bool:
         """Send identify request."""
-        features = await self.features()
-        if not features.has_identify:
-            raise UnsupportedError("Identify is not supported")
-
         await self.request("api/v1/identify", method=METH_PUT)
         return True
 
+    @optional_method
     async def decryption(self) -> Decryption:
         """Return the decryption object."""
         response = await self.request("api/v1/decryption")
         return Decryption.from_dict(response)
 
+    @optional_method
     async def decryption_set(
         self,
         key: str | None = None,
         aad: str | None = None,
     ) -> bool:
         """Set state of device."""
         data = {}
-        features = await self.features()
-        if not features.has_decryption:
-            raise UnsupportedError(
-                "Setting decryption is not supported with this device"
-            )
 
         if key is not None:
             if len(key) != 32:
                 raise ValueError("Key length should be 32 characters long")
             if not all(c in string.hexdigits for c in key):
                 raise ValueError(
                     "Key should only contain hexadecimal characters (0-9/a-f)"
@@ -195,26 +185,21 @@
         if not data:
             _LOGGER.error("At least one decryption key is required")
             return False
 
         await self.request("api/v1/decryption", method=METH_PUT, data=data)
         return True
 
+    @optional_method
     async def decryption_reset(
         self,
         key: bool = False,
         aad: bool = False,
     ) -> bool:
         """Reset decryption keys of device."""
-        features = await self.features()
-        if not features.has_decryption:
-            raise UnsupportedError(
-                "Setting decryption is not supported with this device"
-            )
-
         data = {
             "key": key,
             "aad": aad,
         }
 
         await self.request("api/v1/decryption", method=METH_DELETE, data=data)
         return True
@@ -252,14 +237,18 @@
 
         if resp.status == HTTPStatus.FORBIDDEN:
             # Known case: API disabled
             raise DisabledError(
                 "API disabled. API must be enabled in HomeWizard Energy app"
             )
 
+        if resp.status == HTTPStatus.NOT_FOUND:
+            # Known case: API endpoint not supported
+            raise NotFoundError("Resource not found")
+
         if resp.status != HTTPStatus.OK:
             # Something else went wrong
             raise RequestError(f"API request error ({resp.status})")
 
         content_type = resp.headers.get("Content-Type", "")
         if "application/json" in content_type:
             return await resp.json()
```

### Comparing `python_homewizard_energy-1.8.0/homewizard_energy/models.py` & `python_homewizard_energy-2.0.0/homewizard_energy/models.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-1.8.0/pyproject.toml` & `python_homewizard_energy-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-homewizard-energy"
-version = "1.8.0"
+version = "2.0.0"
 description = "Asynchronous Python client for the HomeWizard Energy"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-homewizard-energy"
 repository = "https://github.com/dcsbl/python-homewizard-energy"
```

### Comparing `python_homewizard_energy-1.8.0/setup.py` & `python_homewizard_energy-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0.0', 'awesomeversion>=22.9.0']
 
 setup_kwargs = {
     'name': 'python-homewizard-energy',
-    'version': '1.8.0',
+    'version': '2.0.0',
     'description': 'Asynchronous Python client for the HomeWizard Energy',
     'long_description': '# python-homewizard-energy\n\nAsyncio package to communicate with HomeWizard Energy devices\nThis package is aimed at basic control of the device. Initial setup and configuration is assumed to done with the official HomeWizard Energy app.\n\n## Disclaimer\n\nThis package is not developed, nor supported by HomeWizard.\n\n## Installation\n```bash\npython3 -m pip install python-homewizard-energy\n```\n\n# Usage\nInstantiate the HWEnergy class and access the API.\n\nFor more details on the API see the official API documentation on\nhttps://homewizard-energy-api.readthedocs.io\n\n# Example\nThe example below is available as a runnable script in the repository.\n\n```python\nfrom homewizard_energy import HomeWizardEnergy\n\n# Make contact with a energy device\nasync with HomeWizardEnergy(args.host) as api:\n\n    # Use the data\n    print(await api.device())\n    print(await api.data())\n    print(await api.state())\n\n    await api.state_set(power_on=True)\n```\n',
     'author': 'DCSBL',
     'author_email': 'None',
     'maintainer': 'DCSBL',
     'maintainer_email': 'None',
     'url': 'https://github.com/dcsbl/python-homewizard-energy',
```

### Comparing `python_homewizard_energy-1.8.0/PKG-INFO` & `python_homewizard_energy-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-homewizard-energy
-Version: 1.8.0
+Version: 2.0.0
 Summary: Asynchronous Python client for the HomeWizard Energy
 Home-page: https://github.com/dcsbl/python-homewizard-energy
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

