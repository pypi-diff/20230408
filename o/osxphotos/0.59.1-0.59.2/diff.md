# Comparing `tmp/osxphotos-0.59.1.tar.gz` & `tmp/osxphotos-0.59.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.59.1.tar", last modified: Mon Apr  3 02:59:43 2023, max compression
+gzip compressed data, was "osxphotos-0.59.2.tar", last modified: Sat Apr  8 19:03:54 2023, max compression
```

## Comparing `osxphotos-0.59.1.tar` & `osxphotos-0.59.2.tar`

### file list

```diff
@@ -1,230 +1,231 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.514163 osxphotos-0.59.1/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.59.1/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.59.1/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-03 02:59:43.513965 osxphotos-0.59.1/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   222713 2023-04-03 02:59:32.000000 osxphotos-0.59.1/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.59.1/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.461929 osxphotos-0.59.1/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1850 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.59.1/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15928 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-04-03 02:59:28.000000 osxphotos-0.59.1/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.59.1/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    17651 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.473166 osxphotos-0.59.1/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3482 2023-02-25 22:39:05.000000 osxphotos-0.59.1/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.59.1/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6838 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9875 2023-03-14 19:25:07.000000 osxphotos-0.59.1/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3628 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    24737 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8517 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.59.1/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      433 2022-03-05 15:19:39.000000 osxphotos-0.59.1/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3457 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106579 2023-04-03 02:44:56.000000 osxphotos-0.59.1/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    21765 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61618 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.59.1/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9663 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20532 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5361 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7033 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23014 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.59.1/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3324 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26903 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.59.1/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    27999 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.59.1/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      633 2022-02-27 00:52:03.000000 osxphotos-0.59.1/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.59.1/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5058 2022-04-30 16:26:36.000000 osxphotos-0.59.1/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-02-05 16:52:41.000000 osxphotos-0.59.1/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.59.1/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-03-24 13:39:33.000000 osxphotos-0.59.1/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.473917 osxphotos-0.59.1/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.59.1/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1465753 2023-04-03 02:59:39.000000 osxphotos-0.59.1/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.59.1/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.59.1/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.59.1/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10002 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5048 2022-01-22 17:22:59.000000 osxphotos-0.59.1/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.59.1/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2906 2022-02-11 06:35:24.000000 osxphotos-0.59.1/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    88910 2023-04-02 19:51:00.000000 osxphotos-0.59.1/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    80746 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46166 2023-03-31 14:06:09.000000 osxphotos-0.59.1/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5511 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5283 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.475912 osxphotos-0.59.1/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.59.1/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10370 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149198 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.59.1/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-04-03 02:59:31.000000 osxphotos-0.59.1/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78831 2023-04-03 02:45:40.000000 osxphotos-0.59.1/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.59.1/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21857 2023-03-24 13:39:33.000000 osxphotos-0.59.1/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.59.1/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.476994 osxphotos-0.59.1/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.59.1/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.59.1/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.59.1/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.59.1/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.59.1/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.59.1/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-03-24 13:39:33.000000 osxphotos-0.59.1/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-01 16:39:20.000000 osxphotos-0.59.1/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.477719 osxphotos-0.59.1/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.59.1/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3201 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.59.1/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1682 2022-05-05 04:33:09.000000 osxphotos-0.59.1/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27026 2023-03-09 14:25:54.000000 osxphotos-0.59.1/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18282 2023-04-03 02:44:56.000000 osxphotos-0.59.1/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.462632 osxphotos-0.59.1/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6285 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-04-03 02:59:43.000000 osxphotos-0.59.1/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-04-03 02:59:43.514200 osxphotos-0.59.1/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.59.1/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.513091 osxphotos-0.59.1/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-03 02:59:43.513600 osxphotos-0.59.1/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.59.1/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.59.1/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.59.1/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.59.1/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.59.1/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    53644 2023-04-02 00:24:02.000000 osxphotos-0.59.1/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   269538 2023-04-01 16:39:20.000000 osxphotos-0.59.1/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1693 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4471 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2125 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6692 2023-03-14 18:58:21.000000 osxphotos-0.59.1/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.59.1/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29889 2023-03-28 04:25:10.000000 osxphotos-0.59.1/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.59.1/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3345 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.59.1/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.59.1/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-01 16:39:20.000000 osxphotos-0.59.1/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.59.1/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1931 2020-06-13 15:30:00.000000 osxphotos-0.59.1/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.59.1/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.59.1/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.59.1/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18530 2023-04-02 19:36:56.000000 osxphotos-0.59.1/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.59.1/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.59.1/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5864 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.59.1/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.59.1/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.59.1/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.59.1/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5059 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.59.1/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.59.1/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.59.1/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.59.1/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.59.1/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.59.1/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18366 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.59.1/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50347 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.59.1/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.59.1/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13297 2021-06-30 00:44:04.000000 osxphotos-0.59.1/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.59.1/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.59.1/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.59.1/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4462 2021-12-31 05:30:53.000000 osxphotos-0.59.1/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.59.1/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.59.1/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.59.1/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.59.1/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.59.1/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.59.1/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.59.1/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.59.1/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.59.1/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.59.1/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.59.1/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    49786 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2324 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     1867 2021-11-07 16:23:19.000000 osxphotos-0.59.1/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-03 02:44:56.000000 osxphotos-0.59.1/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    46803 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.59.1/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.550893 osxphotos-0.59.2/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.59.2/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.59.2/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-08 19:03:54.550669 osxphotos-0.59.2/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   223055 2023-04-08 19:03:42.000000 osxphotos-0.59.2/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.59.2/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.466559 osxphotos-0.59.2/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1850 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.59.2/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15928 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-04-08 19:03:35.000000 osxphotos-0.59.2/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.59.2/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18234 2023-04-08 16:49:38.000000 osxphotos-0.59.2/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.483446 osxphotos-0.59.2/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3482 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.59.2/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6838 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9875 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3628 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    24737 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8517 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.59.2/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      433 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3457 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   106627 2023-04-08 16:09:26.000000 osxphotos-0.59.2/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21765 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61618 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.59.2/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9663 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20532 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5361 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7033 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23014 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.59.2/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3324 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26903 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.59.2/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28013 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.59.2/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      633 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.59.2/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5058 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.59.2/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.484249 osxphotos-0.59.2/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.59.2/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1466587 2023-04-08 19:03:51.000000 osxphotos-0.59.2/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.59.2/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.59.2/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.59.2/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10002 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5048 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.59.2/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2906 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    88922 2023-04-08 18:10:39.000000 osxphotos-0.59.2/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    81848 2023-04-08 18:10:39.000000 osxphotos-0.59.2/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46166 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5511 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5283 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.486915 osxphotos-0.59.2/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.59.2/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10370 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149198 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.59.2/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-04-08 19:03:41.000000 osxphotos-0.59.2/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78831 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.59.2/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21857 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.59.2/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.488157 osxphotos-0.59.2/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.59.2/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.59.2/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.59.2/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.59.2/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.59.2/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.59.2/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.489199 osxphotos-0.59.2/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.59.2/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3201 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.59.2/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1682 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27026 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18282 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.467600 osxphotos-0.59.2/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6319 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-04-08 19:03:54.550933 osxphotos-0.59.2/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.59.2/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.546954 osxphotos-0.59.2/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.550270 osxphotos-0.59.2/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.59.2/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.59.2/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.59.2/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.59.2/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.59.2/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54606 2023-04-08 18:10:39.000000 osxphotos-0.59.2/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   269538 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1693 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4469 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2125 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6692 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.59.2/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 18:03:50.000000 osxphotos-0.59.2/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29889 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.59.2/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3345 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.59.2/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.59.2/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.59.2/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1931 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.59.2/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.59.2/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.59.2/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18530 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.59.2/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.59.2/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5864 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.59.2/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.59.2/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.59.2/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.59.2/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5059 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.59.2/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.59.2/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.59.2/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.59.2/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.59.2/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.59.2/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18366 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.59.2/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50347 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.59.2/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.59.2/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13297 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.59.2/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.59.2/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.59.2/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.59.2/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.59.2/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.59.2/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.59.2/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.59.2/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.59.2/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.59.2/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.59.2/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.59.2/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.59.2/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.59.2/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.59.2/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    49786 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2324 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1867 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    47586 2023-04-08 18:10:39.000000 osxphotos-0.59.2/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.59.1/LICENSE` & `osxphotos-0.59.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/PKG-INFO` & `osxphotos-0.59.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.1
+Version: 0.59.2
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.1/README.md` & `osxphotos-0.59.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osxphotos)
 [![Downloads](https://static.pepy.tech/personalized-badge/osxphotos?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/osxphotos)
 [![subreddit](https://img.shields.io/reddit/subreddit-subscribers/osxphotos?style=social)](https://www.reddit.com/r/osxphotos/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-56-orange.svg?style=flat)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-57-orange.svg?style=flat)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
 
 <p align="center"><img src="docs/screencast/demo.gif?raw=true" width="713" height="430"/></p>
 
 # Table of Contents
@@ -2090,15 +2090,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.59.1'
+{osxphotos_version}             The osxphotos version, e.g. '0.59.2'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2577,15 +2577,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.59.1'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.59.2'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2700,14 +2700,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pweaver"><img src="https://avatars.githubusercontent.com/u/611620?v=4?s=75" width="75px;" alt="Pweaver"/><br /><sub><b>Pweaver</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Apweaver" title="Bug reports">🐛</a> <a href="#ideas-pweaver" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aa599"><img src="https://avatars.githubusercontent.com/u/37746269?v=4?s=75" width="75px;" alt="aa599"/><br /><sub><b>aa599</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aaa599" title="Bug reports">🐛</a> <a href="#ideas-aa599" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/swduncan"><img src="https://avatars.githubusercontent.com/u/2053195?v=4?s=75" width="75px;" alt="Steve Duncan"/><br /><sub><b>Steve Duncan</b></sub></a><br /><a href="#ideas-swduncan" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.projany.com"><img src="https://avatars.githubusercontent.com/u/15144745?v=4?s=75" width="75px;" alt="Ian Moir"/><br /><sub><b>Ian Moir</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aianmmoir" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.patreon.com/cclauss"><img src="https://avatars.githubusercontent.com/u/3709715?v=4?s=75" width="75px;" alt="Christian Clauss"/><br /><sub><b>Christian Clauss</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=cclauss" title="Code">💻</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `osxphotos-0.59.1/README.rst` & `osxphotos-0.59.2/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/__init__.py` & `osxphotos-0.59.2/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/_constants.py` & `osxphotos-0.59.2/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/adjustmentsinfo.py` & `osxphotos-0.59.2/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/albuminfo.py` & `osxphotos-0.59.2/osxphotos/albuminfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -382,15 +382,33 @@
 
 class ProjectInfo(AlbumInfo):
     """
     ProjectInfo with info about projects
     Projects are cards, calendars, slideshows, etc.
     """
 
-    ...
+    @property
+    def folder_names(self):
+        """Return hierarchical list of folders the album is contained in
+        the folder list is in form:
+        ["Top level folder", "sub folder 1", "sub folder 2", ...]
+        or empty list if album is not in any folders
+        """
+
+        # projects are not in folders
+        return []
+
+    @property
+    def folder_list(self):
+        """Returns list of FolderInfo objects for each folder the album is contained in
+        or empty list if album is not in any folders
+        """
+
+        # projects are not in folders
+        return []
 
 
 class FolderInfo:
     """
     Info about a specific folder, contains all the details about the folder
     including folders, albums, etc
     """
```

### Comparing `osxphotos-0.59.1/osxphotos/cli/__init__.py` & `osxphotos-0.59.2/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/about.py` & `osxphotos-0.59.2/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/add_locations.py` & `osxphotos-0.59.2/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/albums.py` & `osxphotos-0.59.2/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/batch_edit.py` & `osxphotos-0.59.2/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/cli.py` & `osxphotos-0.59.2/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/cli_commands.py` & `osxphotos-0.59.2/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/cli_params.py` & `osxphotos-0.59.2/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.59.2/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/color_themes.py` & `osxphotos-0.59.2/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/common.py` & `osxphotos-0.59.2/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/debug_dump.py` & `osxphotos-0.59.2/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/docs.py` & `osxphotos-0.59.2/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/dump.py` & `osxphotos-0.59.2/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.59.2/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/export.py` & `osxphotos-0.59.2/osxphotos/cli/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1438,14 +1438,15 @@
         with rich_progress(console=get_verbose_console(), mock=no_progress) as progress:
             task = progress.add_task(
                 f"Exporting [num]{num_photos}[/] photos{limit_str}", total=num_photos
             )
             for p in photos:
                 photo_num += 1
                 kwargs["photo"] = p
+                kwargs["photo_num"] = photo_num
                 export_results = export_photo(**kwargs)
                 if post_function:
                     for function in post_function:
                         # post function is tuple of (function, filename.py::function_name)
                         verbose(f"Calling post-function [bold]{function[1]}")
                         if not dry_run:
                             try:
```

### Comparing `osxphotos-0.59.1/osxphotos/cli/exportdb.py` & `osxphotos-0.59.2/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/grep.py` & `osxphotos-0.59.2/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/help.py` & `osxphotos-0.59.2/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/import_cli.py` & `osxphotos-0.59.2/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/info.py` & `osxphotos-0.59.2/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.59.2/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/keywords.py` & `osxphotos-0.59.2/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/kvstore.py` & `osxphotos-0.59.2/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/labels.py` & `osxphotos-0.59.2/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/list.py` & `osxphotos-0.59.2/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/orphans.py` & `osxphotos-0.59.2/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/param_types.py` & `osxphotos-0.59.2/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/persons.py` & `osxphotos-0.59.2/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/photo_inspect.py` & `osxphotos-0.59.2/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/places.py` & `osxphotos-0.59.2/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/print_photo_info.py` & `osxphotos-0.59.2/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/query.py` & `osxphotos-0.59.2/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/repl.py` & `osxphotos-0.59.2/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/report_writer.py` & `osxphotos-0.59.2/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/rich_progress.py` & `osxphotos-0.59.2/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/show_command.py` & `osxphotos-0.59.2/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/snap_diff.py` & `osxphotos-0.59.2/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/sync.py` & `osxphotos-0.59.2/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/sync_results.py` & `osxphotos-0.59.2/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/theme.py` & `osxphotos-0.59.2/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/timewarp.py` & `osxphotos-0.59.2/osxphotos/cli/timewarp.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 If the parse pattern includes a time zone, the photo's time will be converted from
 the specified time zone to the local time zone. osxphotos import does not
 currently support setting the time zone of imported photos.
 See also `osxphotos help timewarp` for more information on the timewarp
 command which can be used to change the time zone of photos after import.
 
 
-"""
+"""  # noqa: E501
                 ),
                 width=formatter.width,
                 markdown=True,
             )
         )
         help_text += formatter.getvalue()
         return help_text
```

### Comparing `osxphotos-0.59.1/osxphotos/cli/tutorial.py` & `osxphotos-0.59.2/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/uuid.py` & `osxphotos-0.59.2/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/verbose.py` & `osxphotos-0.59.2/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/cli/version.py` & `osxphotos-0.59.2/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/compare_exif.py` & `osxphotos-0.59.2/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/configoptions.py` & `osxphotos-0.59.2/osxphotos/configoptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.set_attributes(attrs)
 
     def set_attributes(self, args):
         for attr in self._attrs:
             try:
                 arg = args[attr]
                 # don't test 'not arg'; need to handle empty strings as valid values
-                if arg is None or arg == False:
+                if arg is None or arg is False:
                     if type(self._attrs[attr]) == tuple:
                         setattr(self, attr, ())
                     else:
                         setattr(self, attr, self._attrs[attr])
                 else:
                     setattr(self, attr, arg)
             except KeyError as e:
```

### Comparing `osxphotos-0.59.1/osxphotos/crash_reporter.py` & `osxphotos-0.59.2/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/datetime_formatter.py` & `osxphotos-0.59.2/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/datetime_utils.py` & `osxphotos-0.59.2/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/debug.py` & `osxphotos-0.59.2/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/docs/docs.zip` & `osxphotos-0.59.2/osxphotos/docs/docs.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1465753 bytes, number of entries: 99
+Zip file size: 1466587 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Apr-03 02:59 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Apr-08 19:03 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   316793 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/photoexporter.html
--rw-r--r--  3.0 unx   296574 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/phototemplate.html
--rw-r--r--  3.0 unx   200939 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/export_db.html
+-rw-r--r--  3.0 unx   316898 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   296574 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/phototemplate.html
+-rw-r--r--  3.0 unx   200939 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
--rw-r--r--  3.0 unx    49029 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   299968 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx    49029 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/fileutil.html
+-rw-r--r--  3.0 unx   302969 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29240 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   522970 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/photosdb/photosdb.html
--rw-r--r--  3.0 unx    36121 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/photosalbum.html
+-rw-r--r--  3.0 unx   522970 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    36121 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    92801 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
--rw-r--r--  3.0 unx    81685 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/albuminfo.html
+-rw-r--r--  3.0 unx    82949 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    61696 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    61696 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Apr-03 02:59 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Apr-08 19:03 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Apr-03 02:59 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Apr-08 19:03 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Apr-03 02:59 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Apr-08 19:03 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Apr-03 02:59 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Apr-08 19:03 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Apr-03 02:59 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Apr-08 19:03 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Apr-03 02:59 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Apr-08 19:03 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-Apr-03 02:59 docs/cli.html
+-rw-r--r--  3.0 unx   414459 tx defN 23-Apr-08 19:03 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243470 tx defN 23-Apr-03 02:59 docs/genindex.html
--rw-r--r--  3.0 unx   103324 tx defN 23-Apr-03 02:59 docs/index.html
+-rw-r--r--  3.0 unx   243757 tx defN 23-Apr-08 19:03 docs/genindex.html
+-rw-r--r--  3.0 unx   103771 tx defN 23-Apr-08 19:03 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9384 bx stor 23-Apr-03 02:59 docs/objects.inv
+-rw-r--r--  3.0 unx     9391 bx stor 23-Apr-08 19:03 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Apr-03 02:59 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Apr-03 02:59 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Apr-03 02:59 docs/py-modindex.html
--rw-r--r--  3.0 unx   433061 tx defN 23-Apr-03 02:59 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Apr-08 19:03 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Apr-08 19:03 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Apr-08 19:03 docs/py-modindex.html
+-rw-r--r--  3.0 unx   436053 tx defN 23-Apr-08 19:03 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Apr-03 02:59 docs/search.html
--rw-r--r--  3.0 unx   215527 tx defN 23-Apr-03 02:59 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Apr-03 02:59 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Apr-03 02:59 docs/tutorial.html
-99 files, 6891014 bytes uncompressed, 1447021 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Apr-08 19:03 docs/search.html
+-rw-r--r--  3.0 unx   215828 tx defN 23-Apr-08 19:03 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Apr-08 19:03 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Apr-08 19:03 docs/tutorial.html
+99 files, 6899418 bytes uncompressed, 1447855 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.59.1 documentation</title>
+        <title>Overview: module code - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.59.1 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1405,15 +1405,15 @@
                 <span class="o">+</span> <span class="n">update_updated_files</span>
                 <span class="o">+</span> <span class="n">update_skipped_files</span><span class="p">,</span>
                 <span class="n">options</span><span class="p">,</span>
             <span class="p">)</span>
 
         <span class="c1"># set data in the database</span>
         <span class="k">with</span> <span class="n">export_db</span><span class="o">.</span><span class="n">create_or_get_file_record</span><span class="p">(</span><span class="n">dest_str</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span> <span class="k">as</span> <span class="n">rec</span><span class="p">:</span>
-            <span class="n">rec</span><span class="o">.</span><span class="n">photoinfo</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
+            <span class="n">rec</span><span class="o">.</span><span class="n">photoinfo</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">json</span><span class="p">(</span><span class="n">shallow</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
             <span class="n">rec</span><span class="o">.</span><span class="n">export_options</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">bit_flags</span>
             <span class="c1"># don&#39;t set src_sig as that is set above before any modifications by convert_to_jpeg or exiftool</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">ignore_signature</span><span class="p">:</span>
                 <span class="n">rec</span><span class="o">.</span><span class="n">dest_sig</span> <span class="o">=</span> <span class="n">fileutil</span><span class="o">.</span><span class="n">file_sig</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
             <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">exiftool</span><span class="p">:</span>
                 <span class="n">rec</span><span class="o">.</span><span class="n">exifdata</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">exiftool_json_sidecar</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">hexdigest</span> <span class="o">!=</span> <span class="n">rec</span><span class="o">.</span><span class="n">digest</span><span class="p">:</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1395,15 +1395,15 @@
                 + update_skipped_files,
                 options,
             )
 
         # set data in the database
         with export_db.create_or_get_file_record(dest_str, self.photo.uuid) as
 rec:
