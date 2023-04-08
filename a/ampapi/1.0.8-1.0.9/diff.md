# Comparing `tmp/ampapi-1.0.8.tar.gz` & `tmp/ampapi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.0.8.tar", last modified: Wed Mar 15 00:27:03 2023, max compression
+gzip compressed data, was "ampapi-1.0.9.tar", last modified: Sat Apr  8 19:39:26 2023, max compression
```

## Comparing `ampapi-1.0.8.tar` & `ampapi-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-03-15 00:27:03.797469 ampapi-1.0.8/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1160 2022-12-17 05:17:37.000000 ampapi-1.0.8/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-03-15 00:27:03.797469 ampapi-1.0.8/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4206 2023-03-14 23:17:08.000000 ampapi-1.0.8/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-03-15 00:27:03.797469 ampapi-1.0.8/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2022-12-17 05:17:37.000000 ampapi-1.0.8/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    44380 2023-03-15 00:24:30.000000 ampapi-1.0.8/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-03-15 00:27:03.797469 ampapi-1.0.8/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-03-15 00:27:03.000000 ampapi-1.0.8/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-03-15 00:27:03.000000 ampapi-1.0.8/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-03-15 00:27:03.000000 ampapi-1.0.8/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-03-15 00:27:03.000000 ampapi-1.0.8/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2022-12-23 22:22:45.000000 ampapi-1.0.8/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-03-15 00:27:03.797469 ampapi-1.0.8/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1160 2022-12-17 05:17:37.000000 ampapi-1.0.9/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-04-08 19:39:26.373114 ampapi-1.0.9/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4206 2023-03-14 23:17:08.000000 ampapi-1.0.9/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2022-12-17 05:17:37.000000 ampapi-1.0.9/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    44610 2023-04-08 19:34:18.000000 ampapi-1.0.9/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2022-12-23 22:22:45.000000 ampapi-1.0.9/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-08 19:39:26.373114 ampapi-1.0.9/setup.cfg
```

### Comparing `ampapi-1.0.8/LICENCE` & `ampapi-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ampapi-1.0.8/PKG-INFO` & `ampapi-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.0.8/README.md` & `ampapi-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ampapi-1.0.8/ampapi/ampapi.py` & `ampapi-1.0.9/ampapi/ampapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,15 +809,19 @@
         if self.baseUri[-1] != "/": self.baseUri = self.baseUri + "/"
         self.username = username
         self.password = password
         self.rememberMeToken = rememberMeToken
         self.sessionId = sessionId
 
     def Login(self):
-        loginResult = self.Core.Login(self.username, self.password, self.rememberMeToken, True)
+        # TODO: Find where handler the rememberMeToken breaks down
+        # rememberMe: bool = True if self.rememberMeToken != "" else False
+        # loginResult = self.Core.Login(self.username, self.password, self.rememberMeToken, rememberMe)
+
+        loginResult = self.Core.Login(self.username, self.password, "", False)
         if "success" in loginResult.keys() and loginResult["success"]:
             self.rememberMeToken = loginResult["rememberMeToken"]
             self.sessionId = loginResult["sessionID"]
         return loginResult
 
     def initHandler(self):
         try:
```

### Comparing `ampapi-1.0.8/ampapi.egg-info/PKG-INFO` & `ampapi-1.0.9/ampapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.0.8/setup.cfg` & `ampapi-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.0.8
+version = 1.0.9
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```

