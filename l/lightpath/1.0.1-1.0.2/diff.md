# Comparing `tmp/lightpath-1.0.1.tar.gz` & `tmp/lightpath-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightpath-1.0.1.tar", last modified: Tue Oct 25 19:20:15 2022, max compression
+gzip compressed data, was "lightpath-1.0.2.tar", last modified: Tue Apr  4 21:38:13 2023, max compression
```

## Comparing `lightpath-1.0.1.tar` & `lightpath-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,84 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.843404 lightpath-1.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-10-25 19:19:58.000000 lightpath-1.0.1/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2022-10-25 19:19:58.000000 lightpath-1.0.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2022-10-25 19:20:15.843404 lightpath-1.0.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      791 2022-10-25 19:19:58.000000 lightpath-1.0.1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2022-10-25 19:19:58.000000 lightpath-1.0.1/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.887426 lightpath-1.0.1/lightpath/
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)       43 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-10-25 19:20:15.887426 lightpath-1.0.1/lightpath/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23621 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.835399 lightpath-1.0.1/lightpath/happi/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/happi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/happi/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3858 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6456 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/mock_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/path.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.839402 lightpath-1.0.1/lightpath/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7603 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6820 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/test_controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4395 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/test_gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7416 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/test_path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/tests/test_widgets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.843404 lightpath-1.0.1/lightpath/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/ui/device.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    17299 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/ui/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12784 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/ui/lightapp.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     8744 2022-10-25 19:19:58.000000 lightpath-1.0.1/lightpath/ui/widgets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-25 19:20:15.835399 lightpath-1.0.1/lightpath.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      879 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2022-10-25 19:20:15.000000 lightpath-1.0.1/lightpath.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2022-10-25 19:19:58.000000 lightpath-1.0.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2022-10-25 19:20:15.843404 lightpath-1.0.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      792 2022-10-25 19:19:58.000000 lightpath-1.0.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81180 2022-10-25 19:19:58.000000 lightpath-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.432193 lightpath-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-04 21:37:51.000000 lightpath-1.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-04-04 21:37:51.000000 lightpath-1.0.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 21:37:51.000000 lightpath-1.0.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 21:37:51.000000 lightpath-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.420193 lightpath-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 21:37:51.000000 lightpath-1.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-04 21:37:51.000000 lightpath-1.0.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.420193 lightpath-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-04 21:37:51.000000 lightpath-1.0.2/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-04 21:37:51.000000 lightpath-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-04 21:37:51.000000 lightpath-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 21:37:51.000000 lightpath-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3014 2023-04-04 21:37:51.000000 lightpath-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 21:37:51.000000 lightpath-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-04 21:37:51.000000 lightpath-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-04-04 21:38:13.432193 lightpath-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-04 21:37:51.000000 lightpath-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.420193 lightpath-1.0.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-04 21:37:51.000000 lightpath-1.0.2/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-04 21:37:51.000000 lightpath-1.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.424193 lightpath-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7446 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.424193 lightpath-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9839 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/controller.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8573 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/path.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.424193 lightpath-1.0.2/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/source/upcoming_release_notes/template-short.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.424193 lightpath-1.0.2/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (122)   101190 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/static/LCLS_beamline_map.png
+-rw-r--r--   0 runner    (1001) docker     (122)   268651 2023-04-04 21:37:51.000000 lightpath-1.0.2/docs/static/LCLS_beamline_map.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.428193 lightpath-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-04 21:37:51.000000 lightpath-1.0.2/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-04-04 21:37:51.000000 lightpath-1.0.2/github_deploy_key_pcdshub_lightpath.enc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.428193 lightpath-1.0.2/lightpath/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23594 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.432193 lightpath-1.0.2/lightpath/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3873 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17247 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/mock_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22616 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.432193 lightpath-1.0.2/lightpath/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/conf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42695 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/path.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7160 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7448 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.432193 lightpath-1.0.2/lightpath/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9003 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/ui/device.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    17352 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/ui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12784 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/ui/lightapp.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-04-04 21:37:51.000000 lightpath-1.0.2/lightpath/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:38:13.432193 lightpath-1.0.2/lightpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-04 21:38:13.000000 lightpath-1.0.2/lightpath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-04-04 21:37:51.000000 lightpath-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-04 21:37:51.000000 lightpath-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 21:38:13.436193 lightpath-1.0.2/setup.cfg
```

### Comparing `lightpath-1.0.1/LICENSE.md` & `lightpath-1.0.2/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `lightpath-1.0.1/README.rst` & `lightpath-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/controller.py` & `lightpath-1.0.2/lightpath/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 The :class:`.LightController` handles this logic as well as a basic overview of
 where the beam is
 """
 import logging
 import math
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, Optional, Union
 
 import networkx as nx
 from happi import Client, SearchResult
 from networkx.exception import NodeNotFound
 from ophyd import Device
 
 from .config import beamlines
@@ -31,15 +31,15 @@
 from .errors import PathError
 from .mock_devices import Crystal, Valve
 from .path import BeamPath
 
 logger = logging.getLogger(__name__)
 
 NodeName = str
-MaybeBeamPath = List[Union[List[NodeName], BeamPath]]
+MaybeBeamPath = list[Union[list[NodeName], BeamPath]]
 
 
 @dataclass
 class NodeMetadata:
     res: Optional[SearchResult] = None
     dev: Optional[Device] = None
 
@@ -61,16 +61,16 @@
         as None, all endstations will be loaded
     """
     graph: nx.DiGraph
 
     def __init__(
         self,
         client: Client,
-        endstations: Optional[List[str]] = None,
-        cfg: Dict[str, Any] = {}
+        endstations: Optional[list[str]] = None,
+        cfg: dict[str, Any] = {}
     ):
         self.client: Client = client
         config = {
             'beamlines': beamlines,
             'hutches': endstations,
             'sources': default_sources,
             'min_trans': 0.1
@@ -79,17 +79,17 @@
         config.update(cfg)
         self.beamline_config = config['beamlines']
         self.hutches = config['hutches']
         self.default_sources = config['sources']
         self.min_trans = config['min_trans']
 
         # a mapping of endstation name to either a path or initialized BeamPath
-        self.beamlines: Dict[str, MaybeBeamPath] = dict()
+        self.beamlines: dict[str, MaybeBeamPath] = dict()
         # sources found in facility
-        self.sources: Set[str] = set()
+        self.sources: set[str] = set()
 
         # initialize graph -> self.graph
         self.load_facility()
 
         dests = (self.hutches or (self.beamline_config or {}).keys())
         # Find the requisite beamlines to reach our endstation
         for beamline in dests:
@@ -127,16 +127,16 @@
         subgraphs = []
         for branch_name, branch_devs in branch_dict.items():
             subgraph = self.make_graph(
                 branch_devs,
                 sources=self.default_sources,
                 branch_name=branch_name
             )
-            self.sources.update((n for n in subgraph
-                                 if self.is_source_name(n)))
+            self.sources.update(n for n in subgraph
+                                if self.is_source_name(n))
             subgraphs.append(subgraph)
 
         self.graph = nx.compose_all(subgraphs)
 
     def load_beamline(self, endstation: str):
         """
         Load a beamline given the facility graph.  Finds all possible
@@ -174,15 +174,15 @@
                         logger.debug(f'No path between {src} and {branch}')
                 except NodeNotFound:
                     logger.debug(f'Either source {src} or target {branch} '
                                  'not found.')
 
         self.beamlines[endstation] = paths
 
-    def get_paths(self, endstation: str) -> List[BeamPath]:
+    def get_paths(self, endstation: str) -> list[BeamPath]:
         """
         Returns the BeamPaths for a specified endstation.
         Create and fill the BeamPaths if they have not been already
 
         Parameters
         ----------
         endstation : str
@@ -291,15 +291,15 @@
         Returns
         -------
         bool
             if name is a valid source name
         """
         return name.startswith('source_')
 
-    def walk_facility(self) -> Dict[NodeName, List[NodeName]]:
+    def walk_facility(self) -> dict[NodeName, list[NodeName]]:
         """
         Return the paths from each source to its destination by walking the
         graph.
 
         Starting from a source node, steps iteratively through a node's
         successors (nearest neighbors).  If there is one and only one valid
         successor, step to that device and repeat.  Once there are no more
@@ -314,15 +314,15 @@
             A mapping from source node names to path of nodes
 
         Raises
         ------
         PathError
             If a single, valid path cannot be determined
         """
-        paths: Dict[NodeName, List] = {k: [] for k in self.sources}
+        paths: dict[NodeName, list] = {k: [] for k in self.sources}
 
         for src, path in paths.items():
             successors = list(self.graph.successors(src))
             # skip to node after source node
             try:
                 curr = successors[0]
             except IndexError:
@@ -361,15 +361,15 @@
                 path.append(curr)
                 curr_dev = self.get_device(curr)
                 successors = list(self.graph.successors(curr))
 
         return paths
 
     @property
-    def destinations(self) -> List[Device]:
+    def destinations(self) -> list[Device]:
         """
         Current device destinations for the LCLS photon beam
 
         Returns
         -------
         List[Device]
             a list of beam destinations
@@ -387,27 +387,27 @@
                 dest = find_dest(path)
                 if dest is not None:
                     dests.add(dest)
 
         return list(dests)
 
     @property
-    def devices(self) -> List[Device]:
+    def devices(self) -> list[Device]:
         """
         All of the devices loaded in the facility
 
         Returns
         -------
         List[Device]
             list of devices loaded in the facility
         """
         return [n[1]['md'].dev for n in self.graph.nodes.data()]
 
     @property
-    def incident_devices(self) -> List[Device]:
+    def incident_devices(self) -> list[Device]:
         """
         List of all devices in contact with photons along the beamline
 
         Returns
         -------
         List[Device]
             list of all incident devices in facility
@@ -417,15 +417,15 @@
         for endstation in self.beamlines.keys():
             paths = self.get_paths(endstation)
             for path in paths:
                 devices.update(path.incident_devices)
 
         return list(devices)
 
-    def paths_to(self, device: Device) -> List[BeamPath]:
+    def paths_to(self, device: Device) -> list[BeamPath]:
         """
         Create all BeamPaths from the facility source to the requested device
 
         Parameters
         ----------
         device : Device
             A device somewhere in LCLS
@@ -484,17 +484,17 @@
         BeamPath
             path to the specified device
         """
         return sorted(self.paths_to(device), key=self.imped_z)[-1]
 
     @staticmethod
     def make_graph(
-        branch_devs: List[SearchResult],
+        branch_devs: list[SearchResult],
         branch_name: str,
-        sources: List[NodeName] = []
+        sources: list[NodeName] = []
     ) -> nx.DiGraph:
         """
         Create a graph with devices from ``branch_devs`` as nodes,
         arranged in z-order.
 
         It is assumed that all devices lie on branch: ``branch_name``
 
@@ -524,17 +524,17 @@
         # a place for the ophyd device
         nodes = []
         for res in result_list:
             nodes.append((res.metadata['name'],
                          {'md': NodeMetadata(res=res, dev=None)}))
 
         # construct edges
-        edges: List[Tuple[NodeName, NodeName, Dict[str, Any]]] = []
-        skipped_right: List[int] = []
-        skipped_left: List[int] = []
+        edges: list[tuple[NodeName, NodeName, dict[str, Any]]] = []
+        skipped_right: list[int] = []
+        skipped_left: list[int] = []
         last_on_branch = 0
         # weight not used currently, but may be for path finding algos
         edata = {'weight': 0.0, 'branch': branch_name}
         # Need to properly handle "dangling" devices that either:
         # only have the current branch in their input (skipped_right)
         # - these devices will not have output edge
         # only have the current branch in their output (skipped_left)
@@ -634,15 +634,15 @@
                 logger.error(f'Device {device_name} failed to load, '
                              'attempting to make a mock device')
                 dev = make_mock_device(dev_data.res)
                 self.graph.nodes[device_name]['md'].dev = dev
                 return dev
 
 
-def get_active_outputs(device: Device) -> List[str]:
+def get_active_outputs(device: Device) -> list[str]:
     """
     Returns a list of branch names that are receiving beam.
     Alternatively, returns a list of branches this device is delivering
     beam to with transmission > 0.
 
     Parameters
     ----------
```

