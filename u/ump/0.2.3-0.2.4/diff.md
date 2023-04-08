# Comparing `tmp/ump-0.2.3.tar.gz` & `tmp/ump-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ump-0.2.3.tar", last modified: Tue Jul 31 06:08:48 2018, max compression
+gzip compressed data, was "ump-0.2.4.tar", last modified: Sat Apr  8 17:17:59 2023, max compression
```

## Comparing `ump-0.2.3.tar` & `ump-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-31 06:08:48.000000 ump-0.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      214 2018-07-31 06:08:48.000000 ump-0.2.3/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-07-31 06:08:48.000000 ump-0.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      487 2018-07-31 06:08:20.000000 ump-0.2.3/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-31 06:08:48.000000 ump-0.2.3/ump/
--rw-r--r--   0 dantezhu   (501) staff       (20)      218 2018-07-31 06:08:20.000000 ump-0.2.3/ump/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      284 2018-07-31 06:08:20.000000 ump-0.2.3/ump/bill.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-31 06:08:48.000000 ump-0.2.3/ump/bin/
--rw-r--r--   0 dantezhu   (501) staff       (20)      930 2018-07-31 06:08:20.000000 ump-0.2.3/ump/bin/umpctl
--rw-r--r--   0 dantezhu   (501) staff       (20)     1391 2018-07-31 06:08:20.000000 ump-0.2.3/ump/checker.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1728 2018-07-31 06:08:20.000000 ump-0.2.3/ump/cleaner.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      414 2018-07-31 06:08:20.000000 ump-0.2.3/ump/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       67 2018-07-31 06:08:20.000000 ump-0.2.3/ump/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7138 2018-07-31 06:08:20.000000 ump-0.2.3/ump/reader.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      542 2018-07-31 06:08:20.000000 ump-0.2.3/ump/six.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      658 2018-07-31 06:08:20.000000 ump-0.2.3/ump/uploader.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      508 2018-07-31 06:08:20.000000 ump-0.2.3/ump/utils.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     6762 2018-07-31 06:08:20.000000 ump-0.2.3/ump/worker.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2260 2018-07-31 06:08:20.000000 ump-0.2.3/ump/writer.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      214 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      351 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       32 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        4 2018-07-31 06:08:48.000000 ump-0.2.3/ump.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:59.448498 ump-0.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      259 2023-04-08 17:17:59.448727 ump-0.2.4/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      575 2023-04-08 17:17:49.000000 ump-0.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      413 2023-04-08 17:17:59.449799 ump-0.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      487 2023-04-08 17:17:35.000000 ump-0.2.4/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:59.441923 ump-0.2.4/ump/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      218 2023-04-08 17:17:45.000000 ump-0.2.4/ump/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      284 2018-01-29 14:37:51.000000 ump-0.2.4/ump/bill.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:59.447733 ump-0.2.4/ump/bin/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      930 2018-05-17 03:16:02.000000 ump-0.2.4/ump/bin/umpctl
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1391 2018-05-17 03:16:02.000000 ump-0.2.4/ump/checker.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1728 2018-05-17 03:16:02.000000 ump-0.2.4/ump/cleaner.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      414 2018-01-29 14:37:51.000000 ump-0.2.4/ump/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       67 2018-01-23 14:10:07.000000 ump-0.2.4/ump/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7138 2018-05-17 03:23:26.000000 ump-0.2.4/ump/reader.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      542 2018-05-17 03:16:02.000000 ump-0.2.4/ump/six.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      658 2018-01-23 14:10:07.000000 ump-0.2.4/ump/uploader.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      508 2018-05-17 03:16:02.000000 ump-0.2.4/ump/utils.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6762 2018-05-17 03:16:02.000000 ump-0.2.4/ump/worker.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2260 2018-07-31 14:41:32.000000 ump-0.2.4/ump/writer.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:17:59.447103 ump-0.2.4/ump.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      259 2023-04-08 17:17:59.000000 ump-0.2.4/ump.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      376 2023-04-08 17:17:59.000000 ump-0.2.4/ump.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:17:59.000000 ump-0.2.4/ump.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-01-23 14:10:26.000000 ump-0.2.4/ump.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       32 2023-04-08 17:17:59.000000 ump-0.2.4/ump.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        4 2023-04-08 17:17:59.000000 ump-0.2.4/ump.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ump-0.2.3/ump/bin/umpctl` & `ump-0.2.4/ump/bin/umpctl`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/checker.py` & `ump-0.2.4/ump/checker.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/cleaner.py` & `ump-0.2.4/ump/cleaner.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/reader.py` & `ump-0.2.4/ump/reader.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/six.py` & `ump-0.2.4/ump/six.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/uploader.py` & `ump-0.2.4/ump/uploader.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/worker.py` & `ump-0.2.4/ump/worker.py`

 * *Files identical despite different names*

### Comparing `ump-0.2.3/ump/writer.py` & `ump-0.2.4/ump/writer.py`

 * *Files identical despite different names*

