# Comparing `tmp/stripenn-1.1.65.9.tar.gz` & `tmp/stripenn-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripenn-1.1.65.9.tar", last modified: Mon Oct 31 17:54:12 2022, max compression
+gzip compressed data, was "dist/stripenn-1.1.7.tar", last modified: Mon Nov 30 23:53:30 2020, max compression
```

## Comparing `stripenn-1.1.65.9.tar` & `stripenn-1.1.7.tar`

### file list

```diff
@@ -1,85 +1,37 @@
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.112892 stripenn-1.1.65.9/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    11034 2022-10-31 17:54:12.112892 stripenn-1.1.65.9/PKG-INFO
--rw-r--r--   0 sora      (1003) vahedilab (10000)     9054 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/README.rst
--rw-r--r--   0 sora      (1003) vahedilab (10000)      291 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/pyproject.toml
--rw-r--r--   0 sora      (1003) vahedilab (10000)      109 2022-10-31 17:54:12.112892 stripenn-1.1.65.9/setup.cfg
--rw-r--r--   0 sora      (1003) vahedilab (10000)      960 2022-10-31 17:54:09.000000 stripenn-1.1.65.9/setup.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/src/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    10917 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/ImageProcessing.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/__init__.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     3676 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/cli.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)    58757 2022-10-31 17:46:02.000000 stripenn-1.1.65.9/src/getStripe.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     8185 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/observed_over_expected.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2438 2022-10-31 17:15:01.000000 stripenn-1.1.65.9/src/score.py
--rwxr-xr-x   0 sora      (1003) vahedilab (10000)     3325 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/seeimage.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     7101 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/stats.py
--rwxr-xr-x   0 sora      (1003) vahedilab (10000)     6760 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/src/stripenn.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    11034 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/PKG-INFO
--rw-r--r--   0 sora      (1003) vahedilab (10000)     8060 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/README.rst
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2808 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/SOURCES.txt
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.104892 stripenn-1.1.65.9/stripenn.egg-info/build/
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.104892 stripenn-1.1.65.9/stripenn.egg-info/build/lib/
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    10917 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/ImageProcessing.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/__init__.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     3567 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/cli.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)    58343 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/getStripe.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     8185 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/observed_over_expected.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2433 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/score.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     3323 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/seeimage.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     7101 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/stats.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)    10401 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/stripenn.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/__init__.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)      961 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/setup.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    10917 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/ImageProcessing.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/__init__.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     3243 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/cli.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)    29286 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/getStripe.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     8185 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/observed_over_expected.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     1640 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/score.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2309 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/seeimage.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     7100 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/stats.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     9238 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/stripenn.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)       89 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/test_stripenn.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        1 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/dependency_links.txt
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/dist/
--rw-r--r--   0 sora      (1003) vahedilab (10000)    52764 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/dist/stripenn-1.1.46-py3-none-any.whl
--rw-r--r--   0 sora      (1003) vahedilab (10000)    48700 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/dist/stripenn-1.1.46.tar.gz
--rw-r--r--   0 sora      (1003) vahedilab (10000)   265139 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/dist/stripenn-1.1.47-py3-none-any.whl
--rw-r--r--   0 sora      (1003) vahedilab (10000)   224543 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/dist/stripenn-1.1.47.tar.gz
--rw-r--r--   0 sora      (1003) vahedilab (10000)       43 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/entry_points.txt
--rw-r--r--   0 sora      (1003) vahedilab (10000)      291 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/pyproject.toml
--rw-r--r--   0 sora      (1003) vahedilab (10000)       90 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/requires.txt
--rw-r--r--   0 sora      (1003) vahedilab (10000)      109 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/setup.cfg
--rw-r--r--   0 sora      (1003) vahedilab (10000)      957 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/setup.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/src/
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/.gitignore
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.108892 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/inspectionProfiles/
--rw-r--r--   0 sora      (1003) vahedilab (10000)      174 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 sora      (1003) vahedilab (10000)      185 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/misc.xml
--rw-r--r--   0 sora      (1003) vahedilab (10000)      258 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/modules.xml
--rw-r--r--   0 sora      (1003) vahedilab (10000)      441 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/src.iml
--rw-r--r--   0 sora      (1003) vahedilab (10000)     1878 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/.idea/workspace.xml
--rw-r--r--   0 sora      (1003) vahedilab (10000)    10917 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/ImageProcessing.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__init__.py
-drwxr-xr-x   0 sora      (1003) vahedilab (10000)        0 2022-10-31 17:54:12.112892 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/
--rw-r--r--   0 sora      (1003) vahedilab (10000)     7355 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/ImageProcessing.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)      150 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2857 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/cli.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)    36987 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/getStripe.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2240 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/score.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2102 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/seeimage.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     5297 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/stats.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     5429 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/__pycache__/stripenn.cpython-38.pyc
--rw-r--r--   0 sora      (1003) vahedilab (10000)     3567 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/cli.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)    58343 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/getStripe.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     8185 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/observed_over_expected.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     2433 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/score.py
--rwxr-xr-x   0 sora      (1003) vahedilab (10000)     3323 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/seeimage.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)     7101 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/stats.py
--rwxr-xr-x   0 sora      (1003) vahedilab (10000)    10401 2022-10-31 17:02:38.000000 stripenn-1.1.65.9/stripenn.egg-info/src/stripenn.py
--rw-r--r--   0 sora      (1003) vahedilab (10000)        4 2022-10-31 17:54:12.000000 stripenn-1.1.65.9/stripenn.egg-info/top_level.txt
+drwxrwxr-x   0 sora      (1000) sora      (1000)        0 2020-11-30 23:53:30.641714 stripenn-1.1.7/
+-rw-rw-r--   0 sora      (1000) sora      (1000)      749 2020-11-30 23:53:30.641714 stripenn-1.1.7/PKG-INFO
+-rw-rw-r--   0 sora      (1000) sora      (1000)     8060 2020-11-30 22:34:05.000000 stripenn-1.1.7/README.rst
+-rw-rw-r--   0 sora      (1000) sora      (1000)      291 2020-11-24 18:03:32.000000 stripenn-1.1.7/pyproject.toml
+-rw-rw-r--   0 sora      (1000) sora      (1000)      109 2020-11-30 23:53:30.645714 stripenn-1.1.7/setup.cfg
+-rw-rw-r--   0 sora      (1000) sora      (1000)      961 2020-11-30 23:53:05.000000 stripenn-1.1.7/setup.py
+drwxrwxr-x   0 sora      (1000) sora      (1000)        0 2020-11-30 23:53:30.641714 stripenn-1.1.7/stripenn/
+-rw-rw-r--   0 sora      (1000) sora      (1000)    10917 2020-11-04 23:18:46.000000 stripenn-1.1.7/stripenn/ImageProcessing.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)        0 2020-11-24 18:09:17.000000 stripenn-1.1.7/stripenn/__init__.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     3243 2020-11-30 21:01:06.000000 stripenn-1.1.7/stripenn/cli.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)    29286 2020-11-24 12:53:22.000000 stripenn-1.1.7/stripenn/getStripe.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     8185 2020-11-09 21:31:20.000000 stripenn-1.1.7/stripenn/observed_over_expected.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     1640 2020-11-25 00:03:36.000000 stripenn-1.1.7/stripenn/score.py
+-rwxrwxr-x   0 sora      (1000) sora      (1000)     2309 2020-11-24 21:08:52.000000 stripenn-1.1.7/stripenn/seeimage.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     7100 2020-11-12 16:32:10.000000 stripenn-1.1.7/stripenn/stats.py
+-rwxrwxr-x   0 sora      (1000) sora      (1000)     9238 2020-11-24 21:59:30.000000 stripenn-1.1.7/stripenn/stripenn.py
+drwxrwxr-x   0 sora      (1000) sora      (1000)        0 2020-11-30 23:53:30.641714 stripenn-1.1.7/stripenn.egg-info/
+-rw-rw-r--   0 sora      (1000) sora      (1000)      749 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/PKG-INFO
+-rw-rw-r--   0 sora      (1000) sora      (1000)      748 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/SOURCES.txt
+-rw-rw-r--   0 sora      (1000) sora      (1000)        1 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/dependency_links.txt
+-rw-rw-r--   0 sora      (1000) sora      (1000)       48 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/entry_points.txt
+-rw-rw-r--   0 sora      (1000) sora      (1000)       90 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/requires.txt
+-rw-rw-r--   0 sora      (1000) sora      (1000)       15 2020-11-30 23:53:30.000000 stripenn-1.1.7/stripenn.egg-info/top_level.txt
+drwxrwxr-x   0 sora      (1000) sora      (1000)        0 2020-11-30 23:53:30.641714 stripenn-1.1.7/tests/
+-rw-rw-r--   0 sora      (1000) sora      (1000)        0 2020-11-24 18:03:32.000000 stripenn-1.1.7/tests/__init__.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)      961 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/setup.py
+drwxrwxr-x   0 sora      (1000) sora      (1000)        0 2020-11-30 23:53:30.641714 stripenn-1.1.7/tests/stripenn/
+-rw-rw-r--   0 sora      (1000) sora      (1000)    10917 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/ImageProcessing.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)        0 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/__init__.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     3243 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/cli.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)    29286 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/getStripe.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     8185 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/observed_over_expected.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     1640 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/score.py
+-rwxrwxr-x   0 sora      (1000) sora      (1000)     2309 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/seeimage.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)     7100 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/stats.py
+-rwxrwxr-x   0 sora      (1000) sora      (1000)     9238 2020-11-30 22:59:38.000000 stripenn-1.1.7/tests/stripenn/stripenn.py
+-rw-rw-r--   0 sora      (1000) sora      (1000)       89 2020-11-24 18:03:32.000000 stripenn-1.1.7/tests/test_stripenn.py
```

### Comparing `stripenn-1.1.65.9/README.rst` & `stripenn-1.1.7/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,88 @@
 ========
