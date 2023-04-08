# Comparing `tmp/jsonm-1.1.1.tar.gz` & `tmp/jsonm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonm-1.1.1.tar", last modified: Wed May 16 06:19:28 2018, max compression
+gzip compressed data, was "jsonm-1.1.2.tar", last modified: Sat Apr  8 17:31:47 2023, max compression
```

## Comparing `jsonm-1.1.1.tar` & `jsonm-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 06:19:28.000000 jsonm-1.1.1/
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm/
--rw-r--r--   0 dantezhu   (501) staff       (20)      314 2018-05-16 06:19:12.000000 jsonm-1.1.1/jsonm/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2139 2016-12-14 11:12:58.000000 jsonm-1.1.1/jsonm/application.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm/contrib/
--rw-r--r--   0 dantezhu   (501) staff       (20)       70 2016-02-19 09:54:57.000000 jsonm-1.1.1/jsonm/contrib/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1043 2016-02-19 09:55:21.000000 jsonm-1.1.1/jsonm/contrib/datetime_models.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      553 2015-03-11 09:58:18.000000 jsonm-1.1.1/jsonm/fields.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2302 2018-05-16 06:18:06.000000 jsonm-1.1.1/jsonm/model.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      112 2016-02-19 09:11:42.000000 jsonm-1.1.1/jsonm/vals.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      232 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      277 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2018-05-16 06:19:28.000000 jsonm-1.1.1/jsonm.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      232 2018-05-16 06:19:28.000000 jsonm-1.1.1/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      381 2018-05-16 06:18:06.000000 jsonm-1.1.1/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-05-16 06:19:28.000000 jsonm-1.1.1/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      376 2018-05-16 06:19:06.000000 jsonm-1.1.1/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:47.795684 jsonm-1.1.2/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      261 2023-04-08 17:31:47.796403 jsonm-1.1.2/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      381 2018-05-16 06:18:06.000000 jsonm-1.1.2/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:47.790299 jsonm-1.1.2/jsonm/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      314 2023-04-08 17:31:29.000000 jsonm-1.1.2/jsonm/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2139 2016-12-14 11:12:58.000000 jsonm-1.1.2/jsonm/application.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:47.794794 jsonm-1.1.2/jsonm/contrib/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       70 2016-02-19 09:54:57.000000 jsonm-1.1.2/jsonm/contrib/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1043 2016-02-19 09:55:21.000000 jsonm-1.1.2/jsonm/contrib/datetime_models.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      553 2015-03-11 09:58:18.000000 jsonm-1.1.2/jsonm/fields.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2302 2018-05-16 06:18:06.000000 jsonm-1.1.2/jsonm/model.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      112 2016-02-19 09:11:42.000000 jsonm-1.1.2/jsonm/vals.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:47.793027 jsonm-1.1.2/jsonm.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      261 2023-04-08 17:31:47.000000 jsonm-1.1.2/jsonm.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      302 2023-04-08 17:31:47.000000 jsonm-1.1.2/jsonm.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:31:47.000000 jsonm-1.1.2/jsonm.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:31:47.000000 jsonm-1.1.2/jsonm.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      494 2023-04-08 17:31:38.000000 jsonm-1.1.2/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      346 2023-04-08 17:31:47.801284 jsonm-1.1.2/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      376 2023-04-08 17:31:24.000000 jsonm-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsonm-1.1.1/jsonm/application.py` & `jsonm-1.1.2/jsonm/application.py`

 * *Files identical despite different names*

### Comparing `jsonm-1.1.1/jsonm/contrib/datetime_models.py` & `jsonm-1.1.2/jsonm/contrib/datetime_models.py`

 * *Files identical despite different names*

### Comparing `jsonm-1.1.1/jsonm/fields.py` & `jsonm-1.1.2/jsonm/fields.py`

 * *Files identical despite different names*

### Comparing `jsonm-1.1.1/jsonm/model.py` & `jsonm-1.1.2/jsonm/model.py`

 * *Files identical despite different names*

