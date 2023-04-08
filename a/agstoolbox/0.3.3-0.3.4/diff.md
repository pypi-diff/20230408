# Comparing `tmp/agstoolbox-0.3.3.tar.gz` & `tmp/agstoolbox-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agstoolbox-0.3.3.tar", last modified: Sat Apr  8 18:15:19 2023, max compression
+gzip compressed data, was "agstoolbox-0.3.4.tar", last modified: Sat Apr  8 20:10:48 2023, max compression
```

## Comparing `agstoolbox-0.3.3.tar` & `agstoolbox-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.246066 agstoolbox-0.3.3/
--rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/AUTHORS
--rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/COPYING
--rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       86 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1189 2023-04-08 18:15:19.245068 agstoolbox-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.3/README.rst
--rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/agstoolbox
--rw-rw-rw-   0        0        0      400 2023-04-08 03:13:15.000000 agstoolbox-0.3.3/atbx
--rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 18:15:19.246066 agstoolbox-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-08 03:22:46.000000 agstoolbox-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.141407 agstoolbox-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.161407 agstoolbox-0.3.3/src/agstoolbox/
--rw-rw-rw-   0        0        0      198 2023-04-08 18:13:25.000000 agstoolbox-0.3.3/src/agstoolbox/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-04-08 04:29:56.000000 agstoolbox-0.3.3/src/agstoolbox/__main__.py
--rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.3/src/agstoolbox/at_icons.py
--rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.3/src/agstoolbox/at_tasks.py
--rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.3/src/agstoolbox/at_trayindicator.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.208067 agstoolbox-0.3.3/src/agstoolbox/data/
--rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_ags_editor_icon.png
--rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_ags_engine_icon.png
--rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_icon.png
--rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.3/src/agstoolbox/data/at_icon_big.png
--rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.3/src/agstoolbox/data/exit_icon.png
--rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.3/src/agstoolbox/data/refresh_icon.png
--rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.3/src/agstoolbox/data/settings_icon.png
--rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.3/src/agstoolbox/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.177406 agstoolbox-0.3.3/src/agstoolbox.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 18:15:19.000000 agstoolbox-0.3.3/src/agstoolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 18:15:19.244067 agstoolbox-0.3.3/tests/
--rw-rw-rw-   0        0        0     1827 2022-01-29 21:31:17.000000 agstoolbox-0.3.3/tests/test_ags.py
--rw-rw-rw-   0        0        0     1664 2023-04-03 02:26:20.000000 agstoolbox-0.3.3/tests/test_gh.py
--rw-rw-rw-   0        0        0     1737 2023-04-05 23:37:44.000000 agstoolbox-0.3.3/tests/test_pe.py
--rw-rw-rw-   0        0        0     4315 2023-04-07 02:30:24.000000 agstoolbox-0.3.3/tests/test_settings_utils.py
--rw-rw-rw-   0        0        0     1255 2023-04-05 23:35:27.000000 agstoolbox-0.3.3/tests/test_time.py
--rw-rw-rw-   0        0        0     2894 2023-04-05 23:34:14.000000 agstoolbox-0.3.3/tests/test_utils.py
--rw-rw-rw-   0        0        0     3747 2023-04-06 00:01:05.000000 agstoolbox-0.3.3/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.734413 agstoolbox-0.3.4/
+-rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/AUTHORS
+-rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/COPYING
+-rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1189 2023-04-08 20:10:48.734413 agstoolbox-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.4/README.rst
+-rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/agstoolbox
+-rw-rw-rw-   0        0        0      400 2023-04-08 03:13:15.000000 agstoolbox-0.3.4/atbx
+-rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 20:10:48.734413 agstoolbox-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1669 2023-04-08 20:09:20.000000 agstoolbox-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.449090 agstoolbox-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.468094 agstoolbox-0.3.4/src/agstoolbox/
+-rw-rw-rw-   0        0        0      198 2023-04-08 18:39:28.000000 agstoolbox-0.3.4/src/agstoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1017 2023-04-08 04:29:56.000000 agstoolbox-0.3.4/src/agstoolbox/__main__.py
+-rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.4/src/agstoolbox/at_icons.py
+-rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.4/src/agstoolbox/at_tasks.py
+-rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.4/src/agstoolbox/at_trayindicator.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.483344 agstoolbox-0.3.4/src/agstoolbox/core/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.4/src/agstoolbox/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.520167 agstoolbox-0.3.4/src/agstoolbox/core/ags/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/__init__.py
+-rw-rw-rw-   0        0        0      334 2022-03-20 16:55:45.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/ags_editor.py
+-rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/ags_editor_validation_data.py
+-rw-rw-rw-   0        0        0      385 2022-04-27 23:52:03.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/ags_local_run.py
+-rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/game_project.py
+-rw-rw-rw-   0        0        0     3086 2023-04-08 16:50:10.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/get_game_projects.py
+-rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/get_local_ags_editors.py
+-rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.4/src/agstoolbox/core/ags/validate_ags_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.537167 agstoolbox-0.3.4/src/agstoolbox/core/cmdline/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.4/src/agstoolbox/core/cmdline/__init__.py
+-rw-rw-rw-   0        0        0    10551 2023-04-08 17:04:31.000000 agstoolbox-0.3.4/src/agstoolbox/core/cmdline/cmdline.py
+-rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.4/src/agstoolbox/core/cmdline/cmdline_download.py
+-rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.4/src/agstoolbox/core/cmdline/progress.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.559168 agstoolbox-0.3.4/src/agstoolbox/core/gh/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/core/gh/__init__.py
+-rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.4/src/agstoolbox/core/gh/download_release.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 02:15:27.000000 agstoolbox-0.3.4/src/agstoolbox/core/gh/install_release.py
+-rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.4/src/agstoolbox/core/gh/list_releases.py
+-rw-rw-rw-   0        0        0      530 2023-04-08 02:43:46.000000 agstoolbox-0.3.4/src/agstoolbox/core/gh/release.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.576167 agstoolbox-0.3.4/src/agstoolbox/core/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.4/src/agstoolbox/core/settings/__init__.py
+-rw-rw-rw-   0        0        0     5541 2023-04-08 16:42:31.000000 agstoolbox-0.3.4/src/agstoolbox/core/settings/settings.py
+-rw-rw-rw-   0        0        0      289 2023-04-07 02:07:43.000000 agstoolbox-0.3.4/src/agstoolbox/core/settings/settings_data.py
+-rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.4/src/agstoolbox/core/settings/settings_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.639167 agstoolbox-0.3.4/src/agstoolbox/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/basics.py
+-rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/downloader.py
+-rw-rw-rw-   0        0        0     4237 2023-04-08 03:40:39.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/file.py
+-rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/math.py
+-rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/open_in_browser.py
+-rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/pe.py
+-rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/singleton.py
+-rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/startup.py
+-rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/systemdirs.py
+-rw-rw-rw-   0        0        0     1008 2023-04-05 23:29:30.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/time.py
+-rw-rw-rw-   0        0        0     1256 2023-04-03 01:20:15.000000 agstoolbox-0.3.4/src/agstoolbox/core/utils/win_registry.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.649166 agstoolbox-0.3.4/src/agstoolbox/core/version/
+-rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.4/src/agstoolbox/core/version/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.4/src/agstoolbox/core/version/version.py
+-rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.4/src/agstoolbox/core/version/version_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.653245 agstoolbox-0.3.4/src/agstoolbox/data/
+-rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.4/src/agstoolbox/data/at_ags_editor_icon.png
+-rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/data/at_ags_engine_icon.png
+-rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.4/src/agstoolbox/data/at_icon.png
+-rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.4/src/agstoolbox/data/at_icon_big.png
+-rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.4/src/agstoolbox/data/exit_icon.png
+-rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.4/src/agstoolbox/data/refresh_icon.png
+-rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.4/src/agstoolbox/data/settings_icon.png
+-rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.670413 agstoolbox-0.3.4/src/agstoolbox/panels/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/panels/__init__.py
+-rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.4/src/agstoolbox/panels/at_mainpanel.py
+-rw-rw-rw-   0        0        0     7540 2023-04-07 03:11:46.000000 agstoolbox-0.3.4/src/agstoolbox/panels/at_settings_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.680413 agstoolbox-0.3.4/src/agstoolbox/system/
+-rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.4/src/agstoolbox/system/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.4/src/agstoolbox/system/at_runguard.py
+-rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.4/src/agstoolbox/system/at_unique_application.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.713413 agstoolbox-0.3.4/src/agstoolbox/wdgts/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/__init__.py
+-rw-rw-rw-   0        0        0     7388 2023-04-07 02:54:37.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_dirlist_wdgt.py
+-rw-rw-rw-   0        0        0     2528 2023-04-07 02:54:50.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_single_dir_wdgt.py
+-rw-rw-rw-   0        0        0     5943 2022-04-27 23:52:03.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_tree_item_project.py
+-rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_tree_item_tool.py
+-rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
+-rw-rw-rw-   0        0        0     6505 2023-04-05 02:02:50.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.733414 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/
+-rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/action_utils.py
+-rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/ags_local_extra.py
+-rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/file_explorer.py
+-rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.4/src/agstoolbox/wdgts_utils/get_self_path.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:10:48.483344 agstoolbox-0.3.4/src/agstoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-04-08 20:10:48.000000 agstoolbox-0.3.4/src/agstoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2942 2023-04-08 20:10:48.000000 agstoolbox-0.3.4/src/agstoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 20:10:48.000000 agstoolbox-0.3.4/src/agstoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-08 20:10:48.000000 agstoolbox-0.3.4/src/agstoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 20:10:48.000000 agstoolbox-0.3.4/src/agstoolbox.egg-info/top_level.txt
```

### Comparing `agstoolbox-0.3.3/COPYING` & `agstoolbox-0.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/LICENSE` & `agstoolbox-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/PKG-INFO` & `agstoolbox-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.3
+Version: 0.3.4
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.3
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.4
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.3/README.rst` & `agstoolbox-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/pyproject.toml` & `agstoolbox-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/__main__.py` & `agstoolbox-0.3.4/src/agstoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/at_icons.py` & `agstoolbox-0.3.4/src/agstoolbox/at_icons.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/at_tasks.py` & `agstoolbox-0.3.4/src/agstoolbox/at_tasks.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/at_trayindicator.py` & `agstoolbox-0.3.4/src/agstoolbox/at_trayindicator.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/at_ags_editor_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/at_ags_editor_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/at_ags_engine_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/at_ags_engine_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/at_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/at_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/at_icon_big.png` & `agstoolbox-0.3.4/src/agstoolbox/data/at_icon_big.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/exit_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/exit_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/refresh_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/refresh_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/data/settings_icon.png` & `agstoolbox-0.3.4/src/agstoolbox/data/settings_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox/getdata.py` & `agstoolbox-0.3.4/src/agstoolbox/getdata.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.3/src/agstoolbox.egg-info/PKG-INFO` & `agstoolbox-0.3.4/src/agstoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.3
+Version: 0.3.4
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.3
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.4
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

