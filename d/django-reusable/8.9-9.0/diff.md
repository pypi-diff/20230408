# Comparing `tmp/django-reusable-8.9.tar.gz` & `tmp/django-reusable-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-reusable-8.9.tar", last modified: Fri Apr  7 20:44:25 2023, max compression
+gzip compressed data, was "dist/django-reusable-9.0.tar", last modified: Fri Apr  7 23:28:55 2023, max compression
```

## Comparing `django-reusable-8.9.tar` & `django-reusable-9.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/
--rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-8.9/AUTHORS
--rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-8.9/COPYING
--rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-8.9/MANIFEST.in
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 20:44:25.000000 django-reusable-8.9/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-8.9/README.md
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/
--rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-8.9/django_reusable/__init__.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-8.9/django_reusable/admin/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/actions.py
--rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/filters.py
--rw-r--r--   0 narangwa   (501) staff       (20)    16952 2023-04-07 20:40:01.000000 django-reusable-8.9/django_reusable/admin/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/suit_multi_admin.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-8.9/django_reusable/admin/theme.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-8.9/django_reusable/admin/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-8.9/django_reusable/admin/utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-8.9/django_reusable/constants.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/db/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-8.9/django_reusable/db/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-8.9/django_reusable/db/query.py
--rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/db/queryset.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/django_tables2/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-8.9/django_reusable/django_tables2/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/django_tables2/columns.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-8.9/django_reusable/django_tables2/table_mixins.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/error_tracker/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-8.9/django_reusable/error_tracker/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-8.9/django_reusable/error_tracker/error_tracker.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/error_tracker/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-8.9/django_reusable/forms/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/forms/fields.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/forms/forms.py
--rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/forms/validators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-8.9/django_reusable/forms/widgets.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/logging/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-8.9/django_reusable/logging/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-8.9/django_reusable/logging/loggers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/middleware/
--rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-8.9/django_reusable/middleware/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-8.9/django_reusable/middleware/middleware.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/migrations/
--rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-8.9/django_reusable/migrations/0001_initial.py
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-8.9/django_reusable/migrations/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-8.9/django_reusable/models.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/overrides.css
--rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/theme.css
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/
--rw-r--r--   0 narangwa   (501) staff       (20)     4589 2022-05-03 18:09:49.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/dynamic-formsets.js
--rw-r--r--   0 narangwa   (501) staff       (20)     1542 2023-04-07 18:14:43.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-8.9/django_reusable/templates/admin/base.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/
--rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/add_wizard.pug
--rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/create_or_update.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/delete.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/index.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/
--rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/
--rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/detail.html
--rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/list.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/filters/
--rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-8.9/django_reusable/templates/django_reusable/filters/input-filter.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/table_form.html
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
--rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
--rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/tables/
--rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-8.9/django_reusable/templates/django_reusable/tables/enhanced-table.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templatetags/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-8.9/django_reusable/templatetags/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-8.9/django_reusable/templatetags/template_helpers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/urls/
--rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-8.9/django_reusable/urls/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-8.9/django_reusable/urls/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-8.9/django_reusable/urls/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/utils/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-8.9/django_reusable/utils/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-8.9/django_reusable/utils/date_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-8.9/django_reusable/utils/decorators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-8.9/django_reusable/utils/export_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-8.9/django_reusable/utils/file_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/utils/user_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)    16117 2023-02-28 06:04:05.000000 django-reusable-8.9/django_reusable/utils/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/views/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-8.9/django_reusable/views/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-8.9/django_reusable/views/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-8.9/django_reusable/views/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable.egg-info/
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)     3263 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable.egg-info/SOURCES.txt
--rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/dependency_links.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/requires.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/top_level.txt
--rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-8.9/manage.py
--rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-04-07 20:44:25.000000 django-reusable-8.9/setup.cfg
--rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-8.9/setup.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/
+-rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-9.0/AUTHORS
+-rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-9.0/COPYING
+-rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-9.0/MANIFEST.in
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 23:28:55.000000 django-reusable-9.0/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-9.0/README.md
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/
+-rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-9.0/django_reusable/__init__.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-9.0/django_reusable/admin/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/actions.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/filters.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    16960 2023-04-07 23:27:24.000000 django-reusable-9.0/django_reusable/admin/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/admin/suit_multi_admin.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-9.0/django_reusable/admin/theme.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-9.0/django_reusable/admin/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-9.0/django_reusable/admin/utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-9.0/django_reusable/constants.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/db/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-9.0/django_reusable/db/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-9.0/django_reusable/db/query.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/db/queryset.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/django_tables2/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-9.0/django_reusable/django_tables2/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/django_tables2/columns.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-9.0/django_reusable/django_tables2/table_mixins.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/error_tracker/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-9.0/django_reusable/error_tracker/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-9.0/django_reusable/error_tracker/error_tracker.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/error_tracker/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-9.0/django_reusable/forms/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/forms/fields.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/forms/forms.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/forms/validators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-9.0/django_reusable/forms/widgets.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/logging/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-9.0/django_reusable/logging/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-9.0/django_reusable/logging/loggers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/middleware/
+-rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-9.0/django_reusable/middleware/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-9.0/django_reusable/middleware/middleware.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/migrations/
+-rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-9.0/django_reusable/migrations/0001_initial.py
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-9.0/django_reusable/migrations/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-9.0/django_reusable/models.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/overrides.css
+-rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-9.0/django_reusable/static/django_reusable/css/admin/theme.css
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/
+-rw-r--r--   0 narangwa   (501) staff       (20)     4589 2022-05-03 18:09:49.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/dynamic-formsets.js
+-rw-r--r--   0 narangwa   (501) staff       (20)     1542 2023-04-07 18:14:43.000000 django-reusable-9.0/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-9.0/django_reusable/templates/admin/base.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/
+-rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/add_wizard.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/create_or_update.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/delete.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-9.0/django_reusable/templates/django_reusable/crud/index.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/detail.html
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/list.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/filters/
+-rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-9.0/django_reusable/templates/django_reusable/filters/input-filter.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/table_form.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templates/django_reusable/tables/
+-rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-9.0/django_reusable/templates/django_reusable/tables/enhanced-table.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/templatetags/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-9.0/django_reusable/templatetags/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-9.0/django_reusable/templatetags/template_helpers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/urls/
+-rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-9.0/django_reusable/urls/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-9.0/django_reusable/urls/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-9.0/django_reusable/urls/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/utils/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-9.0/django_reusable/utils/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-9.0/django_reusable/utils/date_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-9.0/django_reusable/utils/decorators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-9.0/django_reusable/utils/export_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-9.0/django_reusable/utils/file_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-9.0/django_reusable/utils/user_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    16117 2023-02-28 06:04:05.000000 django-reusable-9.0/django_reusable/utils/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable/views/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-9.0/django_reusable/views/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-9.0/django_reusable/views/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-9.0/django_reusable/views/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 23:28:54.000000 django-reusable-9.0/django_reusable.egg-info/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)     3263 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/SOURCES.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/dependency_links.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/requires.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-04-07 23:28:55.000000 django-reusable-9.0/django_reusable.egg-info/top_level.txt
+-rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-9.0/manage.py
+-rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-04-07 23:28:55.000000 django-reusable-9.0/setup.cfg
+-rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-9.0/setup.py
```

### Comparing `django-reusable-8.9/COPYING` & `django-reusable-9.0/COPYING`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/PKG-INFO` & `django-reusable-9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 8.9
+Version: 9.0
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-8.9/django_reusable/admin/actions.py` & `django-reusable-9.0/django_reusable/admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/admin/filters.py` & `django-reusable-9.0/django_reusable/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/admin/mixins.py` & `django-reusable-9.0/django_reusable/admin/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra_context = extra_context or {}
         if not self.auto_update_template:
             self._add_extra_change_form_buttons(request, object_id, extra_context)
             extra_context.update(
                 hide_save_buttons=self.hide_save_buttons(request, object_id)
             )
-        if request.method == 'POST' and extra_context['hide_save_buttons']:
+        if request.method == 'POST' and self.hide_save_buttons(request, object_id):
             raise PermissionDenied()
         response = super().change_view(request, object_id, form_url, extra_context)
         if request.method == 'POST':
             return self._handle_extra_change_form_buttons(request, object_id) or response
         return response
 
     def remove_inline_instances(self, inline_instances, *inlines_to_remove):
```