### Comparing `lightpath-1.0.1/lightpath/happi/containers.py` & `lightpath-1.0.2/lightpath/happi/containers.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/main.py` & `lightpath-1.0.2/lightpath/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import logging
 from pathlib import Path
-from typing import List, Optional, Union, overload
+from typing import Optional, Union, overload
 
 import coloredlogs
 import happi
 import yaml
 from qtpy.QtWidgets import QApplication
 
 import lightpath
@@ -43,24 +43,26 @@
         else:
             logger.debug("Using existing QApplication")
             qapp = QApplication.instance()
     return qapp
 
 
 @overload
-def main(db: Union[str, Path], hutches: List[str]) -> LightApp: ...
+def main(db: Union[str, Path], hutches: list[str]) -> LightApp:
+    ...
 
 
 @overload
-def main(cfg: Union[str, Path]) -> LightApp: ...
+def main(cfg: Union[str, Path]) -> LightApp:
+    ...
 
 
 def main(
     db: Optional[Union[str, Path]],
-    hutches: Optional[List[str]],
+    hutches: Optional[list[str]],
     cfg: Union[str, Path]
 ) -> LightApp:
     """
     Open the lightpath user interface by specifying a list of hutches
     to load or a configuration file.
 
     Parameters
@@ -72,15 +74,15 @@
         List of hutches to load in Lightpath
 
     cfg : Union[str, Path]
         Path to lightpath config file
     """
     if cfg:
         logger.info(f'reading config from: {cfg}...')