-STRIPENN (ver 1.1.65)
+STRIPENN
 ========
 --------------------------------------------------------------------
 Architectural stripe detection from 3D genome conformation data
 --------------------------------------------------------------------
 
 .. image:: https://img.shields.io/pypi/v/pip.svg
    :target: https://pypi.org/project/stripenn/
 
 .. image:: https://github.com/ysora/stripenn/blob/main/image/example_call.png
-   :height: 500px
-   :width: 500px
+   :height: 20px
+   :width: 20px
 
 Contents
 ########
 * Introduction
 * Installation
 * Quick start
 * Usage
 
 Introduction
 ############
-**Stripenn** is a command line interface python package developed for detection of atchitectural stripes from chromatin conformation capture (3C) data. Then what are 3C data and stripes?
+**stripenn** is a command line interface python package developed for detection of atchitectural stripes from 3D genome conformation data. Then what are 3D genome conformation data and stripes?
 
-* **Chromatin conformation capture technique**
-    Basically, the chromatin conformation capture technique measures the frequency of DNA interactions. There are several sequencing techniques to see the genome-wide DNA interactions such as `Hi-C <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2858594/>`_ , `HiChIP <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5501173/>`_,  `PLAC-seq <https://www.nature.com/articles/cr2016137>`_ and `micro-C <https://www.cell.com/fulltext/S0092-8674(15)00638-8>`_. Currently, imaging-based methods are also developed to construct the spatial distance map of DNA interaction ( `Su et al., 2020 <https://www.sciencedirect.com/science/article/pii/S0092867420309405>`_ ). These data have revealed that our genome is highly organized including special features such as compartment, TAD, loops and stripes.
+* **3D genome conformation data**
+    The human DNA is about 2m in length and it is folded within small cells. However, the folding pattern is not random and this DNA 3D conformation is important in gene regulation. There are several sequencing techniques to see the genome-wide DNA interactions such as `Hi-C <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2858594/>`_ , `HiChIP <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5501173/>`_,  `PLAC-seq <https://www.nature.com/articles/cr2016137>`_ and `micro-C <https://www.cell.com/fulltext/S0092-8674(15)00638-8>`_. Currently, imaging-based methods are also developed to construct the spatial distance map of DNA ( `Su et al., 2020 <https://www.sciencedirect.com/science/article/pii/S0092867420309405>`_ ). From these data, special structures such as compartment, TAD and loops have been revealed.
 
 * **Architectural stripe**
