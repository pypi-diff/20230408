# Comparing `tmp/epub2sphinx-0.0.4.tar.gz` & `tmp/epub2sphinx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epub2sphinx-0.0.4.tar", last modified: Mon Apr  3 07:23:32 2023, max compression
+gzip compressed data, was "epub2sphinx-0.0.5.tar", last modified: Sat Apr  8 17:49:03 2023, max compression
```

## Comparing `epub2sphinx-0.0.4.tar` & `epub2sphinx-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     1804 2022-11-06 04:38:38.000000 epub2sphinx-0.0.4/.gitignore
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      148 2021-11-13 07:20:07.000000 epub2sphinx-0.0.4/AUTHORS
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     1063 2021-11-13 04:08:19.000000 epub2sphinx-0.0.4/LICENSE
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       16 2021-11-13 06:20:57.000000 epub2sphinx-0.0.4/MANIFEST.in
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4715 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/PKG-INFO
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4125 2023-04-03 07:18:54.000000 epub2sphinx-0.0.4/README.md
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4076 2022-11-06 05:34:26.000000 epub2sphinx-0.0.4/cli.py
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/epub2sphinx/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       83 2021-11-25 05:05:17.000000 epub2sphinx-0.0.4/epub2sphinx/__init__.py
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     3373 2021-12-17 18:27:49.000000 epub2sphinx-0.0.4/epub2sphinx/book.py
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     2811 2022-03-13 07:49:04.000000 epub2sphinx-0.0.4/epub2sphinx/chapter.py
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      918 2021-12-02 08:54:44.000000 epub2sphinx-0.0.4/epub2sphinx/constants.py
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     7085 2022-11-06 05:36:40.000000 epub2sphinx-0.0.4/epub2sphinx/convert.py
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/epub2sphinx/templates/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     2030 2021-12-17 19:04:47.000000 epub2sphinx-0.0.4/epub2sphinx/templates/conf.py
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      346 2021-11-25 05:05:17.000000 epub2sphinx-0.0.4/epub2sphinx/templates/index.rst
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/epub2sphinx/templates/makefiles/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      638 2021-11-25 05:05:17.000000 epub2sphinx-0.0.4/epub2sphinx/templates/makefiles/Makefile
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      804 2021-11-25 05:05:17.000000 epub2sphinx-0.0.4/epub2sphinx/templates/makefiles/make.bat
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/epub2sphinx/tests/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      245 2021-11-13 14:01:55.000000 epub2sphinx-0.0.4/epub2sphinx/tests/unit_test.py
-drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/epub2sphinx.egg-info/
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4715 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/PKG-INFO
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)      583 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)        1 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       44 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/entry_points.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       87 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/requires.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       16 2023-04-03 07:23:32.000000 epub2sphinx-0.0.4/epub2sphinx.egg-info/top_level.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       88 2022-03-13 08:55:28.000000 epub2sphinx-0.0.4/requirements.txt
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)       38 2023-04-03 07:23:32.985146 epub2sphinx-0.0.4/setup.cfg
--rw-r--r--   0 nihaal    (1000) nihaal    (1000)     1142 2023-04-03 07:09:50.000000 epub2sphinx-0.0.4/setup.py
+drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-08 17:49:03.866873 epub2sphinx-0.0.5/
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      148 2021-11-13 07:20:07.000000 epub2sphinx-0.0.5/AUTHORS
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     1063 2021-11-13 04:08:19.000000 epub2sphinx-0.0.5/LICENSE
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       16 2023-04-08 17:46:49.000000 epub2sphinx-0.0.5/MANIFEST.in
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4715 2023-04-08 17:49:03.866873 epub2sphinx-0.0.5/PKG-INFO
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4125 2023-04-03 07:18:54.000000 epub2sphinx-0.0.5/README.md
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4076 2022-11-06 05:34:26.000000 epub2sphinx-0.0.5/cli.py
+drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-08 17:49:03.863540 epub2sphinx-0.0.5/epub2sphinx/
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       83 2021-11-25 05:05:17.000000 epub2sphinx-0.0.5/epub2sphinx/__init__.py
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     3373 2021-12-17 18:27:49.000000 epub2sphinx-0.0.5/epub2sphinx/book.py
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     2811 2022-03-13 07:49:04.000000 epub2sphinx-0.0.5/epub2sphinx/chapter.py
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      918 2021-12-02 08:54:44.000000 epub2sphinx-0.0.5/epub2sphinx/constants.py
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     7085 2023-04-08 17:25:57.000000 epub2sphinx-0.0.5/epub2sphinx/convert.py
+drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-08 17:49:03.863540 epub2sphinx-0.0.5/epub2sphinx/templates/
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      638 2021-11-25 05:05:17.000000 epub2sphinx-0.0.5/epub2sphinx/templates/Makefile
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     2030 2021-12-17 19:04:47.000000 epub2sphinx-0.0.5/epub2sphinx/templates/conf.py
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      346 2021-11-25 05:05:17.000000 epub2sphinx-0.0.5/epub2sphinx/templates/index.rst
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      804 2021-11-25 05:05:17.000000 epub2sphinx-0.0.5/epub2sphinx/templates/make.bat
+drwxr-xr-x   0 nihaal    (1000) nihaal    (1000)        0 2023-04-08 17:49:03.863540 epub2sphinx-0.0.5/epub2sphinx.egg-info/
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     4715 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)      504 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)        1 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       44 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/entry_points.txt
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       87 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/requires.txt
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       16 2023-04-08 17:49:03.000000 epub2sphinx-0.0.5/epub2sphinx.egg-info/top_level.txt
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)       38 2023-04-08 17:49:03.866873 epub2sphinx-0.0.5/setup.cfg
+-rw-r--r--   0 nihaal    (1000) nihaal    (1000)     1142 2023-04-08 17:48:28.000000 epub2sphinx-0.0.5/setup.py
```

### Comparing `epub2sphinx-0.0.4/LICENSE` & `epub2sphinx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/PKG-INFO` & `epub2sphinx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub2sphinx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to convert epub to ReST for Sphinx
 Home-page: https://github.com/nifey/epub2sphinx
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nifey/epub2sphinx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epub2sphinx-0.0.4/README.md` & `epub2sphinx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/cli.py` & `epub2sphinx-0.0.5/cli.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/book.py` & `epub2sphinx-0.0.5/epub2sphinx/book.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/chapter.py` & `epub2sphinx-0.0.5/epub2sphinx/chapter.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/constants.py` & `epub2sphinx-0.0.5/epub2sphinx/constants.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/convert.py` & `epub2sphinx-0.0.5/epub2sphinx/convert.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/templates/conf.py` & `epub2sphinx-0.0.5/epub2sphinx/templates/conf.py`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/templates/makefiles/Makefile` & `epub2sphinx-0.0.5/epub2sphinx/templates/Makefile`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx/templates/makefiles/make.bat` & `epub2sphinx-0.0.5/epub2sphinx/templates/make.bat`

 * *Files identical despite different names*

### Comparing `epub2sphinx-0.0.4/epub2sphinx.egg-info/PKG-INFO` & `epub2sphinx-0.0.5/epub2sphinx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub2sphinx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to convert epub to ReST for Sphinx
 Home-page: https://github.com/nifey/epub2sphinx
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nifey/epub2sphinx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epub2sphinx-0.0.4/setup.py` & `epub2sphinx-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name = 'epub2sphinx',
-    version = '0.0.4',
+    version = '0.0.5',
     license = 'MIT',
     description = 'Tool to convert epub to ReST for Sphinx',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/nifey/epub2sphinx',
     project_urls={
         "Bug Tracker": "https://github.com/nifey/epub2sphinx/issues",
```