-            rec.photoinfo = self.photo.json()
+            rec.photoinfo = self.photo.json(shallow=True)
             rec.export_options = options.bit_flags
             # don't set src_sig as that is set above before any modifications
 by convert_to_jpeg or exiftool
             if not options.ignore_signature:
                 rec.dest_sig = fileutil.file_sig(dest)
             if options.exiftool:
                 rec.exifdata = self.exiftool_json_sidecar(options)
```

#### docs/_modules/osxphotos/phototemplate.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.phototemplate - osxphotos 0.59.1 documentation</title>
+        <title>osxphotos.phototemplate - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/export_db.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.export_db - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos.export_db - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/fileutil.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.fileutil - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.fileutil - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -2081,30 +2081,62 @@
             <span class="s2">&quot;uti_raw&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti_raw</span><span class="p">,</span>
             <span class="s2">&quot;uti&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti</span><span class="p">,</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;visible&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">visible</span><span class="p">,</span>
             <span class="s2">&quot;width&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">width</span><span class="p">,</span>
         <span class="p">}</span></div>
 
-<div class="viewcode-block" id="PhotoInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return JSON representation&quot;&quot;&quot;</span>
+<div class="viewcode-block" id="PhotoInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">indent</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">shallow</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Return JSON representation</span>
+
+<span class="sd">        Args:</span>
+<span class="sd">            indent: indent level for JSON, if None, no indent</span>
+<span class="sd">            shallow: if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">            JSON string</span>
+<span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="n">o</span><span class="p">):</span>
             <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">o</span><span class="p">,</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="p">,</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">)):</span>
                 <span class="k">return</span> <span class="n">o</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span>
 
         <span class="n">dict_data</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
+
+        <span class="k">if</span> <span class="n">shallow</span><span class="p">:</span>
+            <span class="c1"># delete items that are not needed for shallow JSON</span>
+            <span class="c1"># these are removed to match behavior of osxphotos &lt; 0.59.0 (See #999, #1039)</span>
+            <span class="k">for</span> <span class="n">key</span> <span class="ow">in</span> <span class="p">[</span>
+                <span class="s2">&quot;adjustments&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;album_info&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_album_info&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_albums&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_default_pick&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_key&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_photos&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;burst_selected&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;cloud_metadata&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;import_info&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;labels_normalized&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;path_derivatives&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;person_info&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;project_info&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;search_info_normalized&quot;</span><span class="p">,</span>
+                <span class="s2">&quot;search_info&quot;</span><span class="p">,</span>
+            <span class="p">]:</span>
+                <span class="k">del</span> <span class="n">dict_data</span><span class="p">[</span><span class="n">key</span><span class="p">]</span>
+
         <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">dict_data</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>
             <span class="c1"># sort lists such as keywords so JSON is consistent</span>
             <span class="c1"># but do not sort certain items like location</span>
             <span class="k">if</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;location&quot;</span><span class="p">]:</span>
                 <span class="k">continue</span>
             <span class="k">if</span> <span class="n">v</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="p">(</span><span class="nb">list</span><span class="p">,</span> <span class="nb">tuple</span><span class="p">))</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="nb">dict</span><span class="p">):</span>
                 <span class="n">dict_data</span><span class="p">[</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">v</span><span class="p">:</span> <span class="n">v</span> <span class="k">if</span> <span class="n">v</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="k">else</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
-        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">dict_data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">)</span></div>
+        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">dict_data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">)</span></div>
 
     <span class="k">def</span> <span class="nf">_json_hexdigest</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;JSON for use by hexdigest()&quot;&quot;&quot;</span>
 
         <span class="c1"># This differs from json() because hexdigest must not change if metadata changed</span>
         <span class="c1"># With json(), sort order of lists of dicts is not consistent but these aren&#39;t needed</span>
         <span class="c1"># for computing hexdigest so we can ignore them</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -2072,32 +2072,68 @@
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
 
-[docs]    def json(self):
-        """Return JSON representation"""
+[docs]    def json(self, indent: int | None = None, shallow: bool = False) -
+> str:
+        """Return JSON representation
+
+        Args:
+            indent: indent level for JSON, if None, no indent
+            shallow: if True, return shallow JSON representation (does not
+contain folder_info, person_info, etc.)
+
+        Returns:
+            JSON string
+        """
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
         dict_data = self.asdict()
+
+        if shallow:
+            # delete items that are not needed for shallow JSON
+            # these are removed to match behavior of osxphotos < 0.59.0 (See
+#999, #1039)
+            for key in [
+                "adjustments",
+                "album_info",
+                "burst_album_info",
+                "burst_albums",
+                "burst_default_pick",
+                "burst_key",
+                "burst_photos",
+                "burst_selected",
+                "cloud_metadata",
+                "import_info",
+                "labels_normalized",
+                "path_derivatives",
+                "person_info",
+                "project_info",
+                "search_info_normalized",
+                "search_info",
+            ]:
+                del dict_data[key]
+
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
             if v and isinstance(v, (list, tuple)) and not isinstance(v[0],
 dict):
                 dict_data[k] = sorted(v, key=lambda v: v if v is not None else
 "")
-        return json.dumps(dict_data, sort_keys=True, default=default)
+        return json.dumps(dict_data, sort_keys=True, default=default,
+indent=indent)
 
 
     def _json_hexdigest(self):
         """JSON for use by hexdigest()"""
 
         # This differs from json() because hexdigest must not change if
 metadata changed
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photosalbum.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosalbum - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.photosalbum - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/albuminfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.albuminfo - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos.albuminfo - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -579,15 +579,33 @@
 
 <div class="viewcode-block" id="ProjectInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.ProjectInfo">[docs]</a><span class="k">class</span> <span class="nc">ProjectInfo</span><span class="p">(</span><span class="n">AlbumInfo</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    ProjectInfo with info about projects</span>
 <span class="sd">    Projects are cards, calendars, slideshows, etc.</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
-    <span class="o">...</span></div>
+    <span class="nd">@property</span>
+    <span class="k">def</span> <span class="nf">folder_names</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return hierarchical list of folders the album is contained in</span>
+<span class="sd">        the folder list is in form:</span>
+<span class="sd">        [&quot;Top level folder&quot;, &quot;sub folder 1&quot;, &quot;sub folder 2&quot;, ...]</span>
+<span class="sd">        or empty list if album is not in any folders</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+
+        <span class="c1"># projects are not in folders</span>
+        <span class="k">return</span> <span class="p">[]</span>
+
+    <span class="nd">@property</span>
+    <span class="k">def</span> <span class="nf">folder_list</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Returns list of FolderInfo objects for each folder the album is contained in</span>
+<span class="sd">        or empty list if album is not in any folders</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+
+        <span class="c1"># projects are not in folders</span>
+        <span class="k">return</span> <span class="p">[]</span></div>
 
 
 <div class="viewcode-block" id="FolderInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.FolderInfo">[docs]</a><span class="k">class</span> <span class="nc">FolderInfo</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Info about a specific folder, contains all the details about the folder</span>
 <span class="sd">    including folders, albums, etc</span>
 <span class="sd">    &quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -444,15 +444,34 @@
 
 [docs]class ProjectInfo(AlbumInfo):
     """
     ProjectInfo with info about projects
     Projects are cards, calendars, slideshows, etc.
     """
 
-    ...
+    @property
+    def folder_names(self):
+        """Return hierarchical list of folders the album is contained in
+        the folder list is in form:
+        ["Top level folder", "sub folder 1", "sub folder 2", ...]
+        or empty list if album is not in any folders
+        """
+
+        # projects are not in folders
+        return []
+
+    @property
+    def folder_list(self):
+        """Returns list of FolderInfo objects for each folder the album is
+contained in
+        or empty list if album is not in any folders
+        """
+
+        # projects are not in folders
+        return []
 
 
 
 [docs]class FolderInfo:
     """
     Info about a specific folder, contains all the details about the folder
     including folders, albums, etc
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.59.0 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.0_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.59.1'
+     - The osxphotos version, e.g. '0.59.2'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.59.1',
+    VERSION: '0.59.2',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.59.1 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.59.2 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -3301,32 +3301,40 @@
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-import-arg-FILES">osxphotos-import command line option</a>
 </li>
         </ul></li>
         <li><a href="reference.html#osxphotos.FileUtil">FileUtil (class in osxphotos)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.ExportOptions.fileutil">fileutil (osxphotos.ExportOptions attribute)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.FileUtilNoOp">FileUtilNoOp (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoTemplate.filter_predicate">filter_predicate() (osxphotos.PhotoTemplate method)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.fingerprint">fingerprint (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.folder">folder (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotosDB.folder_info">folder_info (osxphotos.PhotosDB property)</a>
 </li>
         <li><a href="reference.html#osxphotos.AlbumInfo.folder_list">folder_list (osxphotos.AlbumInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.ProjectInfo.folder_list">(osxphotos.ProjectInfo property)</a>
 </li>
+        </ul></li>
         <li><a href="reference.html#osxphotos.AlbumInfo.folder_names">folder_names (osxphotos.AlbumInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.ProjectInfo.folder_names">(osxphotos.ProjectInfo property)</a>
 </li>
+        </ul></li>
         <li><a href="reference.html#osxphotos.FolderInfo">FolderInfo (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotosDB.folders">folders (osxphotos.PhotosDB property)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.force_update">force_update (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.from_date">from_date (osxphotos.QueryOptions attribute)</a>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1039,40 +1039,42 @@
       (osxphotos.PhotoTemplate_method)      * external_edit_
     * expand_variables_to_str()_              (osxphotos.PhotoInfo_property)
       (osxphotos.PhotoTemplate_method)            o (osxphotos.QueryOptions
                                                     attribute)
 
 ***** F *****
     * face_info_(osxphotos.PersonInfo
-      property)                           * fileutil_(osxphotos.ExportOptions
-          o (osxphotos.PhotoInfo            attribute)
-            property)                     * FileUtilNoOp_(class_in_osxphotos)
-    * face_regions_                       * filter_predicate()_
-      (osxphotos.ExportOptions              (osxphotos.PhotoTemplate_method)
-      attribute)                          * fingerprint_(osxphotos.PhotoInfo
-    * favorite_(osxphotos.PersonInfo        property)
-      property)                           * folder_(osxphotos.QueryOptions
-          o (osxphotos.PhotoInfo            attribute)
-            property)                     * folder_info_(osxphotos.PhotosDB
-          o (osxphotos.QueryOptions         property)
-            attribute)                    * folder_list_(osxphotos.AlbumInfo
-    * favorite_rating_                      property)
-      (osxphotos.ExportOptions            * folder_names_(osxphotos.AlbumInfo
-      attribute)                            property)
-    * feature_less_                       * FolderInfo_(class_in_osxphotos)
-      (osxphotos.PersonInfo_property)     * folders_(osxphotos.PhotosDB
-    * file_sig()_                           property)
-      (osxphotos.FileUtilNoOp_class       * force_update_
-      method)                               (osxphotos.ExportOptions
-    * filename_(osxphotos.PhotoInfo         attribute)
-      property)                           * from_date_(osxphotos.QueryOptions
-    * FILES                                 attribute)
-          o osxphotos-import_command      * function_(osxphotos.QueryOptions
-            line_option                     attribute)
-    * FileUtil_(class_in_osxphotos)
+      property)                             * FileUtilNoOp_(class_in_osxphotos)
+          o (osxphotos.PhotoInfo            * filter_predicate()_
+            property)                         (osxphotos.PhotoTemplate_method)
+    * face_regions_                         * fingerprint_(osxphotos.PhotoInfo
+      (osxphotos.ExportOptions                property)
+      attribute)                            * folder_(osxphotos.QueryOptions
+    * favorite_(osxphotos.PersonInfo          attribute)
+      property)                             * folder_info_(osxphotos.PhotosDB
+          o (osxphotos.PhotoInfo              property)
+            property)                       * folder_list_(osxphotos.AlbumInfo
+          o (osxphotos.QueryOptions           property)
+            attribute)                            o (osxphotos.ProjectInfo
+    * favorite_rating_                              property)
+      (osxphotos.ExportOptions              * folder_names_(osxphotos.AlbumInfo
+      attribute)                              property)
+    * feature_less_                               o (osxphotos.ProjectInfo
+      (osxphotos.PersonInfo_property)               property)
+    * file_sig()_                           * FolderInfo_(class_in_osxphotos)
+      (osxphotos.FileUtilNoOp_class         * folders_(osxphotos.PhotosDB
+      method)                                 property)
+    * filename_(osxphotos.PhotoInfo         * force_update_
+      property)                               (osxphotos.ExportOptions
+    * FILES                                   attribute)
+          o osxphotos-import_command        * from_date_(osxphotos.QueryOptions
+            line_option                       attribute)
+    * FileUtil_(class_in_osxphotos)         * function_(osxphotos.QueryOptions
+    * fileutil_(osxphotos.ExportOptions       attribute)
+      attribute)
 
 ***** G *****
     * get_db_connection()_                 * get_photo_video_type()_
       (osxphotos.PhotosDB_method)            (osxphotos.PhotoTemplate_method)
     * get_export_results()_                * get_photoinfo_for_uuid()_
       (osxphotos.ExportDB_method)            (osxphotos.ExportDB_method)
     * get_exported_files()_                * get_previous_uuids()_
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.59.1 documentation</title>
+        <title>osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -586,15 +586,19 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.photos_by_uuid"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_by_uuid()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.photos_version"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_version</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo.folder_list"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_list</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ProjectInfo.folder_names"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_names</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.QueryOptions"><code class="docutils literal notranslate"><span class="pre">QueryOptions</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.added_after"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_after</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.added_before"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_before</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.added_in_last"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_in_last</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.album"><code class="docutils literal notranslate"><span class="pre">QueryOptions.album</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.burst_photos"><code class="docutils literal notranslate"><span class="pre">QueryOptions.burst_photos</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.burst"><code class="docutils literal notranslate"><span class="pre">QueryOptions.burst</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -385,14 +385,16 @@
                 # PhotosDB.photos()
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
           o ProjectInfo
+                # ProjectInfo.folder_list
+                # ProjectInfo.folder_names
           o QueryOptions
                 # QueryOptions.added_after
                 # QueryOptions.added_before
                 # QueryOptions.added_in_last
                 # QueryOptions.album
                 # QueryOptions.burst_photos
                 # QueryOptions.burst
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -280,14 +280,16 @@
 osxphotos.PhotosDB.photos py:method 1 reference.html#$ -
 osxphotos.PhotosDB.photos_by_uuid py:method 1 reference.html#$ -
 osxphotos.PhotosDB.photos_version py:property 1 reference.html#$ -
 osxphotos.PhotosDB.project_info py:property 1 reference.html#$ -
 osxphotos.PhotosDB.query py:method 1 reference.html#$ -
 osxphotos.PlaceInfo py:class 1 reference.html#$ -
 osxphotos.ProjectInfo py:class 1 reference.html#$ -
+osxphotos.ProjectInfo.folder_list py:property 1 reference.html#$ -
+osxphotos.ProjectInfo.folder_names py:property 1 reference.html#$ -
 osxphotos.QueryOptions py:class 1 reference.html#$ -
 osxphotos.QueryOptions.added_after py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.added_before py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.added_in_last py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.album py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.burst py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.burst_photos py:attribute 1 reference.html#$ -
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.59.1 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.59.2 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1810,16 +1810,27 @@
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.isreference">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">isreference</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.isreference" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a reference (not copied to the Photos library), otherwise False</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.json">
-<span class="sig-name descname"><span class="pre">json</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.json"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.json" title="Permalink to this definition">#</a></dt>
+<span class="sig-name descname"><span class="pre">json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">indent</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shallow</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.json"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.json" title="Permalink to this definition">#</a></dt>
 <dd><p>Return JSON representation</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>indent</strong> – indent level for JSON, if None, no indent</p></li>
+<li><p><strong>shallow</strong> – if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>JSON string</p>
+</dd>
+</dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.keywords">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">keywords</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.keywords" title="Permalink to this definition">#</a></dt>
 <dd><p>list of keywords for picture</p>
 </dd></dl>
@@ -2572,14 +2583,30 @@
 <dd></dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ProjectInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ProjectInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#ProjectInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ProjectInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>ProjectInfo with info about projects
 Projects are cards, calendars, slideshows, etc.</p>
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.ProjectInfo.folder_list">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">folder_list</span></span><a class="headerlink" href="#osxphotos.ProjectInfo.folder_list" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns list of FolderInfo objects for each folder the album is contained in
+or empty list if album is not in any folders</p>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.ProjectInfo.folder_names">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">folder_names</span></span><a class="headerlink" href="#osxphotos.ProjectInfo.folder_names" title="Permalink to this definition">#</a></dt>
+<dd><p>Return hierarchical list of folders the album is contained in
+the folder list is in form:
+[“Top level folder”, “sub folder 1”, “sub folder 2”, …]
+or empty list if album is not in any folders</p>
+</dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.QueryOptions">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">QueryOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">added_after</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_before</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_in_last</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst_photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duplicate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">external_edit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">function</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">callable</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_case</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">max_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">min_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_bursts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">movies</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">person</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">query_eval</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">regex</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selected</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uti</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/queryoptions.html#QueryOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.QueryOptions" title="Permalink to this definition">#</a></dt>
 <dd><p>QueryOptions class for PhotosDB.query</p>
 <dl class="py attribute">
@@ -3993,15 +4020,19 @@
 <li><a class="reference internal" href="#osxphotos.PhotosDB.photos_by_uuid"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_by_uuid()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.photos_version"><code class="docutils literal notranslate"><span class="pre">PhotosDB.photos_version</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.project_info"><code class="docutils literal notranslate"><span class="pre">PhotosDB.project_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotosDB.query"><code class="docutils literal notranslate"><span class="pre">PhotosDB.query()</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.PlaceInfo"><code class="docutils literal notranslate"><span class="pre">PlaceInfo</span></code></a></li>
-<li><a class="reference internal" href="#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.ProjectInfo"><code class="docutils literal notranslate"><span class="pre">ProjectInfo</span></code></a><ul>
+<li><a class="reference internal" href="#osxphotos.ProjectInfo.folder_list"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_list</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.ProjectInfo.folder_names"><code class="docutils literal notranslate"><span class="pre">ProjectInfo.folder_names</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions"><code class="docutils literal notranslate"><span class="pre">QueryOptions</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.added_after"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_after</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.added_before"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_before</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.added_in_last"><code class="docutils literal notranslate"><span class="pre">QueryOptions.added_in_last</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.album"><code class="docutils literal notranslate"><span class="pre">QueryOptions.album</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.burst_photos"><code class="docutils literal notranslate"><span class="pre">QueryOptions.burst_photos</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.burst"><code class="docutils literal notranslate"><span class="pre">QueryOptions.burst</span></code></a></li>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -868,16 +868,23 @@
             Returns True if file is an image, otherwise False
         propertyisraw#
             returns True if photo is a raw image. For images with an associated
             RAW+JPEG pair, see has_raw
         propertyisreference#
             Returns True if photo is a reference (not copied to the Photos
             library), otherwise False
-        json()[source]#
+        json(indent: int | None = None, shallow: bool = False) &#x2192; str
+        [source]#
             Return JSON representation
+              Parameters:
+                      * indent â indent level for JSON, if None, no indent
+                      * shallow â if True, return shallow JSON representation
+                        (does not contain folder_info, person_info, etc.)
+              Returns:
+                  JSON string
         propertykeywords#
             list of keywords for picture
         propertylabels#
             returns list of labels applied to photo by Photos image
             categorization only valid on Photos 5, on older libraries returns
             empty list
         propertylabels_normalized#
@@ -1224,14 +1231,22 @@
             supplied options
               Parameters:
                   options â a QueryOptions instance
   classosxphotos.PlaceInfo[source]#
   classosxphotos.ProjectInfo(db, uuid)[source]#
       ProjectInfo with info about projects Projects are cards, calendars,
       slideshows, etc.
+        propertyfolder_list#
+            Returns list of FolderInfo objects for each folder the album is
+            contained in or empty list if album is not in any folders
+        propertyfolder_names#
+            Return hierarchical list of folders the album is contained in the
+            folder list is in form: [âTop level folderâ, âsub folder
+            1â, âsub folder 2â, â¦] or empty list if album is not in any
+            folders
   classosxphotos.QueryOptions(added_after: Optional[datetime] = None,
   added_before: Optional[datetime] = None, added_in_last: Optional[timedelta] =
   None, album: Optional[Iterable[str]] = None, burst_photos: Optional[bool] =
   None, burst: Optional[bool] = None, cloudasset: Optional[bool] = None,
   deleted_only: Optional[bool] = None, deleted: Optional[bool] = None,
   description: Optional[Iterable[str]] = None, duplicate: Optional[bool] =
   None, edited: Optional[bool] = None, exif: Optional[Iterable[Tuple[str,
@@ -1946,14 +1961,16 @@
                 # PhotosDB.photos()
                 # PhotosDB.photos_by_uuid()
                 # PhotosDB.photos_version
                 # PhotosDB.project_info
                 # PhotosDB.query()
           o PlaceInfo
           o ProjectInfo
+                # ProjectInfo.folder_list
+                # ProjectInfo.folder_names
           o QueryOptions
                 # QueryOptions.added_after
                 # QueryOptions.added_before
                 # QueryOptions.added_in_last
                 # QueryOptions.album
                 # QueryOptions.burst_photos
                 # QueryOptions.burst
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.59.1 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.59.2 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -2243,15 +2243,17 @@
         "restor": 0,
         "scan": 0,
         "midnight": 0,
         "batch": 1,
         "58": [],
         "cd": 5,
         "da": 5,
-        "59": 5
+        "59": 5,
+        "indent": 4,
+        "shallow": 4
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2569,14 +2571,18 @@
             [4, 3, 1, "", "persons_as_dict"],
             [4, 2, 1, "", "photos"],
             [4, 2, 1, "", "photos_by_uuid"],
             [4, 3, 1, "", "photos_version"],
             [4, 3, 1, "", "project_info"],
             [4, 2, 1, "", "query"]
         ],
+        "osxphotos.ProjectInfo": [
+            [4, 3, 1, "", "folder_list"],
+            [4, 3, 1, "", "folder_names"]
+        ],
         "osxphotos.QueryOptions": [
             [4, 4, 1, "", "added_after"],
             [4, 4, 1, "", "added_before"],
             [4, 4, 1, "", "added_in_last"],
             [4, 4, 1, "", "album"],
             [4, 4, 1, "", "burst"],
             [4, 4, 1, "", "burst_photos"],
@@ -6497,17 +6503,23 @@
         ],
         "folder_info (osxphotos.photosdb property)": [
             [4, "osxphotos.PhotosDB.folder_info"]
         ],
         "folder_list (osxphotos.albuminfo property)": [
             [4, "osxphotos.AlbumInfo.folder_list"]
         ],
+        "folder_list (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_list"]
+        ],
         "folder_names (osxphotos.albuminfo property)": [
             [4, "osxphotos.AlbumInfo.folder_names"]
         ],
+        "folder_names (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_names"]
+        ],
         "folders (osxphotos.photosdb property)": [
             [4, "osxphotos.PhotosDB.folders"]
         ],
         "force_update (osxphotos.exportoptions attribute)": [
             [4, "osxphotos.ExportOptions.force_update"]
         ],
         "from_date (osxphotos.queryoptions attribute)": [
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.59.1’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.59.2’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.59.1â
+{osxphotos_version}            The osxphotos version, e.g. â0.59.2â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.59.1 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.59.2 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.59.2_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.59.1/osxphotos/exif_datetime_updater.py` & `osxphotos-0.59.2/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/exifinfo.py` & `osxphotos-0.59.2/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/exiftool.py` & `osxphotos-0.59.2/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/exiftool_filetypes.json` & `osxphotos-0.59.2/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/export_db.py` & `osxphotos-0.59.2/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/export_db_utils.py` & `osxphotos-0.59.2/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/fileutil.py` & `osxphotos-0.59.2/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/frozen_photoinfo.py` & `osxphotos-0.59.2/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/imageconverter.py` & `osxphotos-0.59.2/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/momentinfo.py` & `osxphotos-0.59.2/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/path_utils.py` & `osxphotos-0.59.2/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/personinfo.py` & `osxphotos-0.59.2/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photodates.py` & `osxphotos-0.59.2/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photoexporter.py` & `osxphotos-0.59.2/osxphotos/photoexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1208,15 +1208,15 @@
                 + update_updated_files
                 + update_skipped_files,
                 options,
             )
 
         # set data in the database
         with export_db.create_or_get_file_record(dest_str, self.photo.uuid) as rec:
-            rec.photoinfo = self.photo.json()
+            rec.photoinfo = self.photo.json(shallow=True)
             rec.export_options = options.bit_flags
             # don't set src_sig as that is set above before any modifications by convert_to_jpeg or exiftool
             if not options.ignore_signature:
                 rec.dest_sig = fileutil.file_sig(dest)
             if options.exiftool:
                 rec.exifdata = self.exiftool_json_sidecar(options)
             if self.photo.hexdigest != rec.digest:
```