### Comparing `django-reusable-8.9/django_reusable/admin/suit_multi_admin.py` & `django-reusable-9.0/django_reusable/admin/suit_multi_admin.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/admin/theme.py` & `django-reusable-9.0/django_reusable/admin/theme.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/admin/urls.py` & `django-reusable-9.0/django_reusable/admin/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/admin/utils.py` & `django-reusable-9.0/django_reusable/admin/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/db/queryset.py` & `django-reusable-9.0/django_reusable/db/queryset.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/django_tables2/columns.py` & `django-reusable-9.0/django_reusable/django_tables2/columns.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/django_tables2/table_mixins.py` & `django-reusable-9.0/django_reusable/django_tables2/table_mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/error_tracker/error_tracker.py` & `django-reusable-9.0/django_reusable/error_tracker/error_tracker.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/error_tracker/views.py` & `django-reusable-9.0/django_reusable/error_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/forms/forms.py` & `django-reusable-9.0/django_reusable/forms/forms.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/forms/validators.py` & `django-reusable-9.0/django_reusable/forms/validators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/forms/widgets.py` & `django-reusable-9.0/django_reusable/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/logging/loggers.py` & `django-reusable-9.0/django_reusable/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/middleware/middleware.py` & `django-reusable-9.0/django_reusable/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/migrations/0001_initial.py` & `django-reusable-9.0/django_reusable/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/models.py` & `django-reusable-9.0/django_reusable/models.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/static/django_reusable/css/admin/overrides.css` & `django-reusable-9.0/django_reusable/static/django_reusable/css/admin/overrides.css`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/static/django_reusable/css/admin/theme.css` & `django-reusable-9.0/django_reusable/static/django_reusable/css/admin/theme.css`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/static/django_reusable/js/dynamic-formsets.js` & `django-reusable-9.0/django_reusable/static/django_reusable/js/dynamic-formsets.js`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js` & `django-reusable-9.0/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/admin/base.html` & `django-reusable-9.0/django_reusable/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/crud/add_wizard.pug` & `django-reusable-9.0/django_reusable/templates/django_reusable/crud/add_wizard.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/crud/create_or_update.pug` & `django-reusable-9.0/django_reusable/templates/django_reusable/crud/create_or_update.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/crud/delete.pug` & `django-reusable-9.0/django_reusable/templates/django_reusable/crud/delete.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/formset.pug` & `django-reusable-9.0/django_reusable/templates/django_reusable/dynamic-formset/formset.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/detail.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/list.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/forms/table_form.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/forms/table_form.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_row.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/forms/tabular_inline_row.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templates/django_reusable/tables/enhanced-table.html` & `django-reusable-9.0/django_reusable/templates/django_reusable/tables/enhanced-table.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/templatetags/template_helpers.py` & `django-reusable-9.0/django_reusable/templatetags/template_helpers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/urls/urls.py` & `django-reusable-9.0/django_reusable/urls/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/urls/utils.py` & `django-reusable-9.0/django_reusable/urls/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/date_utils.py` & `django-reusable-9.0/django_reusable/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/decorators.py` & `django-reusable-9.0/django_reusable/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/export_utils.py` & `django-reusable-9.0/django_reusable/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/file_utils.py` & `django-reusable-9.0/django_reusable/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/user_utils.py` & `django-reusable-9.0/django_reusable/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/utils/utils.py` & `django-reusable-9.0/django_reusable/utils/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/views/mixins.py` & `django-reusable-9.0/django_reusable/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable/views/views.py` & `django-reusable-9.0/django_reusable/views/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/django_reusable.egg-info/PKG-INFO` & `django-reusable-9.0/django_reusable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 8.9
+Version: 9.0
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-8.9/django_reusable.egg-info/SOURCES.txt` & `django-reusable-9.0/django_reusable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/manage.py` & `django-reusable-9.0/manage.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.9/setup.py` & `django-reusable-9.0/setup.py`

 * *Files identical despite different names*

