# Comparing `tmp/nabs-1.5.2.tar.gz` & `tmp/nabs-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nabs-1.5.2.tar", last modified: Fri Oct 21 00:47:21 2022, max compression
+gzip compressed data, was "nabs-1.5.3.tar", last modified: Tue Apr  4 21:41:42 2023, max compression
```

## Comparing `nabs-1.5.2.tar` & `nabs-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,76 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-21 00:47:21.701329 nabs-1.5.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-10-21 00:47:03.000000 nabs-1.5.2/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2022-10-21 00:47:03.000000 nabs-1.5.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2022-10-21 00:47:21.701329 nabs-1.5.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2022-10-21 00:47:03.000000 nabs-1.5.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-21 00:47:21.701329 nabs-1.5.2/nabs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-10-21 00:47:21.701329 nabs-1.5.2/nabs/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6601 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/callbacks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/optimize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6014 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/plan_stubs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37311 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/plans.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13326 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/preprocessors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7895 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/simulators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/streams.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-21 00:47:21.701329 nabs-1.5.2/nabs/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3457 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_callbacks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3007 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_optimize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3929 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_plan_stubs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17001 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_plans.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_preprocessors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_simulators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1508 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/tests/test_streams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4842 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2386 2022-10-21 00:47:03.000000 nabs-1.5.2/nabs/visualizations.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-21 00:47:21.701329 nabs-1.5.2/nabs.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2022-10-21 00:47:21.000000 nabs-1.5.2/nabs.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      621 2022-10-21 00:47:21.000000 nabs-1.5.2/nabs.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-10-21 00:47:21.000000 nabs-1.5.2/nabs.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2022-10-21 00:47:21.000000 nabs-1.5.2/nabs.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2022-10-21 00:47:21.701329 nabs-1.5.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      414 2022-10-21 00:47:03.000000 nabs-1.5.2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68576 2022-10-21 00:47:03.000000 nabs-1.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.302133 nabs-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-04 21:41:26.000000 nabs-1.5.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-04-04 21:41:26.000000 nabs-1.5.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 21:41:26.000000 nabs-1.5.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 21:41:26.000000 nabs-1.5.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-04-04 21:41:26.000000 nabs-1.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-04 21:41:26.000000 nabs-1.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 21:41:26.000000 nabs-1.5.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-04-04 21:41:26.000000 nabs-1.5.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 21:41:26.000000 nabs-1.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-04 21:41:26.000000 nabs-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-04-04 21:41:42.298133 nabs-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-04 21:41:26.000000 nabs-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-04 21:41:26.000000 nabs-1.5.3/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-04 21:41:26.000000 nabs-1.5.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      571 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.290133 nabs-1.5.3/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/optimize.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/plans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7156 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_release_notes/template-short.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-04 21:41:26.000000 nabs-1.5.3/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6597 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9809 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6014 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37406 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13326 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7874 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16821 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4836 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-04-04 21:41:26.000000 nabs-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-04 21:41:26.000000 nabs-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 21:41:42.302133 nabs-1.5.3/setup.cfg
```

### Comparing `nabs-1.5.2/LICENSE.md` & `nabs-1.5.3/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `nabs-1.5.2/nabs/callbacks.py` & `nabs-1.5.3/nabs/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     def event(self, doc):
         if doc['descriptor'] not in self._descriptors:
             return
 
         self._data['seq_num'].append(doc['seq_num'])
         self._data['time'].append(
             str(datetime.fromtimestamp(doc['time']).time())[:-4]
-            )
+        )
 
         # this might break for unfilled data, but do we deal with that?
         for k in self._data_keys:
             try:
                 dtype = self._format_info[k]
                 style = self._FMTLOOKUP[dtype]
                 self._data[k].append(style.format(doc['data'][k]))
```

### Comparing `nabs-1.5.2/nabs/optimize.py` & `nabs-1.5.3/nabs/optimize.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/plan_stubs.py` & `nabs-1.5.3/nabs/plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/plans.py` & `nabs-1.5.3/nabs/plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -935,16 +935,16 @@
                          for item in cycle_yy if item["status"] is False))
                     yield from bpp.stub_wrapper(bp.list_scan(detectors,
                                                 x_motor, [x], y_motor, [y]))
             update_sample(sample, path, (n_shots * len(ss)))
         except Exception:
             current_position = x_motor.position
             try:
