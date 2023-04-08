# Comparing `tmp/ads-async-0.3.0.tar.gz` & `tmp/ads-async-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ads-async-0.3.0.tar", last modified: Wed Sep 14 18:24:20 2022, max compression
+gzip compressed data, was "ads-async-0.3.1.tar", last modified: Fri Apr  7 17:33:12 2023, max compression
```

## Comparing `ads-async-0.3.0.tar` & `ads-async-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,77 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.234599 ads-async-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2022-09-14 18:24:05.000000 ads-async-0.3.0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3038 2022-09-14 18:24:05.000000 ads-async-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-09-14 18:24:05.000000 ads-async-0.3.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2022-09-14 18:24:05.000000 ads-async-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1751 2022-09-14 18:24:20.234599 ads-async-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1367 2022-09-14 18:24:05.000000 ads-async-0.3.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.234599 ads-async-0.3.0/ads_async/
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-09-14 18:24:20.234599 ads-async-0.3.0/ads_async/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.230597 ads-async-0.3.0/ads_async/asyncio/
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/asyncio/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32521 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/asyncio/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6849 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/asyncio/server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6429 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/asyncio/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.230597 ads-async-0.3.0/ads_async/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2470 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/ads_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6095 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/download.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3368 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/get.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2456 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3455 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3992 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/route.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6162 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/bin/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13579 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      973 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10669 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/log.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46616 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/protocol.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43807 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/structs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21576 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/symbols.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.230597 ads-async-0.3.0/ads_async/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   566445 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/tests/kmono.tmc
--rw-rw-r--   0 travis    (2000) travis    (2000)     5224 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/tests/test_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1089 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/tests/test_symbol.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1222 2022-09-14 18:24:05.000000 ads-async-0.3.0/ads_async/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.230597 ads-async-0.3.0/ads_async.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1751 2022-09-14 18:24:20.000000 ads-async-0.3.0/ads_async.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2022-09-14 18:24:20.000000 ads-async-0.3.0/ads_async.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-09-14 18:24:20.000000 ads-async-0.3.0/ads_async.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2022-09-14 18:24:20.000000 ads-async-0.3.0/ads_async.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2022-09-14 18:24:20.000000 ads-async-0.3.0/ads_async.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.230597 ads-async-0.3.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      626 2022-09-14 18:24:05.000000 ads-async-0.3.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2022-09-14 18:24:05.000000 ads-async-0.3.0/docs/make.bat
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:20.234599 ads-async-0.3.0/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5505 2022-09-14 18:24:05.000000 ads-async-0.3.0/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2022-09-14 18:24:05.000000 ads-async-0.3.0/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      326 2022-09-14 18:24:05.000000 ads-async-0.3.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-14 18:24:05.000000 ads-async-0.3.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2022-09-14 18:24:20.234599 ads-async-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2022-09-14 18:24:05.000000 ads-async-0.3.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68614 2022-09-14 18:24:05.000000 ads-async-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.639425 ads-async-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-07 17:32:57.000000 ads-async-0.3.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-07 17:32:57.000000 ads-async-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-04-07 17:32:57.000000 ads-async-0.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-07 17:32:57.000000 ads-async-0.3.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-07 17:32:57.000000 ads-async-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.631425 ads-async-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-07 17:32:57.000000 ads-async-0.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-07 17:32:57.000000 ads-async-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.631425 ads-async-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-07 17:32:57.000000 ads-async-0.3.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-04-07 17:32:57.000000 ads-async-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-04-07 17:32:57.000000 ads-async-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-07 17:32:57.000000 ads-async-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3014 2023-04-07 17:32:57.000000 ads-async-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-07 17:32:57.000000 ads-async-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-07 17:32:57.000000 ads-async-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-04-07 17:33:12.639425 ads-async-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-07 17:32:57.000000 ads-async-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/ads_async/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/ads_async/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32409 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/asyncio/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6095 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/asyncio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/ads_async/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2470 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/ads_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6116 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/route.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/bin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13759 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10659 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46562 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9098 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43590 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/structs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21461 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/ads_async/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   566445 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/tests/kmono.tmc
+-rw-r--r--   0 runner    (1001) docker     (122)     5224 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-04-07 17:32:57.000000 ads-async-0.3.1/ads_async/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/ads_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-07 17:33:12.000000 ads-async-0.3.1/ads_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-04-07 17:32:57.000000 ads-async-0.3.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-07 17:32:57.000000 ads-async-0.3.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.635425 ads-async-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-07 17:32:57.000000 ads-async-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-07 17:32:57.000000 ads-async-0.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.639425 ads-async-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-04-07 17:32:57.000000 ads-async-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-04-07 17:32:57.000000 ads-async-0.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-04-07 17:32:57.000000 ads-async-0.3.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-07 17:32:57.000000 ads-async-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 17:32:57.000000 ads-async-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 17:33:12.639425 ads-async-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 17:33:12.639425 ads-async-0.3.1/test-ioc/
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-07 17:32:57.000000 ads-async-0.3.1/test-ioc/envPaths
+-rwxr-xr-x   0 runner    (1001) docker     (122)      224 2023-04-07 17:32:57.000000 ads-async-0.3.1/test-ioc/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-04-07 17:32:57.000000 ads-async-0.3.1/test-ioc/st.cmd
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-04-07 17:32:57.000000 ads-async-0.3.1/test-ioc/test.db
```

### Comparing `ads-async-0.3.0/CONTRIBUTING.rst` & `ads-async-0.3.1/CONTRIBUTING.rst`

 * *Files 9% similar despite different names*

```diff
@@ -59,31 +59,32 @@
 1. Fork the `ads-async` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/ads-async.git
 
 3. Install your local copy into a new conda environment. Assuming you have conda installed, this is how you set up your fork for local development::
 
-    $ conda create -n ads-async python=3.7
+    $ conda create -n ads-async python=3.9 pip
     $ cd ads-async/
     $ pip install -e .
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-5. When you're done making changes, check that your changes pass flake8::
+5. Install and enable ``pre-commit`` for this repository::
 
-    $ flake8 ads_async
+    $ pip install pre-commit
+    $ pre-commit install
 
 6. Add new tests for any additional functionality or bugs you may have discovered.  And, of course, be sure that all previous tests still pass by running::
 
-    $ python run_tests.py -v
+    $ pytest -v
 
 7. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