-        with open(cfg, 'r') as f:
+        with open(cfg) as f:
             conf = yaml.safe_load(f)
     else:
         conf = {}
 
     timeout = float(conf.get('timeout', 10))  # timeout (s)
     from ophyd.signal import EpicsSignalBase
     EpicsSignalBase.set_defaults(timeout=timeout,
@@ -98,17 +100,16 @@
     # Create PyDM Application
     app = get_qapp()
     # Create Lightpath UI from provided database
     lc = lightpath.LightController(client, endstations=hutches, cfg=conf)
     lp = LightApp(lc)
     # Execute
     lp.show()
-    app.exec_()
-
-    return lp
+    exit_code = app.exec_()
+    return exit_code
 
 
 def entrypoint():
     args = create_arg_parser().parse_args()
     if args.version:
         print("Lightpath Version ", lightpath.__version__)
         return
```

### Comparing `lightpath-1.0.1/lightpath/path.py` & `lightpath-1.0.2/lightpath/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import enum
 import logging
 import math
 from collections import OrderedDict
 from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Optional, TextIO, Tuple, Union
+from typing import Callable, TextIO
 
 from ophyd import Device, DeviceStatus
 from ophyd.ophydobj import OphydObject
 from ophyd.status import wait as status_wait
 from ophyd.utils import DisconnectedError
 from prettytable import PrettyTable
 
@@ -49,15 +49,15 @@
     removed : bool
 
     output : Dict[str, float]
         mapping from output branch to transmission
     """
     inserted: bool
     removed: bool
-    output: Dict[str, float]
+    output: dict[str, float]
 
 
 class DeviceState(enum.IntEnum):
     """
     Description of BeamStates
 
     The standard Inserted, Removed or Unknown have been expanded within
@@ -91,15 +91,15 @@
     Inserted = 1
     Unknown = 2
     Inconsistent = 3
     Disconnected = 4
     Error = 5
 
 
-def find_device_state(device: Device) -> Tuple[DeviceState, LightpathState]:
+def find_device_state(device: Device) -> tuple[DeviceState, LightpathState]:
     """
     Report the state of a device
 
     The device must implement ``get_lightpath_state``, which returns a
     ``LightpathState`` object.
 
     Parameters
@@ -184,15 +184,15 @@
     SUB_PTH_CHNG = 'beampath_changed'
     _default_sub = SUB_PTH_CHNG
 
     def __init__(
         self,
         *devices: OphydObject,
         minimum_transmission: float = 0.1,
-        name: Optional[str] = None,
+        name: str | None = None,
     ):
         super().__init__(name=name)
         self.minimum_transmission = minimum_transmission
         self.devices = devices
         if len(self.devices) < 1:
             raise ValueError('BeamPath must have at least one device')
 
@@ -225,30 +225,30 @@
 
         except AttributeError as e:
             raise TypeError('One of the devices does not meet the '
                             'neccesary lightpath interface. Missing '
                             'attribute {}'.format(e))
 
     @property
-    def branching_devices(self) -> List[Device]:
+    def branching_devices(self) -> list[Device]:
         """ List[Device]: Branching devices along the path """
         return [d for d in self.devices
                 if len(getattr(d, 'output_branches', ['1'])) > 1]
 
     @property
-    def range(self) -> Tuple[float, float]:
+    def range(self) -> tuple[float, float]:
         """ Tuple[float, float]: Starting z position of beamline """
         return self.path[0].md.z, self.path[-1].md.z
 
     @property
-    def path(self) -> List[Device]:
+    def path(self) -> list[Device]:
         """ List[Device]: List of devices ordered by coordinates """
         return list(self._next_device.values())
 
-    def get_device_output(self, dev: Device) -> Tuple[str, float]:
+    def get_device_output(self, dev: Device) -> tuple[str, float]:
         """
         Find relevant output item by attempting to match with the
         input branch of the next device in this path.
 
         Parameters
         ----------
         dev : Device
@@ -275,15 +275,15 @@
                             f'outputs along this path: {output_keys}')
         elif len(output_keys) == 0:
             return '', 0
 
         return output_keys[0], output[output_keys[0]]
 
     @property