-                last_index = next((index for (index, d) in enumerate(xx)
-                                  if np.isclose(d["pos"], current_position)))
+                last_index = next(index for (index, d) in enumerate(xx)
+                                  if np.isclose(d["pos"], current_position))
                 update_sample(sample, path, (last_index - next_index + 1))
             except Exception:
                 logger.warning('Could not find the index in the targets list '
                                'for the current motor value: %d',
                                current_position)
     return (yield from inner_scan())
 
@@ -1003,26 +1003,32 @@
     def inner_scan():
         try:
             temp_index = next_index - 1
             for i in range(len(ss)):
                 temp_index += 1
                 yield from bps.mv(scan_motor, ss[i])
                 for j in range(n_shots):
-                    x = next((d['pos'] for (index, d) in enumerate(xx)
-                              if index == temp_index))
-                    y = next((d['pos'] for (index, d) in enumerate(yy)
-                              if index == temp_index))
+                    x = next(
+                        d["pos"] for (index, d) in enumerate(xx)
+                        if index == temp_index
+                    )
+                    y = next(
+                        d["pos"] for (index, d) in enumerate(yy)
+                        if index == temp_index
+                    )
                     yield from bpp.stub_wrapper(bp.list_scan(detectors,
                                                 x_motor, [x], y_motor, [y]))
             update_sample(sample, path, (len(ss)))
         except Exception:
             current_position = x_motor.position
             try:
-                last_index = next((index for (index, d) in enumerate(xx)
-                                   if np.isclose(d["pos"], current_position)))
+                last_index = next(
+                    index for (index, d) in enumerate(xx)
+                    if np.isclose(d["pos"], current_position)
+                )
                 update_sample(sample, path, (last_index - next_index + 1))
             except Exception:
                 logger.warning('Could not find the index in the targets list '
                                'for the current motor value: %s',
                                current_position)
     return (yield from inner_scan())
```

### Comparing `nabs-1.5.2/nabs/preprocessors.py` & `nabs-1.5.3/nabs/preprocessors.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/simulators.py` & `nabs-1.5.3/nabs/simulators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simulation and validation functions for plans"""
 import itertools
 import logging
 import sys
 from contextlib import contextmanager
-from typing import Any, Generator, Iterator, List, Tuple
+from typing import Any, Generator, Iterator
 
 import epics
 from bluesky.simulators import check_limits
 from ophyd.epics_motor import PositionerBase
 from ophyd.signal import EpicsSignal
 from ophyd.sim import SynAxis
 
@@ -124,15 +124,15 @@
         raise ValidError(
             "Plan ended without unstaging all staged devices."
         )
 
 
 def check_stray_calls(
     plan: Iterator[Any],
-    patches: List[str] = default_patches
+    patches: list[str] = default_patches
 ) -> None:
     """
     Validate that plan does not invoke any caput functionality
     outside of messages.
 
     Runs the check within a multiprocessing.Process to isolate
     namespace from the parent process.
@@ -182,15 +182,15 @@
         check_limits,
     ]
 
 
 def validate_plan(
     plan: Generator,
     validators=validators
-) -> Tuple[bool, str]:
+) -> tuple[bool, str]:
     """
     Validate plan with all available checkers.
 
     Parameters
     ----------
     plan: generator function
         Once called, must yield `Msg` objects.
@@ -233,15 +233,15 @@
     print lcls-daq information specifically
 
     Parameters
     ----------
     plan : iterable
         Must yield `Msg` objects
     """
-    read_cache: List[str] = []
+    read_cache: list[str] = []
     daq_keys = ['events', 'record', 'use_l3t', 'duration']
     daq_cfg = {k: None for k in daq_keys}
     for msg in plan:
         cmd = msg.command
         if cmd == 'open_run':
             print('{:=^80}'.format(' Open Run '))
         elif cmd == 'close_run':
@@ -263,8 +263,8 @@
             read_cache = []
         elif cmd == 'read':
             read_cache.append(msg.obj.name)
             if msg.obj.name == 'daq':
                 print(f'  Run DAQ for {daq_cfg["events"]} events, '
                       f'(record={daq_cfg["record"]})')
         elif cmd == 'save':