@@ -94,10 +95,9 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put your
    new functionality into a function with a docstring, and add the feature to
    the list in README.rst.
-3. The pull request should work for Python 3.5 and up. Check
-   https://travis-ci.org/pcdshub/ads-async/pull_requests
+3. The pull request should work for Python 3.9 and up. Check the GitHub Actions status
    and make sure that the tests pass for all supported Python versions.
```

### Comparing `ads-async-0.3.0/LICENSE` & `ads-async-0.3.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `ads-async-0.3.0/README.rst` & `ads-async-0.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 ===============================
 ads-async
 ===============================
 
-.. image:: https://img.shields.io/travis/pcdshub/ads-async.svg
-        :target: https://travis-ci.org/pcdshub/ads-async
-
 .. image:: https://img.shields.io/pypi/v/ads-async.svg
         :target: https://pypi.python.org/pypi/ads-async
 
 
 Asyncio (or sans-i/o) TwinCAT AMS/ADS testing server in pure Python.
 
 ... and maybe a prototype client, too.
 
 Requirements
 ------------
 
-* Python 3.6+
+* Python 3.9+
 * (Optional) pytmc (for loading .tmc files in the server)
 
 Server Functionality
 --------------------
 
 * Reference asyncio implementation.
 * Loads .tmc files for symbol information (basic types only).
```

### Comparing `ads-async-0.3.0/ads_async/asyncio/client.py` & `ads-async-0.3.1/ads_async/asyncio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import asyncio
 import collections
 import contextvars
 import ctypes
 import ipaddress
 import os
 import typing
-from typing import Dict, Optional
 
 from .. import constants, exceptions, protocol, structs
 from ..constants import AdsTransmissionMode, AmsPort
 from . import utils
 
 _target_address = contextvars.ContextVar("_target_address", default=None)
 
@@ -186,18 +185,18 @@
                 await self._unsubscribe()
                 self.most_recent_notification = None
 
 
 class _BlockingRequest:
     """Helper for handling blocking requests in the client."""
 
-    owner: "AsyncioClientConnection"
+    owner: AsyncioClientConnection
     request: structs.T_AdsStructure
-    header: Optional[structs.AoEHeader]
-    response: Optional[structs.T_AdsStructure]
+    header: structs.AoEHeader | None
+    response: structs.T_AdsStructure | None
     options: dict
 
     def __init__(self, owner, request, error_event, **options):
         self.owner = owner
         self.request = request
         self.options = options
         self._event = asyncio.Event()
@@ -238,29 +237,29 @@
 class Symbol:
     """
     A symbol from an AsyncioClientCircuit.
 
     Not to be instantiated by itself.
     """
 
-    owner: "AsyncioClientCircuit"
-    index_group: Optional[int]
-    index_offset: Optional[int]
-    name: Optional[str]
-    info: Optional[structs.AdsSymbolEntry]
-    handle: Optional[int]
+    owner: AsyncioClientCircuit
+    index_group: int | None
+    index_offset: int | None
+    name: str | None
+    info: structs.AdsSymbolEntry | None
+    handle: int | None
     string_encoding: str
 
     def __init__(
         self,
-        owner: "AsyncioClientCircuit",
+        owner: AsyncioClientCircuit,
         *,
-        index_group: Optional[int] = None,
-        index_offset: Optional[int] = None,
-        name: Optional[str] = None,
+        index_group: int | None = None,
+        index_offset: int | None = None,
+        name: str | None = None,
         string_encoding: str = constants.ADS_ASYNC_STRING_ENCODING,
     ):
         self.owner = owner
         self.name = name
         self.index_group = index_group
         self.index_offset = index_offset
         self.info = None
@@ -371,22 +370,22 @@
     default_port : AmsPort, optional
         The default port to use in communciation (R0_PLC_TC3 port).
     """
 
     circuit: protocol.ClientCircuit
     _response_handlers: typing.DefaultDict[int, list]
     _symbols: dict
-    connection: "AsyncioClientConnection"
+    connection: AsyncioClientConnection
     default_port: AmsPort
     log: log.ComposableLogAdapter
     net_id: str
 
     def __init__(
         self,
-        connection: "AsyncioClientConnection",
+        connection: AsyncioClientConnection,
         net_id: str,
         default_port=AmsPort.R0_PLC_TC3,
     ):
         self._response_handlers = collections.defaultdict(list)
         self._symbols = {}
         self.circuit = connection.connection.get_circuit(net_id)
         self.connection = connection
@@ -408,16 +407,16 @@
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
     async def send(
         self,
         *items,
         ads_error: constants.AdsError = constants.AdsError.NOERR,
-        port: Optional[AmsPort] = None,
-        response_handler: Optional[typing.Coroutine] = None,
+        port: AmsPort | None = None,
+        response_handler: typing.Coroutine | None = None,
     ):
         """
         Package and send items over the wire.
 
         Parameters
         ----------
         *items :
@@ -483,16 +482,16 @@
         self,
         index_group: int,
         index_offset: int,
         length: int,
         mode: AdsTransmissionMode = AdsTransmissionMode.SERVERCYCLE,
         max_delay: int = 1,
         cycle_time: int = 100,
-        net_id: Optional[str] = None,
-        port: Optional[AmsPort] = None,
+        net_id: str | None = None,
+        port: AmsPort | None = None,
     ) -> Notification:
         """
         Add an advanced notification by way of index group/offset.
 
         Parameters
         -----------
         index_group : int
@@ -534,15 +533,15 @@
             ),
             port=port or self.default_port,
         )
 
     async def write_and_read(
         self,
         item,
-        port: Optional[AmsPort] = None,
+        port: AmsPort | None = None,
     ):
         """
         Write `item` and read the server's response.
 
         Parameters
         ----------
         item : T_AdsStructure
@@ -668,15 +667,15 @@
     async def get_task_count(self) -> int:
         """Get the number of tasks running on the PLC."""
         (count,) = await self.get_symbol_by_name(
             "TwinCAT_SystemInfoVarList._AppInfo.TaskCnt"
         ).read()
         return count
 
-    async def get_task_names(self) -> typing.Dict[int, str]:
+    async def get_task_names(self) -> dict[int, str]:
         """Get the names of tasks running on the PLC."""
         task_count = await self.get_task_count()
         names = {}
         for task_id in range(1, task_count + 1):
             names[task_id] = await self.get_symbol_by_name(
                 f"TwinCAT_SystemInfoVarList._TaskInfo[{task_id}].TaskName"
             ).read()
