# Comparing `tmp/extotype-0.4.tar.gz` & `tmp/extotype-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extotype-0.4.tar", last modified: Sat Apr  8 21:21:52 2023, max compression
+gzip compressed data, was "extotype-0.5.tar", last modified: Sat Apr  8 21:27:24 2023, max compression
```

## Comparing `extotype-0.4.tar` & `extotype-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:21:52.355516 extotype-0.4/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:21:52.355516 extotype-0.4/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      435 2023-04-08 01:30:33.000000 extotype-0.4/README.md
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:21:52.355516 extotype-0.4/extotype/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1703 2023-04-08 21:20:17.000000 extotype-0.4/extotype/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:21:52.355516 extotype-0.4/extotype/static/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      777 2023-04-08 00:25:09.000000 extotype-0.4/extotype/static/extotype.js
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:21:52.355516 extotype-0.4/extotype/templates/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      214 2023-04-08 00:26:12.000000 extotype-0.4/extotype/templates/search.html
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:21:52.355516 extotype-0.4/extotype.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:21:52.000000 extotype-0.4/extotype.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      257 2023-04-08 21:21:52.000000 extotype-0.4/extotype.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-08 21:21:52.000000 extotype-0.4/extotype.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        7 2023-04-08 21:21:52.000000 extotype-0.4/extotype.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        9 2023-04-08 21:21:52.000000 extotype-0.4/extotype.egg-info/top_level.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-08 21:21:52.355516 extotype-0.4/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      306 2023-04-08 21:21:35.000000 extotype-0.4/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:27:24.279419 extotype-0.5/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:27:24.279419 extotype-0.5/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      435 2023-04-08 01:30:33.000000 extotype-0.5/README.md
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:27:24.279419 extotype-0.5/extotype/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1703 2023-04-08 21:20:17.000000 extotype-0.5/extotype/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:27:24.279419 extotype-0.5/extotype/static/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      777 2023-04-08 00:25:09.000000 extotype-0.5/extotype/static/extotype.js
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:27:24.279419 extotype-0.5/extotype/templates/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      214 2023-04-08 00:26:12.000000 extotype-0.5/extotype/templates/search.html
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:27:24.279419 extotype-0.5/extotype.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:27:24.000000 extotype-0.5/extotype.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      257 2023-04-08 21:27:24.000000 extotype-0.5/extotype.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-08 21:27:24.000000 extotype-0.5/extotype.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       19 2023-04-08 21:27:24.000000 extotype-0.5/extotype.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        9 2023-04-08 21:27:24.000000 extotype-0.5/extotype.egg-info/top_level.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-08 21:27:24.279419 extotype-0.5/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      343 2023-04-08 21:26:56.000000 extotype-0.5/setup.py
```

### Comparing `extotype-0.4/extotype/__init__.py` & `extotype-0.5/extotype/__init__.py`

 * *Files identical despite different names*

### Comparing `extotype-0.4/extotype/static/extotype.js` & `extotype-0.5/extotype/static/extotype.js`

 * *Files identical despite different names*

