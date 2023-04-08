# Comparing `tmp/agstoolbox-0.3.2.tar.gz` & `tmp/agstoolbox-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agstoolbox-0.3.2.tar", last modified: Sat Apr  8 04:31:06 2023, max compression
+gzip compressed data, was "agstoolbox-0.3.3.tar", last modified: Sat Apr  8 18:15:19 2023, max compression
```

## Comparing `agstoolbox-0.3.2.tar` & `agstoolbox-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.356097 agstoolbox-0.3.2/
--rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/AUTHORS
--rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/COPYING
--rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       86 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1189 2023-04-08 04:31:06.356097 agstoolbox-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.2/README.rst
--rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/agstoolbox
--rw-rw-rw-   0        0        0      400 2023-04-08 03:13:15.000000 agstoolbox-0.3.2/atbx
--rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 04:31:06.356097 agstoolbox-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-08 03:22:46.000000 agstoolbox-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.310112 agstoolbox-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.328097 agstoolbox-0.3.2/src/agstoolbox/
--rw-rw-rw-   0        0        0      206 2023-04-08 04:29:59.000000 agstoolbox-0.3.2/src/agstoolbox/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-04-08 04:29:56.000000 agstoolbox-0.3.2/src/agstoolbox/__main__.py
--rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.2/src/agstoolbox/at_icons.py
--rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.2/src/agstoolbox/at_tasks.py
--rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.2/src/agstoolbox/at_trayindicator.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.349097 agstoolbox-0.3.2/src/agstoolbox/data/
--rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.2/src/agstoolbox/data/at_ags_editor_icon.png
--rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/src/agstoolbox/data/at_ags_engine_icon.png
--rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.2/src/agstoolbox/data/at_icon.png
--rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.2/src/agstoolbox/data/at_icon_big.png
--rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.2/src/agstoolbox/data/exit_icon.png
--rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.2/src/agstoolbox/data/refresh_icon.png
--rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.2/src/agstoolbox/data/settings_icon.png
--rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.2/src/agstoolbox/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.343096 agstoolbox-0.3.2/src/agstoolbox.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-08 04:31:06.000000 agstoolbox-0.3.2/src/agstoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-04-08 04:31:06.000000 agstoolbox-0.3.2/src/agstoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 04:31:06.000000 agstoolbox-0.3.2/src/agstoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-08 04:31:06.000000 agstoolbox-0.3.2/src/agstoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 04:31:06.000000 agstoolbox-0.3.2/src/agstoolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 04:31:06.355097 agstoolbox-0.3.2/tests/
--rw-rw-rw-   0        0        0     1827 2022-01-29 21:31:17.000000 agstoolbox-0.3.2/tests/test_ags.py
--rw-rw-rw-   0        0        0     1664 2023-04-03 02:26:20.000000 agstoolbox-0.3.2/tests/test_gh.py
--rw-rw-rw-   0        0        0     1737 2023-04-05 23:37:44.000000 agstoolbox-0.3.2/tests/test_pe.py
--rw-rw-rw-   0        0        0     4315 2023-04-07 02:30:24.000000 agstoolbox-0.3.2/tests/test_settings_utils.py
--rw-rw-rw-   0        0        0     1255 2023-04-05 23:35:27.000000 agstoolbox-0.3.2/tests/test_time.py
--rw-rw-rw-   0        0        0     2894 2023-04-05 23:34:14.000000 agstoolbox-0.3.2/tests/test_utils.py
--rw-rw-rw-   0        0        0     3747 2023-04-06 00:01:05.000000 agstoolbox-0.3.2/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.246066 agstoolbox-0.3.3/
+-rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/AUTHORS
+-rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/COPYING
+-rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       86 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1189 2023-04-08 18:15:19.245068 agstoolbox-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.3/README.rst
+-rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/agstoolbox
+-rw-rw-rw-   0        0        0      400 2023-04-08 03:13:15.000000 agstoolbox-0.3.3/atbx
+-rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:15:19.246066 agstoolbox-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-04-08 03:22:46.000000 agstoolbox-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.141407 agstoolbox-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.161407 agstoolbox-0.3.3/src/agstoolbox/
+-rw-rw-rw-   0        0        0      198 2023-04-08 18:13:25.000000 agstoolbox-0.3.3/src/agstoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1017 2023-04-08 04:29:56.000000 agstoolbox-0.3.3/src/agstoolbox/__main__.py
+-rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.3/src/agstoolbox/at_icons.py
+-rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.3/src/agstoolbox/at_tasks.py
+-rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.3/src/agstoolbox/at_trayindicator.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.208067 agstoolbox-0.3.3/src/agstoolbox/data/
+-rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_ags_editor_icon.png
+-rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_ags_engine_icon.png
+-rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_icon.png
+-rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_icon_big.png
+-rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.3/src/agstoolbox/data/exit_icon.png
+-rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.3/src/agstoolbox/data/refresh_icon.png
+-rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.3/src/agstoolbox/data/settings_icon.png
+-rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/src/agstoolbox/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.177406 agstoolbox-0.3.3/src/agstoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.244067 agstoolbox-0.3.3/tests/
+-rw-rw-rw-   0        0        0     1827 2022-01-29 21:31:17.000000 agstoolbox-0.3.3/tests/test_ags.py
+-rw-rw-rw-   0        0        0     1664 2023-04-03 02:26:20.000000 agstoolbox-0.3.3/tests/test_gh.py
+-rw-rw-rw-   0        0        0     1737 2023-04-05 23:37:44.000000 agstoolbox-0.3.3/tests/test_pe.py
+-rw-rw-rw-   0        0        0     4315 2023-04-07 02:30:24.000000 agstoolbox-0.3.3/tests/test_settings_utils.py
+-rw-rw-rw-   0        0        0     1255 2023-04-05 23:35:27.000000 agstoolbox-0.3.3/tests/test_time.py
+-rw-rw-rw-   0        0        0     2894 2023-04-05 23:34:14.000000 agstoolbox-0.3.3/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3747 2023-04-06 00:01:05.000000 agstoolbox-0.3.3/tests/test_version.py
```

### Comparing `agstoolbox-0.3.2/COPYING` & `agstoolbox-0.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/LICENSE` & `agstoolbox-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/PKG-INFO` & `agstoolbox-0.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.2
+Version: 0.3.3
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.2
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.3
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.2/README.rst` & `agstoolbox-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/pyproject.toml` & `agstoolbox-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/setup.py` & `agstoolbox-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/__main__.py` & `agstoolbox-0.3.3/src/agstoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/at_icons.py` & `agstoolbox-0.3.3/src/agstoolbox/at_icons.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/at_tasks.py` & `agstoolbox-0.3.3/src/agstoolbox/at_tasks.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/at_trayindicator.py` & `agstoolbox-0.3.3/src/agstoolbox/at_trayindicator.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/at_ags_editor_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/at_ags_editor_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/at_ags_engine_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/at_ags_engine_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/at_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/at_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/at_icon_big.png` & `agstoolbox-0.3.3/src/agstoolbox/data/at_icon_big.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/exit_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/exit_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/refresh_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/refresh_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/data/settings_icon.png` & `agstoolbox-0.3.3/src/agstoolbox/data/settings_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox/getdata.py` & `agstoolbox-0.3.3/src/agstoolbox/getdata.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/src/agstoolbox.egg-info/PKG-INFO` & `agstoolbox-0.3.3/src/agstoolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.2
+Version: 0.3.3
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.2
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.3
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.2/src/agstoolbox.egg-info/SOURCES.txt` & `agstoolbox-0.3.3/src/agstoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_ags.py` & `agstoolbox-0.3.3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_gh.py` & `agstoolbox-0.3.3/tests/test_gh.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_pe.py` & `agstoolbox-0.3.3/tests/test_pe.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_settings_utils.py` & `agstoolbox-0.3.3/tests/test_settings_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_time.py` & `agstoolbox-0.3.3/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_utils.py` & `agstoolbox-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.2/tests/test_version.py` & `agstoolbox-0.3.3/tests/test_version.py`

 * *Files identical despite different names*