@@ -697,15 +696,15 @@
             "boot/CurrentConfig.tszip", buffer_size=buffer_size
         )
         return utils.InMemoryZipFile(current_config)
 
     async def download_projects(
         self,
         buffer_size: int = 16384,
-    ) -> Dict[str, utils.InMemoryZipFile]:
+    ) -> dict[str, utils.InMemoryZipFile]:
         """Download the active project."""
         current_config = await self.download_current_config_file(
             buffer_size=buffer_size
         )
         projects = {}
         for fn in current_config.zip.filelist:
             if fn.filename.startswith("_Config/PLC/"):
@@ -849,17 +848,17 @@
     client: protocol.ClientConnection
     log: log.ComposableLogAdapter
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
 
     def __init__(
         self,
-        their_address: typing.Tuple[str, int],
-        our_net_id: Optional[str] = None,  # can be determined later
-        reconnect_rate: Optional[int] = 10,
+        their_address: tuple[str, int],
+        our_net_id: str | None = None,  # can be determined later
+        reconnect_rate: int | None = 10,
         request_timeout: float = 2.0,
     ):
         self.connection = protocol.ClientConnection(
             their_address=their_address,
             our_net_id=our_net_id,
             our_address=("(client)", 0),  # TODO
         )
@@ -881,15 +880,15 @@
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
     def __getitem__(self, key):
         return self.get_circuit(key)
 
-    def get_circuit(self, net_id: Optional[str] = None):
+    def get_circuit(self, net_id: str | None = None):
         """
         Get a circuit to the given target Net ID.
 
         Parameters
         ----------
         net_id : str, optional
             The target Net ID.  Defaults to (their_address).1.1 as a common
```

### Comparing `ads-async-0.3.0/ads_async/asyncio/server.py` & `ads-async-0.3.1/ads_async/asyncio/server.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/asyncio/utils.py` & `ads-async-0.3.1/ads_async/asyncio/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import inspect
 import io
-import sys
 import threading
 import weakref
 import zipfile
 
 
 class _TaskHandler:
     # Borrowed from caproto
@@ -207,22 +206,10 @@
     def __enter__(self) -> InMemoryZipFile:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
 
-if sys.version_info < (3, 7):
-    # python <= 3.6 compatibility
-    def get_running_loop():
-        return asyncio.get_event_loop()
-
-    def run(coro, debug=False):
-        return get_running_loop().run_until_complete(coro)
-
-    def create_task(coro):
-        return get_running_loop().create_task(coro)
-
-else:
-    get_running_loop = asyncio.get_running_loop
-    run = asyncio.run
-    create_task = asyncio.create_task
+get_running_loop = asyncio.get_running_loop
+run = asyncio.run
+create_task = asyncio.create_task
```

### Comparing `ads-async-0.3.0/ads_async/bin/ads_async.py` & `ads-async-0.3.1/ads_async/bin/ads_async.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/bin/download.py` & `ads-async-0.3.1/ads_async/bin/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 import argparse
 import dataclasses
 import json
 import logging
 import os
 import sys
-from typing import AsyncGenerator, List, Optional
+from collections.abc import AsyncGenerator
+from typing import Optional
 
 from .. import constants, structs
 from .utils import setup_connection
 
 DESCRIPTION = __doc__
 
 module_logger = logging.getLogger(__name__)
@@ -98,15 +99,15 @@
     #: Exception raised during the download process.  Only set if ``data`` is
     #: None.
     error: Optional[Exception] = None
 
 
 async def async_download(
     plc_hostname: str,
-    filenames: List[str],
+    filenames: list[str],
     our_net_id: str,
     plc_net_id: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     project: bool = False,
     route_host: str = "",
 ) -> AsyncGenerator[DownloadItem, None]:
@@ -158,15 +159,15 @@
                         stat=None,
                         error=None,
                     )
 
 
 async def main(
     host: str,
-    filenames: List[str],
+    filenames: list[str],
     save_to: str = ".",
     net_id: Optional[str] = None,
     our_net_id: Optional[str] = None,
     our_host: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     route_host: Optional[str] = None,
```

### Comparing `ads-async-0.3.0/ads_async/bin/get.py` & `ads-async-0.3.1/ads_async/bin/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 "ads-async get" is a command line utility to get symbol information from a
 given TwinCAT3 PLC.
 """
 import argparse
 import json
 import logging
-from typing import List, Optional
+from typing import Optional
 
 from .. import constants
 from .utils import setup_connection
 
 DESCRIPTION = __doc__
 
 module_logger = logging.getLogger(__name__)
@@ -58,15 +58,15 @@
         "--timeout", type=float, default=2.0, help="Timeout for responses"
     )
     return argparser
 
 
 async def get_symbols(
     plc_hostname: str,
-    symbols: List[str],
+    symbols: list[str],
     our_net_id: str,
     plc_net_id: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     route_host: str = "",
     include_exceptions: bool = True,
 ) -> dict:
@@ -106,15 +106,15 @@
                     result[symbol_name] = f"(Exception) {ex.__class__.__name__} {ex}"
 
     return result
 
 
 async def main(
     host: str,
-    symbols: List[str],
+    symbols: list[str],
     net_id: Optional[str] = None,
     our_net_id: Optional[str] = None,
     our_host: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     route_host: Optional[str] = None,
 ):
```

### Comparing `ads-async-0.3.0/ads_async/bin/info.py` & `ads-async-0.3.1/ads_async/bin/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 "ads-async info" is a command line utility for getting information about a
 given TwinCAT3 PLC.
 """
 
 import argparse
 import json
 import logging
-from typing import Generator
+from collections.abc import Generator
 
 from .. import service
 from .utils import send_and_receive_service_udp
 
 DESCRIPTION = __doc__
 
 module_logger = logging.getLogger(__name__)
```

### Comparing `ads-async-0.3.0/ads_async/bin/monitor.py` & `ads-async-0.3.1/ads_async/bin/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 "ads-async monitor" is a command line utility to monitor symbol values from a
 given TwinCAT3 PLC.
 """
 import argparse
 import asyncio
 import logging
-from typing import List, Optional
+from typing import Optional
 
 from .. import constants, structs
 from .utils import setup_connection
 
 DESCRIPTION = __doc__
 
 module_logger = logging.getLogger(__name__)
