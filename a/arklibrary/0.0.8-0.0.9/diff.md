# Comparing `tmp/arklibrary-0.0.8.tar.gz` & `tmp/arklibrary-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arklibrary-0.0.8.tar", last modified: Sat Aug 20 23:21:30 2022, max compression
+gzip compressed data, was "arklibrary-0.0.9.tar", last modified: Sun Aug 21 00:22:06 2022, max compression
```

## Comparing `arklibrary-0.0.8.tar` & `arklibrary-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.695291 arklibrary-0.0.8/
--rw-rw-rw-   0        0        0     1095 2022-08-11 13:59:26.000000 arklibrary-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      662 2022-08-20 23:21:30.696292 arklibrary-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-08-17 05:16:41.000000 arklibrary-0.0.8/README.md
--rw-rw-rw-   0        0        0      536 2022-08-17 05:16:41.000000 arklibrary-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      995 2022-08-20 23:21:30.697292 arklibrary-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.641293 arklibrary-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.648291 arklibrary-0.0.8/src/arklibrary/
--rw-rw-rw-   0        0        0      130 2022-08-20 20:36:56.000000 arklibrary-0.0.8/src/arklibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.664294 arklibrary-0.0.8/src/arklibrary/admin/
--rw-rw-rw-   0        0        0      303 2022-08-20 22:13:21.000000 arklibrary-0.0.8/src/arklibrary/admin/__init__.py
--rw-rw-rw-   0        0        0     1800 2022-08-20 22:37:07.000000 arklibrary-0.0.8/src/arklibrary/admin/admin.py
--rw-rw-rw-   0        0        0    10216 2022-08-20 22:38:20.000000 arklibrary-0.0.8/src/arklibrary/admin/bundle.py
--rw-rw-rw-   0        0        0    20084 2022-08-20 22:38:20.000000 arklibrary-0.0.8/src/arklibrary/admin/commands.py
--rw-rw-rw-   0        0        0     2123 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/admin/run_driver.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.683291 arklibrary-0.0.8/src/arklibrary/blueprints/
--rw-rw-rw-   0        0        0     1101 2022-08-20 22:13:21.000000 arklibrary-0.0.8/src/arklibrary/blueprints/__init__.py
--rw-rw-rw-   0        0        0     3803 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/ammunitions.py
--rw-rw-rw-   0        0        0     9636 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/armours.py
--rw-rw-rw-   0        0        0     9294 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/artifacts.py
--rw-rw-rw-   0        0        0    11005 2021-10-13 20:30:55.000000 arklibrary-0.0.8/src/arklibrary/blueprints/beacons.py
--rw-rw-rw-   0        0        0    17601 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/chibis.py
--rw-rw-rw-   0        0        0     7885 2021-10-13 20:02:05.000000 arklibrary-0.0.8/src/arklibrary/blueprints/colors.py
--rw-rw-rw-   0        0        0     9913 2021-09-24 02:50:11.000000 arklibrary-0.0.8/src/arklibrary/blueprints/commands.py
--rw-rw-rw-   0        0        0    21773 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/consumables.py
--rw-rw-rw-   0        0        0    78373 2022-08-20 22:11:17.000000 arklibrary-0.0.8/src/arklibrary/blueprints/creatures.py
--rw-rw-rw-   0        0        0     3028 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/dyes.py
--rw-rw-rw-   0        0        0    11739 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/eggs.py
--rw-rw-rw-   0        0        0      942 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/farming.py
--rw-rw-rw-   0        0        0     2368 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/recipes.py
--rw-rw-rw-   0        0        0    11037 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/resources.py
--rw-rw-rw-   0        0        0    13208 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/saddles.py
--rw-rw-rw-   0        0        0     2146 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/seeds.py
--rw-rw-rw-   0        0        0    33071 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/skins.py
--rw-rw-rw-   0        0        0    52735 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/structures.py
--rw-rw-rw-   0        0        0     3409 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/tools.py
--rw-rw-rw-   0        0        0     5723 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/trophies.py
--rw-rw-rw-   0        0        0     8052 2022-08-20 22:05:40.000000 arklibrary-0.0.8/src/arklibrary/blueprints/weapons.py
--rw-rw-rw-   0        0        0      227 2022-08-15 04:49:50.000000 arklibrary-0.0.8/src/arklibrary/config.ini
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.686294 arklibrary-0.0.8/src/arklibrary/data_structures/
--rw-rw-rw-   0        0        0       88 2022-08-20 20:52:25.000000 arklibrary-0.0.8/src/arklibrary/data_structures/__init__.py
--rw-rw-rw-   0        0        0      602 2022-08-20 23:21:23.000000 arklibrary-0.0.8/src/arklibrary/data_structures/encoder.py
--rw-rw-rw-   0        0        0     2228 2022-08-20 23:11:46.000000 arklibrary-0.0.8/src/arklibrary/data_structures/stream.py
--rw-rw-rw-   0        0        0     4224 2022-08-20 22:39:42.000000 arklibrary-0.0.8/src/arklibrary/data_structures/tri.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.688291 arklibrary-0.0.8/src/arklibrary/events/
--rw-rw-rw-   0        0        0        0 2022-08-20 18:00:52.000000 arklibrary-0.0.8/src/arklibrary/events/__init__.py
--rw-rw-rw-   0        0        0     5211 2021-10-17 07:56:36.000000 arklibrary-0.0.8/src/arklibrary/events/events.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.689294 arklibrary-0.0.8/src/arklibrary/lib/
--rw-rw-rw-   0        0        0       69 2022-08-17 05:16:41.000000 arklibrary-0.0.8/src/arklibrary/lib/__init__.py
--rw-rw-rw-   0        0        0     2278 2022-08-20 22:39:42.000000 arklibrary-0.0.8/src/arklibrary/lib/configuration.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.694293 arklibrary-0.0.8/src/arklibrary/tools/
--rw-rw-rw-   0        0        0        2 2021-10-15 20:23:29.000000 arklibrary-0.0.8/src/arklibrary/tools/__init__.py
--rw-rw-rw-   0        0        0     2831 2021-10-05 00:32:43.000000 arklibrary-0.0.8/src/arklibrary/tools/ark_generic_scraper.py
--rw-rw-rw-   0        0        0    14575 2021-10-13 20:49:49.000000 arklibrary-0.0.8/src/arklibrary/tools/ark_image_scraper.py
--rw-rw-rw-   0        0        0     4478 2021-09-24 02:58:55.000000 arklibrary-0.0.8/src/arklibrary/tools/clipboard.py
--rw-rw-rw-   0        0        0      956 2022-08-20 22:39:42.000000 arklibrary-0.0.8/src/arklibrary/tools/config.py
--rw-rw-rw-   0        0        0     1196 2021-09-24 02:57:41.000000 arklibrary-0.0.8/src/arklibrary/tools/read.py
-drwxrwxrwx   0        0        0        0 2022-08-20 23:21:30.659291 arklibrary-0.0.8/src/arklibrary.egg-info/
--rw-rw-rw-   0        0        0      662 2022-08-20 23:21:30.000000 arklibrary-0.0.8/src/arklibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1776 2022-08-20 23:21:30.000000 arklibrary-0.0.8/src/arklibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-20 23:21:30.000000 arklibrary-0.0.8/src/arklibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2022-08-20 23:21:30.000000 arklibrary-0.0.8/src/arklibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-08-20 23:21:30.000000 arklibrary-0.0.8/src/arklibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.676860 arklibrary-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2022-08-11 13:59:26.000000 arklibrary-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      662 2022-08-21 00:22:06.677859 arklibrary-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2022-08-17 05:16:41.000000 arklibrary-0.0.9/README.md
+-rw-rw-rw-   0        0        0      536 2022-08-17 05:16:41.000000 arklibrary-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      995 2022-08-21 00:22:06.682860 arklibrary-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.626860 arklibrary-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.633859 arklibrary-0.0.9/src/arklibrary/
+-rw-rw-rw-   0        0        0      130 2022-08-20 20:36:56.000000 arklibrary-0.0.9/src/arklibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.646865 arklibrary-0.0.9/src/arklibrary/admin/
+-rw-rw-rw-   0        0        0      303 2022-08-20 22:13:21.000000 arklibrary-0.0.9/src/arklibrary/admin/__init__.py
+-rw-rw-rw-   0        0        0     1800 2022-08-20 22:37:07.000000 arklibrary-0.0.9/src/arklibrary/admin/admin.py
+-rw-rw-rw-   0        0        0    10216 2022-08-20 22:38:20.000000 arklibrary-0.0.9/src/arklibrary/admin/bundle.py
+-rw-rw-rw-   0        0        0    20084 2022-08-20 22:38:20.000000 arklibrary-0.0.9/src/arklibrary/admin/commands.py
+-rw-rw-rw-   0        0        0     2123 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/admin/run_driver.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.664860 arklibrary-0.0.9/src/arklibrary/blueprints/
+-rw-rw-rw-   0        0        0     1101 2022-08-20 22:13:21.000000 arklibrary-0.0.9/src/arklibrary/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     3803 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/ammunitions.py
+-rw-rw-rw-   0        0        0     9636 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/armours.py
+-rw-rw-rw-   0        0        0     9294 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/artifacts.py
+-rw-rw-rw-   0        0        0    11005 2021-10-13 20:30:55.000000 arklibrary-0.0.9/src/arklibrary/blueprints/beacons.py
+-rw-rw-rw-   0        0        0    17601 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/chibis.py
+-rw-rw-rw-   0        0        0     7885 2021-10-13 20:02:05.000000 arklibrary-0.0.9/src/arklibrary/blueprints/colors.py
+-rw-rw-rw-   0        0        0     9913 2021-09-24 02:50:11.000000 arklibrary-0.0.9/src/arklibrary/blueprints/commands.py
+-rw-rw-rw-   0        0        0    21773 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/consumables.py
+-rw-rw-rw-   0        0        0    78373 2022-08-20 22:11:17.000000 arklibrary-0.0.9/src/arklibrary/blueprints/creatures.py
+-rw-rw-rw-   0        0        0     3028 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/dyes.py
+-rw-rw-rw-   0        0        0    11739 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/eggs.py
+-rw-rw-rw-   0        0        0      942 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/farming.py
+-rw-rw-rw-   0        0        0     2368 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/recipes.py
+-rw-rw-rw-   0        0        0    11037 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/resources.py
+-rw-rw-rw-   0        0        0    13208 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/saddles.py
+-rw-rw-rw-   0        0        0     2146 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/seeds.py
+-rw-rw-rw-   0        0        0    33071 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/skins.py
+-rw-rw-rw-   0        0        0    52735 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/structures.py
+-rw-rw-rw-   0        0        0     3409 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/tools.py
+-rw-rw-rw-   0        0        0     5723 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/trophies.py
+-rw-rw-rw-   0        0        0     8052 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/weapons.py
+-rw-rw-rw-   0        0        0      227 2022-08-15 04:49:50.000000 arklibrary-0.0.9/src/arklibrary/config.ini
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.668862 arklibrary-0.0.9/src/arklibrary/data_structures/
+-rw-rw-rw-   0        0        0       88 2022-08-20 20:52:25.000000 arklibrary-0.0.9/src/arklibrary/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-08-20 23:21:23.000000 arklibrary-0.0.9/src/arklibrary/data_structures/encoder.py
+-rw-rw-rw-   0        0        0     2306 2022-08-21 00:21:58.000000 arklibrary-0.0.9/src/arklibrary/data_structures/stream.py
+-rw-rw-rw-   0        0        0     4224 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/data_structures/tri.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.669859 arklibrary-0.0.9/src/arklibrary/events/
+-rw-rw-rw-   0        0        0        0 2022-08-20 18:00:52.000000 arklibrary-0.0.9/src/arklibrary/events/__init__.py
+-rw-rw-rw-   0        0        0     5211 2021-10-17 07:56:36.000000 arklibrary-0.0.9/src/arklibrary/events/events.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.671861 arklibrary-0.0.9/src/arklibrary/lib/
+-rw-rw-rw-   0        0        0       69 2022-08-17 05:16:41.000000 arklibrary-0.0.9/src/arklibrary/lib/__init__.py
+-rw-rw-rw-   0        0        0     2278 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/lib/configuration.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.676860 arklibrary-0.0.9/src/arklibrary/tools/
+-rw-rw-rw-   0        0        0        2 2021-10-15 20:23:29.000000 arklibrary-0.0.9/src/arklibrary/tools/__init__.py
+-rw-rw-rw-   0        0        0     2831 2021-10-05 00:32:43.000000 arklibrary-0.0.9/src/arklibrary/tools/ark_generic_scraper.py
+-rw-rw-rw-   0        0        0    14575 2021-10-13 20:49:49.000000 arklibrary-0.0.9/src/arklibrary/tools/ark_image_scraper.py
+-rw-rw-rw-   0        0        0     4478 2021-09-24 02:58:55.000000 arklibrary-0.0.9/src/arklibrary/tools/clipboard.py
+-rw-rw-rw-   0        0        0      956 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/tools/config.py
+-rw-rw-rw-   0        0        0     1196 2021-09-24 02:57:41.000000 arklibrary-0.0.9/src/arklibrary/tools/read.py
+drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.642859 arklibrary-0.0.9/src/arklibrary.egg-info/
+-rw-rw-rw-   0        0        0      662 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1776 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/top_level.txt
```

### Comparing `arklibrary-0.0.8/LICENSE` & `arklibrary-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/PKG-INFO` & `arklibrary-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arklibrary-0.0.8/pyproject.toml` & `arklibrary-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/setup.cfg` & `arklibrary-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6c69 6272 6172 790d 0a76   = arklibrary..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
 00000030: 6175 7468 6f72 203d 204d 6175 7269 6369  author = Maurici
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 6465 762e 6d61 7572 6963 696f 2e6c  = dev.mauricio.l
 00000060: 6f6d 656c 6940 676d 6169 6c2e 636f 6d0d  omeli@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 00000080: 6869 7320 6170 706c 6963 6174 696f 6e20  his application 
 00000090: 6163 6365 7373 6573 2074 6865 2041 726b  accesses the Ark
