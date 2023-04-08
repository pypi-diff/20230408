# Comparing `tmp/maple-4.1.4.tar.gz` & `tmp/maple-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maple-4.1.4.tar", last modified: Sat Jul 18 17:36:50 2020, max compression
+gzip compressed data, was "maple-4.1.5.tar", last modified: Sat Apr  8 17:05:40 2023, max compression
```

## Comparing `maple-4.1.4.tar` & `maple-4.1.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.884767 maple-4.1.4/
--rw-rw-rw-   0        0        0      285 2020-07-18 17:36:50.884767 maple-4.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.869807 maple-4.1.4/maple/
--rw-rw-rw-   0        0        0      230 2020-07-18 17:36:00.000000 maple-4.1.4/maple/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.873796 maple-4.1.4/maple/contrib/
--rw-rw-rw-   0        0        0        1 2020-05-23 15:30:29.000000 maple-4.1.4/maple/contrib/__init__.py
--rw-rw-rw-   0        0        0     1966 2020-05-23 17:02:09.000000 maple-4.1.4/maple/contrib/virtual_request.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.877786 maple-4.1.4/maple/share/
--rw-rw-rw-   0        0        0        0 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/__init__.py
--rw-rw-rw-   0        0        0     1082 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/constants.py
--rw-rw-rw-   0        0        0       90 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/log.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.878784 maple-4.1.4/maple/share/proto/
--rw-rw-rw-   0        0        0        0 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/proto/__init__.py
--rw-rw-rw-   0        0        0     6389 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/proto/maple_pb2.py
--rw-rw-rw-   0        0        0     1823 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/task.py
--rw-rw-rw-   0        0        0      577 2020-05-23 17:02:09.000000 maple-4.1.4/maple/share/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.879780 maple-4.1.4/maple/trigger/
--rw-rw-rw-   0        0        0        0 2020-05-23 15:30:29.000000 maple-4.1.4/maple/trigger/__init__.py
--rw-rw-rw-   0        0        0     4740 2020-05-23 17:02:09.000000 maple-4.1.4/maple/trigger/client.py
--rw-rw-rw-   0        0        0     2875 2020-07-18 17:35:22.000000 maple-4.1.4/maple/trigger/trigger.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.880778 maple-4.1.4/maple/workshop/
--rw-rw-rw-   0        0        0        0 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/__init__.py
--rw-rw-rw-   0        0        0      564 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/blueprint.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.881775 maple-4.1.4/maple/workshop/common/
--rw-rw-rw-   0        0        0        0 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/common/__init__.py
--rw-rw-rw-   0        0        0     4780 2020-07-15 15:12:51.000000 maple-4.1.4/maple/workshop/common/mixins.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.882772 maple-4.1.4/maple/workshop/master/
--rw-rw-rw-   0        0        0       27 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/master/__init__.py
--rw-rw-rw-   0        0        0     3560 2020-07-08 15:38:34.000000 maple-4.1.4/maple/workshop/master/master.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.884767 maple-4.1.4/maple/workshop/worker/
--rw-rw-rw-   0        0        0       91 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/worker/__init__.py
--rw-rw-rw-   0        0        0     7546 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/worker/connection.py
--rw-rw-rw-   0        0        0     6138 2020-07-15 15:12:51.000000 maple-4.1.4/maple/workshop/worker/request.py
--rw-rw-rw-   0        0        0     1640 2020-06-13 16:51:59.000000 maple-4.1.4/maple/workshop/worker/worker.py
--rw-rw-rw-   0        0        0     3018 2020-07-15 15:12:51.000000 maple-4.1.4/maple/workshop/workshop.py
-drwxrwxrwx   0        0        0        0 2020-07-18 17:36:50.872799 maple-4.1.4/maple.egg-info/
--rw-rw-rw-   0        0        0      285 2020-07-18 17:36:50.000000 maple-4.1.4/maple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      823 2020-07-18 17:36:50.000000 maple-4.1.4/maple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-18 17:36:50.000000 maple-4.1.4/maple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2020-07-18 17:36:50.000000 maple-4.1.4/maple.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-07-18 17:36:50.000000 maple-4.1.4/maple.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-18 17:36:50.885764 maple-4.1.4/setup.cfg
--rw-rw-rw-   0        0        0      477 2020-07-18 17:36:04.000000 maple-4.1.4/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.343913 maple-4.1.5/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      303 2023-04-08 17:05:40.344124 maple-4.1.5/PKG-INFO
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.308558 maple-4.1.5/maple/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      230 2023-04-08 17:05:02.000000 maple-4.1.5/maple/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.318576 maple-4.1.5/maple/contrib/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:35:49.000000 maple-4.1.5/maple/contrib/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1966 2020-05-25 02:04:23.000000 maple-4.1.5/maple/contrib/virtual_request.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.323859 maple-4.1.5/maple/share/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1082 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       90 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/log.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.325371 maple-4.1.5/maple/share/proto/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/proto/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6389 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/proto/maple_pb2.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1823 2020-06-10 06:31:56.000000 maple-4.1.5/maple/share/task.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      577 2020-05-25 02:04:23.000000 maple-4.1.5/maple/share/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.330326 maple-4.1.5/maple/trigger/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2014-12-01 08:21:49.000000 maple-4.1.5/maple/trigger/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4740 2020-05-25 02:04:23.000000 maple-4.1.5/maple/trigger/client.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2875 2020-07-21 01:43:15.000000 maple-4.1.5/maple/trigger/trigger.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.334833 maple-4.1.5/maple/workshop/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      564 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/blueprint.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.336845 maple-4.1.5/maple/workshop/common/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/common/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4780 2020-07-15 01:59:11.000000 maple-4.1.5/maple/workshop/common/mixins.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.338922 maple-4.1.5/maple/workshop/master/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/master/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3560 2020-07-08 04:24:14.000000 maple-4.1.5/maple/workshop/master/master.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.343232 maple-4.1.5/maple/workshop/worker/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       91 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/worker/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7546 2020-07-13 12:43:31.000000 maple-4.1.5/maple/workshop/worker/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6138 2020-07-15 01:59:11.000000 maple-4.1.5/maple/workshop/worker/request.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1640 2020-06-12 01:55:57.000000 maple-4.1.5/maple/workshop/worker/worker.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3018 2020-07-15 01:59:11.000000 maple-4.1.5/maple/workshop/workshop.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:05:40.315961 maple-4.1.5/maple.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      303 2023-04-08 17:05:40.000000 maple-4.1.5/maple.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      848 2023-04-08 17:05:40.000000 maple-4.1.5/maple.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:05:40.000000 maple-4.1.5/maple.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       43 2023-04-08 17:05:40.000000 maple-4.1.5/maple.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:05:40.000000 maple-4.1.5/maple.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      611 2023-04-08 17:05:27.000000 maple-4.1.5/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      436 2023-04-08 17:05:40.345374 maple-4.1.5/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      477 2023-04-08 17:04:52.000000 maple-4.1.5/setup.py
```

### Comparing `maple-4.1.4/maple/contrib/virtual_request.py` & `maple-4.1.5/maple/contrib/virtual_request.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/share/constants.py` & `maple-4.1.5/maple/share/constants.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/share/proto/maple_pb2.py` & `maple-4.1.5/maple/share/proto/maple_pb2.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/share/task.py` & `maple-4.1.5/maple/share/task.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/share/utils.py` & `maple-4.1.5/maple/share/utils.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/trigger/client.py` & `maple-4.1.5/maple/trigger/client.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/trigger/trigger.py` & `maple-4.1.5/maple/trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/blueprint.py` & `maple-4.1.5/maple/workshop/blueprint.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/common/mixins.py` & `maple-4.1.5/maple/workshop/common/mixins.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/master/master.py` & `maple-4.1.5/maple/workshop/master/master.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/worker/connection.py` & `maple-4.1.5/maple/workshop/worker/connection.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/worker/request.py` & `maple-4.1.5/maple/workshop/worker/request.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/worker/worker.py` & `maple-4.1.5/maple/workshop/worker/worker.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple/workshop/workshop.py` & `maple-4.1.5/maple/workshop/workshop.py`

 * *Files identical despite different names*

### Comparing `maple-4.1.4/maple.egg-info/SOURCES.txt` & `maple-4.1.5/maple.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+pyproject.toml
+setup.cfg
 setup.py
 maple/__init__.py
 maple.egg-info/PKG-INFO
 maple.egg-info/SOURCES.txt
 maple.egg-info/dependency_links.txt
 maple.egg-info/requires.txt
 maple.egg-info/top_level.txt
```