-    def blocking_devices(self) -> List[Device]:
+    def blocking_devices(self) -> list[Device]:
         """
         A list of devices that are currently inserted or are in unknown
         positions. This includes devices downstream of the first
         :attr:`.impediment`.
 
         Returns
         -------
@@ -331,15 +331,15 @@
 
             # stash previous device
             prev_device = device
             prev_dev_branch = curr_dev_branch
         return block
 
     @property
-    def incident_devices(self) -> List[Device]:
+    def incident_devices(self) -> list[Device]:
         """
         A list of devices the beam is currently incident on. This includes the
         current :attr:`.impediment` and any upstream devices that may be
         inserted but have more transmission than :attr:`.minimum_transmission`
 
         Returns
         -------
@@ -404,18 +404,18 @@
             whether beamline is clear of impediments
         """
         return not any(self.blocking_devices)
 
     def clear(
         self,
         wait: bool = False,
-        timeout: Optional[float] = None,
-        ignore: Optional[List[Device]] = None,
+        timeout: float | None = None,
+        ignore: list[Device] | None = None,
         passive: bool = False,
-    ) -> List[DeviceStatus]:
+    ) -> list[DeviceStatus]:
         """
         Clear the beampath of all obstructions
 
         Parameters
         ----------
         wait : bool, optional
             Wait for all devices to complete their motion
