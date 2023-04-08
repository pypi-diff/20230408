# Comparing `tmp/fsspec-2023.3.0.tar.gz` & `tmp/fsspec-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsspec-2023.3.0.tar", last modified: Sat Mar  4 18:35:57 2023, max compression
+gzip compressed data, was "fsspec-2023.4.0.tar", last modified: Sat Apr  8 17:50:33 2023, max compression
```

## Comparing `fsspec-2023.3.0.tar` & `fsspec-2023.4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 18:35:57.552848 fsspec-2023.3.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.3.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.3.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     4429 2023-03-04 18:35:57.552940 fsspec-2023.3.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3108 2023-01-09 15:00:42.000000 fsspec-2023.3.0/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 18:35:57.554251 fsspec-2023.3.0/fsspec/
--rw-r--r--   0 mdurant    (502) staff       (20)     1528 2023-02-11 21:27:15.000000 fsspec-2023.3.0/fsspec/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-03-04 18:35:57.554334 fsspec-2023.3.0/fsspec/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.3.0/fsspec/archive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    32292 2023-03-03 20:38:31.000000 fsspec-2023.3.0/fsspec/asyn.py
--rw-r--r--   0 mdurant    (502) staff       (20)    25771 2023-02-28 15:02:12.000000 fsspec-2023.3.0/fsspec/caching.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/callbacks.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4193 2023-02-28 15:02:12.000000 fsspec-2023.3.0/fsspec/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.3.0/fsspec/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)    20623 2023-01-15 01:42:39.000000 fsspec-2023.3.0/fsspec/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.3.0/fsspec/dircache.py
--rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10187 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.3.0/fsspec/generic.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13766 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 18:35:57.552607 fsspec-2023.3.0/fsspec/implementations/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/implementations/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-02-13 14:39:57.000000 fsspec-2023.3.0/fsspec/implementations/arrow.py
--rw-r--r--   0 mdurant    (502) staff       (20)    30448 2023-03-04 01:48:45.000000 fsspec-2023.3.0/fsspec/implementations/cached.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4441 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/implementations/dask.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14648 2022-09-21 20:03:17.000000 fsspec-2023.3.0/fsspec/implementations/dbfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10826 2023-03-03 20:38:31.000000 fsspec-2023.3.0/fsspec/implementations/dirfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10993 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/implementations/ftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.3.0/fsspec/implementations/git.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.3.0/fsspec/implementations/github.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-02-28 15:02:12.000000 fsspec-2023.3.0/fsspec/implementations/http.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/implementations/jupyter.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/implementations/libarchive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    12508 2023-01-09 18:41:59.000000 fsspec-2023.3.0/fsspec/implementations/local.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9631 2023-01-09 15:22:42.000000 fsspec-2023.3.0/fsspec/implementations/memory.py
--rw-r--r--   0 mdurant    (502) staff       (20)    36645 2023-02-28 14:46:20.000000 fsspec-2023.3.0/fsspec/implementations/reference.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.3.0/fsspec/implementations/sftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/implementations/smb.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4088 2023-01-09 15:00:42.000000 fsspec-2023.3.0/fsspec/implementations/tar.py
--rw-r--r--   0 mdurant    (502) staff       (20)    15219 2023-01-09 15:00:42.000000 fsspec-2023.3.0/fsspec/implementations/webhdfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4212 2023-01-20 20:07:35.000000 fsspec-2023.3.0/fsspec/implementations/zip.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-02-28 15:02:12.000000 fsspec-2023.3.0/fsspec/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.3.0/fsspec/parquet.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9766 2023-03-03 20:38:31.000000 fsspec-2023.3.0/fsspec/registry.py
--rw-r--r--   0 mdurant    (502) staff       (20)    60885 2023-03-04 01:35:57.000000 fsspec-2023.3.0/fsspec/spec.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.3.0/fsspec/transaction.py
--rw-r--r--   0 mdurant    (502) staff       (20)    16659 2023-03-03 20:38:31.000000 fsspec-2023.3.0/fsspec/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 18:35:57.547065 fsspec-2023.3.0/fsspec.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     4429 2023-03-04 18:35:57.000000 fsspec-2023.3.0/fsspec.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1294 2023-03-04 18:35:57.000000 fsspec-2023.3.0/fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-03-04 18:35:57.000000 fsspec-2023.3.0/fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.3.0/fsspec.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      395 2023-03-04 18:35:57.000000 fsspec-2023.3.0/fsspec.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-03-04 18:35:57.000000 fsspec-2023.3.0/fsspec.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      384 2022-09-16 19:17:16.000000 fsspec-2023.3.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.3.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      723 2023-03-04 18:35:57.553817 fsspec-2023.3.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     2125 2023-02-13 14:39:57.000000 fsspec-2023.3.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-02-11 21:43:26.000000 fsspec-2023.3.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.894985 fsspec-2023.4.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.4.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.4.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-04-08 17:50:33.895072 fsspec-2023.4.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3464 2023-04-08 17:02:08.000000 fsspec-2023.4.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.895650 fsspec-2023.4.0/fsspec/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1800 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-08 17:50:33.895702 fsspec-2023.4.0/fsspec/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.4.0/fsspec/archive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    32277 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/asyn.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    26395 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/caching.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/callbacks.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4193 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21507 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.4.0/fsspec/dircache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10187 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.4.0/fsspec/generic.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13766 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.894748 fsspec-2023.4.0/fsspec/implementations/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-03-12 01:59:42.000000 fsspec-2023.4.0/fsspec/implementations/arrow.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    30448 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/cached.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/implementations/dask.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14648 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/implementations/dbfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10826 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/dirfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10993 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/ftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.4.0/fsspec/implementations/git.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.4.0/fsspec/implementations/github.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/implementations/http.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/jupyter.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/libarchive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    12575 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/implementations/local.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9631 2023-01-09 15:22:42.000000 fsspec-2023.4.0/fsspec/implementations/memory.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    32532 2023-04-08 16:57:33.000000 fsspec-2023.4.0/fsspec/implementations/reference.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.4.0/fsspec/implementations/sftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/implementations/smb.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4088 2023-01-09 15:00:42.000000 fsspec-2023.4.0/fsspec/implementations/tar.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    15391 2023-03-16 17:24:28.000000 fsspec-2023.4.0/fsspec/implementations/webhdfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4212 2023-01-20 20:07:35.000000 fsspec-2023.4.0/fsspec/implementations/zip.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.4.0/fsspec/parquet.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9900 2023-04-08 17:02:08.000000 fsspec-2023.4.0/fsspec/registry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    60922 2023-04-01 20:24:09.000000 fsspec-2023.4.0/fsspec/spec.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.4.0/fsspec/transaction.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    16659 2023-03-13 14:48:58.000000 fsspec-2023.4.0/fsspec/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 17:50:33.888389 fsspec-2023.4.0/fsspec.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1294 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.4.0/fsspec.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      599 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-04-08 17:50:33.000000 fsspec-2023.4.0/fsspec.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      506 2023-04-08 17:02:08.000000 fsspec-2023.4.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.4.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      723 2023-04-08 17:50:33.895424 fsspec-2023.4.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     2427 2023-04-08 17:02:08.000000 fsspec-2023.4.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-03-12 01:59:42.000000 fsspec-2023.4.0/versioneer.py
```

### Comparing `fsspec-2023.3.0/LICENSE` & `fsspec-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/PKG-INFO` & `fsspec-2023.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
@@ -36,14 +36,16 @@
 Provides-Extra: oci
 Provides-Extra: smb
 Provides-Extra: ssh
 Provides-Extra: fuse
 Provides-Extra: libarchive
 Provides-Extra: gui
 Provides-Extra: tqdm
