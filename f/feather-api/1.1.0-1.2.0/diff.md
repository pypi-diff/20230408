# Comparing `tmp/feather-api-1.1.0.tar.gz` & `tmp/feather-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feather-api-1.1.0.tar", last modified: Mon Mar 27 21:44:25 2023, max compression
+gzip compressed data, was "feather-api-1.2.0.tar", last modified: Fri Apr  7 23:22:27 2023, max compression
```

## Comparing `feather-api-1.1.0.tar` & `feather-api-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:44:25.957461 feather-api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-27 21:44:25.957461 feather-api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-27 21:44:01.000000 feather-api-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:44:25.957461 feather-api-1.1.0/feather_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 21:44:25.000000 feather-api-1.1.0/feather_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:44:25.957461 feather-api-1.1.0/featherapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-03-27 21:44:01.000000 feather-api-1.1.0/featherapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:44:25.957461 feather-api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-27 21:44:01.000000 feather-api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:22:27.323263 feather-api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-07 23:22:27.323263 feather-api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-07 23:22:08.000000 feather-api-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:22:27.323263 feather-api-1.2.0/feather_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 23:22:27.000000 feather-api-1.2.0/feather_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:22:27.323263 feather-api-1.2.0/featherapi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-04-07 23:22:08.000000 feather-api-1.2.0/featherapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:22:27.323263 feather-api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 23:22:08.000000 feather-api-1.2.0/setup.py
```

### Comparing `feather-api-1.1.0/PKG-INFO` & `feather-api-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feather-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python wrapper for Feather's API
 Home-page: http://github.com/Feather-Official/featherdbtools
 Author: Feather Technology Inc.
 Author-email: support@try-feather.com
 Description-Content-Type: text/markdown
 
 # Feather API Python Client
```

### Comparing `feather-api-1.1.0/README.md` & `feather-api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `feather-api-1.1.0/feather_api.egg-info/PKG-INFO` & `feather-api-1.2.0/feather_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feather-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python wrapper for Feather's API
 Home-page: http://github.com/Feather-Official/featherdbtools
 Author: Feather Technology Inc.
 Author-email: support@try-feather.com
 Description-Content-Type: text/markdown
 
 # Feather API Python Client
```

### Comparing `feather-api-1.1.0/featherapi/__init__.py` & `feather-api-1.2.0/featherapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -225,18 +225,18 @@
         """
 
         path = f'/equity/{symbol}/stock-price-historical'
 
         query_params = {}
         if start or end:
             
-            if start[5] != '-' or start[8] != '-':
+            if start[4] != '-' or start[8] != '-':
                 raise ValueError('Start date must be in the format YYYY-MM-DD')
             
-            if end[5] != '-' or end[8] != '-':
+            if end[4] != '-' or end[8] != '-':
                 raise ValueError('End date must be in the format YYYY-MM-DD')
             
             if start and end:
                 if int(start.replace('-', '')) > int(end.replace('-', '')):
                     raise ValueError('Start date must be before end date.')
             
             query_params = {
@@ -256,34 +256,58 @@
         path = f'/equity/{symbol}/institutional-holders'
         response = self.__get_url(path)
         data = pd.DataFrame(response['data'])
         return data
     
     def get_insider_trades(self, symbol):
         """
-        Get avaialble insider trades for a given equity symbol.
+        Get available insider trades for a given equity symbol.
         """
 
         path = f'/equity/{symbol}/insider-trades'
         response = self.__get_url(path)
         data = pd.DataFrame(response['data'])
         return data
     
     def get_earnings(self, symbol):
         """
-        Get avaialble earnings history for a given equity symbol.
+        Get available earnings history for a given equity symbol.
         Parameters
         - `symbol`: The equity symbol to get the earnings history for.
         """
 
         path = f'/equity/{symbol}/earnings'
         response = self.__get_url(path)
         data = pd.DataFrame(response['data'])
         return data
 
+    def get_analyst_ratings(self, symbol):
+        """
+        Get available analyst ratings for a given equity symbol.
+        Parameters
+        - `symbol`: The equity symbol to get the analyst sentiments for.
+        """
+
+        path = f'/equity/{symbol}/analyst-ratings'
+        response = self.__get_url(path)
+        data = pd.DataFrame(response['data'])
+        return data
+
+    def get_analyst_consensus(self, symbol):
+        """
+        Get available analyst consensus for a given equity symbol.
+        Parameters
+        - `symbol`: The equity symbol to get the analyst sentiments for.
+        """
+
+        path = f'/equity/{symbol}/analyst-consensus'
+        response = self.__get_url(path)
+        data = pd.DataFrame(response['data'])
+        return data
+
     def get_articles(self, keyword=None, limit=None):
         """
         Get the latest available articles.
         Parameters
         - (Optional) `keyword`: A keyword to filter articles by.
         - (Optional) `limit`: The number of articles to return. Default is maximum number of available articles.
         """
```

### Comparing `feather-api-1.1.0/setup.py` & `feather-api-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(name='feather-api',
-      version='1.1.0',
+      version='1.2.0',
       description='Python wrapper for Feather\'s API',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/Feather-Official/featherdbtools',
       author='Feather Technology Inc.',
       author_email='support@try-feather.com',
       packages=['featherapi'],
```