@@ -479,17 +479,17 @@
         TypeError:
             Raised if a non-BeamPath object is supplied
         """
         return BeamPath.from_join(self, *beampaths, name=self.name)
 
     def split(
         self,
-        z: Optional[float] = None,
-        device: Optional[Device] = None
-    ) -> Tuple[BeamPath, BeamPath]:
+        z: float | None = None,
+        device: Device | None = None
+    ) -> tuple[BeamPath, BeamPath]:
         """
         Split the beampath producing two new BeamPath objects either by a
         specific position or a devices location
 
         Parameters
         ----------
         z : float
@@ -554,17 +554,17 @@
         # Flatten path lists
         devices = [device for path in beampaths for device in path.devices]
         # Create a new instance
         return BeamPath(*set(devices), name=name)
 
     def _ignore(
         self,
-        ignore_devices: Optional[Union[Device, List[Device]]] = None,
+        ignore_devices: Device | list[Device] | None = None,
         passive: bool = False
-    ) -> Tuple[List[Device], List[Device]]:
+    ) -> tuple[list[Device], list[Device]]:
         """
         Assemble list of available devices with some exclusions
 
         Parameters
         ----------
         ignore_devices : list
             Device(s) to ignore
@@ -611,15 +611,15 @@
         # If device is upstream of impediment
         if obj is not None and obj.parent.md.z <= block:
             self._run_subs(sub_type=self.SUB_PTH_CHNG, device=obj)
 
     def subscribe(
         self,
         cb: Callable,
-        event_type: Optional[str] = None,
+        event_type: str | None = None,
         run: bool = True
     ):
         """
         Subscribe to changes of the valve
 
         Parameters
         ----------
