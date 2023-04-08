# Comparing `tmp/shock-0.2.3.tar.gz` & `tmp/shock-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shock-0.2.3.tar", last modified: Mon Jul 16 15:44:52 2018, max compression
+gzip compressed data, was "shock-0.2.4.tar", last modified: Sat Apr  8 17:36:57 2023, max compression
```

## Comparing `shock-0.2.3.tar` & `shock-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:44:52.000000 shock-0.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      241 2018-07-16 15:44:52.000000 shock-0.2.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-07-16 15:44:52.000000 shock-0.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      419 2018-07-16 15:44:30.000000 shock-0.2.3/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:44:52.000000 shock-0.2.3/shock/
--rw-r--r--   0 dantezhu   (501) staff       (20)      123 2018-07-16 15:44:31.000000 shock-0.2.3/shock/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:44:52.000000 shock-0.2.3/shock/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)     3460 2018-05-19 12:58:05.000000 shock-0.2.3/shock/bin/shock
--rw-r--r--   0 dantezhu   (501) staff       (20)       39 2016-10-26 06:33:08.000000 shock-0.2.3/shock/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     5922 2018-05-19 12:58:05.000000 shock-0.2.3/shock/shock_connect.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     8392 2018-05-19 12:58:05.000000 shock-0.2.3/shock/shock_echo.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      451 2018-05-19 12:58:05.000000 shock-0.2.3/shock/six.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2201 2018-07-16 15:43:43.000000 shock-0.2.3/shock/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      241 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      304 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-11-29 09:56:07.000000 shock-0.2.3/shock.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       26 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2018-07-16 15:44:52.000000 shock-0.2.3/shock.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:57.086236 shock-0.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:36:57.086392 shock-0.2.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      522 2023-04-08 17:36:48.000000 shock-0.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      373 2023-04-08 17:36:57.088897 shock-0.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      419 2023-04-08 17:36:36.000000 shock-0.2.4/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:57.079273 shock-0.2.4/shock/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      123 2023-04-08 17:36:41.000000 shock-0.2.4/shock/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:57.085427 shock-0.2.4/shock/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)     3460 2018-05-19 12:58:05.000000 shock-0.2.4/shock/bin/shock
+-rw-r--r--   0 dantezhu   (501) staff       (20)       39 2016-10-26 06:33:08.000000 shock-0.2.4/shock/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     5922 2018-05-19 12:58:05.000000 shock-0.2.4/shock/shock_connect.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     8392 2018-05-19 12:58:05.000000 shock-0.2.4/shock/shock_echo.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      451 2018-05-19 12:58:05.000000 shock-0.2.4/shock/six.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2201 2018-07-16 15:43:43.000000 shock-0.2.4/shock/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:36:57.084578 shock-0.2.4/shock.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:36:57.000000 shock-0.2.4/shock.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      329 2023-04-08 17:36:57.000000 shock-0.2.4/shock.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:36:57.000000 shock-0.2.4/shock.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-11-29 09:56:07.000000 shock-0.2.4/shock.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       26 2023-04-08 17:36:57.000000 shock-0.2.4/shock.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:36:57.000000 shock-0.2.4/shock.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `shock-0.2.3/shock/bin/shock` & `shock-0.2.4/shock/bin/shock`

 * *Files identical despite different names*

### Comparing `shock-0.2.3/shock/shock_connect.py` & `shock-0.2.4/shock/shock_connect.py`

 * *Files identical despite different names*

### Comparing `shock-0.2.3/shock/shock_echo.py` & `shock-0.2.4/shock/shock_echo.py`

 * *Files identical despite different names*

### Comparing `shock-0.2.3/shock/utils.py` & `shock-0.2.4/shock/utils.py`

 * *Files identical despite different names*

