# Comparing `tmp/svdog-0.2.3.tar.gz` & `tmp/svdog-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/svdog-0.2.3.tar", last modified: Mon Jul 16 15:46:46 2018, max compression
+gzip compressed data, was "svdog-0.2.4.tar", last modified: Sat Apr  8 17:36:21 2023, max compression
```

## Comparing `svdog-0.2.3.tar` & `svdog-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:46:46.000000 svdog-0.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      244 2018-07-16 15:46:46.000000 svdog-0.2.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      710 2018-05-16 07:44:29.000000 svdog-0.2.3/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-07-16 15:46:46.000000 svdog-0.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      418 2018-07-16 15:46:03.000000 svdog-0.2.3/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog/
--rw-r--r--   0 dantezhu   (501) staff       (20)     1128 2018-07-16 15:46:04.000000 svdog-0.2.3/svdog/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)      964 2018-07-16 15:45:37.000000 svdog-0.2.3/svdog/bin/run_svdog.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      244 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      231 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2013-12-23 07:11:39.000000 svdog-0.2.3/svdog.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       18 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2018-07-16 15:46:46.000000 svdog-0.2.3/svdog.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:21.037569 svdog-0.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      291 2023-04-08 17:36:21.037778 svdog-0.2.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      710 2018-05-16 07:44:29.000000 svdog-0.2.4/README.md
+-rw-r--r--   0 dantezhu   (501) staff       (20)      521 2023-04-08 17:36:12.000000 svdog-0.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      374 2023-04-08 17:36:21.038574 svdog-0.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      418 2023-04-08 17:36:01.000000 svdog-0.2.4/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:21.032025 svdog-0.2.4/svdog/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1128 2023-04-08 17:36:07.000000 svdog-0.2.4/svdog/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:21.036838 svdog-0.2.4/svdog/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)      964 2018-07-16 15:45:37.000000 svdog-0.2.4/svdog/bin/run_svdog.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:21.035936 svdog-0.2.4/svdog.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      291 2023-04-08 17:36:21.000000 svdog-0.2.4/svdog.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      256 2023-04-08 17:36:21.000000 svdog-0.2.4/svdog.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:36:21.000000 svdog-0.2.4/svdog.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2013-12-23 07:11:39.000000 svdog-0.2.4/svdog.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       18 2023-04-08 17:36:21.000000 svdog-0.2.4/svdog.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:36:21.000000 svdog-0.2.4/svdog.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `svdog-0.2.3/README.md` & `svdog-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `svdog-0.2.3/svdog/__init__.py` & `svdog-0.2.4/svdog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 import re
 import sys
 import logging
 import logging.config
 
 from supervisor import childutils
```

### Comparing `svdog-0.2.3/svdog/bin/run_svdog.py` & `svdog-0.2.4/svdog/bin/run_svdog.py`

 * *Files identical despite different names*