+Provides-Extra: full
+Provides-Extra: devel
 License-File: LICENSE
 
 # filesystem_spec
 
 [![PyPI version](https://badge.fury.io/py/fsspec.svg)](https://pypi.python.org/pypi/fsspec/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/fsspec/badges/version.svg)](https://anaconda.org/conda-forge/fsspec)
 ![Build](https://github.com/fsspec/filesystem_spec/workflows/CI/badge.svg)
@@ -52,19 +54,26 @@
 A specification for pythonic filesystems.
 
 ## Install
 
 ```bash
 pip install fsspec
 ```
-or
+
+would install the base fsspec. Various optionally supported features might require specification of custom
+extra require, e.g. `pip install fsspec[ssh]` will install dependencies for `ssh` backends support.
+Use `pip install fsspec[full]` for installation of all known extra dependencies.
+
+Up-to-date package also provided through conda-forge distribution:
+
 ```bash
 conda install -c conda-forge fsspec
 ```
 
+
 ## Purpose
 
 To produce a template or specification for a file-system interface, that specific implementations should follow,
 so that applications making use of them can rely on a common behaviour and not have to worry about the specific
 internal implementation decisions with any given backend. Many such implementations are included in this package,
 or in sister projects such as `s3fs` and `gcsfs`.
```

### Comparing `fsspec-2023.3.0/README.md` & `fsspec-2023.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,26 @@
 A specification for pythonic filesystems.
 
 ## Install
 
 ```bash
 pip install fsspec
 ```
-or
+
+would install the base fsspec. Various optionally supported features might require specification of custom
+extra require, e.g. `pip install fsspec[ssh]` will install dependencies for `ssh` backends support.
+Use `pip install fsspec[full]` for installation of all known extra dependencies.
+
+Up-to-date package also provided through conda-forge distribution:
+
 ```bash
 conda install -c conda-forge fsspec
 ```
 
+
 ## Purpose
 
 To produce a template or specification for a file-system interface, that specific implementations should follow,
 so that applications making use of them can rely on a common behaviour and not have to worry about the specific
 internal implementation decisions with any given backend. Many such implementations are included in this package,
 or in sister projects such as `s3fs` and `gcsfs`.
```

### Comparing `fsspec-2023.3.0/fsspec/__init__.py` & `fsspec-2023.4.0/fsspec/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,12 +47,18 @@
             if hasattr(eps, "select"):  # Python 3.10+ / importlib_metadata >= 3.9.0
                 specs = eps.select(group="fsspec.specs")
             else:
                 specs = eps.get("fsspec.specs", [])
             for spec in specs:
                 err_msg = f"Unable to load filesystem from {spec}"
                 register_implementation(
-                    spec.name, spec.value.replace(":", "."), errtxt=err_msg
+                    spec.name,
+                    spec.value.replace(":", "."),
+                    errtxt=err_msg,
+                    # We take our implementations as the ones to overload with if
+                    # for some reason we encounter some, may be the same, already
+                    # registered
+                    clobber=True,
                 )
 
 
 process_entries()
```

### Comparing `fsspec-2023.3.0/fsspec/archive.py` & `fsspec-2023.4.0/fsspec/archive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/asyn.py` & `fsspec-2023.4.0/fsspec/asyn.py`

 * *Files 1% similar despite different names*

```diff
@@ -956,25 +956,25 @@
             self.offset = 0
             try:
                 await self._initiate_upload()
             except:  # noqa: E722
                 self.closed = True
                 raise
 
-        if self._upload_chunk(final=force) is not False:
+        if await self._upload_chunk(final=force) is not False:
             self.offset += self.buffer.seek(0, 2)
             self.buffer = io.BytesIO()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     async def _fetch_range(self, start, end):
         raise NotImplementedError
 
     async def _initiate_upload(self):
-        raise NotImplementedError
+        pass
 
     async def _upload_chunk(self, final=False):
         raise NotImplementedError
```

### Comparing `fsspec-2023.3.0/fsspec/caching.py` & `fsspec-2023.4.0/fsspec/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -657,30 +657,33 @@
             # Background thread is running. Check we we can or must join it.
             if self._fetch_future is not None:
                 if self._fetch_future.done():
                     logger.info("BlockCache joined background fetch without waiting.")
                     self._fetch_block_cached.add_key(
                         self._fetch_future.result(), self._fetch_future_block_number
                     )
+                    # Cleanup the fetch variables. Done with fetching the block.
+                    self._fetch_future_block_number = None
+                    self._fetch_future = None
                 else:
                     # Must join if we need the block for the current fetch
                     must_join = bool(
                         start_block_number
                         <= self._fetch_future_block_number
                         <= end_block_number
                     )
                     if must_join:
                         # Copy to the local variables to release lock
                         # before waiting for result
                         fetch_future_block_number = self._fetch_future_block_number
                         fetch_future = self._fetch_future
 
-            # Cleanup the fetch variables. Either done or have a local copy.
-            self._fetch_future_block_number = None
-            self._fetch_future = None
+                        # Cleanup the fetch variables. Have a local copy.
+                        self._fetch_future_block_number = None
+                        self._fetch_future = None
 
         # Need to wait for the future for the current read
         if fetch_future is not None:
             logger.info("BlockCache waiting for background fetch.")
             # Wait until result and put it in cache
             self._fetch_block_cached.add_key(
                 fetch_future.result(), fetch_future_block_number
@@ -760,18 +763,43 @@
             # final block
             out.append(self._fetch_block_cached(end_block_number)[:end_pos])
 
             return b"".join(out)
 
 
 caches = {
-    "none": BaseCache,
+    # one custom case
     None: BaseCache,
-    "mmap": MMapCache,
-    "bytes": BytesCache,
-    "readahead": ReadAheadCache,
-    "block": BlockCache,
-    "first": FirstChunkCache,
-    "all": AllBytes,
-    "parts": KnownPartsOfAFile,
-    "background": BackgroundBlockCache,
 }
+
+
+def register_cache(cls, clobber=False):
+    """'Register' cache implementation.
+
+    Parameters
+    ----------
+    clobber: bool, optional
+        If set to True (default is False) - allow to overwrite existing
+        entry.
+
+    Raises
+    ------
+    ValueError
+    """
+    name = cls.name
+    if not clobber and name in caches:
+        raise ValueError(f"Cache with name {name!r} is already known: {caches[name]}")
+    caches[name] = cls
+
+
+for c in (
+    BaseCache,
+    MMapCache,
+    BytesCache,
+    ReadAheadCache,
+    BlockCache,
+    FirstChunkCache,
+    AllBytes,
+    KnownPartsOfAFile,
+    BackgroundBlockCache,
+):
+    register_cache(c)
```

### Comparing `fsspec-2023.3.0/fsspec/callbacks.py` & `fsspec-2023.4.0/fsspec/callbacks.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/compression.py` & `fsspec-2023.4.0/fsspec/compression.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/config.py` & `fsspec-2023.4.0/fsspec/config.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/conftest.py` & `fsspec-2023.4.0/fsspec/conftest.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/core.py` & `fsspec-2023.4.0/fsspec/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -264,14 +264,24 @@
     ...     's3://bucket/2015-*-*.csv.gz', compression='gzip'
     ... )  # doctest: +SKIP
 
     Returns
     -------
     An ``OpenFiles`` instance, which is a list of ``OpenFile`` objects that can
     be used as a single context
+
+    Notes
+    -----
+    For a full list of the available protocols and the implementations that
+    they map across to see the latest online documentation:
+
+    - For implementations built into ``fsspec`` see
+      https://filesystem-spec.readthedocs.io/en/latest/api.html#built-in-implementations
+    - For implementations in separate packages see
+      https://filesystem-spec.readthedocs.io/en/latest/api.html#other-known-implementations
     """
     fs, fs_token, paths = get_fs_token_paths(
         urlpath,
         mode,
         num=num,
         name_function=name_function,
         storage_options=kwargs,
@@ -411,14 +421,24 @@
     >>> with openfile as f:
     ...     df = pd.read_csv(f)  # doctest: +SKIP
     ...
 
     Returns
     -------
     ``OpenFile`` object.
+
+    Notes
+    -----
+    For a full list of the available protocols and the implementations that
+    they map across to see the latest online documentation:
+
+    - For implementations built into ``fsspec`` see
+      https://filesystem-spec.readthedocs.io/en/latest/api.html#built-in-implementations
+    - For implementations in separate packages see
+      https://filesystem-spec.readthedocs.io/en/latest/api.html#other-known-implementations
     """
     return open_files(
         urlpath=[urlpath],
         mode=mode,
         compression=compression,
         encoding=encoding,
         errors=errors,
```

### Comparing `fsspec-2023.3.0/fsspec/dircache.py` & `fsspec-2023.4.0/fsspec/dircache.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/fuse.py` & `fsspec-2023.4.0/fsspec/fuse.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/generic.py` & `fsspec-2023.4.0/fsspec/generic.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/gui.py` & `fsspec-2023.4.0/fsspec/gui.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/arrow.py` & `fsspec-2023.4.0/fsspec/implementations/arrow.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/cached.py` & `fsspec-2023.4.0/fsspec/implementations/cached.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/dask.py` & `fsspec-2023.4.0/fsspec/implementations/dask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dask
 from distributed.client import Client, _get_global_client
-from distributed.worker import get_worker
+from distributed.worker import Worker
 
 from fsspec import filesystem
 from fsspec.spec import AbstractBufferedFile, AbstractFileSystem
 from fsspec.utils import infer_storage_options
 
 
 def _get_client(client):
@@ -13,14 +13,18 @@
     elif isinstance(client, Client):
         return client
     else:
         # e.g., connection string
         return Client(client)
 
 
+def _in_worker():
+    return bool(Worker._instances)
+
+
 class DaskWorkerFileSystem(AbstractFileSystem):
     """View files accessible to a worker as any other remote file-system
 
     When instances are run on the worker, uses the real filesystem. When
     run on the client, they call the worker to provide information or data.
 
     **Warning** this implementation is experimental, and read-only for now.
@@ -47,22 +51,21 @@
         so = infer_storage_options(path)
         if "host" in so and "port" in so:
             return {"client": f"{so['host']}:{so['port']}"}
         else:
             return {}
 
     def _determine_worker(self):
-        try:
-            get_worker()
+        if _in_worker():
             self.worker = True
             if self.fs is None:
                 self.fs = filesystem(
                     self.target_protocol, **(self.target_options or {})
                 )
-        except ValueError:
+        else:
             self.worker = False
             self.client = _get_client(self.client)
             self.rfs = dask.delayed(self)
 
     def mkdir(self, *args, **kwargs):
         if self.worker:
             self.fs.mkdir(*args, **kwargs)
```

### Comparing `fsspec-2023.3.0/fsspec/implementations/dbfs.py` & `fsspec-2023.4.0/fsspec/implementations/dbfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/dirfs.py` & `fsspec-2023.4.0/fsspec/implementations/dirfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/ftp.py` & `fsspec-2023.4.0/fsspec/implementations/ftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/git.py` & `fsspec-2023.4.0/fsspec/implementations/git.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/github.py` & `fsspec-2023.4.0/fsspec/implementations/github.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/http.py` & `fsspec-2023.4.0/fsspec/implementations/http.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/jupyter.py` & `fsspec-2023.4.0/fsspec/implementations/jupyter.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/libarchive.py` & `fsspec-2023.4.0/fsspec/implementations/libarchive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/local.py` & `fsspec-2023.4.0/fsspec/implementations/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
             return cls.root_marker
 
     @classmethod
     def _strip_protocol(cls, path):
         path = stringify_path(path)
         if path.startswith("file://"):
             path = path[7:]
+        elif path.startswith("file:"):
+            path = path[5:]
         return make_path_posix(path).rstrip("/") or cls.root_marker
 
     def _isfilestore(self):
         # Inheriting from DaskFileSystem makes this False (S3, etc. were)
         # the original motivation. But we are a posix-like file system.
         # See https://github.com/dask/dask/issues/5526
         return True
```

### Comparing `fsspec-2023.3.0/fsspec/implementations/memory.py` & `fsspec-2023.4.0/fsspec/implementations/memory.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/reference.py` & `fsspec-2023.4.0/fsspec/implementations/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import ast
 import base64
+import collections
 import io
 import itertools
 import logging
 import os
 from functools import lru_cache
 
 import fsspec.core
@@ -12,15 +12,14 @@
     import ujson as json
 except ImportError:
     import json
 
 from ..asyn import AsyncFileSystem
 from ..callbacks import _DEFAULT_CALLBACK
 from ..core import filesystem, open, split_protocol
-from ..spec import AbstractFileSystem
 from ..utils import isfilelike, merge_offset_ranges, other_paths
 
 logger = logging.getLogger("fsspec.reference")
 
 
 class ReferenceNotReachable(RuntimeError):
     def __init__(self, reference, target, *args):
@@ -48,32 +47,240 @@
     out = {}
     for path in paths:
         protocol = _prot_in_references(path, references)
         out.setdefault(protocol, []).append(path)
     return out
 
 
+class RefsValuesView(collections.abc.ValuesView):
+    def __iter__(self):
+        for val in self._mapping.zmetadata.values():
+            yield json.dumps(val).encode()
+        yield from self._mapping._items.values()
+        for field in self._mapping.listdir():
+            chunk_sizes = self._mapping._get_chunk_sizes(field)
+            if chunk_sizes.size == 0:
+                yield self._mapping[field + "/0"]
+                continue
+            yield from self._mapping._generate_all_records(field)
+
+
+class RefsItemsView(collections.abc.ItemsView):
+    def __iter__(self):
+        return zip(self._mapping.keys(), self._mapping.values())
+
+
+class LazyReferenceMapper(collections.abc.MutableMapping):
+    """Interface to read parquet store as if it were a standard kerchunk
+    references dict."""
+
+    # import is class level to prevent numpy dep requirement for fsspec
+    @property
+    def np(self):
+        import numpy as np
+
+        return np
+
+    @property
+    def pd(self):
+        import pandas as pd
+
+        return pd
+
+    def __init__(
+        self,
+        root,
+        fs=None,
+        cache_size=128,
+    ):
+        """
+        Parameters
+        ----------
+        root : str
+            Root of parquet store
+        fs : fsspec.AbstractFileSystem
+            fsspec filesystem object, default is local filesystem.
+        cache_size : int
+            Maximum size of LRU cache, where cache_size*record_size denotes
+            the total number of references that can be loaded in memory at once.
+        """
+        self.root = root
+        self.chunk_sizes = {}
+        self._items = {}
+        self.dirs = None
+        self.fs = fsspec.filesystem("file") if fs is None else fs
+        with self.fs.open("/".join([self.root, ".zmetadata"]), "rb") as f:
+            self._items[".zmetadata"] = f.read()
+        met = json.loads(self._items[".zmetadata"])
+        self.record_size = met["record_size"]
+        self.zmetadata = met["metadata"]
+        if self.root:
+            self.url = self.root + "/{field}/refs.{record}.parq"
+        else:
+            self.url = "{field}/refs.{record}.parq"
+
+        # Define function to open and decompress refs
+        @lru_cache(maxsize=cache_size)
+        def open_refs(field, record):
+            path = self.url.format(field=field, record=record)
+            with self.fs.open(path) as f:
+                df = self.pd.read_parquet(f, engine="fastparquet")
+            refs = {c: df[c].values for c in df.columns}
+            # Return both df and dict of views because the former is
+            # more convenient for iterating sequentially while the latter
+            # is faster for random access.
+            return df, refs
+
+        self.open_refs = open_refs
+
+    def listdir(self, basename=True):
+        if self.dirs is None:
+            dirs = [p.split("/", 1)[0] for p in self.zmetadata]
+            self.dirs = set(sorted(p for p in dirs if p and not p.startswith(".")))
+        listing = self.dirs
+        if basename:
+            listing = [os.path.basename(path) for path in listing]
+        return listing
+
+    def _load_one_key(self, key):
+        if key in self._items:
+            return self._items[key]
+        elif key in self.zmetadata:
+            return json.dumps(self.zmetadata[key]).encode()
+        elif "/" not in key:
+            raise KeyError(key)
+        field, sub_key = key.split("/")
+        # Chunk keys can be loaded from row group and cached in LRU cache
+        try:
+            record, ri, chunk_size = self._key_to_record(key)
+            if chunk_size == 0:
+                return b""
+            _, refs = self.open_refs(field, record)
+        except (ValueError, TypeError, FileNotFoundError):
+            raise KeyError(key)
+        columns = ["path", "offset", "size", "raw"]
+        selection = [refs[c][ri] if c in refs else None for c in columns]
+        raw = selection[-1]
+        if raw is not None:
+            return raw
+        data = selection[:-1]
+        if data[1:] == [0, 0]:
+            data = data[:1]
+        return data
+
+    def _key_to_record(self, key):
+        field, chunk = key.split("/")
+        chunk_sizes = self._get_chunk_sizes(field)
+        if chunk_sizes.size == 0:
+            return 0, 0, 0
+        chunk_idx = self.np.array([int(c) for c in chunk.split(".")])
+        chunk_number = self.np.ravel_multi_index(chunk_idx, chunk_sizes)
+        record = chunk_number // self.record_size
+        ri = chunk_number % self.record_size
+        return record, ri, chunk_sizes.size
+
+    def _get_chunk_sizes(self, field):
+        if field not in self.chunk_sizes:
+            zarray = self.zmetadata[f"{field}/.zarray"]
+            size_ratio = self.np.array(zarray["shape"]) / self.np.array(
+                zarray["chunks"]
+            )
+            self.chunk_sizes[field] = self.np.ceil(size_ratio).astype(int)
+        return self.chunk_sizes[field]
+
+    def _generate_record(self, field, record):
+        df, _ = self.open_refs(field, record)
+        it = df.itertuples(name=None, index=False)
+        if df.columns.size == 3:
+            # All urls
+            return (list(t) for t in it)
+        elif df.columns.size == 1:
+            # All raws
+            return (t[0] for t in it)
+        else:
+            # Mix of urls and raws
+            return (list(t[:3]) if not t[3] else t[3] for t in it)
+
+    def _generate_all_records(self, field):
+        chunk_size = self._get_chunk_sizes(field)
+        nrec = int(self.np.ceil(self.np.product(chunk_size) / self.record_size))
+        for record in range(nrec):
+            yield from self._generate_record(field, record)
+
+    def values(self):
+        return RefsValuesView(self)
+
+    def items(self):
+        return RefsItemsView(self)
+
+    def __getitem__(self, key):
+        if key in self._items:
+            val = self._items[key]
+            if val is None:
+                raise KeyError
+        if key in self.zmetadata:
+            # spec requires bytes even if we already decoded the metadata
+            return json.dumps(self.zmetadata[key]).encode()
+        return self._load_one_key(key)
+
+    def __setitem__(self, key, value):
+        self._items[key] = value
+
+    def __delitem__(self, key):
+        if key in self._items:
+            del self._items[key]
+        elif key in self.zmetadata:
+            del self.zmetadata[key]
+        else:
+            # TODO: Add method to RefFs that tracks changes in _items
+            # and updates / copies appropriate parquet ref files.
+            self._items[key] = None
+
+    def __len__(self):
+        # Caveat: This counts expected references, not actual
+        count = 0
+        for field in self.listdir():
+            if field.startswith("."):
+                count += 1
+            else:
+                chunk_sizes = self._get_chunk_sizes(field)
+                nchunks = self.np.product(chunk_sizes)
+                count += nchunks
+        count += len(self.zmetadata)  # all metadata keys
+        count += len(self._items)  # the metadata file itself
+        return count
+
+    def __iter__(self):
+        # Caveat: Note that this generates all expected keys, but does not
+        # account for reference keys that are missing.
+        yield from self.zmetadata
+        yield from self._items
+        for field in self.listdir():
+            chunk_sizes = self._get_chunk_sizes(field)
+            if chunk_sizes.size == 0:
+                yield field + "/0"
+                continue
+            inds = self.np.ndindex(*chunk_sizes)
+            for ind in inds:
+                yield field + "/" + ".".join([str(c) for c in ind])
+
+
 class ReferenceFileSystem(AsyncFileSystem):
     """View byte ranges of some other file as a file system
-
     Initial version: single file system target, which must support
     async, and must allow start and end args in _cat_file. Later versions
     may allow multiple arbitrary URLs for the targets.
-
     This FileSystem is read-only. It is designed to be used with async
     targets (for now). This FileSystem only allows whole-file access, no
     ``open``. We do not get original file details from the target FS.
-
     Configuration is by passing a dict of references at init, or a URL to
     a JSON file containing the same; this dict
     can also contain concrete data for some set of paths.
-
     Reference dict format:
     {path0: bytes_data, path1: (target_url, offset, size)}
-
     https://github.com/fsspec/kerchunk/blob/main/README.md
     """
 
     protocol = "reference"
 
     def __init__(
         self,
@@ -85,24 +292,26 @@
         remote_protocol=None,
         remote_options=None,
         fs=None,
         template_overrides=None,
         simple_templates=True,
         max_gap=64_000,
         max_block=256_000_000,
+        cache_size=128,
         **kwargs,
     ):
         """
-
         Parameters
         ----------
         fo : dict or str
             The set of references to use for this instance, with a structure as above.
-            If str, will use fsspec.open, in conjunction with target_options
-            and target_protocol to open and parse JSON at this location.
+            If str referencing a JSON file, will use fsspec.open, in conjunction
+            with target_options and target_protocol to open and parse JSON at this
+            location. If a directory, then assume references are a set of parquet
+            files to be loaded lazily.
         target : str
             For any references having target_url as None, this is the default file
             target to use
         ref_storage_args : dict
             If references is a str, use these kwargs for loading the JSON file.
             Deprecated: use target_options instead.
         target_protocol : str
@@ -136,42 +345,50 @@
             For merging multiple concurrent requests to the same remote file.
             Neighboring byte ranges will only be merged when their
             inter-range gap is <= ``max_gap``. Default is 64KB. Set to 0
             to only merge when it requires no extra bytes. Pass a negative
             number to disable merging, appropriate for local target files.
             Neighboring byte ranges will only be merged when the size of
             the aggregated range is <= ``max_block``. Default is 256MB.
+        cache_size : int
+            Maximum size of LRU cache, where cache_size*record_size denotes
+            the total number of references that can be loaded in memory at once.
+            Only used for lazily loaded references.
         kwargs : passed to parent class
         """
         super().__init__(**kwargs)
         self.target = target
         self.template_overrides = template_overrides
         self.simple_templates = simple_templates
         self.templates = {}
         self.fss = {}
         self._dircache = {}
         self.max_gap = max_gap
         self.max_block = max_block
-        if hasattr(fo, "read"):
-            text = json.load(fo)
-            text = text.decode() if isinstance(text, bytes) else text
-        elif isinstance(fo, str):
-            if target_protocol:
-                extra = {"protocol": target_protocol}
-            else:
-                extra = {}
-            dic = dict(**(ref_storage_args or target_options or {}), **extra)
-            # text JSON
-            with open(fo, "rb", **dic) as f:
-                logger.info("Read reference from URL %s", fo)
-                text = json.load(f)
+        if isinstance(fo, str):
+            dic = dict(
+                **(ref_storage_args or target_options or {}), protocol=target_protocol
+            )
+            ref_fs, fo = fsspec.core.url_to_fs(fo, **dic)
+            if ref_fs.isfile(fo):
+                # text JSON
+                with ref_fs.open(fo, "rb") as f:
+                    logger.info("Read reference from URL %s", fo)
+                    text = json.load(f)
+                self._process_references(text, template_overrides)
+            else:
+                # Lazy parquet refs
+                self.references = LazyReferenceMapper(
+                    fo,
+                    fs=ref_fs,
+                    cache_size=cache_size,
+                )
         else:
             # dictionaries
-            text = fo
-        self._process_references(text, template_overrides)
+            self._process_references(fo, template_overrides)
         if isinstance(fs, dict):
             self.fss = {
                 k: (
                     fsspec.filesystem(k.split(":", 1)[0], **opts)
                     if isinstance(opts, dict)
                     else opts
                 )
@@ -225,15 +442,15 @@
         if isinstance(part, bytes):
             logger.debug(f"Reference: {path}, type bytes")
             if part.startswith(b"base64:"):
                 part = base64.b64decode(part[7:])
             return part, None, None
 
         if len(part) == 1:
-            logger.debug(f"Reference: {path}, whole file")
+            logger.debug(f"Reference: {path}, whole file => {part}")
             url = part[0]
             start1, end1 = start, end
         else:
             url, start0, size = part
             logger.debug(f"Reference: {path} => {url}, offset {start0}, size {size}")
             end0 = start0 + size
 
@@ -414,17 +631,14 @@
         else:
             raise ValueError(f"Unknown reference spec version: {vers}")
         # TODO: we make dircache by iterating over all entries, but for Spec >= 1,
         #  can replace with programmatic. Is it even needed for mapper interface?
 
     def _process_references0(self, references):
         """Make reference dict for Spec Version 0"""
-        if "zarr_consolidated_format" in references:
-            # special case for Ike prototype
-            references = _unmodel_hdf5(references)
         self.references = references
 
     def _process_references1(self, references, template_overrides=None):
         if not self.simple_templates or self.templates:
             import jinja2
         self.references = {}
         self._process_templates(references.get("templates", {}))
@@ -627,332 +841,7 @@
                     out[k] = v.decode("ascii")
                 except UnicodeDecodeError:
                     out[k] = (b"base64:" + base64.b64encode(v)).decode()
             else:
                 out[k] = v
         with fsspec.open(url, "wb", **storage_options) as f:
             f.write(json.dumps({"version": 1, "refs": out}).encode())
-
-
-def prefix(x):
-    if "/.z" in x or "/" not in x:
-        return "metadata", x
-    return x.split("/", 1)
-
-
-def constant_prefix(x):
-    return "metadata", x
-
-
-class DFReferenceFileSystem(AbstractFileSystem):
-    """
-    (Experimental) Parquet-based Reference Filesystem
-
-    Putative replacement or adjunct to ReferenceFileSystem with
-    additional capabilities:
-    - loads from parquet for better on-disk and in-memory space
-    - optional lazy loading by key prefix (lazy=True)
-    - multiple targets for a given key (allow_multi=True), concatenated
-      together by default, of multi_func=
-    - per-chunk processing with extra parameters stored in the parquet
-      (chunk_func=)
-
-    This implementation is not (yet) multable.
-    """
-
-    def __init__(
-        self,
-        fo,
-        target_options=None,
-        remote_protocol=None,
-        remote_options=None,
-        fs=None,
-        max_gap=64_000,
-        max_block=256_000_000,
-        parquet_kwargs=None,
-        chunk_func=None,
-        allow_multi=False,
-        multi_func=b"".join,
-        prefix_func=prefix,
-        lazy=False,
-        **kwargs,
-    ):
-        self.fo = fo
-        self.target_options = target_options or {}
-        self.max_gap = max_gap
-        self.max_block = max_block
-        self.dataframes = {}
-        self.keysets = {}
-        self.url_dict = {}
-        self.template_dict = {}
-        self.prefs = None
-        self.fss = {}
-        self.dirs = None
-        self.lazy = lazy
-        self.chunk_func = chunk_func
-        self.allow_multi = allow_multi
-        self.multi_func = multi_func
-        self.prefix_func = prefix_func if lazy else constant_prefix
-        self.pkwargs = parquet_kwargs or {}
-        if fs is not None:
-            # single remote FS
-            remote_protocol = (
-                fs.protocol[0] if isinstance(fs.protocol, tuple) else fs.protocol
-            )
-            self.fss[remote_protocol] = fs
-
-        if remote_protocol and remote_protocol not in self.fss:
-            fs = filesystem(remote_protocol, **(remote_options or {}))
-            self.fss[remote_protocol] = fs
-
-        if fs:
-            self.fss[None] = fs
-        elif self.fss:
-            self.fss[None] = iter(self.fss.values()).__next__()
-        else:
-            self.fss[None] = fsspec.filesystem(
-                remote_protocol, **(remote_options or {})
-            )
-
-        super().__init__(**kwargs)
-        self._reference_part()
-
-    def _reference_part(self, part="metadata"):
-        """Load some references from parquet
-
-        If lazy is False, this is called exactly once per instance
-
-        If lazy is true, selecting a path will determine the name of
-        the target parquet file, and the resultant columns will be
-        cached so the file need not be read again
-        """
-        import fastparquet
-
-        if part != "metadata" and part not in self.dirs:
-            raise FileNotFoundError(f"prefix {part}")
-        if part not in self.dataframes:
-            url = f"{self.fo}/{part}.parq" if self.lazy else self.fo
-            fs, path = fsspec.core.url_to_fs(url, **self.target_options)
-            pf = fastparquet.ParquetFile(path, fs=fs)
-            self.template_dict[part] = pf.key_value_metadata
-            df = pf.to_pandas()
-            thispart = {}
-            for k in df:
-                if df[k].dtype == "category" and k == "path":
-                    self.url_dict[part] = df[k].cat.categories.values
-                    thispart[k] = df[k].cat.codes.values
-                else:
-                    thispart[k] = df[k].values
-            self.dataframes[part] = thispart
-            if self.allow_multi is False:
-                self.keysets[part] = {
-                    k: i for (i, k) in enumerate(self.dataframes[part]["key"])
-                }
-            else:
-                self.keysets[part] = {}
-                for i, k in enumerate(self.dataframes[part]["key"]):
-                    self.keysets[part].setdefault(k, []).append(i)
-            if part == "metadata":
-                self.dirs = {
-                    k.rsplit("/", 1)[0]
-                    for k in self.dataframes[part]["key"]
-                    if "/" in k
-                }
-                self.prefs = (
-                    ast.literal_eval(pf.key_value_metadata["prefs"])
-                    if "prefs" in pf.key_value_metadata
-                    else set()
-                )
-
-        return self.dataframes[part]
-
-    def isdir(self, path):
-        return path in self.dirs
-
-    def cat_file(self, path, start=None, end=None, **kwargs):
-        return self.cat_ranges([path], [start], [end])[0]
-
-    def cat(self, path, recursive=False, on_error="return", **kwargs):
-        paths = self.expand_path(path, recursive=recursive)
-        paths1 = [p for p in paths if not self.isdir(p)]
-        result = {
-            p: data
-            for p, data in zip(
-                paths1, self.cat_ranges(paths1, on_error=on_error, **kwargs)
-            )
-        }
-        if len(paths1) == 1 and recursive is False and "*" not in path:
-            # same as cat_file
-            return list(result.values())[0]
-        return result
-
-    def cat_ranges(self, paths, starts=None, ends=None, on_error="return", **kwargs):
-        out = []  # eventual output; initially each key contains raw bytes or None
-        proto_dict = {}  # mapping of protocol to lists of URL/start/end to fetch
-        assign_dict = {}  # how to assign the results of cat_ranges to output
-        if starts is None:
-            starts = [None] * len(paths)
-        if ends is None:
-            ends = [None] * len(paths)
-        for p, s, e in zip(paths, starts, ends):
-            thislist = []
-            out.append(thislist)
-            if self.lazy:
-                pref, p0 = self.prefix_func(p)
-                if pref in self.prefs:
-                    # reference already inlined in metadata file
-                    pref = "metadata"
-                else:
-                    # new key in the target pref file
-                    p = p0
-            else:
-                # everything is in the same file
-                pref = "metadata"
-            self._reference_part(pref)
-            inds = self.keysets[pref][p]
-            if isinstance(inds, int):
-                inds = [inds]
-            for i in inds:
-                if x := self.dataframes[pref]["raw"][i]:
-                    thislist.append(x)
-                else:
-                    # infer path - cache this?
-                    path = self.dataframes[pref]["path"][i]
-                    if pref in self.url_dict:
-                        # dict-encoded columns; actually, numpy can do
-                        # many of these at once with int fancy indexing
-                        path = self.url_dict[pref][path]
-                    # apply template: common prefix
-                    path = path.format(**self.template_dict[pref])
-
-                    prot, _ = split_protocol(path)
-                    proto_dict.setdefault(prot, [[], [], []])
-                    proto_dict[prot][0].append(path)
-                    if s is None or s >= 0:
-                        proto_dict[prot][1].append(
-                            self.dataframes[pref]["offset"][i] or s
-                        )
-                    else:
-                        # range is from end of file, which we do not know
-                        # the size of, so this can only work if there is no
-                        # merging
-                        proto_dict[prot][1].append(s)
-
-                    if e is None or e >= 0:
-                        proto_dict[prot][2].append(
-                            self.dataframes[pref]["offset"][i]
-                            + self.dataframes[pref]["size"][i]
-                            or e
-                        )
-                    else:
-                        # range is from end of file, which we do not know
-                        # the size of, so this can only work if there is no
-                        # merging
-                        proto_dict[prot][1].append(e)
-                    thislist.append(None)
-                    assign_dict.setdefault(prot, []).append(
-                        (thislist, len(thislist) - 1)
-                    )
-
-        for proto, (urls2, starts2, ends2) in proto_dict.items():
-            fs = self.fss[proto]
-
-            new_paths, new_starts, new_ends = merge_offset_ranges(
-                list(urls2),
-                list(starts2),
-                list(ends2),
-                sort=True,
-                max_gap=self.max_gap,
-                max_block=self.max_block,
-            )
-            bytes_out = fs.cat_ranges(new_paths, new_starts, new_ends)
-            if len(urls2) == len(bytes_out):
-                # we didn't do any merging
-                for (l, i), d in zip(assign_dict[proto], bytes_out):
-                    l[i] = d
-            else:
-                # unbundle from merged bytes - simple approach
-                for u, s, e, (l, i) in zip(urls2, starts2, ends2, assign_dict[proto]):
-                    if p in out:
-                        continue  # was bytes, already handled
-                    for np, ns, ne, b in zip(
-                        new_paths, new_starts, new_ends, bytes_out
-                    ):
-                        if np == u and (ns is None or ne is None):
-                            l[i] = b[s:e]
-                        elif np == u and s >= ns and e <= ne:
-                            l[i] = b[s - ns : (e - ne) or None]
-
-        out = [self.multi_func(part) for part in out]
-        return out
-
-    def find(self, path, detail=False, withdirs=False, **kwargs):
-        path = self._strip_protocol(path)
-        if path in self.dirs:
-            path = path + "/"
-        pref, p = self.prefix_func(path)
-        dirs = (
-            [
-                {"name": d, "size": 0, "type": "directory"}
-                for d in self.dirs
-                if d.startswith(path)
-            ]
-            if withdirs
-            else []
-        )
-        if pref in self.prefs:
-            pref = "metadata"
-        df = self._reference_part(pref)
-        files = [
-            {"name": k, "type": "file", "size": _size(self.dataframes["metadata"], i)}
-            for k, i in self.keysets["metadata"].items()
-            if k.startswith(path)
-        ]
-        if self.lazy and pref != "metadata":
-            files.extend(
-                [
-                    {"name": f"{pref}/{k}", "type": "file", "size": _size(df, i)}
-                    for k, i in self.keysets[pref].items()
-                    if k.startswith(p)
-                ]
-            )
-        if detail:
-            return dirs + files
-        return [k["name"] for k in dirs + files]
-
-    def ls(self, path, detail=True, **kwargs):
-        path = self._strip_protocol(path)
-        allfiles = self.find(path, detail=True, withdirs=True)
-        isdir = path in self.dirs
-        subdfiles = [
-            p for p in allfiles if p["name"].count("/") == path.count("/") + isdir
-        ]
-        if detail:
-            return subdfiles
-        return [p["name"] for p in subdfiles]
-
-    def info(self, path, **kwargs):
-        path = self._strip_protocol(path)
-
-        if path in self.dirs:
-            return {"name": path, "type": "directory", "Size": 0}
-        return self.ls(path, detail=True)[0]
-
-
-def _size(df, i):
-    if isinstance(i, int):
-        return len(df["raw"][i]) if df["raw"][i] else df["size"][i]
-    return sum(len(df["raw"][_]) if df["raw"][_] else df["size"][_] for _ in i)
-
-
-def _unmodel_hdf5(references):
-    """Special JSON format from HDF5 prototype"""
-    # see https://gist.github.com/ajelenak/80354a95b449cedea5cca508004f97a9
-    ref = {}
-    for key, value in references["metadata"].items():
-        if key.endswith(".zchunkstore"):
-            source = value.pop("source")["uri"]
-            for k, v in value.items():
-                ref[k] = (source, v["offset"], v["offset"] + v["size"])
-        else:
-            ref[key] = json.dumps(value).encode()
-    return ref
```

### Comparing `fsspec-2023.3.0/fsspec/implementations/sftp.py` & `fsspec-2023.4.0/fsspec/implementations/sftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/smb.py` & `fsspec-2023.4.0/fsspec/implementations/smb.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/tar.py` & `fsspec-2023.4.0/fsspec/implementations/tar.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/implementations/webhdfs.py` & `fsspec-2023.4.0/fsspec/implementations/webhdfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,15 +416,17 @@
         location = self.fs._apply_proxy(out.headers["Location"])
         if "w" in self.mode:
             # create empty file to append to
             out2 = self.fs.session.put(
                 location, headers={"content-type": "application/octet-stream"}
             )
             out2.raise_for_status()
-        self.location = location.replace("CREATE", "APPEND")
+            # after creating empty file, change location to append to
+            out2 = self.fs._call("APPEND", "POST", self.path, redirect=False, **kwargs)
+            self.location = self.fs._apply_proxy(out2.headers["Location"])
 
     def _fetch_range(self, start, end):
         start = max(start, 0)
         end = min(self.size, end)
         if start >= end or start >= self.size:
             return b""
         out = self.fs._call(
```

### Comparing `fsspec-2023.3.0/fsspec/implementations/zip.py` & `fsspec-2023.4.0/fsspec/implementations/zip.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/mapping.py` & `fsspec-2023.4.0/fsspec/mapping.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/parquet.py` & `fsspec-2023.4.0/fsspec/parquet.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/registry.py` & `fsspec-2023.4.0/fsspec/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 _registry = {}
 
 # external, immutable
 registry = types.MappingProxyType(_registry)
 default = "file"
 
 
-def register_implementation(name, cls, clobber=True, errtxt=None):
+def register_implementation(name, cls, clobber=False, errtxt=None):
     """Add implementation class to the registry
 
     Parameters
     ----------
     name: str
         Protocol name to associate with the class
     cls: class or str
@@ -175,14 +175,18 @@
         "class": "webdav4.fsspec.WebdavFileSystem",
         "err": "Install webdav4 to access WebDAV",
     },
     "dvc": {
         "class": "dvc.api.DVCFileSystem",
         "err": "Install dvc to access DVCFileSystem",
     },
+    "hf": {
+        "class": "huggingface_hub.HfFileSystem",
+        "err": "Install huggingface_hub to access HfFileSystem",
+    },
     "root": {
         "class": "fsspec_xrootd.XRootDFileSystem",
         "err": "Install fsspec-xrootd to access xrootd storage system."
         + " Note: 'root' is the protocol name for xrootd storage systems,"
         + " not referring to root directories",
     },
     "dir": {"class": "fsspec.implementations.dirfs.DirFileSystem"},
```

### Comparing `fsspec-2023.3.0/fsspec/spec.py` & `fsspec-2023.4.0/fsspec/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1021,24 +1021,27 @@
                     rec = set(
                         self.find(p, maxdepth=maxdepth, withdirs=True, detail=False)
                     )
                     out |= rec
                 if p not in out and (recursive is False or self.exists(p)):
                     # should only check once, for the root
                     out.add(p)
-            # reduce depth on each recursion level unless None or 0
-            maxdepth = maxdepth if not maxdepth else maxdepth - 1
         if not out:
             raise FileNotFoundError(path)
         return list(sorted(out))
 
     def mv(self, path1, path2, recursive=False, maxdepth=None, **kwargs):
         """Move file(s) from one location to another"""
-        self.copy(path1, path2, recursive=recursive, maxdepth=maxdepth)
-        self.rm(path1, recursive=recursive)
+        if path1 == path2:
+            logger.debug(
+                "%s mv: The paths are the same, so no files were moved." % (self)
+            )
+        else:
+            self.copy(path1, path2, recursive=recursive, maxdepth=maxdepth)
+            self.rm(path1, recursive=recursive)
 
     def rm_file(self, path):
         """Delete a file"""
         self._rm(path)
 
     def _rm(self, path):
         """Delete one file"""
```

### Comparing `fsspec-2023.3.0/fsspec/transaction.py` & `fsspec-2023.4.0/fsspec/transaction.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec/utils.py` & `fsspec-2023.4.0/fsspec/utils.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/fsspec.egg-info/PKG-INFO` & `fsspec-2023.4.0/fsspec.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
@@ -36,14 +36,16 @@
 Provides-Extra: oci
 Provides-Extra: smb
 Provides-Extra: ssh
 Provides-Extra: fuse
 Provides-Extra: libarchive
 Provides-Extra: gui
 Provides-Extra: tqdm
+Provides-Extra: full
+Provides-Extra: devel
 License-File: LICENSE
 
 # filesystem_spec
 
 [![PyPI version](https://badge.fury.io/py/fsspec.svg)](https://pypi.python.org/pypi/fsspec/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/fsspec/badges/version.svg)](https://anaconda.org/conda-forge/fsspec)
 ![Build](https://github.com/fsspec/filesystem_spec/workflows/CI/badge.svg)
@@ -52,19 +54,26 @@
 A specification for pythonic filesystems.
 
 ## Install
 
 ```bash
 pip install fsspec
 ```
-or
+
+would install the base fsspec. Various optionally supported features might require specification of custom
+extra require, e.g. `pip install fsspec[ssh]` will install dependencies for `ssh` backends support.
+Use `pip install fsspec[full]` for installation of all known extra dependencies.
+
+Up-to-date package also provided through conda-forge distribution:
+
 ```bash
 conda install -c conda-forge fsspec
 ```
 
+
 ## Purpose
 
 To produce a template or specification for a file-system interface, that specific implementations should follow,
 so that applications making use of them can rely on a common behaviour and not have to worry about the specific
 internal implementation decisions with any given backend. Many such implementations are included in this package,
 or in sister projects such as `s3fs` and `gcsfs`.
```

### Comparing `fsspec-2023.3.0/fsspec.egg-info/SOURCES.txt` & `fsspec-2023.4.0/fsspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/setup.cfg` & `fsspec-2023.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fsspec-2023.3.0/setup.py` & `fsspec-2023.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,49 @@
 
 import versioneer
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+extras_require = {
+    "entrypoints": [],
+    "abfs": ["adlfs"],
+    "adl": ["adlfs"],
+    "dask": ["dask", "distributed"],
+    "dropbox": ["dropboxdrivefs", "requests", "dropbox"],
+    "gcs": ["gcsfs"],
+    "git": ["pygit2"],
+    "github": ["requests"],
+    "gs": ["gcsfs"],
+    "hdfs": ["pyarrow >= 1"],
+    "arrow": ["pyarrow >= 1"],
+    "http": ["requests", "aiohttp !=4.0.0a0, !=4.0.0a1"],
+    "sftp": ["paramiko"],
+    "s3": ["s3fs"],
+    "oci": ["ocifs"],
+    "smb": ["smbprotocol"],
+    "ssh": ["paramiko"],
+    "fuse": ["fusepy"],
+    "libarchive": ["libarchive-c"],
+    "gui": ["panel"],
+    "tqdm": ["tqdm"],
+}
+# To simplify full installation
+extras_require["full"] = sorted(set(sum(extras_require.values(), [])))
+
+extras_require["devel"] = [
+    "pytest",
+    "pytest-cov",
+    # might want to add other optional depends which are used exclusively
+    # in the tests or not listed/very optional for other extra depends, e.g.
+    # 'pyftpdlib',
+    # 'fastparquet',
+]
+
 setup(
     name="fsspec",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
@@ -34,32 +69,10 @@
     maintainer="Martin Durant",
     maintainer_email="mdurant@anaconda.com",
     license="BSD",
     keywords="file",
     packages=["fsspec", "fsspec.implementations"],
     python_requires=">=3.8",
     install_requires=open("requirements.txt").read().strip().split("\n"),
-    extras_require={
-        "entrypoints": [],
-        "abfs": ["adlfs"],
-        "adl": ["adlfs"],
-        "dask": ["dask", "distributed"],
-        "dropbox": ["dropboxdrivefs", "requests", "dropbox"],
-        "gcs": ["gcsfs"],
-        "git": ["pygit2"],
-        "github": ["requests"],
-        "gs": ["gcsfs"],
-        "hdfs": ["pyarrow >= 1"],
-        "arrow": ["pyarrow >= 1"],
-        "http": ["requests", "aiohttp !=4.0.0a0, !=4.0.0a1"],
-        "sftp": ["paramiko"],
-        "s3": ["s3fs"],
-        "oci": ["ocifs"],
-        "smb": ["smbprotocol"],
-        "ssh": ["paramiko"],
-        "fuse": ["fusepy"],
-        "libarchive": ["libarchive-c"],
-        "gui": ["panel"],
-        "tqdm": ["tqdm"],
-    },
+    extras_require=extras_require,
     zip_safe=False,
 )
```

### Comparing `fsspec-2023.3.0/versioneer.py` & `fsspec-2023.4.0/versioneer.py`

 * *Files identical despite different names*