-    Architectural stripes are shown in the figure above (highlighted in green border). Stripe is one of the distinctive features found from 3C data. It was first predicted by `Fudenberg et al., Cell Reports, 2016 <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4889513/>`_. As shown in the figure above, it is a linear pattern where an anchor forms interaction with contiguous genomic region. It is known that stripes are enriched with super-enhancers, and also it is a hopspot for DNA damage. To address more characteristics of stripes, we need accurate stripe caller and that's why we've developed Stripenn.
-
-Requirement
-############
-**Python 3.8 or higher version**
+    Architectural stripes are one of the distinctive features found from 3D genome conformation data. It was first reported from `Vian et al., Cell, 2018 <https://www.sciencedirect.com/science/article/pii/S0092867418304045>`_. As shown in the figure above, it has anchor domain and contiguous regions are subsequently interacting with the anchor. It is known that stripes contains a large number of super-enhancers, and also it is a hopspot for DNA damage. However, more systematic analysis of this feature is needed, and that's why we developed Stripenn. :)
 
 Installation
 ############
 **Linux / Mac**
 
 Open terminal and type following:
 ::
 
     pip install stripenn
 
 If pip is not installed, install pip first: `pip installation <https://pip.pypa.io/en/stable/installing/>`_
 
-When pip is not working, replace it with 'pip3'. Installation may take several minutes.
+When pip is not working, replace it with 'pip3'
 
 **Windows**
 
 Windows users will fail to install stripenn using the above command. This is because the pypairix package installed with the cooler package does not support Windows. But we can still install stripenn on Windows! The strategy is (1) to install all dependency packages except pypairix and then (2) to install stripenn without dependency packages. To do this, type followings on command windows:
 ::
 
    pip install simplejson multiprocess pandas numpy matplotlib opencv-python scikit-image scipy joblib tqdm Bottleneck typer pathlib
    pip install --no-deps cooler
    pip install --no-deps stripenn
 
 If you have any trouble with installation, please leave it on issue board.
 
 Quick start (Example run)
 #########################
-Let's check if stripenn is working or not with a simple example which might take less than 5 minutes. This example .cool file is Smc1-HiChIP of only chr16 of mouse T lymphocyte (`Fasolino et al., Immunity, 2020 <https://www.sciencedirect.com/science/article/pii/S1074761320300303>`_).
+Let's check if stripenn is working or not with a simple example.
 ::
 
    cd <Test_Directory> # Move to your test directory
-   wget https://www.dropbox.com/s/1bb2npvrzp3by5y/BL6.DPT.chr16.mcool?dl=0 -O test.mcool --no-check-certificate
-   stripenn compute --cool test.mcool::resolutions/5000 --out output_dir/ -k 16 -m 0.95,0.96,0.97,0.98,0.99
-
-*Tip*: For those whose computer has not enough memory (e.g., < 24GB), we provide slow version of Stripenn as follow:
-::
+   wget https://data.4dnucleome.org/files-processed/4DNFISA93XFU/@@download/4DNFISA93XFU.mcool -O Vian_aB_30hrs.mcool
+   stripenn compute --cool ../hic/Vian_aB_30hrs.mcool::resolutions/5000 --out output_dir/ -k chr19 -m 0.99
 
-   stripenn compute --cool test.mcool::resolutions/5000 --out output_dir/ -k 16 -m 0.95,0.96,0.97,0.98,0.99 -s
+Here, the example mcool file contains Hi-C data of mouse activated B cell (`Vian et al., Cell, 2018 <https://www.sciencedirect.com/science/article/pii/S0092867418304045>`_).
 
-In this example, stripes are searched from chromosome 16 of 5kb-resolution data for short running time.
+Stripes are searched from chromosome 19 of 5kb-resolution data for short running time.
 
 **Output**
 ::
 
    cat output_dir/result_filtered.txt
 
 will show a result table including 12 columns like below.
 
 .. csv-table:: result_filtered.txt
    :header: "chr", "pos1","pos2","chr2","pos3","pos4","length","width","Mean","maxpixel","pvalue","Stripiness"
 
-    "16", "23970001", "24015000", "16", "23970001", "24870000", "900000", "45000", "2.913", "98.0%", "0.025", "10.809"
-    "16", "10550001", "10595000", "16", "10550001", "10870000", "320000", "45000", "6.638", "99.0%", "0.042", "10.020"
-    "16", "32490001", "32525000", "16", "32490001", "32700000", "210000", "35000", "8.117", "98.0%", "0.012", "5.254"
+    "chr19", "24285001", "24320000", "chr19", "24285001", "24640000", "355000", "35000", "10.3924", "98.0%", "0.04653", "3.6686"
+    "chr19", "6305001", "6345000", "chr19", "6125001", "6345000", "220000", "40000", "17.5088", "98.0%", "0.059462", "2.0324"
+    "chr19", "53905001", "53940000", "chr19", "53750001", "53940000", "190000", "35000", "15.7701", "98.0%", "0.03981", "0.5934"
 
 Each line represents the coordinates and other information of a vertical stripe.
 
 .. image:: https://github.com/ysora/stripenn/blob/main/image/readme1.png
 
 * chr: chromosome
 * pos1: x1 position of stripe
