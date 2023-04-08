# Comparing `tmp/lazr.config-2.2.3.tar.gz` & `tmp/lazr.config-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lazr.config-2.2.3.tar", last modified: Tue Jan 26 09:50:23 2021, max compression
+gzip compressed data, was "lazr.config-3.0.tar", last modified: Sat Apr  8 17:11:59 2023, max compression
```

## Comparing `lazr.config-2.2.3.tar` & `lazr.config-3.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.852736 lazr.config-2.2.3/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     7637 2015-01-04 16:09:20.000000 lazr.config-2.2.3/COPYING.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1463 2015-01-04 16:09:20.000000 lazr.config-2.2.3/HACKING.rst
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      102 2017-10-19 09:33:59.000000 lazr.config-2.2.3/MANIFEST.in
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     3186 2021-01-26 09:50:16.000000 lazr.config-2.2.3/NEWS.rst
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1517 2021-01-26 09:50:23.852736 lazr.config-2.2.3/PKG-INFO
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      254 2019-11-02 23:50:14.000000 lazr.config-2.2.3/README.rst
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     8532 2017-10-19 09:33:59.000000 lazr.config-2.2.3/conf.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      253 2021-01-26 09:50:23.852736 lazr.config-2.2.3/setup.cfg
--rwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)     2643 2019-11-04 17:06:07.000000 lazr.config-2.2.3/setup.py
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.844736 lazr.config-2.2.3/src/
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.844736 lazr.config-2.2.3/src/lazr/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      905 2015-08-27 00:22:47.000000 lazr.config-2.2.3/src/lazr/__init__.py
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.848736 lazr.config-2.2.3/src/lazr/config/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1032 2017-10-19 09:33:59.000000 lazr.config-2.2.3/src/lazr/config/__init__.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)    31075 2021-01-26 09:49:13.000000 lazr.config-2.2.3/src/lazr/config/_config.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       22 2021-01-26 09:50:08.000000 lazr.config-2.2.3/src/lazr/config/_version.py
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.848736 lazr.config-2.2.3/src/lazr/config/docs/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        0 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/docs/__init__.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1248 2015-08-27 00:22:47.000000 lazr.config-2.2.3/src/lazr/config/docs/fixture.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)    39092 2019-11-04 17:06:07.000000 lazr.config-2.2.3/src/lazr/config/docs/usage.rst
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      930 2015-08-27 00:22:47.000000 lazr.config-2.2.3/src/lazr/config/docs/usage_fixture.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     8678 2015-08-27 00:22:47.000000 lazr.config-2.2.3/src/lazr/config/interfaces.py
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.848736 lazr.config-2.2.3/src/lazr/config/tests/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        0 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/__init__.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     8453 2021-01-26 09:48:17.000000 lazr.config-2.2.3/src/lazr/config/tests/test_config.py
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.852736 lazr.config-2.2.3/src/lazr/config/tests/testdata/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        0 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/__init__.py
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       70 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-invalid-name-chars.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       79 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-invalid-name.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       56 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-nonascii.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       63 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-redefined-key.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      104 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-redefined-section.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       50 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/bad-sectionless.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      813 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/base.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      160 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/local.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       86 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/master-local.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      121 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/master.conf
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      124 2015-01-04 16:09:20.000000 lazr.config-2.2.3/src/lazr/config/tests/testdata/shared.conf
-drwxr-xr-x   0 cjwatson  (1000) cjwatson  (1000)        0 2021-01-26 09:50:23.848736 lazr.config-2.2.3/src/lazr.config.egg-info/
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1517 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/PKG-INFO
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)     1295 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/SOURCES.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        1 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/dependency_links.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        5 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/namespace_packages.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        1 2017-10-20 00:51:51.000000 lazr.config-2.2.3/src/lazr.config.egg-info/not-zip-safe
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)       41 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/requires.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)        5 2021-01-26 09:50:23.000000 lazr.config-2.2.3/src/lazr.config.egg-info/top_level.txt
--rw-r--r--   0 cjwatson  (1000) cjwatson  (1000)      159 2019-11-04 17:06:07.000000 lazr.config-2.2.3/tox.ini
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.140464 lazr.config-3.0/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      955 2023-04-08 16:39:40.000000 lazr.config-3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     5174 2022-04-21 14:28:37.000000 lazr.config-3.0/.woke.yaml
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1502 2021-11-09 15:34:08.000000 lazr.config-3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     7637 2021-11-05 11:54:41.000000 lazr.config-3.0/COPYING.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      117 2023-04-08 16:43:14.000000 lazr.config-3.0/MANIFEST.in
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     3545 2023-04-08 16:42:20.000000 lazr.config-3.0/NEWS.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1692 2023-04-08 17:11:59.140464 lazr.config-3.0/PKG-INFO
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       69 2021-11-05 13:00:38.000000 lazr.config-3.0/README.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       56 2023-04-08 16:39:40.000000 lazr.config-3.0/pyproject.toml
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      145 2023-04-08 17:11:59.140464 lazr.config-3.0/setup.cfg
+-rwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)     2972 2023-04-08 16:42:39.000000 lazr.config-3.0/setup.py
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.132465 lazr.config-3.0/src/
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.136464 lazr.config-3.0/src/lazr/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      905 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/__init__.py
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.136464 lazr.config-3.0/src/lazr/config/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1072 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/__init__.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)    31122 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/_config.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       20 2023-04-08 16:45:58.000000 lazr.config-3.0/src/lazr/config/_version.py
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.136464 lazr.config-3.0/src/lazr/config/docs/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       42 2022-04-21 14:28:37.000000 lazr.config-3.0/src/lazr/config/docs/CONTRIBUTING.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       34 2022-04-21 14:28:37.000000 lazr.config-3.0/src/lazr/config/docs/NEWS.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        0 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/docs/__init__.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     7699 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/docs/conf.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)    39141 2021-11-05 13:00:38.000000 lazr.config-3.0/src/lazr/config/docs/index.rst
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     8520 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/interfaces.py
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.136464 lazr.config-3.0/src/lazr/config/tests/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        0 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/__init__.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     8494 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/tests/test_config.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1714 2023-04-08 16:39:40.000000 lazr.config-3.0/src/lazr/config/tests/test_docs.py
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.140464 lazr.config-3.0/src/lazr/config/tests/testdata/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        0 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/__init__.py
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       70 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-invalid-name-chars.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       79 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-invalid-name.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       55 2021-11-05 12:58:45.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-nonascii.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       62 2021-11-05 12:58:45.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-redefined-key.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      103 2021-11-05 12:58:45.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-redefined-section.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       50 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/bad-sectionless.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      813 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/base.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      160 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/local.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       86 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/master-local.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      121 2021-11-05 11:54:41.000000 lazr.config-3.0/src/lazr/config/tests/testdata/master.conf
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)      123 2021-11-05 12:58:45.000000 lazr.config-3.0/src/lazr/config/tests/testdata/shared.conf
+drwxrwxr-x   0 jugmac00  (1001) jugmac00  (1001)        0 2023-04-08 17:11:59.136464 lazr.config-3.0/src/lazr.config.egg-info/
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1692 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/PKG-INFO
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1404 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/SOURCES.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        1 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/dependency_links.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        5 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        1 2021-11-05 11:58:52.000000 lazr.config-3.0/src/lazr.config.egg-info/not-zip-safe
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)       56 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/requires.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)        5 2023-04-08 17:11:59.000000 lazr.config-3.0/src/lazr.config.egg-info/top_level.txt
+-rw-rw-r--   0 jugmac00  (1001) jugmac00  (1001)     1124 2023-04-08 16:42:55.000000 lazr.config-3.0/tox.ini
```

### Comparing `lazr.config-2.2.3/COPYING.txt` & `lazr.config-3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `lazr.config-2.2.3/HACKING.rst` & `lazr.config-3.0/CONTRIBUTING.rst`

 * *Files 23% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     https://launchpad.net/~lazr-developers
 
 or send a message to:
 
     lazr-developers@lists.launchpad.net
 
 
