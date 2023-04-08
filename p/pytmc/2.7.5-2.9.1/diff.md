# Comparing `tmp/pytmc-2.7.5.tar.gz` & `tmp/pytmc-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytmc-2.7.5.tar", last modified: Wed Sep  2 15:34:06 2020, max compression
+gzip compressed data, was "dist/pytmc-2.9.1.tar", last modified: Tue Apr 27 21:16:50 2021, max compression
```

## Comparing `pytmc-2.7.5.tar` & `pytmc-2.9.1.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/
--rw-r--r--   0 klauer   (1318172782) 1704612529     2499 2019-01-09 21:05:14.000000 pytmc-2.7.5/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      134 2020-08-28 21:14:15.000000 pytmc-2.7.5/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529     1015 2020-09-02 15:34:06.000000 pytmc-2.7.5/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      623 2019-02-20 21:28:59.000000 pytmc-2.7.5/README.rst
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/
--rw-r--r--   0 klauer   (1318172782) 1704612529      370 2019-08-14 19:25:46.000000 pytmc-2.7.5/pytmc/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      466 2019-04-17 18:47:18.000000 pytmc-2.7.5/pytmc/beckhoff.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/benchmark/
--rw-r--r--   0 klauer   (1318172782) 1704612529       44 2020-08-29 00:20:56.000000 pytmc-2.7.5/pytmc/benchmark/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2519 2020-08-28 22:56:50.000000 pytmc-2.7.5/pytmc/benchmark/profile.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3043 2020-08-28 22:56:08.000000 pytmc-2.7.5/pytmc/benchmark/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/bin/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2019-03-19 17:49:42.000000 pytmc-2.7.5/pytmc/bin/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1799 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/bin/code.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9111 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/bin/db.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11593 2019-12-19 19:09:48.000000 pytmc-2.7.5/pytmc/bin/debug.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5068 2019-09-16 23:11:41.000000 pytmc-2.7.5/pytmc/bin/iocboot.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9947 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/bin/pragmalint.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2289 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/bin/pytmc.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9392 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/bin/stcmd.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    12287 2020-08-28 23:08:24.000000 pytmc-2.7.5/pytmc/bin/summary.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4092 2019-08-14 19:25:46.000000 pytmc-2.7.5/pytmc/bin/types.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1442 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/bin/util.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1883 2019-08-14 19:25:46.000000 pytmc-2.7.5/pytmc/bin/xmltranslate.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5707 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/code.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/default_settings/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2019-12-06 23:09:51.000000 pytmc-2.7.5/pytmc/default_settings/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7109 2019-12-06 23:09:51.000000 pytmc-2.7.5/pytmc/default_settings/unified_ordered_field_list.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      240 2019-04-17 18:47:18.000000 pytmc-2.7.5/pytmc/defaults.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4666 2020-06-04 23:55:10.000000 pytmc-2.7.5/pytmc/linter.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    54813 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/parser.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    20507 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/pragmas.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    27293 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/record.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/templates/
--rw-r--r--   0 klauer   (1318172782) 1704612529      211 2019-01-09 21:05:14.000000 pytmc-2.7.5/pytmc/templates/EPICS_proto_template.proto
--rw-r--r--   0 klauer   (1318172782) 1704612529       42 2019-01-09 21:05:14.000000 pytmc-2.7.5/pytmc/templates/asyn_standard_file.jinja2
--rw-r--r--   0 klauer   (1318172782) 1704612529      966 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/templates/asyn_standard_record.jinja2
--rw-r--r--   0 klauer   (1318172782) 1704612529     3981 2020-08-28 21:14:15.000000 pytmc-2.7.5/pytmc/templates/stcmd_default.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2109 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/conftest.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2655 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_archive.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2486 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_commandline.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2204 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_integrations.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3940 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_lint.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1090 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_motion.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6949 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_parsing.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1193 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_project.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1668 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_record.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    16897 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_xml_collector.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7929 2020-09-02 15:34:04.000000 pytmc-2.7.5/pytmc/tests/test_xml_obj.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc/validation/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2019-01-09 21:05:14.000000 pytmc-2.7.5/pytmc/validation/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2019-01-09 21:05:14.000000 pytmc-2.7.5/pytmc/validation/v0.1.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1015 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1372 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       48 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       24 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        6 2020-09-02 15:34:06.000000 pytmc-2.7.5/pytmc.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       24 2020-06-11 18:05:28.000000 pytmc-2.7.5/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      169 2020-09-02 15:34:06.000000 pytmc-2.7.5/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1313 2019-12-06 23:09:51.000000 pytmc-2.7.5/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2019-01-09 21:05:14.000000 pytmc-2.7.5/versioneer.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2499 2021-04-27 21:16:44.000000 pytmc-2.9.1/LICENSE
+-rw-r--r--   0 klauer   (1318172782) 1704612529      134 2021-04-27 21:16:44.000000 pytmc-2.9.1/MANIFEST.in
+-rw-r--r--   0 klauer   (1318172782) 1704612529      857 2021-04-27 21:16:50.000000 pytmc-2.9.1/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529      489 2021-04-27 21:16:44.000000 pytmc-2.9.1/README.rst
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      370 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      497 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/_version.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      466 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/beckhoff.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/bin/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1799 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/code.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     9605 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/db.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    12505 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/debug.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5068 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/iocboot.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10005 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/pragmalint.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2300 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/pytmc.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     9392 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/stcmd.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    12287 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/summary.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    15939 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/template.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4092 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/types.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1442 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/util.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1883 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/bin/xmltranslate.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5707 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/code.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/default_settings/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/default_settings/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     7109 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/default_settings/unified_ordered_field_list.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      240 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/defaults.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4741 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/linter.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    58421 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/parser.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    26088 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/pragmas.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    29533 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/record.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/templates/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      211 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/templates/EPICS_proto_template.proto
+-rw-r--r--   0 klauer   (1318172782) 1704612529       42 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/templates/asyn_standard_file.jinja2
+-rw-r--r--   0 klauer   (1318172782) 1704612529      966 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/templates/asyn_standard_record.jinja2
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3981 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/templates/stcmd_default.cmd
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/tests/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2109 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/conftest.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2655 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_archive.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     4077 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_commandline.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2204 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_integrations.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3940 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_lint.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2187 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_motion.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     6949 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_parsing.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1193 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_project.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1668 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_record.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    25155 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_xml_collector.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     7929 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/tests/test_xml_obj.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc/validation/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/validation/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:44.000000 pytmc-2.9.1/pytmc/validation/v0.1.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      857 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1314 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/SOURCES.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        1 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/dependency_links.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       48 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/entry_points.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       31 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/requires.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        6 2021-04-27 21:16:50.000000 pytmc-2.9.1/pytmc.egg-info/top_level.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       31 2021-04-27 21:16:44.000000 pytmc-2.9.1/requirements.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529      169 2021-04-27 21:16:50.000000 pytmc-2.9.1/setup.cfg
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1313 2021-04-27 21:16:44.000000 pytmc-2.9.1/setup.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2021-04-27 21:16:44.000000 pytmc-2.9.1/versioneer.py
```

### Comparing `pytmc-2.7.5/LICENSE` & `pytmc-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/code.py` & `pytmc-2.9.1/pytmc/bin/code.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/db.py` & `pytmc-2.9.1/pytmc/bin/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,29 @@
 
         ex = LinterError(message)
         if not allow_errors:
             raise ex
         exceptions.append(ex)
         logger.error(message)
 
