# Comparing `tmp/kpush-0.1.0.tar.gz` & `tmp/kpush-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kpush-0.1.0.tar", last modified: Sun Apr 19 14:41:16 2015, max compression
+gzip compressed data, was "kpush-0.1.1.tar", last modified: Sat Apr  8 17:35:01 2023, max compression
```

## Comparing `kpush-0.1.0.tar` & `kpush-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2015-04-19 14:41:16.000000 kpush-0.1.0/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2015-04-19 14:41:16.000000 kpush-0.1.0/kpush/
--rw-r--r--   0 dantezhu   (501) staff       (20)     1672 2015-04-19 14:40:56.000000 kpush-0.1.0/kpush/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2015-04-19 14:41:16.000000 kpush-0.1.0/kpush.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2015-04-19 14:41:10.000000 kpush-0.1.0/kpush.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      219 2015-04-19 14:41:10.000000 kpush-0.1.0/kpush.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)        9 2015-04-19 14:41:10.000000 kpush-0.1.0/kpush.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      170 2015-04-19 14:41:11.000000 kpush-0.1.0/kpush.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2015-04-19 14:41:10.000000 kpush-0.1.0/kpush.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      219 2015-04-19 14:41:16.000000 kpush-0.1.0/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       59 2015-04-19 14:41:16.000000 kpush-0.1.0/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      373 2015-04-19 14:09:01.000000 kpush-0.1.0/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:35:01.268981 kpush-0.1.1/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      248 2023-04-08 17:35:01.269232 kpush-0.1.1/PKG-INFO
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:35:01.264823 kpush-0.1.1/kpush/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1672 2023-04-08 17:34:47.000000 kpush-0.1.1/kpush/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:35:01.268260 kpush-0.1.1/kpush.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      248 2023-04-08 17:35:01.000000 kpush-0.1.1/kpush.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      195 2023-04-08 17:35:01.000000 kpush-0.1.1/kpush.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:35:01.000000 kpush-0.1.1/kpush.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        9 2023-04-08 17:35:01.000000 kpush-0.1.1/kpush.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:35:01.000000 kpush-0.1.1/kpush.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      491 2023-04-08 17:34:51.000000 kpush-0.1.1/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      341 2023-04-08 17:35:01.270430 kpush-0.1.1/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      373 2023-04-08 17:34:42.000000 kpush-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kpush-0.1.0/kpush/__init__.py` & `kpush-0.1.1/kpush/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import json
 import hashlib
 import requests
 
 
 def safe_str(src):
```