@@ -109,77 +102,66 @@
 
 Stripenn has three functions.
 
 * compute
 * score
 * seeimage
 
-**compute**
-:It is main function of stripenn that detects stripes using image-processing method. There are several options in it.
+1) compute: It is main function of stripenn that detects stripes using image-processing method. There are several options in it.
 
 Options:
   --cool TEXT             Path to cool file  [required]
   -o, --out TEXT          Path to output directory  [required]
   --norm TEXT             Normalization method. It should be one of the column
                           name of Cooler.bin(). Check it with
                           Cooler.bins().columns (e.g., KR, VC, VC_SQRT)
                           [default: KR]
 
   -k, --chrom TEXT        Set of chromosomes. e.g., 'chr1,chr2,chr3', 'all'
                           will generate stripes from all chromosomes
                           [default: all]
 
-  -c, --canny FLOAT       Canny edge detection parameter.  [default: 2.0]
+  -c, --canny FLOAT       Canny edge detection parameter.  [default: 2.5]
   -l, --minL INTEGER      Minimum length of stripe.  [default: 10]
-  -w, --maxW INTEGER      Maximum width of stripe.  [default: 8]
+  -w, --maxW INTEGER      Maximum width of stripe.  [default: 8] --> we recommend to adjust it to 16 using 5kb-resolution data
   -m, --maxpixel TEXT     Percentiles of the contact frequency data to
                           saturate the image. Separated by comma  [default:
                           0.95,0.96,0.97,0.98,0.99]
 
   -n, --numcores INTEGER  The number of cores will be used.  [default: 40]
   -p, --pvalue FLOAT      P-value cutoff for stripe.  [default: 0.1]
-  --mask TEXT             Column coordinates to be masked. e.g.,
-                          chr9:12345678-12345789  [default: 0]
+  --help                  Show this message and exit.
 
-  -s BOOLEAN_FLAG         Use this if system memory is low.  [default: False]
-  -b --bfilter INTEGER    Kernel size of Mean filter.  [default: 3]
-
-
-**score**
-:It calculates p-value and stripiness of given stripes on given 3D genome conformation data. It is useful to compare stripiness of given stripes in two datasets.
+2) score: It calculates p-value and stripiness of given stripes on given 3D genome conformation data. It is useful to compare stripiness of given stripes in two datasets.
 
 Options:
   --cool TEXT             Path to cool file  [required]
   -c, --coord TEXT        Path to stripe coordinate table  [required]
   --norm TEXT             Normalization method. It should be one of the column
                           name of Cooler.bin(). Check it with
                           Cooler.bins().columns (e.g., KR, VC, VC_SQRT)
                           [default: KR]
 
   -h, --header            Does the stripe coordinate table have header?
                           [default: False]
 
   -n, --numcores INTEGER  The number of cores will be used.  [default: 40]
   -o, --out TEXT          Path to output file  [default: scores.out]
-  
-   In the output, four columns (O_Mean_added, O_Sum_added, O/E_Mean_added and O/E_Total_added) are added in addition to the stripiness and P-value, and each represents (1) Mean of observed contact frequency, (2) Total sum of observed contact frequency, (3) Mean of observed/expected contact frequency and (4) total sum of observed/expected contact frequency within stripe. 
+  --help                  Show this message and exit.
 
-**seeimage**
-:This function was included to help users choose proper maximum-pixel-value. It draws heatmap image of given position for given maximum pixel paramter.
+3) seeimage: This function was included to help users choose proper maximum-pixel-value.
 
-Options:
-  --cool TEXT          Path to cool file  [required]
-  -p, --position TEXT  Genomic position (e.g., chr1:135010000-136000000)
-                       [required]
-
-  -m, --maxpixel TEXT  Quantile for the pixel saturation. (e.g., 0.95)
-                       [default: 0.95,0.96,0.97,0.98,0.99]
-
-  -o, --out TEXT       Output prefix  [default: ./my_heatmap]
-  --norm TEXT          Normalization method. It should be one of the column
-                       name of Cooler.bin(). Check it with
-                       Cooler.bins().columns (e.g., KR, VC, VC_SQRT)
-                       [default: KR]
+  --cool TEXT           Path to cool file  [required]
+  -p, --position TEXT   Genomic position (e.g., chr1:135010000-136000000)
+                        [required]
+
+  -m, --maxpixel FLOAT  Quantile for the pixel saturation. (e.g., 0.95)
+                        [default: 0.95]
 
-  -s                   Use if system memory is low.  [default: False]
+  -o, --out TEXT        Path to output directory  [default: ./heatmap.png]
+  --norm TEXT           Normalization method. It should be one of the column
+                        name of Cooler.bin(). Check it with
+                        Cooler.bins().columns (e.g., KR, VC, VC_SQRT)
+                        [default: KR]
 
+  --help                Show this message and exit.
```

### Comparing `stripenn-1.1.65.9/setup.py` & `stripenn-1.1.7/tests/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-README = (HERE / "README.rst").read_text()
+README = (HERE / "README.md").read_text()
 
 setup(
     name = 'stripenn',
-    version = '1.1.65.9',
+    version = '1.1.5',
     author = 'Sora Yoon',
     author_email = 'sora.yoon@pennmedicine.upenn.edu',
     description = "Image-processing based detection of architectural stripes from chromatic conformation data",
     long_description=README,
     long_description_content_type="text/markdown",
     url = 'https://github.com/ysora/stripenn',
     #package_dir={'': 'src'},
@@ -19,10 +19,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["cooler","pandas","numpy","matplotlib","opencv-python","scikit-image","scipy","joblib","tqdm",'typer','pathlib'],
     entry_points={
-    	"console_scripts": ["stripenn=src.cli:main"]
+    	"console_scripts": ["stripenn=stripenn.cli:main"]
     },
 )
