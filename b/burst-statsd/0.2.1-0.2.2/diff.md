# Comparing `tmp/burst_statsd-0.2.1.tar.gz` & `tmp/burst_statsd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/burst_statsd-0.2.1.tar", last modified: Wed May 16 07:29:11 2018, max compression
+gzip compressed data, was "burst_statsd-0.2.2.tar", last modified: Sat Apr  8 17:15:00 2023, max compression
```

## Comparing `burst_statsd-0.2.1.tar` & `burst_statsd-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd/
--rw-r--r--   0 dantezhu   (501) staff       (20)      124 2018-05-16 07:28:17.000000 burst_statsd-0.2.1/burst_statsd/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      310 2016-05-23 03:43:41.000000 burst_statsd-0.2.1/burst_statsd/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      480 2016-06-17 14:18:31.000000 burst_statsd-0.2.1/burst_statsd/stat_reader.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3023 2018-05-16 07:24:53.000000 burst_statsd-0.2.1/burst_statsd/stat_reporter.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-05-19 12:15:13.000000 burst_statsd-0.2.1/burst_statsd.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)      242 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)        7 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      341 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       13 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/burst_statsd.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      242 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       71 2018-05-16 07:28:44.000000 burst_statsd-0.2.1/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-05-16 07:29:11.000000 burst_statsd-0.2.1/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      449 2018-05-16 07:28:10.000000 burst_statsd-0.2.1/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:15:00.845388 burst_statsd-0.2.2/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1079 2016-05-19 08:14:23.000000 burst_statsd-0.2.2/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      318 2023-04-08 17:15:00.845600 burst_statsd-0.2.2/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)       71 2018-05-16 07:28:44.000000 burst_statsd-0.2.2/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:15:00.837253 burst_statsd-0.2.2/burst_statsd/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      124 2023-04-08 17:14:50.000000 burst_statsd-0.2.2/burst_statsd/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      310 2016-05-23 03:43:41.000000 burst_statsd-0.2.2/burst_statsd/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      480 2016-06-17 14:18:31.000000 burst_statsd-0.2.2/burst_statsd/stat_reader.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3023 2018-05-16 07:24:53.000000 burst_statsd-0.2.2/burst_statsd/stat_reporter.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:15:00.844799 burst_statsd-0.2.2/burst_statsd.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      318 2023-04-08 17:15:00.000000 burst_statsd-0.2.2/burst_statsd.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      374 2023-04-08 17:15:00.000000 burst_statsd-0.2.2/burst_statsd.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:15:00.000000 burst_statsd-0.2.2/burst_statsd.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-05-19 12:15:13.000000 burst_statsd-0.2.2/burst_statsd.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2023-04-08 17:15:00.000000 burst_statsd-0.2.2/burst_statsd.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       13 2023-04-08 17:15:00.000000 burst_statsd-0.2.2/burst_statsd.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      535 2023-04-08 17:14:52.000000 burst_statsd-0.2.2/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      388 2023-04-08 17:15:00.846560 burst_statsd-0.2.2/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      449 2023-04-08 17:14:44.000000 burst_statsd-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `burst_statsd-0.2.1/burst_statsd/stat_reporter.py` & `burst_statsd-0.2.2/burst_statsd/stat_reporter.py`

 * *Files identical despite different names*

