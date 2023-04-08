# Comparing `tmp/pycryptlib-1.0.0.tar.gz` & `tmp/pycryptlib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptlib-1.0.0.tar", last modified: Thu Apr  6 20:27:58 2023, max compression
+gzip compressed data, was "pycryptlib-1.1.5.tar", last modified: Sat Apr  8 17:51:30 2023, max compression
```

## Comparing `pycryptlib-1.0.0.tar` & `pycryptlib-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:27:58.699774 pycryptlib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-06 20:27:58.699774 pycryptlib-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:27:58.699774 pycryptlib-1.0.0/pycryptlib/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-06 20:27:58.000000 pycryptlib-1.0.0/pycryptlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:27:58.699774 pycryptlib-1.0.0/pycryptlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-06 20:27:58.000000 pycryptlib-1.0.0/pycryptlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-06 20:27:58.000000 pycryptlib-1.0.0/pycryptlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 20:27:58.000000 pycryptlib-1.0.0/pycryptlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-06 20:27:58.000000 pycryptlib-1.0.0/pycryptlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 20:27:58.699774 pycryptlib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-06 20:27:57.000000 pycryptlib-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 17:51:30.108103 pycryptlib-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-08 17:51:30.108103 pycryptlib-1.1.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 17:51:30.104103 pycryptlib-1.1.5/pycryptlib/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-08 17:51:29.000000 pycryptlib-1.1.5/pycryptlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 17:51:30.108103 pycryptlib-1.1.5/pycryptlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-08 17:51:30.000000 pycryptlib-1.1.5/pycryptlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-08 17:51:30.000000 pycryptlib-1.1.5/pycryptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 17:51:30.000000 pycryptlib-1.1.5/pycryptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-08 17:51:30.000000 pycryptlib-1.1.5/pycryptlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 17:51:30.108103 pycryptlib-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-08 17:51:28.000000 pycryptlib-1.1.5/setup.py
```

### Comparing `pycryptlib-1.0.0/setup.py` & `pycryptlib-1.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Package"
-LONG_DESCRIPTION = "Package"
+VERSION = '1.1.5'
+DESCRIPTION = "Package that helps with cryptography"
+LONG_DESCRIPTION = "Package that helps with cryptography"
 
 # Setting up
 setup(
     name="pycryptlib",
     version=VERSION,
     author="NHJonas",
-    author_email="NHJonas@gmail.com",
+    author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
```

