# Comparing `tmp/maple_guard-0.2.3.tar.gz` & `tmp/maple_guard-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maple_guard-0.2.3.tar", last modified: Mon Jul 16 15:41:47 2018, max compression
+gzip compressed data, was "maple_guard-0.2.4.tar", last modified: Sat Apr  8 17:17:17 2023, max compression
```

## Comparing `maple_guard-0.2.3.tar` & `maple_guard-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      224 2018-07-16 15:41:47.000000 maple_guard-0.2.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      410 2018-05-16 07:15:03.000000 maple_guard-0.2.3/README.md
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard/
--rw-r--r--   0 dantezhu   (501) staff       (20)      116 2018-07-16 15:41:17.000000 maple_guard-0.2.3/maple_guard/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)     1285 2018-07-16 15:41:03.000000 maple_guard-0.2.3/maple_guard/bin/run_maple_guard.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard/client/
--rw-r--r--   0 dantezhu   (501) staff       (20)       23 2016-11-02 12:23:52.000000 maple_guard-0.2.3/maple_guard/client/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2522 2017-08-30 08:52:20.000000 maple_guard-0.2.3/maple_guard/client/client.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      321 2017-05-24 06:34:47.000000 maple_guard-0.2.3/maple_guard/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      109 2016-11-02 11:22:03.000000 maple_guard-0.2.3/maple_guard/log.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard/server/
--rw-r--r--   0 dantezhu   (501) staff       (20)       23 2016-11-02 12:21:22.000000 maple_guard-0.2.3/maple_guard/server/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      748 2016-11-02 16:13:38.000000 maple_guard-0.2.3/maple_guard/server/blocker.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1140 2016-12-22 03:42:34.000000 maple_guard-0.2.3/maple_guard/server/rate_limiter.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1650 2016-11-02 13:51:58.000000 maple_guard-0.2.3/maple_guard/server/redis_extend.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     6740 2016-12-22 03:43:58.000000 maple_guard-0.2.3/maple_guard/server/server.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      388 2018-05-16 06:29:04.000000 maple_guard-0.2.3/maple_guard/six.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1711 2018-05-16 06:29:27.000000 maple_guard-0.2.3/maple_guard/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      224 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      589 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 06:32:44.000000 maple_guard-0.2.3/maple_guard.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       19 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       12 2018-07-16 15:41:47.000000 maple_guard-0.2.3/maple_guard.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-07-16 15:41:47.000000 maple_guard-0.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      476 2018-07-16 15:41:17.000000 maple_guard-0.2.3/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.241308 maple_guard-0.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1069 2016-11-02 10:49:59.000000 maple_guard-0.2.4/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      299 2023-04-08 17:17:17.241505 maple_guard-0.2.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      410 2018-05-16 07:15:03.000000 maple_guard-0.2.4/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.197628 maple_guard-0.2.4/maple_guard/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      116 2023-04-08 17:17:03.000000 maple_guard-0.2.4/maple_guard/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.230329 maple_guard-0.2.4/maple_guard/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)     1285 2018-07-16 15:41:03.000000 maple_guard-0.2.4/maple_guard/bin/run_maple_guard.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.235042 maple_guard-0.2.4/maple_guard/client/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2016-11-02 12:23:52.000000 maple_guard-0.2.4/maple_guard/client/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2522 2017-08-30 08:52:20.000000 maple_guard-0.2.4/maple_guard/client/client.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      321 2017-05-24 06:34:47.000000 maple_guard-0.2.4/maple_guard/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      109 2016-11-02 11:22:03.000000 maple_guard-0.2.4/maple_guard/log.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.240520 maple_guard-0.2.4/maple_guard/server/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2016-11-02 12:21:22.000000 maple_guard-0.2.4/maple_guard/server/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      748 2016-11-02 16:13:38.000000 maple_guard-0.2.4/maple_guard/server/blocker.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1140 2016-12-22 03:42:34.000000 maple_guard-0.2.4/maple_guard/server/rate_limiter.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1650 2016-11-02 13:51:58.000000 maple_guard-0.2.4/maple_guard/server/redis_extend.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6740 2016-12-22 03:43:58.000000 maple_guard-0.2.4/maple_guard/server/server.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      388 2018-05-16 06:29:04.000000 maple_guard-0.2.4/maple_guard/six.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1711 2018-05-16 06:29:27.000000 maple_guard-0.2.4/maple_guard/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:17.229634 maple_guard-0.2.4/maple_guard.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      299 2023-04-08 17:17:17.000000 maple_guard-0.2.4/maple_guard.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      622 2023-04-08 17:17:17.000000 maple_guard-0.2.4/maple_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:17:17.000000 maple_guard-0.2.4/maple_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 06:32:44.000000 maple_guard-0.2.4/maple_guard.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       19 2023-04-08 17:17:17.000000 maple_guard-0.2.4/maple_guard.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       12 2023-04-08 17:17:17.000000 maple_guard-0.2.4/maple_guard.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      589 2023-04-08 17:17:06.000000 maple_guard-0.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      429 2023-04-08 17:17:17.244595 maple_guard-0.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      476 2023-04-08 17:16:56.000000 maple_guard-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `maple_guard-0.2.3/maple_guard/bin/run_maple_guard.py` & `maple_guard-0.2.4/maple_guard/bin/run_maple_guard.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/client/client.py` & `maple_guard-0.2.4/maple_guard/client/client.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/server/blocker.py` & `maple_guard-0.2.4/maple_guard/server/blocker.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/server/rate_limiter.py` & `maple_guard-0.2.4/maple_guard/server/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/server/redis_extend.py` & `maple_guard-0.2.4/maple_guard/server/redis_extend.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/server/server.py` & `maple_guard-0.2.4/maple_guard/server/server.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard/utils.py` & `maple_guard-0.2.4/maple_guard/utils.py`

 * *Files identical despite different names*

### Comparing `maple_guard-0.2.3/maple_guard.egg-info/SOURCES.txt` & `maple_guard-0.2.4/maple_guard.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+LICENSE
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 maple_guard/__init__.py
 maple_guard/constants.py
 maple_guard/log.py
 maple_guard/six.py
 maple_guard/utils.py
 maple_guard.egg-info/PKG-INFO
```