-Running the tests
-=================
-
-The tests suite requires tox_ and nose_ and is compatible with both Python 2
-and Python 3.  To run the full test suite::
-
-    $ tox
-
-.. _nose: https://nose.readthedocs.org/en/latest/
-.. _tox: https://testrun.org/tox/latest/
+============
+Contributing
+============
+
+To run this project's tests, use `tox <https://tox.readthedocs.io/en/latest/>`_.
+
+To update the `project's documentation
+<https://lazrconfig.readthedocs.io/en/latest/>`_ you need to trigger a manual
+build on the project's dashboard on https://readthedocs.org.
```

### Comparing `lazr.config-2.2.3/NEWS.rst` & `lazr.config-3.0/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 ====================
 NEWS for lazr.config
 ====================
 
+3.0 (2023-04-08)
+================
+- Add basic pre-commit configuration.
+- Publish Documentation on Read the Docs.
+- Apply inclusive naming via the woke pre-commit hook.
+- Test using ``zope.testrunner`` rather than ``nose``.
+- Officially add support for Python 3.9, 3.10 and 3.11.
+- Drop support for Python 2.6, 2.7, and 3.4.
+- Apply ``black`` and ``isort``.
+
 2.2.3 (2021-01-26)
 ==================
 - Fix tests with zope.interface >= 5.0.0.
 - Fix deprecation warning on Python >= 3.2.  (LP: #1870199)
 
 2.2.2 (2019-11-04)
 ==================
```

### Comparing `lazr.config-2.2.3/PKG-INFO` & `lazr.config-3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: lazr.config
-Version: 2.2.3
+Version: 3.0
 Summary: Create configuration schemas, and process and validate configurations.
 Home-page: https://launchpad.net/lazr.config
+Download-URL: https://launchpad.net/lazr.config/+download
 Maintainer: LAZR Developers
 Maintainer-email: lazr-developers@lists.launchpad.net
 License: LGPL v3
-Download-URL: https://launchpad.net/lazr.config/+download
-Description: 
-        The LAZR config system is typically used to manage process configuration.
-        Process configuration is for saying how things change when we run systems on
-        different machines, or under different circumstances.
-        
-        This system uses ini-like file format of section, keys, and values.  The
-        config file supports inheritance to minimize duplication of information across
-        files. The format supports schema validation.
-        
-Platform: UNKNOWN
+Project-URL: Source, https://code.launchpad.net/lazr.config
+Project-URL: Issue Tracker, https://bugs.launchpad.net/lazr.config
+Project-URL: Documentation, https://lazrconfig.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.5
+Provides-Extra: docs
+License-File: COPYING.txt
+
+
+The LAZR config system is typically used to manage process configuration.
+Process configuration is for saying how things change when we run systems on
+different machines, or under different circumstances.
+
+This system uses ini-like file format of section, keys, and values.  The
+config file supports inheritance to minimize duplication of information across
+files. The format supports schema validation.
```

### Comparing `lazr.config-2.2.3/conf.py` & `lazr.config-3.0/src/lazr/config/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,268 +1,239 @@
-# -*- coding: utf-8 -*-
-#
 # lazr.config documentation build configuration file, created by
 # sphinx-quickstart on Mon Jan  7 10:37:37 2013.
 #
-# This file is execfile()d with the current directory set to its containing dir.
+# This file is execfile()d with the current directory set to its containing
+# dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-from __future__ import print_function
-import sys, os
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
-# -- General configuration -----------------------------------------------------
+# -- General configuration ----------------------------------------------------
+
+from lazr.config import __version__
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
-# Add any Sphinx extension module names here, as strings. They can be extensions
-# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'README'
+master_doc = "index"
 
 # General information about the project.
-project = u'lazr.config'
-copyright = u'2013-2015, LAZR developers'
+project = "lazr.config"
+copyright = "2013-2021, LAZR developers"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-with open('src/lazr/config/_version.py') as version_file:
-    exec(version_file.read())  # sets __version__
 version = __version__
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build', 'eggs']
+exclude_patterns = ["_build", "eggs"]
 
-# The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# The reST default role (used for this markup: `text`) to use for all
+# documents.
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
-# -- Options for HTML output ---------------------------------------------------
+# -- Options for HTML output --------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+
+# This is required for the alabaster theme
+# refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
+html_sidebars = {
+    "**": [
+        "globaltoc.html",
+        "relations.html",  # needs 'show_related': True theme option to display
+        "searchbox.html",
+    ]
+}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'lazrconfigdoc'
+htmlhelp_basename = "lazrconfigdoc"
 
 
-# -- Options for LaTeX output --------------------------------------------------
+# -- Options for LaTeX output -------------------------------------------------
 
-latex_elements = {
+# latex_elements = {
 # The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
+# 'papersize': 'letterpaper',
 
 # The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
+# 'pointsize': '10pt',
 
 # Additional stuff for the LaTeX preamble.
-#'preamble': '',
-}
+# 'preamble': '',
+# }
 
 # Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [
-  ('index', 'lazrconfig.tex', u'lazr.config Documentation',
-   u'LAZR developers', 'manual'),
-]
+# (source start file, target name, title, author, documentclass
+# [howto/manual]).
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
-# -- Options for manual page output --------------------------------------------
+# -- Options for manual page output -------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'lazrconfig', u'lazr.config Documentation',
-     [u'LAZR developers'], 1)
-]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
-# -- Options for Texinfo output ------------------------------------------------
+# -- Options for Texinfo output -----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
-texinfo_documents = [
-  ('index', 'lazrconfig', u'lazr.config Documentation',
-   u'LAZR developers', 'lazrconfig', 'One line description of project.',
-   'Miscellaneous'),
-]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
-
-# Make upload to packages.python.org happy.
-def index_html():
-    import errno
-    cwd = os.getcwd()
-    try:
-        try:
-            os.makedirs('build/sphinx/html')
-        except OSError as error:
-            if error.errno != errno.EEXIST:
-                raise
-        os.chdir('build/sphinx/html')
-        try:
-            os.symlink('README.html', 'index.html')
-            print('index.html -> README.html')
-        except OSError as error:
-            if error.errno != errno.EEXIST:
-                raise
-    finally:
-        os.chdir(cwd)
-
-import atexit
-atexit.register(index_html)
+# texinfo_show_urls = 'footnote'
```

### Comparing `lazr.config-2.2.3/setup.py` & `lazr.config-3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,57 +10,68 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with lazr.config.  If not, see <http://www.gnu.org/licenses/>.
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-with open('src/lazr/config/_version.py') as version_file:
+with open("src/lazr/config/_version.py") as version_file:
     exec(version_file.read())  # sets __version__
 
 setup(
-    name='lazr.config',
-    version=__version__,
-    namespace_packages=['lazr'],
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
+    name="lazr.config",
+    version=__version__,  # noqa: F821
+    namespace_packages=["lazr"],
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    maintainer='LAZR Developers',
-    maintainer_email='lazr-developers@lists.launchpad.net',
-    description=('Create configuration schemas, and process and '
-                 'validate configurations.'),
+    maintainer="LAZR Developers",
+    maintainer_email="lazr-developers@lists.launchpad.net",
+    description=(
+        "Create configuration schemas, and process and "
+        "validate configurations."
+    ),
     long_description="""
 The LAZR config system is typically used to manage process configuration.
 Process configuration is for saying how things change when we run systems on
 different machines, or under different circumstances.
 
 This system uses ini-like file format of section, keys, and values.  The
 config file supports inheritance to minimize duplication of information across
 files. The format supports schema validation.
 """,
-    license='LGPL v3',
+    license="LGPL v3",
     install_requires=[
-        'setuptools',
-        'zope.interface',
-        'lazr.delegates',
-        ],
-    url='https://launchpad.net/lazr.config',
-    download_url='https://launchpad.net/lazr.config/+download',
+        "setuptools",
+        "zope.interface",
+        "lazr.delegates",
+    ],
+    url="https://launchpad.net/lazr.config",
+    project_urls={
+        "Source": "https://code.launchpad.net/lazr.config",
+        "Issue Tracker": "https://bugs.launchpad.net/lazr.config",
+        "Documentation": "https://lazrconfig.readthedocs.io/en/latest/",
+    },
+    download_url="https://launchpad.net/lazr.config/+download",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
+        "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",  # noqa
         "Operating System :: OS Independent",
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        ],
-    )
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    extras_require=dict(
+        docs=["Sphinx"],
+    ),
+    python_requires=">=3.5",
+)
```

### Comparing `lazr.config-2.2.3/src/lazr/__init__.py` & `lazr.config-3.0/src/lazr/__init__.py`

 * *Files identical despite different names*

### Comparing `lazr.config-2.2.3/src/lazr/config/__init__.py` & `lazr.config-3.0/src/lazr/config/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with lazr.config.  If not, see <http://www.gnu.org/licenses/>.
 
 """A configuration file system."""
 
