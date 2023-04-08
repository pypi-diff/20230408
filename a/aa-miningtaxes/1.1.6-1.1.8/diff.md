# Comparing `tmp/aa-miningtaxes-1.1.6.tar.gz` & `tmp/aa-miningtaxes-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-miningtaxes-1.1.6.tar", last modified: Sun Dec 11 21:40:06 2022, max compression
+gzip compressed data, was "aa-miningtaxes-1.1.8.tar", last modified: Wed Dec 21 21:29:49 2022, max compression
```

## Comparing `aa-miningtaxes-1.1.6.tar` & `aa-miningtaxes-1.1.8.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.419484 aa-miningtaxes-1.1.6/
--rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7283 2022-12-11 21:40:06.419484 aa-miningtaxes-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5580 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.395484 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7283 2022-12-11 21:40:06.000000 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2604 2022-12-11 21:40:06.000000 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-11 21:40:06.000000 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2022-12-11 21:40:06.000000 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-11 21:40:06.000000 aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.402484 aa-miningtaxes-1.1.6/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)      108 2022-12-11 21:18:14.000000 aa-miningtaxes-1.1.6/miningtaxes/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/miningtaxes/admin.py
--rw-r--r--   0 root         (0) root         (0)     1546 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.6/miningtaxes/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.1.6/miningtaxes/apps.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.1.6/miningtaxes/auth_hooks.py
--rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.1.6/miningtaxes/decorators.py
--rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.1.6/miningtaxes/forms.py
--rw-r--r--   0 root         (0) root         (0)     2061 2022-11-03 15:03:29.000000 aa-miningtaxes-1.1.6/miningtaxes/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.390484 aa-miningtaxes-1.1.6/miningtaxes/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.403484 aa-miningtaxes-1.1.6/miningtaxes/management/commands/
--rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.1.6/miningtaxes/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2022-10-29 11:13:21.000000 aa-miningtaxes-1.1.6/miningtaxes/management/commands/miningtaxes_preload_prices.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.1.6/miningtaxes/management/commands/miningtaxes_zero_all.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.405484 aa-miningtaxes-1.1.6/miningtaxes/migrations/
--rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0002_all_models.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0003_alter_general_options.py
--rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
--rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.1.6/miningtaxes/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.407484 aa-miningtaxes-1.1.6/miningtaxes/models/
--rw-r--r--   0 root         (0) root         (0)      399 2022-11-20 04:46:19.000000 aa-miningtaxes-1.1.6/miningtaxes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6754 2022-11-06 19:16:46.000000 aa-miningtaxes-1.1.6/miningtaxes/models/admin.py
--rw-r--r--   0 root         (0) root         (0)    16180 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.6/miningtaxes/models/character.py
--rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.1.6/miningtaxes/models/general.py
--rw-r--r--   0 root         (0) root         (0)     3366 2022-11-14 17:38:09.000000 aa-miningtaxes-1.1.6/miningtaxes/models/orePrices.py
--rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.6/miningtaxes/models/settings.py
--rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.1.6/miningtaxes/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.390484 aa-miningtaxes-1.1.6/miningtaxes/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.391484 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.408484 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/
--rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/billboards_dark.css
--rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/billboards_light.css
--rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/global.css
--rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/launcher.css
--rw-r--r--   0 root         (0) root         (0)     1363 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/miningtaxes.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.409484 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/
--rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq1.png
--rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq2.png
--rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq3.png
--rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.1.6/miningtaxes/swagger.json
--rw-r--r--   0 root         (0) root         (0)    12185 2022-11-23 21:19:21.000000 aa-miningtaxes-1.1.6/miningtaxes/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.391484 aa-miningtaxes-1.1.6/miningtaxes/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.413484 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/
--rw-r--r--   0 root         (0) root         (0)     5067 2022-11-21 03:39:06.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/admin_launcher.html
--rw-r--r--   0 root         (0) root         (0)    20140 2022-11-28 20:07:21.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/admin_tables.html
--rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/base.html
--rw-r--r--   0 root         (0) root         (0)     2755 2022-11-05 18:05:41.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/character_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1740 2022-11-21 01:21:27.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/faq.html
--rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/index.html
--rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/launcher.html
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/ore_prices.html
--rw-r--r--   0 root         (0) root         (0)     9758 2022-12-08 11:39:36.000000 aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/user_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.414484 aa-miningtaxes-1.1.6/miningtaxes/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.415484 aa-miningtaxes-1.1.6/miningtaxes/tests/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_admin_character.py
--rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_character.py
--rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_orePrice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.416484 aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/
--rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/esi_client_stub.py
--rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/load_entities.py
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/load_eveuniverse.py
--rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.1.6/miningtaxes/tests/utils.py
--rw-r--r--   0 root         (0) root         (0)     2491 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.6/miningtaxes/urls.py
--rw-r--r--   0 root         (0) root         (0)    33405 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.6/miningtaxes/views.py
--rw-r--r--   0 root         (0) root         (0)      252 2022-12-11 21:40:06.420484 aa-miningtaxes-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 21:40:06.419484 aa-miningtaxes-1.1.6/testauth/
--rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/testauth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.1.6/testauth/settingsAA2.py
--rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.1.6/testauth/settingsAA3.py
--rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/testauth/urls.py
--rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.6/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2022-11-06 18:50:28.000000 aa-miningtaxes-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7283 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5580 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.415578 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7283 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2604 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-12-21 21:29:49.000000 aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.417578 aa-miningtaxes-1.1.8/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)      108 2022-12-21 21:23:09.000000 aa-miningtaxes-1.1.8/miningtaxes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/miningtaxes/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2022-12-11 21:19:35.000000 aa-miningtaxes-1.1.8/miningtaxes/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-10-27 10:33:48.000000 aa-miningtaxes-1.1.8/miningtaxes/apps.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-10-24 21:25:29.000000 aa-miningtaxes-1.1.8/miningtaxes/auth_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2022-11-07 04:47:52.000000 aa-miningtaxes-1.1.8/miningtaxes/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      264 2022-11-05 16:57:46.000000 aa-miningtaxes-1.1.8/miningtaxes/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2022-11-03 15:03:29.000000 aa-miningtaxes-1.1.8/miningtaxes/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.417578 aa-miningtaxes-1.1.8/miningtaxes/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-10-29 09:17:21.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2022-10-29 11:13:21.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/miningtaxes_preload_prices.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-22 12:21:22.000000 aa-miningtaxes-1.1.8/miningtaxes/management/commands/miningtaxes_zero_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.418578 aa-miningtaxes-1.1.8/miningtaxes/migrations/
+-rw-r--r--   0 root         (0) root         (0)      902 2022-11-06 17:28:27.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)    15700 2022-11-06 17:28:28.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0002_all_models.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-11-08 09:05:56.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0003_alter_general_options.py
+-rw-r--r--   0 root         (0) root         (0)      939 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py
+-rw-r--r--   0 root         (0) root         (0)      737 2022-11-14 03:13:49.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      452 2022-11-22 12:29:33.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/0006_charactertaxcredits_credit_type.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 16:52:52.000000 aa-miningtaxes-1.1.8/miningtaxes/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.418578 aa-miningtaxes-1.1.8/miningtaxes/models/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-11-20 04:46:19.000000 aa-miningtaxes-1.1.8/miningtaxes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2022-11-06 19:16:46.000000 aa-miningtaxes-1.1.8/miningtaxes/models/admin.py
+-rw-r--r--   0 root         (0) root         (0)    16180 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.8/miningtaxes/models/character.py
+-rw-r--r--   0 root         (0) root         (0)      712 2022-11-08 03:08:01.000000 aa-miningtaxes-1.1.8/miningtaxes/models/general.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2022-11-14 17:38:09.000000 aa-miningtaxes-1.1.8/miningtaxes/models/orePrices.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2022-11-12 04:17:36.000000 aa-miningtaxes-1.1.8/miningtaxes/models/settings.py
+-rw-r--r--   0 root         (0) root         (0)      246 2022-10-27 10:44:31.000000 aa-miningtaxes-1.1.8/miningtaxes/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.419578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/
+-rw-r--r--   0 root         (0) root         (0)     4582 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_dark.css
+-rw-r--r--   0 root         (0) root         (0)     4558 2022-11-05 13:42:07.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_light.css
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/global.css
+-rw-r--r--   0 root         (0) root         (0)     4331 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/launcher.css
+-rw-r--r--   0 root         (0) root         (0)     1363 2022-10-27 12:54:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/miningtaxes.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.419578 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/
+-rw-r--r--   0 root         (0) root         (0)    34837 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq1.png
+-rw-r--r--   0 root         (0) root         (0)   132605 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq2.png
+-rw-r--r--   0 root         (0) root         (0)   342376 2022-11-19 22:22:28.000000 aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq3.png
+-rw-r--r--   0 root         (0) root         (0)   881821 2022-10-27 12:49:53.000000 aa-miningtaxes-1.1.8/miningtaxes/swagger.json
+-rw-r--r--   0 root         (0) root         (0)    12185 2022-11-23 21:19:21.000000 aa-miningtaxes-1.1.8/miningtaxes/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.414578 aa-miningtaxes-1.1.8/miningtaxes/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.421578 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/
+-rw-r--r--   0 root         (0) root         (0)     5082 2022-12-11 21:49:11.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_launcher.html
+-rw-r--r--   0 root         (0) root         (0)    20176 2022-12-21 21:25:40.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_tables.html
+-rw-r--r--   0 root         (0) root         (0)     2396 2022-11-28 15:03:03.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/base.html
+-rw-r--r--   0 root         (0) root         (0)     2755 2022-11-05 18:05:41.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/character_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1740 2022-11-21 01:21:27.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/faq.html
+-rw-r--r--   0 root         (0) root         (0)      480 2022-10-24 21:28:14.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/index.html
+-rw-r--r--   0 root         (0) root         (0)     6466 2022-11-01 15:07:04.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/launcher.html
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-22 12:28:46.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/ore_prices.html
+-rw-r--r--   0 root         (0) root         (0)     9758 2022-12-08 11:39:36.000000 aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/user_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.421578 aa-miningtaxes-1.1.8/miningtaxes/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 22:43:55.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.422578 aa-miningtaxes-1.1.8/miningtaxes/tests/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-19 23:50:12.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2022-11-21 22:33:02.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_admin_character.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2022-11-22 12:24:37.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2022-11-20 04:46:58.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_orePrice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.422578 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/
+-rw-r--r--   0 root         (0) root         (0)     1361 2022-11-21 20:39:23.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/esi_client_stub.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2022-11-20 16:09:12.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_entities.py
+-rw-r--r--   0 root         (0) root         (0)      434 2022-11-20 04:51:22.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-11-21 22:30:35.000000 aa-miningtaxes-1.1.8/miningtaxes/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2022-12-08 04:56:42.000000 aa-miningtaxes-1.1.8/miningtaxes/urls.py
+-rw-r--r--   0 root         (0) root         (0)    33402 2022-12-20 18:08:37.000000 aa-miningtaxes-1.1.8/miningtaxes/views.py
+-rw-r--r--   0 root         (0) root         (0)      252 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1586 2022-11-23 22:55:27.000000 aa-miningtaxes-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 21:29:49.423578 aa-miningtaxes-1.1.8/testauth/
+-rw-r--r--   0 root         (0) root         (0)       46 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      612 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/celery.py
+-rwxr-xr-x   0 root         (0) root         (0)     9919 2022-11-03 12:24:46.000000 aa-miningtaxes-1.1.8/testauth/settingsAA2.py
+-rwxr-xr-x   0 root         (0) root         (0)     9932 2022-11-03 12:24:55.000000 aa-miningtaxes-1.1.8/testauth/settingsAA3.py
+-rw-r--r--   0 root         (0) root         (0)      174 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/urls.py
+-rw-r--r--   0 root         (0) root         (0)      397 2022-10-24 20:51:10.000000 aa-miningtaxes-1.1.8/testauth/wsgi.py
```

### Comparing `aa-miningtaxes-1.1.6/LICENSE` & `aa-miningtaxes-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/PKG-INFO` & `aa-miningtaxes-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.1.6
+Version: 1.1.8
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
```

### Comparing `aa-miningtaxes-1.1.6/README.md` & `aa-miningtaxes-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/PKG-INFO` & `aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-miningtaxes
-Version: 1.1.6
+Version: 1.1.8
 Summary: An Alliance Auth app that tracks and applies taxes for mining
 Home-page: https://gitlab.com/arctiru/aa-miningtaxes
 Author: Arc Tiru
 Author-email: arcturusstl@gmail.com
 License: MIT
 Description: # Mining Taxes