@@ -58,15 +58,15 @@
         "--timeout", type=float, default=2.0, help="Timeout for responses"
     )
     return argparser
 
 
 async def monitor_symbols(
     plc_hostname: str,
-    symbols: List[str],
+    symbols: list[str],
     our_net_id: str,
     plc_net_id: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     route_host: str = "",
     include_exceptions: bool = True,
 ) -> dict:
@@ -108,15 +108,15 @@
             for symbol_name in symbols
         ]
         return await asyncio.gather(*tasks)
 
 
 async def main(
     host: str,
-    symbols: List[str],
+    symbols: list[str],
     net_id: Optional[str] = None,
     our_net_id: Optional[str] = None,
     our_host: Optional[str] = None,
     timeout: float = 2.0,
     add_route: bool = False,
     route_host: Optional[str] = None,
 ):
```

### Comparing `ads-async-0.3.0/ads_async/bin/route.py` & `ads-async-0.3.1/ads_async/bin/route.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/bin/utils.py` & `ads-async-0.3.1/ads_async/bin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import contextlib
 import logging
 import socket
-from typing import Generator, Optional
+from collections.abc import Generator
+from typing import Optional
 
 from .. import constants, service
 from ..asyncio.client import Client
 from ..service import BadResponse
 
 module_logger = logging.getLogger(__name__)
```

### Comparing `ads-async-0.3.0/ads_async/constants.py` & `ads-async-0.3.1/ads_async/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 ADS_ASYNC_PASSWORD = os.environ.get("ADS_ASYNC_PASSWORD", "1")
 
 
 class Role(str, enum.Enum):
     Client = "Client"
     Server = "Server"
 
+    def __str__(self) -> str:
+        return self.value
+
+    __repr__ = __str__
+
 
 class AmsPort(enum.IntEnum):
     LOGGER = 100
     R0_RTIME = 200
     R0_TRACE = R0_RTIME + 90
     R0_IO = 300
     R0_SPS = 400
@@ -344,15 +349,16 @@
     CLIENT_NOMORESYM = 0x53 + ERR_ADSERRS
     # invalid response received
     CLIENT_SYNCRESINVALID = 0x54 + ERR_ADSERRS
     # sync port is locked
     CLIENT_SYNCPORTLOCKED = 0x55 + ERR_ADSERRS
 
     @classmethod
-    def _missing_(cls, value):
+    def _missing_(cls, value: int):
+        value = int(value)
         if not 0 <= value <= 0xFFFF:
             return None
 
         try:
             return cls._value2member_map_[value]
         except KeyError:
             member = int.__new__(cls, value)
@@ -376,18 +382,18 @@
     BIGTYPE = 65
     STRING = 30
     WSTRING = 31
     REAL80 = 32
     BIT = 33
     MAXTYPES = 34
 
-    to_ctypes: typing.Mapping["AdsDataType", typing.Type[ctypes._SimpleCData]]
+    to_ctypes: typing.Mapping["AdsDataType", type[ctypes._SimpleCData]]
 
     @property
-    def ctypes_type(self) -> typing.Type[ctypes._SimpleCData]:
+    def ctypes_type(self) -> type[ctypes._SimpleCData]:
         """Get the ctypes _SimpleCData type associated with the data type."""
         return self.to_ctypes[self]
 
 
 AdsDataType.to_ctypes = {
     # AdsDataType.VOID: None,
     AdsDataType.INT8: ctypes.c_int8,
@@ -456,7 +462,12 @@
 
 SDO_UPLOAD = 0xF302
 
 
 class DownloadPath(str, enum.Enum):
     boot = "boot"
     target = "target"
+
+    def __str__(self) -> str:
+        return self.value
+
+    __repr__ = __str__
```

### Comparing `ads-async-0.3.0/ads_async/exceptions.py` & `ads-async-0.3.1/ads_async/exceptions.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/log.py` & `ads-async-0.3.1/ads_async/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         record.asctime = self.formatTime(record, self.datefmt)
 
         formatted = self._fmt % record.__dict__
 
         if record.exc_info and not record.exc_text:
             record.exc_text = self.formatException(record.exc_info)
         if record.exc_text:
-            formatted = "{}\n{}".format(formatted.rstrip(), record.exc_text)
+            formatted = f"{formatted.rstrip()}\n{record.exc_text}"
         return formatted.replace("\n", "\n    ")
 
 
 def validate_level(level) -> int:
     """Return an integer for level comparison."""
     if isinstance(level, int):
         return level
```

### Comparing `ads-async-0.3.0/ads_async/protocol.py` & `ads-async-0.3.1/ads_async/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import copy
 import ctypes
 import inspect
 import logging
 import typing
-from typing import Callable, Dict, Generator, Optional, Tuple, Union
+from collections.abc import Generator
+from typing import Callable
 
 from . import constants, log, structs, utils
 from .constants import (
     AdsCommandId,
     AdsError,
     AdsIndexGroup,
     AdsTransmissionMode,
@@ -18,30 +19,30 @@
     Role,
 )
 from .exceptions import RequestFailedError
 from .structs import AmsNetId
 from .symbols import Database, Symbol
 
 module_logger = logging.getLogger(__name__)
-IPPort = typing.Tuple[str, int]
+IPPort = tuple[str, int]
 
 # TODO: AMS can be over serial, UDP, etc. and not just TCP
 _AMS_HEADER_LENGTH = ctypes.sizeof(structs.AmsTcpHeader)
 _AOE_HEADER_LENGTH = ctypes.sizeof(structs.AoEHeader)
 
 
 class MissingHandlerError(RuntimeError):
     ...
 
 
 def from_wire(
     buf: bytearray,
     *,
     logger: logging.Logger = module_logger,
-) -> Generator[Tuple[structs.AoEHeader, typing.Any], None, None]:
+) -> Generator[tuple[structs.AoEHeader, typing.Any], None, None]:
     """
     Deserialize data from the wire into ctypes structures.
 
     Parameters
     ----------
     buf : bytearray
         The receive data buffer.
@@ -131,15 +132,15 @@
         yield required_bytes, item
 
 
 def response_to_wire(
     *items: structs.T_Serializable,
     request_header: structs.AoEHeader,
     ads_error: AdsError = AdsError.NOERR,
-) -> Tuple[list, bytearray]:
+) -> tuple[list, bytearray]:
     """
     Prepare `items` to be sent over the wire.
 
     Parameters
     -------
     *items : structs.T_AdsStructure or bytes
         Individual structures or pre-serialized data to send.
