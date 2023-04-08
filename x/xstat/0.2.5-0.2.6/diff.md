# Comparing `tmp/xstat-0.2.5.tar.gz` & `tmp/xstat-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xstat-0.2.5.tar", last modified: Sat Jun  2 07:47:08 2018, max compression
+gzip compressed data, was "xstat-0.2.6.tar", last modified: Sat Apr  8 17:20:55 2023, max compression
```

## Comparing `xstat-0.2.5.tar` & `xstat-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-06-02 07:47:08.000000 xstat-0.2.5/
--rw-r--r--   0 dantezhu   (501) staff       (20)      261 2018-06-02 07:47:08.000000 xstat-0.2.5/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)       95 2018-06-02 07:45:21.000000 xstat-0.2.5/README.md
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-06-02 07:47:08.000000 xstat-0.2.5/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      439 2018-06-02 07:46:30.000000 xstat-0.2.5/setup.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat/
--rw-r--r--   0 dantezhu   (501) staff       (20)      335 2018-06-02 07:46:35.000000 xstat-0.2.5/xstat/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       43 2018-06-02 07:45:21.000000 xstat-0.2.5/xstat/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1882 2018-06-02 07:46:00.000000 xstat-0.2.5/xstat/django_stat.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1661 2018-06-02 07:45:21.000000 xstat-0.2.5/xstat/flask_stat.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       77 2018-06-02 07:45:21.000000 xstat-0.2.5/xstat/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1690 2018-06-02 07:45:21.000000 xstat-0.2.5/xstat/maple_stat.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      309 2018-06-02 07:45:21.000000 xstat-0.2.5/xstat/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      261 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)        7 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)      288 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2018-06-02 07:47:08.000000 xstat-0.2.5/xstat.egg-info/top_level.txt
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:20:55.849929 xstat-0.2.6/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      290 2023-04-08 17:20:55.850068 xstat-0.2.6/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)       95 2018-05-16 07:36:48.000000 xstat-0.2.6/README.md
+-rw-r--r--   0 dantezhu   (501) staff       (20)      531 2023-04-08 17:20:46.000000 xstat-0.2.6/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      381 2023-04-08 17:20:55.850704 xstat-0.2.6/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      439 2023-04-08 17:20:35.000000 xstat-0.2.6/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:20:55.846967 xstat-0.2.6/xstat/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      335 2023-04-08 17:20:43.000000 xstat-0.2.6/xstat/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       43 2015-04-17 01:55:40.000000 xstat-0.2.6/xstat/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1882 2019-01-09 01:44:11.000000 xstat-0.2.6/xstat/django_stat.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1661 2018-05-16 07:29:46.000000 xstat-0.2.6/xstat/flask_stat.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       77 2015-04-17 01:54:00.000000 xstat-0.2.6/xstat/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1690 2018-05-16 07:29:46.000000 xstat-0.2.6/xstat/maple_stat.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      309 2018-05-16 07:29:46.000000 xstat-0.2.6/xstat/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:20:55.849463 xstat-0.2.6/xstat.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      290 2023-04-08 17:20:55.000000 xstat-0.2.6/xstat.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      313 2023-04-08 17:20:55.000000 xstat-0.2.6/xstat.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:20:55.000000 xstat-0.2.6/xstat.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2023-04-08 17:20:55.000000 xstat-0.2.6/xstat.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2023-04-08 17:20:55.000000 xstat-0.2.6/xstat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xstat-0.2.5/xstat/django_stat.py` & `xstat-0.2.6/xstat/django_stat.py`

 * *Files identical despite different names*

### Comparing `xstat-0.2.5/xstat/flask_stat.py` & `xstat-0.2.6/xstat/flask_stat.py`

 * *Files identical despite different names*

### Comparing `xstat-0.2.5/xstat/maple_stat.py` & `xstat-0.2.6/xstat/maple_stat.py`

 * *Files identical despite different names*