@@ -653,16 +653,16 @@
         """
         if self._has_subscribed:
             for dev in self.devices:
                 dev.lightpath_summary.clear_sub(self._device_moved)
             self._has_subscribed = False
 
     def _repr_info(self):
-        yield('range',   self.range)
-        yield('devices', len(self.devices))
+        yield 'range', self.range
+        yield 'devices', len(self.devices)
 
     __hash = object.__hash__
 
     def __eq__(self, *args, **kwargs):
         try:
             return self.devices == args[0].devices
         except AttributeError:
```

### Comparing `lightpath-1.0.1/lightpath/tests/conftest.py` & `lightpath-1.0.2/lightpath/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 @pytest.fixture(scope='session', autouse=True)
 def set_level(pytestconfig):
     # Read user input logging level
     log_level = getattr(logging, pytestconfig.getoption('--log'), None)
 
     # Report invalid logging level
     if not isinstance(log_level, int):
-        raise ValueError("Invalid log level : {}".format(log_level))
+        raise ValueError(f"Invalid log level : {log_level}")
 
     # Create basic configuration
     logging.basicConfig(level=log_level,
                         filename=pytestconfig.getoption('--logfile'))
 
 
 ############
@@ -177,15 +177,15 @@
     print(f'first item: {lcls_client.search()[0]}')
     return LightController(lcls_client)
 
 
 @pytest.fixture(scope='function')
 def cfg():
     cfg_path = os.path.join(os.path.dirname(__file__), 'conf.yml')
-    with open(cfg_path, 'r') as f:
+    with open(cfg_path) as f:
         cfg = yaml.safe_load(f)
 
     return cfg
 
 
 @contextmanager
 def cli_args(args):
```

### Comparing `lightpath-1.0.1/lightpath/tests/test_cli.py` & `lightpath-1.0.2/lightpath/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from pathlib import Path
-from typing import Any, Dict, List
+from typing import Any
 
+import ophyd
 import pydm
 import pytest
 from qtpy.QtWidgets import QApplication
 
 from lightpath.main import entrypoint
 from lightpath.ui import LightApp
 
@@ -15,68 +16,51 @@
 @pytest.fixture(scope='function')
 def no_gui_launch(monkeypatch):
 
     def no_op(*args, **kwargs):
         pass
 
     monkeypatch.setattr(QApplication, 'exec_', no_op)
+    monkeypatch.setattr(QApplication, 'exit', no_op)
     monkeypatch.setattr(pydm.Display, 'show', no_op)
 
+    # also prevent changing of tiemout
+    monkeypatch.setattr(ophyd.signal.EpicsSignalBase, 'set_defaults', no_op)
+
 
 @pytest.fixture(scope='session')
 def sim_cfg_path(tmp_path_factory):
     cfg_path = os.path.join(os.path.dirname(__file__), 'conf.yml')
 
     db_line = f'\ndb: {os.path.join(os.path.dirname(__file__), "path.json")}\n'
     # add sim db path to cfg file
-    with open(cfg_path, 'r') as f_in:
+    with open(cfg_path) as f_in:
         orig_conf = f_in.readlines()
         orig_conf.append(db_line)
 
     sim_path = tmp_path_factory.mktemp('cfg') / 'conf.yml'
     with open(sim_path, 'w') as f_out:
         f_out.write(''.join(orig_conf))
 
     return sim_path
 
 
 @pytest.fixture(scope='function')
 def launch_cli(qtbot, no_gui_launch, sim_cfg_path: Path):
-    def starter(args: List[str]) -> LightApp:
+
+    def starter(args: list[str]) -> LightApp:
         """ Launches the gui with the given args, filling cfg if needed """
         if '--cfg' in args:
             args.append(str(sim_cfg_path))
 
         with cli_args(args):
-            lp = entrypoint()
-        qtbot.addWidget(lp)
-        return lp
+            entrypoint()
 
     return starter
 
 
-def test_cli_cfg(launch_cli, cfg: Dict[str, Any]):
-    # smoke test
-    lp = launch_cli(['lightpath', '--cfg'])
-
-    lines = set([lp.destination_combo.itemText(i)
-                 for i in range(lp.destination_combo.count())])
-    assert lines == set(cfg['hutches'])
-    lp.close()
-
-
-def test_cli_no_args(launch_cli):
-    lp = launch_cli(['lightpath', '--sim'])
-
-    assert lp.destination_combo.count() == 9
-
-    lp.close()
-
-
-def test_cli_hutch_cfg(launch_cli, cfg: Dict[str, Any]):
-    lp = launch_cli(['lightpath', '--hutches', 'XCS', '--cfg'])
+def test_cli_no_args_smoke(launch_cli):
+    launch_cli(['lightpath', '--sim'])
 
-    # cfg overrides hutches setting
-    assert lp.destination_combo.count() == len(cfg['hutches'])
-    assert lp.path.minimum_transmission == cfg['min_trans']
 
-    lp.close()
+def test_cli_hutch_cfg_smoke(launch_cli, cfg: dict[str, Any]):
+    launch_cli(['lightpath', '--hutches', 'XCS', '--cfg'])
```

### Comparing `lightpath-1.0.1/lightpath/tests/test_controller.py` & `lightpath-1.0.2/lightpath/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict
+from pathlib import Path
+from typing import Any
 
 import happi
 import pytest
 
 from lightpath import LightController
 from lightpath.errors import PathError
 
@@ -136,27 +137,27 @@
     assert walk['source_K0'][-1] == 'im4k1'
     assert len(walk['source_L0']) == 5
     assert len(walk['source_K0']) == 11
 
     # These beam paths do not represent impediments or destinations.
     # simply represents where device configurations point
     incidents = [d.name for d in lcls_ctrl.incident_devices]
-    assert set(incidents) == set(['mr1l0', 'mr1k1'])
+    assert set(incidents) == {'mr1l0', 'mr1k1'}
     assert len(lcls_ctrl.destinations) == 0
 
 
 def test_mock_device(lcls_ctrl: LightController):
     # break some metadata
     lcls_ctrl.graph.nodes['sl1k2']['md'].res.metadata['device_class'] = ''
 
     # smoke test device loading
     lcls_ctrl.get_device('sl1k2')
 
 
-def test_cfg_loading(lcls_client: happi.Client, cfg: Dict[str, Any]):
+def test_cfg_loading(lcls_client: happi.Client, cfg: dict[str, Any]):
     # load lcls with config modifications
     lc = LightController(lcls_client, ['XCS'], cfg=cfg)
 
     # check modifications to default parameters
     # only loaded beamlines specified, cfg overrides endstations
     assert set(lc.beamlines.keys()) == set(cfg['hutches'])
     assert 'CRIX' not in lc.beamlines.keys()
@@ -170,7 +171,19 @@
     bad_cfg = {
         'beamlines': {'NOT': ['NO_BR']},
         'hutches': ['NOT']
     }
     with pytest.raises(PathError):
         bad_lc = LightController(lcls_client, cfg=bad_cfg)
         bad_lc.active_path('NOT')
+
+
+def test_sim_ctrl():
+    # make sure sim beamline loads
+    sim_db_path = Path(__file__).parent / 'path.json'
+    sim_client = happi.Client(path=sim_db_path)
+
+    lc = LightController(sim_client)
+
+    assert len(lc.beamlines.keys()) == 9
+    assert len(lc.active_path('XCS').devices) == 13
+    assert lc.get_device('sl2k0')
```

### Comparing `lightpath-1.0.1/lightpath/tests/test_gui.py` & `lightpath-1.0.2/lightpath/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/tests/test_path.py` & `lightpath-1.0.2/lightpath/tests/test_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import io
 import re
+import time
 from unittest.mock import Mock
 
 from ophyd.device import Device
 
 from lightpath import BeamPath
 from lightpath.mock_devices import Crystal, Status
 from lightpath.path import DeviceState, find_device_state
@@ -199,14 +200,15 @@
 def test_callback(path: BeamPath):
     # Create mock callback
     cb = Mock()
     # Subscribe to event changes
     path.subscribe(cb, run=False)
     # Change state of beampath
     path.devices[4].insert()
+    time.sleep(0.2)
     # Assert callback has been run
     assert cb.called
 
 
 def test_attenuation(path: BeamPath):
     assert path.impediment is None
```

### Comparing `lightpath-1.0.1/lightpath/tests/test_widgets.py` & `lightpath-1.0.2/lightpath/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/ui/device.ui` & `lightpath-1.0.2/lightpath/ui/device.ui`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/ui/gui.py` & `lightpath-1.0.2/lightpath/ui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,15 @@
         slide_scroll.rangeChanged.connect(self.slide.setRange)
         slide_scroll.valueChanged.connect(self.slide.setSliderPosition)
         # Add destinations
         for line in self.destinations():
             self.destination_combo.addItem(line)
 
         # Connect signals to slots
-        self.destination_combo.currentIndexChanged.connect(
-                                            self.change_path_display)
+        self.destination_combo.currentIndexChanged.connect(self.change_path_display)
         self.device_combo.activated[str].connect(self.focus_on_device)
         self.impediment_button.pressed.connect(self.focus_on_device)
         self.upstream_device_combo.activated[str].connect(self.update_upstream)
         self.remove_check.toggled.connect(self.filter)
         self.detail_hide.clicked.connect(self.hide_detailed)
         self.refresh_button.clicked.connect(self.change_path_display)
 
@@ -235,30 +234,33 @@
                 # Cache row to later clear subscriptions
                 self.rows.append(row)
                 # Add widget to layout
                 self.lightLayout.addWidget(row[0])
                 self.overview.layout().addWidget(row[1])
                 # Connect condensed widget to focus_on_device
                 row[1].device_drawing.clicked.connect(
-                        partial(self.focus_on_device,
-                                name=row[1].device.name))
+                    partial(self.focus_on_device, name=row[1].device.name)
+                )
                 # Connect large widget to show Typhos screen
                 row[0].device_drawing.clicked.connect(
-                        partial(self.show_detailed, row[0].device))
+                    partial(self.show_detailed, row[0].device)
+                )
                 # Add device to combo
                 self.device_combo.addItem(row[0].device.name)
                 self.upstream_device_combo.addItem(row[0].device.name)
         # Initialize interface
         for row in self.rows:
             for widget in row:
                 widget.update_state()
         # Update the state of the path
         self.update_path()
         # Update device type checkboxes
         self.update_device_types()
+        # re-filter based on present settings
+        self.filter()
         self.setWindowTitle(f'Lightpath - {self.selected_beamline()}')
 
     @contextlib.contextmanager
     def open_splash(self, msg: str):
         """
         Context manager for opening the loading splash screen, and
         closing it always
