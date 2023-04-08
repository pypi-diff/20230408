# Comparing `tmp/aa-memberaudit-2.6.0.tar.gz` & `tmp/aa_memberaudit-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-memberaudit-2.6.0.tar", last modified: Thu Mar 23 15:11:54 2023, max compression
+gzip compressed data, was "aa_memberaudit-2.6.1.tar", last modified: Sat Apr  8 19:47:29 2023, max compression
```

## Comparing `aa-memberaudit-2.6.0.tar` & `aa_memberaudit-2.6.1.tar`

### file list

```diff
@@ -1,260 +1,276 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.850360 aa-memberaudit-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-07 16:50:18.000000 aa-memberaudit-2.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      263 2022-06-17 10:57:57.000000 aa-memberaudit-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6593 2023-03-23 15:11:54.850360 aa-memberaudit-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5613 2022-10-21 17:48:21.000000 aa-memberaudit-2.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.798359 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6593 2023-03-23 15:11:54.000000 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10774 2023-03-23 15:11:54.000000 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 15:11:54.000000 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2023-03-23 15:11:54.000000 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-23 15:11:54.000000 aa-memberaudit-2.6.0/aa_memberaudit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.798359 aa-memberaudit-2.6.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1971 2022-07-22 17:17:58.000000 aa-memberaudit-2.6.0/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.802359 aa-memberaudit-2.6.0/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-03-23 14:57:05.000000 aa-memberaudit-2.6.0/memberaudit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21864 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2021-05-04 15:11:43.000000 aa-memberaudit-2.6.0/memberaudit/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-03-22 20:38:17.000000 aa-memberaudit-2.6.0/memberaudit/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-22 22:31:11.000000 aa-memberaudit-2.6.0/memberaudit/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.806360 aa-memberaudit-2.6.0/memberaudit/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 17:29:05.000000 aa-memberaudit-2.6.0/memberaudit/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11673 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/core/data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    19049 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/core/eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5305 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/core/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2022-09-03 21:36:22.000000 aa-memberaudit-2.6.0/memberaudit/core/skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/core/skills.py
--rw-rw-rw-   0 root         (0) root         (0)     3150 2022-07-14 11:30:46.000000 aa-memberaudit-2.6.0/memberaudit/core/xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2336 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-02-24 17:52:57.000000 aa-memberaudit-2.6.0/memberaudit/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.790360 aa-memberaudit-2.6.0/memberaudit/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.806360 aa-memberaudit-2.6.0/memberaudit/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      102 2020-11-24 21:31:34.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-04 15:11:43.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2021-05-04 15:11:43.000000 aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_update_characters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.806360 aa-memberaudit-2.6.0/memberaudit/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-18 15:52:38.000000 aa-memberaudit-2.6.0/memberaudit/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13007 2023-02-24 14:11:29.000000 aa-memberaudit-2.6.0/memberaudit/managers/character.py
--rw-rw-rw-   0 root         (0) root         (0)    21180 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/managers/general.py
--rw-rw-rw-   0 root         (0) root         (0)    48369 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/managers/sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.810360 aa-memberaudit-2.6.0/memberaudit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    65995 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/memberaudit/migrations/0001_initial_new.py
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/memberaudit/migrations/0002_add_mining_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/memberaudit/migrations/0003_add_notify_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/memberaudit/migrations/0004_character_is_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/migrations/0005_add_fw_stats.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:18:29.000000 aa-memberaudit-2.6.0/memberaudit/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.810360 aa-memberaudit-2.6.0/memberaudit/models/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53140 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/models/character.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-01-17 22:43:01.000000 aa-memberaudit-2.6.0/memberaudit/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    14223 2022-10-21 17:48:21.000000 aa-memberaudit-2.6.0/memberaudit/models/general.py
--rw-rw-rw-   0 root         (0) root         (0)    39924 2023-03-22 22:31:11.000000 aa-memberaudit-2.6.0/memberaudit/models/sections.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-17 10:57:57.000000 aa-memberaudit-2.6.0/memberaudit/providers.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-03-05 14:47:06.000000 aa-memberaudit-2.6.0/memberaudit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.790360 aa-memberaudit-2.6.0/memberaudit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.790360 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.814360 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:11:29.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-02-09 21:55:36.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/character_finder.css
--rw-rw-rw-   0 root         (0) root         (0)     5638 2022-10-13 18:45:54.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/character_viewer.css
--rw-rw-rw-   0 root         (0) root         (0)     2540 2021-01-29 15:59:17.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/data_export.css
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-04 21:32:43.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      646 2021-01-29 15:59:17.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/global.min.css
--rw-rw-rw-   0 root         (0) root         (0)     4331 2020-11-03 21:09:40.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/launcher.css
--rw-rw-rw-   0 root         (0) root         (0)     2765 2021-01-29 15:59:17.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/launcher.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1363 2021-02-16 17:03:36.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/memberaudit.css
--rw-rw-rw-   0 root         (0) root         (0)      617 2021-02-16 17:03:36.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-rw-rw-   0 root         (0) root         (0)      611 2021-02-17 10:40:00.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/reports.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.814360 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2020-10-26 16:42:17.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2020-10-26 16:42:17.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)     1862 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/charisma.png
--rw-rw-rw-   0 root         (0) root         (0)      694 2020-11-03 21:09:40.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/eve-prism.png
--rw-rw-rw-   0 root         (0) root         (0)      220 2020-11-03 21:09:40.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/evelogo.png
--rw-rw-rw-   0 root         (0) root         (0)      595 2020-11-03 21:09:40.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/evesearch.png
--rw-rw-rw-   0 root         (0) root         (0)     1966 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/intelligence.png
--rw-rw-rw-   0 root         (0) root         (0)     1809 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/memory.png
--rw-rw-rw-   0 root         (0) root         (0)     1803 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/perception.png
--rw-rw-rw-   0 root         (0) root         (0)     1782 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/willpower.png
--rw-rw-rw-   0 root         (0) root         (0)      259 2020-10-22 17:18:29.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/zkillboard.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.790360 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.790360 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.818359 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5573 2020-10-22 17:18:29.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-01 19:48:30.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.818359 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/moment/
--rw-rw-rw-   0 root         (0) root         (0)    69950 2020-10-28 14:46:25.000000 aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)   881821 2023-02-16 19:01:05.000000 aa-memberaudit-2.6.0/memberaudit/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)    39964 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.794360 aa-memberaudit-2.6.0/memberaudit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.794360 aa-memberaudit-2.6.0/memberaudit/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.794360 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.818359 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/character/
--rw-rw-rw-   0 root         (0) root         (0)      640 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.818359 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/skillset/
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-rw-rw-   0 root         (0) root         (0)      830 2022-09-03 16:21:19.000000 aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.818359 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      367 2020-12-07 00:53:01.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/base.html
--rw-rw-rw-   0 root         (0) root         (0)     4679 2022-04-01 19:48:30.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/character_finder.html
--rw-rw-rw-   0 root         (0) root         (0)    27476 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/character_viewer.html
--rw-rw-rw-   0 root         (0) root         (0)     2669 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/data_export.html
--rw-rw-rw-   0 root         (0) root         (0)     8152 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/launcher.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.794360 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.822359 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     1238 2021-01-29 15:52:00.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-rw-rw-   0 root         (0) root         (0)     4307 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2021-02-18 07:41:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1246 2020-11-01 21:48:51.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-rw-rw-   0 root         (0) root         (0)     8003 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-rw-rw-   0 root         (0) root         (0)      640 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-09 21:55:36.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-09 21:55:36.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-rw-rw-   0 root         (0) root         (0)     3880 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.822359 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.822359 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     9001 2022-07-22 18:45:02.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     1359 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-rw-rw-   0 root         (0) root         (0)      561 2021-02-18 10:40:48.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.826360 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/
--rw-rw-rw-   0 root         (0) root         (0)     1218 2021-01-29 15:52:00.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-rw-rw-   0 root         (0) root         (0)      520 2021-02-23 10:36:55.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-rw-rw-   0 root         (0) root         (0)     2604 2021-02-23 15:40:36.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-02-08 21:33:10.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-rw-rw-   0 root         (0) root         (0)      808 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-rw-rw-   0 root         (0) root         (0)      919 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      543 2020-11-09 19:29:14.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2020-12-14 23:31:49.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-rw-rw-   0 root         (0) root         (0)     2768 2023-03-22 22:31:11.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-rw-rw-   0 root         (0) root         (0)      505 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-rw-rw-   0 root         (0) root         (0)      678 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-rw-rw-   0 root         (0) root         (0)      148 2020-11-09 19:29:14.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-rw-rw-   0 root         (0) root         (0)      572 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2022-02-09 21:55:36.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2022-10-13 17:41:55.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)      626 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-rw-rw-   0 root         (0) root         (0)      822 2021-02-16 14:35:06.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      554 2020-11-14 02:21:27.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-rw-rw-   0 root         (0) root         (0)      889 2021-01-25 17:36:44.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-rw-rw-   0 root         (0) root         (0)      898 2021-01-25 17:36:44.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-23 15:08:18.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.826360 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.826360 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-02-16 15:13:05.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      742 2022-04-01 19:28:56.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      887 2021-02-17 10:40:00.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-16 15:13:05.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)      675 2020-11-09 19:29:14.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-rw-rw-   0 root         (0) root         (0)     9420 2022-04-01 19:56:47.000000 aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/reports.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.830360 aa-memberaudit-2.6.0/memberaudit/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:18:30.000000 aa-memberaudit-2.6.0/memberaudit/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2021-01-05 22:10:38.000000 aa-memberaudit-2.6.0/memberaudit/templatetags/memberaudit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.830360 aa-memberaudit-2.6.0/memberaudit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-29 20:04:28.000000 aa-memberaudit-2.6.0/memberaudit/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.834360 aa-memberaudit-2.6.0/memberaudit/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6340 2022-07-14 11:30:46.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_core_xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    20438 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4627 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2022-09-03 21:36:22.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2022-09-02 18:40:08.000000 aa-memberaudit-2.6.0/memberaudit/tests/core/test_skills.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.834360 aa-memberaudit-2.6.0/memberaudit/tests/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18357 2023-02-24 14:11:29.000000 aa-memberaudit-2.6.0/memberaudit/tests/managers/test_character.py
--rw-rw-rw-   0 root         (0) root         (0)    39823 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/managers/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     3382 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/managers/test_sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.838359 aa-memberaudit-2.6.0/memberaudit/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34701 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_1.py
--rw-rw-rw-   0 root         (0) root         (0)    35834 2023-02-16 19:01:05.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_2.py
--rw-rw-rw-   0 root         (0) root         (0)    40698 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_3.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-03-22 21:45:48.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_4.py
--rw-rw-rw-   0 root         (0) root         (0)    10448 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-22 22:31:11.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/test_sections.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/models/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11633 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-02-24 17:52:57.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-08-07 14:05:02.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3516 2022-09-03 16:21:19.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2023-02-24 17:52:57.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    12216 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-05 14:47:06.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)    36109 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2021-05-04 15:11:43.000000 aa-memberaudit-2.6.0/memberaudit/tests/test_templatetags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.842360 aa-memberaudit-2.6.0/memberaudit/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      267 2020-10-22 17:18:30.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2022-10-12 21:43:27.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2022-02-10 22:57:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/entities.json
--rw-rw-rw-   0 root         (0) root         (0)     4703 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)    40192 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/esi_testdata.json
--rw-rw-rw-   0 root         (0) root         (0)  1159197 2022-10-12 21:43:27.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)    11769 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.846360 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      799 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-rw-rw-   0 root         (0) root         (0)      700 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-rw-rw-   0 root         (0) root         (0)      460 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-01-20 23:34:01.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/generate_character.py
--rw-rw-rw-   0 root         (0) root         (0)     3859 2022-01-20 23:34:01.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/generate_doctrines.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/load_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2020-10-22 17:18:30.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2022-02-10 21:29:55.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/load_locations.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/testdata/profiler_toolbox.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.850360 aa-memberaudit-2.6.0/memberaudit/tests/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2022-09-03 16:21:19.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    32680 2023-03-22 21:45:48.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22475 2022-10-13 12:47:37.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)    14577 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_characters.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    16230 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/tests/views/test_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     7031 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.850360 aa-memberaudit-2.6.0/memberaudit/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2022-04-01 19:33:31.000000 aa-memberaudit-2.6.0/memberaudit/views/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4636 2022-09-03 16:21:19.000000 aa-memberaudit-2.6.0/memberaudit/views/admin.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/views/character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    25425 2023-03-22 20:57:15.000000 aa-memberaudit-2.6.0/memberaudit/views/character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22486 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/memberaudit/views/character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)     7845 2023-03-22 16:51:39.000000 aa-memberaudit-2.6.0/memberaudit/views/characters.py
--rw-rw-rw-   0 root         (0) root         (0)     2186 2022-11-27 20:20:23.000000 aa-memberaudit-2.6.0/memberaudit/views/data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    13074 2022-08-07 14:41:41.000000 aa-memberaudit-2.6.0/memberaudit/views/reports.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-03-23 14:29:25.000000 aa-memberaudit-2.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1522 2023-03-23 15:11:54.854359 aa-memberaudit-2.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:11:54.850360 aa-memberaudit-2.6.0/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2020-10-22 17:18:30.000000 aa-memberaudit-2.6.0/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-05-04 15:11:43.000000 aa-memberaudit-2.6.0/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10412 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-02-24 17:11:11.000000 aa-memberaudit-2.6.0/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2020-10-22 17:18:30.000000 aa-memberaudit-2.6.0/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:29.013099 aa_memberaudit-2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)    25013 2023-04-08 19:04:21.000000 aa_memberaudit-2.6.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-07 16:50:18.000000 aa_memberaudit-2.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-27 13:03:22.000000 aa_memberaudit-2.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-04-08 19:47:29.013099 aa_memberaudit-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2023-03-23 15:22:24.000000 aa_memberaudit-2.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15032 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-08 19:47:28.000000 aa_memberaudit-2.6.1/aa_memberaudit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.897099 aa_memberaudit-2.6.1/memberaudit/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-08 19:04:21.000000 aa_memberaudit-2.6.1/memberaudit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21864 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.1/memberaudit/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-03-22 20:38:17.000000 aa_memberaudit-2.6.1/memberaudit/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.1/memberaudit/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.897099 aa_memberaudit-2.6.1/memberaudit/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 17:29:05.000000 aa_memberaudit-2.6.1/memberaudit/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11673 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/core/data_exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)    19049 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.1/memberaudit/core/eft_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5305 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.1/memberaudit/core/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.1/memberaudit/core/skill_plans.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.1/memberaudit/core/skills.py
+-rw-rw-rw-   0 root         (0) root         (0)     3150 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.1/memberaudit/core/xml_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2336 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.1/memberaudit/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20772 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20766 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20766 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/ko/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/ko/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20759 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20910 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.953099 aa_memberaudit-2.6.1/memberaudit/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    20759 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.957099 aa_memberaudit-2.6.1/memberaudit/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2020-11-24 21:31:34.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_update_characters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.901099 aa_memberaudit-2.6.1/memberaudit/managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-18 15:52:38.000000 aa_memberaudit-2.6.1/memberaudit/managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13007 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.1/memberaudit/managers/character.py
+-rw-rw-rw-   0 root         (0) root         (0)    21180 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/managers/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    48369 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/managers/sections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.905099 aa_memberaudit-2.6.1/memberaudit/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    65995 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.1/memberaudit/migrations/0001_initial_new.py
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.1/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.1/memberaudit/migrations/0003_add_notify_permission.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.1/memberaudit/migrations/0004_character_is_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/migrations/0005_add_fw_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.1/memberaudit/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.905099 aa_memberaudit-2.6.1/memberaudit/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    53140 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/models/character.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2021-01-17 22:43:01.000000 aa_memberaudit-2.6.1/memberaudit/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    14223 2022-10-21 17:48:21.000000 aa_memberaudit-2.6.1/memberaudit/models/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    39924 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.1/memberaudit/models/sections.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-17 10:57:57.000000 aa_memberaudit-2.6.1/memberaudit/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.1/memberaudit/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.965099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/character_finder.css
+-rw-rw-rw-   0 root         (0) root         (0)     5638 2022-10-13 18:45:54.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/data_export.css
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-04 21:32:43.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/global.css
+-rw-rw-rw-   0 root         (0) root         (0)      646 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/global.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/launcher.css
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-rw-rw-   0 root         (0) root         (0)      617 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-rw-rw-   0 root         (0) root         (0)      611 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/reports.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.973099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43262 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-rw-rw-   0 root         (0) root         (0)    43381 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/charisma.png
+-rw-rw-rw-   0 root         (0) root         (0)      694 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-rw-rw-   0 root         (0) root         (0)      220 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/evelogo.png
+-rw-rw-rw-   0 root         (0) root         (0)      595 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/evesearch.png
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/intelligence.png
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/memory.png
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/perception.png
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/willpower.png
+-rw-rw-rw-   0 root         (0) root         (0)      259 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/zkillboard.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.877099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.973099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     5573 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.973099 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/moment/
+-rw-rw-rw-   0 root         (0) root         (0)    69950 2020-10-28 14:46:25.000000 aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)   881821 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.1/memberaudit/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)    39964 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.881099 aa_memberaudit-2.6.1/memberaudit/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.881099 aa_memberaudit-2.6.1/memberaudit/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.881099 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.977099 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/character/
+-rw-rw-rw-   0 root         (0) root         (0)      640 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.977099 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/skillset/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      830 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.981099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/
+-rw-rw-rw-   0 root         (0) root         (0)      367 2020-12-07 00:53:01.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/character_finder.html
+-rw-rw-rw-   0 root         (0) root         (0)    27476 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/character_viewer.html
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/data_export.html
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/launcher.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.881099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.985099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2021-02-18 07:41:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2020-11-01 21:48:51.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-rw-rw-   0 root         (0) root         (0)     8003 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      640 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.985099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.985099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)     9001 2022-07-22 18:45:02.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-rw-rw-   0 root         (0) root         (0)      561 2021-02-18 10:40:48.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.997099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-rw-rw-   0 root         (0) root         (0)      520 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2021-02-23 15:40:36.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      279 2022-02-08 21:33:10.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-rw-rw-   0 root         (0) root         (0)      808 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-rw-rw-   0 root         (0) root         (0)      919 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      543 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-rw-rw-   0 root         (0) root         (0)      894 2020-12-14 23:31:49.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-rw-rw-   0 root         (0) root         (0)     2768 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      505 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-rw-rw-   0 root         (0) root         (0)      678 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-rw-rw-   0 root         (0) root         (0)      148 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-rw-rw-   0 root         (0) root         (0)      572 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-rw-rw-   0 root         (0) root         (0)      741 2022-10-13 17:41:55.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-rw-rw-   0 root         (0) root         (0)      626 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-rw-rw-   0 root         (0) root         (0)      822 2021-02-16 14:35:06.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-rw-rw-   0 root         (0) root         (0)      554 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-rw-rw-   0 root         (0) root         (0)      889 2021-01-25 17:36:44.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-rw-rw-   0 root         (0) root         (0)      898 2021-01-25 17:36:44.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-23 15:08:18.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.997099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.997099 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/
+-rw-rw-rw-   0 root         (0) root         (0)      796 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-rw-rw-   0 root         (0) root         (0)      742 2022-04-01 19:28:56.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-rw-rw-   0 root         (0) root         (0)      887 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-rw-rw-   0 root         (0) root         (0)      675 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-rw-rw-   0 root         (0) root         (0)     9420 2022-04-01 19:56:47.000000 aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/reports.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.909099 aa_memberaudit-2.6.1/memberaudit/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.1/memberaudit/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2021-01-05 22:10:38.000000 aa_memberaudit-2.6.1/memberaudit/templatetags/memberaudit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.917099 aa_memberaudit-2.6.1/memberaudit/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-29 20:04:28.000000 aa_memberaudit-2.6.1/memberaudit/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.921099 aa_memberaudit-2.6.1/memberaudit/tests/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6340 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_core_xml_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    12708 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_data_exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)    20438 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_eft_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4627 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4082 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_skill_plans.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.1/memberaudit/tests/core/test_skills.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.925099 aa_memberaudit-2.6.1/memberaudit/tests/managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18357 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.1/memberaudit/tests/managers/test_character.py
+-rw-rw-rw-   0 root         (0) root         (0)    39823 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/managers/test_general.py
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/managers/test_sections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.929099 aa_memberaudit-2.6.1/memberaudit/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34701 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    35834 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    40698 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_3.py
+-rw-rw-rw-   0 root         (0) root         (0)    28275 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_4.py
+-rw-rw-rw-   0 root         (0) root         (0)    10448 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/test_sections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/models/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11633 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-08-07 14:05:02.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12216 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)    36109 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.1/memberaudit/tests/test_templatetags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.941099 aa_memberaudit-2.6.1/memberaudit/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2022-02-10 22:57:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/entities.json
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/esi_client_stub.py
+-rw-rw-rw-   0 root         (0) root         (0)    40192 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/esi_testdata.json
+-rw-rw-rw-   0 root         (0) root         (0)  1159197 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/eveuniverse.json
+-rw-rw-rw-   0 root         (0) root         (0)    11769 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:29.009099 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-rw-rw-   0 root         (0) root         (0)      503 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      700 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      410 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/generate_character.py
+-rw-rw-rw-   0 root         (0) root         (0)     3859 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/generate_doctrines.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/load_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2022-02-10 21:29:55.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/load_locations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.945099 aa_memberaudit-2.6.1/memberaudit/tests/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    32680 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_viewer_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    22475 2022-10-13 12:47:37.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_viewer_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    14577 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_characters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)    16230 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/tests/views/test_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:29.009099 aa_memberaudit-2.6.1/memberaudit/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2022-10-21 18:07:26.000000 aa_memberaudit-2.6.1/memberaudit/tools/drop_tables.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2020-12-16 22:00:54.000000 aa_memberaudit-2.6.1/memberaudit/tools/total_size.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7031 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 19:47:28.949099 aa_memberaudit-2.6.1/memberaudit/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.1/memberaudit/views/_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.1/memberaudit/views/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)    12471 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/views/character_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    25425 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.1/memberaudit/views/character_viewer_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    22486 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.1/memberaudit/views/character_viewer_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.1/memberaudit/views/characters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2186 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.1/memberaudit/views/data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)    13074 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.1/memberaudit/views/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-04-08 19:47:29.013099 aa_memberaudit-2.6.1/setup.cfg
```

### Comparing `aa-memberaudit-2.6.0/LICENSE` & `aa_memberaudit-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/PKG-INFO` & `aa_memberaudit-2.6.1/aa_memberaudit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.6.0
+Version: 2.6.1
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Home-page: https://gitlab.com/ErikKalkoken/aa-memberaudit
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
-Keywords: allianceauth
+Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Member Audit
@@ -67,17 +69,19 @@
 - Leadership can get full access to characters of their members for auditing (e.g. to check suspicious members)
 - Full access to characters currently includes the following information:
   - Assets
   - Bio
   - Contacts
   - Contracts
   - Corporation history