```

### Comparing `stripenn-1.1.65.9/src/ImageProcessing.py` & `stripenn-1.1.7/stripenn/ImageProcessing.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/src/cli.py` & `stripenn-1.1.7/stripenn/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 import typer
-from src import stripenn
-from src import getStripe
-from src import seeimage
-from src import score
+from . import stripenn
+from . import getStripe
+from . import seeimage
+from . import score
 import multiprocessing
 
 app = typer.Typer()
 
 @app.command('compute')
 def execute(
     cool: str = typer.Option(..., "--cool",help="Path to cool file"),
     out: str = typer.Option(..., "--out", "-o", help="Path to output directory"),
     norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
     chrom: str = typer.Option('all', "--chrom", "-k", help="Set of chromosomes. e.g., 'chr1,chr2,chr3', 'all' will generate stripes from all chromosomes"),
-    canny: float = typer.Option(2.0, "--canny", "-c", help="Canny edge detection parameter."),
-    minL: int = typer.Option(10,'--minL','-l', help="Minimum length of stripe."),
-    maxW: int = typer.Option(8, '--maxW','-w', help="Maximum width of stripe."),
-    maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99','--maxpixel','-m', help="Percentiles of the contact frequency data to saturate the image. Separated by comma"),
-    numcores: int = typer.Option(multiprocessing.cpu_count(), '--numcores','-n', help='The number of cores will be used.'),
-    pvalue: float = typer.Option(0.1,  '--pvalue','-p', help='P-value cutoff for stripe.'),
-    mask: str = typer.Option('0', "--mask", help='Column coordinates to be masked. e.g., chr9:12345678-12345789'),
-    slow: bool= typer.Option(False,"-s", help='Use if system memory is low.'),
-    bfilter: int=typer.Option(3,"--bfilter",'-b',help="Mean filter size. should be an odd number")
+    canny: float = typer.Option(2.5, "--canny", "-c", help="Canny edge detection parameter."),
+    minL: int = typer.Option(10,'-l','--minL', help="Minimum length of stripe."),
+    maxW: int = typer.Option(8, '-w','--maxW', help="Maximum width of stripe."),
+    maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99','-m','--maxpixel', help="Percentiles of the contact frequency data to saturate the image. Separated by comma"),
+    numcores: int = typer.Option(multiprocessing.cpu_count(), '-n','--numcores', help='The number of cores will be used.'),
+    pvalue: float = typer.Option(0.1, '-p', '--pvalue', help='P-value cutoff for stripe.')
 ):
     """Finds stripe coordinates from 3D genomic data
     """
-    stripenn.compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue, mask, slow, bfilter)
+    stripenn.compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue)
 
 @app.command('seeimage')
 def seeimag(
         cool: str = typer.Option(..., "--cool",help="Path to cool file"),
         position: str = typer.Option(..., "--position",'-p', help="Genomic position (e.g., chr1:135010000-136000000)"),
-        maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99',"--maxpixel",'-m', help="Quantile for the pixel saturation. (e.g., 0.95)"),
+        maxpixel: float = typer.Option(0.95,"--maxpixel",'-m', help="Quantile for the pixel saturation. (e.g., 0.95)"),
         out: str = typer.Option('./heatmap.png', "--out", "-o", help="Path to output directory"),
         norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
-        slow: bool= typer.Option(False,'-s' , help='Use if system memory is low.')
 ):
     """ Draws heatmap image of given position and color saturation parameter (maxpixel).
     """
-    seeimage.seeimage(cool, position, maxpixel, norm, out, slow)
+    seeimage.seeimage(cool, position, maxpixel, norm, out)
     return 0
 
 @app.command('score')
 def scoring(
     cool: str = typer.Option(..., "--cool",help="Path to cool file"),
     coordinates: str = typer.Option(..., "--coord",'-c', help="Path to stripe coordinate table"),
     norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
+    header: bool = typer.Option(False, "--header", '-h', help="Does the stripe coordinate table have header?"),
     numcores: int = typer.Option(multiprocessing.cpu_count(), '-n','--numcores', help='The number of cores will be used.'),
-    out: str = typer.Option('scores.out','--out','-o',help='Path to output file'),
-    mask: str = typer.Option('0', "--mask", help='Column coordinates to be masked. e.g., chr9:12345678-12345789')
+    out: str = typer.Option('scores.out','--out','-o',help='Path to output file')
 ):
     """ Calculates p-value and stripiness of given stripes based on given 3D genome conformation data.
     """
-    score.getScore(cool, coordinates,norm,numcores,out,mask)
+    score.getScore(cool, coordinates,norm,header,numcores,out)
 
 
 def main():
     app()
 
 if __name__ == "__main__":
     app()
```

### Comparing `stripenn-1.1.65.9/src/observed_over_expected.py` & `stripenn-1.1.7/stripenn/observed_over_expected.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/src/stats.py` & `stripenn-1.1.7/stripenn/stats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
             tempVal += K[0][j]*COL[j][i-1] + K[1][j]*COL[j][i] + K[2][j]*COL[j][i+1]
         if ncol_K == 3 and tempVal < 0:
             tempVal *= -1
         result.append(tempVal)
     return result
 
 def moving_average(x,w):
