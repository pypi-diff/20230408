# Comparing `tmp/dearwatson-0.5.8.tar.gz` & `tmp/dearwatson-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.5.8.tar", last modified: Mon Mar 27 20:48:09 2023, max compression
+gzip compressed data, was "dearwatson-0.5.9.tar", last modified: Tue Mar 28 09:34:36 2023, max compression
```

## Comparing `dearwatson-0.5.8.tar` & `dearwatson-0.5.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.991239 dearwatson-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-27 20:47:53.000000 dearwatson-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-27 20:47:53.000000 dearwatson-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-27 20:48:09.991239 dearwatson-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-27 20:47:53.000000 dearwatson-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.987239 dearwatson-0.5.8/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-27 20:48:09.000000 dearwatson-0.5.8/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-27 20:48:09.000000 dearwatson-0.5.8/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:48:09.000000 dearwatson-0.5.8/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-27 20:48:09.000000 dearwatson-0.5.8/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 20:48:09.000000 dearwatson-0.5.8/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:48:09.991239 dearwatson-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-27 20:47:54.000000 dearwatson-0.5.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-27 20:47:54.000000 dearwatson-0.5.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.987239 dearwatson-0.5.8/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.987239 dearwatson-0.5.8/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.983239 dearwatson-0.5.8/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.987239 dearwatson-0.5.8/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.987239 dearwatson-0.5.8/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-03-27 20:47:54.000000 dearwatson-0.5.8/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:48:09.991239 dearwatson-0.5.8/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:47:56.000000 dearwatson-0.5.8/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-27 20:47:56.000000 dearwatson-0.5.8/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-03-27 20:47:56.000000 dearwatson-0.5.8/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   109758 2023-03-27 20:47:55.000000 dearwatson-0.5.8/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.356158 dearwatson-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 09:34:17.000000 dearwatson-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 09:34:17.000000 dearwatson-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-28 09:34:36.356158 dearwatson-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 09:34:17.000000 dearwatson-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:34:36.356158 dearwatson-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-28 09:34:19.000000 dearwatson-0.5.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-28 09:34:19.000000 dearwatson-0.5.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.348158 dearwatson-0.5.9/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.356158 dearwatson-0.5.9/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109758 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/watson.py
```

### Comparing `dearwatson-0.5.8/LICENSE` & `dearwatson-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/PKG-INFO` & `dearwatson-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.5.8
+Version: 0.5.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.5.8/README.md` & `dearwatson-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.5.9/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.5.8
+Version: 0.5.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.5.8/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.5.9/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/setup.py` & `dearwatson-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.5.8"
+version = "0.5.9"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -23,15 +23,15 @@
     python_requires='>=3.8',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "cython==0.29.21",
                         "extension-helpers==0.1",
                         "imageio==2.9.0",
-                        "lcbuilder==0.10.11",
+                        "lcbuilder==0.10.12",
                         "matplotlib==3.5.2",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==5.4.1",
                         "reportlab==3.5.59",
                         'setuptools>=41.0.0',
     ]
 )
```

### Comparing `dearwatson-0.5.8/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.5.9/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/neighbours.py` & `dearwatson-0.5.9/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/report.py` & `dearwatson-0.5.9/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/resources/images/sherlock3.png` & `dearwatson-0.5.9/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/resources/images/watson.png` & `dearwatson-0.5.9/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/tests/test_watson.py` & `dearwatson-0.5.9/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.8/watson/watson.py` & `dearwatson-0.5.9/watson/watson.py`

 * *Files identical despite different names*

