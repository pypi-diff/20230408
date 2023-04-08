# Comparing `tmp/flask_autorest-0.1.5.tar.gz` & `tmp/flask_autorest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask_autorest-0.1.5.tar", last modified: Sun Aug 17 13:04:30 2014, max compression
+gzip compressed data, was "flask_autorest-0.1.6.tar", last modified: Sat Apr  8 17:34:47 2023, max compression
```

## Comparing `flask_autorest-0.1.5.tar` & `flask_autorest-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2014-08-17 13:04:30.000000 flask_autorest-0.1.5/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2014-08-17 13:04:30.000000 flask_autorest-0.1.5/flask_autorest/
--rw-r--r--   0 dantezhu   (501) staff       (20)      672 2014-08-17 13:03:47.000000 flask_autorest-0.1.5/flask_autorest/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1683 2014-08-09 05:55:38.000000 flask_autorest-0.1.5/flask_autorest/autorest.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      257 2014-08-17 12:53:50.000000 flask_autorest-0.1.5/flask_autorest/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      779 2014-08-09 06:01:45.000000 flask_autorest-0.1.5/flask_autorest/utils.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     5263 2014-08-17 13:03:11.000000 flask_autorest-0.1.5/flask_autorest/views.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2014-08-17 13:04:30.000000 flask_autorest-0.1.5/flask_autorest.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-08-17 13:04:13.000000 flask_autorest-0.1.5/flask_autorest.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-08-09 05:24:49.000000 flask_autorest-0.1.5/flask_autorest.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)      283 2014-08-17 13:04:13.000000 flask_autorest-0.1.5/flask_autorest.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       14 2014-08-17 13:04:13.000000 flask_autorest-0.1.5/flask_autorest.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      364 2014-08-17 13:04:13.000000 flask_autorest-0.1.5/flask_autorest.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       15 2014-08-17 13:04:13.000000 flask_autorest-0.1.5/flask_autorest.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      283 2014-08-17 13:04:30.000000 flask_autorest-0.1.5/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       59 2014-08-17 13:04:30.000000 flask_autorest-0.1.5/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      475 2014-08-17 13:03:54.000000 flask_autorest-0.1.5/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:34:47.169792 flask_autorest-0.1.6/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1075 2014-08-08 12:32:03.000000 flask_autorest-0.1.6/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      361 2023-04-08 17:34:47.170089 flask_autorest-0.1.6/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)       96 2014-08-08 12:32:03.000000 flask_autorest-0.1.6/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:34:47.161356 flask_autorest-0.1.6/flask_autorest/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      672 2023-04-08 17:34:30.000000 flask_autorest-0.1.6/flask_autorest/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1683 2014-08-09 05:55:38.000000 flask_autorest-0.1.6/flask_autorest/autorest.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      257 2014-08-17 12:53:50.000000 flask_autorest-0.1.6/flask_autorest/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      779 2014-08-09 06:01:45.000000 flask_autorest-0.1.6/flask_autorest/utils.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     5263 2014-08-17 13:03:11.000000 flask_autorest-0.1.6/flask_autorest/views.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:34:47.169019 flask_autorest-0.1.6/flask_autorest.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      361 2023-04-08 17:34:47.000000 flask_autorest-0.1.6/flask_autorest.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      407 2023-04-08 17:34:47.000000 flask_autorest-0.1.6/flask_autorest.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:34:47.000000 flask_autorest-0.1.6/flask_autorest.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-08-09 05:24:49.000000 flask_autorest-0.1.6/flask_autorest.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       14 2023-04-08 17:34:47.000000 flask_autorest-0.1.6/flask_autorest.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       15 2023-04-08 17:34:47.000000 flask_autorest-0.1.6/flask_autorest.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      593 2023-04-08 17:34:37.000000 flask_autorest-0.1.6/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      437 2023-04-08 17:34:47.171796 flask_autorest-0.1.6/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      475 2023-04-08 17:34:22.000000 flask_autorest-0.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flask_autorest-0.1.5/flask_autorest/__init__.py` & `flask_autorest-0.1.6/flask_autorest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         }
     }
 AUTOREST_BLUEPRINT_NAME
 AUTOREST_URL_PREFIX
 
 """
 
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 from .autorest import AutoRest
```

### Comparing `flask_autorest-0.1.5/flask_autorest/autorest.py` & `flask_autorest-0.1.6/flask_autorest/autorest.py`

 * *Files identical despite different names*

### Comparing `flask_autorest-0.1.5/flask_autorest/utils.py` & `flask_autorest-0.1.6/flask_autorest/utils.py`

 * *Files identical despite different names*

### Comparing `flask_autorest-0.1.5/flask_autorest/views.py` & `flask_autorest-0.1.6/flask_autorest/views.py`

 * *Files identical despite different names*