```

### Comparing `arklibrary-0.0.8/src/arklibrary/admin/admin.py` & `arklibrary-0.0.9/src/arklibrary/admin/admin.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/admin/bundle.py` & `arklibrary-0.0.9/src/arklibrary/admin/bundle.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/admin/commands.py` & `arklibrary-0.0.9/src/arklibrary/admin/commands.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/admin/run_driver.py` & `arklibrary-0.0.9/src/arklibrary/admin/run_driver.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/__init__.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/ammunitions.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/ammunitions.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/armours.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/armours.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/artifacts.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/artifacts.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/beacons.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/beacons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/chibis.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/chibis.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/colors.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/colors.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/commands.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/commands.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/consumables.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/consumables.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/creatures.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/creatures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/dyes.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/dyes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/eggs.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/eggs.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/farming.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/farming.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/recipes.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/recipes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/resources.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/resources.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/saddles.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/saddles.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/seeds.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/seeds.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/skins.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/skins.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/structures.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/structures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/tools.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/tools.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/trophies.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/trophies.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/blueprints/weapons.py` & `arklibrary-0.0.9/src/arklibrary/blueprints/weapons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/data_structures/encoder.py` & `arklibrary-0.0.9/src/arklibrary/data_structures/encoder.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/data_structures/stream.py` & `arklibrary-0.0.9/src/arklibrary/data_structures/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         attrs = defaultdict(lambda: None)
         attrs.update(kwargs)
         self.from_address = attrs['from_address']
         self.to_address = attrs['to_address']
         self.authentication = attrs['authentication']
         self.expiration = attrs['expiration']
         self.body = attrs['body']
+        self.function = attrs['function']
+        self.type = attrs['type']
 
     def keys(self):
         return self.__dict__.keys()
 
     def items(self):
         return self.__dict__.items()
```

### Comparing `arklibrary-0.0.8/src/arklibrary/data_structures/tri.py` & `arklibrary-0.0.9/src/arklibrary/data_structures/tri.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/events/events.py` & `arklibrary-0.0.9/src/arklibrary/events/events.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/lib/configuration.py` & `arklibrary-0.0.9/src/arklibrary/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/tools/ark_generic_scraper.py` & `arklibrary-0.0.9/src/arklibrary/tools/ark_generic_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/tools/ark_image_scraper.py` & `arklibrary-0.0.9/src/arklibrary/tools/ark_image_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/tools/clipboard.py` & `arklibrary-0.0.9/src/arklibrary/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/tools/config.py` & `arklibrary-0.0.9/src/arklibrary/tools/config.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary/tools/read.py` & `arklibrary-0.0.9/src/arklibrary/tools/read.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.8/src/arklibrary.egg-info/PKG-INFO` & `arklibrary-0.0.9/src/arklibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arklibrary-0.0.8/src/arklibrary.egg-info/SOURCES.txt` & `arklibrary-0.0.9/src/arklibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