-            print('  Read {}'.format(read_cache))
+            print(f'  Read {read_cache}')
```

### Comparing `nabs-1.5.2/nabs/streams.py` & `nabs-1.5.3/nabs/streams.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/tests/conftest.py` & `nabs-1.5.3/nabs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/tests/test_callbacks.py` & `nabs-1.5.3/nabs/tests/test_callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,31 @@
     elogc = ELogPoster(elog, ipython)
     elogc.enable_run_posts = True
 
     elog_uid = RE.subscribe(elogc)
 
     ipython.user_ns["In"].append(
         "RE(bp.scan([hw.det], hw.motor, 0, 1, num=10))"
-        )
+    )
     RE(bp.scan([hw.det], hw.motor, 0, 1, num=10))
 
     assert len(elog.posts) == 2  # start and table posts
     assert 'plan_info' in elog.posts[0][1]['tags']
     assert 'RE' in elog.posts[0][1]['tags']
 
     ipython.user_ns["In"].append(
         "RE(bp.scan([hw.det], hw.motor, 0, 1, num=10), post=False)"
-        )
+    )
     RE(bp.scan([hw.det], hw.motor, 0, 1, num=10), post=False)
     assert len(elog.posts) == 2  # confirm no new entries
 
     elog.enable_run_posts = False
     ipython.user_ns["In"].append(
         "RE(bp.scan([hw.det], hw.motor, 0, 1, num=10))"
-        )
+    )
     RE(bp.scan([hw.det], hw.motor, 0, 1, num=10))
     assert len(elog.posts) == 2  # confirm no new entries
 
     # Test override of elog default
     last_cmd = "RE(bp.scan([hw.det], hw.motor, 10, 0, num=10), post=True)"
     ipython.user_ns["In"].append(last_cmd)
     RE(bp.scan([hw.det], hw.motor, 10, 0, num=10), post=True)
@@ -46,18 +46,21 @@
     assert len(elog.posts) == 5  # empty table should not be posted
 
     # cleanup
     RE.unsubscribe(elog_uid)
 
 
 @pytest.mark.parametrize(
-    'disable_plots, disable_table',
+    "disable_plots, disable_table",
     [
-     (True, True), (True, False), (False, True), (False, False),
-    ]
+        (True, True),
+        (True, False),
+        (False, True),
+        (False, False),
+    ],
 )
 def test_bec_options(RE, hw, disable_plots, disable_table):
     bec = BECOptionsPerRun()
     RE.subscribe(bec)
 
     # starts plotting by default
     RE(bp.scan([hw.det], hw.motor, -5, 5, 5))
```

### Comparing `nabs-1.5.2/nabs/tests/test_optimize.py` & `nabs-1.5.3/nabs/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/tests/test_plan_stubs.py` & `nabs-1.5.3/nabs/tests/test_plan_stubs.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,62 +28,66 @@
     RE(measure_plan([hw.motor, hw.noisy_det]), {'event': [cnt]})
     # Check that we saw the right number of events
     assert cnt.value == 250
 
 
 def test_update_sample(sample_file):
     # current sample name: test_sample
-    sample = 'test_sample'
-    xx, yy = get_sample_targets(
-        sample_name=sample, path=sample_file)
+    sample = "test_sample"
+    xx, yy = get_sample_targets(sample_name=sample, path=sample_file)
     # expected values:
-    xx_expected = [{"pos": -20.59374999999996, "status": True},
-                   {"pos": -20.342057291666624, "status": True},
-                   {"pos": -20.090364583333283, "status": True},
-                   {"pos": -19.838671874999946, "status": True},
-                   {"pos": -19.834546874999948, "status": False},
-                   {"pos": -20.08622265624995, "status": False},
-                   {"pos": -20.33789843749996, "status": False},
-                   {"pos": -20.589574218749963, "status": False}]
-    yy_expected = [{"pos": 26.41445312499999, "status": True},
-                   {"pos": 26.412369791666656, "status": True},
-                   {"pos": 26.41028645833332, "status": True},
-                   {"pos": 26.408203124999986, "status": True},
-                   {"pos":  26.664453124999994, "status": False},
-                   {"pos":  26.66232812499999, "status": False},
-                   {"pos":  26.660203124999992, "status": False},
-                   {"pos":  26.65807812499999, "status": False}]
-    update_sample(sample_name=sample,
-                  path=sample_file, n_shots=4)
-    xx, yy = get_sample_targets(
-        sample_name=sample, path=sample_file)
+    xx_expected = [
+        {"pos": -20.59374999999996, "status": True},
+        {"pos": -20.342057291666624, "status": True},
+        {"pos": -20.090364583333283, "status": True},
+        {"pos": -19.838671874999946, "status": True},
+        {"pos": -19.834546874999948, "status": False},
+        {"pos": -20.08622265624995, "status": False},
+        {"pos": -20.33789843749996, "status": False},
+        {"pos": -20.589574218749963, "status": False},
+    ]
+    yy_expected = [
+        {"pos": 26.41445312499999, "status": True},
+        {"pos": 26.412369791666656, "status": True},
+        {"pos": 26.41028645833332, "status": True},
+        {"pos": 26.408203124999986, "status": True},
+        {"pos": 26.664453124999994, "status": False},
+        {"pos": 26.66232812499999, "status": False},
+        {"pos": 26.660203124999992, "status": False},
+        {"pos": 26.65807812499999, "status": False},
+    ]
+    update_sample(sample_name=sample, path=sample_file, n_shots=4)
+    xx, yy = get_sample_targets(sample_name=sample, path=sample_file)
     assert xx == xx_expected
     assert yy == yy_expected
 
 
 def test_get_sample_targets(sample_file):
     # expected values:
