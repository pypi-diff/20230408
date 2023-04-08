# Comparing `tmp/maple_timer-1.0.7.tar.gz` & `tmp/maple_timer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maple_timer-1.0.7.tar", last modified: Fri Feb 19 03:49:35 2016, max compression
+gzip compressed data, was "maple_timer-1.0.8.tar", last modified: Sat Apr  8 17:13:21 2023, max compression
```

## Comparing `maple_timer-1.0.7.tar` & `maple_timer-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2016-02-19 03:49:35.000000 maple_timer-1.0.7/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2016-02-19 03:49:35.000000 maple_timer-1.0.7/maple_timer/
--rw-r--r--   0 dantezhu   (501) staff       (20)       59 2016-02-19 03:48:53.000000 maple_timer-1.0.7/maple_timer/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4646 2016-02-19 03:48:33.000000 maple_timer-1.0.7/maple_timer/maple_timer.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2016-02-19 03:49:35.000000 maple_timer-1.0.7/maple_timer.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-02-19 03:49:26.000000 maple_timer-1.0.7/maple_timer.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      253 2016-02-19 03:49:26.000000 maple_timer-1.0.7/maple_timer.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      199 2016-02-19 03:49:26.000000 maple_timer-1.0.7/maple_timer.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       12 2016-02-19 03:49:26.000000 maple_timer-1.0.7/maple_timer.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      253 2016-02-19 03:49:35.000000 maple_timer-1.0.7/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       59 2016-02-19 03:49:35.000000 maple_timer-1.0.7/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      422 2016-02-19 03:48:49.000000 maple_timer-1.0.7/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:13:21.558597 maple_timer-1.0.8/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:13:21.558877 maple_timer-1.0.8/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      200 2018-05-16 07:16:05.000000 maple_timer-1.0.8/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:13:21.554050 maple_timer-1.0.8/maple_timer/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       59 2023-04-08 17:13:04.000000 maple_timer-1.0.8/maple_timer/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4646 2018-05-16 07:12:45.000000 maple_timer-1.0.8/maple_timer/maple_timer.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:13:21.557862 maple_timer-1.0.8/maple_timer.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:13:21.000000 maple_timer-1.0.8/maple_timer.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      234 2023-04-08 17:13:21.000000 maple_timer-1.0.8/maple_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:13:21.000000 maple_timer-1.0.8/maple_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       12 2023-04-08 17:13:21.000000 maple_timer-1.0.8/maple_timer.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      515 2023-04-08 17:13:12.000000 maple_timer-1.0.8/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      367 2023-04-08 17:13:21.560151 maple_timer-1.0.8/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      422 2023-04-08 17:12:57.000000 maple_timer-1.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `maple_timer-1.0.7/maple_timer/maple_timer.py` & `maple_timer-1.0.8/maple_timer/maple_timer.py`

 * *Files identical despite different names*