@@ -287,15 +289,15 @@
     def ui_filepath(self):
         """
         Full path to :attr:`.ui_filename`
         """
         return os.path.join(os.path.dirname(os.path.abspath(__file__)),
                             self.ui_filename())
 
-    def update_path(self, *args,  **kwargs):
+    def update_path(self, *args, **kwargs):
         """
         Update the PyDMRectangles to show devices as in the beam or not
         """
         with self._lock:
             block = self.path.impediment
             # Set the current impediment label
             if block:
@@ -361,15 +363,15 @@
         upstream_device = self.selected_upstream_from()
         upstream_device_z = self.light.get_device(upstream_device).md.z
         for row in self.rows:
             device = row[0].device
             # Hide if a hidden instance of a device type
             hidden_device_type = any([device.__module__ == dtype
                                       for dtype in self.hidden_devices])
-            # Hide if removed
+            # Hide if removed (checked if showing removed devices)
             hidden_removed = (not self.remove_check.isChecked()
                               and row[0].last_state == DeviceState.Removed)
             # Hide if upstream
             # TODO: This now looks at the whole active path, which includes
             # upstream devices.  Need to figure out how best to define
             # "upstream" devices now.  Possibly by branch name?
             hidden_upstream = (device.md.z < upstream_device_z)
```

### Comparing `lightpath-1.0.1/lightpath/ui/lightapp.ui` & `lightpath-1.0.2/lightpath/ui/lightapp.ui`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.1/lightpath/ui/widgets.py` & `lightpath-1.0.2/lightpath/ui/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         super().__init__(parent=parent)
         self.device = device
         self.path = path
         # Initialize prior state variable
         self.last_state = DeviceState.Disconnected
         # Create labels
         self.name_label.setText(clean_name(device, strip_parent=False))
-        self.prefix_label.setText('({})'.format(device.prefix))
+        self.prefix_label.setText(f'({device.prefix})')
         # By default we mark the device as Disconnected
         self.state_label.setText('Disconnected')
         self.state_label.setStyleSheet("QLabel {color : rgb(255,0,255)}")
         self.device_drawing = DeviceWidget(device)
         self.horizontalWidget.layout().insertWidget(1, self.device_drawing)
 
     def ui_filename(self):
```

