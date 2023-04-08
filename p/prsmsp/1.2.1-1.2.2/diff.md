# Comparing `tmp/prsmsp-1.2.1.tar.gz` & `tmp/prsmsp-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.2.1.tar", last modified: Wed Apr  5 16:58:14 2023, max compression
+gzip compressed data, was "prsmsp-1.2.2.tar", last modified: Sat Apr  8 19:20:55 2023, max compression
```

## Comparing `prsmsp-1.2.1.tar` & `prsmsp-1.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-05 16:58:14.187066 prsmsp-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-05 16:58:02.000000 prsmsp-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.183066 prsmsp-1.2.1/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/prsmsp/abctracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/abctracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/abctracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/prsmsp/exeptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/exeptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/exeptions/abctracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/exeptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/exeptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-05 16:58:02.000000 prsmsp-1.2.1/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.183066 prsmsp-1.2.1/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 16:58:14.000000 prsmsp-1.2.1/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-05 16:58:14.187066 prsmsp-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-05 16:58:02.000000 prsmsp-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:14.187066 prsmsp-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:58:02.000000 prsmsp-1.2.1/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 19:20:55.817584 prsmsp-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-08 19:20:46.000000 prsmsp-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-08 19:20:55.817584 prsmsp-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 19:20:46.000000 prsmsp-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/tests/test_app.py
```

### Comparing `prsmsp-1.2.1/PKG-INFO` & `prsmsp-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.2.1
+Version: 1.2.2
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

### Comparing `prsmsp-1.2.1/README.md` & `prsmsp-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.1/prsmsp/factories/auth_factory.py` & `prsmsp-1.2.2/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.1/prsmsp/models/response.py` & `prsmsp-1.2.2/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.1/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.2.2/prsmsp/panels/ghasedaksms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class GhasedakSms(ABCSmsPanel):
     def __init__(self, api_key: str) -> None:
         """Take the auth info
```

### Comparing `prsmsp-1.2.1/prsmsp/panels/kavenegar.py` & `prsmsp-1.2.2/prsmsp/panels/kavenegar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class Kavenegar(ABCSmsPanel):
     def __init__(self, api_key: str) -> None:
         """Take the auth info
```

### Comparing `prsmsp-1.2.1/prsmsp/panels/mediana.py` & `prsmsp-1.2.2/prsmsp/panels/mediana.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class Mediana(ABCSmsPanel):
     # this is the client version for mediana package
     # this is not relevant to our package version,
```

### Comparing `prsmsp-1.2.1/prsmsp/panels/melipayamak.py` & `prsmsp-1.2.2/prsmsp/panels/melipayamak.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class MeliPayamak(ABCSmsPanel):
     def __init__(self, username, password):
         """Take the auth info
```

### Comparing `prsmsp-1.2.1/prsmsp/panels/smsdotir.py` & `prsmsp-1.2.2/prsmsp/panels/smsdotir.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class SmsDotIr(ABCSmsPanel):
     def __init__(self, api_key: str):
         """Take the auth info
```

### Comparing `prsmsp-1.2.1/prsmsp/panels/webonesms.py` & `prsmsp-1.2.2/prsmsp/panels/webonesms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import requests
 
-from prsmsp.abctracts.abcpanel import ABCSmsPanel
+from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class WebOneSms(ABCSmsPanel):
     def __init__(self, username, password):
         """Take the auth info
```

### Comparing `prsmsp-1.2.1/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.2.2/prsmsp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.2.1
+Version: 1.2.2
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

### Comparing `prsmsp-1.2.1/setup.cfg` & `prsmsp-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.2.1
+version = 1.2.2
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