```

### Comparing `aa-miningtaxes-1.1.6/aa_miningtaxes.egg-info/SOURCES.txt` & `aa-miningtaxes-1.1.8/aa_miningtaxes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/app_settings.py` & `aa-miningtaxes-1.1.8/miningtaxes/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/auth_hooks.py` & `aa-miningtaxes-1.1.8/miningtaxes/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/decorators.py` & `aa-miningtaxes-1.1.8/miningtaxes/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/helpers.py` & `aa-miningtaxes-1.1.8/miningtaxes/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/migrations/0001_initial.py` & `aa-miningtaxes-1.1.8/miningtaxes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/migrations/0002_all_models.py` & `aa-miningtaxes-1.1.8/miningtaxes/migrations/0002_all_models.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/migrations/0003_alter_general_options.py` & `aa-miningtaxes-1.1.8/miningtaxes/migrations/0003_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py` & `aa-miningtaxes-1.1.8/miningtaxes/migrations/0004_settings_interest_rate_alter_settings_phrase.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py` & `aa-miningtaxes-1.1.8/miningtaxes/migrations/0005_oreprices_raw_price_oreprices_refined_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/models/admin.py` & `aa-miningtaxes-1.1.8/miningtaxes/models/admin.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/models/character.py` & `aa-miningtaxes-1.1.8/miningtaxes/models/character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/models/general.py` & `aa-miningtaxes-1.1.8/miningtaxes/models/general.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/models/orePrices.py` & `aa-miningtaxes-1.1.8/miningtaxes/models/orePrices.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/models/settings.py` & `aa-miningtaxes-1.1.8/miningtaxes/models/settings.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/billboards_dark.css` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/billboards_light.css` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/billboards_light.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/global.css` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/launcher.css` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/css/miningtaxes.css` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/css/miningtaxes.css`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq1.png` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq1.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq2.png` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq2.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/static/miningtaxes/images/faq3.png` & `aa-miningtaxes-1.1.8/miningtaxes/static/miningtaxes/images/faq3.png`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/swagger.json` & `aa-miningtaxes-1.1.8/miningtaxes/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tasks.py` & `aa-miningtaxes-1.1.8/miningtaxes/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/admin_launcher.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_launcher.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {% load humanize %}
 {% load evelinks %}
 {% load bootstrap %}
 
 {% block details %}
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
-            <h3 class="panel-title">{% translate 'Tax Settings' %}</h3>
+		<h3 class="panel-title">{% translate 'MiningTaxes Settings' %} (v{{ version }})</h3>
         </div>
         <div class="panel-body">
 	    <form class="form" action="{{ url }}" method="POST">
 		    {% csrf_token %}
 		    {{ form|bootstrap }}
 		    <button type="submit" class="btn btn-primary">Edit Settings</button>
 	    </form>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'miningtaxes/base.html' %} {% load i18n %} {% load static %} {% load
 humanize %} {% load evelinks %} {% load bootstrap %} {% block details %}
-**** {% translate 'Tax Settings' %} ****
+**** {% translate 'MiningTaxes Settings' %} (v{{ version }}) ****
 {% csrf_token %} {{ form|bootstrap }} Edit Settings
 **** {% translate 'Accountant Characters (add only one accountant per corp)' %}
 ****
     * {% translate 'Register Character' %}
       [Add_character]
       {%_translate_'Register'_%}
     * {% if has_registered_characters %}  {% for auth_character in
```

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/admin_tables.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/admin_tables.html`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             <tbody></tbody>
         </table>
     </div>
 			</div>
 		</div>
 	</div>
 </div>
+<!--
 <div class="row">
 	<div class="col-md-12">
     		<div class="panel panel-default">
 			<div class="panel-heading" style="display:flex;">
 			    <h3 class="panel-title">Taxes by Character</h3>
 			</div>
 			<div class="panel-body">
@@ -97,14 +98,15 @@
             <tbody></tbody>
         </table>
     </div>
 			</div>
 		</div>
 	</div>
 </div>
+-->
 
 <div class="modal" id="modalCredit" tabindex="-1" role="dialog" aria-labelledby="modalCredit">
     <div class="modal-dialog  modal-sm" role="document" id="modalCredit">
         <div class="modal-content">
             <div class="modal-header">
                 <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">
                     &times;
@@ -423,30 +425,30 @@
 			},
 			{
 			    data: 'quantity',
 			    render: $.fn.dataTable.render.number(',', '.', 0)
 			},
 			{ data: 'last' },
 		    ],
-		    order: [[1, "desc"]]
+		    order: [[3, "desc"]]
 		});
 		unknown_table = $('#unknown').DataTable({
 		    columns: [
 			{ data: 'name' },
 			{
 			    data: 'isk',
 			    render: $.fn.dataTable.render.number(',', '.', 2)
 			},
 			{
 			    data: 'quantity',
 			    render: $.fn.dataTable.render.number(',', '.', 0)
 			},
 			{ data: 'last' },
 		    ],
-		    order: [[1, "desc"]]
+		    order: [[3, "desc"]]
 		});
 		corpmoon_table = $('#corpmoon').DataTable({
 		    columns: [
 			{ data: 'date' },
 			{ data: 'name' },
 			{ data: 'ore' },
 			{
@@ -704,14 +706,15 @@
                     data: 'amount',
                     render: $.fn.dataTable.render.number(',', '.', 2)
                 },
                 { data: 'reason' },
             ],
             order: [[0, "desc"]]
         });
+      /*
         $('#chars').DataTable({
             ajax: {
                 url: "{% url 'miningtaxes:admin_char_json' %}",
                 dataSrc: 'data',
                 cache: false
             },
             columns: [
@@ -729,9 +732,10 @@
                 {
                     data: 'balance',
                     render: $.fn.dataTable.render.number(',', '.', 2)
                 }
             ],
             order: [[5, "desc"]]
         });
+									      */
 });
 {% endblock %}
```

