# Comparing `tmp/flask-mulang-1.0.0.tar.gz` & `tmp/flask-mulang-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-mulang-1.0.0.tar", last modified: Fri Mar 10 18:14:36 2023, max compression
+gzip compressed data, was "flask-mulang-1.1.0.tar", last modified: Fri Apr  7 23:08:41 2023, max compression
```

## Comparing `flask-mulang-1.0.0.tar` & `flask-mulang-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-03-10 18:14:36.469187 flask-mulang-1.0.0/
--rw-r--r--   0 human     (1000) human     (1000)      512 2023-03-10 18:14:36.469187 flask-mulang-1.0.0/PKG-INFO
--rw-r--r--   0 human     (1000) human     (1000)      418 2023-03-10 18:09:29.000000 flask-mulang-1.0.0/README.md
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-03-10 18:14:36.465854 flask-mulang-1.0.0/flask_mulang/
--rw-r--r--   0 human     (1000) human     (1000)     5355 2023-02-15 19:32:31.000000 flask-mulang-1.0.0/flask_mulang/__init__.py
--rw-r--r--   0 human     (1000) human     (1000)     9286 2023-03-10 17:51:07.000000 flask-mulang-1.0.0/flask_mulang/flask_multilananger.py
--rw-r--r--   0 human     (1000) human     (1000)     5308 2022-12-06 04:15:06.000000 flask-mulang-1.0.0/flask_mulang/generator.py
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-03-10 18:14:36.469187 flask-mulang-1.0.0/flask_mulang.egg-info/
--rw-r--r--   0 human     (1000) human     (1000)      512 2023-03-10 18:14:36.000000 flask-mulang-1.0.0/flask_mulang.egg-info/PKG-INFO
--rw-r--r--   0 human     (1000) human     (1000)      284 2023-03-10 18:14:36.000000 flask-mulang-1.0.0/flask_mulang.egg-info/SOURCES.txt
--rw-r--r--   0 human     (1000) human     (1000)        1 2023-03-10 18:14:36.000000 flask-mulang-1.0.0/flask_mulang.egg-info/dependency_links.txt
--rw-r--r--   0 human     (1000) human     (1000)       26 2023-03-10 18:14:36.000000 flask-mulang-1.0.0/flask_mulang.egg-info/requires.txt
--rw-r--r--   0 human     (1000) human     (1000)       13 2023-03-10 18:14:36.000000 flask-mulang-1.0.0/flask_mulang.egg-info/top_level.txt
--rw-r--r--   0 human     (1000) human     (1000)       38 2023-03-10 18:14:36.469187 flask-mulang-1.0.0/setup.cfg
--rw-r--r--   0 human     (1000) human     (1000)      826 2023-03-10 18:14:19.000000 flask-mulang-1.0.0/setup.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-04-07 23:08:41.804593 flask-mulang-1.1.0/
+-rw-r--r--   0 human     (1000) human     (1000)      516 2023-04-07 23:08:41.804593 flask-mulang-1.1.0/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)      418 2023-03-10 18:09:29.000000 flask-mulang-1.1.0/README.md
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-04-07 23:08:41.804593 flask-mulang-1.1.0/flask_mulang/
+-rw-r--r--   0 human     (1000) human     (1000)     5427 2023-04-07 23:01:33.000000 flask-mulang-1.1.0/flask_mulang/__init__.py
+-rw-r--r--   0 human     (1000) human     (1000)     9287 2023-03-10 18:16:53.000000 flask-mulang-1.1.0/flask_mulang/flask_multilananger.py
+-rw-r--r--   0 human     (1000) human     (1000)     5308 2022-12-06 04:15:06.000000 flask-mulang-1.1.0/flask_mulang/generator.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-04-07 23:08:41.804593 flask-mulang-1.1.0/flask_mulang.egg-info/
+-rw-r--r--   0 human     (1000) human     (1000)      516 2023-04-07 23:08:41.000000 flask-mulang-1.1.0/flask_mulang.egg-info/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)      284 2023-04-07 23:08:41.000000 flask-mulang-1.1.0/flask_mulang.egg-info/SOURCES.txt
+-rw-r--r--   0 human     (1000) human     (1000)        1 2023-04-07 23:08:41.000000 flask-mulang-1.1.0/flask_mulang.egg-info/dependency_links.txt
+-rw-r--r--   0 human     (1000) human     (1000)       26 2023-04-07 23:08:41.000000 flask-mulang-1.1.0/flask_mulang.egg-info/requires.txt
+-rw-r--r--   0 human     (1000) human     (1000)       13 2023-04-07 23:08:41.000000 flask-mulang-1.1.0/flask_mulang.egg-info/top_level.txt
+-rw-r--r--   0 human     (1000) human     (1000)       38 2023-04-07 23:08:41.804593 flask-mulang-1.1.0/setup.cfg
+-rw-r--r--   0 human     (1000) human     (1000)      830 2023-04-07 23:08:35.000000 flask-mulang-1.1.0/setup.py
```

### Comparing `flask-mulang-1.0.0/PKG-INFO` & `flask-mulang-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flask-mulang
-Version: 1.0.0
-Summary: Flask Extension to for multi languages.
+Version: 1.1.0
+Summary: Flask Extension for multi language support.
 Author: Mohamed El-Hasnaouy
 Author-email: <elhasnaouymed@proton.me>
 Keywords: python,flask,language,babel,full stack,development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `flask-mulang-1.0.0/flask_mulang/__init__.py` & `flask-mulang-1.1.0/flask_mulang/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         :param app: valid Flask app
         :param languages_folder: the source directory of lang files
         :param def_lang: default lang
         :param ext: extension of lang files
         :param auto_markdown: to auto markdown values, you can choose for each value later
         :return: None
         """
+        self.DEFAULT_LANG = def_lang if def_lang else self.DEFAULT_LANG
         # > check if already initialized before doing it
         if self._initialized:
             raise Exception('Cannot have Mulang() instance initialized more than once.')
         # > check if the $app argument is valid Flask
         if isinstance(app, _Flask):
             # > get the languages_folder to be within the app root path
             root_lang_source_dir = os.path.join(app.root_path, languages_folder)
```

### Comparing `flask-mulang-1.0.0/flask_mulang/flask_multilananger.py` & `flask-mulang-1.1.0/flask_mulang/flask_multilananger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import os
 from datetime import datetime, tzinfo
 from configparser import ConfigParser
 from markupsafe import escape
 from markdown import markdown
```

### Comparing `flask-mulang-1.0.0/flask_mulang/generator.py` & `flask-mulang-1.1.0/flask_mulang/generator.py`

 * *Files identical despite different names*

### Comparing `flask-mulang-1.0.0/flask_mulang.egg-info/PKG-INFO` & `flask-mulang-1.1.0/flask_mulang.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flask-mulang
-Version: 1.0.0
-Summary: Flask Extension to for multi languages.
+Version: 1.1.0
+Summary: Flask Extension for multi language support.
 Author: Mohamed El-Hasnaouy
 Author-email: <elhasnaouymed@proton.me>
 Keywords: python,flask,language,babel,full stack,development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `flask-mulang-1.0.0/setup.py` & `flask-mulang-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '1.0.0'
-DESCRIPTION = 'Flask Extension to for multi languages.'
+VERSION = '1.1.0'
+DESCRIPTION = 'Flask Extension for multi language support.'
 
 # Setting up
 setup(
     name="flask-mulang",
     version=VERSION,
     author="Mohamed El-Hasnaouy",
     author_email="<elhasnaouymed@proton.me>",
```

