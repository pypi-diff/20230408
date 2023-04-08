# Comparing `tmp/wfgfw-0.1.7.tar.gz` & `tmp/wfgfw-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wfgfw-0.1.7.tar", last modified: Mon Aug 12 04:37:25 2019, max compression
+gzip compressed data, was "wfgfw-0.1.8.tar", last modified: Sat Apr  8 17:19:47 2023, max compression
```

## Comparing `wfgfw-0.1.7.tar` & `wfgfw-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2019-08-12 04:37:25.000000 wfgfw-0.1.7/
--rw-rw-rw-   0        0        0      317 2019-08-12 04:37:25.000000 wfgfw-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      158 2019-05-04 09:13:54.000000 wfgfw-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2019-08-12 04:37:25.000000 wfgfw-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      394 2019-08-12 04:36:59.000000 wfgfw-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw/
--rw-rw-rw-   0        0        0      114 2019-08-12 04:36:59.000000 wfgfw-0.1.7/wfgfw/__init__.py
--rw-rw-rw-   0        0        0      691 2019-08-12 04:05:39.000000 wfgfw-0.1.7/wfgfw/flask_wfgfw.py
--rw-rw-rw-   0        0        0     7283 2019-08-12 04:36:01.000000 wfgfw-0.1.7/wfgfw/wfgfw.py
-drwxrwxrwx   0        0        0        0 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw.egg-info/
--rw-rw-rw-   0        0        0      317 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-05-04 09:18:36.000000 wfgfw-0.1.7/wfgfw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2019-08-12 04:37:25.000000 wfgfw-0.1.7/wfgfw.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:47.965640 wfgfw-0.1.8/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      354 2023-04-08 17:19:47.966319 wfgfw-0.1.8/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      158 2013-12-24 04:50:43.000000 wfgfw-0.1.8/README.md
+-rw-r--r--   0 dantezhu   (501) staff       (20)      502 2023-04-08 17:19:39.000000 wfgfw-0.1.8/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      366 2023-04-08 17:19:47.970502 wfgfw-0.1.8/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      394 2023-04-08 17:19:31.000000 wfgfw-0.1.8/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:47.959764 wfgfw-0.1.8/wfgfw/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      114 2023-04-08 17:19:35.000000 wfgfw-0.1.8/wfgfw/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      691 2020-11-15 15:58:04.000000 wfgfw-0.1.8/wfgfw/flask_wfgfw.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7283 2020-11-15 15:58:04.000000 wfgfw-0.1.8/wfgfw/wfgfw.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:19:47.964183 wfgfw-0.1.8/wfgfw.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      354 2023-04-08 17:19:47.000000 wfgfw-0.1.8/wfgfw.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      241 2023-04-08 17:19:47.000000 wfgfw-0.1.8/wfgfw.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:19:47.000000 wfgfw-0.1.8/wfgfw.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2013-12-28 12:11:08.000000 wfgfw-0.1.8/wfgfw.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:19:47.000000 wfgfw-0.1.8/wfgfw.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wfgfw-0.1.7/wfgfw/flask_wfgfw.py` & `wfgfw-0.1.8/wfgfw/flask_wfgfw.py`

 * *Files identical despite different names*

### Comparing `wfgfw-0.1.7/wfgfw/wfgfw.py` & `wfgfw-0.1.8/wfgfw/wfgfw.py`

 * *Files identical despite different names*