@@ -183,15 +184,15 @@
 def request_to_wire(
     *items: structs.T_Serializable,
     target: structs.AmsAddr,
     source: structs.AmsAddr,
     invoke_id: int,
     state_flags: AoEHeaderFlag = AoEHeaderFlag.ADS_COMMAND,
     error_code: int = 0,
-) -> Tuple[list, bytearray]:
+) -> tuple[list, bytearray]:
     """
     Prepare `items` to be sent over the wire.
 
     Parameters
     -------
     *items : structs.T_AdsStructure or bytes
         Individual structures or pre-serialized data to send.
@@ -306,25 +307,25 @@
         The class to create circuits with - as this differs on server/client
         instances.
     """
 
     _our_address: IPPort
     _our_net_id: str
     circuit_class: type
-    circuits: Dict[str, _Circuit]
+    circuits: dict[str, _Circuit]
     recv_buffer: bytearray
     role: Role
     their_address: IPPort
 
     def __init__(
         self,
         their_address: IPPort,
         role: constants.Role,
-        our_address: Optional[IPPort] = None,
-        our_net_id: Optional[str] = None,
+        our_address: IPPort | None = None,
+        our_net_id: str | None = None,
     ):
         self.recv_buffer = bytearray()
         self.circuits = {}
         self.their_address = their_address
 
         self._log_tags = {
             "role": str(role),
@@ -372,15 +373,15 @@
                     direction="<-",
                     bytesize=consumed,
                 ),
             )
             self.recv_buffer = self.recv_buffer[consumed:]
             yield item
 
-    def get_circuit(self, net_id: Union[AmsNetId, str]) -> _Circuit:
+    def get_circuit(self, net_id: AmsNetId | str) -> _Circuit:
         """Get a circuit for (their) Net ID."""
         if isinstance(net_id, AmsNetId):
             net_id = repr(net_id)
 
         try:
             return self.circuits[net_id]
         except KeyError:
@@ -445,19 +446,19 @@
 
     Attributes
     ----------
     server : Server
         The server instance.
     """
 
-    server: "Server"
+    server: Server
 
     def __init__(
         self,
-        server: "Server",
+        server: Server,
         our_address: IPPort,
         our_net_id: str,
         their_address: IPPort,
     ):
         self.circuit_class = ServerCircuit  # forward definition
         self.server = server
         super().__init__(
@@ -476,17 +477,17 @@
     on top to have a functional server.
 
     See Also
     --------
     :class:`.asyncio.server.AsyncioServer`
     """
 
-    _version: Tuple[int, int, int] = (0, 0, 0)  # TODO: from versioneer
+    _version: tuple[int, int, int] = (0, 0, 0)  # TODO: from versioneer
     _name: str
-    connections: Dict[IPPort, ServerConnection]
+    connections: dict[IPPort, ServerConnection]
     database: Database
     log: log.ComposableLogAdapter
 
     def __init__(self, database: Database, net_id: str, *, name="AdsAsync"):
         self._name = name
         self.database = database
         self.connections = {}
@@ -546,15 +547,15 @@
 
     @property
     def ads_state(self) -> constants.AdsState:
         """The current state of the server."""
         return constants.AdsState.RUN
 
     @property
-    def version(self) -> Tuple[int, int, int]:
+    def version(self) -> tuple[int, int, int]:
         """The server version."""
         return self._version
 
     @property
     def name(self) -> str:
         """The server name."""
         return self._name
@@ -589,18 +590,18 @@
     handle_to_symbol: dict
     log: log.ComposableLogAdapter
     our_port: AmsPort
     tags: dict
 
     def __init__(
         self,
-        connection: "_Connection",
+        connection: _Connection,
         our_net_id: str,
         their_net_id: str,
-        tags: Optional[dict] = None,
+        tags: dict | None = None,
         our_port: AmsPort = AmsPort.R0_PLC_TC3,
         their_port: AmsPort = AmsPort.R0_PLC_TC3,
     ):
         self.connection = connection
         self.our_net_id = our_net_id
         self.their_net_id = their_net_id
         self.our_port = our_port
@@ -640,15 +641,15 @@
     def __repr__(self):
         return (
             f"<{self.__class__.__name__} our_net_id={self.our_net_id} "
             f"their_net_id={self.their_net_id}>"
         )
 
     def get_handler(
-        self, header: structs.AoEHeader, command: Optional[structs.T_AdsStructure]
+        self, header: structs.AoEHeader, command: structs.T_AdsStructure | None
     ) -> list:
         """
         Top-level command dispatcher.
 
         First stop to determine which method will handle the given command.
 
         Parameters
@@ -725,15 +726,15 @@
 
         return bytes_to_send
 
     def request_to_wire(
         self,
         *items: structs.T_Serializable,
         ads_error: AdsError = AdsError.NOERR,
-        target: Optional[structs.AmsAddr] = None,
+        target: structs.AmsAddr | None = None,
     ) -> bytearray:
         """
         Prepare `items` to be sent over the wire.
 
         Parameters
         -------
         *items : structs.T_AdsStructure or bytes
@@ -801,24 +802,24 @@
 
     address : (host, port)
         The client address.
     """
 
     _handle_counter: utils.ThreadsafeCounter
     _notification_counter: utils.ThreadsafeCounter
-    _handlers: Dict[Tuple[AdsCommandId, Optional[AdsIndexGroup]], Callable]
+    _handlers: dict[tuple[AdsCommandId, AdsIndexGroup | None], Callable]
     address: IPPort
     server_host: IPPort
 
     def __init__(
         self,
         connection: ClientConnection,
         our_net_id: str,
         their_net_id: str,
-        tags: Optional[dict] = None,
+        tags: dict | None = None,
         our_port: AmsPort = AmsPort.R0_PLC_TC3,
         their_port: AmsPort = AmsPort.R0_PLC_TC3,
     ):
         self.unknown_notifications = set()
         tags = dict(tags or {})
         tags.update(
             {
@@ -1285,26 +1286,26 @@
 
     address : (host, port)
         The client address.
     """
 
     _handle_counter: utils.ThreadsafeCounter
     _notification_counter: utils.ThreadsafeCounter