### Comparing `osxphotos-0.59.1/osxphotos/photoinfo.py` & `osxphotos-0.59.2/osxphotos/photoinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1884,30 +1884,62 @@
             "uti_raw": self.uti_raw,
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
-    def json(self):
-        """Return JSON representation"""
+    def json(self, indent: int | None = None, shallow: bool = False) -> str:
+        """Return JSON representation
+
+        Args:
+            indent: indent level for JSON, if None, no indent
+            shallow: if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)
+
+        Returns:
+            JSON string
+        """
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
         dict_data = self.asdict()
+
+        if shallow:
+            # delete items that are not needed for shallow JSON
+            # these are removed to match behavior of osxphotos < 0.59.0 (See #999, #1039)
+            for key in [
+                "adjustments",
+                "album_info",
+                "burst_album_info",
+                "burst_albums",
+                "burst_default_pick",
+                "burst_key",
+                "burst_photos",
+                "burst_selected",
+                "cloud_metadata",
+                "import_info",
+                "labels_normalized",
+                "path_derivatives",
+                "person_info",
+                "project_info",
+                "search_info_normalized",
+                "search_info",
+            ]:
+                del dict_data[key]
+
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
             if v and isinstance(v, (list, tuple)) and not isinstance(v[0], dict):
                 dict_data[k] = sorted(v, key=lambda v: v if v is not None else "")
