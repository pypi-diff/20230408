# Comparing `tmp/danidisp-0.0.4.tar.gz` & `tmp/danidisp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danidisp-0.0.4.tar", last modified: Wed Mar 29 13:35:48 2023, max compression
+gzip compressed data, was "danidisp-0.0.5.tar", last modified: Sat Apr  8 18:06:22 2023, max compression
```

## Comparing `danidisp-0.0.4.tar` & `danidisp-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-03-29 13:35:48.248874 danidisp-0.0.4/
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1096 2023-03-29 13:33:14.000000 danidisp-0.0.4/LICENSE
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      411 2023-03-29 13:35:48.240716 danidisp-0.0.4/PKG-INFO
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      462 2023-03-29 13:33:14.000000 danidisp-0.0.4/README.md
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)       38 2023-03-29 13:35:48.248874 danidisp-0.0.4/setup.cfg
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      504 2023-03-29 13:31:53.000000 danidisp-0.0.4/setup.py
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-03-29 13:35:47.786368 danidisp-0.0.4/src/
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-03-29 13:35:48.148570 danidisp-0.0.4/src/danidisp.egg-info/
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      411 2023-03-29 13:35:46.000000 danidisp-0.0.4/src/danidisp.egg-info/PKG-INFO
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      186 2023-03-29 13:35:46.000000 danidisp-0.0.4/src/danidisp.egg-info/SOURCES.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        1 2023-03-29 13:35:46.000000 danidisp-0.0.4/src/danidisp.egg-info/dependency_links.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        9 2023-03-29 13:35:46.000000 danidisp-0.0.4/src/danidisp.egg-info/top_level.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      208 2023-03-29 13:29:56.000000 danidisp-0.0.4/src/danidisp.py
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-04-08 18:06:22.826909 danidisp-0.0.5/
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1096 2023-03-29 13:33:14.000000 danidisp-0.0.5/LICENSE
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      478 2023-04-08 18:06:22.819243 danidisp-0.0.5/PKG-INFO
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      689 2023-03-29 13:43:30.000000 danidisp-0.0.5/README.md
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)       38 2023-04-08 18:06:22.826909 danidisp-0.0.5/setup.cfg
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      572 2023-04-08 18:06:14.000000 danidisp-0.0.5/setup.py
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-04-08 18:06:22.430815 danidisp-0.0.5/src/
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2023-04-08 18:06:22.752241 danidisp-0.0.5/src/danidisp.egg-info/
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      478 2023-04-08 18:06:20.000000 danidisp-0.0.5/src/danidisp.egg-info/PKG-INFO
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      186 2023-04-08 18:06:20.000000 danidisp-0.0.5/src/danidisp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        1 2023-04-08 18:06:20.000000 danidisp-0.0.5/src/danidisp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        9 2023-04-08 18:06:20.000000 danidisp-0.0.5/src/danidisp.egg-info/top_level.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1285 2023-04-08 18:04:11.000000 danidisp-0.0.5/src/danidisp.py
```

### Comparing `danidisp-0.0.4/LICENSE` & `danidisp-0.0.5/LICENSE`

 * *Files identical despite different names*

