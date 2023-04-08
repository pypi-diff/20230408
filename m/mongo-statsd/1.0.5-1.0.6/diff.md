# Comparing `tmp/mongo_statsd-1.0.5.tar.gz` & `tmp/mongo_statsd-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mongo_statsd-1.0.5.tar", last modified: Thu Mar 23 06:28:56 2017, max compression
+gzip compressed data, was "mongo_statsd-1.0.6.tar", last modified: Sat Apr  8 17:30:12 2023, max compression
```

## Comparing `mongo_statsd-1.0.5.tar` & `mongo_statsd-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd/
--rw-r--r--   0 dantezhu   (501) staff       (20)      124 2017-03-23 06:28:22.000000 mongo_statsd-1.0.5/mongo_statsd/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)     1628 2017-03-23 06:26:48.000000 mongo_statsd-1.0.5/mongo_statsd/bin/run_mongo_statsd.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3034 2017-03-23 06:16:03.000000 mongo_statsd-1.0.5/mongo_statsd/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1000 2017-03-23 06:19:10.000000 mongo_statsd-1.0.5/mongo_statsd/stat_reader.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2862 2017-03-23 06:17:14.000000 mongo_statsd-1.0.5/mongo_statsd/stat_reporter.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2017-03-23 05:56:55.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)      244 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)        7 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      368 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       13 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/mongo_statsd.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      244 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2017-03-23 06:28:56.000000 mongo_statsd-1.0.5/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      505 2017-03-23 06:28:22.000000 mongo_statsd-1.0.5/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:30:12.501354 mongo_statsd-1.0.6/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      298 2023-04-08 17:30:12.502589 mongo_statsd-1.0.6/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)       38 2017-03-23 02:24:31.000000 mongo_statsd-1.0.6/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:30:12.492419 mongo_statsd-1.0.6/mongo_statsd/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      124 2023-04-08 17:29:59.000000 mongo_statsd-1.0.6/mongo_statsd/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:30:12.498117 mongo_statsd-1.0.6/mongo_statsd/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)     1628 2017-03-23 06:26:48.000000 mongo_statsd-1.0.6/mongo_statsd/bin/run_mongo_statsd.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3034 2017-03-23 06:16:03.000000 mongo_statsd-1.0.6/mongo_statsd/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1000 2017-03-23 06:19:10.000000 mongo_statsd-1.0.6/mongo_statsd/stat_reader.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2862 2017-03-23 06:17:14.000000 mongo_statsd-1.0.6/mongo_statsd/stat_reporter.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:30:12.497152 mongo_statsd-1.0.6/mongo_statsd.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      298 2023-04-08 17:30:12.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      403 2023-04-08 17:30:12.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:30:12.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2017-03-23 05:56:55.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2023-04-08 17:30:12.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       13 2023-04-08 17:30:12.000000 mongo_statsd-1.0.6/mongo_statsd.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      593 2023-04-08 17:30:03.000000 mongo_statsd-1.0.6/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      437 2023-04-08 17:30:12.503949 mongo_statsd-1.0.6/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      505 2023-04-08 17:29:53.000000 mongo_statsd-1.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mongo_statsd-1.0.5/mongo_statsd/bin/run_mongo_statsd.py` & `mongo_statsd-1.0.6/mongo_statsd/bin/run_mongo_statsd.py`

 * *Files identical despite different names*

### Comparing `mongo_statsd-1.0.5/mongo_statsd/constants.py` & `mongo_statsd-1.0.6/mongo_statsd/constants.py`

 * *Files identical despite different names*

### Comparing `mongo_statsd-1.0.5/mongo_statsd/stat_reader.py` & `mongo_statsd-1.0.6/mongo_statsd/stat_reader.py`

 * *Files identical despite different names*

### Comparing `mongo_statsd-1.0.5/mongo_statsd/stat_reporter.py` & `mongo_statsd-1.0.6/mongo_statsd/stat_reporter.py`

 * *Files identical despite different names*