-from lazr.config._version import __version__
-__version__
-
 # While we generally frown on "*" imports, this, combined with the fact we
 # only test code from this module, means that we can verify what has been
 # exported.
-from lazr.config._config import *
-from lazr.config._config import __all__
+from lazr.config._config import *  # noqa: F401, F403
+from lazr.config._config import __all__  # noqa: F401, F402
+from lazr.config._version import __version__
+
+__version__
```

### Comparing `lazr.config-2.2.3/src/lazr/config/_config.py` & `lazr.config-3.0/src/lazr/config/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,74 +12,81 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with lazr.config.  If not, see <http://www.gnu.org/licenses/>.
 
 """Implementation classes for config."""
 
-from __future__ import absolute_import, print_function, unicode_literals
-
-__metaclass__ = type
 __all__ = [
-    'Config',
-    'ConfigData',
-    'ConfigSchema',
-    'ImplicitTypeSchema',
-    'ImplicitTypeSection',
-    'Section',
-    'SectionSchema',
-    'as_boolean',
-    'as_host_port',
-    'as_log_level',
-    'as_timedelta',
-    'as_username_groupname',
-    ]
+    "Config",
+    "ConfigData",
+    "ConfigSchema",
+    "ImplicitTypeSchema",
+    "ImplicitTypeSection",
+    "Section",
+    "SectionSchema",
+    "as_boolean",
+    "as_host_port",
+    "as_log_level",
+    "as_timedelta",
+    "as_username_groupname",
+]
 
 
 import datetime
 import grp
 import logging
 import os
 import pwd
 import re
-import sys
-
 from os.path import abspath, basename, dirname
 from textwrap import dedent
 
 try:
-    from io import StringIO
     from configparser import NoSectionError, RawConfigParser
+    from io import StringIO
 
     def _parser_read_file(parser, f, source=None):
         parser.read_file(f, source)
+
 except ImportError:
     # Python 2.
-    from StringIO import StringIO
     from ConfigParser import NoSectionError, RawConfigParser
+    from StringIO import StringIO
 
     def _parser_read_file(parser, f, source=None):
         parser.readfp(f, source)
 
 
 from zope.interface import implementer
 
 from lazr.config.interfaces import (
-    ConfigErrors, ICategory, IConfigData, IConfigLoader, IConfigSchema,
-    InvalidSectionNameError, ISection, ISectionSchema, IStackableConfig,
-    NoCategoryError, NoConfigError, RedefinedSectionError, UnknownKeyError,
-    UnknownSectionError)
+    ConfigErrors,
+    ICategory,
+    IConfigData,
+    IConfigLoader,
+    IConfigSchema,
+    InvalidSectionNameError,
+    ISection,
+    ISectionSchema,
+    IStackableConfig,
+    NoCategoryError,
+    NoConfigError,
+    RedefinedSectionError,
+    UnknownKeyError,
+    UnknownSectionError,
+)
 from lazr.delegates import delegate_to
 
 _missing = object()
 
 
 def read_content(filename):
     """Return the content of a file at filename as a string."""
-    with open(filename, 'rt') as fp:
+    with open(filename) as fp:
         return fp.read()
 
 
 @implementer(ISectionSchema)
 class SectionSchema:
     """See `ISectionSchema`."""
 
@@ -96,66 +103,65 @@
         self.name = name
         self._options = options
         self.optional = is_optional
         self.master = is_master
 
     def __iter__(self):
         """See `ISectionSchema`"""
-        for key in self._options.keys():
-            yield key
+        yield from self._options.keys()
 
     def __contains__(self, name):
         """See `ISectionSchema`"""
         return name in self._options
 
     def __getitem__(self, key):
         """See `ISectionSchema`"""
         return self._options[key]
 
     @property
     def category_and_section_names(self):
         """See `ISectionSchema`."""
-        if '.' in self.name:
-            return tuple(self.name.split('.'))
+        if "." in self.name:
+            return tuple(self.name.split("."))
         else:
             return (None, self.name)
 
     def clone(self):
         """Return a copy of this section schema."""
-        return self.__class__(self.name, self._options.copy(),
-                              self.optional, self.master)
+        return self.__class__(
+            self.name, self._options.copy(), self.optional, self.master
+        )
 
 
-@delegate_to(ISectionSchema, context='schema')
+@delegate_to(ISectionSchema, context="schema")
 @implementer(ISection)
 class Section:
     """See `ISection`."""
 
     def __init__(self, schema, _options=None):
         """Create an `ISection` from schema.
 
         :param schema: The ISectionSchema that defines this ISection.
         """
         # Use __dict__ because __getattr__ limits access to self.options.
-        self.__dict__['schema'] = schema
+        self.__dict__["schema"] = schema
         if _options is None:
-            _options = dict((key, schema[key]) for key in schema)
-        self.__dict__['_options'] = _options
+            _options = {key: schema[key] for key in schema}
+        self.__dict__["_options"] = _options
 
     def __getitem__(self, key):
         """See `ISection`"""
         return self._options[key]
 
     def __getattr__(self, name):
         """See `ISection`."""
         if name in self._options:
             return self._options[name]
         else:
-            raise AttributeError(
-                "No section key named %s." % name)
+            raise AttributeError("No section key named %s." % name)
 
     def __setattr__(self, name, value):
         """Callsites cannot mutate the config by direct manipulation."""
         raise AttributeError("Config options cannot be set directly.")
 
     @property
     def category_and_section_names(self):
@@ -169,15 +175,15 @@
             the key. An empty list is returned if there are no errors.
         """
         errors = []
         for key, value in items:
             if key in self._options:
                 self._options[key] = value
             else:
-                msg = "%s does not have a %s key." % (self.name, key)
+                msg = "{} does not have a {} key.".format(self.name, key)
                 errors.append(UnknownKeyError(msg))
         return errors
 
     def clone(self):
         """Return a copy of this section.
 
         The extension mechanism requires a copy of a section to prevent
@@ -189,52 +195,56 @@
 class ImplicitTypeSection(Section):
     """See `ISection`.
 
     ImplicitTypeSection supports implicit conversion of key values to
     simple datatypes. It accepts the same section data as Section; the
     datatype information is not embedded in the schema or the config file.
     """
