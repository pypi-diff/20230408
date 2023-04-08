# Comparing `tmp/yunbk-0.2.1.tar.gz` & `tmp/yunbk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yunbk-0.2.1.tar", last modified: Wed May 16 08:02:03 2018, max compression
+gzip compressed data, was "yunbk-0.2.2.tar", last modified: Sat Apr  8 17:21:21 2023, max compression
```

## Comparing `yunbk-0.2.1.tar` & `yunbk-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 08:02:03.000000 yunbk-0.2.1/
--rw-r--r--   0 dantezhu   (501) staff       (20)      219 2018-05-16 08:02:03.000000 yunbk-0.2.1/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      238 2018-05-16 08:01:23.000000 yunbk-0.2.1/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-05-16 08:02:03.000000 yunbk-0.2.1/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      452 2018-05-16 08:01:40.000000 yunbk-0.2.1/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk/
--rw-r--r--   0 dantezhu   (501) staff       (20)       73 2018-05-16 08:01:48.000000 yunbk-0.2.1/yunbk/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk/backend/
--rw-r--r--   0 dantezhu   (501) staff       (20)       23 2014-04-08 14:48:23.000000 yunbk-0.2.1/yunbk/backend/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1746 2018-05-16 07:50:24.000000 yunbk-0.2.1/yunbk/backend/ali_oss.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      355 2018-05-16 07:50:24.000000 yunbk-0.2.1/yunbk/backend/base.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1630 2018-05-16 07:50:24.000000 yunbk-0.2.1/yunbk/backend/ftp.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1127 2018-05-16 07:50:24.000000 yunbk-0.2.1/yunbk/backend/local.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2227 2018-05-16 08:01:04.000000 yunbk-0.2.1/yunbk/backend/sftp.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1465 2017-07-29 02:53:40.000000 yunbk-0.2.1/yunbk/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      109 2018-05-16 08:01:04.000000 yunbk-0.2.1/yunbk/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      388 2018-05-16 08:01:04.000000 yunbk-0.2.1/yunbk/six.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      969 2018-05-16 08:01:04.000000 yunbk-0.2.1/yunbk/utils.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2767 2018-05-16 08:01:04.000000 yunbk-0.2.1/yunbk/yunbk.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-04-08 14:51:49.000000 yunbk-0.2.1/yunbk.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)      219 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       27 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      422 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2018-05-16 08:02:03.000000 yunbk-0.2.1/yunbk.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:21:21.148897 yunbk-0.2.2/
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1074 2014-05-20 07:08:11.000000 yunbk-0.2.2/LICENSE
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:21:21.149197 yunbk-0.2.2/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      238 2018-05-16 08:01:23.000000 yunbk-0.2.2/README.md
+-rw-r--r--   0 dantezhu   (501) staff       (20)      538 2023-04-08 17:21:11.000000 yunbk-0.2.2/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      387 2023-04-08 17:21:21.151499 yunbk-0.2.2/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      452 2023-04-08 17:21:03.000000 yunbk-0.2.2/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:21:21.129468 yunbk-0.2.2/yunbk/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       73 2023-04-08 17:21:08.000000 yunbk-0.2.2/yunbk/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:21:21.147103 yunbk-0.2.2/yunbk/backend/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2014-04-08 14:48:23.000000 yunbk-0.2.2/yunbk/backend/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1746 2018-05-16 07:50:24.000000 yunbk-0.2.2/yunbk/backend/ali_oss.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      355 2018-05-16 07:50:24.000000 yunbk-0.2.2/yunbk/backend/base.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1630 2018-05-16 07:50:24.000000 yunbk-0.2.2/yunbk/backend/ftp.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1127 2018-05-16 07:50:24.000000 yunbk-0.2.2/yunbk/backend/local.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2227 2018-05-16 08:01:04.000000 yunbk-0.2.2/yunbk/backend/sftp.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1465 2017-07-29 02:53:40.000000 yunbk-0.2.2/yunbk/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      109 2018-05-16 08:01:04.000000 yunbk-0.2.2/yunbk/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      388 2018-05-16 08:01:04.000000 yunbk-0.2.2/yunbk/six.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      969 2018-05-16 08:01:04.000000 yunbk-0.2.2/yunbk/utils.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2767 2018-05-16 08:01:04.000000 yunbk-0.2.2/yunbk/yunbk.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:21:21.139385 yunbk-0.2.2/yunbk.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      288 2023-04-08 17:21:21.000000 yunbk-0.2.2/yunbk.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      455 2023-04-08 17:21:21.000000 yunbk-0.2.2/yunbk.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:21:21.000000 yunbk-0.2.2/yunbk.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2014-04-08 14:51:49.000000 yunbk-0.2.2/yunbk.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2023-04-08 17:21:21.000000 yunbk-0.2.2/yunbk.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:21:21.000000 yunbk-0.2.2/yunbk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yunbk-0.2.1/yunbk/backend/ali_oss.py` & `yunbk-0.2.2/yunbk/backend/ali_oss.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/backend/ftp.py` & `yunbk-0.2.2/yunbk/backend/ftp.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/backend/local.py` & `yunbk-0.2.2/yunbk/backend/local.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/backend/sftp.py` & `yunbk-0.2.2/yunbk/backend/sftp.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/constants.py` & `yunbk-0.2.2/yunbk/constants.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/utils.py` & `yunbk-0.2.2/yunbk/utils.py`

 * *Files identical despite different names*

### Comparing `yunbk-0.2.1/yunbk/yunbk.py` & `yunbk-0.2.2/yunbk/yunbk.py`

 * *Files identical despite different names*

