# Comparing `tmp/coolfunc-1.0.tar.gz` & `tmp/coolfunc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolfunc-1.0.tar", last modified: Sun Mar 26 13:04:01 2023, max compression
+gzip compressed data, was "coolfunc-1.0.1.tar", last modified: Sat Apr  8 18:36:23 2023, max compression
```

## Comparing `coolfunc-1.0.tar` & `coolfunc-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 coolfunc-1.0/LICENSE
--rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 coolfunc-1.0/README.md
--rw-r--r--   0        0        0       40 2023-03-05 13:34:26.457361 coolfunc-1.0/coolfunc/__init__.py
--rw-r--r--   0        0        0     1694 2023-03-05 13:23:09.230912 coolfunc-1.0/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0      418 2023-03-26 12:49:22.980186 coolfunc-1.0/pyproject.toml
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 coolfunc-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 coolfunc-1.0.1/LICENSE
+-rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 coolfunc-1.0.1/README.md
+-rw-r--r--   0        0        0       40 2023-03-05 13:34:26.457361 coolfunc-1.0.1/coolfunc/__init__.py
+-rw-r--r--   0        0        0     1694 2023-03-05 13:23:09.230912 coolfunc-1.0.1/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0      460 2023-04-08 18:34:43.091346 coolfunc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 coolfunc-1.0.1/PKG-INFO
```

### Comparing `coolfunc-1.0/LICENSE` & `coolfunc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolfunc-1.0/coolfunc/_coolfunc.py` & `coolfunc-1.0.1/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