-    re_types = re.compile(r'''
+
+    re_types = re.compile(
+        r"""
         (?P<false> ^false$) |
         (?P<true> ^true$) |
         (?P<none> ^none$) |
         (?P<int> ^[+-]?\d+$) |
         (?P<str> ^.*)
-        ''', re.IGNORECASE | re.VERBOSE)
+        """,
+        re.IGNORECASE | re.VERBOSE,
+    )
 
     def _convert(self, value):
         """Return the value as the datatype the str appears to be.
 
         Conversion rules:
         * bool: a single word, 'true' or 'false', case insensitive.
         * int: a single word that is a number. Signed is supported,
             hex and octal numbers are not.
         * str: anything else.
         """
         match = self.re_types.match(value)
-        if match.group('false'):
+        if match.group("false"):
             return False
-        elif match.group('true'):
+        elif match.group("true"):
             return True
-        elif match.group('none'):
+        elif match.group("none"):
             return None
-        elif match.group('int'):
+        elif match.group("int"):
             return int(value)
         else:
             # match.group('str'); just return the sripped value.
             return value.strip()
 
     def __getitem__(self, key):
         """See `ISection`."""
-        value = super(ImplicitTypeSection, self).__getitem__(key)
+        value = super().__getitem__(key)
         return self._convert(value)
 
     def __getattr__(self, name):
         """See `ISection`."""
-        value = super(ImplicitTypeSection, self).__getattr__(name)
+        value = super().__getattr__(name)
         return self._convert(value)
 
 
 @implementer(IConfigSchema, IConfigLoader)
 class ConfigSchema:
     """See `IConfigSchema`."""
 
@@ -274,65 +284,74 @@
         """Return the contents of the schema at filename as a StringIO.
 
         This method verifies that the file is ascii encoded and that no
         section name is redefined.
         """
         raw_schema = read_content(filename)
         # Verify that the string is ascii.
-        raw_schema.encode('ascii', 'strict')
+        raw_schema.encode("ascii", "strict")
         # Verify that no sections are redefined.
         section_names = []
-        for section_name in re.findall(r'^\s*\[[^\]]+\]', raw_schema, re.M):
+        for section_name in re.findall(r"^\s*\[[^\]]+\]", raw_schema, re.M):
             if section_name in section_names:
                 raise RedefinedSectionError(section_name)
             else:
                 section_names.append(section_name)
         return StringIO(raw_schema)
 
     def _setSectionSchemasAndCategoryNames(self, parser):
         """Set the SectionSchemas and category_names from the config."""
         category_names = set()
         templates = {}
         # Retrieve all the templates first because section() does not follow
         # the order of the conf file.
         for name in parser.sections():
-            (section_name, category_name,
-             is_template, is_optional,
-             is_master) = self._parseSectionName(name)
+            (
+                section_name,
+                category_name,
+                is_template,
+                is_optional,
+                is_master,
+            ) = self._parseSectionName(name)
             if is_template or is_master:
                 templates[category_name] = dict(parser.items(name))
         for name in parser.sections():
-            (section_name, category_name,
-             is_template, is_optional,
-             is_master) = self._parseSectionName(name)
+            (
+                section_name,
+                category_name,
+                is_template,
+                is_optional,
+                is_master,
+            ) = self._parseSectionName(name)
             if is_template:
                 continue
             options = dict(templates.get(category_name, {}))
             options.update(parser.items(name))
             self._section_schemas[section_name] = SectionSchema(
-                section_name, options, is_optional, is_master)
+                section_name, options, is_optional, is_master
+            )
             if category_name is not None:
                 category_names.add(category_name)
         self._category_names = sorted(category_names)
 
-    _section_name_pattern = re.compile(r'\w[\w.-]+\w')
+    _section_name_pattern = re.compile(r"\w[\w.-]+\w")
 
     def _parseSectionName(self, name):
         """Return a tuple of names and kinds embedded in the name.
 
         :return: (section_name, category_name, is_template, is_optional).
             section_name is always a string. category_name is a string or
             None if there is no prefix. is_template and is_optional
             are False by default, but will be true if the name's suffix
             ends in '.template' or '.optional'.
         """
-        name_parts = name.split('.')
-        is_template = name_parts[-1] == 'template'
-        is_optional = name_parts[-1] == 'optional'
-        is_master = name_parts[-1] == 'master'
+        name_parts = name.split(".")
+        is_template = name_parts[-1] == "template"
+        is_optional = name_parts[-1] == "optional"
+        is_master = name_parts[-1] == "master"
         if is_template or is_optional:
             # The suffix is not a part of the section name.
             # Example: [name.optional] or [category.template]
             del name_parts[-1]
         count = len(name_parts)
         if count == 1 and is_template:
             # Example: [category.template]
@@ -341,37 +360,42 @@
         elif count == 1:
             # Example: [name]
             category_name = None
             section_name = name_parts[0]
         elif count == 2:
             # Example: [category.name]
             category_name = name_parts[0]
-            section_name = '.'.join(name_parts)
+            section_name = ".".join(name_parts)
         else:
-            raise InvalidSectionNameError('[%s] has too many parts.' % name)
+            raise InvalidSectionNameError("[%s] has too many parts." % name)
         if self._section_name_pattern.match(section_name) is None:
             raise InvalidSectionNameError(
-                '[%s] name does not match [\w.-]+.' % name)
-        return (section_name, category_name,
-                is_template, is_optional, is_master)
+                r"[%s] name does not match [\w.-]+." % name
+            )
+        return (
+            section_name,
+            category_name,
+            is_template,
+            is_optional,
+            is_master,
+        )
 
     @property
     def section_factory(self):
         """See `IConfigSchema`."""
         return self._section_factory
 
     @property
     def category_names(self):
         """See `IConfigSchema`."""
         return self._category_names
 
     def __iter__(self):
         """See `IConfigSchema`."""
-        for value in self._section_schemas.values():
-            yield value
+        yield from self._section_schemas.values()
 
     def __contains__(self, name):
         """See `IConfigSchema`."""
         return name in self._section_schemas.keys()
 
     def __getitem__(self, name):
         """See `IConfigSchema`."""
@@ -385,41 +409,43 @@
         if name not in self.category_names:
             if default is _missing:
                 raise NoCategoryError(name)
             return default
         section_schemas = []
         for key in self._section_schemas:
             section = self._section_schemas[key]
-            category, dummy = section.category_and_section_names
+            category, _ = section.category_and_section_names
             if name == category:
                 section_schemas.append(section)
         return section_schemas
 
     def _getRequiredSections(self):
         """return a dict of `Section`s from the required `SectionSchemas`."""
         sections = {}
         for section_schema in self:
             if not section_schema.optional:
                 sections[section_schema.name] = self.section_factory(
-                    section_schema)
+                    section_schema
+                )
         return sections
 
     def load(self, filename):
         """See `IConfigLoader`."""
         conf_data = read_content(filename)
         return self._load(filename, conf_data)
 
     def loadFile(self, source_file, filename=None):
         """See `IConfigLoader`."""
         conf_data = source_file.read()
         if filename is None:
-            filename = getattr(source_file, 'name')
+            filename = getattr(source_file, "name")
             assert filename is not None, (
-                'filename must be provided if the file-like object '
-                'does not have a name attribute.')
+                "filename must be provided if the file-like object "
+                "does not have a name attribute."
+            )
         return self._load(filename, conf_data)
 
     def _load(self, filename, conf_data):
         """Return a Config parsed from conf_data."""
         config = Config(self)
         config.push(filename, conf_data)
         return config
@@ -452,28 +478,27 @@
             self._errors = errors
 
     def _getCategoryNames(self):
         """Return a tuple of category names that the `Section`s belong to."""
         category_names = set()
         for section_name in self._sections:
             section = self._sections[section_name]
-            category, dummy = section.category_and_section_names
+            category, _ = section.category_and_section_names
             if category is not None:
                 category_names.add(category)
         return tuple(category_names)
 
     @property
     def category_names(self):
         """See `IConfigData`."""
         return self._category_names
 
     def __iter__(self):
         """See `IConfigData`."""
-        for value in self._sections.values():
-            yield value
+        yield from self._sections.values()
 
     def __contains__(self, name):
         """See `IConfigData`."""
         return name in self._sections.keys()
 
     def __getitem__(self, name):
         """See `IConfigData`."""
@@ -487,31 +512,33 @@
         if name not in self.category_names:
             if default is _missing:
                 raise NoCategoryError(name)
             return default
         sections = []
         for key in self._sections:
             section = self._sections[key]
-            category, dummy = section.category_and_section_names
+            category, _ = section.category_and_section_names
             if name == category:
                 sections.append(section)
         return sections
 
 
-@delegate_to(IConfigData, context='data')
+@delegate_to(IConfigData, context="data")
 @implementer(IStackableConfig)
 class Config:
     """See `IStackableConfig`."""
+
     # LAZR config classes may access ConfigData private data.
     # pylint: disable-msg=W0212
 
     def __init__(self, schema):
         """Set the schema and configuration."""
         self._overlays = (
-            ConfigData(schema.filename, schema._getRequiredSections()), )
+            ConfigData(schema.filename, schema._getRequiredSections()),
+        )
         self.schema = schema
 
     def __getattr__(self, name):
         """See `IStackableConfig`."""
         if name in self.data._sections:
             return self.data._sections[name]
         elif name in self.data._category_names:
@@ -555,16 +582,17 @@
         confs = self._getExtendedConfs(conf_name, conf_data)
         confs.reverse()
         for conf_name, parser, encoding_errors in confs:
             if self.data.filename == self.schema.filename == conf_name:
                 # Do not parse the schema file twice in a row.
                 continue
             config_data = self._createConfigData(
-                conf_name, parser, encoding_errors)
-            self._overlays = (config_data, ) + self._overlays
+                conf_name, parser, encoding_errors
+            )
+            self._overlays = (config_data,) + self._overlays
 
     def _getExtendedConfs(self, conf_filename, conf_data, confs=None):
         """Return a list of tuple (conf_name, parser, encoding_errors).
 
         :param conf_filename: The path and name of the conf file.
         :param conf_data: Unparsed config data.
         :param confs: A list of confs that extend filename.