-    _handlers: Dict[Tuple[AdsCommandId, Optional[AdsIndexGroup]], Callable]
+    _handlers: dict[tuple[AdsCommandId, AdsIndexGroup | None], Callable]
     address: IPPort
-    server: "Server"
+    server: Server
     server_host: IPPort
     connection: ServerConnection
 
     def __init__(
         self,
         connection: ServerConnection,
         our_net_id: str,
         their_net_id: str,
-        tags: Optional[dict] = None,
+        tags: dict | None = None,
         our_port: AmsPort = AmsPort.R0_PLC_TC3,
         their_port: AmsPort = AmsPort.R0_PLC_TC3,
     ):
         tags = dict(tags or {})
         tags.update(
             {
                 "role": Role.Server,
@@ -1319,15 +1320,15 @@
             tags=tags,
             our_port=our_port,
             their_port=their_port,
         )
         self.server = connection.server
 
     def handle_command(
-        self, header: structs.AoEHeader, request: Optional[structs.T_AdsStructure]
+        self, header: structs.AoEHeader, request: structs.T_AdsStructure | None
     ) -> list:
         """
         Top-level command dispatcher.
 
         First stop to determine which method will handle the given command.
 
         Parameters
```

### Comparing `ads-async-0.3.0/ads_async/service.py` & `ads-async-0.3.1/ads_async/service.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/structs.py` & `ads-async-0.3.1/ads_async/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import typing
 
 from . import constants, exceptions, utils
 from .constants import AoEHeaderFlag
 
 T_AdsStructure = typing.TypeVar("T_AdsStructure", bound="_AdsStructBase")
 T_Serializable = typing.Union[T_AdsStructure, bytes, ctypes._SimpleCData]
-T_PayloadField = typing.Tuple[str, str, int, typing.Callable, typing.Callable]
-_T_Commands = typing.Dict[constants.AdsCommandId, typing.Dict[str, T_AdsStructure]]
+T_PayloadField = tuple[str, str, int, typing.Callable, typing.Callable]
+_T_Commands = dict[constants.AdsCommandId, dict[str, T_AdsStructure]]
 
 _commands = {}  # type: _T_Commands
 
 
 def _use_for(
     key: str, command_id: constants.AdsCommandId, cls: T_AdsStructure
 ) -> T_AdsStructure:
@@ -105,16 +105,16 @@
         - Removing alignment by way of _pack_
     """
 
     # To be overridden by subclasses:
     _command_id: constants.AdsCommandId = constants.AdsCommandId.INVALID
 
     _pack_ = 1
-    _dict_mapping: typing.Dict[str, str] = {}
-    _payload_fields: typing.List[T_PayloadField] = []
+    _dict_mapping: dict[str, str] = {}
+    _payload_fields: list[T_PayloadField] = []
 
     def __init_subclass__(cls):
         super().__init_subclass__()
 
         dict_mapping = {}
         all_fields = []
         for base in reversed(cls.mro()):
@@ -154,15 +154,15 @@
                 value = serialize(value)
             packed.extend(struct.pack(fmt, value) + b"\00" * padding)
 
         return packed
 
     @classmethod
     def deserialize(
-        cls: typing.Type[T_AdsStructure], buf: typing.Union[memoryview, bytearray]
+        cls: type[T_AdsStructure], buf: memoryview | bytearray
     ) -> T_AdsStructure:
         """
         Deserialize data from `buf` into a structure + payload.
 
         Parameters
         ----------
         buf : bytearray
@@ -199,15 +199,15 @@
     def command_id(self) -> constants.AdsCommandId:
         """The command ID associated with this request/response."""
         return self._command_id
 
 
 def _enum_property(
     field_name: str,
-    enum_cls: typing.Type[enum.Enum],
+    enum_cls: type[enum.Enum],
     *,
     doc: str = None,
     strict: bool = True,
 ) -> property:
     """
     Create a property which makes a field value into an enum value.
 
@@ -269,15 +269,15 @@
     def fget(self) -> str:
         value = getattr(self, field_name)
         try:
             return value.decode(encoding)
         except ValueError:
             return value
 
-    def fset(self, value: typing.Union[str, bytes]):
+    def fset(self, value: str | bytes):
         if isinstance(value, str):
             value = value.encode(encoding)
         setattr(self, field_name, value)
 
     return property(fget, fset, doc=doc)
 
 
@@ -296,16 +296,16 @@
     ]
 
     def __repr__(self):
         return ".".join(str(c) for c in self.octets)
 
     @classmethod
     def from_ipv4(
-        cls: typing.Type[T_AdsStructure],
-        ip: typing.Union[str, ipaddress.IPv4Address],
+        cls: type[T_AdsStructure],
+        ip: str | ipaddress.IPv4Address,
         octet5: int = 1,
         octet6: int = 1,
     ) -> T_AdsStructure:
         """
         Create an AMS Net ID based on an IPv4 address.
 
         Parameters
@@ -325,15 +325,15 @@
         """
         if not isinstance(ip, ipaddress.IPv4Address):
             ip = ipaddress.IPv4Address(ip)
 
         return cls(tuple(ip.packed) + (octet5, octet6))
 
     @classmethod
-    def from_string(cls: typing.Type[T_AdsStructure], addr: str) -> T_AdsStructure:
+    def from_string(cls: type[T_AdsStructure], addr: str) -> T_AdsStructure:
         """
         Create an AMS Net ID based on an AMS ID string.
 
         Parameters
         ----------
         addr : str
             The net ID string.
@@ -387,15 +387,15 @@
     _fields_ = [
         ("version", ctypes.c_uint8),
         ("revision", ctypes.c_uint8),
         ("build", ctypes.c_uint16),
     ]
 
     @property
-    def as_tuple(self) -> typing.Tuple[int, int, int]:
+    def as_tuple(self) -> tuple[int, int, int]:
         """The version tuple: (Version, Revision, Build)"""
         return (self.version, self.revision, self.build)
 
 
 class AdsNotificationAttrib(_AdsStructBase):  # TODO: Unused; may be removed?
     """
     Contains all the attributes for the definition of a notification.
@@ -482,15 +482,15 @@
 
     @property
     def sender_name(self):
         return bytes(self._sender_name).split(b"\0")[0]
 
     @classmethod
     def deserialize(
-        cls: typing.Type[T_AdsStructure], buf: typing.Union[memoryview, bytearray]
+        cls: type[T_AdsStructure], buf: memoryview | bytearray
     ) -> AdsNotificationLogMessage:
         """Deserialize a log message."""
         # message_length is not reliable when nearing 255+ characters!
         new_struct = cls.from_buffer(buf)
         payload_buf = memoryview(buf)[ctypes.sizeof(cls) :]
         new_struct.message = bytes(payload_buf)
         return new_struct
