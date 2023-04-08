# Comparing `tmp/vmklib-1.8.0.tar.gz` & `tmp/vmklib-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmklib-1.8.0.tar", last modified: Fri Apr  7 23:32:13 2023, max compression
+gzip compressed data, was "vmklib-1.8.1.tar", last modified: Sat Apr  8 01:24:18 2023, max compression
```

## Comparing `vmklib-1.8.0.tar` & `vmklib-1.8.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 23:30:05.000000 vmklib-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-07 23:32:13.945634 vmklib-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-07 23:30:05.000000 vmklib-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-07 23:30:05.000000 vmklib-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:32:13.945634 vmklib-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-07 23:30:05.000000 vmklib-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.941634 vmklib-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-07 23:30:05.000000 vmklib-1.8.0/tests/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.941634 vmklib-1.8.0/vmklib/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/conf.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/data/edit_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/data/fresh_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/data/header.mk
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/datazen.mk
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/functions.mk
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/grip.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/data/lib_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/lib_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/data/lib_tasks/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-07 23:30:54.000000 vmklib-1.8.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/lib_tasks/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/python/build.mk
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/python/docs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/python/pypi.mk
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/python/upload.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/python.mk
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/time.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/venv.mk
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/vmklib.mk
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/data/yaml.mk
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/tasks/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/mixins/concrete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/tasks/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.945634 vmklib-1.8.0/vmklib/tasks/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/datazen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/python/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-07 23:30:05.000000 vmklib-1.8.0/vmklib/tasks/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:32:13.941634 vmklib-1.8.0/vmklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 23:32:13.000000 vmklib-1.8.0/vmklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 01:22:01.000000 vmklib-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-08 01:24:18.800661 vmklib-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-08 01:22:01.000000 vmklib-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-08 01:22:01.000000 vmklib-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 01:24:18.800661 vmklib-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-08 01:22:01.000000 vmklib-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.788661 vmklib-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-08 01:22:01.000000 vmklib-1.8.1/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.792661 vmklib-1.8.1/vmklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/conf.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/edit_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/fresh_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/header.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/datazen.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/functions.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/grip.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/lib_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/lib_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-08 01:22:12.000000 vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/lib_tasks/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/build.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/docs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/pypi.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/upload.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/time.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/venv.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/vmklib.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/yaml.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/tasks/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/mixins/concrete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/vmklib/tasks/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/vmklib/tasks/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/datazen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.792661 vmklib-1.8.1/vmklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/top_level.txt
```

### Comparing `vmklib-1.8.0/LICENSE` & `vmklib-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/PKG-INFO` & `vmklib-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -46,19 +46,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6fdb7522a28ac67fae20b5b157dcf716
+    hash=86cb90c0ad730eedd704cb4110084afd
     =====================================
 -->
 
-# vmklib ([1.8.0](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
```

### Comparing `vmklib-1.8.0/README.md` & `vmklib-1.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6fdb7522a28ac67fae20b5b157dcf716
+    hash=86cb90c0ad730eedd704cb4110084afd
     =====================================
 -->
 
-# vmklib ([1.8.0](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
```

### Comparing `vmklib-1.8.0/pyproject.toml` & `vmklib-1.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vmklib"
-version = "1.8.0"
+version = "1.8.1"
 description = "Simplify project workflows by standardizing use of GNU Make."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
   "workflow",
   "tool",
@@ -34,20 +34,13 @@
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
-  "pylint",
-  "flake8",
-  "pytest",
-  "pytest-cov",
-  "mypy",
-  "black",
-  "isort",
   "pytest-asyncio",
   "setuptools-wrapper"
 ]
 
 [project.scripts]
 mk = "vmklib.entry:main"
```

### Comparing `vmklib-1.8.0/setup.py` & `vmklib-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/tests/test_entry.py` & `vmklib-1.8.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/app.py` & `vmklib-1.8.1/vmklib/app.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/conf.mk` & `vmklib-1.8.1/vmklib/data/conf.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/data/header.mk` & `vmklib-1.8.1/vmklib/data/data/header.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/datazen.mk` & `vmklib-1.8.1/vmklib/data/datazen.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/functions.mk` & `vmklib-1.8.1/vmklib/data/functions.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/grip.mk` & `vmklib-1.8.1/vmklib/data/grip.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc` & `vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr  7 23:30:05 2023 UTC, .py size: 2374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7da7 3064 4609 0000  U.......}.0dF...
+00000000: 550d 0d0a 0000 0000 b9c1 3064 4609 0000  U.........0dF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0f  m.Z...d.d.l.m.Z.
@@ -68,15 +68,15 @@
 00000430: 7c03 8304 7d05 716e 7c05 5300 2908 7a26  |...}.qn|.S.).z&
 00000440: 5265 6769 7374 6572 2070 6163 6b61 6765  Register package
 00000450: 2074 6173 6b73 2074 6f20 7468 6520 6d61   tasks to the ma
 00000460: 6e61 6765 722e da05 6275 696c 6429 0472  nager...build).r
 00000470: 1f00 0000 da04 7665 6e76 720a 0000 00da  ......venvr.....
 00000480: 0470 726f 6ada 0670 7974 686f 6e29 025a  .proj..python).Z
 00000490: 085f 5f64 6972 735f 5f5a 095f 5f66 696c  .__dirs__Z.__fil