-    return np.convolve(x, np.ones(w),'valid')/w
+    return np.convolve(x, np.ones(w),'valid')/w
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/ImageProcessing.py` & `stripenn-1.1.7/tests/stripenn/ImageProcessing.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/cli.py` & `stripenn-1.1.7/tests/stripenn/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 import typer
-from src import stripenn
-from src import getStripe
-from src import seeimage
-from src import score
+from . import stripenn
+from . import getStripe
+from . import seeimage
+from . import score
 import multiprocessing
 
 app = typer.Typer()
 
 @app.command('compute')
 def execute(
     cool: str = typer.Option(..., "--cool",help="Path to cool file"),
     out: str = typer.Option(..., "--out", "-o", help="Path to output directory"),
     norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
     chrom: str = typer.Option('all', "--chrom", "-k", help="Set of chromosomes. e.g., 'chr1,chr2,chr3', 'all' will generate stripes from all chromosomes"),
     canny: float = typer.Option(2.5, "--canny", "-c", help="Canny edge detection parameter."),
-    minL: int = typer.Option(10,'--minL','-l', help="Minimum length of stripe."),
-    maxW: int = typer.Option(8, '--maxW','-w', help="Maximum width of stripe."),
-    maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99','--maxpixel','-m', help="Percentiles of the contact frequency data to saturate the image. Separated by comma"),
-    numcores: int = typer.Option(multiprocessing.cpu_count(), '--numcores','-n', help='The number of cores will be used.'),
-    pvalue: float = typer.Option(0.1,  '--pvalue','-p', help='P-value cutoff for stripe.'),
-    mask: str = typer.Option('0', "--mask", help='Column coordinates to be masked. e.g., chr9:12345678-12345789'),
-    slow: bool= typer.Option(False,"-s", help='Use if system memory is low.')
+    minL: int = typer.Option(10,'-l','--minL', help="Minimum length of stripe."),
+    maxW: int = typer.Option(8, '-w','--maxW', help="Maximum width of stripe."),
+    maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99','-m','--maxpixel', help="Percentiles of the contact frequency data to saturate the image. Separated by comma"),
+    numcores: int = typer.Option(multiprocessing.cpu_count(), '-n','--numcores', help='The number of cores will be used.'),
+    pvalue: float = typer.Option(0.1, '-p', '--pvalue', help='P-value cutoff for stripe.')
 ):
     """Finds stripe coordinates from 3D genomic data
     """
-    stripenn.compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue, mask, slow)
+    stripenn.compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue)
 
 @app.command('seeimage')
 def seeimag(
         cool: str = typer.Option(..., "--cool",help="Path to cool file"),
         position: str = typer.Option(..., "--position",'-p', help="Genomic position (e.g., chr1:135010000-136000000)"),
-        maxpixel: str = typer.Option('0.95,0.96,0.97,0.98,0.99',"--maxpixel",'-m', help="Quantile for the pixel saturation. (e.g., 0.95)"),
+        maxpixel: float = typer.Option(0.95,"--maxpixel",'-m', help="Quantile for the pixel saturation. (e.g., 0.95)"),
         out: str = typer.Option('./heatmap.png', "--out", "-o", help="Path to output directory"),
         norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
-        slow: bool= typer.Option(False,'-s' , help='Use if system memory is low.')
 ):
     """ Draws heatmap image of given position and color saturation parameter (maxpixel).
     """
-    seeimage.seeimage(cool, position, maxpixel, norm, out, slow)
+    seeimage.seeimage(cool, position, maxpixel, norm, out)
     return 0
 
 @app.command('score')
 def scoring(
     cool: str = typer.Option(..., "--cool",help="Path to cool file"),
     coordinates: str = typer.Option(..., "--coord",'-c', help="Path to stripe coordinate table"),
     norm: str = typer.Option('KR',"--norm",help="Normalization method. It should be one of the column name of Cooler.bin(). Check it with Cooler.bins().columns (e.g., KR, VC, VC_SQRT)"),
+    header: bool = typer.Option(False, "--header", '-h', help="Does the stripe coordinate table have header?"),
     numcores: int = typer.Option(multiprocessing.cpu_count(), '-n','--numcores', help='The number of cores will be used.'),
-    out: str = typer.Option('scores.out','--out','-o',help='Path to output file'),
-    mask: str = typer.Option('0', "--mask", help='Column coordinates to be masked. e.g., chr9:12345678-12345789')
+    out: str = typer.Option('scores.out','--out','-o',help='Path to output file')
 ):
     """ Calculates p-value and stripiness of given stripes based on given 3D genome conformation data.
     """
-    score.getScore(cool, coordinates,norm,numcores,out,mask)
+    score.getScore(cool, coordinates,norm,header,numcores,out)
 
 
 def main():
     app()
 
 if __name__ == "__main__":
     app()
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/observed_over_expected.py` & `stripenn-1.1.7/tests/stripenn/observed_over_expected.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/seeimage.py` & `stripenn-1.1.7/stripenn/seeimage.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 import os
 import pandas as pd
 import numpy as np
 import warnings
 import time
 import sys
 import cv2 as cv
-import matplotlib
-matplotlib.use('Agg')
 import matplotlib.pyplot as plt
-from src import getStripe
 
 '''
 def argumentParser():
     parser = argparse.ArgumentParser(description='Stripenn')
     parser.add_argument("cool", help="Balanced cool file.")
     parser.add_argument("position", help="Genomic position (e.g., chr1:135010000-136000000)")
     parser.add_argument("maxpixel", help="Quantile for the pixel saturation. (e.g., 0.95)")
@@ -30,21 +27,18 @@
     norm = args.norm
     maxpixel = args.maxpixel
     maxpixel = float(maxpixel)
 
     return(cool, position, maxpixel, norm, out)
 '''
 
-def seeimage(cool, position, maxpixel, norm, out, slow):
+def seeimage(cool, position, maxpixel, norm, out):
     #cool, position, maxpixel, norm, out = argumentParser()
     Lib = cooler.Cooler(cool)
 
-    maxpixel = maxpixel.split(',')
-    maxpixel = list(map(float, maxpixel))
-
     PossibleNorm = Lib.bins().columns
     if norm == 'None':
         norm = False
     elif norm not in PossibleNorm:
         print('Possible normalization methods are:')
         print('None')
         for n in range(3,len(PossibleNorm)):
