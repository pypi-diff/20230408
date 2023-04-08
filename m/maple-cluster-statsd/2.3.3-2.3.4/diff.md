# Comparing `tmp/maple_cluster_statsd-2.3.3.tar.gz` & `tmp/maple_cluster_statsd-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maple_cluster_statsd-2.3.3.tar", last modified: Wed May 16 07:11:30 2018, max compression
+gzip compressed data, was "maple_cluster_statsd-2.3.4.tar", last modified: Sat Apr  8 17:23:16 2023, max compression
```

## Comparing `maple_cluster_statsd-2.3.3.tar` & `maple_cluster_statsd-2.3.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd/
--rw-r--r--   0 dantezhu   (501) staff       (20)      676 2018-05-16 07:10:31.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3149 2016-11-11 09:18:20.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      558 2016-05-19 09:26:18.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd/stat_reader.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1985 2018-05-16 07:09:14.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd/stat_reporter.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-10-19 05:02:37.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)      266 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)        7 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      421 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       21 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/maple_cluster_statsd.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      266 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       90 2016-10-19 05:04:19.000000 maple_cluster_statsd-2.3.3/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-05-16 07:11:30.000000 maple_cluster_statsd-2.3.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      473 2018-05-16 07:10:30.000000 maple_cluster_statsd-2.3.3/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:23:16.153252 maple_cluster_statsd-2.3.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1079 2016-02-26 07:26:44.000000 maple_cluster_statsd-2.3.4/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      350 2023-04-08 17:23:16.153373 maple_cluster_statsd-2.3.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      118 2018-05-16 07:15:39.000000 maple_cluster_statsd-2.3.4/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:23:16.146927 maple_cluster_statsd-2.3.4/maple_cluster_statsd/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      676 2023-04-08 17:23:02.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3149 2016-11-11 09:18:20.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      558 2016-05-19 09:26:18.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd/stat_reader.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1985 2018-05-16 07:09:14.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd/stat_reporter.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:23:16.152938 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      350 2023-04-08 17:23:16.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      454 2023-04-08 17:23:16.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:23:16.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-10-19 05:02:37.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2023-04-08 17:23:16.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       21 2023-04-08 17:23:16.000000 maple_cluster_statsd-2.3.4/maple_cluster_statsd.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      566 2023-04-08 17:23:06.000000 maple_cluster_statsd-2.3.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      412 2023-04-08 17:23:16.154243 maple_cluster_statsd-2.3.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      473 2023-04-08 17:22:57.000000 maple_cluster_statsd-2.3.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `maple_cluster_statsd-2.3.3/maple_cluster_statsd/__init__.py` & `maple_cluster_statsd-2.3.4/maple_cluster_statsd/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '2.3.3'
+__version__ = '2.3.4'
 
 from .stat_reporter import StatReporter
 from .stat_reader import StatReader
 from . import constants
 
 
 def create_gateway_reporter(cmd, statsd_client, statsd_name_converter=None):
```

### Comparing `maple_cluster_statsd-2.3.3/maple_cluster_statsd/constants.py` & `maple_cluster_statsd-2.3.4/maple_cluster_statsd/constants.py`

 * *Files identical despite different names*

### Comparing `maple_cluster_statsd-2.3.3/maple_cluster_statsd/stat_reader.py` & `maple_cluster_statsd-2.3.4/maple_cluster_statsd/stat_reader.py`

 * *Files identical despite different names*

### Comparing `maple_cluster_statsd-2.3.3/maple_cluster_statsd/stat_reporter.py` & `maple_cluster_statsd-2.3.4/maple_cluster_statsd/stat_reporter.py`

 * *Files identical despite different names*