-        return json.dumps(dict_data, sort_keys=True, default=default)
+        return json.dumps(dict_data, sort_keys=True, default=default, indent=indent)
 
     def _json_hexdigest(self):
         """JSON for use by hexdigest()"""
 
         # This differs from json() because hexdigest must not change if metadata changed
         # With json(), sort order of lists of dicts is not consistent but these aren't needed
         # for computing hexdigest so we can ignore them
```

### Comparing `osxphotos-0.59.1/osxphotos/photokit.py` & `osxphotos-0.59.2/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosalbum.py` & `osxphotos-0.59.2/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photoscript_utils.py` & `osxphotos-0.59.2/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/photosdb.py` & `osxphotos-0.59.2/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.59.2/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/phototemplate.cog.md` & `osxphotos-0.59.2/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/phototemplate.md` & `osxphotos-0.59.2/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/phototemplate.py` & `osxphotos-0.59.2/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/phototemplate.tx` & `osxphotos-0.59.2/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/phototz.py` & `osxphotos-0.59.2/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/placeinfo.py` & `osxphotos-0.59.2/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/pyrepl.py` & `osxphotos-0.59.2/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.59.2/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/query_builder.py` & `osxphotos-0.59.2/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/queryoptions.py` & `osxphotos-0.59.2/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/scoreinfo.py` & `osxphotos-0.59.2/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/searchinfo.py` & `osxphotos-0.59.2/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/sqlgrep.py` & `osxphotos-0.59.2/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/sqlite_utils.py` & `osxphotos-0.59.2/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/sqlitekvstore.py` & `osxphotos-0.59.2/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/template_counter.py` & `osxphotos-0.59.2/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.59.2/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.59.2/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/text_detection.py` & `osxphotos-0.59.2/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/timeutils.py` & `osxphotos-0.59.2/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/timezones.py` & `osxphotos-0.59.2/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/tutorial.md` & `osxphotos-0.59.2/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/uti.py` & `osxphotos-0.59.2/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos/utils.py` & `osxphotos-0.59.2/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.59.2/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.1
+Version: 0.59.2
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.1/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.59.2/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 tests/test_cli_add_locations.py
 tests/test_cli_add_to_album.py
 tests/test_cli_all_commands.py
 tests/test_cli_batch_edit.py
 tests/test_cli_dump.py
 tests/test_cli_exiftool.py
 tests/test_cli_export_cloud.py