@@ -52,52 +46,32 @@
         print("Invalid normalization method. Normalization method is forced to None")
         norm = False
 
     unbalLib = Lib.matrix(balance=norm)
     all_chromnames = Lib.chromnames
     chr = position.split(':')
     chr = chr[0]
-
     if chr not in all_chromnames:
         sys.exit("Invalid chromosome name.")
-
-    all_chromnames = Lib.chromnames
-    all_chromsizes = Lib.chromsizes
-    chrom_remain_idx = np.where(all_chromsizes > 500000)[0]
-    all_chromnames = [all_chromnames[i] for i in chrom_remain_idx]
-    all_chromsizes = all_chromsizes[chrom_remain_idx]
-    chromnames = [chr]
-    chromsizes = all_chromsizes[chr]
-    if len(all_chromnames) == 0:
-        sys.exit("Exit: All chromosomes are shorter than 50kb.")
-
-    unbalLib = Lib.matrix(balance=norm)
-    resol = Lib._info['bin-size']
-    obj = getStripe.getStripe(unbalLib, resol, 10, 8, 2.5, all_chromnames, chromnames, all_chromsizes, chromsizes,2)
-
-    if slow:
-        print("#####...Slowly estimating Maximum pixel values...#####")
-        MP = obj.getQuantile_slow(Lib, [chr], maxpixel)
-    else:
-        MP = obj.getQuantile_original(Lib, [chr], maxpixel)
+    cfm = unbalLib.fetch(chr)
+    M = np.quantile(a=cfm[cfm > 0], q=maxpixel, interpolation='linear')
+    del cfm
 
     A = unbalLib.fetch(position,position)
 
     framesize = A.shape[0]
+    red = np.ones((framesize, framesize)) * 255
+    blue = 255 * (M - A) / M
+    blue[np.where(blue < 0)] = 0
+    green = blue
+
+    img = cv.merge((red / 255, green / 255, blue / 255))
+    img = np.clip(img, a_min=0, a_max=1)
+
 
-    for i in range(len(maxpixel)):
-        perc = str(maxpixel[i])
-        M = MP[chr][i]
-        red = np.ones((framesize, framesize)) * 255
-        blue = 255 * (M - A) / M
-        blue[np.where(blue < 0)] = 0
-        green = blue
-
-        img = cv.merge((red / 255, green / 255, blue / 255))
-        img = np.clip(img, a_min=0, a_max=1)
-
-        fig = plt.subplot(111)
-        plt.imshow(img)
-        plt.title(position)
-        fig.figure.savefig(out + "_" + position + "_" + perc + "qt" + '.png')
+    fig = plt.subplot(111)
+    plt.imshow(img)
+    plt.title(position)
+    plt.show()
+    fig.figure.savefig(out)
 
     return 0
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/stats.py` & `stripenn-1.1.7/tests/stripenn/stats.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
             tempVal += K[0][j]*COL[j][i-1] + K[1][j]*COL[j][i] + K[2][j]*COL[j][i+1]
         if ncol_K == 3 and tempVal < 0:
             tempVal *= -1
         result.append(tempVal)
     return result
 
 def moving_average(x,w):
-    return np.convolve(x, np.ones(w),'valid')/w
+    return np.convolve(x, np.ones(w),'valid')/w
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/src/stripenn.py` & `stripenn-1.1.7/stripenn/stripenn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import cooler
 import multiprocessing
-from src import getStripe
+from stripenn import getStripe
 import os
 import shutil
 import errno
 import pandas as pd
 import numpy as np
 import warnings
 import time
