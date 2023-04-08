# Comparing `tmp/ws_proxy-0.2.7.tar.gz` & `tmp/ws_proxy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ws_proxy-0.2.7.tar", last modified: Thu Aug  2 07:01:09 2018, max compression
+gzip compressed data, was "ws_proxy-0.2.8.tar", last modified: Sat Apr  8 17:19:21 2023, max compression
```

## Comparing `ws_proxy-0.2.7.tar` & `ws_proxy-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/
--rw-r--r--   0 dantezhu   (501) staff       (20)      228 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      469 2018-08-02 07:00:56.000000 ws_proxy-0.2.7/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy/
--rw-r--r--   0 dantezhu   (501) staff       (20)      130 2018-08-02 07:01:00.000000 ws_proxy-0.2.7/ws_proxy/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)      995 2018-08-02 07:00:29.000000 ws_proxy-0.2.7/ws_proxy/bin/ws_proxy
--rw-r--r--   0 dantezhu   (501) staff       (20)     3176 2018-08-02 06:44:18.000000 ws_proxy-0.2.7/ws_proxy/connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       43 2018-08-02 06:43:46.000000 ws_proxy-0.2.7/ws_proxy/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       99 2018-08-02 06:25:44.000000 ws_proxy-0.2.7/ws_proxy/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1334 2018-08-02 06:45:18.000000 ws_proxy-0.2.7/ws_proxy/server.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      592 2018-08-02 06:43:40.000000 ws_proxy-0.2.7/ws_proxy/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      228 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      339 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-08-02 03:45:16.000000 ws_proxy-0.2.7/ws_proxy.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       24 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        9 2018-08-02 07:01:09.000000 ws_proxy-0.2.7/ws_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:21.815657 ws_proxy-0.2.8/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      278 2023-04-08 17:19:21.815859 ws_proxy-0.2.8/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      582 2023-04-08 17:19:13.000000 ws_proxy-0.2.8/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      424 2023-04-08 17:19:21.817072 ws_proxy-0.2.8/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      469 2023-04-08 17:18:58.000000 ws_proxy-0.2.8/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:21.809405 ws_proxy-0.2.8/ws_proxy/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      130 2023-04-08 17:19:04.000000 ws_proxy-0.2.8/ws_proxy/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:21.814838 ws_proxy-0.2.8/ws_proxy/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)      995 2018-08-02 07:00:29.000000 ws_proxy-0.2.8/ws_proxy/bin/ws_proxy
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3176 2018-08-02 06:44:18.000000 ws_proxy-0.2.8/ws_proxy/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       43 2018-08-02 06:43:46.000000 ws_proxy-0.2.8/ws_proxy/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       99 2018-08-02 06:25:44.000000 ws_proxy-0.2.8/ws_proxy/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1334 2018-08-02 06:45:18.000000 ws_proxy-0.2.8/ws_proxy/server.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      592 2018-08-02 06:43:40.000000 ws_proxy-0.2.8/ws_proxy/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:21.814124 ws_proxy-0.2.8/ws_proxy.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      278 2023-04-08 17:19:21.000000 ws_proxy-0.2.8/ws_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      364 2023-04-08 17:19:21.000000 ws_proxy-0.2.8/ws_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:19:21.000000 ws_proxy-0.2.8/ws_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-08-02 03:45:16.000000 ws_proxy-0.2.8/ws_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       24 2023-04-08 17:19:21.000000 ws_proxy-0.2.8/ws_proxy.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        9 2023-04-08 17:19:21.000000 ws_proxy-0.2.8/ws_proxy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ws_proxy-0.2.7/ws_proxy/bin/ws_proxy` & `ws_proxy-0.2.8/ws_proxy/bin/ws_proxy`

 * *Files identical despite different names*

### Comparing `ws_proxy-0.2.7/ws_proxy/connection.py` & `ws_proxy-0.2.8/ws_proxy/connection.py`

 * *Files identical despite different names*

### Comparing `ws_proxy-0.2.7/ws_proxy/server.py` & `ws_proxy-0.2.8/ws_proxy/server.py`

 * *Files identical despite different names*

### Comparing `ws_proxy-0.2.7/ws_proxy/utils.py` & `ws_proxy-0.2.8/ws_proxy/utils.py`

 * *Files identical despite different names*