-    xx_expected = [{"pos": -20.59374999999996, "status": False},
-                   {"pos": -20.342057291666624, "status": False},
-                   {"pos": -20.090364583333283, "status": False},
-                   {"pos": -19.838671874999946, "status": False},
-                   {"pos": -19.834546874999948, "status": False},
-                   {"pos": -20.08622265624995, "status": False},
-                   {"pos": -20.33789843749996, "status": False},
-                   {"pos": -20.589574218749963, "status": False}]
-    yy_expected = [{"pos": 26.41445312499999, "status": False},
-                   {"pos": 26.412369791666656, "status": False},
-                   {"pos": 26.41028645833332, "status": False},
-                   {"pos": 26.408203124999986, "status": False},
-                   {"pos":  26.664453124999994, "status": False},
-                   {"pos":  26.66232812499999, "status": False},
-                   {"pos":  26.660203124999992, "status": False},
-                   {"pos":  26.65807812499999, "status": False}]
-    xx, yy = get_sample_targets(
-        sample_name='test_sample', path=sample_file)
+    xx_expected = [
+        {"pos": -20.59374999999996, "status": False},
+        {"pos": -20.342057291666624, "status": False},
+        {"pos": -20.090364583333283, "status": False},
+        {"pos": -19.838671874999946, "status": False},
+        {"pos": -19.834546874999948, "status": False},
+        {"pos": -20.08622265624995, "status": False},
+        {"pos": -20.33789843749996, "status": False},
+        {"pos": -20.589574218749963, "status": False},
+    ]
+    yy_expected = [
+        {"pos": 26.41445312499999, "status": False},
+        {"pos": 26.412369791666656, "status": False},
+        {"pos": 26.41028645833332, "status": False},
+        {"pos": 26.408203124999986, "status": False},
+        {"pos": 26.664453124999994, "status": False},
+        {"pos": 26.66232812499999, "status": False},
+        {"pos": 26.660203124999992, "status": False},
+        {"pos": 26.65807812499999, "status": False},
+    ]
+    xx, yy = get_sample_targets(sample_name="test_sample", path=sample_file)
     assert xx == xx_expected
     assert yy == yy_expected
 
     with pytest.raises(Exception):
         get_sample_targets(
             sample_name='bad_test_sample_name', path=sample_file)
     with pytest.raises(Exception):
```

### Comparing `nabs-1.5.2/nabs/tests/test_plans.py` & `nabs-1.5.3/nabs/tests/test_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 import logging
-import sys
 from collections import defaultdict
 
 import numpy as np
 import pytest
 from bluesky.simulators import summarize_plan
 from ophyd.device import Component as Cpt
 from ophyd.signal import Signal
+from pcdsdevices.pseudopos import DelayBase
+from pcdsdevices.sim import FastMotor
 
 import nabs.plans as nbp
 from nabs.utils import orange
 
