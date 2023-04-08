# Comparing `tmp/PSNAWP-1.2.2.tar.gz` & `tmp/PSNAWP-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSNAWP-1.2.2.tar", last modified: Sun Apr  2 20:24:29 2023, max compression
+gzip compressed data, was "PSNAWP-1.2.3.tar", last modified: Sat Apr  8 21:27:22 2023, max compression
```

## Comparing `PSNAWP-1.2.2.tar` & `PSNAWP-1.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.571699 PSNAWP-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.575699 PSNAWP-1.2.2/src/PSNAWP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-02 20:24:29.000000 PSNAWP-1.2.2/src/PSNAWP.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.575699 PSNAWP-1.2.2/src/psnawp_api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.575699 PSNAWP-1.2.2/src/psnawp_api/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/core/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/core/psnawp_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/src/psnawp_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/game_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/title_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/src/psnawp_api/models/trophies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/trophies/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/psnawp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:29.579699 PSNAWP-1.2.2/src/psnawp_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/utils/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-02 20:24:10.000000 PSNAWP-1.2.2/src/psnawp_api/utils/request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.068305 PSNAWP-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.068305 PSNAWP-1.2.3/src/PSNAWP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/psnawp_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/game_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/title_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/models/trophies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/psnawp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/request_builder.py
```

### Comparing `PSNAWP-1.2.2/LICENSE.md` & `PSNAWP-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/PKG-INFO` & `PSNAWP-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.2 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.3 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
```

### Comparing `PSNAWP-1.2.2/README.md` & `PSNAWP-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/pyproject.toml` & `PSNAWP-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/requirements.txt` & `PSNAWP-1.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/requirements_dev.txt` & `PSNAWP-1.2.3/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/setup.cfg` & `PSNAWP-1.2.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PSNAWP
-version = 1.2.2
+version = 1.2.3
 author = Yoshikage Kira (@isFakeAccount)
 author_email = trevorphillips@gmx.us
 url = https://github.com/isFakeAccount/psnawp
 description = Python API Wrapper for PlayStation Network API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `PSNAWP-1.2.2/src/PSNAWP.egg-info/PKG-INFO` & `PSNAWP-1.2.3/src/PSNAWP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.2 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.3 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
```

### Comparing `PSNAWP-1.2.2/src/PSNAWP.egg-info/SOURCES.txt` & `PSNAWP-1.2.3/src/PSNAWP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/PSNAWP.egg-info/requires.txt` & `PSNAWP-1.2.3/src/PSNAWP.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/core/authenticator.py` & `PSNAWP-1.2.3/src/psnawp_api/core/authenticator.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/core/psnawp_exceptions.py` & `PSNAWP-1.2.3/src/psnawp_api/core/psnawp_exceptions.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/client.py` & `PSNAWP-1.2.3/src/psnawp_api/models/client.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/game_title.py` & `PSNAWP-1.2.3/src/psnawp_api/models/game_title.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/group.py` & `PSNAWP-1.2.3/src/psnawp_api/models/group.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/search.py` & `PSNAWP-1.2.3/src/psnawp_api/models/search.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/title_stats.py` & `PSNAWP-1.2.3/src/psnawp_api/models/title_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,37 +61,37 @@
         )
         return title_instance
 
     @classmethod
     def from_endpoint(cls, request_builder: RequestBuilder, account_id: str, limit: Optional[int]) -> Iterator[TitleStats]:
 
         offset = 0
-        limit_per_page = min(limit, 1000) if limit is not None else 1000
+        limit_per_page = min(limit, 500) if limit is not None else 500
         params: dict[str, Any] = {"categories": "ps4_game,ps5_native_game", "limit": limit_per_page, "offset": offset}
 
-        total_items = 0
         while True:
             params["offset"] = offset
             try:
                 response = request_builder.get(
                     url=f"{BASE_PATH['games_list']}{API_PATH['user_game_data'].format(account_id=account_id)}",
                     params=params,
                 ).json()
             except PSNAWPForbidden as forbidden:
                 raise PSNAWPForbidden("The following user has made their profile private.") from forbidden
 
             titles: list[dict[str, Any]] = response.get("titles")
 
+            per_page_items = 0
             for title in titles:
                 title_instance = TitleStats.from_dict({**title, "totalItemCount": response.get("totalItemCount")})
                 yield title_instance
-                total_items += 1
+                per_page_items += 1
 
             if limit is not None:
-                limit -= total_items
+                limit -= per_page_items
                 params["limit"] = min(limit, limit_per_page)
 
                 # If limit is reached
                 if limit <= 0:
                     break
 
             offset = response.get("nextOffset") or 0
```

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy.py` & `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_constants.py` & `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_constants.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_group.py` & `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_group.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_summary.py` & `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_summary.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/trophies/trophy_titles.py` & `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_titles.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/models/user.py` & `PSNAWP-1.2.3/src/psnawp_api/models/user.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/psnawp.py` & `PSNAWP-1.2.3/src/psnawp_api/psnawp.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/utils/endpoints.py` & `PSNAWP-1.2.3/src/psnawp_api/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/utils/misc.py` & `PSNAWP-1.2.3/src/psnawp_api/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.2/src/psnawp_api/utils/request_builder.py` & `PSNAWP-1.2.3/src/psnawp_api/utils/request_builder.py`

 * *Files identical despite different names*