-000004a0: 6573 5f5f da04 6661 696c 7a0b 766d 6b6c  es__..failz.vmkl
+000004a0: 6573 5f5f 5a04 6661 696c 7a0b 766d 6b6c  es__Z.failz.vmkl
 000004b0: 6962 2e69 6e69 7454 2910 da08 6a6f 696e  ib.initT)...join
 000004c0: 7061 7468 720b 0000 0072 0a00 0000 7209  pathr....r....r.
 000004d0: 0000 0072 0c00 0000 7207 0000 00da 0d72  ...r....r......r
 000004e0: 6567 6973 7465 725f 7665 6e76 da14 7265  egister_venv..re
 000004f0: 6769 7374 6572 5f70 7974 686f 6e5f 6c69  gister_python_li
 00000500: 6e74 da17 7265 6769 7374 6572 5f70 7974  nt..register_pyt
 00000510: 686f 6e5f 7061 636b 6167 65da 1472 6567  hon_package..reg
@@ -94,41 +94,41 @@
 000005d0: 6c74 da03 6465 7072 1000 0000 7210 0000  lt..depr....r...
 000005e0: 0072 1400 0000 7209 0000 0023 0000 0073  .r....r....#...s
 000005f0: 3000 0000 000c 0801 0601 0601 08fc 0406  0...............
 00000600: 0cf9 060b 0e03 1203 0402 0201 0201 0201  ................
 00000610: 0201 0201 0201 0201 0201 0201 02f6 080c  ................
 00000620: 0401 1002 7209 0000 004e 2928 7219 0000  ....r....N)(r...
 00000630: 00da 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
-00000640: 0674 7970 696e 6772 0300 0000 5a0d 7663  .typingr....Z.vc
+00000640: 0674 7970 696e 6772 0300 0000 da0d 7663  .typingr......vc
 00000650: 6f72 656c 6962 2e74 6173 6b72 0400 0000  orelib.taskr....
 00000660: 7205 0000 0072 0600 0000 5a19 7663 6f72  r....r....Z.vcor
 00000670: 656c 6962 2e74 6173 6b2e 6469 6374 2e6d  elib.task.dict.m
 00000680: 656c 6465 7272 0700 0000 da15 7663 6f72  elderr......vcor
 00000690: 656c 6962 2e74 6173 6b2e 6d61 6e61 6765  elib.task.manage
-000006a0: 7272 0800 0000 da11 766d 6b6c 6962 2e74  rr......vmklib.t
-000006b0: 6173 6b73 2e6e 6f64 6572 0900 0000 722e  asks.noder....r.
+000006a0: 7272 0800 0000 5a11 766d 6b6c 6962 2e74  rr....Z.vmklib.t
+000006b0: 6173 6b73 2e6e 6f64 6572 0900 0000 722d  asks.noder....r-
 000006c0: 0000 005a 1376 6d6b 6c69 622e 7461 736b  ...Z.vmklib.task
 000006d0: 732e 7079 7468 6f6e 720a 0000 0072 0b00  s.pythonr....r..
 000006e0: 0000 5a19 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
-000006f0: 2e70 7974 686f 6e2e 6275 696c 6472 2900  .python.buildr).
+000006f0: 2e70 7974 686f 6e2e 6275 696c 6472 2800  .python.buildr(.
 00000700: 0000 5a1b 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
 00000710: 2e70 7974 686f 6e2e 6461 7461 7a65 6e72  .python.datazenr
-00000720: 2c00 0000 5a18 766d 6b6c 6962 2e74 6173  ,...Z.vmklib.tas
-00000730: 6b73 2e70 7974 686f 6e2e 646f 6373 722d  ks.python.docsr-
+00000720: 2b00 0000 5a18 766d 6b6c 6962 2e74 6173  +...Z.vmklib.tas
+00000730: 6b73 2e70 7974 686f 6e2e 646f 6373 722c  ks.python.docsr,
 00000740: 0000 005a 1876 6d6b 6c69 622e 7461 736b  ...Z.vmklib.task
-00000750: 732e 7079 7468 6f6e 2e6c 696e 7472 2600  s.python.lintr&.
+00000750: 732e 7079 7468 6f6e 2e6c 696e 7472 2500  s.python.lintr%.
 00000760: 0000 5a1b 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
 00000770: 2e70 7974 686f 6e2e 7061 636b 6167 6572  .python.packager
-00000780: 2700 0000 5a16 766d 6b6c 6962 2e74 6173  '...Z.vmklib.tas
-00000790: 6b73 2e70 7974 686f 6e2e 7361 722a 0000  ks.python.sar*..
+00000780: 2600 0000 5a16 766d 6b6c 6962 2e74 6173  &...Z.vmklib.tas
+00000790: 6b73 2e70 7974 686f 6e2e 7361 7229 0000  ks.python.sar)..
 000007a0: 005a 1876 6d6b 6c69 622e 7461 736b 732e  .Z.vmklib.tasks.