@@ -109,70 +109,66 @@
     lef = unbalLib.fetch('chr16:96100001-96150000','chr16:95330001-96220000')
     lefmean = np.mean(lef,axis=0)
     rig = unbalLib.fetch('chr16:96220001-96270000','chr16:95330001-96220000')
     rigmean = np.mean(rig,axis=0)
     ld = np.subtract(amean,lefmean)
     rd = np.subtract(amean,rigmean)
     '''
-def addlog(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue, mask):
+def addlog(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue):
     if out[-1] != '/':
         out += '/'
     outfile=open(out + "stripenn.log",'w')
     outfile.write('cool: ' + cool + '\n')
     outfile.write('out: ' + out + '\n')
     outfile.write('norm: ' + norm + '\n')
-    outfile.write('chrom: ' + str(chrom) + '\n')
-    outfile.write('canny: ' + str(canny) + '\n')
+    outfile.write('chrom: ' + chrom + '\n')            
     outfile.write('minL: ' + str(minL) + '\n')            
     outfile.write('maxW: ' + str(maxW) + '\n')                
-    outfile.write('maxpixel: ' + str(maxpixel) + '\n')
+    outfile.write('maxpixel: ' + maxpixel + '\n')
     outfile.write('num_cores: ' + str(numcores) + '\n')
     outfile.write('pvalue: ' + str(pvalue) + '\n')
-    outfile.write('mask: ' + str(mask) + '\n')
+    
     outfile.close()
     
     
-def compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue, mask, slow):
+def compute(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue):
     np.seterr(divide='ignore', invalid='ignore')
     t_start = time.time()
     if out[-1] != '/':
         out += '/'
     makeOutDir(out)
-    addlog(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue, mask)
+    addlog(cool, out, norm, chrom, canny, minL, maxW, maxpixel, numcores, pvalue)
     maxpixel = maxpixel.split(',')
     maxpixel = list(map(float, maxpixel))
     chroms = chrom.split(',')
     minH = minL
     core = numcores
     pcut = pvalue
     #cool, out, norm, chroms, canny, minH, maxW, maxpixel, core, pcut = argumentParser()
     print('Result will be stored in %s' % (out))
 
     Lib = cooler.Cooler(cool)
     PossibleNorm = Lib.bins().columns
     if norm == 'None':
         norm = False
-    elif norm == 'weight':
-        norm = True
     elif norm not in PossibleNorm:
         print('Possible normalization methods are:')
         print('None')
         for n in range(3,len(PossibleNorm)):
             print(PossibleNorm[n])
         print("Invalid normalization method. Normalization method is forced to None")
         norm = False
 
     all_chromnames = Lib.chromnames
     all_chromsizes = Lib.chromsizes
-    chrom_remain_idx = [i for i in range(len(all_chromnames)) if 'JH5' not in all_chromnames[i] and 'GL4' not in all_chromnames[i] and all_chromnames[i] != 'M' and all_chromnames[i] != "chrM" and all_chromnames[i] != "Y" and all_chromnames[i] != "chrY"]
+    chrom_remain_idx = np.where(all_chromsizes > 500000)[0]
     all_chromnames = [all_chromnames[i] for i in chrom_remain_idx]
     all_chromsizes = all_chromsizes[chrom_remain_idx]
     chromnames = all_chromnames
     chromsizes = all_chromsizes
-
     if len(all_chromnames) == 0:
         sys.exit("Exit: All chromosomes are shorter than 50kb.")
     warnflag = False
     if chroms[0] != 'all':
         idx = []
         for item in chroms:
             if item in all_chromnames:
@@ -181,55 +177,41 @@
                 warnings.warn('\nThere is no chromosomes called '+str(item)+' in the provided .cool file or it is shorter than 50kb.')
                 warnflag = True
         if warnflag:
             warnings.warn('\nThe possible chromosomes are: '+ ', '.join(all_chromnames))
         chromnames = chroms
         chromsizes = all_chromsizes[idx]
 
+
     unbalLib = Lib.matrix(balance=norm)
-    resol = Lib.binsize
+    resol = Lib._info['bin-size']
     obj = getStripe.getStripe(unbalLib, resol, minH, maxW, canny, all_chromnames, chromnames, all_chromsizes, chromsizes,core)
-    print('#######################################\nMaximum pixel value calculation ... \n#######################################')
-    if slow:
-        print("#####...Slowly estimating Maximum pixel values...#####")
-        MP = getStripe.getStripe.getQuantile_slow(obj,Lib,chromnames,maxpixel)
-    else:
-        MP = getStripe.getStripe.getQuantile_original(obj,Lib,chromnames,maxpixel)
-    print('#######################################\nExpected value calculation ...\n#######################################\n')
-    EV = getStripe.getStripe.mpmean(obj)
     print('#######################################\nBackground distribution estimation ...\n#######################################\n')
-    bgleft_up, bgright_up, bgleft_down, bgright_down = getStripe.getStripe.nulldist(obj)
+    bgleft, bgright = getStripe.getStripe.nulldist(obj)
     print('#################################################\nFinding candidate stripes from each chromosome ...\n#################################################\n')
     result_table = pd.DataFrame(columns=['chr', 'pos1', 'pos2', 'chr2', 'pos3', 'pos4', 'length', 'width', 'total', 'Mean',
                                    'maxpixel', 'num', 'start', 'end', 'x', 'y', 'h', 'w', 'medpixel','pvalue'])
-    for i in range(len(maxpixel)):
-        perc = maxpixel[i]
-        result = obj.extract(MP, i, perc, bgleft_up, bgright_up, bgleft_down, bgright_down)
+    for mp in maxpixel:
+        result = obj.extract(mp, bgleft, bgright)
         result_table = result_table.append(result)
-#    for mp in maxpixel:
-#        result = obj.extract(mp, bgleft, bgright)
-#        result_table = result_table.append(result)
 
     result_table = getStripe.getStripe.RemoveRedundant(obj,df=result_table,by='pvalue')
 
     print('##########################\nStripiness calculation ...\n##########################\n')
-    s = obj.scoringstripes(result_table, EV, mask)
-    s = s[0]
+    s = obj.scoringstripes(result_table)
     result_table = result_table.drop(columns=['total', 'num', 'start', 'end', 'x', 'y', 'h', 'w', 'medpixel'])
     result_table.insert(result_table.shape[1],'Stripiness',s,True)
     res_filter = result_table[result_table['pvalue'] < pcut]
     res_filter = res_filter.sort_values(by=['Stripiness'], ascending=False)
 
-
     res1 = out + 'result_unfiltered.txt'
     res2 = out + 'result_filtered.txt'
 
     result_table.to_csv(res1,sep="\t",header=True,index=False)
     res_filter.to_csv(res2,sep="\t",header=True,index=False)
 
     print('\n'+str(round((time.time()-t_start)/60,3))+'min taken.')
     print('Check the result stored in %s' % (out))
     return 0
 
 #if __name__ == "__main__":
 #    main()
-
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/setup.py` & `stripenn-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name = 'stripenn',
-    version = '1.1.5',
+    version = '1.1.7',
     author = 'Sora Yoon',
     author_email = 'sora.yoon@pennmedicine.upenn.edu',
     description = "Image-processing based detection of architectural stripes from chromatic conformation data",
     long_description=README,
     long_description_content_type="text/markdown",
     url = 'https://github.com/ysora/stripenn',
     #package_dir={'': 'src'},
```

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/getStripe.py` & `stripenn-1.1.7/stripenn/getStripe.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/score.py` & `stripenn-1.1.7/stripenn/score.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/seeimage.py` & `stripenn-1.1.7/tests/stripenn/seeimage.py`

 * *Files identical despite different names*

### Comparing `stripenn-1.1.65.9/stripenn.egg-info/build/lib/tests/stripenn/stripenn.py` & `stripenn-1.1.7/tests/stripenn/stripenn.py`

 * *Files identical despite different names*