+    too_long = [record_name for record_name in record_names
+                if len(record_name) > linter.MAX_RECORD_LENGTH]
+    if too_long:
+        message = '\n'.join(
+            [f'Records exceeding the maximum length of '
+             f'{linter.MAX_RECORD_LENGTH} were found:'] +
+            [f'    {record}' for record in too_long]
+        )
+
+        ex = LinterError(message)
+        if not allow_errors:
+            raise ex
+        exceptions.append(ex)
+        logger.error(message)
+
     if dbd_file is not None:
         results, rendered = validate_with_dbd(records, dbd_file)
         for warning in results.warnings:
             logger.warning('[%s line %s] %s', warning['file'], warning['line'],
                            warning['message'])
         for error in results.errors:
             logger.error('[%s line %s] %s', error['file'], error['line'],
```

### Comparing `pytmc-2.7.5/pytmc/bin/debug.py` & `pytmc-2.9.1/pytmc/bin/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import pathlib
 import sys
 
 from qtpy import QtWidgets
 from qtpy.QtCore import Qt, Signal
 
 import pytmc
-from .db import process
 
+from .db import process
 
 DESCRIPTION = __doc__
 logger = logging.getLogger(__name__)
 
 
 def _grep_record_names(text):
     if not text:
         return []
 
-    records = [line.rstrip('{')
+    records = [line.rstrip('{ ')
                for line in text.splitlines()
                if line.startswith('record')   # regular line
                or line.startswith('. record')  # linted line
                or line.startswith('X record')  # linted error line
                ]
 
     def split_rtyp(line):
@@ -82,23 +82,23 @@
     ----------
     tmc : TmcFile
         The tmc file to inspect
     '''
 
     item_selected = Signal(object)
 
-    def __init__(self, tmc, dbd):
+    def __init__(self, tmc, dbd, allow_no_pragma=False):
         super().__init__()
         self.tmc = tmc
         self.chains = {}
         self.incomplete_chains = {}
         self.records = {}
 
         records, self.exceptions = process(tmc, allow_errors=True,
-                                           allow_no_pragma=True)
+                                           allow_no_pragma=allow_no_pragma)
 
         for record in records:
             if not record.valid:
                 self.incomplete_chains[record.tcname] = record
                 continue
 
             self.chains[record.tcname] = record
@@ -134,16 +134,18 @@
 
         self.item_view_type = QtWidgets.QComboBox()
         self.item_view_type.addItem('Chains')
         self.item_view_type.addItem('Records')
         self.item_view_type.addItem('Chains w/o Records')
         self.item_view_type.currentTextChanged.connect(self._update_view_type)
         self.item_list = QtWidgets.QListWidget()
+        self.item_list_filter = QtWidgets.QLineEdit()
 
         self.left_layout.addWidget(self.item_view_type)
+        self.left_layout.addWidget(self.item_list_filter)
         self.left_layout.addWidget(self.item_list)
 
         # Right part of the window
         self.right_frame = QtWidgets.QFrame()
         self.right_layout = QtWidgets.QVBoxLayout()
         self.right_frame.setLayout(self.right_layout)
 
@@ -178,14 +180,22 @@
         self.setCentralWidget(self.top_splitter)
         self.item_list.currentItemChanged.connect(self._item_selected)
 
         self.item_selected.connect(self._update_config_info)
         self.item_selected.connect(self._update_chain_info)
         self.item_selected.connect(self._update_record_text)
 
+        def set_filter(text):
+            text = text.strip().lower()
+            for idx in range(self.item_list.count()):
+                item = self.item_list.item(idx)
+                item.setHidden(bool(text and text not in item.text().lower()))
+
+        self.item_list_filter.textEdited.connect(set_filter)
+
         self._update_item_list()
 
     def _item_selected(self, current, previous):
         'Slot - new list item selected'
         if current is None:
             return
 
@@ -198,14 +208,15 @@
             self.item_selected.emit(record)
 
     def _update_config_info(self, record):
         'Slot - update config information when a new record is selected'
         chain = record.chain
 
         self.config_info.clear()
+        self.item_list_filter.setText('')
         self.config_info.setRowCount(len(chain.chain))
 
         def add_dict_to_table(row: int, d: dict):
             """
             Parameters
             ----------
             row : int
@@ -296,33 +307,37 @@
         for name, record in sorted(items,
                                    key=lambda item: item[0]):
             item = QtWidgets.QListWidgetItem(name)
             item.setData(Qt.UserRole, record)
             self.item_list.addItem(item)
 
 
-def create_debug_gui(tmc, dbd=None):
+def create_debug_gui(tmc, dbd=None, allow_no_pragma=False):
     '''
-    Show the results of tmc processing in a Qt gui
+    Show the results of tmc processing in a Qt gui.
 
     Parameters
     ----------
     tmc : TmcFile, str, pathlib.Path
-        The tmc file to show
+        The tmc file to show.
+
     dbd : DbdFile, optional
-        The dbd file to lint against
+        The dbd file to lint against.
+
+    allow_no_pragma : bool, optional
+        Look for chains that have missing pragmas.
     '''
 
     if isinstance(tmc, (str, pathlib.Path)):
         tmc = pytmc.parser.parse(tmc)
 
     if dbd is not None and not isinstance(dbd, pytmc.linter.DbdFile):
         dbd = pytmc.linter.DbdFile(dbd)
 
-    return TmcSummary(tmc, dbd)
+    return TmcSummary(tmc, dbd, allow_no_pragma=allow_no_pragma)
 
 
 def build_arg_parser(parser=None):
     if parser is None:
         parser = argparse.ArgumentParser()
 
     parser.description = DESCRIPTION
@@ -337,15 +352,22 @@
         '-d', '--dbd',
         default=None,
         type=str,
         help=('Specify an expanded .dbd file for validating fields '
               '(requires pyPDB)')
     )
 
+    parser.add_argument(
+        '-a', '--allow-no-pragma',
+        action='store_true',
+        help='Show all items, even those missing pragmas (warning: slow)',
+    )
+
     return parser
 
 
-def main(tmc_file, *, dbd=None):
+def main(tmc_file, *, dbd=None, allow_no_pragma=False):
     app = QtWidgets.QApplication([])
-    interface = create_debug_gui(tmc_file, dbd)
+    interface = create_debug_gui(tmc_file, dbd,
+                                 allow_no_pragma=allow_no_pragma)
     interface.show()
     sys.exit(app.exec_())
```

### Comparing `pytmc-2.7.5/pytmc/bin/iocboot.py` & `pytmc-2.9.1/pytmc/bin/iocboot.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/pragmalint.py` & `pytmc-2.9.1/pytmc/bin/pragmalint.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         yield match.start(0), match_single_pragma(code[match.start(0):])
 
 
 def lint_pragma(pragma):
     '''
     Lint a pragma against the PRAGMA_RE regular expression. Raises LinterError
     '''
-    if 'pytmc' not in pragma:
+    if pragma is None or 'pytmc' not in pragma:
         return
 
     pragma = pragma.strip()
     match = PRAGMA_RE.match(pragma)
     if not match:
         raise LinterError()
 
@@ -269,32 +269,34 @@
         for i, plc in enumerate(project.plcs, 1):
             util.heading(f'PLC Project ({i}): {plc.project_path.stem}')
             for fn, source in plc.source.items():
                 for info in lint_source(fn, source, verbose=verbose):
                     pragma_count += 1
                     if info.exception is not None:
                         linter_errors += 1
-                        logger.error('Linter error: %s\n%s:line %s: %s',
-                                     info.exception, info.filename,
-                                     info.line_number,
-                                     textwrap.indent(info.pragma, '    '))
+                        logger.error(
+                            'Linter error: %s\n%s:line %s: %s',
+                            info.exception, info.filename,
+                            info.line_number,
+                            textwrap.indent(info.pragma or '', '    '),
+                        )
                         if hasattr(info.exception, 'original_ex'):
                             logger.error(
                                 'Unhandled exception (may be a pytmc bug)',
                                 exc_info=info.exception.original_ex
                             )
     else:
         source = project
         for info in lint_source(filename, source, verbose=verbose):
             pragma_count += 1
             if info.exception is not None:
                 linter_errors += 1
                 logger.error('Linter error: %s\n%s:line %s: %s',
                              info.exception, info.filename, info.line_number,
-                             textwrap.indent(info.pragma, '    '))
+                             textwrap.indent(info.pragma or '', '    '))
                 if hasattr(info.exception, 'original_ex'):
                     logger.error(
                         'Unhandled exception (may be a pytmc bug)',
                         exc_info=info.exception.original_ex
                     )
 
     logger.info('Total pragmas found: %d Total linter errors: %d',
```

### Comparing `pytmc-2.7.5/pytmc/bin/pytmc.py` & `pytmc-2.9.1/pytmc/bin/pytmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 
 import argparse
 import importlib
 import logging
 
 import pytmc
 
-
 DESCRIPTION = __doc__
 
 
 MODULES = ('summary', 'stcmd', 'db', 'xmltranslate', 'debug', 'types',
-           'iocboot', 'pragmalint', 'code')
+           'iocboot', 'pragmalint', 'code', 'template')
 
 
 def _try_import(module):
     relative_module = f'.{module}'
     return importlib.import_module(relative_module, 'pytmc.bin')
```

### Comparing `pytmc-2.7.5/pytmc/bin/stcmd.py` & `pytmc-2.9.1/pytmc/bin/stcmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 import argparse
 import getpass
 import logging
 import pathlib
 
 import jinja2
 
-from . import db, util
 from .. import pragmas
-
-from ..parser import parse, Symbol, separate_by_classname, NC
-
+from ..parser import NC, Symbol, parse, separate_by_classname
+from . import db, util
 
 DESCRIPTION = __doc__
 logger = logging.getLogger(__name__)
 
 
 def build_arg_parser(parser=None):
     if parser is None:
@@ -134,15 +132,15 @@
     item_and_config = pragmas.expand_configurations_from_chain([obj])
     delim = user_config['delim']
     prefix = user_config['prefix']
     if item_and_config:
         item_to_config = dict(item_and_config[0])
         config = pragmas.squash_configs(*item_to_config.values())
         # PV name specified in the pragma - use it as-is
-        if 'pv' in config:
+        if config.get('pv'):
             pv = delim.join(config['pv'])
             if delim in pv:
                 pv_parts = pv.split(delim)
                 # Break the PV parts into a prefix and suffix, using all but
                 # the last section as the prefix.
                 prefix = delim.join(pv_parts[:-1]) + delim
                 suffix = pv_parts[-1]
```

### Comparing `pytmc-2.7.5/pytmc/bin/summary.py` & `pytmc-2.9.1/pytmc/bin/summary.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/types.py` & `pytmc-2.9.1/pytmc/bin/types.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/util.py` & `pytmc-2.9.1/pytmc/bin/util.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/bin/xmltranslate.py` & `pytmc-2.9.1/pytmc/bin/xmltranslate.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/code.py` & `pytmc-2.9.1/pytmc/code.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/default_settings/unified_ordered_field_list.py` & `pytmc-2.9.1/pytmc/default_settings/unified_ordered_field_list.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/linter.py` & `pytmc-2.9.1/pytmc/linter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
+
 import pyPDB.dbd.yacc as _yacc
 import pyPDB.dbdlint as _dbdlint
 from pyPDB.dbdlint import DBSyntaxError
 
+MAX_RECORD_LENGTH = int(os.environ.get('EPICS_MAX_RECORD_LENGTH', '60'))
+
 
 class LinterResults(_dbdlint.Results):
     '''
     Container for dbdlint results, with easier-to-access attributes
 
     Extends pyPDB.dbdlint.Results
```

### Comparing `pytmc-2.7.5/pytmc/parser.py` & `pytmc-2.9.1/pytmc/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import collections
 import logging
 import os
 import pathlib
 import re
 import types
 import typing
+from typing import Optional, Union
 
 import lxml
 import lxml.etree
 
 from .code import (determine_block_type, get_pou_call_blocks,
                    program_name_from_declaration, variables_from_declaration)
 
@@ -924,14 +925,19 @@
             raise AttributeError('GUID unavailable') from None
 
     @property
     def qualified_type_name(self):
         namespace = self.namespace
         return f'{namespace}.{self.text}' if namespace else self.text
 
+    @property
+    def type_name(self):
+        """The type name, without a namespace."""
+        return self.text
+
 
 class BaseType(Type):
     '[TMC] A reference to the data type of a symbol'
     # Inherits everything from :class:`Type`
 
 
 class DataType(_TmcItem):
@@ -1743,14 +1749,42 @@
 
 
 class Box(_IoTreeItem):
     '[XTI] A box / module'
     _load_path_hint = USE_NAME_AS_PATH
 
 
+class EtherCAT(TwincatItem):
+    """
+    EtherCAT information for a given Box.
+
+    Contains SyncMan, Fmmu, DcMode, Pdo, etc.
+    """
+    ...
+
+
+class Pdo(TwincatItem):
+    """Process data objects, part of an EtherCAT block."""
+    ...
+
+
+class Entry(TwincatItem):
+    """Pdo Entry, containing name and type information."""
+
+    @property
+    def entry_type(self) -> typing.Optional[Type]:
+        """The type of the entry."""
+        return getattr(self, 'Type', [None])[0]
+
+    @property
+    def comment(self) -> str:
+        """The comment associated with the entry."""
+        return self.Comment[0].text if hasattr(self, 'Comment') else ''
+
+
 class RemoteConnections(TwincatItem):
     '[StaticRoutes] Routes contained in the TwinCat configuration'
     def post_init(self):
         def to_dict(child):
             return {
                 item.tag: item.text
                 for item in child._children
@@ -1764,14 +1798,117 @@
             }
 
         self.by_name = keyed_on('Name')
         self.by_address = keyed_on('Address')
         self.by_ams_id = keyed_on('NetId')
 
 
+class Resolution(TwincatItem):
+    """Library version resolution."""
+    @property
+    def resolution(self):
+        if not self.text:
+            return {}
+
+        return Resolution.split_resolution(self.text)
+
+    @staticmethod
+    def split_resolution(text):
+        library_name, version_and_vendor = text.split(',')
+        version, vendor = version_and_vendor.strip().split('(')
+        vendor = vendor.rstrip(')')
+        version = version.strip()
+
+        return {
+            'name': library_name,
+            'vendor': vendor,
+            'version': version,
+            'vendor_short': vendor.split(' ')[0] if ' ' in vendor else vendor,
+         }
+
+
+class DefaultResolution(Resolution):
+    """Library default version resolution."""
+
+
+class _VersionItemMixin:
+    @property
+    def resolution(self) -> Optional[Union[DefaultResolution, Resolution]]:
+        try:
+            resolution, = self.Resolution
+        except AttributeError:
+            try:
+                resolution, = self.DefaultResolution
+            except AttributeError:
+                resolution = None
+        return resolution
+
+    @property
+    def full_include_name(self) -> str:
+        if hasattr(self, 'Namespace'):
+            namespace, = self.Namespace
+            return f'{namespace.namespace}.{self.include_name}'
+
+        return self.include_name
+
+    @property
+    def include_name(self) -> str:
+        return self.attributes['Include']
+
+    def get_resolution_info(self):
+        resolution = self.resolution
+        resolution_info = (
+            resolution.resolution if resolution is not None else {}
+        )
+        return {
+            'resolution': resolution,
+            'name': self.include_name,
+            'full_name': self.full_include_name,
+            **resolution_info
+        }
+
+
+class PlaceholderReference(TwincatItem, _VersionItemMixin):
+    """Library placeholder reference."""
+
+
+class PlaceholderResolution(TwincatItem, _VersionItemMixin):
+    """Library placeholder resolution."""
+
+
+class LibraryReference(TwincatItem, _VersionItemMixin):
+    """Library reference."""
+
+    def get_resolution_info(self):
+        if ',' not in self.include_name:
+            # Unknown
+            return {}
+
+        name, version, vendor = self.include_name.split(',')
+        full_name = self.full_include_name
+        if ',' in full_name:
+            full_name = full_name.split(',')[0]
+
+        return {
+            'resolution': None,
+            'full_name': full_name,
+            'name': name,
+            'version': version,
+            'vendor': vendor,
+            'vendor_short': vendor.split(' ')[0] if ' ' in vendor else vendor,
+        }
+
+
+class Namespace(TwincatItem):
+    """Type / library namespace information."""
+    @property
+    def namespace(self) -> str:
+        return self.text
+
+
 class _ArrayItemProxy:
     '''
     A TwincatItem proxy that represents a single element of an array value.
 
     Adjusts 'name' such that access from EPICS will refer to the correct index.
 
     Parameters
```

### Comparing `pytmc-2.7.5/pytmc/pragmas.py` & `pytmc-2.9.1/pytmc/pragmas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This file contains the objects for taking in pytmc-parsed TMC files and
 generating Python-level configuration information.
 """
+import copy
 import itertools
 import logging
 import math
 import re
 from typing import Generator, Type, Union
 
 from . import parser
@@ -46,14 +47,22 @@
     r'^(?P<rate>\d*\.\d+|\d+)\s*(?P<hz_or_sec>hz|s)'
     # Poll or notify (or default)
     r'(\s+(?P<method>scan|monitor))?$',
     flags=re.IGNORECASE
 )
 ARCHIVE_DEFAULT = {'frequency': 1, 'seconds': 1, 'method': 'scan'}
 
+# Special, reserved keys:
+SUBITEM = '_subitem_'
+PRAGMA = '_pragma_'
+DISALLOWED_SUBITEMS = {'pv', SUBITEM, PRAGMA, 'field', 'link'}
+
+# Default for array index expansion:
+EXPAND_DEFAULT = ':%.2d'
+
 
 def split_pytmc_pragma(pragma_text):
     """
     Return dictionaries for each line.
     Derived from raw_config
 
     Parameters
@@ -154,15 +163,22 @@
         if config is not None:
             config.append(line)
 
     if config is not None:
         yield pv, config
 
 
-def dictify_config(conf, array_index=None, expand_default=':%.2d'):
+def get_array_suffix(config, array_index, *, default=EXPAND_DEFAULT):
+    '''
+    Return array index suffix based on the expand settings in the config.
+    '''
+    return config.get('expand', default) % array_index
+
+
+def dictify_config(raw_conf, array_index=None):
     '''
     Make a raw config list into an easier-to-use dictionary
 
     Example::
         [{'title': 'pv', 'tag': 'a'},
          {'title': 'io', 'tag': 'io_for_a'},
          {'title': 'field', 'tag': {'f_name': 'fieldname', 'f_set': 'value'}},
@@ -171,30 +187,149 @@
     Becomes::
 
         {'pv': 'a',
          'io': 'io_for_a',
          'field': {'fieldname': 'value'}}
     '''
 
+    title_tag_pairs = [(item['title'], item['tag']) for item in raw_conf]
+
     fields = {
-        item['tag']['f_name']: item['tag']['f_set']
-        for item in conf
-        if item['title'] == 'field'
+        tag['f_name']: tag['f_set']
+        for title, tag in title_tag_pairs
+        if title == 'field'
+    }
+
+    config = {
+        title: tag
+        for title, tag in title_tag_pairs
+        if '.' not in title  # Handle subitem entries specially
     }
-    config = {item['title']: item['tag']
-              for item in conf}
+
     if fields:
         config['field'] = fields
 
     if array_index is not None:
-        config['pv'] += config.get('expand', expand_default) % array_index
+        config['pv'] += get_array_suffix(config, array_index)
+
+    def add_subitem(d, key, value):
+        """Add a subitem `key: value` to dictionary `d`."""
+        if '.' in key:
+            # The first a.b.c.pragma indicate the sub-(sub-) item for 'pragma':
+            child, remainder = key.split('.', 1)
+            if child not in d:
+                d[child] = {PRAGMA: []}
+            return add_subitem(d[child], remainder, value)
+
+        if key in DISALLOWED_SUBITEMS:
+            raise ValueError(f'Unsupported pragma key in subitem: {key}')
+        # The final key is a pytmc-supported pragma:
+        d[PRAGMA].append((key, value))
+
+    for title, tag in title_tag_pairs:
+        if '.' in title:
+            if SUBITEM not in config:
+                config[SUBITEM] = {}
+            add_subitem(config[SUBITEM], title, tag)
 
     return config
 
 
+def _merge_subitems(target: dict, source: dict):
+    """
+    In-place merge `source` into `target`.
+
+    Sub-item dictionaries, held at the top-level key ``_subitem_``, are nested
+    dictionaries containing sub-item names or the special key ``_pragma_``,
+    which can modify the pragma at the given level.
+
+    For example::
+
+        {'_subitem_': {'member1': {'_pragma_': [('key', '1')], ... }}}
+
+    This top-level _subitem_ pragma dictionary contains a pragma ``key: 1``
+    for the ".member1" member.  ``member1``, if structured, may also have
+    keys in its dictionary named after its members.
+    """
+    if PRAGMA not in target:
+        target[PRAGMA] = []
+
+    for key, value in source.items():
+        if key == PRAGMA:
+            target[PRAGMA].extend(value)
+        else:
+            if key not in target:
+                target[key] = {}
+            _merge_subitems(target[key], value)
+
+
+def _expand_configurations_from_chain(chain, *, pragma: str = 'pytmc',
+                                      allow_no_pragma=False):
+    """
+    Wrapped by ``expand_configurations_from_chain``, usable for callers that
+    don't want the full product of all configurations.
+    """
+
+    def handle_scalar(item, pvname, config):
+        """Handler for scalar simple or structured items."""
+        yield item, config
+
+    def handle_array_complex(item, pvname, config):
+        """Handler for arrays of structured items (or enums)."""
+        low, high = item.array_info.bounds
+        expand_digits = math.floor(math.log10(high)) + 2
+        array_element_pragma = config.get('array', '')
+        for idx in parse_array_settings(array_element_pragma, (low, high)):
+            # shallow-copy; only touching the top level "pv" key
+            idx_config = copy.copy(config)
+            idx_config['pv'] += get_array_suffix(
+                config, idx, default=f':%.{expand_digits}d')
+            yield parser._ArrayItemProxy(item, idx), idx_config
+
+    def get_all_options(subitems, handler, pragmas):
+        split_pragma = split_pytmc_pragma('\n'.join(pragmas))
+        for pvname, separated_cfg in separate_configs_by_pv(split_pragma):
+            config = dictify_config(separated_cfg)
+
+            # config will have the SUBITEM key, applicable to its level
+            # in the hierarchy. If it exists, merge it with our current set.
+            if SUBITEM in config:
+                _merge_subitems(subitems, config[SUBITEM])
+
+            for key, value in subitems.get(PRAGMA, []):
+                config[key] = value
+
+            yield from handler(item, pvname, config)
+
+    # `subitems` keeps track of forward references with pragmas of members
+    # and sub-members (and so on)
+    subitems = {}
+
+    for item in chain:
+        subitems = subitems.get(item.name, {})
+        pragmas = list(pragma for pragma in get_pragma(item, name=pragma)
+                       if pragma is not None)
+        if not pragmas:
+            if allow_no_pragma:
+                pragmas = [None]
+                yield [(item, None)]
+                continue
+
+            # If any pragma in the chain is unset, escape early
+            return []
+
+        if item.array_info and (item.data_type.is_complex_type or
+                                item.data_type.is_enum):
+            options = get_all_options(subitems, handle_array_complex, pragmas)
+        else:
+            options = get_all_options(subitems, handle_scalar, pragmas)
+
+        yield list(options)
+
+
 def expand_configurations_from_chain(chain, *, pragma: str = 'pytmc',
                                      allow_no_pragma=False):
     '''
     Generate all possible configuration combinations
 
     For example, from a chain with two items::
 
@@ -212,53 +347,20 @@
     individual elements.  That is, `arr : ARRAY [1..5] of ST_Structure` will be
     unrolled into `arr[1]` through `arr[5]`.
 
     Returns
     -------
     tuple
         Tuple of tuples. See description above.
-
     '''
-    result = []
-
-    def dictify_scalar(item):
-        for pvname, config in separate_configs_by_pv(
-                split_pytmc_pragma('\n'.join(pragmas))):
-            yield (item, dictify_config(config))
-
-    def dictify_complex_array(item):
-        low, high = item.array_info.bounds
-        expand_digits = math.floor(math.log10(high)) + 2
-        expand_default = f':%.{expand_digits}d'
-        for pvname, config in separate_configs_by_pv(
-                split_pytmc_pragma('\n'.join(pragmas))):
-            for idx in range(low, high + 1):
-                yield (parser._ArrayItemProxy(item, idx),
-                       dictify_config(config, array_index=idx,
-                                      expand_default=expand_default))
-
-    for item in chain:
-        pragmas = list(pragma for pragma in get_pragma(item, name=pragma)
-                       if pragma is not None)
-        if not pragmas:
-            if allow_no_pragma:
-                pragmas = [None]
-                result.append([(item, None)])
-                continue
-            else:
-                # If any pragma in the chain is unset, escape early
-                return []
-
-        if item.array_info and (item.data_type.is_complex_type or
-                                item.data_type.is_enum):
-            dictify_func = dictify_complex_array
-        else:
-            dictify_func = dictify_scalar
-
-        result.append(list(dictify_func(item)))
+    result = _expand_configurations_from_chain(
+        chain, pragma=pragma, allow_no_pragma=allow_no_pragma
+    )
+    if not result:
+        return []
 
     return list(itertools.product(*result))
 
 
 def squash_configs(*configs):
     '''
     Take a list of configurations, and squash them into one dictionary
@@ -330,15 +432,15 @@
 def _parse_rate(rate, hz_or_sec):
     '''
     Parse rate into frequency and seconds
 
     Parameters
     ----------
     rate : str
-        The pragma-specified rate
+        The pragma-specified rate.
 
     hz_or_sec : str
         {'hz', 's'}
 
     Returns
     -------
     dict
@@ -366,15 +468,15 @@
 def parse_update_rate(update, default=UPDATE_RATE_DEFAULT):
     '''
     Parse an 'update' specifier in a pragma
 
     Parameters
     ----------
     update : str
-        The I/O specifier from the pragma
+        The update rate specifier from the pragma.
 
     Returns
     -------
     dict
         With keys {'seconds', 'frequency', 'method'}
         Where 'method' is one of: {'poll', 'notify'}
 
@@ -412,15 +514,15 @@
 def parse_archive_settings(archive, default=ARCHIVE_DEFAULT):
     '''
     Parse an 'archive' specifier in a pragma
 
     Parameters
     ----------
     archive : str
-        The I/O specifier from the pragma
+        The archive specifier from the pragma.
 
     Returns
     -------
     dict
         With keys {'seconds', 'frequency', 'method'}
         Where 'method' is one of: {'scan', 'monitor'}
 
@@ -448,14 +550,92 @@
         res['method'] = method
         # Rate + frequency/seconds
         res.update(_parse_rate(d['rate'], d['hz_or_sec']))
 
     return res
 
 
+def parse_array_settings(pragma, dimensions):
+    '''
+    Parse an 'array' specifier in a pragma, yielding array elements.
+
+    Parameters
+    ----------
+    pragma : str
+        The I/O specifier from the pragma.
+
+    dimensions : 2-tuple
+        Lower and upper-bound of the array corresponding to the pragma.
+
+    Yields
+    ------
+    element : int
+        Integer element of selected array indices.
+
+    Raises
+    ------
+    ValueError
+        If an invalid pragma is supplied
+    '''
+    pragma = pragma.strip()
+
+    try:
+        low, high = dimensions
+    except Exception:
+        raise ValueError(
+            f'Invalid dimensions {dimensions!r} for array specifier in pragma '
+            f'{pragma!r}'
+        )
+
+    if not pragma:
+        yield from range(low, high + 1)
+        return
+
+    def _parse_element(elem):
+        if '..' not in elem:
+            return [int(elem)]
+
+        # Split by .., such that this will support:
+        #   ..to, from.., from..to, from..to..step
+        range_args = [int(idx) if idx else None
+                      for idx in elem.split('..')]
+
+        # Ensure we have start, stop, step
+        range_args += [None] * (3 - len(range_args))
+        elem_low, elem_high, elem_step = range_args
+
+        elem_low = low if elem_low is None else elem_low
+        # Add one to make the exclusive upper bound inclusive:
+        elem_high = high + 1 if elem_high is None else elem_high + 1
+        elem_step = 1 if elem_step is None else elem_step
+        return range(elem_low, elem_high, elem_step)
+
+    try:
+        for elem in pragma.split(','):
+            for idx in _parse_element(elem):
+                if not low <= idx <= high:
+                    raise ValueError(
+                        f'Array pragma index out of bounds: '
+                        f'{low} < {elem} < {high}'
+                    )
+                yield idx
+    except Exception as ex:
+        raise ValueError(
+            f'Invalid array pragma: {pragma} ({ex})'
+        )
+
+
+# Helpers which normalize various pragma values.
+_normalizers = {
+    'io': (normalize_io, 'io'),
+    'update': (parse_update_rate, '1s poll'),
+    'archive': (parse_archive_settings, '1s scan'),
+}
+
+
 def normalize_config(config):
     '''
     Parse and normalize pragma values into Python representations
 
     The following keys will be interpreted: ``io``, ``archive``, ``update``
 
     Parameters
@@ -464,20 +644,16 @@
         The configuration
 
     Returns
     -------
     dict
         A shallow-copy of ``config`` with parsed and normalized values
     '''
-    key_to_parser = {'io': (normalize_io, 'io'),
-                     'update': (parse_update_rate, '1s poll'),
-                     'archive': (parse_archive_settings, '1s scan'),
-                     }
     ret = dict(config)
-    for key, (parser_func, default) in key_to_parser.items():
+    for key, (parser_func, default) in _normalizers.items():
         ret[key] = parser_func(ret.get(key, default))
     return ret
 
 
 class SingularChain:
     '''
     A chain of data types, all with pytmc pragmas, representing a single piece
@@ -584,16 +760,19 @@
                        allow_no_pragma=False):
     'Build all SingularChain instances from a Symbol'
     if allow_no_pragma:
         condition = always_true
     else:
         condition = has_pragma
     for full_chain in symbol.walk(condition=condition):
-        for item_and_config in expand_configurations_from_chain(
-                full_chain, allow_no_pragma=allow_no_pragma):
+        configs = itertools.product(
+            *_expand_configurations_from_chain(full_chain,
+                                               allow_no_pragma=allow_no_pragma)
+        )
+        for item_and_config in configs:
             yield SingularChain(dict(item_and_config))
 
 
 def record_packages_from_symbol(symbol, *, pragma: str = 'pytmc',
                                 yield_exceptions=False,
                                 allow_no_pragma=False):
     'Create all record packages from a given Symbol'
@@ -602,20 +781,20 @@
         for chain in chains_from_symbol(symbol, pragma=pragma,
                                         allow_no_pragma=allow_no_pragma):
             try:
                 yield RecordPackage.from_chain(ads_port, chain=chain)
             except Exception as ex:
                 if yield_exceptions:
                     yield type(ex)(f"Symbol {symbol.name} "
-                                   f"chain: {chain.tcname}: {ex.args[0]}")
+                                   f"chain: {chain.tcname}: {ex}")
                 else:
                     raise
     except Exception as ex:
         if yield_exceptions:
-            yield type(ex)(f"Symbol {symbol.name} failure: {ex.args[0]}")
+            yield type(ex)(f"Symbol {symbol.name} failure: {ex}")
         else:
             raise
 
 
 def _attach_pragma(item, name, value):
     """Attach a pragma to a TwincatItem using `_make_fake_item`."""
     if not hasattr(item, 'Properties'):
```

### Comparing `pytmc-2.7.5/pytmc/record.py` & `pytmc-2.9.1/pytmc/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 import jinja2
 
 import pytmc
 
 from .default_settings.unified_ordered_field_list import unified_lookup_list
 
 logger = logging.getLogger(__name__)
-MAX_ARCHIVE_ELEMENTS = 1024
+
+# NOTE: Some PLCs may fill a buffer on a per-cycle basis. At 1KHz, 1000 is the
+# magic number that would be used.  This threshold reflects the fact that we do
+# not want to include those PVs in the archiver:
+MAX_ARCHIVE_ELEMENTS = 999
+
+# This field length maximum is based on the .DESC field length in epics-base:
 MAX_DESC_FIELD_LENGTH = 40
 
 _default_jinja_env = jinja2.Environment(
     loader=jinja2.PackageLoader("pytmc", "templates"),
     trim_blocks=True,
     lstrip_blocks=True,
 )
@@ -115,14 +121,27 @@
             for config_key in [f'autosave_pass{pass_}',
                                f'autosave_{self.direction}_pass{pass_}']:
                 if config_key in config:
                     record_key = f'pass{pass_}'
                     fields = set(config[config_key].split(' '))
                     self.autosave[record_key] = fields
 
+    def update_pini_for_autosave(self):
+        """
+        Set PINI=1 if VAL is autosaved at pass1.
+
+        This is a bandaid fix for unexplained behavior where the
+        autosave pass1 does not send values to the PLC unless
+        PINI=1.
+
+        This is intended to be called for output records.
+        """
+        if 'VAL' in self.autosave['pass1']:
+            self.fields['PINI'] = 1
+
     def render(self, sort: bool = True):
         """Render the provided template"""
         for field, value in list(self.fields.items()):
             self.fields[field] = str(value).strip('"')
 
         if sort:
             self.fields = sort_fields(self.fields)
@@ -283,14 +302,20 @@
             try:
                 spec = DATA_TYPES[data_type.name]
             except KeyError:
                 raise ValueError(
                     f'Unsupported data type {data_type.name} in chain: '
                     f'{chain.tcname} record: {chain.pvname}'
                 ) from None
+            if spec is IntegerRecordPackage:
+                if "scale" in chain.config or "offset" in chain.config:
+                    # longin/longout do not support scaling. Special-case and
+                    # cast to a FloatRecordPackage.
+                    spec = FloatRecordPackage
+
         return spec(*args, chain=chain, **kwargs)
 
 
 class TwincatTypeRecordPackage(RecordPackage):
     """
     The common parent for all RecordPackages for basic Twincat types
 
@@ -499,14 +524,15 @@
              }
         )
 
         # Set a default description to the tcname
         _update_description(record, self.chain.tcname)
 
         record.update_autosave_from_pragma(self.config)
+        record.update_pini_for_autosave()
         return record
 
     @property
     def records(self):
         """All records that will be created in the package"""
         records = [self.generate_input_record()]
         if self.io_direction == 'output':
@@ -548,14 +574,45 @@
     autosave_defaults = {
         'input': dict(pass0={'PREC'},
                       pass1={}),
         'output': dict(pass0={'VAL', 'PREC'},
                        pass1={}),
     }
 
+    def get_scale_offset(self):
+        """Get the scale and offset for the analog record(s)."""
+        scale = self.config.get("scale", None)
+        offset = self.config.get("offset", None)
+        if scale is None and offset is None:
+            return None, None
+
+        scale = "1.0" if scale is None else scale
+        offset = offset or "0.0"
+        return scale, offset
+
+    def generate_input_record(self):
+        record = super().generate_input_record()
+        scale, offset = self.get_scale_offset()
+        if scale is not None:
+            # If LINR==SLOPE, VAL = RVAL * ESLO + EOFF
+            record.fields["LINR"] = "SLOPE"
+            record.fields["ESLO"] = scale
+            record.fields["EOFF"] = offset
+        return record
+
+    def generate_output_record(self):
+        record = super().generate_output_record()
+        scale, offset = self.get_scale_offset()
+        if scale is not None:
+            # If LINR==SLOPE, then RVAL = (VAL - EOFF) / ESLO
+            record.fields["LINR"] = "SLOPE"
+            record.fields["ESLO"] = scale
+            record.fields["EOFF"] = offset
+        return record
+
 
 class EnumRecordPackage(TwincatTypeRecordPackage):
     """Create a set of record for a ENUM Twincat Variable"""
     input_rtyp = 'mbbi'
     output_rtyp = 'mbbo'
     dtyp = 'asynInt32'
     output_only_fields = {'DOL', 'IVOA', 'IVOV', 'OMSL', 'ORBV', 'RBV'}
@@ -592,14 +649,18 @@
             self.field_defaults.setdefault(string_field, string)
 
 
 class WaveformRecordPackage(TwincatTypeRecordPackage):
     """Create a set of records for a Twincat Array"""
     input_rtyp = 'waveform'
     output_rtyp = 'waveform'
+    field_defaults = {
+        'APST': 'On Change',
+        'MPST': 'On Change',
+    }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.nelm > MAX_ARCHIVE_ELEMENTS:
             self.archive_settings = None
 
     @property
```

### Comparing `pytmc-2.7.5/pytmc/templates/asyn_standard_record.jinja2` & `pytmc-2.9.1/pytmc/templates/asyn_standard_record.jinja2`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/templates/stcmd_default.cmd` & `pytmc-2.9.1/pytmc/templates/stcmd_default.cmd`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/conftest.py` & `pytmc-2.9.1/pytmc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_archive.py` & `pytmc-2.9.1/pytmc/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_commandline.py` & `pytmc-2.9.1/pytmc/tests/test_commandline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import pytest
+import io
 import sys
 
+import pytest
+
 import pytmc.bin.pytmc as pytmc_main
+from pytmc.bin.code import main as code_main
 from pytmc.bin.db import main as db_main
 from pytmc.bin.debug import create_debug_gui
 from pytmc.bin.pragmalint import main as pragmalint_main
 from pytmc.bin.stcmd import main as stcmd_main
 from pytmc.bin.summary import main as summary_main
+from pytmc.bin.template import main as template_main
 from pytmc.bin.types import create_types_gui
 from pytmc.bin.xmltranslate import main as xmltranslate_main
-from pytmc.bin.code import main as code_main
 
 
 def test_help_main(monkeypatch):
     monkeypatch.setattr(sys, 'argv', ['--help'])
     pytmc_main.main()
 
 
@@ -75,7 +78,56 @@
 def test_debug(qtbot, tmc_filename):
     widget = create_debug_gui(tmc_filename)
     qtbot.addWidget(widget)
 
 
 def test_code(project_filename):
     code_main(project_filename)
+
+
+def test_template_basic(project_filename):
+    template = '{% for project in projects %}{{ project }}{% endfor %}'
+    with io.StringIO(template) as template_fp:
+        templated = template_main([project_filename], template=template_fp)
+
+    print('templated', templated)
+    assert templated == project_filename
+
+
+@pytest.mark.parametrize(
+    'template',
+    [
+        pytest.param(
+            """
+            {% for project_path, project in projects.items() %}
+                {% set nc = get_nc(project) %}
+                {% for box in get_boxes(project) %}
+                    box: {{ box.attributes["Id"] }}
+                {% endfor %}
+
+                {% for dt in get_data_types(project) %}
+                    data type: {{ dt }}
+                {% endfor %}
+
+                {% for link in get_links(project) %}
+                    link: {{ link.a }}
+                {% endfor %}
+
+                {% for plc in project.plcs %}
+                    {% set results = get_linter_results(plc) %}
+                    Pragma count: {{ results.pragma_count }}
+
+                    {% for lib in get_library_versions(plc) %}
+                        library: {{ lib }}
+                    {% endfor %}
+
+                {% endfor %}
+            {% endfor %}
+            """,
+            id='helpers'),
+    ],
+)
+def test_template_smoke(project_filename, template):
+    with io.StringIO(template) as template_fp:
+        templated = template_main([project_filename], template=template_fp)
+
+    print('templated', templated)
```

### Comparing `pytmc-2.7.5/pytmc/tests/test_integrations.py` & `pytmc-2.9.1/pytmc/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_lint.py` & `pytmc-2.9.1/pytmc/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_parsing.py` & `pytmc-2.9.1/pytmc/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_project.py` & `pytmc-2.9.1/pytmc/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_record.py` & `pytmc-2.9.1/pytmc/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc/tests/test_xml_collector.py` & `pytmc-2.9.1/pytmc/tests/test_xml_collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import types
 
 import pytest
 
 from pytmc import parser, pragmas
-from pytmc.record import (BinaryRecordPackage, EnumRecordPackage,
-                          FloatRecordPackage, IntegerRecordPackage,
-                          RecordPackage, StringRecordPackage,
-                          WaveformRecordPackage)
+from pytmc.record import (MAX_ARCHIVE_ELEMENTS, BinaryRecordPackage,
+                          EnumRecordPackage, FloatRecordPackage,
+                          IntegerRecordPackage, RecordPackage,
+                          StringRecordPackage, WaveformRecordPackage)
 
 from . import conftest
 
 logger = logging.getLogger(__name__)
 
 
 def make_mock_twincatitem(name, data_type, *, pragma=None, array_info=None,
@@ -330,26 +330,26 @@
     record = RecordPackage.from_chain(chain=chain, ads_port=851)
     for rec in record.records:
         assert rec.fields.get('NELM') == final_NELM
 
 
 def test_scalar():
     item = make_mock_twincatitem(
-        name='tcname', data_type=make_mock_type('DINT'),
+        name='Main.tcname', data_type=make_mock_type('DINT'),
         pragma='pv: PVNAME')
 
     record, = list(pragmas.record_packages_from_symbol(item))
     assert record.pvname == 'PVNAME'
-    assert record.tcname == 'tcname'
+    assert record.tcname == 'Main.tcname'
     assert isinstance(record, IntegerRecordPackage)
 
 
 def test_complex_array():
     array = make_mock_twincatitem(
-        name='array_base',
+        name='Main.array_base',
         data_type=make_mock_type('MY_DUT', is_complex_type=True),
         pragma='pv: ARRAY', array_info=(1, 4))
 
     subitem1 = make_mock_twincatitem(
         name='subitem1', data_type=make_mock_type('INT'),
         pragma='pv: subitem1')
 
@@ -379,17 +379,90 @@
     assert isinstance(records['ARRAY:01:subitem1'], IntegerRecordPackage)
     assert isinstance(records['ARRAY:01:subitem2'], FloatRecordPackage)
 
     assert records['ARRAY:01:subitem1'].io_direction == 'output'
     assert records['ARRAY:01:subitem2'].io_direction == 'input'
 
 
+@pytest.mark.parametrize(
+    'dimensions, pragma, expected_records',
+    [
+        pytest.param([0, 3],
+                     '',
+                     {'ARRAY:00:subitem1',
+                      'ARRAY:01:subitem1',
+                      'ARRAY:02:subitem1',
+                      'ARRAY:03:subitem1'},
+                     id='no-pragma'),
+        pytest.param([0, 3],
+                     'array: 0..1',
+                     {'ARRAY:00:subitem1',
+                      'ARRAY:01:subitem1'},
+                     id='0..1'),
+        pytest.param([0, 3],
+                     'array: 0..1, 3',
+                     {'ARRAY:00:subitem1',
+                      'ARRAY:01:subitem1',
+                      'ARRAY:03:subitem1'},
+                     id='0..1,3'),
+        pytest.param([0, 3],
+                     'array: ..1',
+                     {'ARRAY:00:subitem1',
+                      'ARRAY:01:subitem1'},
+                     id='..1'),
+        pytest.param([0, 3],
+                     'array: 1..',
+                     {'ARRAY:01:subitem1',
+                      'ARRAY:02:subitem1',
+                      'ARRAY:03:subitem1'},
+                     id='1..'),
+        pytest.param([0, 100],
+                     'array: 0..1, 99..',
+                     {'ARRAY:0000:subitem1',
+                      'ARRAY:0001:subitem1',
+                      'ARRAY:0099:subitem1',
+                      'ARRAY:0100:subitem1'},
+                     id='0..1,99..'),
+        pytest.param([0, 100],
+                     """
+                     array: 0
+                     pv: OTHER
+                     array: 2..3
+                     """,
+                     {'ARRAY:0000:subitem1',
+                      'OTHER:0002:subitem1',
+                      'OTHER:0003:subitem1',
+                      },
+                     id='separate_prefixes'),
+    ]
+)
+def test_complex_array_partial(dimensions, pragma, expected_records):
+    array = make_mock_twincatitem(
+        name='Main.array_base',
+        data_type=make_mock_type('MY_DUT', is_complex_type=True),
+        pragma='\n'.join(('pv: ARRAY', pragma)),
+        array_info=dimensions,
+    )
+
+    subitem1 = make_mock_twincatitem(
+        name='subitem1', data_type=make_mock_type('INT'),
+        pragma='pv: subitem1')
+
+    def walk(condition=None):
+        yield [array, subitem1]
+
+    array.walk = walk
+    record_names = (record.pvname for record in
+                    pragmas.record_packages_from_symbol(array))
+    assert set(record_names) == expected_records
+
+
 def test_enum_array():
     array = make_mock_twincatitem(
-        name='enum_array',
+        name='Main.enum_array',
         data_type=make_mock_type('MY_ENUM', is_enum=True,
                                  enum_dict={1: 'ONE', 2: 'TWO'}),
         pragma='pv: ENUMS', array_info=(1, 4)
     )
 
     records = {
         record.pvname: record
@@ -410,15 +483,15 @@
     assert enum01.field_defaults['ZRST'] == "ONE"
     assert enum01.field_defaults['ONVL'] == 2
     assert enum01.field_defaults['ONST'] == "TWO"
 
 
 def test_unroll_formatting():
     array = make_mock_twincatitem(
-        name='enum_array',
+        name='Main.enum_array',
         data_type=make_mock_type('MY_ENUM', is_enum=True,
                                  enum_dict={1: 'ONE', 2: 'TWO'}),
         pragma='pv: ENUMS\nexpand: _EXPAND%d', array_info=(1, 4)
     )
 
     records = {
         record.pvname: record
@@ -431,30 +504,30 @@
         'ENUMS_EXPAND3',
         'ENUMS_EXPAND4',
     }
 
 
 def test_pv_linking():
     item = make_mock_twincatitem(
-        name='tcname', data_type=make_mock_type('DINT'),
+        name='Main.tcname', data_type=make_mock_type('DINT'),
         pragma='pv: PVNAME; link: OTHER:RECORD')
 
     pkg, = list(pragmas.record_packages_from_symbol(item))
     assert pkg.pvname == 'PVNAME'
-    assert pkg.tcname == 'tcname'
+    assert pkg.tcname == 'Main.tcname'
     assert isinstance(pkg, IntegerRecordPackage)
     rec = pkg.generate_output_record()
     assert rec.fields['OMSL'] == 'closed_loop'
     assert rec.fields['DOL'] == 'OTHER:RECORD CPP MS'
     assert rec.fields['SCAN'] == '.5 second'
 
 
 def test_pv_linking_special():
     struct = make_mock_twincatitem(
-        name='array_base',
+        name='Main.array_base',
         data_type=make_mock_type('MY_DUT', is_complex_type=True),
         pragma='pv: PREFIX')
 
     subitem1 = make_mock_twincatitem(
         name='subitem1', data_type=make_mock_type('INT'),
         pragma='pv: ABCD; link: **ABCD.STAT')
 
@@ -462,7 +535,203 @@
         yield [struct, subitem1]
 
     struct.walk = walk
 
     pkg, = list(pragmas.record_packages_from_symbol(struct))
     rec = pkg.generate_output_record()
     assert rec.fields['DOL'] == 'PREFIX:ABCD.STAT CPP MS'
+
+
+@pytest.mark.parametrize(
+    'elements, archive_settings',
+    [pytest.param(MAX_ARCHIVE_ELEMENTS + 1,
+                  None,
+                  id='over_threshold'),
+     pytest.param(MAX_ARCHIVE_ELEMENTS,
+                  {'frequency': 1, 'seconds': 1, 'method': 'scan',
+                   'fields': {'VAL'}},
+                  id='under_threshold'),
+     ],
+)
+def test_waveform_archive(chain, dbd_file, elements, archive_settings):
+    chain.data_type = make_mock_type('INT', is_array=True,
+                                     length=elements)
+    chain.config['io'] = 'io'
+    record = RecordPackage.from_chain(chain=chain, ads_port=851)
+    assert record.archive_settings == archive_settings
+    assert len(record.records) == 2
+    for rec in record.records:
+        print()
+        print('Archive settings', record.archive_settings)
+        print(rec.render())
+
+        assert rec.fields.get('APST') == 'On Change'
+        assert rec.fields.get('MPST') == 'On Change'
+
+    conftest.lint_record(dbd_file, record)
+
+
+@pytest.mark.parametrize(
+    'dimensions, pragma, expected_records',
+    [
+        pytest.param(
+            [0, 3],
+            '',
+            {'OUTER:INNER:00:item1',
+             'OUTER:INNER:01:item1',
+             'OUTER:INNER:02:item1',
+             'OUTER:INNER:03:item1',
+             },
+            id='no-pragma'
+        ),
+        pytest.param(
+            [0, 3],
+            'my_dut2.array: 0..1',
+            {'OUTER:INNER:00:item1',
+             'OUTER:INNER:01:item1',
+             },
+            id='0..1'
+        ),
+        pytest.param(
+            [0, 99],
+            'my_dut2.array: 1..3,5,7,9',
+            {'OUTER:INNER:001:item1',
+             'OUTER:INNER:002:item1',
+             'OUTER:INNER:003:item1',
+             'OUTER:INNER:005:item1',
+             'OUTER:INNER:007:item1',
+             'OUTER:INNER:009:item1',
+             },
+            id='1..3,5,7,9'
+        ),
+    ]
+)
+def test_complex_sub_array_partial(dimensions, pragma, expected_records):
+    outer = make_mock_twincatitem(
+        name='Main.my_dut',
+        data_type=make_mock_type('MY_DUT', is_complex_type=True),
+        pragma='\n'.join(('pv: OUTER', pragma)),
+    )
+
+    inner = make_mock_twincatitem(
+        name='my_dut2',
+        data_type=make_mock_type('MY_DUT2', is_complex_type=True),
+        pragma='pv: INNER',
+        array_info=dimensions,
+    )
+
+    subsubitem1 = make_mock_twincatitem(
+        name='item1', data_type=make_mock_type('INT'),
+        pragma='pv: item1'
+    )
+
+    def walk(condition=None):
+        yield [outer, inner, subsubitem1]
+
+    outer.walk = walk
+    record_names = (record.pvname for record in
+                    pragmas.record_packages_from_symbol(outer))
+    assert set(record_names) == expected_records
+
+
+@pytest.mark.parametrize(
+    'dimensions, pragma, expected_records',
+    [
+        pytest.param(
+            [0, 3],
+            '',
+            {'OUTER:INNER:00:item1_RBV',
+             'OUTER:INNER:01:item1_RBV',
+             'OUTER:INNER:02:item1_RBV',
+             'OUTER:INNER:03:item1_RBV',
+             },
+            id='no-pragma'
+        ),
+        pytest.param(
+            [0, 3],
+            ('my_dut2.array: 0..1\n'
+             'my_dut2.item1.io: io\n'
+             ),
+            {'OUTER:INNER:00:item1',
+             'OUTER:INNER:01:item1',
+             'OUTER:INNER:00:item1_RBV',
+             'OUTER:INNER:01:item1_RBV',
+             },
+            id='change_to_io'
+        ),
+    ]
+)
+def test_sub_io_change(dimensions, pragma, expected_records):
+    outer = make_mock_twincatitem(
+        name='Main.my_dut',
+        data_type=make_mock_type('MY_DUT', is_complex_type=True),
+        pragma='\n'.join(('pv: OUTER', pragma)),
+    )
+
+    inner = make_mock_twincatitem(
+        name='my_dut2',
+        data_type=make_mock_type('MY_DUT2', is_complex_type=True),
+        pragma='pv: INNER',
+        array_info=dimensions,
+    )
+
+    subsubitem1 = make_mock_twincatitem(
+        name='item1', data_type=make_mock_type('INT'),
+        pragma='\n'.join(('pv: item1', 'io: i'))
+    )
+
+    def walk(condition=None):
+        yield [outer, inner, subsubitem1]
+
+    outer.walk = walk
+    record_names = (record.pvname
+                    for pkg in pragmas.record_packages_from_symbol(outer)
+                    for record in pkg.records)
+    assert set(record_names) == expected_records
+
+
+@pytest.mark.parametrize(
+    "data_type, pragma, expected_scale, expected_offset",
+    [
+        pytest.param(
+            "FLOAT",
+            "pv: PREFIX; scale: 2.0; offset: 1.0",
+            "2.0",
+            "1.0",
+            id="float-scale-and-offset",
+        ),
+        pytest.param(
+            "UDINT",
+            "pv: PREFIX; scale: 3.0; offset: 0.1",
+            "3.0",
+            "0.1",
+            id="int-scale-and-offset",
+        ),
+        pytest.param(
+            "UDINT",
+            "pv: PREFIX; scale: 3.0",
+            "3.0",
+            "0.0",
+            id="int-no-offset",
+        ),
+        pytest.param(
+            "UDINT",
+            "pv: PREFIX; offset: 3.0",
+            "1.0",
+            "3.0",
+            id="int-no-scale",
+        ),
+    ],
+)
+def test_scale_and_offset(data_type, pragma, expected_scale, expected_offset):
+    item = make_mock_twincatitem(
+        name='Main.obj',
+        data_type=make_mock_type('UDINT', is_complex_type=False),
+        pragma=pragma,
+    )
+
+    pkg, = list(pragmas.record_packages_from_symbol(item))
+    for rec in pkg.records:
+        assert rec.fields['LINR'] == "SLOPE"
+        assert rec.fields['ESLO'] == expected_scale
+        assert rec.fields['EOFF'] == expected_offset
+        assert rec.record_type in {"ai", "ao"}
```

### Comparing `pytmc-2.7.5/pytmc/tests/test_xml_obj.py` & `pytmc-2.9.1/pytmc/tests/test_xml_obj.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/pytmc.egg-info/SOURCES.txt` & `pytmc-2.9.1/pytmc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,26 +16,24 @@
 pytmc/record.py
 pytmc.egg-info/PKG-INFO
 pytmc.egg-info/SOURCES.txt
 pytmc.egg-info/dependency_links.txt
 pytmc.egg-info/entry_points.txt
 pytmc.egg-info/requires.txt
 pytmc.egg-info/top_level.txt
-pytmc/benchmark/__init__.py
-pytmc/benchmark/profile.py
-pytmc/benchmark/utils.py
 pytmc/bin/__init__.py
 pytmc/bin/code.py
 pytmc/bin/db.py
 pytmc/bin/debug.py
 pytmc/bin/iocboot.py
 pytmc/bin/pragmalint.py
 pytmc/bin/pytmc.py
 pytmc/bin/stcmd.py
 pytmc/bin/summary.py
+pytmc/bin/template.py
 pytmc/bin/types.py
 pytmc/bin/util.py
 pytmc/bin/xmltranslate.py
 pytmc/default_settings/__init__.py
 pytmc/default_settings/unified_ordered_field_list.py
 pytmc/templates/EPICS_proto_template.proto
 pytmc/templates/asyn_standard_file.jinja2
```

### Comparing `pytmc-2.7.5/setup.py` & `pytmc-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytmc-2.7.5/versioneer.py` & `pytmc-2.9.1/versioneer.py`

 * *Files identical despite different names*