-000007b0: 7079 7468 6f6e 2e74 6573 7472 2b00 0000  python.testr+...
+000007b0: 7079 7468 6f6e 2e74 6573 7472 2a00 0000  python.testr*...
 000007c0: 5a18 766d 6b6c 6962 2e74 6173 6b73 2e70  Z.vmklib.tasks.p
-000007d0: 7974 686f 6e2e 7961 6d6c 7228 0000 005a  ython.yamlr(...Z
+000007d0: 7974 686f 6e2e 7961 6d6c 7227 0000 005a  ython.yamlr'...Z
 000007e0: 1176 6d6b 6c69 622e 7461 736b 732e 7665  .vmklib.tasks.ve
-000007f0: 6e76 7225 0000 0072 0c00 0000 da03 7374  nvr%...r......st
+000007f0: 6e76 7224 0000 0072 0c00 0000 da03 7374  nvr$...r......st
 00000800: 7272 1a00 0000 7210 0000 0072 1000 0000  rr....r....r....
 00000810: 7210 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
 00000820: 756c 653e 0100 0000 732e 0000 0004 050c  ule>....s.......
 00000830: 010c 0314 010c 010c 030c 0110 010c 010c  ................
 00000840: 010c 010c 010c 010c 010c 010c 010c 0310  ................
 00000850: 0802 0102 0102 010a 0102 fb              ...........
```

### Comparing `vmklib-1.8.0/vmklib/data/lib_tasks/conf.py` & `vmklib-1.8.1/vmklib/data/lib_tasks/conf.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/python/build.mk` & `vmklib-1.8.1/vmklib/data/python/build.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/python/docs.mk` & `vmklib-1.8.1/vmklib/data/python/docs.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/python/pypi.mk` & `vmklib-1.8.1/vmklib/data/python/pypi.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/python/upload.mk` & `vmklib-1.8.1/vmklib/data/python/upload.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/python.mk` & `vmklib-1.8.1/vmklib/data/python.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/time.mk` & `vmklib-1.8.1/vmklib/data/time.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/venv.mk` & `vmklib-1.8.1/vmklib/data/venv.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/data/vmklib.mk` & `vmklib-1.8.1/vmklib/data/vmklib.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/entry.py` & `vmklib-1.8.1/vmklib/entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/resources.py` & `vmklib-1.8.1/vmklib/resources.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/args.py` & `vmklib-1.8.1/vmklib/tasks/args.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/mixins/concrete.py` & `vmklib-1.8.1/vmklib/tasks/mixins/concrete.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/node/__init__.py` & `vmklib-1.8.1/vmklib/tasks/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/__init__.py` & `vmklib-1.8.1/vmklib/tasks/python/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/build.py` & `vmklib-1.8.1/vmklib/tasks/python/build.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/datazen.py` & `vmklib-1.8.1/vmklib/tasks/python/datazen.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/docs.py` & `vmklib-1.8.1/vmklib/tasks/python/docs.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/lint.py` & `vmklib-1.8.1/vmklib/tasks/python/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return list(str(x) for x in filter(lambda x: x.exists(), sources))
 
     async def run(self, inbox: Inbox, outbox: Outbox, *args, **kwargs) -> bool:
         """Run a Python linter."""
 
         cwd: Path = args[0]
         project: str = args[1]
-        linter: str = kwargs["linter"]
+        linter: str = kwargs.get("package", kwargs.get("linter", "UNKNOWN"))
 
         return await self.exec(
             str(inbox["venv"]["venv{python_version}"]["bin"].joinpath(linter)),
             *args[2:],
             # Get extra arguments from the environment.
             *environ_fallback_split(
                 "PY_LINT_" + linter.upper() + "_EXTRA_ARGS", **kwargs
@@ -65,21 +65,21 @@
 
     # A target ensuring that linter packages are installed.
     for kind in ["install", "upgrade"]:
         manager.register(
             Phony(prefix + f"lint-{kind}"),
             [
                 f"{prefix}{kind}-{x}"
-                for x in ["pylint", "flake8", "black", "isort", "ruff", "mypy"]
+                for x in ["pylint", "flake8", "black", "ruff", "mypy", "isort"]
             ],
         )
 
     manager.register(
-        PythonLinter(prefix + "lint-{linter}", cwd, project),
-        [prefix + "lint-install"],
+        PythonLinter(prefix + "lint-{package}", cwd, project),
+        [prefix + "install-{package}"],
     )
 
     line_length = ["--line-length", str(substitutions.get("line_length", 79))]
 
     isort_args = line_length + [
         "--profile",
         substitutions.get("isort_profile", "black"),
@@ -93,51 +93,51 @@
             prefix + "format-check-isort",
             cwd,
             project,
             "--check-only",
             *isort_args,
             linter="isort",
         ),
-        [],
+        [f"{prefix}install-isort"],
     )
 
     manager.register(
         PythonLinter(
             prefix + "format-isort",
             cwd,
             project,
             *isort_args,
             linter="isort",
         ),
-        [],
+        [f"{prefix}install-isort"],
     )
 
     manager.register(
         PythonLinter(
             prefix + "format-check-black",
             cwd,
             project,
             "--check",
             *line_length,
             linter="black",
         ),
-        [],
+        [f"{prefix}install-black"],
     )
 
     manager.register(
         PythonLinter(
             prefix + "format-black",
             cwd,
             project,
             *line_length,
             linter="black",
         ),
         # Depend on 'isort' so that we don't format multiple files at the same
         # time.
-        [prefix + "format-isort"],
+        [f"{prefix}install-black", prefix + "format-isort"],
     )
 
     manager.register(
         Phony(prefix + "format-check"),
         [prefix + "format-check-black", prefix + "format-check-isort"],
     )
     manager.register(
```

### Comparing `vmklib-1.8.0/vmklib/tasks/python/package.py` & `vmklib-1.8.1/vmklib/tasks/python/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from typing import Dict
 
 # third-party
 from vcorelib.task import Inbox, Outbox, Phony
 from vcorelib.task.manager import TaskManager
 from vcorelib.task.subprocess.run import SubprocessLogMixin
 
-from vmklib.tasks.mixins.concrete import ConcreteOnceMixin
-
 # internal
+from vmklib.tasks.mixins.concrete import ConcreteOnceMixin
 from vmklib.tasks.python import PREFIX
 
 
 class PythonPackage(ConcreteOnceMixin, SubprocessLogMixin):
     """A task for installing a single Python package."""
 
     default_requirements = {"venv", "vmklib.init"}
```

### Comparing `vmklib-1.8.0/vmklib/tasks/python/sa.py` & `vmklib-1.8.1/vmklib/tasks/python/sa.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         PythonLinter(
             PREFIX + "sa-types-init",
             cwd,
             project,
             ignore_errors=True,
             linter="mypy",
         ),
-        [],
+        [PREFIX + "install-mypy"],
     )
     manager.register(
         PythonLinter(
             PREFIX + "sa-types",
             cwd,
             project,
             "--install-types",
```

### Comparing `vmklib-1.8.0/vmklib/tasks/python/test.py` & `vmklib-1.8.1/vmklib/tasks/python/test.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/python/yaml.py` & `vmklib-1.8.1/vmklib/tasks/python/yaml.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib/tasks/venv.py` & `vmklib-1.8.1/vmklib/tasks/venv.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.0/vmklib.egg-info/PKG-INFO` & `vmklib-1.8.1/vmklib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -46,19 +46,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6fdb7522a28ac67fae20b5b157dcf716
+    hash=86cb90c0ad730eedd704cb4110084afd
     =====================================
 -->
 
-# vmklib ([1.8.0](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
```

### Comparing `vmklib-1.8.0/vmklib.egg-info/SOURCES.txt` & `vmklib-1.8.1/vmklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