@@ -572,15 +572,15 @@
 
     @property
     def timestamp(self):
         return utils.get_datetime_from_timestamp(self._timestamp)
 
     @classmethod
     def deserialize(
-        cls: typing.Type[T_AdsStructure], buf: typing.Union[memoryview, bytearray]
+        cls: type[T_AdsStructure], buf: memoryview | bytearray
     ) -> T_AdsStructure:
         new_struct = cls.from_buffer(buf)
         payload_buf = memoryview(buf)[ctypes.sizeof(cls) :]
 
         new_struct.byte_size = 0
         new_struct.samples = []
         for idx in range(new_struct.num_samples):
@@ -605,15 +605,15 @@
         ("_stamp_start", ctypes.c_ubyte * 0),
     ]
 
     _dict_mapping = {"_stamp_start": "stamps"}
 
     @classmethod
     def deserialize(
-        cls: typing.Type[T_AdsStructure], buf: typing.Union[memoryview, bytearray]
+        cls: type[T_AdsStructure], buf: memoryview | bytearray
     ) -> T_AdsStructure:
         new_struct = cls.from_buffer(buf)
         payload_buf = memoryview(buf)[ctypes.sizeof(cls) :]
 
         new_struct.stamps = []
         for stamp in range(new_struct.num_stamps):
             stamp = AdsNotificationStampHeader.deserialize(payload_buf)
@@ -1255,21 +1255,21 @@
         self.result = result
         self.version.version = version
         self.version.revision = revision
         self.version.build = build
         self.name = name
 
     @property
-    def version_tuple(self) -> typing.Tuple[int, int, int]:
+    def version_tuple(self) -> tuple[int, int, int]:
         """The version tuple: (Version, Revision, Build)"""
         return self.version.as_tuple
 
     @classmethod
     def deserialize(
-        cls: typing.Type[T_AdsStructure], buf: typing.Union[memoryview, bytearray]
+        cls: type[T_AdsStructure], buf: memoryview | bytearray
     ) -> T_AdsStructure:
         buf = bytearray(buf)
         if len(buf) < ctypes.sizeof(AdsDeviceInfo):
             # Empty response is possible if there's no project loaded
             buf.extend(b"\x00" * (ctypes.sizeof(AdsDeviceInfo) - len(buf)))
         return super().deserialize(buf)
 
@@ -1382,15 +1382,15 @@
 
 def serialize_data(
     data_type: constants.AdsDataType,
     data: typing.Any,
     length: int = None,
     *,
     endian="<",
-) -> typing.Tuple[int, bytes]:
+) -> tuple[int, bytes]:
     """
     Serialize symbol data for transmission over the wire.
 
     Parameters
     ----------
     data_type : constants.AdsDataType
         The data type of the data to serialize.
@@ -1416,15 +1416,15 @@
     ctypes_type = data_type.ctypes_type._type_  # type: ignore
     st = struct.Struct(f"{endian}{length}{ctypes_type}")
     return st.size, st.pack(data)
 
 
 def deserialize_data(
     data_type: constants.AdsDataType, length: int, data: bytes, *, endian="<"
-) -> typing.Tuple[int, typing.Any]:
+) -> tuple[int, typing.Any]:
     """
     Deserialize symbol data from the wire.
 
     Parameters
     ----------
     data_type : constants.AdsDataType
         The data type of the data to deserialize.
@@ -1453,15 +1453,15 @@
 
 def deserialize_data_by_symbol_entry(
     info: AdsSymbolEntry,
     data: bytes,
     *,
     endian="<",
     string_encoding: str = constants.ADS_ASYNC_STRING_ENCODING,
-) -> typing.Tuple[int, typing.Any]:
+) -> tuple[int, typing.Any]:
     """
     Deserialize symbol data from the wire, given AdsSymbolEntry information.
 
     Parameters
     ----------
     info : AdsSymbolEntry
         The data type information.
```

### Comparing `ads-async-0.3.0/ads_async/symbols.py` & `ads-async-0.3.1/ads_async/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 import enum
 import logging
 import math
 import sys
 import textwrap
 import typing
-from typing import Optional, Type
+from typing import Optional
 
 from . import constants, log, structs
 from .constants import AdsDataType
 
 try:
     import pytmc
 except ImportError:
@@ -169,15 +169,15 @@
         return ptr_value
 
     @property
     def value(self):
         return self.read()
 
     @property
-    def memory_range(self) -> typing.Tuple[int, int]:
+    def memory_range(self) -> tuple[int, int]:
         offset = self.offset if not self.pointer else self._dereference_pointer()
         return (offset, offset + self.byte_size)
 
     def __repr__(self):
         try:
             mem_start, mem_end = self.memory_range
         except NullPointerDereferencedError:
@@ -196,15 +196,14 @@
 def tmc_to_symbols(
     item: typing.Union["pytmc.parser.Symbol", "pytmc.parser.SubItem"],
     data_area: "DataArea",
     *,
     parent_name: str = "",
     parent_bit_offset: int = 0,
 ) -> typing.Generator["Symbol", None, None]:
-
     bit_offset = item.BitOffs[0].bit_offset + parent_bit_offset
     bit_size = item.BitSize[0].bit_size
     byte_offset = bit_offset // 8
     if (bit_offset % 8) != 0 or (bit_size % 8) != 0:
         bit_offset_obj = OffsetSize(bit_offset - (byte_offset * 8), bit_size)
     else:
         bit_offset_obj = None
@@ -241,18 +240,18 @@
     else:
         # hack to just get first-level sub-items, including subclass (=extended
         # type) items
 
         # TODO is this a bug?
         if isinstance(item, pytmc.parser.Symbol):
             sub_items = list(
-                set(sub_item[1] for sub_item in item.walk() if len(sub_item) > 1)
+                {sub_item[1] for sub_item in item.walk() if len(sub_item) > 1}
             )
         else:
-            sub_items = list(set(sub_item[0] for sub_item in data_type.walk()))
+            sub_items = list({sub_item[0] for sub_item in data_type.walk()})
 
         sub_items.sort(key=lambda item: item.bit_offset)
 
         if (bit_size % 8) != 0:
             raise ValueError("ComplexSymbol not byte aligned?")
 
         if pointer:
@@ -287,17 +286,15 @@
     INT8 UINT8 INT16 UINT16 INT32 UINT32 INT64 UINT64 REAL32 REAL64 STRING
     WSTRING REAL80 BIT
 
     Notably, this does not include BIGTYPE, which is represented by
     :class:`ComplexSymbol`.
     """
 
