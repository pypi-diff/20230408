# Comparing `tmp/python_homewizard_energy-2.0.0.tar.gz` & `tmp/python_homewizard_energy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_homewizard_energy-2.0.0.tar", max compression
+gzip compressed data, was "python_homewizard_energy-2.0.1.tar", max compression
```

## Comparing `python_homewizard_energy-2.0.0.tar` & `python_homewizard_energy-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11346 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/LICENSE
--rw-r--r--   0        0        0      936 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/README.md
--rw-r--r--   0        0        0      468 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/__init__.py
--rw-r--r--   0        0        0      244 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/const.py
--rw-r--r--   0        0        0      765 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/errors.py
--rw-r--r--   0        0        0     8412 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/homewizard_energy.py
--rw-r--r--   0        0        0    11246 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/models.py
--rw-r--r--   0        0        0        0 2023-04-08 18:31:38.786255 python_homewizard_energy-2.0.0/homewizard_energy/py.typed
--rw-r--r--   0        0        0     2383 2023-04-08 18:32:26.890309 python_homewizard_energy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.0/setup.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/LICENSE
+-rw-r--r--   0        0        0      936 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/README.md
+-rw-r--r--   0        0        0      468 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/const.py
+-rw-r--r--   0        0        0      765 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/errors.py
+-rw-r--r--   0        0        0     8438 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/homewizard_energy.py
+-rw-r--r--   0        0        0    11246 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/models.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/py.typed
+-rw-r--r--   0        0        0     2383 2023-04-08 19:08:08.635884 python_homewizard_energy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.1/setup.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.1/PKG-INFO
```

### Comparing `python_homewizard_energy-2.0.0/LICENSE` & `python_homewizard_energy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.0/README.md` & `python_homewizard_energy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.0/homewizard_energy/errors.py` & `python_homewizard_energy-2.0.1/homewizard_energy/errors.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.0/homewizard_energy/homewizard_energy.py` & `python_homewizard_energy-2.0.1/homewizard_energy/homewizard_energy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import string
 from collections.abc import Callable, Coroutine
 from http import HTTPStatus
-from typing import Any
+from typing import Any, TypeVar
 
 import async_timeout
 from aiohttp.client import ClientError, ClientResponseError, ClientSession
 from aiohttp.hdrs import METH_DELETE, METH_GET, METH_PUT
 
 from .const import SUPPORTED_API_VERSION
 from .errors import DisabledError, NotFoundError, RequestError, UnsupportedError
 from .models import Data, Decryption, Device, State, System
 
 _LOGGER = logging.getLogger(__name__)
 
+T = TypeVar("T")
+
 
 def optional_method(
-    func: Callable[..., Coroutine[Any, Any, None]]
-) -> Callable[..., Coroutine[Any, Any, None]]:
+    func: Callable[..., Coroutine[Any, Any, T]]
+) -> Callable[..., Coroutine[Any, Any, T]]:
     """Check if method is supported."""
 
-    async def wrapper(self, *args, **kwargs):
+    async def wrapper(self, *args, **kwargs) -> T:
         try:
             return await func(self, *args, **kwargs)
         except NotFoundError as ex:
             raise UnsupportedError(f"{func.__name__} is not supported") from ex
 
     return wrapper
```

### Comparing `python_homewizard_energy-2.0.0/homewizard_energy/models.py` & `python_homewizard_energy-2.0.1/homewizard_energy/models.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.0/pyproject.toml` & `python_homewizard_energy-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-homewizard-energy"
-version = "2.0.0"
+version = "2.0.1"
 description = "Asynchronous Python client for the HomeWizard Energy"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-homewizard-energy"
 repository = "https://github.com/dcsbl/python-homewizard-energy"
```

### Comparing `python_homewizard_energy-2.0.0/setup.py` & `python_homewizard_energy-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0.0', 'awesomeversion>=22.9.0']
 
 setup_kwargs = {
     'name': 'python-homewizard-energy',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Asynchronous Python client for the HomeWizard Energy',
     'long_description': '# python-homewizard-energy\n\nAsyncio package to communicate with HomeWizard Energy devices\nThis package is aimed at basic control of the device. Initial setup and configuration is assumed to done with the official HomeWizard Energy app.\n\n## Disclaimer\n\nThis package is not developed, nor supported by HomeWizard.\n\n## Installation\n```bash\npython3 -m pip install python-homewizard-energy\n```\n\n# Usage\nInstantiate the HWEnergy class and access the API.\n\nFor more details on the API see the official API documentation on\nhttps://homewizard-energy-api.readthedocs.io\n\n# Example\nThe example below is available as a runnable script in the repository.\n\n```python\nfrom homewizard_energy import HomeWizardEnergy\n\n# Make contact with a energy device\nasync with HomeWizardEnergy(args.host) as api:\n\n    # Use the data\n    print(await api.device())\n    print(await api.data())\n    print(await api.state())\n\n    await api.state_set(power_on=True)\n```\n',
     'author': 'DCSBL',
     'author_email': 'None',
     'maintainer': 'DCSBL',
     'maintainer_email': 'None',
     'url': 'https://github.com/dcsbl/python-homewizard-energy',
```

### Comparing `python_homewizard_energy-2.0.0/PKG-INFO` & `python_homewizard_energy-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-homewizard-energy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Asynchronous Python client for the HomeWizard Energy
 Home-page: https://github.com/dcsbl/python-homewizard-energy
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