@@ -579,24 +607,21 @@
         if confs is None:
             confs = []
         encoding_errors = self._verifyEncoding(conf_data)
         # LP: #1397779.  In Python 3, RawConfigParser grew a `strict` keyword
         # option and in Python 3.2, this argument changed its default from
         # False to True.  This breaks behavior compatibility with Python 2, so
         # under Python 3, always force strict=False.
-        kws = {}
-        if sys.version_info >= (3,):
-            kws['strict'] = False
-        parser = RawConfigParser(**kws)
+        parser = RawConfigParser(strict=False)
         _parser_read_file(parser, StringIO(conf_data), conf_filename)
         confs.append((conf_filename, parser, encoding_errors))
-        if parser.has_option('meta', 'extends'):
+        if parser.has_option("meta", "extends"):
             base_path = dirname(conf_filename)
-            extends_name = parser.get('meta', 'extends')
-            extends_filename = abspath('%s/%s' % (base_path, extends_name))
+            extends_name = parser.get("meta", "extends")
+            extends_filename = abspath("{}/{}".format(base_path, extends_name))
             extends_data = read_content(extends_filename)
             self._getExtendedConfs(extends_filename, extends_data, confs)
         return confs
 
     def _createConfigData(self, conf_name, parser, encoding_errors):
         """Return a new ConfigData object created from a parsed conf file.
 
@@ -614,58 +639,65 @@
         for section in self.data:
             sections[section.name] = section.clone()
         errors = list(self.data._errors)
         errors.extend(encoding_errors)
         extends = None
         masters = set()
         for section_name in parser.sections():
-            if section_name == 'meta':
+            if section_name == "meta":
                 extends, meta_errors = self._loadMetaData(parser)
                 errors.extend(meta_errors)
                 continue
-            if (section_name.endswith('.template') or
-                section_name.endswith('.optional') or
-                section_name.endswith('.master')):
+            if (
+                section_name.endswith(".template")
+                or section_name.endswith(".optional")
+                or section_name.endswith(".master")
+            ):
                 # This section is a schema directive.
                 continue
             # Calculate the section master name.
             # Check for sections which extend .masters.
-            if '.' in section_name:
-                category, section = section_name.split('.')
-                master_name = category + '.master'
+            if "." in section_name:
+                category, section = section_name.split(".")
+                master_name = category + ".master"
             else:
                 master_name = None
-            if (section_name not in self.schema and
-                master_name not in self.schema):
+            if (
+                section_name not in self.schema
+                and master_name not in self.schema
+            ):
                 # Any section not in the the schema is an error.
-                msg = "%s does not have a %s section." % (
-                    self.schema.name, section_name)
+                msg = "{} does not have a {} section.".format(
+                    self.schema.name,
+                    section_name,
+                )
                 errors.append(UnknownSectionError(msg))
                 continue
             if section_name not in self.data:
                 # Is there a master section?
                 try:
                     section_schema = self.schema[master_name]
                 except NoSectionError:
                     # There's no master for this section, so just treat it
                     # like a regular category.
                     pass
                 else:
-                    assert section_schema.master, '.master is not a master?'
+                    assert section_schema.master, ".master is not a master?"
                     schema = section_schema.clone()
                     schema.name = section_name
                     section = self.schema.section_factory(schema)
                     section.update(parser.items(section_name))
                     sections[section_name] = section
                     masters.add(master_name)
                     continue
                 # Create the optional section from the schema.
                 section_schema = self.schema[section_name]
                 sections[section_name] = self.schema.section_factory(
-                    section_schema)
+                    section_schema
+                )
             # Update the section with the parser options.
             items = parser.items(section_name)
             section_errors = sections[section_name].update(items)
             errors.extend(section_errors)
         # master sections are like templates.  They show up in the schema but
         # not in the config.
         for master in masters:
@@ -677,33 +709,33 @@
 
         :return: a list of UnicodeDecodeError errors. If there are no
             errors, return an empty list.
         """
         errors = []
         try:
             if isinstance(config_data, bytes):
-                config_data.decode('ascii', 'strict')
+                config_data.decode("ascii", "strict")
             else:
-                config_data.encode('ascii', 'strict')
+                config_data.encode("ascii", "strict")
         except UnicodeError as error:
             errors.append(error)
         return errors
 
     def _loadMetaData(self, parser):
         """Load the config meta data from the ConfigParser.
 
         The meta section is reserved for the LAZR config parser.
 
         :return: a list of errors if there are errors, or an empty list.
         """
         extends = None
         errors = []
-        for key in parser.options('meta'):
+        for key in parser.options("meta"):
             if key == "extends":
-                extends = parser.get('meta', 'extends')
+                extends = parser.get("meta", "extends")
             else:
                 # Any other key is an error.
                 msg = "The meta section does not have a %s key." % key
                 errors.append(UnknownKeyError(msg))
         return (extends, errors)
 
     def pop(self, conf_name):
@@ -722,15 +754,15 @@
         schema_index = len(self.overlays) - 1
         for index, config_data in enumerate(self.overlays):
             if index == schema_index and config_data.name == conf_name:
                 raise NoConfigError("Cannot pop the schema's default config.")
             if config_data.name == conf_name:
                 return index + 1
         # The config data was not found in the overlays.
-        raise NoConfigError('No config with name: %s.' % conf_name)
+        raise NoConfigError("No config with name: %s." % conf_name)
 
 
 @implementer(ICategory)
 class Category:
     """See `ICategory`."""
 
     def __init__(self, name, sections):
@@ -738,15 +770,15 @@
         self.name = name
         self._sections = {}
         for section in sections:
             self._sections[section.name] = section
 
     def __getattr__(self, name):
         """See `ICategory`."""
