# Comparing `tmp/kcp_net-0.2.3.tar.gz` & `tmp/kcp_net-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kcp_net-0.2.3.tar", last modified: Mon Oct  7 14:08:31 2019, max compression
+gzip compressed data, was "kcp_net-0.2.4.tar", last modified: Sat Apr  8 17:16:03 2023, max compression
```

## Comparing `kcp_net-0.2.3.tar` & `kcp_net-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-10-07 14:08:31.000000 kcp_net-0.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      212 2019-10-07 14:08:31.000000 kcp_net-0.2.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      241 2019-10-07 12:30:14.000000 kcp_net-0.2.3/README.md
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net/
--rw-r--r--   0 dantezhu   (501) staff       (20)      236 2019-10-07 14:08:00.000000 kcp_net-0.2.3/kcp_net/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7076 2019-10-07 14:07:13.000000 kcp_net-0.2.3/kcp_net/connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       43 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      109 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      929 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/mixins.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      404 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/output_listener.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1445 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/server.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1459 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/timer.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      602 2019-10-07 12:30:14.000000 kcp_net-0.2.3/kcp_net/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      212 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      377 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       26 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        8 2019-10-07 14:08:31.000000 kcp_net-0.2.3/kcp_net.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2019-10-07 14:08:31.000000 kcp_net-0.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      444 2019-10-07 14:08:00.000000 kcp_net-0.2.3/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:16:03.390660 kcp_net-0.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      261 2023-04-08 17:16:03.390874 kcp_net-0.2.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      241 2019-10-07 12:30:14.000000 kcp_net-0.2.4/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:16:03.384493 kcp_net-0.2.4/kcp_net/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      236 2023-04-08 17:15:51.000000 kcp_net-0.2.4/kcp_net/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7076 2019-10-07 14:07:13.000000 kcp_net-0.2.4/kcp_net/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       43 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      109 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      929 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/mixins.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      404 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/output_listener.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1445 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/server.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1459 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/timer.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      602 2019-10-07 12:30:14.000000 kcp_net-0.2.4/kcp_net/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:16:03.390159 kcp_net-0.2.4/kcp_net.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      261 2023-04-08 17:16:03.000000 kcp_net-0.2.4/kcp_net.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      402 2023-04-08 17:16:03.000000 kcp_net-0.2.4/kcp_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:16:03.000000 kcp_net-0.2.4/kcp_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-10-07 14:08:31.000000 kcp_net-0.2.4/kcp_net.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       26 2023-04-08 17:16:03.000000 kcp_net-0.2.4/kcp_net.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        8 2023-04-08 17:16:03.000000 kcp_net-0.2.4/kcp_net.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      530 2023-04-08 17:15:54.000000 kcp_net-0.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      379 2023-04-08 17:16:03.392109 kcp_net-0.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      444 2023-04-08 17:15:45.000000 kcp_net-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kcp_net-0.2.3/kcp_net/connection.py` & `kcp_net-0.2.4/kcp_net/connection.py`

 * *Files identical despite different names*

### Comparing `kcp_net-0.2.3/kcp_net/mixins.py` & `kcp_net-0.2.4/kcp_net/mixins.py`

 * *Files identical despite different names*

### Comparing `kcp_net-0.2.3/kcp_net/server.py` & `kcp_net-0.2.4/kcp_net/server.py`

 * *Files identical despite different names*

### Comparing `kcp_net-0.2.3/kcp_net/timer.py` & `kcp_net-0.2.4/kcp_net/timer.py`

 * *Files identical despite different names*

### Comparing `kcp_net-0.2.3/kcp_net/utils.py` & `kcp_net-0.2.4/kcp_net/utils.py`

 * *Files identical despite different names*

