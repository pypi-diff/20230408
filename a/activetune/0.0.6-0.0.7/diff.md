# Comparing `tmp/activetune-0.0.6.tar.gz` & `tmp/activetune-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activetune-0.0.6.tar", last modified: Thu Apr  6 14:58:35 2023, max compression
+gzip compressed data, was "activetune-0.0.7.tar", last modified: Sat Apr  8 21:49:21 2023, max compression
```

## Comparing `activetune-0.0.6.tar` & `activetune-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:35.382501 activetune-0.0.6/
--rw-rw-rw-   0        0        0       89 2023-04-06 14:58:35.382501 activetune-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:35.382501 activetune-0.0.6/activetune/
--rw-rw-rw-   0        0        0       47 2023-04-06 14:58:04.000000 activetune-0.0.6/activetune/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-04-06 14:57:42.000000 activetune-0.0.6/activetune/api.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:58:35.382501 activetune-0.0.6/activetune.egg-info/
--rw-rw-rw-   0        0        0       89 2023-04-06 14:58:35.000000 activetune-0.0.6/activetune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-06 14:58:35.000000 activetune-0.0.6/activetune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:58:35.000000 activetune-0.0.6/activetune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.6/activetune.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-06 14:58:35.000000 activetune-0.0.6/activetune.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-06 14:58:35.000000 activetune-0.0.6/activetune.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 14:58:35.382501 activetune-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      350 2023-04-06 14:58:08.000000 activetune-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/
+-rw-rw-rw-   0        0        0       89 2023-04-08 21:49:21.719337 activetune-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/activetune/
+-rw-rw-rw-   0        0        0       47 2023-04-08 21:48:44.000000 activetune-0.0.7/activetune/__init__.py
+-rw-rw-rw-   0        0        0     2782 2023-04-08 21:47:01.000000 activetune-0.0.7/activetune/api.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:49:21.719337 activetune-0.0.7/activetune.egg-info/
+-rw-rw-rw-   0        0        0       89 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.7/activetune.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 21:49:21.000000 activetune-0.0.7/activetune.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 21:49:21.719337 activetune-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      350 2023-04-08 21:48:55.000000 activetune-0.0.7/setup.py
```

### Comparing `activetune-0.0.6/README.md` & `activetune-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `activetune-0.0.6/activetune/api.py` & `activetune-0.0.7/activetune/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         input: str = "",
         model_output: str = "",
         model_id: str = "",
         expected_output: str = "",
         feedback=0,
         meta={},
     ):
-        return requests.get(
+        return requests.post(
             self.url + "/api/add_sample",
-            {
+            json={
                 "token": self.token,
                 "dataset_id": dataset_id,
                 "input": input,
                 "model_output": model_output,
                 "model_id": model_id,
                 "expected_output": expected_output,
                 "feedback": feedback,
```