-        full_name = "%s.%s" % (self.name, name)
+        full_name = "{}.{}".format(self.name, name)
         if full_name in self._sections:
             return self._sections[full_name]
         raise AttributeError("No section named %s." % name)
 
 
 def as_boolean(value):
     """Turn a string into a boolean.
@@ -756,38 +788,38 @@
         false, no, 0, off, disable, disabled (for False).  Everything else is
         an error.
     :type value: string
     :return: True or False.
     :rtype: boolean
     """
     value = value.lower()
-    if value in ('true', 'yes', '1', 'on', 'enabled', 'enable'):
+    if value in ("true", "yes", "1", "on", "enabled", "enable"):
         return True
-    if value in ('false', 'no', '0', 'off', 'disabled', 'disable'):
+    if value in ("false", "no", "0", "off", "disabled", "disable"):
         return False
-    raise ValueError('Invalid boolean value: %s' % value)
+    raise ValueError("Invalid boolean value: %s" % value)
 
 
-def as_host_port(value, default_host='localhost', default_port=25):
+def as_host_port(value, default_host="localhost", default_port=25):
     """Return a 2-tuple of (host, port) from a value like 'host:port'.
 
     :param value: The configuration value.
     :type value: string
     :param default_host: Optional host name to use if the configuration value
         is missing the host name.
     :type default_host: string
     :param default_port: Optional port number to use if the configuration
         value is missing the port number.
     :type default_port: integer
     :return: a 2-tuple of the form (host, port)
     :rtype: 2-tuple of (string, integer)
     """
-    if ':' in value:
-        host, port = value.split(':')
-        if host == '':
+    if ":" in value:
+        host, port = value.split(":")
+        if host == "":
             host = default_host
         port = int(port)
     else:
         host = value
         port = default_port
     return host, port
 
@@ -798,62 +830,65 @@
     :param value: The configuration value.
     :type value: a string containing exactly one colon, or None
     :return: a 2-tuple of (username, groupname).  If `value` was None, then
         the current user and group names are returned.
     :rtype: 2-tuple of type (string, string)
     """
     if value:
-        user, group = value.split(':', 1)
+        user, group = value.split(":", 1)
     else:
-        user  = pwd.getpwuid(os.getuid()).pw_name
+        user = pwd.getpwuid(os.getuid()).pw_name
         group = grp.getgrgid(os.getgid()).gr_name
     return user, group
 
 
 def _sortkey(item):
     """Return a value that sorted(..., key=_sortkey) can use."""
     order = dict(
-        w=0,    # weeks
-        d=1,    # days
-        h=2,    # hours
-        m=3,    # minutes
-        s=4,    # seconds
-        )
+        w=0,  # weeks
+        d=1,  # days
+        h=2,  # hours
+        m=3,  # minutes
+        s=4,  # seconds
+    )
     return order.get(item[-1])
 
+
 def as_timedelta(value):
     """Convert a value string to the equivalent timedeta."""
     # Technically, the regex will match multiple decimal points in the
     # left-hand side, but that's okay because the float/int conversion below
     # will properly complain if there's more than one dot.
-    components = sorted(re.findall(r'([\d.]+[smhdw])', value), key=_sortkey)
+    components = sorted(re.findall(r"([\d.]+[smhdw])", value), key=_sortkey)
     # Complain if the components are out of order.
-    if ''.join(components) != value:
+    if "".join(components) != value:
         raise ValueError
-    keywords = dict((interval[0].lower(), interval)
-                    for interval in ('weeks', 'days', 'hours',
-                                     'minutes', 'seconds'))
+    keywords = {
+        interval[0].lower(): interval
+        for interval in ("weeks", "days", "hours", "minutes", "seconds")
+    }
     keyword_arguments = {}
     for interval in components:
         if len(interval) == 0:
             raise ValueError
         keyword = keywords.get(interval[-1].lower())
         if keyword is None:
             raise ValueError
         if keyword in keyword_arguments:
             raise ValueError
-        if '.' in interval[:-1]:
+        if "." in interval[:-1]:
             converted = float(interval[:-1])
         else:
             converted = int(interval[:-1])
         keyword_arguments[keyword] = converted
     if len(keyword_arguments) == 0:
         raise ValueError
     return datetime.timedelta(**keyword_arguments)
 
+
 def as_log_level(value):
     """Turn a string into a log level.
 
     :param value: A string with a value (case-insensitive) equal to one of the
         symbolic logging levels.
     :type value: string
     :return: A logging level constant.
```

### Comparing `lazr.config-2.2.3/src/lazr/config/docs/usage.rst` & `lazr.config-3.0/src/lazr/config/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1335,10 +1335,12 @@
 
 Other Documents
 ===============
 
 .. toctree::
    :glob:
 
-   *
+   self
+   Contributing <CONTRIBUTING>
+   News <NEWS>
 
 .. _timedelta: http://docs.python.org/3/library/datetime.html#timedelta-objects
```

### Comparing `lazr.config-2.2.3/src/lazr/config/interfaces.py` & `lazr.config-3.0/src/lazr/config/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,34 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with lazr.config.  If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable-msg=E0211,E0213,W0231
 """Interfaces for process configuration.."""
 
-from __future__ import absolute_import, print_function, unicode_literals
-
-__metaclass__ = type
 __all__ = [
-    'ConfigErrors',
-    'ConfigSchemaError',
-    'IConfigData',
-    'NoConfigError',
-    'ICategory',
-    'IConfigLoader',
-    'IConfigSchema',
-    'InvalidSectionNameError',
-    'ISection',
-    'ISectionSchema',
-    'IStackableConfig',
-    'NoCategoryError',
-    'RedefinedKeyError',
-    'RedefinedSectionError',
-    'UnknownKeyError',
-    'UnknownSectionError']
+    "ConfigErrors",
+    "ConfigSchemaError",
+    "IConfigData",
+    "NoConfigError",
+    "ICategory",
+    "IConfigLoader",
+    "IConfigSchema",
+    "InvalidSectionNameError",
+    "ISection",
+    "ISectionSchema",
+    "IStackableConfig",
+    "NoCategoryError",
+    "RedefinedKeyError",
+    "RedefinedSectionError",
+    "UnknownKeyError",
+    "UnknownSectionError",
+]
 
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute, Interface
 
 
 class ConfigSchemaError(Exception):
     """A base class of all `IConfigSchema` errors."""
 
 
 class RedefinedKeyError(ConfigSchemaError):
@@ -64,43 +62,46 @@
 class UnknownSectionError(ConfigSchemaError):
     """The config has a section that is not in the schema."""
 
 
 class UnknownKeyError(ConfigSchemaError):
     """The section has a key that is not in the schema."""
 
+
 class NoConfigError(ConfigSchemaError):
     """No config has the name."""
 
+
 class ConfigErrors(ConfigSchemaError):
     """The errors in a Config.
 
     The list of errors can be accessed via the errors attribute.
     """
 
     def __init__(self, message, errors=None):
         """Initialize the error with a message and errors.
 
         :param message: a message string
         :param errors: a list of errors in the config, or None
         """
-        # Without the suppression above, this produces a warning in Python 2.6.
         self.message = message
         self.errors = errors
 
     def __str__(self):
-        return '%s: %s' % (self.__class__.__name__, self.message)
+        return "{}: {}".format(self.__class__.__name__, self.message)
 
 
 class ISectionSchema(Interface):
     """Defines the valid keys and default values for a configuration group."""
+
     name = Attribute("The section name.")
     optional = Attribute("Is the section optional in the config?")
     category_and_section_names = Attribute(
-        "A 2-Tuple of the category and specific name parts.")
+        "A 2-Tuple of the category and specific name parts."
+    )
 
     def __iter__():
         """Iterate over the keys."""
 
     def __contains__(name):
         """Return True or False if name is a key."""
 
