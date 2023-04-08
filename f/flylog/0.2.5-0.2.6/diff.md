# Comparing `tmp/flylog-0.2.5.tar.gz` & `tmp/flylog-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flylog-0.2.5.tar", last modified: Fri Apr 12 02:26:17 2019, max compression
+gzip compressed data, was "flylog-0.2.6.tar", last modified: Sat Apr  8 17:31:29 2023, max compression
```

## Comparing `flylog-0.2.5.tar` & `flylog-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:17.000000 flylog-0.2.5/
--rw-rw-rw-   0        0        0      242 2019-04-12 02:26:17.000000 flylog-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      377 2019-04-12 02:24:44.000000 flylog-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog/
--rw-rw-rw-   0        0        0      196 2019-04-12 02:25:28.000000 flylog-0.2.5/flylog/__init__.py
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog/api/
--rw-rw-rw-   0        0        0       23 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/api/__init__.py
--rw-rw-rw-   0        0        0     1090 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/api/client.py
--rw-rw-rw-   0        0        0     1586 2019-04-12 02:25:02.000000 flylog-0.2.5/flylog/api/log_handler.py
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog/bin/
--rw-rw-rw-   0        0        0     1231 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/bin/run_flylog.py
--rw-rw-rw-   0        0        0       81 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/constants.py
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:17.000000 flylog-0.2.5/flylog/server/
--rw-rw-rw-   0        0        0       23 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/__init__.py
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:17.000000 flylog-0.2.5/flylog/server/backends/
--rw-rw-rw-   0        0        0       23 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/backends/__init__.py
--rw-rw-rw-   0        0        0     3851 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/backends/ding.py
--rw-rw-rw-   0        0        0     2372 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/backends/mail.py
--rw-rw-rw-   0        0        0     1146 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/backends/sendcloud.py
--rw-rw-rw-   0        0        0      117 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/log.py
--rw-rw-rw-   0        0        0     3865 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/server.py
--rw-rw-rw-   0        0        0      502 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/six.py
--rw-rw-rw-   0        0        0     1711 2019-04-12 02:24:44.000000 flylog-0.2.5/flylog/server/utils.py
-drwxrwxrwx   0        0        0        0 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/
--rw-rw-rw-   0        0        0      242 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2019-04-12 02:26:16.000000 flylog-0.2.5/flylog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-04-12 02:26:17.000000 flylog-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      458 2019-04-12 02:25:23.000000 flylog-0.2.5/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.804151 flylog-0.2.6/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      280 2023-04-08 17:31:29.804347 flylog-0.2.6/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      377 2019-04-29 10:50:05.000000 flylog-0.2.6/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.781314 flylog-0.2.6/flylog/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      196 2023-04-08 17:31:14.000000 flylog-0.2.6/flylog/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.791397 flylog-0.2.6/flylog/api/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2016-03-24 10:59:40.000000 flylog-0.2.6/flylog/api/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1090 2018-05-16 07:05:00.000000 flylog-0.2.6/flylog/api/client.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1586 2019-04-12 13:54:29.000000 flylog-0.2.6/flylog/api/log_handler.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.792316 flylog-0.2.6/flylog/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)     1231 2018-07-16 15:34:50.000000 flylog-0.2.6/flylog/bin/run_flylog.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       81 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/constants.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.798194 flylog-0.2.6/flylog/server/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/server/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.803377 flylog-0.2.6/flylog/server/backends/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       23 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/server/backends/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3851 2018-05-16 07:01:59.000000 flylog-0.2.6/flylog/server/backends/ding.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2372 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/server/backends/mail.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1146 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/server/backends/sendcloud.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      117 2017-03-31 06:49:56.000000 flylog-0.2.6/flylog/server/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3865 2018-05-16 07:05:00.000000 flylog-0.2.6/flylog/server/server.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      502 2018-05-16 07:05:00.000000 flylog-0.2.6/flylog/server/six.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1711 2018-05-16 07:05:00.000000 flylog-0.2.6/flylog/server/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:31:29.788664 flylog-0.2.6/flylog.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      280 2023-04-08 17:31:29.000000 flylog-0.2.6/flylog.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      603 2023-04-08 17:31:29.000000 flylog-0.2.6/flylog.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:31:29.000000 flylog-0.2.6/flylog.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2017-03-31 06:46:51.000000 flylog-0.2.6/flylog.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)        9 2023-04-08 17:31:29.000000 flylog-0.2.6/flylog.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2023-04-08 17:31:29.000000 flylog-0.2.6/flylog.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      571 2023-04-08 17:31:19.000000 flylog-0.2.6/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      415 2023-04-08 17:31:29.805389 flylog-0.2.6/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      458 2023-04-08 17:31:09.000000 flylog-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flylog-0.2.5/flylog/api/client.py` & `flylog-0.2.6/flylog/api/client.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/api/log_handler.py` & `flylog-0.2.6/flylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/bin/run_flylog.py` & `flylog-0.2.6/flylog/bin/run_flylog.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/server/backends/ding.py` & `flylog-0.2.6/flylog/server/backends/ding.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/server/backends/mail.py` & `flylog-0.2.6/flylog/server/backends/mail.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/server/backends/sendcloud.py` & `flylog-0.2.6/flylog/server/backends/sendcloud.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/server/server.py` & `flylog-0.2.6/flylog/server/server.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog/server/utils.py` & `flylog-0.2.6/flylog/server/utils.py`

 * *Files identical despite different names*

### Comparing `flylog-0.2.5/flylog.egg-info/SOURCES.txt` & `flylog-0.2.6/flylog.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 flylog/__init__.py
 flylog/constants.py
 flylog.egg-info/PKG-INFO
 flylog.egg-info/SOURCES.txt
 flylog.egg-info/dependency_links.txt
 flylog.egg-info/not-zip-safe
 flylog.egg-info/requires.txt
 flylog.egg-info/top_level.txt
-flylog/bin/run_flylog.py
 flylog/api/__init__.py
 flylog/api/client.py
 flylog/api/log_handler.py
+flylog/bin/run_flylog.py
 flylog/server/__init__.py
 flylog/server/log.py
 flylog/server/server.py
 flylog/server/six.py
 flylog/server/utils.py
 flylog/server/backends/__init__.py
 flylog/server/backends/ding.py
```

