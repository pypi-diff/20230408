# Comparing `tmp/enjoy_slurm-0.0.3.tar.gz` & `tmp/enjoy_slurm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enjoy_slurm-0.0.3.tar", last modified: Tue Mar 21 23:02:45 2023, max compression
+gzip compressed data, was "enjoy_slurm-0.0.4.tar", last modified: Sat Apr  8 20:23:01 2023, max compression
```

## Comparing `enjoy_slurm-0.0.3.tar` & `enjoy_slurm-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.393220 enjoy_slurm-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.397220 enjoy_slurm-0.0.3/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.397220 enjoy_slurm-0.0.3/.github/workflows/optional/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.github/workflows/optional/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.github/workflows/slurm.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.397220 enjoy_slurm-0.0.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.397220 enjoy_slurm-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/new_section.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/tutorial.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.397220 enjoy_slurm-0.0.3/enjoy_slurm/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/enjoy_slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/enjoy_slurm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/enjoy_slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/enjoy_slurm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-21 23:02:45.000000 enjoy_slurm-0.0.3/enjoy_slurm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/notebooks/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/notebooks/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/scripts/configure.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:45.401220 enjoy_slurm-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-21 23:02:36.000000 enjoy_slurm-0.0.3/tests/test_with_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/workflows/optional/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/optional/linting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/new_section.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/tutorial.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/enjoy_slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/scripts/configure.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_with_slurm.py
```

### Comparing `enjoy_slurm-0.0.3/.github/workflows/release.yaml` & `enjoy_slurm-0.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/.github/workflows/slurm.yml` & `enjoy_slurm-0.0.4/.github/workflows/slurm.yml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/.github/workflows/test.yaml` & `enjoy_slurm-0.0.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/.gitignore` & `enjoy_slurm-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/LICENSE.txt` & `enjoy_slurm-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/PKG-INFO` & `enjoy_slurm-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enjoy_slurm
-Version: 0.0.3
+Version: 0.0.4
 Summary: naive python slurm control
 Home-page: https://github.com/larsbuntemeyer/enjoy-slurm
 Author: Lars Buntemeyer
 Author-email: lars.buntemeyer@hereon.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -27,23 +27,38 @@
 [![Build Status](https://github.com/larsbuntemeyer/enjoy-slurm/workflows/Tests/badge.svg)](https://github.com/larsbuntemeyer/enjoy-slurm/actions)
 [![codecov](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm/branch/main/graph/badge.svg)](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm)
 [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
 [![pypi](https://img.shields.io/pypi/v/enjoy-slurm.svg)](https://pypi.org/project/enjoy-slurm)
 [![Documentation Status](https://readthedocs.org/projects/enjoy-slurm/badge/?version=latest)](https://enjoy-slurm.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/larsbuntemeyer/enjoy-slurm/main.svg)](https://results.pre-commit.ci/latest/github/larsbuntemeyer/enjoy-slurm/main)
 
-`enjoy-slurm` is a naive python slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
+`enjoy-slurm` is a naive slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
 line tools and arguments. That's why we call it *naive*. However, it should avoid having to rewrite some scripts required to submit and control many
 Slurm jobs on an HPC computer. This package is a successor of the retired [HPC scheduler package](https://github.com/larsbuntemeyer/hpc-scheduler).
 
 ## Features
 
-* Use `sbatch`, `sacct`, `scontrol` etc. directly from python.
+* Use `sbatch`, `sacct`, `scontrol` etc. directly from python with a pythonic API.
 * Parse command outputs into python objects like pandas DataFrames or dictionaries.
 
+## Examples
+
+```python
+import enjoy_slurm as slurm
+
+jobid = slurm.sbatch("job.sh", partition="compute", account="my_account")
+acct = slurm.sacct(jobid=jobid)
+
+# run another job that depends on the first
+jobid1 = slurm.sbatch(
+    "another_job.sh", dependency=jobid, partition="shared", account="my_account"
+)
+acct1 = slurm.sacct(jobid=jobid1)
+```
+
 ## Related projects
 
 * [pyslurm](https://github.com/PySlurm/pyslurm)
 * [simple_slurm](https://github.com/amq92/simple_slurm)
 * [ipyslurm](https://github.com/auneri/ipyslurm)
 
 --------
```

### Comparing `enjoy_slurm-0.0.3/README.md` & `enjoy_slurm-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,38 @@
 [![Build Status](https://github.com/larsbuntemeyer/enjoy-slurm/workflows/Tests/badge.svg)](https://github.com/larsbuntemeyer/enjoy-slurm/actions)
 [![codecov](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm/branch/main/graph/badge.svg)](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm)
 [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
 [![pypi](https://img.shields.io/pypi/v/enjoy-slurm.svg)](https://pypi.org/project/enjoy-slurm)
 [![Documentation Status](https://readthedocs.org/projects/enjoy-slurm/badge/?version=latest)](https://enjoy-slurm.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/larsbuntemeyer/enjoy-slurm/main.svg)](https://results.pre-commit.ci/latest/github/larsbuntemeyer/enjoy-slurm/main)
 
-`enjoy-slurm` is a naive python slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
+`enjoy-slurm` is a naive slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
 line tools and arguments. That's why we call it *naive*. However, it should avoid having to rewrite some scripts required to submit and control many
 Slurm jobs on an HPC computer. This package is a successor of the retired [HPC scheduler package](https://github.com/larsbuntemeyer/hpc-scheduler).
 
 ## Features
 
-* Use `sbatch`, `sacct`, `scontrol` etc. directly from python.
+* Use `sbatch`, `sacct`, `scontrol` etc. directly from python with a pythonic API.
 * Parse command outputs into python objects like pandas DataFrames or dictionaries.
 
+## Examples
+
+```python
+import enjoy_slurm as slurm
+
+jobid = slurm.sbatch("job.sh", partition="compute", account="my_account")
+acct = slurm.sacct(jobid=jobid)
+
+# run another job that depends on the first
+jobid1 = slurm.sbatch(
+    "another_job.sh", dependency=jobid, partition="shared", account="my_account"
+)
+acct1 = slurm.sacct(jobid=jobid1)
+```
+
 ## Related projects
 
 * [pyslurm](https://github.com/PySlurm/pyslurm)
 * [simple_slurm](https://github.com/amq92/simple_slurm)
 * [ipyslurm](https://github.com/auneri/ipyslurm)
 
 --------
```

### Comparing `enjoy_slurm-0.0.3/docs/Makefile` & `enjoy_slurm-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/docs/conf.py` & `enjoy_slurm-0.0.4/docs/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 import os
 import pathlib
 import sys
 
-
 print("python exec:", sys.executable)
 print("sys.path:", sys.path)
 root = pathlib.Path(__file__).parent.parent.absolute()
 os.environ["PYTHONPATH"] = str(root)
 sys.path.insert(0, str(root))
 
-import enjoy_slurm  # isort:skip
+# import enjoy_slurm  # isort:skip
 
 # -- Project information -----------------------------------------------------
 
 project = "enjoy-slurm"
 copyright = "2021, Lars Buntemeyer"
 author = "Lars Buntemeyer"
 
@@ -58,14 +57,19 @@
     "nbsphinx",
     "nbsphinx_link",
     "IPython.sphinxext.ipython_directive",
     "IPython.sphinxext.ipython_console_highlighting",
     "sphinxcontrib.srclinks",
 ]
 
+extlinks = {
+    "issue": ("https://github.com/larsbuntemeyer/enjoy-slurm/issues/%s", "GH#"),
+    "pr": ("https://github.com/larsbuntemeyer/enjoy-slurm/pull/%s", "GH#"),
+}
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "**.ipynb_checkpoints", "Thumbs.db", ".DS_Store"]
@@ -73,31 +77,62 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 # html_theme = "pangeo"
-html_theme = "sphinx_book_theme"
-html_title = "enjoy slurm!"
-
+# html_theme = "sphinx_book_theme"
+html_theme = "furo"
+html_title = "enjoy-slurmi"
+
+# html_theme_options = dict(
+#    repository_url="https://github.com/larsbuntemeyer/enjoy-slurm",
+#    repository_branch="main",
+#    path_to_docs="docs",
+#    use_edit_page_button=True,
+#    use_repository_button=True,
+#    use_issues_button=True,
+#    home_page_in_toc=False,
+#    extra_navbar="",
+#    navbar_footer_text="",
+# )
+
+css_vars = {
+    "admonition-font-size": "0.9rem",
+    "font-size--small": "92%",
+    "font-size--small--2": "87.5%",
+}
 html_theme_options = dict(
-    repository_url="https://github.com/larsbuntemeyer/enjoy-slurm",
-    repository_branch="main",
-    path_to_docs="docs",
-    use_edit_page_button=True,
-    use_repository_button=True,
-    use_issues_button=True,
-    home_page_in_toc=False,
-    extra_navbar="",
-    navbar_footer_text="",
+    source_repository="https://github.com/larsbuntemeyer/enjoy-slurm",
+    source_branch="main",
+    sidebar_hide_name=True,
+    source_directory="docs/",
+    light_css_variables=css_vars,
+    dark_css_variables=css_vars,
 )
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 
 # -- nbsphinx specific options ----------------------------------------------
 # this allows notebooks to be run even if they produce errors.
 nbsphinx_allow_errors = True
+
+
+autosummary_generate = True
+
+autodoc_typehints = "description"
+autodoc_typehints_description_target = "documented"
+autodoc_default_options = {
+    "members": True,
+    "undoc-members": True,
+    "private-members": True,
+}
+napoleon_use_param = True
+napoleon_use_rtype = True
+
+numpydoc_show_class_members = False
+# numpydoc_validation_checks = {"all"}
```

### Comparing `enjoy_slurm-0.0.3/docs/index.rst` & `enjoy_slurm-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/enjoy_slurm.egg-info/PKG-INFO` & `enjoy_slurm-0.0.4/enjoy_slurm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enjoy-slurm
-Version: 0.0.3
+Version: 0.0.4
 Summary: naive python slurm control
 Home-page: https://github.com/larsbuntemeyer/enjoy-slurm
 Author: Lars Buntemeyer
 Author-email: lars.buntemeyer@hereon.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -27,23 +27,38 @@
 [![Build Status](https://github.com/larsbuntemeyer/enjoy-slurm/workflows/Tests/badge.svg)](https://github.com/larsbuntemeyer/enjoy-slurm/actions)
 [![codecov](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm/branch/main/graph/badge.svg)](https://codecov.io/gh/larsbuntemeyer/enjoy-slurm)
 [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
 [![pypi](https://img.shields.io/pypi/v/enjoy-slurm.svg)](https://pypi.org/project/enjoy-slurm)
 [![Documentation Status](https://readthedocs.org/projects/enjoy-slurm/badge/?version=latest)](https://enjoy-slurm.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/larsbuntemeyer/enjoy-slurm/main.svg)](https://results.pre-commit.ci/latest/github/larsbuntemeyer/enjoy-slurm/main)
 
-`enjoy-slurm` is a naive python slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
+`enjoy-slurm` is a naive slurm control package for python. It does interact with Slurm exactly as any user would do, simply through the command
 line tools and arguments. That's why we call it *naive*. However, it should avoid having to rewrite some scripts required to submit and control many
 Slurm jobs on an HPC computer. This package is a successor of the retired [HPC scheduler package](https://github.com/larsbuntemeyer/hpc-scheduler).
 
 ## Features
 
-* Use `sbatch`, `sacct`, `scontrol` etc. directly from python.
+* Use `sbatch`, `sacct`, `scontrol` etc. directly from python with a pythonic API.
 * Parse command outputs into python objects like pandas DataFrames or dictionaries.
 
+## Examples
+
+```python
+import enjoy_slurm as slurm
+
+jobid = slurm.sbatch("job.sh", partition="compute", account="my_account")
+acct = slurm.sacct(jobid=jobid)
+
+# run another job that depends on the first
+jobid1 = slurm.sbatch(
+    "another_job.sh", dependency=jobid, partition="shared", account="my_account"
+)
+acct1 = slurm.sacct(jobid=jobid1)
+```
+
 ## Related projects
 
 * [pyslurm](https://github.com/PySlurm/pyslurm)
 * [simple_slurm](https://github.com/amq92/simple_slurm)
 * [ipyslurm](https://github.com/auneri/ipyslurm)
 
 --------
```

### Comparing `enjoy_slurm-0.0.3/enjoy_slurm.egg-info/SOURCES.txt` & `enjoy_slurm-0.0.4/enjoy_slurm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,22 +21,27 @@
 docs/index.rst
 docs/new_section.rst
 docs/tutorial.nblink
 docs/whats_new.rst
 enjoy_slurm/__init__.py
 enjoy_slurm/_version.py
 enjoy_slurm/config.py
+enjoy_slurm/parser.py
 enjoy_slurm/slurm.py
+enjoy_slurm/tutorial.py
 enjoy_slurm/utils.py
 enjoy_slurm.egg-info/PKG-INFO
 enjoy_slurm.egg-info/SOURCES.txt
 enjoy_slurm.egg-info/dependency_links.txt
 enjoy_slurm.egg-info/not-zip-safe
 enjoy_slurm.egg-info/requires.txt
 enjoy_slurm.egg-info/top_level.txt
 notebooks/.gitkeep
 notebooks/test.sh
 notebooks/tutorial.ipynb
 scripts/configure.sh
 tests/__init__.py
+tests/test_job.py
 tests/test_parser.py
+tests/test_tutorial.py
+tests/test_utils.py
 tests/test_with_slurm.py
```

### Comparing `enjoy_slurm-0.0.3/notebooks/tutorial.ipynb` & `enjoy_slurm-0.0.4/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/pyproject.toml` & `enjoy_slurm-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/scripts/configure.sh` & `enjoy_slurm-0.0.4/scripts/configure.sh`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.3/setup.cfg` & `enjoy_slurm-0.0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,24 @@
 	*.enc
 	notebooks
 	notebooks/*
 	tests
 	tests/*
 
 [flake8]
-max-line-length = 105
-select = C,E,F,W,B,B950
-ignore = E203, E501, W503
-exclude = enjoy_slurm/_version.py
+ignore = 
+	E203
+	E402
+	E501
+	E731
+	W503
+exclude = 
+	build
+	docs
+	.git
 
 [metadata]
 name = enjoy_slurm
 description = naive python slurm control
 author = Lars Buntemeyer
 url = https://github.com/larsbuntemeyer/enjoy-slurm
 long_description = file: README.md
```

### Comparing `enjoy_slurm-0.0.3/tests/__init__.py` & `enjoy_slurm-0.0.4/tests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Unit test package for enjoy-slurm."""
 
-import pytest
-
-import subprocess
 import socket
+import subprocess
+
+import pytest
 
 
 def _cmlorskip(command):
     try:
         commands = [command, "-V"]
-        output = subprocess.run(
-            commands, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-        )
+        subprocess.run(commands, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         has = True
     except FileNotFoundError:
         has = False
-    func = pytest.mark.skipif(not has, reason=f"requires slurm")
+    func = pytest.mark.skipif(not has, reason="requires slurm")
     return has, func
 
 
 def _machine(machine):
     try:
         host = socket.gethostname().split(".", 1)[1]
         on = host == machine
```

### Comparing `enjoy_slurm-0.0.3/tests/test_with_slurm.py` & `enjoy_slurm-0.0.4/tests/test_with_slurm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import pytest
-import enjoy_slurm as slurm
-from . import hostname, requires_slurm, on_levante, requires_levante
+from enjoy_slurm import Job, sacct, sbatch, scontrol
 
+from . import hostname, on_levante, requires_slurm
 
 test_kwargs = {
     "levante": {"partitions": ["compute", "shared"]},
     "docker": {"partitions": ["debug", "normal"]},
 }
 
 print(hostname)
@@ -18,28 +17,40 @@
 
 @requires_slurm
 def test_sbatch():
     if on_levante:
         kwargs = {"partition": "shared", "account": "ch0636"}
     else:
         kwargs = {}
-    jobid = slurm.sbatch(wrap="echo Hello World", **kwargs)
+    jobid = sbatch(wrap="echo Hello World", **kwargs)
     print(jobid)
 
 
 @requires_slurm
 def test_partitions():
     if on_levante:
         partitions = test_kwargs["levante"]["partitions"]
     else:
         partitions = test_kwargs["docker"]["partitions"]
     for p in partitions:
-        pdict = slurm.scontrol.show(partition=p)
+        pdict = scontrol.show(partition=p)
         assert p in pdict
 
 
 @requires_slurm
 def test_sacct():
-    jobid = slurm.sbatch(wrap="echo Hello World", **kwargs)
-    acct = slurm.sacct(jobid=jobid)
-    scon = slurm.scontrol.show(jobid=jobid)
+    jobid = sbatch(wrap="echo Hello World", **kwargs)
+    sacct(jobid=jobid)
+    scon = scontrol.show(jobid=jobid)
     assert str(jobid) in scon
+
+
+@requires_slurm
+def test_job():
+    import time
+
+    jobid = sbatch(wrap="echo Hello World", **kwargs)
+    time.sleep(5)
+    job = Job(jobid=jobid)
+    assert job.jobid == jobid
+    assert job.partition
+    assert job.account
```