@@ -109,24 +110,26 @@
 
         :raise `KeyError`: if the key does not exist.
         """
 
 
 class ISection(ISectionSchema):
     """Defines the values for a configuration group."""
+
     schema = Attribute("The ISectionSchema that defines this ISection.")
 
     def __getattr__(name):
         """Return the named key.
 
         :name: a key name.
         :return: the value of the matching key.
         :raise: AttributeError if there is no key with the name.
         """
 
+
 class IConfigLoader(Interface):
     """A configuration file loader."""
 
     def load(filename):
         """Load a configuration from the file at filename."""
 
     def loadFile(source_file, filename=None):
@@ -148,17 +151,18 @@
     by a colon (:).
 
     Multiple sections with the same major category may have their keys defined
     in another section that appends the '.template' or '.master' suffixes to
     the category name. A section with '.optional' suffix is not
     required. Lines that start with a hash (#) are comments.
     """
-    name = Attribute('The basename of the config filename.')
-    filename = Attribute('The path to config file')
-    category_names = Attribute('The list of section category names.')
+
+    name = Attribute("The basename of the config filename.")
+    filename = Attribute("The path to config file")
+    category_names = Attribute("The list of section category names.")
 
     def __iter__():
         """Iterate over the `ISectionSchema`s."""
 
     def __contains__(name):
         """Return True or False if the name matches a `ISectionSchema`."""
 
@@ -202,20 +206,20 @@
     in the 'meta' section of the config data file:
         [meta]
         extends: common.conf
 
     The push() and pop() methods can be used to test processes where the
     test environment must be configured differently.
     """
+
     schema = Attribute("The schema that defines the config.")
     data = Attribute("The current ConfigData. use by the config.")
     extends = Attribute("The ConfigData that this config extends.")
     overlays = Attribute("The stack of ConfigData that define this config.")
 
-
     def __getattr__(name):
         """Return the named section.
 
         :name: a section or category name.
         :return: the matching `ISection` or `ICategory`.
         :raise: AttributeError if there is no section or category with the
             name.
```

### Comparing `lazr.config-2.2.3/src/lazr/config/tests/test_config.py` & `lazr.config-3.0/src/lazr/config/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,222 +12,257 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with lazr.config.  If not, see <http://www.gnu.org/licenses/>.
 
 """Tests of lazr.config."""
 
-from __future__ import absolute_import, print_function, unicode_literals
-
-__metaclass__ = type
 __all__ = [
-    'TestConfig',
-    ]
+    "TestConfig",
+]
 
 
 import unittest
+
 import pkg_resources
+
 try:
     from configparser import MissingSectionHeaderError, NoSectionError
 except ImportError:
     # Python 2
     from ConfigParser import MissingSectionHeaderError, NoSectionError
 try:
     from io import StringIO
 except ImportError:
     # Python 2
     from StringIO import StringIO
 
 from operator import attrgetter
+
 from zope.interface.exceptions import DoesNotImplement
 from zope.interface.verify import verifyObject
 
 from lazr.config import ConfigSchema, ImplicitTypeSchema
 from lazr.config.interfaces import (
-    ConfigErrors, IStackableConfig, InvalidSectionNameError, NoCategoryError,
-    NoConfigError, RedefinedSectionError, UnknownKeyError,
-    UnknownSectionError)
+    ConfigErrors,
+    InvalidSectionNameError,
+    IStackableConfig,
+    NoCategoryError,
+    NoConfigError,
+    RedefinedSectionError,
+    UnknownKeyError,
+    UnknownSectionError,
+)
 
 
 class TestConfig(unittest.TestCase):