-# pcdsdevices no longer imports properly on python 3.8
-if sys.version_info >= (3, 9):
-    from pcdsdevices.pseudopos import DelayBase
-    from pcdsdevices.sim import FastMotor
-    run_time_motor_tests = True
-else:
-    DelayBase = object
-    FastMotor = object
-    run_time_motor_tests = False
+run_time_motor_tests = True
 
 
 PLAN_TIMEOUT = 60
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.timeout(PLAN_TIMEOUT)
@@ -404,23 +397,23 @@
     assert len(reads) == 24
     RE(msgs)
     summarize_plan(msgs)
 
 
 @pytest.mark.timeout(PLAN_TIMEOUT)
 @pytest.mark.parametrize(
-    'start, stop, num, n_reads',
+    "start, stop, num, n_reads",
     [
-     (-5, 5, 11, 33),    # expect 3 reads / point (det, motor, daq)
-     (-5, 5, float(1.), 33),    # step size, include endpoint
-     (-1, 1, np.float64(0.2), 33),   # step size, end point not close
-     (1, -1, -0.4, 18),  # positive to negative direction
-     (1, -1, np.float64(0.4), 18),   # ignore step sign
-     (-1, 0, np.float32(0.1), 33),  # close to 0, end near start
-    ]
+        (-5, 5, 11, 33),  # expect 3 reads / point (det, motor, daq)
+        (-5, 5, float(1.0), 33),  # step size, include endpoint
+        (-1, 1, np.float64(0.2), 33),  # step size, end point not close
+        (1, -1, -0.4, 18),  # positive to negative direction
+        (1, -1, np.float64(0.4), 18),  # ignore step sign
+        (-1, 0, np.float32(0.1), 33),  # close to 0, end near start
+    ],
 )
 def test_daq_step_size(daq, hw, start, stop, num, n_reads):
     x_start = 1
     # absolute scan
     hw.motor1.set(x_start)
     msgs = list(nbp.daq_ascan([hw.det], hw.motor1,
                               start, stop, num, events=1))
```

### Comparing `nabs-1.5.2/nabs/tests/test_preprocessors.py` & `nabs-1.5.3/nabs/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/tests/test_simulators.py` & `nabs-1.5.3/nabs/tests/test_simulators.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,34 +67,33 @@
 
 
 def bad_stage():
     yield from bps.stage(hw.det)
 
 
 @pytest.mark.parametrize(
-    'plan',
+    "plan",
     [
-     bad_limits,
-     bad_nesting,
-     bad_call,
-    ]
+        bad_limits,
+        bad_nesting,
+        bad_call,
+    ],
 )
 def test_bad_plans(RE, plan):
-    if sys.platform == 'win32' and plan is bad_call:
-        pytest.skip(reason='bad_call check does not work on windows')
+    if sys.platform == "win32" and plan is bad_call:
+        pytest.skip(reason="bad_call check does not work on windows")
     success, _ = validate_plan(plan())
     assert not success, "Plan was supposed to be bad"
 
 
 @pytest.mark.parametrize(
-    'plan',
+    "plan",
     [
-     sim_plan_outer(4),
-     bp.count([hw.det], num=2),
-     bp.scan([hw.det, hw.det2, hw.motor],
-             hw.motor, 0, 1, hw.motor2, 1, 20, 10),
-     nbp.daq_dscan([hw.det], hw.motor, 1, 0, 2, events=1)
-    ]
+        sim_plan_outer(4),
+        bp.count([hw.det], num=2),
+        bp.scan([hw.det, hw.det2, hw.motor], hw.motor, 0, 1, hw.motor2, 1, 20, 10),
+        nbp.daq_dscan([hw.det], hw.motor, 1, 0, 2, events=1),
+    ],
 )
 def test_good_plans(RE, plan, daq):
     success, msg = validate_plan(plan)
     assert success, msg
```

### Comparing `nabs-1.5.2/nabs/tests/test_streams.py` & `nabs-1.5.3/nabs/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.2/nabs/utils.py` & `nabs-1.5.3/nabs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import multiprocessing as mp
 import numbers
 import traceback
-from typing import Any, Callable, Dict, Union
+from typing import Any, Callable, Union
 
 import numpy as np
 from ophyd.signal import DerivedSignal, SignalRO
 
 
 class InvertedSignal(DerivedSignal):
     """
@@ -66,15 +66,15 @@
 
     def trigger(self):
         return self.derived_from.trigger()
 
 
 def add_named_kwargs_to_signature(
     func_or_signature: Union[inspect.Signature, Callable],
-    kwargs: Dict[str, Any]
+    kwargs: dict[str, Any]
 ) -> inspect.Signature:
     """
     Add named keyword arguments with default values to a function signature.
 
     Parameters
     ----------
     func_or_signature : inspect.Signature or callable
```

### Comparing `nabs-1.5.2/nabs/visualizations.py` & `nabs-1.5.3/nabs/visualizations.py`

 * *Files identical despite different names*