+  - Faction Warfare statistics
   - Implants
   - Jump clones
   - Mails
+  - Mining ledger
   - Loyalty points
   - Skill queue
   - Skill sets
   - Skills
   - Wallet (journal and transactions)
 
 - Leadership can define Skill Sets, which are a way of defining skills needed to perform a specific activity or fly a doctrine ship. They allow recruiters and leadership to see at a glance what a character can do (e.g. which doctrine ships he/she can fly)
@@ -85,15 +89,15 @@
 - Leadership can see reports and analytics about their members. Those currently include:
   - Compliance: if users have added all their characters
   - Skill Sets: which character has which skill sets
 
 - Admins can use the flexible permission system to grant access levels for different roles (e.g. corp leadership may only have access to reports about their own corp members)
 - Admins can customize and configure Member Audit to fit their needs. e.g. change the app's name and define how often which type of data is updated from the Eve server
 
-- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](#compliance-groups))
+- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](https://aa-memberaudit.readthedocs.io/en/latest/user.html#compliance-groups))
 - Get notifications when a user removes a character that they had previously registered.
 - Designed to work efficiently with large number of characters
 - Data retention policy allows managing storage capacity needs
 - Data can be exported for processing it with third party apps like Google Sheets (currently wallet journal only)
 
 ## Highlights
```

### Comparing `aa-memberaudit-2.6.0/README.md` & `aa_memberaudit-2.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,19 @@
 - Leadership can get full access to characters of their members for auditing (e.g. to check suspicious members)
 - Full access to characters currently includes the following information:
   - Assets
   - Bio
   - Contacts
   - Contracts
   - Corporation history
+  - Faction Warfare statistics
   - Implants
   - Jump clones
   - Mails
+  - Mining ledger
   - Loyalty points
   - Skill queue
   - Skill sets
   - Skills
   - Wallet (journal and transactions)
 
 - Leadership can define Skill Sets, which are a way of defining skills needed to perform a specific activity or fly a doctrine ship. They allow recruiters and leadership to see at a glance what a character can do (e.g. which doctrine ships he/she can fly)
@@ -60,15 +62,15 @@
 - Leadership can see reports and analytics about their members. Those currently include:
   - Compliance: if users have added all their characters
   - Skill Sets: which character has which skill sets
 
 - Admins can use the flexible permission system to grant access levels for different roles (e.g. corp leadership may only have access to reports about their own corp members)
 - Admins can customize and configure Member Audit to fit their needs. e.g. change the app's name and define how often which type of data is updated from the Eve server
 
-- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](#compliance-groups))
+- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](https://aa-memberaudit.readthedocs.io/en/latest/user.html#compliance-groups))
 - Get notifications when a user removes a character that they had previously registered.
 - Designed to work efficiently with large number of characters
 - Data retention policy allows managing storage capacity needs
 - Data can be exported for processing it with third party apps like Google Sheets (currently wallet journal only)
 
 ## Highlights
```

### Comparing `aa-memberaudit-2.6.0/aa_memberaudit.egg-info/PKG-INFO` & `aa_memberaudit-2.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
-Name: aa-memberaudit
-Version: 2.6.0
+Name: aa_memberaudit
+Version: 2.6.1
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Home-page: https://gitlab.com/ErikKalkoken/aa-memberaudit
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
-Keywords: allianceauth
+Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Member Audit
@@ -67,17 +69,19 @@
 - Leadership can get full access to characters of their members for auditing (e.g. to check suspicious members)
 - Full access to characters currently includes the following information:
   - Assets
   - Bio
   - Contacts
   - Contracts
   - Corporation history
+  - Faction Warfare statistics
   - Implants
   - Jump clones
   - Mails
+  - Mining ledger
   - Loyalty points
   - Skill queue
   - Skill sets
   - Skills
   - Wallet (journal and transactions)
 
 - Leadership can define Skill Sets, which are a way of defining skills needed to perform a specific activity or fly a doctrine ship. They allow recruiters and leadership to see at a glance what a character can do (e.g. which doctrine ships he/she can fly)
@@ -85,15 +89,15 @@
 - Leadership can see reports and analytics about their members. Those currently include:
   - Compliance: if users have added all their characters
   - Skill Sets: which character has which skill sets
 
 - Admins can use the flexible permission system to grant access levels for different roles (e.g. corp leadership may only have access to reports about their own corp members)
 - Admins can customize and configure Member Audit to fit their needs. e.g. change the app's name and define how often which type of data is updated from the Eve server
 
-- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](#compliance-groups))
+- Ensure that only users who have registered all their characters have access to services (see also [Compliance Groups](https://aa-memberaudit.readthedocs.io/en/latest/user.html#compliance-groups))
 - Get notifications when a user removes a character that they had previously registered.
 - Designed to work efficiently with large number of characters
 - Data retention policy allows managing storage capacity needs
 - Data can be exported for processing it with third party apps like Google Sheets (currently wallet journal only)
 
 ## Highlights
```

### Comparing `aa-memberaudit-2.6.0/memberaudit/admin.py` & `aa_memberaudit-2.6.1/memberaudit/admin.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/app_settings.py` & `aa_memberaudit-2.6.1/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/auth_hooks.py` & `aa_memberaudit-2.6.1/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/checks.py` & `aa_memberaudit-2.6.1/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/constants.py` & `aa_memberaudit-2.6.1/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.6.1/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.6.1/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/fittings.py` & `aa_memberaudit-2.6.1/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.6.1/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/skills.py` & `aa_memberaudit-2.6.1/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.6.1/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/decorators.py` & `aa_memberaudit-2.6.1/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/forms.py` & `aa_memberaudit-2.6.1/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/helpers.py` & `aa_memberaudit-2.6.1/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.6.1/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/managers/character.py` & `aa_memberaudit-2.6.1/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/managers/general.py` & `aa_memberaudit-2.6.1/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/managers/sections.py` & `aa_memberaudit-2.6.1/memberaudit/managers/sections.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.6.1/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.6.1/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.6.1/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.6.1/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.6.1/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/models/__init__.py` & `aa_memberaudit-2.6.1/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/models/character.py` & `aa_memberaudit-2.6.1/memberaudit/models/character.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/models/general.py` & `aa_memberaudit-2.6.1/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/models/sections.py` & `aa_memberaudit-2.6.1/memberaudit/models/sections.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.6.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/swagger.json` & `aa_memberaudit-2.6.1/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tasks.py` & `aa_memberaudit-2.6.1/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.6.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.6.1/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.6.1/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.6.1/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.6.1/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/managers/test_sections.py` & `aa_memberaudit-2.6.1/memberaudit/tests/managers/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_1.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_2.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_3.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_character_4.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/models/utils.py` & `aa_memberaudit-2.6.1/memberaudit/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.6.1/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.6.1/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/utils.py` & `aa_memberaudit-2.6.1/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.6.1/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/urls.py` & `aa_memberaudit-2.6.1/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/_common.py` & `aa_memberaudit-2.6.1/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/admin.py` & `aa_memberaudit-2.6.1/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/character_finder.py` & `aa_memberaudit-2.6.1/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.6.1/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.6.1/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/characters.py` & `aa_memberaudit-2.6.1/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/data_export.py` & `aa_memberaudit-2.6.1/memberaudit/views/data_export.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/memberaudit/views/reports.py` & `aa_memberaudit-2.6.1/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa-memberaudit-2.6.0/setup.cfg` & `aa_memberaudit-2.6.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 [metadata]
-name = aa-memberaudit
+name = aa_memberaudit
 version = attr: memberaudit.__version__
-author = Erik Kalkoken
-author_email = kalkoken87@gmail.com
 description = An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/ErikKalkoken/aa-memberaudit
-keywords = allianceauth
+author = Erik Kalkoken
+author_email = kalkoken87@gmail.com
 license = MIT
+license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
+	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
+keywords = 
+	allianceauth
+	eveonline
+	memberaudit
 
 [options]
-include_package_data = True
-packages = find_namespace:
-python_requires = ~=3.8
+packages = find:
 install_requires = 
 	allianceauth>=3
-	django-eveuniverse>=0.19
 	allianceauth-app-utils>=1.16.1
-	humanize
-	dj-datatables-view
 	bleach
+	dj-datatables-view
+	django-eveuniverse>=0.19
+	humanize
 	unidecode
+python_requires = ~=3.8
+include_package_data = True
+package_dir = 
+	=.
+zip_safe = False
+
+[options.packages.find]
+include = memberaudit*
+
+[options.package_data]
+* = *
 
 [flake8]
 exclude = .git, *migrations*, .tox, dist, htmlcov
 max-line-length = 88
 select = C,E,F,W,B,B950
 ignore = E203, E231, E501, W503, W291, W293
```