-    def setUp(self):
-        # Python 2.6 does not have assertMultilineEqual
-        self.meq = getattr(self, 'assertMultiLineEqual', self.assertEqual)
-
     def _testfile(self, conf_file):
         return pkg_resources.resource_filename(
-            'lazr.config.tests.testdata', conf_file)
+            "lazr.config.tests.testdata", conf_file
+        )
 
     def test_missing_category(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        self.assertRaises(NoCategoryError, schema.getByCategory, 'non-section')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        self.assertRaises(NoCategoryError, schema.getByCategory, "non-section")
 
     def test_missing_file(self):
-        self.assertRaises(IOError, ConfigSchema, '/does/not/exist')
+        self.assertRaises(IOError, ConfigSchema, "/does/not/exist")
 
     def test_must_be_ascii(self):
-        self.assertRaises(UnicodeError,
-                          ConfigSchema, self._testfile('bad-nonascii.conf'))
+        self.assertRaises(
+            UnicodeError, ConfigSchema, self._testfile("bad-nonascii.conf")
+        )
 
     def test_missing_schema_section(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        self.assertRaises(NoSectionError, schema.__getitem__, 'section-4')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        self.assertRaises(NoSectionError, schema.__getitem__, "section-4")
 
     def test_missing_header_section(self):
-        self.assertRaises(MissingSectionHeaderError,
-                          ConfigSchema, self._testfile('bad-sectionless.conf'))
+        self.assertRaises(
+            MissingSectionHeaderError,
+            ConfigSchema,
+            self._testfile("bad-sectionless.conf"),
+        )
 
     def test_redefined_section(self):
-        self.assertRaises(RedefinedSectionError,
-                          ConfigSchema,
-                          self._testfile('bad-redefined-section.conf'))
+        self.assertRaises(
+            RedefinedSectionError,
+            ConfigSchema,
+            self._testfile("bad-redefined-section.conf"),
+        )
         # XXX sinzui 2007-12-13:
         # ConfigSchema should raise RedefinedKeyError when a section redefines
         # a key.
 
     def test_invalid_section_name(self):
-        self.assertRaises(InvalidSectionNameError,
-                          ConfigSchema,
-                          self._testfile('bad-invalid-name.conf'))
+        self.assertRaises(
+            InvalidSectionNameError,
+            ConfigSchema,
+            self._testfile("bad-invalid-name.conf"),
+        )
 
     def test_invalid_characters(self):
-        self.assertRaises(InvalidSectionNameError,
-                          ConfigSchema,
-                          self._testfile('bad-invalid-name-chars.conf'))
+        self.assertRaises(
+            InvalidSectionNameError,
+            ConfigSchema,
+            self._testfile("bad-invalid-name-chars.conf"),
+        )
 
     def test_load_missing_file(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        self.assertRaises(IOError, schema.load, '/no/such/file.conf')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        self.assertRaises(IOError, schema.load, "/no/such/file.conf")
 
     def test_no_name_argument(self):
         config = """
 [meta]
 metakey: unsupported
 [unknown-section]
 key1 = value1
 [section_1]
 keyn: unknown key
 key1: bad character in caf\xc3)
 [section_3.template]
 key1: schema suffixes are not permitted
 """
-        schema = ConfigSchema(self._testfile('base.conf'))
+        schema = ConfigSchema(self._testfile("base.conf"))
         self.assertRaises(AttributeError, schema.loadFile, StringIO(config))
 
     def test_missing_section(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        self.assertRaises(NoSectionError, config.__getitem__, 'section-4')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        self.assertRaises(NoSectionError, config.__getitem__, "section-4")
 
     def test_undeclared_optional_section(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        self.assertRaises(NoSectionError,
-                          config.__getitem__, 'section_3.app_a')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        self.assertRaises(
+            NoSectionError, config.__getitem__, "section_3.app_a"
+        )
 
     def test_nonexistent_category_name(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        self.assertRaises(NoCategoryError,
-                          config.getByCategory, 'non-section')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        self.assertRaises(NoCategoryError, config.getByCategory, "non-section")
 
     def test_all_config_errors(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.loadFile(StringIO("""
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.loadFile(
+            StringIO(
+                """
 [meta]
 metakey: unsupported
 [unknown-section]
 key1 = value1
 [section_1]
 keyn: unknown key
 key1: bad character in caf\xc3)
 [section_3.template]
 key1: schema suffixes are not permitted
-"""), 'bad config')
+"""
+            ),
+            "bad config",
+        )
         try:
             config.validate()
         except ConfigErrors as errors:
             sorted_errors = sorted(
-                errors.errors, key=attrgetter('__class__.__name__'))
-            self.assertEqual(str(errors),
-                             'ConfigErrors: bad config is not valid.')
+                errors.errors, key=attrgetter("__class__.__name__")
+            )
+            self.assertEqual(
+                str(errors), "ConfigErrors: bad config is not valid."
+            )
         else:
-            self.fail('ConfigErrors expected')
+            self.fail("ConfigErrors expected")
         self.assertEqual(len(sorted_errors), 4)
-        self.assertEqual([error.__class__ for error in sorted_errors],
-                         [UnicodeEncodeError, UnknownKeyError,
-                          UnknownKeyError, UnknownSectionError])
+        self.assertEqual(
+            [error.__class__ for error in sorted_errors],
+            [
+                UnicodeEncodeError,
+                UnknownKeyError,
+                UnknownKeyError,
+                UnknownSectionError,
+            ],
+        )
 
     def test_not_stackable(self):
         try:
             from zope.interface.exceptions import MultipleInvalid
         except ImportError:  # zope.interface < 5.0.0
+
             class MultipleInvalid(Exception):
                 pass
 
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
         try:
             verifyObject(IStackableConfig, config.extends)
         except DoesNotImplement:
             pass
         except MultipleInvalid as e:
-            if not any(isinstance(invalid, DoesNotImplement)
-                       for invalid in e.exceptions):
-                self.fail('MultipleInvalid raised without DoesNotImplement')
+            if not any(
+                isinstance(invalid, DoesNotImplement)
+                for invalid in e.exceptions
+            ):
+                self.fail("MultipleInvalid raised without DoesNotImplement")
         else:
-            self.fail('DoesNotImplement not raised')
+            self.fail("DoesNotImplement not raised")
 
     def test_bad_pop(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        config.push('one', '')
-        config.push('two', '')
-        self.assertRaises(NoConfigError, config.pop, 'bad-name')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        config.push("one", "")
+        config.push("two", "")
+        self.assertRaises(NoConfigError, config.pop, "bad-name")
 
     def test_cannot_pop_bottom(self):
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        config.pop('local.conf')
-        self.assertRaises(NoConfigError, config.pop, 'base.conf')
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        config.pop("local.conf")
+        self.assertRaises(NoConfigError, config.pop, "base.conf")
 
     def test_multiline_preserves_indentation(self):
-        schema = ImplicitTypeSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        convert = config['section_1']._convert
+        schema = ImplicitTypeSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        convert = config["section_1"]._convert
         orig = """\
 multiline value 1
     multiline value 2"""
         new = convert(orig)
-        self.meq(new, orig)
+        self.assertMultiLineEqual(new, orig)
 
     def test_multiline_strips_leading_and_trailing_whitespace(self):
-        schema = ImplicitTypeSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        convert = config['section_1']._convert
+        schema = ImplicitTypeSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        convert = config["section_1"]._convert
         orig = """
     multiline value 1
     multiline value 2
     """
         new = convert(orig)
-        self.meq(new, orig.strip())
+        self.assertMultiLineEqual(new, orig.strip())
 
     def test_multiline_key(self):
-        schema = ImplicitTypeSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        self.meq(config['section_33'].key2, """\
+        schema = ImplicitTypeSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        self.assertMultiLineEqual(
+            config["section_33"].key2,
+            """\
 multiline value 1
-multiline value 2""")
+multiline value 2""",
+        )
 
     def test_lp1397779(self):
         # Fix DuplicateSectionErrors when you .push() a config that has a
         # section already defined in the config.
-        schema = ConfigSchema(self._testfile('base.conf'))
-        config = schema.load(self._testfile('local.conf'))
-        self.assertEqual(config['section_1']['key1'], 'foo')
-        config.push('dupsec', """\
+        schema = ConfigSchema(self._testfile("base.conf"))
+        config = schema.load(self._testfile("local.conf"))
+        self.assertEqual(config["section_1"]["key1"], "foo")
+        config.push(
+            "dupsec",
+            """\
 [section_1]
 key1: baz
 [section_1]
 key1: qux
-""")
-        self.assertEqual(config['section_1']['key1'], 'qux')
+""",
+        )
+        self.assertEqual(config["section_1"]["key1"], "qux")
```

### Comparing `lazr.config-2.2.3/src/lazr/config/tests/testdata/base.conf` & `lazr.config-3.0/src/lazr/config/tests/testdata/base.conf`

 * *Files identical despite different names*

### Comparing `lazr.config-2.2.3/src/lazr.config.egg-info/PKG-INFO` & `lazr.config-3.0/src/lazr.config.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: lazr.config
-Version: 2.2.3
+Version: 3.0
 Summary: Create configuration schemas, and process and validate configurations.
 Home-page: https://launchpad.net/lazr.config
+Download-URL: https://launchpad.net/lazr.config/+download
 Maintainer: LAZR Developers
 Maintainer-email: lazr-developers@lists.launchpad.net
 License: LGPL v3
-Download-URL: https://launchpad.net/lazr.config/+download
-Description: 
-        The LAZR config system is typically used to manage process configuration.
-        Process configuration is for saying how things change when we run systems on
-        different machines, or under different circumstances.
-        
-        This system uses ini-like file format of section, keys, and values.  The
-        config file supports inheritance to minimize duplication of information across
-        files. The format supports schema validation.
-        
-Platform: UNKNOWN
+Project-URL: Source, https://code.launchpad.net/lazr.config
+Project-URL: Issue Tracker, https://bugs.launchpad.net/lazr.config
+Project-URL: Documentation, https://lazrconfig.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.5
+Provides-Extra: docs
+License-File: COPYING.txt
+
+
+The LAZR config system is typically used to manage process configuration.
+Process configuration is for saying how things change when we run systems on
+different machines, or under different circumstances.
+
+This system uses ini-like file format of section, keys, and values.  The
+config file supports inheritance to minimize duplication of information across
+files. The format supports schema validation.
```

### Comparing `lazr.config-2.2.3/src/lazr.config.egg-info/SOURCES.txt` & `lazr.config-3.0/src/lazr.config.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+.pre-commit-config.yaml
+.woke.yaml
+CONTRIBUTING.rst
 COPYING.txt
-HACKING.rst
 MANIFEST.in
 NEWS.rst
 README.rst
-conf.py
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 src/lazr/__init__.py
 src/lazr.config.egg-info/PKG-INFO
 src/lazr.config.egg-info/SOURCES.txt
 src/lazr.config.egg-info/dependency_links.txt
@@ -15,20 +17,22 @@
 src/lazr.config.egg-info/not-zip-safe
 src/lazr.config.egg-info/requires.txt
 src/lazr.config.egg-info/top_level.txt
 src/lazr/config/__init__.py
 src/lazr/config/_config.py
 src/lazr/config/_version.py
 src/lazr/config/interfaces.py
+src/lazr/config/docs/CONTRIBUTING.rst
+src/lazr/config/docs/NEWS.rst
 src/lazr/config/docs/__init__.py
-src/lazr/config/docs/fixture.py
-src/lazr/config/docs/usage.rst
-src/lazr/config/docs/usage_fixture.py
+src/lazr/config/docs/conf.py
+src/lazr/config/docs/index.rst
 src/lazr/config/tests/__init__.py
 src/lazr/config/tests/test_config.py
+src/lazr/config/tests/test_docs.py
 src/lazr/config/tests/testdata/__init__.py
 src/lazr/config/tests/testdata/bad-invalid-name-chars.conf
 src/lazr/config/tests/testdata/bad-invalid-name.conf
 src/lazr/config/tests/testdata/bad-nonascii.conf
 src/lazr/config/tests/testdata/bad-redefined-key.conf
 src/lazr/config/tests/testdata/bad-redefined-section.conf
 src/lazr/config/tests/testdata/bad-sectionless.conf
```

