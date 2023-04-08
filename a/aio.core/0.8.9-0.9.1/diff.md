# Comparing `tmp/aio.core-0.8.9.tar.gz` & `tmp/aio.core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio.core-0.8.9.tar", last modified: Wed Jun 15 14:26:46 2022, max compression
+gzip compressed data, was "aio.core-0.9.1.tar", last modified: Sun Jul 10 07:18:18 2022, max compression
```

## Comparing `aio.core-0.8.9.tar` & `aio.core-0.9.1.tar`

### file list

```diff
@@ -1,67 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-15 14:26:46.000000 aio.core-0.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-15 14:26:46.712073 aio.core-0.8.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.704073 aio.core-0.8.9/aio/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio/core/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio/core/dev/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/dev/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/dev/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio/core/directory/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio/core/directory/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12965 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/abstract/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/directory/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio/core/event/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/event/executive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/event/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/event/reactive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/log/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/log/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/pipe/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/pipe/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/pipe/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/pipe/abstract/pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/pipe/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/pipe/pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/stream/_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/stream/_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/subprocess/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/subprocess/async_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/subprocess/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/subprocess/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.712073 aio.core-0.8.9/aio/core/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/tasks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16996 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/tasks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:26:46.708073 aio.core-0.8.9/aio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-15 14:26:46.000000 aio.core-0.8.9/aio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-06-15 14:26:46.000000 aio.core-0.8.9/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-15 14:26:46.712073 aio.core-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-06-15 14:26:46.000000 aio.core-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.910404 aio.core-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-10 07:18:18.000000 aio.core-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-07-10 07:18:18.910404 aio.core-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.902404 aio.core-0.9.1/aio/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/dev/debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/dev/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/directory/
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/directory/abstract/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12965 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/abstract/directory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/directory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/directory/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/event/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/event/executive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/event/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/event/reactive.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio/core/log/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/log/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.910404 aio.core-0.9.1/aio/core/pipe/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.910404 aio.core-0.9.1/aio/core/pipe/abstract/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/pipe/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/pipe/abstract/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/pipe/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/pipe/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.910404 aio.core-0.9.1/aio/core/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/subprocess/async_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/subprocess/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/subprocess/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.910404 aio.core-0.9.1/aio/core/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/tasks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16996 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/tasks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 07:18:18.906404 aio.core-0.9.1/aio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-10 07:18:18.000000 aio.core-0.9.1/aio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2022-07-10 07:18:18.000000 aio.core-0.9.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-10 07:18:18.910404 aio.core-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-07-10 07:18:18.000000 aio.core-0.9.1/setup.py
```

### Comparing `aio.core-0.8.9/aio/core/dev/debug.py` & `aio.core-0.9.1/aio/core/dev/debug.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/directory/__init__.py` & `aio.core-0.9.1/aio/core/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/directory/abstract/directory.py` & `aio.core-0.9.1/aio/core/directory/abstract/directory.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/directory/context.py` & `aio.core-0.9.1/aio/core/directory/context.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/directory/directory.py` & `aio.core-0.9.1/aio/core/directory/directory.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/event/executive.py` & `aio.core-0.9.1/aio/core/event/executive.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/event/loader.py` & `aio.core-0.9.1/aio/core/event/loader.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/event/reactive.py` & `aio.core-0.9.1/aio/core/event/reactive.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/__init__.py` & `aio.core-0.9.1/aio/core/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/collections.py` & `aio.core-0.9.1/aio/core/functional/collections.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/decorators.py` & `aio.core-0.9.1/aio/core/functional/decorators.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/generator.py` & `aio.core-0.9.1/aio/core/functional/generator.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/process.py` & `aio.core-0.9.1/aio/core/functional/process.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/functional/utils.py` & `aio.core-0.9.1/aio/core/functional/utils.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/log/logging.py` & `aio.core-0.9.1/aio/core/log/logging.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/pipe/abstract/pipe.py` & `aio.core-0.9.1/aio/core/pipe/abstract/pipe.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/pipe/interface.py` & `aio.core-0.9.1/aio/core/pipe/interface.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/subprocess/async_subprocess.py` & `aio.core-0.9.1/aio/core/subprocess/async_subprocess.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/subprocess/handler.py` & `aio.core-0.9.1/aio/core/subprocess/handler.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/tasks/tasks.py` & `aio.core-0.9.1/aio/core/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio/core/utils.py` & `aio.core-0.9.1/aio/core/utils.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/aio.core.egg-info/SOURCES.txt` & `aio.core-0.9.1/aio.core.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,14 @@
 aio/core/log/__init__.py
 aio/core/log/logging.py
 aio/core/pipe/__init__.py
 aio/core/pipe/interface.py
 aio/core/pipe/pipe.py
 aio/core/pipe/abstract/__init__.py
 aio/core/pipe/abstract/pipe.py
-aio/core/stream/__init__.py
-aio/core/stream/_reader.py
-aio/core/stream/_writer.py
-aio/core/stream/base.py
 aio/core/subprocess/__init__.py
 aio/core/subprocess/async_subprocess.py
 aio/core/subprocess/exceptions.py
 aio/core/subprocess/handler.py
 aio/core/tasks/__init__.py
 aio/core/tasks/exceptions.py
 aio/core/tasks/tasks.py
```

### Comparing `aio.core-0.8.9/backend_shim.py` & `aio.core-0.9.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `aio.core-0.8.9/setup.py` & `aio.core-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 setup(**{
     'author': 'Ryan Northey',
     'author_email': 'ryan@synca.io',
     'description': 'A collection of functional utils for asyncio',
     'install_requires': (
         'abstracts>=0.0.12',
-        'aiofiles',
-        'aiohttp>=3.8.1',
         'orjson',
         'trycast>=0.7.3',
         'types-orjson',
     ),
     'license': 'Apache Software License 2.0',
     'long_description': """
 aio.core
@@ -39,14 +37,13 @@
         'aio.core.directory',
         'aio.core.directory.abstract',
         'aio.core.event',
         'aio.core.functional',
         'aio.core.log',
         'aio.core.pipe',
         'aio.core.pipe.abstract',
-        'aio.core.stream',
         'aio.core.subprocess',
         'aio.core.tasks',
     ),
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/aio.core',
-    'version': '0.8.9',
+    'version': '0.9.1',
 })
```