+tests/test_cli_export_projects.py
 tests/test_cli_exportdb.py
 tests/test_cli_import.py
 tests/test_cli_orphans.py
 tests/test_cli_param_types.py
 tests/test_cli_sync.py
 tests/test_cli_timewarp.py
 tests/test_cli_utils.py
```

### Comparing `osxphotos-0.59.1/osxphotos.egg-info/requires.txt` & `osxphotos-0.59.2/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/setup.py` & `osxphotos-0.59.2/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_10_12_6.py` & `osxphotos-0.59.2/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.59.2/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.59.2/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.59.2/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_catalina_10_15_7.py` & `osxphotos-0.59.2/tests/test_catalina_10_15_7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Basic tests for Photos 5 on MacOS 10.15.7 """
 
 import datetime
+import json
 import os
 import os.path
 import pathlib
 import sqlite3
 import tempfile
 import time
 from collections import Counter, namedtuple
@@ -337,86 +338,75 @@
     mocker.patch("osxphotos.photosdb.photosdb.get_last_library_path", new=bad_library)
 
     with pytest.raises(Exception):
         assert osxphotos.PhotosDB()
 
 
 def test_db_len(photosdb):
-
     # assert photosdb.db_version in osxphotos._TESTED_DB_VERSIONS
     assert len(photosdb) == PHOTOS_DB_LEN
 
 
 def test_db_version(photosdb):
-
     # assert photosdb.db_version in osxphotos._TESTED_DB_VERSIONS
     assert photosdb.db_version == "6000"
 
 
 def test_persons(photosdb):
-
     assert "Katie" in photosdb.persons
     assert Counter(PERSONS) == Counter(photosdb.persons)
 
 
 def test_photos_version(photosdb):
     assert photosdb.photos_version == 5
 
 
 def test_keywords(photosdb):
-
     assert "wedding" in photosdb.keywords
     assert Counter(KEYWORDS) == Counter(photosdb.keywords)
 
 
 def test_album_names(photosdb):
-
     assert "Pumpkin Farm" in photosdb.albums
     assert Counter(ALBUMS) == Counter(photosdb.albums)
 
 
 def test_keywords_dict(photosdb):
-
     keywords = photosdb.keywords_as_dict
     assert keywords["wedding"] == 3
     assert keywords == KEYWORDS_DICT
 
 
 def test_persons_as_dict(photosdb):
-
     persons = photosdb.persons_as_dict
     assert persons["Maria"] == 2
     assert persons == PERSONS_DICT
 
 
 def test_albums_as_dict(photosdb):
-
     albums = photosdb.albums_as_dict
     assert albums["Pumpkin Farm"] == 3
     assert albums == ALBUM_DICT
 
 
 def test_album_sort_order(photosdb):
-
     album = [a for a in photosdb.album_info if a.title == "Pumpkin Farm"][0]
     photos = album.photos
 
     uuids = [p.uuid for p in photos]
     assert uuids == ALBUM_SORT_ORDER
 
 
 def test_album_empty_album(photosdb):
-
     album = [a for a in photosdb.album_info if a.title == "EmptyAlbum"][0]
     photos = album.photos
     assert photos == []
 
 
 def test_attributes(photosdb):
-
     photos = photosdb.photos(uuid=["D79B8D77-BFFC-460B-9312-034F2877D35B"])
     assert len(photos) == 1
     p = photos[0]
     assert p.keywords == ["Kids"]
     assert p.original_filename == "Pumkins2.jpg"
     assert p.filename == "D79B8D77-BFFC-460B-9312-034F2877D35B.jpeg"
     assert p.date == datetime.datetime(
@@ -480,48 +470,43 @@
     assert p.original_width == 2048
     assert p.orientation == 1
     assert p.original_orientation == 1
     assert p.original_filesize == 460483
 
 
 def test_missing(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["missing"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.path is None
     assert p.ismissing == True
 
 
 def test_favorite(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.favorite == True
 
 
 def test_not_favorite(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["not_favorite"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.favorite == False
 
 
 def test_hidden(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["hidden"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.hidden == True
 
 
 def test_not_hidden(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["not_hidden"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.hidden == False
 
 
 def test_visible(photosdb):
@@ -652,15 +637,14 @@
 
     photos = photosdb.photos(uuid=[UUID_DICT["no_adjustments"]])
     p = photos[0]
     assert not p.ismovie
 
 
 def test_count(photosdb):
-
     photos = photosdb.photos()
     assert len(photos) == PHOTOS_NOT_IN_TRASH_LEN
 
 
 def test_photos_intrash_1(photosdb):
     """test PhotosDB.photos(intrash=True)"""
 
@@ -731,21 +715,19 @@
 
     p = photosdb.photos(uuid=[UUID_DICT["not_intrash"]])[0]
     assert not p.intrash
     assert p.date_trashed is None
 
 
 def test_keyword_2(photosdb):
-
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
 
@@ -754,28 +736,25 @@
     """Test query with album name same as a folder name"""
 
     photos = photosdb.photos(albums=["Pumpkin Farm"])
     assert sorted(p.uuid for p in photos) == sorted(UUID_PUMPKIN_FARM)
 
 
 def test_multi_person(photosdb):
-
     photos = photosdb.photos(persons=["Katie", "Suzy"])
 
     assert len(photos) == 3
 
 
 def test_get_db_path(photosdb):
-
     db_path = photosdb.db_path
     assert db_path.endswith(PHOTOS_DB_PATH)
 
 
 def test_get_library_path(photosdb):
-
     lib_path = photosdb.library_path
     assert lib_path.endswith(PHOTOS_LIBRARY_PATH)
 
 
 def test_get_db_connection(photosdb):
     """Test PhotosDB.get_db_connection"""
 
@@ -1076,33 +1055,30 @@
     albums = photos1[0].albums
     assert albums
 
     assert photos1[0] == photos2[0]
 
 
 def test_not_eq(photosdb):
-
     photos1 = photosdb.photos(uuid=[UUID_DICT["export"]])
     photos2 = photosdb.photos(uuid=[UUID_DICT["missing"]])
     assert photos1[0] != photos2[0]
 
 
 def test_photosdb_repr():
-
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photosdb2 = eval(repr(photosdb))
 
     ignore_keys = ["_tmp_db", "_tempdir", "_tempdir_name", "_db_connection"]
     assert {k: v for k, v in photosdb.__dict__.items() if k not in ignore_keys} == {
         k: v for k, v in photosdb2.__dict__.items() if k not in ignore_keys
     }
 
 
 def test_photosinfo_repr(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"]])
     photo = photos[0]
     photo2 = eval(repr(photo))
 
     assert {k: str(v).encode("utf-8") for k, v in photo.__dict__.items()} == {
         k: str(v).encode("utf-8") for k, v in photo2.__dict__.items()
     }
@@ -1498,7 +1474,37 @@
 
 
 def test_fingerprint(photosdb):
     """Test fingerprint"""
     for uuid, fingerprint in UUID_FINGERPRINT.items():
         photo = photosdb.get_photo(uuid)
         assert photo.fingerprint == fingerprint
+
+
+def test_asdict(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.asdict()"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = photo.asdict()
+    assert photo_dict["favorite"]
+
+
+def test_json(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json()"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json())
+    assert photo_dict["favorite"]
+
+
+def test_json_indent(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json() with indent"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json(indent=4))
+    assert photo_dict["favorite"]
+    assert "album_info" in photo_dict
+
+
+def test_json_shallow(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json() with shallow=True"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json(shallow=True))
+    assert photo_dict["favorite"]
+    assert "album_info" not in photo_dict
```

### Comparing `osxphotos-0.59.1/tests/test_cli.py` & `osxphotos-0.59.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_add_locations.py` & `osxphotos-0.59.2/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_add_to_album.py` & `osxphotos-0.59.2/tests/test_cli_add_to_album.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 UUID_EXPORT = {"3DD2C897-F19E-4CA6-8C22-B027D5A71907": {"filename": "IMG_4547.jpg"}}
 UUID_MISSING = {
     "8E1D7BC9-9321-44F9-8CFB-4083F6B9232A": {"filename": "IMG_2000.JPGssss"}
 }
 
 # photos with matching names
-QUERY_NAME = "AAF035"
-QUERY_COUNT = 4
+QUERY_NAME = "IMG_"
+QUERY_COUNT = 6
 
 
 @pytest.mark.addalbum
 def test_export_add_to_album(addalbum_library):
     from osxphotos.cli import export
 
     runner = CliRunner()
```

### Comparing `osxphotos-0.59.1/tests/test_cli_all_commands.py` & `osxphotos-0.59.2/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_batch_edit.py` & `osxphotos-0.59.2/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_dump.py` & `osxphotos-0.59.2/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_exiftool.py` & `osxphotos-0.59.2/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_export_cloud.py` & `osxphotos-0.59.2/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_exportdb.py` & `osxphotos-0.59.2/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_import.py` & `osxphotos-0.59.2/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_orphans.py` & `osxphotos-0.59.2/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_param_types.py` & `osxphotos-0.59.2/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_sync.py` & `osxphotos-0.59.2/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_timewarp.py` & `osxphotos-0.59.2/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_utils.py` & `osxphotos-0.59.2/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cli_verbose.py` & `osxphotos-0.59.2/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_cloud_owner_catalina.py` & `osxphotos-0.59.2/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_comments.py` & `osxphotos-0.59.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_concurrent_export.py` & `osxphotos-0.59.2/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_configoptions.py` & `osxphotos-0.59.2/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_datetime_formatter.py` & `osxphotos-0.59.2/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_datetime_utils.py` & `osxphotos-0.59.2/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_debug.py` & `osxphotos-0.59.2/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_empty_library_4_0.py` & `osxphotos-0.59.2/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_exif_info.py` & `osxphotos-0.59.2/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_exiftool.py` & `osxphotos-0.59.2/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_exiftool_caching.py` & `osxphotos-0.59.2/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.59.2/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.59.2/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.59.2/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_db.py` & `osxphotos-0.59.2/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_exportresults.py` & `osxphotos-0.59.2/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_faceinfo.py` & `osxphotos-0.59.2/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_fileutil.py` & `osxphotos-0.59.2/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_highsierra.py` & `osxphotos-0.59.2/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_image_converter.py` & `osxphotos-0.59.2/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.59.2/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.59.2/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.59.2/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.59.2/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_monterey_12_0_1.py` & `osxphotos-0.59.2/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.59.2/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_movies_4_0.py` & `osxphotos-0.59.2/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_movies_5_0.py` & `osxphotos-0.59.2/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_path_utils.py` & `osxphotos-0.59.2/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_personinfo.py` & `osxphotos-0.59.2/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_photokit.py` & `osxphotos-0.59.2/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_photosdb_utils.py` & `osxphotos-0.59.2/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_placeinfo.py` & `osxphotos-0.59.2/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.59.2/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_projects_catalina.py` & `osxphotos-0.59.2/tests/test_projects_catalina.py`

 * *Files 14% similar despite different names*

```diff
@@ -145,7 +145,15 @@
 @pytest.mark.parametrize("uuid,expected_projects", PHOTO_PROJECTS.items())
 def test_photoinfo_project_info(photosdb, uuid, expected_projects):
     """Test PhotoInfo.project_info"""
     photo = photosdb.get_photo(uuid)
 
     project_names = [p.title for p in photo.project_info]
     assert sorted(project_names) == sorted(expected_projects)
+
+
+@pytest.mark.parametrize("uuid,expected_projects", PHOTO_PROJECTS.items())
+def test_photoinfo_project_info_asdict(photosdb, uuid, expected_projects):
+    """Test PhotoInfo.project_info.asdict() #999"""
+    photo = photosdb.get_photo(uuid)
+    for p in photo.project_info:
+        assert p.asdict()
```

### Comparing `osxphotos-0.59.1/tests/test_projects_sierra.py` & `osxphotos-0.59.2/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_score_info.py` & `osxphotos-0.59.2/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_search_info_10_14_6.py` & `osxphotos-0.59.2/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_search_info_10_15_4.py` & `osxphotos-0.59.2/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_search_info_10_15_5.py` & `osxphotos-0.59.2/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_search_info_10_15_7.py` & `osxphotos-0.59.2/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_sidecar_xmp.py` & `osxphotos-0.59.2/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.59.2/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.59.2/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.59.2/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_specials_sierra_10_12.py` & `osxphotos-0.59.2/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_sqlitekvstore.py` & `osxphotos-0.59.2/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_template.py` & `osxphotos-0.59.2/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_template_counter.py` & `osxphotos-0.59.2/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_template_today.py` & `osxphotos-0.59.2/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_uti.py` & `osxphotos-0.59.2/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_utils.py` & `osxphotos-0.59.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.1/tests/test_ventura_13_0_0.py` & `osxphotos-0.59.2/tests/test_ventura_13_0_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test macOS 13.0 Photos library"""
 
+import json
 from collections import namedtuple
 
 import pytest
 
 import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 
@@ -656,15 +657,14 @@
 
 def test_keyword_2(photosdb):
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
 
@@ -1269,7 +1269,30 @@
 def test_person_feature_less(photosdb):
     """Test person feature less"""
     photo = photosdb.get_photo(UUID_PERSON_FEATURE_LESS)
     assert photo.person_info[0].feature_less
 
     photo = photosdb.get_photo(UUID_PERSON_NOT_FEATURE_LESS)
     assert not photo.person_info[0].feature_less
+
+
+def test_json(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json()"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json())
+    assert photo_dict["favorite"]
+
+
+def test_json_indent(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json() with indent"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json(indent=4))
+    assert photo_dict["favorite"]
+    assert "album_info" in photo_dict
+
+
+def test_json_shallow(photosdb: osxphotos.PhotosDB):
+    """Test PhotoInfo.json() with shallow=True"""
+    photo = photosdb.get_photo(UUID_DICT["favorite"])
+    photo_dict = json.loads(photo.json(shallow=True))
+    assert photo_dict["favorite"]
+    assert "album_info" not in photo_dict
```

### Comparing `osxphotos-0.59.1/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.59.2/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

