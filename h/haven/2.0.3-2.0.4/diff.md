# Comparing `tmp/haven-2.0.3.tar.gz` & `tmp/haven-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/haven-2.0.3.tar", last modified: Wed Jul 15 02:47:53 2020, max compression
+gzip compressed data, was "haven-2.0.4.tar", last modified: Sat Apr  8 17:10:51 2023, max compression
```

## Comparing `haven-2.0.3.tar` & `haven-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-15 02:47:53.000000 haven-2.0.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      259 2020-07-15 02:47:53.000000 haven-2.0.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      545 2019-01-11 15:25:06.000000 haven-2.0.3/README.md
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-15 02:47:53.000000 haven-2.0.3/haven/
--rw-r--r--   0 dantezhu   (501) staff       (20)      250 2020-07-15 02:47:33.000000 haven-2.0.3/haven/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      521 2020-06-08 04:00:30.000000 haven-2.0.3/haven/blueprint.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4311 2020-06-08 04:00:30.000000 haven-2.0.3/haven/connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      167 2020-06-08 04:00:31.000000 haven-2.0.3/haven/constants.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-15 02:47:53.000000 haven-2.0.3/haven/contrib/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-06-08 04:00:27.000000 haven-2.0.3/haven/contrib/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3511 2020-06-08 04:00:30.000000 haven-2.0.3/haven/contrib/websocket_gevent_impl.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3590 2020-06-08 04:00:30.000000 haven-2.0.3/haven/gevent_impl.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3734 2020-07-15 02:43:36.000000 haven-2.0.3/haven/haven.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       83 2020-06-08 04:00:30.000000 haven-2.0.3/haven/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4255 2020-07-15 02:43:09.000000 haven-2.0.3/haven/mixins.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2227 2020-07-15 02:45:33.000000 haven-2.0.3/haven/request.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3669 2020-06-08 04:00:30.000000 haven-2.0.3/haven/thread_impl.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      577 2020-06-08 04:00:30.000000 haven-2.0.3/haven/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      259 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      449 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-06-20 13:57:32.000000 haven-2.0.3/haven.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       51 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2020-07-15 02:47:53.000000 haven-2.0.3/haven.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-07-15 02:47:53.000000 haven-2.0.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      503 2020-07-15 02:47:32.000000 haven-2.0.3/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:10:51.413206 haven-2.0.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1074 2014-06-20 12:35:10.000000 haven-2.0.4/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      328 2023-04-08 17:10:51.413442 haven-2.0.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      545 2019-01-11 15:25:06.000000 haven-2.0.4/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:10:51.401075 haven-2.0.4/haven/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      250 2023-04-08 17:10:37.000000 haven-2.0.4/haven/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      521 2020-06-08 04:00:30.000000 haven-2.0.4/haven/blueprint.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4311 2020-06-08 04:00:30.000000 haven-2.0.4/haven/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      167 2020-06-08 04:00:31.000000 haven-2.0.4/haven/constants.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:10:51.412266 haven-2.0.4/haven/contrib/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-06-08 04:00:27.000000 haven-2.0.4/haven/contrib/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3511 2020-06-08 04:00:30.000000 haven-2.0.4/haven/contrib/websocket_gevent_impl.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3590 2020-06-08 04:00:30.000000 haven-2.0.4/haven/gevent_impl.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3734 2020-07-15 02:43:36.000000 haven-2.0.4/haven/haven.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       83 2020-06-08 04:00:30.000000 haven-2.0.4/haven/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4255 2020-07-15 02:43:09.000000 haven-2.0.4/haven/mixins.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2227 2020-07-15 02:45:33.000000 haven-2.0.4/haven/request.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3669 2020-06-08 04:00:30.000000 haven-2.0.4/haven/thread_impl.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      577 2020-06-08 04:00:30.000000 haven-2.0.4/haven/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:10:51.410663 haven-2.0.4/haven.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      328 2023-04-08 17:10:51.000000 haven-2.0.4/haven.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      482 2023-04-08 17:10:51.000000 haven-2.0.4/haven.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:10:51.000000 haven-2.0.4/haven.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-06-20 13:57:32.000000 haven-2.0.4/haven.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       51 2023-04-08 17:10:51.000000 haven-2.0.4/haven.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:10:51.000000 haven-2.0.4/haven.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      634 2023-04-08 17:10:42.000000 haven-2.0.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      456 2023-04-08 17:10:51.414625 haven-2.0.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      503 2023-04-08 17:10:33.000000 haven-2.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `haven-2.0.3/README.md` & `haven-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/blueprint.py` & `haven-2.0.4/haven/blueprint.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/connection.py` & `haven-2.0.4/haven/connection.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/contrib/websocket_gevent_impl.py` & `haven-2.0.4/haven/contrib/websocket_gevent_impl.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/gevent_impl.py` & `haven-2.0.4/haven/gevent_impl.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/haven.py` & `haven-2.0.4/haven/haven.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/mixins.py` & `haven-2.0.4/haven/mixins.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/request.py` & `haven-2.0.4/haven/request.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/thread_impl.py` & `haven-2.0.4/haven/thread_impl.py`

 * *Files identical despite different names*

### Comparing `haven-2.0.3/haven/utils.py` & `haven-2.0.4/haven/utils.py`

 * *Files identical despite different names*

