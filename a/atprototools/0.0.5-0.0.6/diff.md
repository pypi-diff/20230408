# Comparing `tmp/atprototools-0.0.5.tar.gz` & `tmp/atprototools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.5.tar", last modified: Sat Apr  8 20:43:40 2023, max compression
+gzip compressed data, was "atprototools-0.0.6.tar", last modified: Sat Apr  8 21:35:05 2023, max compression
```

## Comparing `atprototools-0.0.5.tar` & `atprototools-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:43:40.478540 atprototools-0.0.5/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.5/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/atprototools/
--rw-r--r--   0 user      (1000) user      (1000)     1274 2023-04-08 18:50:48.000000 atprototools-0.0.5/atprototools/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 20:43:40.478540 atprototools-0.0.5/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-08 20:43:40.000000 atprototools-0.0.5/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 20:43:40.478540 atprototools-0.0.5/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 20:43:23.000000 atprototools-0.0.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 21:35:05.348036 atprototools-0.0.6/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-08 20:12:15.000000 atprototools-0.0.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/atprototools/
+-rw-r--r--   0 user      (1000) user      (1000)     1885 2023-04-08 21:28:47.000000 atprototools-0.0.6/atprototools/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-08 21:35:05.348036 atprototools-0.0.6/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-08 21:35:05.000000 atprototools-0.0.6/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-08 21:35:05.348036 atprototools-0.0.6/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-08 21:34:58.000000 atprototools-0.0.6/setup.py
```

### Comparing `atprototools-0.0.5/PKG-INFO` & `atprototools-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.5
+Version: 0.0.6
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.5/atprototools/__init__.py` & `atprototools-0.0.6/atprototools/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import requests
 import datetime
 
 ATP_HOST = "https://bsky.social"
 ATP_AUTH_TOKEN = ""
-
-USERNAME = "YOURUSERNAME.bsky.social"
-PASSWORD = "CHANGEME"
 DID = "" # leave blank
 
 
-def login():
-    data = {"identifier": USERNAME, "password": PASSWORD}
+def login(username, password):
+    data = {"identifier": username, "password": password}
     resp = requests.post(
         ATP_HOST + "/xrpc/com.atproto.server.createSession",
         json=data
     )
 
     global ATP_AUTH_TOKEN
     ATP_AUTH_TOKEN = resp.json().get('accessJwt')
@@ -23,16 +20,17 @@
 
     global DID
     DID = resp.json().get("did")
 
     return resp
 
 
-def post(postcontent):
-    timestamp = datetime.datetime.now(datetime.timezone.utc)
+def post_skoot(postcontent, timestamp=None):
+    if not timestamp:
+        timestamp = datetime.datetime.now(datetime.timezone.utc)
     timestamp = timestamp.isoformat().replace('+00:00', 'Z')
 
     headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
 
     data = {
         "collection": "app.bsky.feed.post",
         "$type": "app.bsky.feed.post",
@@ -48,10 +46,28 @@
         ATP_HOST + "/xrpc/com.atproto.repo.createRecord",
         json=data,
         headers=headers
     )
 
     return resp
 
+def delete_skoot(did,rkey):
+    data = {"collection":"app.bsky.feed.post","repo":"did:plc:{}".format(did),"rkey":"{}".format(rkey)}
+    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
+    resp = requests.post(
+        ATP_HOST + "/xrpc/com.atproto.repo.deleteRecord",
+        json = data,
+        headers=headers
+    )
+    return resp
+
+def get_latest_skoot(accountname):
+    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
+    resp = requests.get(
+        ATP_HOST + "/xrpc/app.bsky.feed.getAuthorFeed?actor={}&limit=1".format(accountname),
+        headers = headers
+    )
+    return resp
+
 
 # resp = login()
 # post("test post")
```

### Comparing `atprototools-0.0.5/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.6/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.5
+Version: 0.0.6
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.5/setup.py` & `atprototools-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.5',
+    version='0.0.6',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```

