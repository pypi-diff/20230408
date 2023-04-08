# Comparing `tmp/test_rest_api-0.0.0.0.24.tar.gz` & `tmp/test_rest_api-0.0.0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.24.tar", last modified: Fri Apr  7 17:21:44 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.25.tar", last modified: Sat Apr  8 17:09:37 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.24.tar` & `test_rest_api-0.0.0.0.25.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.860928 test_rest_api-0.0.0.0.24/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    19654 2023-04-07 17:21:44.860291 test_rest_api-0.0.0.0.24/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    17931 2023-04-07 07:45:37.000000 test_rest_api-0.0.0.0.24/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-07 17:21:44.861106 test_rest_api-0.0.0.0.24/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-07 17:21:11.000000 test_rest_api-0.0.0.0.24/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.835726 test_rest_api-0.0.0.0.24/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.840625 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2568 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.842678 test_rest_api-0.0.0.0.24/test_rest_api/logger/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      848 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.845383 test_rest_api-0.0.0.0.24/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 16:39:07.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.849191 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     5987 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.853036 test_rest_api-0.0.0.0.24/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-07 13:46:31.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 14:33:51.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.859166 test_rest_api-0.0.0.0.24/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.838767 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    19654 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.081971 test_rest_api-0.0.0.0.25/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    63924 2023-04-08 17:09:37.081467 test_rest_api-0.0.0.0.25/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62201 2023-04-08 17:01:58.000000 test_rest_api-0.0.0.0.25/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-08 17:09:37.082122 test_rest_api-0.0.0.0.25/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-08 17:07:04.000000 test_rest_api-0.0.0.0.25/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.058951 test_rest_api-0.0.0.0.25/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.063709 test_rest_api-0.0.0.0.25/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-08 13:00:44.000000 test_rest_api-0.0.0.0.25/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.065729 test_rest_api-0.0.0.0.25/test_rest_api/logger/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/logger/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/logger/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      848 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/logger/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.068389 test_rest_api-0.0.0.0.25/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.25/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.25/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.071913 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-08 13:55:22.000000 test_rest_api-0.0.0.0.25/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.075482 test_rest_api-0.0.0.0.25/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.25/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-08 13:49:13.000000 test_rest_api-0.0.0.0.25/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.25/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.25/test_rest_api/testing/runner.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.080455 test_rest_api-0.0.0.0.25/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/colors.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.25/test_rest_api/utils/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:09:37.061844 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    63924 2023-04-08 17:09:36.000000 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-08 17:09:37.000000 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-08 17:09:36.000000 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-08 17:09:36.000000 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-08 17:09:36.000000 test_rest_api-0.0.0.0.25/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.24/LICENSE` & `test_rest_api-0.0.0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/setup.py` & `test_rest_api-0.0.0.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.24',
+      version='0.0.0.0.25',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
```

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.25/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/global_variables/exception.py` & `test_rest_api-0.0.0.0.25/test_rest_api/global_variables/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.25/test_rest_api/global_variables/global_variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
     def set(cls, name, value, is_constant: bool = False):
         """
         Set the global variable value
         """
         # Check if name is of type string
         if not isinstance(name, str):
             raise Exception('Invalid data type for name. Please provide a valid string')
+        # Check if name not empty
+        if name.strip() == '':
+            raise Exception('Empty value for name. Please provide a valid string')
         # Check if is_constant is of type bool
         if not isinstance(is_constant, bool):
             raise Exception('Invalid data type for is_constant. Please provide a valid boolean')
         try:
             variable_obj = cls._get_variable_obj(name=name)
         except Exception as exc:
             variable_obj = None
```

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/logger/exception.py` & `test_rest_api-0.0.0.0.25/test_rest_api/logger/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/logger/logger.py` & `test_rest_api-0.0.0.0.25/test_rest_api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.25/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.25/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/rest_api/exception.py` & `test_rest_api-0.0.0.0.25/test_rest_api/rest_api/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.25/test_rest_api/rest_api/rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 """
 
     async def send(self, method: str):
         """
         Send the rest api by providing the request method
         """
         try:
+            # Check if method is of type string
+            if not isinstance(method, str):
+                raise Exception('Invalid data type for method. Please provide a valid string')
             # Convert to lowercase
             method = method.lower()
             # Check if the method is valid
             if method not in asdict(self.METHODS).values():
                 raise Exception(ErrorMsg.INVALID_METHOD)
             # Send the request
             async with getattr(self._session, method)(url=self.url,
```

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.25/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.25/test_rest_api/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/testing/exception.py` & `test_rest_api-0.0.0.0.25/test_rest_api/testing/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.25/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.25/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/utils/colors.py` & `test_rest_api-0.0.0.0.25/test_rest_api/utils/colors.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.25/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.25/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.25/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.24/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.25/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