-    ctypes_data_type: typing.Union[
-        typing.Type[ctypes.Array], typing.Type[ctypes._SimpleCData]
-    ]
+    ctypes_data_type: typing.Union[type[ctypes.Array], type[ctypes._SimpleCData]]
 
     def _configure_data_type(self):
         ctypes_base_type = self.data_type.ctypes_type
         if self.array_length > 1:
             self.ctypes_data_type = self.array_length * ctypes_base_type
         else:
             self.ctypes_data_type = ctypes_base_type
@@ -306,15 +303,15 @@
 
 class ComplexSymbol(Symbol):
     def __init__(
         self,
         *,
         struct_size: Optional[int] = None,
         data_type: AdsDataType = AdsDataType.BIGTYPE,
-        cls: Optional[Type[ctypes.Structure]] = None,
+        cls: Optional[type[ctypes.Structure]] = None,
         **kwargs,
     ):
         if struct_size is None:
             if cls is not None:
                 struct_size = ctypes.sizeof(cls)
             else:
                 raise ValueError("Must specify structure class or byte size")
@@ -344,26 +341,25 @@
         self.byte_size = self._struct_size * self.array_length
         self.ctypes_data_type = (ctypes.c_ubyte * self._struct_size) * self.array_length
 
 
 class DataArea:
     memory: PlcMemory
     index_group: constants.AdsIndexGroup
-    symbols: typing.Dict[str, Symbol]
+    symbols: dict[str, Symbol]
     area_type: str
 
     def __init__(
         self,
         index_group: constants.AdsIndexGroup,
         area_type: str,
         *,
         memory: PlcMemory = None,
         memory_size: typing.Optional[int] = None,
     ):
-
         self.index_group = index_group
         self.area_type = area_type
         self.symbols = {}
 
         if memory is not None:
             self.memory = memory
         elif memory_size is not None:
@@ -447,16 +443,16 @@
     # RetainDst
     # InfoData
     # RedundancySrc
     # RedundancyDst
 
 
 class Database:
-    data_areas: typing.List[DataArea]
-    index_groups: typing.Dict[constants.AdsIndexGroup, DataArea]
+    data_areas: list[DataArea]
+    index_groups: dict[constants.AdsIndexGroup, DataArea]
 
     def get_symbol_by_name(self, symbol_name) -> Symbol:
         raise KeyError(symbol_name)
 
 
 class TmcDatabase(Database):
     tmc: "pytmc.parser.TcModuleClass"
@@ -564,15 +560,15 @@
         )
         self.data_area.symbols[name] = sym
         return sym
 
     def add_complex_symbol(
         self,
         name: str,
-        cls: Type[ctypes.LittleEndianStructure],
+        cls: type[ctypes.LittleEndianStructure],
         array_length: int = 1,
         comment: Optional[str] = None,
     ) -> ComplexSymbol:
         """Add a complex (structured) symbol."""
         sym = ComplexSymbol(
             name=name,
             offset=self.next_offset,
@@ -586,16 +582,16 @@
         return sym
 
     def get_symbol_by_name(self, symbol_name: str) -> Symbol:
         return self.data_area.symbols[symbol_name]
 
 
 def map_symbols_in_memory(
-    memory: PlcMemory, symbols: typing.List[Symbol]
-) -> typing.Dict[int, typing.List[Symbol]]:
+    memory: PlcMemory, symbols: list[Symbol]
+) -> dict[int, list[Symbol]]:
     """
     Map out memory indicating where Symbols are located.
 
     Not memory or time efficient; call sparingly.
 
     Parameters
     ----------
@@ -613,15 +609,15 @@
     byte_to_symbol = {idx: [] for idx in range(len(memory))}
 
     def symbol_sort(sym):
         # In order of memory location, in reverse size (parent symbol overlap
         # with all its members -> keep parent symbol first)
         return (sym.memory_range[0], -sym.byte_size)
 
-    pointers = set(sym for sym in symbols if sym.pointer)
+    pointers = {sym for sym in symbols if sym.pointer}
     symbols = set(symbols) - pointers
 
     for sym in sorted(symbols, key=symbol_sort):
         for offset in range(*sym.memory_range):
             byte_to_symbol[offset].append(sym)
 
     for sym in pointers:
@@ -629,17 +625,17 @@
             byte_to_symbol[idx].append(sym)
 
     return byte_to_symbol
 
 
 def dump_memory(
     memory: PlcMemory,
-    symbols: typing.List[Symbol],
+    symbols: list[Symbol],
     file=sys.stdout,
-) -> typing.Dict[int, typing.List[Symbol]]:
+) -> dict[int, list[Symbol]]:
     """
     Map out memory indicating where Symbols are located and print to `file`.
 
     Not memory or time efficient; call sparingly.
 
     Parameters
     ----------
```

### Comparing `ads-async-0.3.0/ads_async/tests/kmono.tmc` & `ads-async-0.3.1/ads_async/tests/kmono.tmc`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/tests/test_server.py` & `ads-async-0.3.1/ads_async/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/tests/test_symbol.py` & `ads-async-0.3.1/ads_async/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/ads_async/utils.py` & `ads-async-0.3.1/ads_async/utils.py`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/docs/Makefile` & `ads-async-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/docs/make.bat` & `ads-async-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ads-async-0.3.0/docs/source/conf.py` & `ads-async-0.3.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
@@ -12,16 +11,14 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 from datetime import datetime
 
-import sphinx_rtd_theme
-
 module_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../../")
 sys.path.insert(0, module_path)
 
 # -- Project information -----------------------------------------------------
 
 project = "ads-async"
 author = "SLAC National Accelerator Laboratory"
@@ -41,14 +38,15 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
+    "sphinxcontrib.jquery",
     "sphinx.ext.autodoc",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
     "numpydoc",
@@ -70,15 +68,15 @@
 master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `ads-async-0.3.0/docs/source/index.rst` & `ads-async-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