#### html2text {}

```diff
@@ -8,17 +8,14 @@
 **** Overall Monthly Tax Revenue ****
 Export CSV
 **** Monthly Taxes by Users ****
 Export CSV
 **** Taxes by User ****
 {% translate {% translate 'Corp' {% translate {% translate 'Last {% translate
 'Name' %}    %}                  'Balance' %} Paid' %}           'Actions' %}
-**** Taxes by Character ****
-{% translate {% translate {% translate {% translate {% translate {% translate
-'Name' %}    'Corp' %}    'Main' %}    'Taxes' %}   'Credits' %} 'Balance' %}
  ×
 *** Tax Credits ***
 {% csrf_token %}
 Recipient:
 Tax credit amount: [creditbox           ]
  {% translate 'Submit' %}
 **** Corp Ledgers ****
@@ -77,18 +74,18 @@
 ("#userid").val(user_data[rowi].user); const bal = Math.round((user_data
 [rowi].balance + Number.EPSILON) * 100) / 100 $("#creditbox").val(bal); }
 function draw_corp_moons() { $.getJSON("{% url 'miningtaxes:
 admin_corp_mining_history' %}", function (d) { unregistered_table = $
 ('#unregistered').DataTable({ columns: [ { data: 'name' }, { data: 'isk',
 render: $.fn.dataTable.render.number(',', '.', 2) }, { data: 'quantity',
 render: $.fn.dataTable.render.number(',', '.', 0) }, { data: 'last' }, ],
-order: [[1, "desc"]] }); unknown_table = $('#unknown').DataTable({ columns: [
+order: [[3, "desc"]] }); unknown_table = $('#unknown').DataTable({ columns: [
 { data: 'name' }, { data: 'isk', render: $.fn.dataTable.render.number(',', '.',
 2) }, { data: 'quantity', render: $.fn.dataTable.render.number(',', '.', 0) },
-{ data: 'last' }, ], order: [[1, "desc"]] }); corpmoon_table = $
+{ data: 'last' }, ], order: [[3, "desc"]] }); corpmoon_table = $
 ('#corpmoon').DataTable({ columns: [ { data: 'date' }, { data: 'name' },
 { data: 'ore' }, { data: 'quantity', render: $.fn.dataTable.render.number(',',
 '.', 0) }, { data: 'location' }, ], order: [[0, "desc"]] }); unknown_data = d
 ["unknown_data"]; unknown_data.forEach( function(row) { unknown_table.row.add
 (row); }); unknown_table.draw(); unregistered_data = d["unregistered_data"];
 unregistered_data.forEach( function(row) { unregistered_table.row.add(row); });
 unregistered_table.draw(); mining_data = d["mining_log"]; mining_data.forEach
@@ -142,14 +139,14 @@
 (); }); user_table = $('#mains').DataTable({ columns: [ { data: 'name' },
 { data: 'corp' }, { data: 'balance', render: $.fn.dataTable.render.number(',',
 '.', 2) }, { data: 'last_paid' }, { data: 'action' }, ], order: [[2, "desc"]]
 }); $('#corp_ledgers').DataTable({ ajax: { url: "{% url 'miningtaxes:
 admin_corp_ledger' %}", dataSrc: 'data', cache: false }, columns: [ { data:
 'date' }, { data: 'name' }, { data: 'amount', render:
 $.fn.dataTable.render.number(',', '.', 2) }, { data: 'reason' }, ], order: [[0,
-"desc"]] }); $('#chars').DataTable({ ajax: { url: "{% url 'miningtaxes:
+"desc"]] }); /* $('#chars').DataTable({ ajax: { url: "{% url 'miningtaxes:
 admin_char_json' %}", dataSrc: 'data', cache: false }, columns: [ { data:
 'name' }, { data: 'corp' }, { data: 'main_name' }, { data: 'taxes', render:
 $.fn.dataTable.render.number(',', '.', 2) }, { data: 'credits', render:
 $.fn.dataTable.render.number(',', '.', 2) }, { data: 'balance', render:
-$.fn.dataTable.render.number(',', '.', 2) } ], order: [[5, "desc"]] }); }); {%
-endblock %}
+$.fn.dataTable.render.number(',', '.', 2) } ], order: [[5, "desc"]] }); */ });
+{% endblock %}
```

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/base.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/base.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/character_viewer.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/faq.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/faq.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/launcher.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/launcher.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/ore_prices.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/ore_prices.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/templates/miningtaxes/user_summary.html` & `aa-miningtaxes-1.1.8/miningtaxes/templates/miningtaxes/user_summary.html`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_admin_character.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_admin_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_character.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_character.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/models/test_orePrice.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/models/test_orePrice.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/esi_client_stub.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/testdata/load_entities.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/tests/utils.py` & `aa-miningtaxes-1.1.8/miningtaxes/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/urls.py` & `aa-miningtaxes-1.1.8/miningtaxes/urls.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/miningtaxes/views.py` & `aa-miningtaxes-1.1.8/miningtaxes/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.helpers import humanize_number
 from app_utils.logging import LoggerAddTag
 from app_utils.views import bootstrap_icon_plus_name_html
 
-from . import __title__, tasks
+from . import __title__, __version__, tasks
 from .app_settings import MININGTAXES_TAX_CACHE_VIEW_TIMEOUT
 from .forms import SettingsForm
 from .helpers import PriceGroups
 from .models import (
     AdminCharacter,
     AdminMiningCorpLedgerEntry,
     AdminMiningObsLog,
@@ -75,14 +75,15 @@
             }
         )
 
     context = {
         "page_title": "Admin Settings",
         "auth_characters": auth_characters,
         "has_registered_characters": len(auth_characters) > 0,
+        "version": __version__,
         "form": form,
     }
     return render(request, "miningtaxes/admin_launcher.html", context)
 
 
 @login_required
 @cache_page(MININGTAXES_TAX_CACHE_VIEW_TIMEOUT)
@@ -181,15 +182,14 @@
                 "user": char2user[m],
             }
         )
     return JsonResponse({"data": main_data})
 
 
 @login_required
-@cache_page(MININGTAXES_TAX_CACHE_VIEW_TIMEOUT)
 @permission_required("miningtaxes.auditor_access")
 def admin_tables(request):
     if request.method == "POST":
         isk = request.POST["creditbox"].replace(",", "")
         try:
             isk = float(isk)
         except ValueError:
```

### Comparing `aa-miningtaxes-1.1.6/setup.py` & `aa-miningtaxes-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/testauth/celery.py` & `aa-miningtaxes-1.1.8/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/testauth/settingsAA2.py` & `aa-miningtaxes-1.1.8/testauth/settingsAA2.py`

 * *Files identical despite different names*

### Comparing `aa-miningtaxes-1.1.6/testauth/settingsAA3.py` & `aa-miningtaxes-1.1.8/testauth/settingsAA3.py`

 * *Files identical despite different names*

