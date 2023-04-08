# Comparing `tmp/iommi-5.8.1.tar.gz` & `tmp/iommi-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iommi-5.8.1.tar", last modified: Tue Feb 28 07:15:55 2023, max compression
+gzip compressed data, was "iommi-5.9.0.tar", last modified: Tue Mar 28 08:52:34 2023, max compression
```

## Comparing `iommi-5.8.1.tar` & `iommi-5.9.0.tar`

### file list

```diff
@@ -1,134 +1,142 @@
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.406683 iommi-5.8.1/
--rw-r--r--   0 johanlu    (503) staff       (20)      893 2023-01-25 13:54:49.000000 iommi-5.8.1/AUTHORS.rst
--rw-r--r--   0 johanlu    (503) staff       (20)      212 2023-01-25 13:54:49.000000 iommi-5.8.1/CONTRIBUTING.rst
--rw-r--r--   0 johanlu    (503) staff       (20)    35556 2023-02-28 07:14:19.000000 iommi-5.8.1/HISTORY.rst
--rw-r--r--   0 johanlu    (503) staff       (20)     1485 2023-01-25 13:54:49.000000 iommi-5.8.1/LICENSE
--rw-r--r--   0 johanlu    (503) staff       (20)      332 2023-01-25 13:54:49.000000 iommi-5.8.1/MANIFEST.in
--rw-r--r--   0 johanlu    (503) staff       (20)     3149 2023-02-28 07:15:55.406788 iommi-5.8.1/PKG-INFO
--rw-r--r--   0 johanlu    (503) staff       (20)     2892 2023-02-08 09:18:54.000000 iommi-5.8.1/README.rst
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.395905 iommi-5.8.1/iommi/
--rw-r--r--   0 johanlu    (503) staff       (20)     3078 2023-02-28 07:15:31.000000 iommi-5.8.1/iommi/__init__.py
--rw-r--r--   0 johanlu    (503) staff       (20)     6330 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/_db_compat.py
--rw-r--r--   0 johanlu    (503) staff       (20)     6165 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/_web_compat.py
--rw-r--r--   0 johanlu    (503) staff       (20)      490 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/_web_compat_flask.py
--rw-r--r--   0 johanlu    (503) staff       (20)     5757 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/action.py
--rw-r--r--   0 johanlu    (503) staff       (20)    20956 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/admin.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1631 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/apps.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1950 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/asset.py
--rw-r--r--   0 johanlu    (503) staff       (20)     5011 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/attrs.py
--rw-r--r--   0 johanlu    (503) staff       (20)     2525 2023-02-08 09:18:54.000000 iommi-5.8.1/iommi/base.py
--rw-r--r--   0 johanlu    (503) staff       (20)     4902 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/datetime_parsing.py
--rw-r--r--   0 johanlu    (503) staff       (20)    10221 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/debug.py
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.398517 iommi-5.8.1/iommi/declarative/
--rw-r--r--   0 johanlu    (503) staff       (20)     5447 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/declarative/__init__.py
--rw-r--r--   0 johanlu    (503) staff       (20)      571 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/declarative/dispatch.py
--rw-r--r--   0 johanlu    (503) staff       (20)     7724 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/declarative/namespace.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1938 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/declarative/util.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1425 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/declarative/with_meta.py
--rw-r--r--   0 johanlu    (503) staff       (20)    11970 2023-02-08 09:18:54.000000 iommi-5.8.1/iommi/docs.py
--rw-r--r--   0 johanlu    (503) staff       (20)    16263 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/edit_table.py
--rw-r--r--   0 johanlu    (503) staff       (20)     3769 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/endpoint.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1477 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/error.py
--rw-r--r--   0 johanlu    (503) staff       (20)     4924 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/evaluate.py
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.398846 iommi-5.8.1/iommi/experimental/
--rw-r--r--   0 johanlu    (503) staff       (20)        0 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/experimental/__init__.py
--rw-r--r--   0 johanlu    (503) staff       (20)      133 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/experimental/edit_table.py
--rw-r--r--   0 johanlu    (503) staff       (20)    64957 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/form.py
--rw-r--r--   0 johanlu    (503) staff       (20)     8160 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/fragment.py
--rw-r--r--   0 johanlu    (503) staff       (20)    10054 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/from_model.py
--rw-r--r--   0 johanlu    (503) staff       (20)    19377 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/live_edit.py
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.383713 iommi-5.8.1/iommi/locale/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.383562 iommi-5.8.1/iommi/locale/de/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.399411 iommi-5.8.1/iommi/locale/de/LC_MESSAGES/
--rw-r--r--   0 johanlu    (503) staff       (20)     4463 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 johanlu    (503) staff       (20)     6167 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.383655 iommi-5.8.1/iommi/locale/sv/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.399896 iommi-5.8.1/iommi/locale/sv/LC_MESSAGES/
--rw-r--r--   0 johanlu    (503) staff       (20)     2239 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 johanlu    (503) staff       (20)     5863 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.383756 iommi-5.8.1/iommi/locale/zh_Hans/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.400535 iommi-5.8.1/iommi/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 johanlu    (503) staff       (20)     3995 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 johanlu    (503) staff       (20)     5638 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 johanlu    (503) staff       (20)    10064 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/member.py
--rw-r--r--   0 johanlu    (503) staff       (20)    10419 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/menu.py
--rw-r--r--   0 johanlu    (503) staff       (20)     3761 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/page.py
--rw-r--r--   0 johanlu    (503) staff       (20)     8267 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/part.py
--rw-r--r--   0 johanlu    (503) staff       (20)     6531 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/path.py
--rw-r--r--   0 johanlu    (503) staff       (20)     6201 2023-02-08 09:18:54.000000 iommi-5.8.1/iommi/profiling.py
--rw-r--r--   0 johanlu    (503) staff       (20)    36300 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/query.py
--rw-r--r--   0 johanlu    (503) staff       (20)     8657 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/refinable.py
--rw-r--r--   0 johanlu    (503) staff       (20)     2717 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/shortcut.py
--rw-r--r--   0 johanlu    (503) staff       (20)     2541 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/sort_after.py
--rw-r--r--   0 johanlu    (503) staff       (20)    16882 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/sql_trace.py
--rw-r--r--   0 johanlu    (503) staff       (20)     3732 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/struct.py
--rw-r--r--   0 johanlu    (503) staff       (20)    10205 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/style.py
--rw-r--r--   0 johanlu    (503) staff       (20)     4566 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/style_base.py
--rw-r--r--   0 johanlu    (503) staff       (20)     5989 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_bootstrap.py
--rw-r--r--   0 johanlu    (503) staff       (20)     6001 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_bootstrap5.py
--rw-r--r--   0 johanlu    (503) staff       (20)      518 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_bootstrap_docs.py
--rw-r--r--   0 johanlu    (503) staff       (20)      533 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_bootstrap_icons.py
--rw-r--r--   0 johanlu    (503) staff       (20)     4490 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_bulma.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1856 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_django_admin.py
--rw-r--r--   0 johanlu    (503) staff       (20)      551 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_font_awesome_4.py
--rw-r--r--   0 johanlu    (503) staff       (20)     2551 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_foundation.py
--rw-r--r--   0 johanlu    (503) staff       (20)     3644 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_semantic_ui.py
--rw-r--r--   0 johanlu    (503) staff       (20)      884 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/style_test_base.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1775 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/style_uikit.py
--rw-r--r--   0 johanlu    (503) staff       (20)      309 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/style_water.py
--rw-r--r--   0 johanlu    (503) staff       (20)     1820 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/synthetic_traceback.py
--rw-r--r--   0 johanlu    (503) staff       (20)    81715 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/table.py
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.383866 iommi-5.8.1/iommi/templates/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.401114 iommi-5.8.1/iommi/templates/iommi/
--rw-r--r--   0 johanlu    (503) staff       (20)      443 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/base.html
--rw-r--r--   0 johanlu    (503) staff       (20)        0 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/blank.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.402707 iommi-5.8.1/iommi/templates/iommi/form/
--rw-r--r--   0 johanlu    (503) staff       (20)      873 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/actions.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.402886 iommi-5.8.1/iommi/templates/iommi/form/bulma/
--rw-r--r--   0 johanlu    (503) staff       (20)      255 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/templates/iommi/form/bulma/field.html
--rw-r--r--   0 johanlu    (503) staff       (20)      495 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/choice.html
--rw-r--r--   0 johanlu    (503) staff       (20)      709 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/choice_select2.html
--rw-r--r--   0 johanlu    (503) staff       (20)      353 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/form.html
--rw-r--r--   0 johanlu    (503) staff       (20)       78 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/heading.html
--rw-r--r--   0 johanlu    (503) staff       (20)      187 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/image_row.html
--rw-r--r--   0 johanlu    (503) staff       (20)     1425 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/init_select2.js
--rw-r--r--   0 johanlu    (503) staff       (20)      415 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/radio.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.403250 iommi-5.8.1/iommi/templates/iommi/form/semantic_ui/
--rw-r--r--   0 johanlu    (503) staff       (20)      496 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/semantic_ui/radio.html
--rw-r--r--   0 johanlu    (503) staff       (20)      166 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.403434 iommi-5.8.1/iommi/templates/iommi/form/uikit/
--rw-r--r--   0 johanlu    (503) staff       (20)      379 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/templates/iommi/form/uikit/row_checkbox.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.404100 iommi-5.8.1/iommi/templates/iommi/query/
--rw-r--r--   0 johanlu    (503) staff       (20)     2622 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/query/advanced.html
--rw-r--r--   0 johanlu    (503) staff       (20)     5931 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/query/ajax_enhance.js
--rw-r--r--   0 johanlu    (503) staff       (20)     1498 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/query/form.html
--rw-r--r--   0 johanlu    (503) staff       (20)     2808 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/query/form_toggle_script.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.406010 iommi-5.8.1/iommi/templates/iommi/table/
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.406205 iommi-5.8.1/iommi/templates/iommi/table/bootstrap/
--rw-r--r--   0 johanlu    (503) staff       (20)     1526 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/bootstrap/paginator.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.406357 iommi-5.8.1/iommi/templates/iommi/table/bulma/
--rw-r--r--   0 johanlu    (503) staff       (20)     1554 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/bulma/paginator.html
--rw-r--r--   0 johanlu    (503) staff       (20)      188 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/header.html
--rw-r--r--   0 johanlu    (503) staff       (20)     2303 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/js_select_all.html
--rw-r--r--   0 johanlu    (503) staff       (20)     1814 2023-02-28 07:07:09.000000 iommi-5.8.1/iommi/templates/iommi/table/paginator.html
--rw-r--r--   0 johanlu    (503) staff       (20)      102 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/row_group.html
--rw-r--r--   0 johanlu    (503) staff       (20)      196 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/select_column_header.html
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.406529 iommi-5.8.1/iommi/templates/iommi/table/semantic_ui/
--rw-r--r--   0 johanlu    (503) staff       (20)     1091 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/semantic_ui/paginator.html
--rw-r--r--   0 johanlu    (503) staff       (20)       18 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/table.html
--rw-r--r--   0 johanlu    (503) staff       (20)      508 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/table_container.html
--rw-r--r--   0 johanlu    (503) staff       (20)      209 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/table_header_rows.html
--rw-r--r--   0 johanlu    (503) staff       (20)      453 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/templates/iommi/table/table_tag.html
--rw-r--r--   0 johanlu    (503) staff       (20)      207 2023-01-25 13:54:49.000000 iommi-5.8.1/iommi/thread_locals.py
--rw-r--r--   0 johanlu    (503) staff       (20)    11883 2023-02-08 09:18:54.000000 iommi-5.8.1/iommi/traversable.py
-drwxr-xr-x   0 johanlu    (503) staff       (20)        0 2023-02-28 07:15:55.397213 iommi-5.8.1/iommi.egg-info/
--rw-r--r--   0 johanlu    (503) staff       (20)     3149 2023-02-28 07:15:55.000000 iommi-5.8.1/iommi.egg-info/PKG-INFO
--rw-r--r--   0 johanlu    (503) staff       (20)     3083 2023-02-28 07:15:55.000000 iommi-5.8.1/iommi.egg-info/SOURCES.txt
--rw-r--r--   0 johanlu    (503) staff       (20)        1 2023-02-28 07:15:55.000000 iommi-5.8.1/iommi.egg-info/dependency_links.txt
--rw-r--r--   0 johanlu    (503) staff       (20)        1 2023-01-25 15:01:04.000000 iommi-5.8.1/iommi.egg-info/not-zip-safe
--rw-r--r--   0 johanlu    (503) staff       (20)       22 2023-02-28 07:15:55.000000 iommi-5.8.1/iommi.egg-info/requires.txt
--rw-r--r--   0 johanlu    (503) staff       (20)        6 2023-02-28 07:15:55.000000 iommi-5.8.1/iommi.egg-info/top_level.txt
--rw-r--r--   0 johanlu    (503) staff       (20)      208 2023-01-25 13:54:49.000000 iommi-5.8.1/pyproject.toml
--rw-r--r--   0 johanlu    (503) staff       (20)       10 2023-01-25 13:54:49.000000 iommi-5.8.1/requirements.txt
--rw-r--r--   0 johanlu    (503) staff       (20)     1144 2023-02-28 07:15:55.407185 iommi-5.8.1/setup.cfg
--rwxr-xr-x   0 johanlu    (503) staff       (20)     2947 2023-01-25 13:54:49.000000 iommi-5.8.1/setup.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.029060 iommi-5.9.0/
+-rw-r--r--   0 boxed      (501) staff       (20)      940 2023-03-28 08:51:20.000000 iommi-5.9.0/AUTHORS.rst
+-rw-r--r--   0 boxed      (501) staff       (20)      212 2021-01-28 10:44:48.000000 iommi-5.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 boxed      (501) staff       (20)    36124 2023-03-28 08:50:59.000000 iommi-5.9.0/HISTORY.rst
+-rw-r--r--   0 boxed      (501) staff       (20)     1485 2021-01-28 10:44:48.000000 iommi-5.9.0/LICENSE
+-rw-r--r--   0 boxed      (501) staff       (20)      332 2022-01-21 14:21:52.000000 iommi-5.9.0/MANIFEST.in
+-rw-r--r--   0 boxed      (501) staff       (20)     3027 2023-03-28 08:52:34.029319 iommi-5.9.0/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     2781 2023-03-10 13:41:56.000000 iommi-5.9.0/README.rst
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.016283 iommi-5.9.0/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     8196 2023-03-09 20:55:15.000000 iommi-5.9.0/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)     3078 2023-03-28 08:51:34.000000 iommi-5.9.0/iommi/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6302 2023-03-17 11:57:14.000000 iommi-5.9.0/iommi/_db_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5965 2023-03-28 08:45:40.000000 iommi-5.9.0/iommi/_web_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)      490 2022-07-17 13:13:13.000000 iommi-5.9.0/iommi/_web_compat_flask.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5757 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/action.py
+-rw-r--r--   0 boxed      (501) staff       (20)    20986 2023-03-09 08:48:12.000000 iommi-5.9.0/iommi/admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1916 2023-03-17 11:56:17.000000 iommi-5.9.0/iommi/apps.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1950 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/asset.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5011 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/attrs.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2525 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4902 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/datetime_parsing.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10221 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/debug.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.018021 iommi-5.9.0/iommi/declarative/
+-rw-r--r--   0 boxed      (501) staff       (20)     5447 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/declarative/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      571 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/declarative/dispatch.py
+-rw-r--r--   0 boxed      (501) staff       (20)     7724 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/declarative/namespace.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1938 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/declarative/util.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1425 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/declarative/with_meta.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11917 2023-03-18 10:30:08.000000 iommi-5.9.0/iommi/docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)    16263 2023-02-27 14:56:27.000000 iommi-5.9.0/iommi/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3769 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/endpoint.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1477 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/error.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4924 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/evaluate.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.018720 iommi-5.9.0/iommi/experimental/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-5.9.0/iommi/experimental/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/experimental/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      133 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/experimental/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)    66017 2023-03-27 19:20:47.000000 iommi-5.9.0/iommi/form.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8160 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/fragment.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10054 2023-02-14 19:04:05.000000 iommi-5.9.0/iommi/from_model.py
+-rw-r--r--   0 boxed      (501) staff       (20)    19377 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/live_edit.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.018914 iommi-5.9.0/iommi/locale/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-08-10 12:35:42.000000 iommi-5.9.0/iommi/locale/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.019227 iommi-5.9.0/iommi/locale/de/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-5.9.0/iommi/locale/de/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.020058 iommi-5.9.0/iommi/locale/de/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     4463 2022-11-04 19:46:47.000000 iommi-5.9.0/iommi/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     6167 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.020271 iommi-5.9.0/iommi/locale/sv/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-5.9.0/iommi/locale/sv/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.020629 iommi-5.9.0/iommi/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     2239 2022-11-04 19:46:47.000000 iommi-5.9.0/iommi/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     5863 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.000431 iommi-5.9.0/iommi/locale/zh_Hans/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.021064 iommi-5.9.0/iommi/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     3995 2023-02-14 19:06:05.000000 iommi-5.9.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     5638 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 boxed      (501) staff       (20)    10064 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/member.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10419 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/menu.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3761 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/page.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8267 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/part.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6531 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/path.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6201 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/profiling.py
+-rw-r--r--   0 boxed      (501) staff       (20)    36300 2023-03-08 19:11:46.000000 iommi-5.9.0/iommi/query.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8657 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/refinable.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2717 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/shortcut.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2541 2023-03-22 09:15:30.000000 iommi-5.9.0/iommi/sort_after.py
+-rw-r--r--   0 boxed      (501) staff       (20)    16904 2023-03-17 14:18:56.000000 iommi-5.9.0/iommi/sql_trace.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3732 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/struct.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10253 2023-03-20 18:59:25.000000 iommi-5.9.0/iommi/style.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4566 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/style_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5989 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/style_bootstrap.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6001 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/style_bootstrap5.py
+-rw-r--r--   0 boxed      (501) staff       (20)      518 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/style_bootstrap_docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)      533 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/style_bootstrap_icons.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4490 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/style_bulma.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1856 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/style_django_admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)      551 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/style_font_awesome_4.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2551 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/style_foundation.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3644 2022-03-31 08:31:56.000000 iommi-5.9.0/iommi/style_semantic_ui.py
+-rw-r--r--   0 boxed      (501) staff       (20)      884 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/style_test_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1775 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/style_uikit.py
+-rw-r--r--   0 boxed      (501) staff       (20)      309 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/style_water.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1820 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/synthetic_traceback.py
+-rw-r--r--   0 boxed      (501) staff       (20)    81715 2023-03-08 19:11:39.000000 iommi-5.9.0/iommi/table.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.021289 iommi-5.9.0/iommi/templates/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-30 21:47:17.000000 iommi-5.9.0/iommi/templates/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.021977 iommi-5.9.0/iommi/templates/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-5.9.0/iommi/templates/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      443 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/base.html
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/templates/iommi/blank.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.024026 iommi-5.9.0/iommi/templates/iommi/form/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 19:05:37.000000 iommi-5.9.0/iommi/templates/iommi/form/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      873 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/form/actions.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.024172 iommi-5.9.0/iommi/templates/iommi/form/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)      255 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/templates/iommi/form/bulma/field.html
+-rw-r--r--   0 boxed      (501) staff       (20)      495 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/form/choice.html
+-rw-r--r--   0 boxed      (501) staff       (20)      709 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/form/choice_select2.html
+-rw-r--r--   0 boxed      (501) staff       (20)      353 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/templates/iommi/form/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)       78 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/templates/iommi/form/heading.html
+-rw-r--r--   0 boxed      (501) staff       (20)      187 2022-02-09 12:13:49.000000 iommi-5.9.0/iommi/templates/iommi/form/image_row.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1776 2023-03-28 08:43:44.000000 iommi-5.9.0/iommi/templates/iommi/form/init_select2.js
+-rw-r--r--   0 boxed      (501) staff       (20)      415 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/form/radio.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.024670 iommi-5.9.0/iommi/templates/iommi/form/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)      496 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/form/semantic_ui/radio.html
+-rw-r--r--   0 boxed      (501) staff       (20)      166 2022-03-31 08:29:44.000000 iommi-5.9.0/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.024907 iommi-5.9.0/iommi/templates/iommi/form/uikit/
+-rw-r--r--   0 boxed      (501) staff       (20)      379 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/templates/iommi/form/uikit/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.025898 iommi-5.9.0/iommi/templates/iommi/query/
+-rw-r--r--   0 boxed      (501) staff       (20)     2622 2022-01-19 10:19:49.000000 iommi-5.9.0/iommi/templates/iommi/query/advanced.html
+-rw-r--r--   0 boxed      (501) staff       (20)     5931 2023-03-28 08:45:40.000000 iommi-5.9.0/iommi/templates/iommi/query/ajax_enhance.js
+-rw-r--r--   0 boxed      (501) staff       (20)     1498 2021-04-15 06:01:07.000000 iommi-5.9.0/iommi/templates/iommi/query/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2808 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/query/form_toggle_script.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.028250 iommi-5.9.0/iommi/templates/iommi/table/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.028445 iommi-5.9.0/iommi/templates/iommi/table/bootstrap/
+-rw-r--r--   0 boxed      (501) staff       (20)     1526 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/bootstrap/paginator.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.028732 iommi-5.9.0/iommi/templates/iommi/table/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)     1554 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/bulma/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      188 2022-12-05 09:07:16.000000 iommi-5.9.0/iommi/templates/iommi/table/header.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2303 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/table/js_select_all.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1814 2023-02-14 18:44:36.000000 iommi-5.9.0/iommi/templates/iommi/table/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      102 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/row_group.html
+-rw-r--r--   0 boxed      (501) staff       (20)      196 2022-10-31 14:55:23.000000 iommi-5.9.0/iommi/templates/iommi/table/select_column_header.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.028881 iommi-5.9.0/iommi/templates/iommi/table/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)     1091 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/semantic_ui/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)       18 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/table.html
+-rw-r--r--   0 boxed      (501) staff       (20)      508 2021-04-15 06:01:07.000000 iommi-5.9.0/iommi/templates/iommi/table/table_container.html
+-rw-r--r--   0 boxed      (501) staff       (20)      209 2021-01-28 10:44:48.000000 iommi-5.9.0/iommi/templates/iommi/table/table_header_rows.html
+-rw-r--r--   0 boxed      (501) staff       (20)      453 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/templates/iommi/table/table_tag.html
+-rw-r--r--   0 boxed      (501) staff       (20)      207 2022-01-13 18:46:04.000000 iommi-5.9.0/iommi/thread_locals.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11883 2023-02-13 19:03:15.000000 iommi-5.9.0/iommi/traversable.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-03-28 08:52:34.017120 iommi-5.9.0/iommi.egg-info/
+-rw-r--r--   0 boxed      (501) staff       (20)     3027 2023-03-28 08:52:33.000000 iommi-5.9.0/iommi.egg-info/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     3298 2023-03-28 08:52:33.000000 iommi-5.9.0/iommi.egg-info/SOURCES.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2023-03-28 08:52:33.000000 iommi-5.9.0/iommi.egg-info/dependency_links.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2021-01-28 11:41:36.000000 iommi-5.9.0/iommi.egg-info/not-zip-safe
+-rw-r--r--   0 boxed      (501) staff       (20)       22 2023-03-28 08:52:33.000000 iommi-5.9.0/iommi.egg-info/requires.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        6 2023-03-28 08:52:33.000000 iommi-5.9.0/iommi.egg-info/top_level.txt
+-rw-r--r--   0 boxed      (501) staff       (20)      208 2023-02-13 19:03:15.000000 iommi-5.9.0/pyproject.toml
+-rw-r--r--   0 boxed      (501) staff       (20)       10 2023-02-13 19:03:15.000000 iommi-5.9.0/requirements.txt
+-rw-r--r--   0 boxed      (501) staff       (20)     1158 2023-03-28 08:52:34.029800 iommi-5.9.0/setup.cfg
+-rwxr-xr-x   0 boxed      (501) staff       (20)     2937 2023-03-10 13:33:59.000000 iommi-5.9.0/setup.py
```

### Comparing `iommi-5.8.1/AUTHORS.rst` & `iommi-5.9.0/AUTHORS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -20,7 +20,8 @@
 * Andreas Rasmusson <andreas.rasmusson@trioptima.com>
 * Martin Barksten <martin.barksten@trioptima.com>
 * Rasmus Spiegelberg <rasmus.spiegelberg@trioptima.com>
 * Benedikt Grundmann <benedikt.grundmann@gmail.com>
 * flying_sausages
 * Nigel Metheringham <nigel.metheringham@gmail.com>
 * Maximilian Albert <https://github.com/maxalbert>
+* Yury Bulka <setthemfree@privacyrequired.com>
```

### Comparing `iommi-5.8.1/HISTORY.rst` & `iommi-5.9.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 ---------
 
+5.9.0 (2023-03-28)
+~~~~~~~~~~~~~~~~~~
+
+* `iommi.forms.save_nested_form` added. This is useful for when you want to save multiple forms with one submit button.
+
+* Fixed admin defaults to have lower priority so you can properly override them.
+
+* Added dummy factory registration to not crash on `GenericRelation` and `GenericForeignKey`
+
+* Forms: check `model.validate_constraints()` on Django 4.1+ (Thanks Yury Bulka!)
+
+* Enable users to disable full form state sending on select2 ajax. To disable, set the `data-select2-full-state` attribute to `false` on the form.
+
+
 5.8.1 (2023-02-28)
 ~~~~~~~~~~~~~~~~~~
 
 * Fix bug where form submit include dispatch parameters e.g. bulk forms break after table tbody reload.
 
 
 5.8.0 (2023-02-14)
```

### Comparing `iommi-5.8.1/LICENSE` & `iommi-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/PKG-INFO` & `iommi-5.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 5.8.1
+Version: 5.9.0
 Summary: iommi is a high level framework built on django
-Home-page: https://github.com/TriOptima/iommi
+Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
-Author-email: anders.hovmoller@trioptima.com
+Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -17,27 +17,24 @@
 
 iommi
 =====
 
 .. image:: https://img.shields.io/discord/773470009795018763?logo=discord&logoColor=fff?label=Discord&color=7389d8
     :target: https://discord.gg/ZyYRYhf7Pd
 
-.. image:: https://github.com/TriOptima/iommi/workflows/tests/badge.svg
-    :target: https://github.com/TriOptima/iommi/actions?query=workflow%3Atests+branch%3Amaster
+.. image:: https://github.com/iommirocks/iommi/workflows/tests/badge.svg
+    :target: https://github.com/iommirocks/iommi/actions?query=workflow%3Atests+branch%3Amaster
 
-.. image:: https://codecov.io/gh/TriOptima/iommi/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/TriOptima/iommi
+.. image:: https://codecov.io/gh/iommirocks/iommi/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/iommirocks/iommi
 
 .. image:: https://readthedocs.org/projects/iommi/badge/?version=latest
     :target: https://docs.iommi.rocks
     :alt: Documentation Status
 
-.. image:: https://repl.it/badge/github/boxed/iommi-repl.it
-    :target: https://repl.it/github/boxed/iommi-repl.it
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 iommi is a toolkit to build web apps faster. It's built on Django but goes a lot further.
 
 It has:
 
@@ -72,15 +69,15 @@
     ]
 
 
 This creates a page with three separate tables, a header and some text:
 
 .. image:: docs/README-screenshot.png
 
-For more examples, see the `examples project <https://github.com/TriOptima/iommi/tree/master/examples/examples>`_.
+For more examples, see the `examples project <https://github.com/iommirocks/iommi/tree/master/examples/examples>`_.
 
 
 Getting started
 ---------------
 
 See `getting started <https://docs.iommi.rocks/en/latest/getting_started.html>`_.
```

### Comparing `iommi-5.8.1/README.rst` & `iommi-5.9.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 .. raw:: html
 
-    <p class="mobile-logo" align="center"><a href="#"><img class="logo" src="https://raw.githubusercontent.com/TriOptima/iommi/master/logo_with_outline.svg" alt="iommi" style="max-width: 200px" width=300></a></p>
+    <p class="mobile-logo" align="center"><a href="#"><img class="logo" src="https://raw.githubusercontent.com/iommirocks/iommi/master/logo_with_outline.svg" alt="iommi" style="max-width: 200px" width=300></a></p>
 
     <h3 class="pun">Your first pick for a django power chord</h3>
 
 .. image:: https://img.shields.io/discord/773470009795018763?logo=discord&logoColor=fff?label=Discord&color=7389d8
     :target: https://discord.gg/ZyYRYhf7Pd
 
-.. image:: https://github.com/TriOptima/iommi/workflows/tests/badge.svg
-    :target: https://github.com/TriOptima/iommi/actions?query=workflow%3Atests+branch%3Amaster
+.. image:: https://github.com/iommirocks/iommi/workflows/tests/badge.svg
+    :target: https://github.com/iommirocks/iommi/actions?query=workflow%3Atests+branch%3Amaster
 
-.. image:: https://codecov.io/gh/TriOptima/iommi/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/TriOptima/iommi
+.. image:: https://codecov.io/gh/iommirocks/iommi/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/iommirocks/iommi
 
 .. image:: https://readthedocs.org/projects/iommi/badge/?version=latest
     :target: https://docs.iommi.rocks
     :alt: Documentation Status
 
-.. image:: https://repl.it/badge/github/boxed/iommi-repl.it
-    :target: https://repl.it/github/boxed/iommi-repl.it
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 iommi is a toolkit to build web apps faster. It's built on Django but goes a lot further.
 
 It has:
 
@@ -58,15 +55,15 @@
     ]
 
 
 This creates a page with three separate tables, a header and some text:
 
 .. image:: docs/README-screenshot.png
 
-For more examples, see the `examples project <https://github.com/TriOptima/iommi/tree/master/examples/examples>`_.
+For more examples, see the `examples project <https://github.com/iommirocks/iommi/tree/master/examples/examples>`_.
 
 
 Getting started
 ---------------
 
 See `getting started <https://docs.iommi.rocks/en/latest/getting_started.html>`_.
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
 .. raw:: html
                                     [iommi]
 **** Your first pick for a django power chord ****
 .. image:: https://img.shields.io/discord/
 773470009795018763?logo=discord&logoColor=fff?label=Discord&color=7389d8 :
-target: https://discord.gg/ZyYRYhf7Pd .. image:: https://github.com/TriOptima/
-iommi/workflows/tests/badge.svg :target: https://github.com/TriOptima/iommi/
+target: https://discord.gg/ZyYRYhf7Pd .. image:: https://github.com/iommirocks/
+iommi/workflows/tests/badge.svg :target: https://github.com/iommirocks/iommi/
 actions?query=workflow%3Atests+branch%3Amaster .. image:: https://codecov.io/
-gh/TriOptima/iommi/branch/master/graph/badge.svg :target: https://codecov.io/
-gh/TriOptima/iommi .. image:: https://readthedocs.org/projects/iommi/badge/
+gh/iommirocks/iommi/branch/master/graph/badge.svg :target: https://codecov.io/
+gh/iommirocks/iommi .. image:: https://readthedocs.org/projects/iommi/badge/
 ?version=latest :target: https://docs.iommi.rocks :alt: Documentation Status ..
-image:: https://repl.it/badge/github/boxed/iommi-repl.it :target: https://
-repl.it/github/boxed/iommi-repl.it .. image:: https://img.shields.io/badge/
-code%20style-black-000000.svg :target: https://github.com/psf/black iommi is a
-toolkit to build web apps faster. It's built on Django but goes a lot further.
-It has: - `forms
+image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
+https://github.com/psf/black iommi is a toolkit to build web apps faster. It's
+built on Django but goes a lot further. It has: - `forms
 docs.iommi.rocks/en/latest/forms.html>`_: that feel familiar, but can handle
 growing complexity better than Django's forms - `tables
 docs.iommi.rocks/en/latest/tables.html>`_: that are powerful out of the box and
 scale up to arbitrary complexity - a system to `compose parts
 docs.iommi.rocks/en/latest/pages.html>`_:, like forms, menus, and tables, into
 bigger pages - tools that will speed up your development like live edit, jump
 to code, great feedback for missing select/prefetch related, a profiler, and
@@ -25,13 +23,13 @@
 demo.gif Example: .. code-block:: python class IndexPage(Page): title = html.h1
 ('Supernaut') welcome_text = 'This is a discography of the best acts in music!'
 artists = Table(auto__model=Artist, page_size=5) albums = Table
 ( auto__model=Album, page_size=5, ) tracks = Table(auto__model=Album,
 page_size=5) urlpatterns = [ path('', IndexPage().as_view()), ] This creates a
 page with three separate tables, a header and some text: .. image:: docs/
 README-screenshot.png For more examples, see the `examples project
-github.com/TriOptima/iommi/tree/master/examples/examples>`_. Getting started --
-------------- See `getting started
+github.com/iommirocks/iommi/tree/master/examples/examples>`_. Getting started -
+-------------- See `getting started
 docs.iommi.rocks/en/latest/getting_started.html>`_. Running tests ------------
 - You need to have tox installed, then: .. code-block:: make venv source venv/
 bin/activate make test make test-docs License ------- BSD Documentation -------
 ------ https://docs.iommi.rocks
```

### Comparing `iommi-5.8.1/iommi/__init__.py` & `iommi-5.9.0/iommi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '5.8.1'
+__version__ = '5.9.0'
 
 from functools import wraps
 
 import django
 
 from iommi._db_compat import (
     register_factory,
```

### Comparing `iommi-5.8.1/iommi/_db_compat.py` & `iommi-5.9.0/iommi/_db_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from django.db.models import ManyToManyField
 from iommi.shortcut import Shortcut
 
 from iommi.base import MISSING
 
 
 def setup_db_compat():
     setup_db_compat_django()
@@ -161,15 +160,15 @@
         r['display_name'] = capitalize(model_field.verbose_name)
 
     return r
 
 
 # TODO: move to form.py! remember to take the tests with them
 def field_defaults_factory(model_field):
-    from django.db.models import BooleanField
+    from django.db.models import BooleanField, ManyToManyField
 
     r = base_defaults_factory(model_field)
 
     if hasattr(model_field, 'null') and not isinstance(model_field, BooleanField):
         r['required'] = not model_field.null and not model_field.blank
 
     if isinstance(model_field, ManyToManyField):
```

### Comparing `iommi-5.8.1/iommi/_web_compat.py` & `iommi-5.9.0/iommi/_web_compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,180 +1,177 @@
 from django.template.utils import InvalidTemplateEngineError
 
-template_types = tuple()
-
-try:
-    from django.core.exceptions import (
-        ImproperlyConfigured,
-        ValidationError,
-    )
-    from django.core.validators import validate_email, URLValidator
-    from django.http import HttpResponse
-    from django.http import QueryDict  # noqa: F401
-    from django.template import RequestContext
-    from django.template.loader import render_to_string
-    from django.template.loader import get_template  # noqa: F401
-    from django.template.exceptions import TemplateDoesNotExist  # noqa: F401
-    from django.utils.html import format_html
-    from django.utils.text import slugify
-    from django.http import HttpResponseRedirect
-    from django.shortcuts import render
-    from django.utils.encoding import smart_str
-    from django.template.context_processors import csrf as csrf_
-    from django.utils.safestring import mark_safe
-    from django.http import HttpRequest
-    from django.http.response import HttpResponseBase
-    from django.template.backends.django import Template as DjangoLoadedTemplate
-
-    DjangoTemplate = None
-    JinjaTemplate = None
-
-    from django.conf import settings
-
-    template_types = tuple()
-
-    try:
-        if not settings.TEMPLATES or any('DjangoTemplates' in x['BACKEND'] for x in settings.TEMPLATES):
-            from django.template import Template as DjangoTemplate
-
-            template_types += (DjangoTemplate, DjangoLoadedTemplate)
-
-        if any('Jinja2' in x['BACKEND'] for x in settings.TEMPLATES):
-            import jinja2  # noqa: F401
-            from jinja2 import Template as JinjaTemplate
-
-            template_types += (JinjaTemplate,)
-    except ImproperlyConfigured:
-        pass
-
-    class Template:
-        def __init__(self, template_string):
-            self.s = template_string
-
-        def render(self, context):
-            if DjangoTemplate is not None:
-                return DjangoTemplate(self.s).render(context=context)
-            else:
-                assert JinjaTemplate is not None
-                return JinjaTemplate(self.s).render(**context.flatten())
-
-    template_types = template_types + (Template,)
-
-    def csrf(request):
-        return {} if request is None else csrf_(request)
-
-    try:
-        from django.template.loader import get_template_from_string
-    except ImportError:  # pragma: no cover
-        # Django 1.8+
-        # noinspection PyUnresolvedReferences
-        from django.template import engines
-
-        def get_template_from_string(template_code, origin=None, name=None):
-            del origin, name  # the origin and name parameters seems not to be implemented in django 1.8
-            try:
-                engine = engines['django']
-            except InvalidTemplateEngineError:
-                engine = engines.all()[0]
-
-            return engine.from_string(template_code)
-
-    def render_template(request, template, context):
-        """
-        @type request: django.http.HttpRequest
-        @type template: str|django.template.Template|django.template.backends.django.Template
-        @type context: dict
-        """
-        from iommi._web_compat import template_types
-
-        if template is None:
-            return ''
-        elif isinstance(template, str):
-            return mark_safe(render_to_string(template_name=template, context=context, request=request))
-        elif isinstance(template, DjangoLoadedTemplate):
-            return mark_safe(template.render(context=context, request=request))
-        elif isinstance(template, template_types):
-            return mark_safe(template.render(context=RequestContext(request, context)))
-        else:
-            return mark_safe(template.render(context, request))
-
-except ImportError:  # pragma: no cover This flask support is a work in progress/future plan
-    from jinja2 import Markup
-    from flask import render_template as render
-    from ._web_compat_flask import HttpRequest  # noqa: F401
-
-    csrf = None
-
-    class HttpResponse:
-        def __init__(self, content, content_type=None):
-            from flask import Response
-
-            self.r = Response(content, content_type=content_type)
-
-        @property
-        def content(self):
-            return self.r.get_rows()
-
-        @property
-        def _headers(self):
-            return {k.lower(): [v] for k, v in self.r.headers._list}
-
-    HttpResponseBase = HttpResponse
+from django.core.exceptions import (
+    ImproperlyConfigured,
+    ValidationError,
+)
+from django.core.validators import validate_email, URLValidator
+from django.http import HttpResponse
+from django.http import QueryDict  # noqa: F401
+from django.template import RequestContext
+from django.template.loader import render_to_string
+from django.template.loader import get_template  # noqa: F401
+from django.template.exceptions import TemplateDoesNotExist  # noqa: F401
+from django.utils.html import format_html
+from django.utils.text import slugify
+from django.http import HttpResponseRedirect
+from django.shortcuts import render
+from django.utils.encoding import smart_str
+from django.template.context_processors import csrf as csrf_
+from django.utils.safestring import mark_safe
+from django.http import HttpRequest
+from django.http.response import HttpResponseBase
+from django.template.backends.django import Template as DjangoLoadedTemplate
 
-    def format_html(format_string, *args, **kwargs):
-        return Markup(format_string).format(*args, **kwargs)
+DjangoTemplate = None
+JinjaTemplate = None
 
-    class ValidationError(Exception):
-        def __init__(self, messages):
-            if isinstance(messages, list):
-                self.messages = messages
-            else:
-                self.messages = [messages]
+from django.conf import settings
 
-    def HttpResponseRedirect(url, code=302):
-        from flask import redirect
-
-        return redirect(url, code=code)
+template_types = tuple()
 
-    def smart_str(s):
-        return str(s)
+try:
+    if not settings.TEMPLATES or any('DjangoTemplates' in x['BACKEND'] for x in settings.TEMPLATES):
+        from django.template import Template as DjangoTemplate
 
-    def render_template(request, template, context):
-        if template is None:
-            return ''
+        template_types += (DjangoTemplate, DjangoLoadedTemplate)
 
-        if isinstance(template, str):
-            return Markup(render(template, **(context or {})))
+    if any('Jinja2' in x['BACKEND'] for x in settings.TEMPLATES):
+        import jinja2  # noqa: F401
+        from jinja2 import Template as JinjaTemplate
+
+        template_types += (JinjaTemplate,)
+except ImproperlyConfigured:
+    pass
+
+class Template:
+    def __init__(self, template_string):
+        self.s = template_string
+
+    def render(self, context):
+        if DjangoTemplate is not None:
+            return DjangoTemplate(self.s).render(context=context)
         else:
-            return Markup(template.render(context=context, request=request))
-
-    def validate_email(s):
-        if '@' not in s:
-            raise ValidationError(messages=['Enter a valid email address.'])
-
-        return s
-
-    class URLValidator:
-        def __call__(self, string_value):
-            if '://' not in string_value:
-                raise ValidationError('Enter a valid URL.')
+            assert JinjaTemplate is not None
+            return JinjaTemplate(self.s).render(**context.flatten())
 
-    def get_template_from_string(s, origin=None, name=None):
-        return Template(s)
+template_types = template_types + (Template,)
 
-    def render_to_string(template_name, context, request=None):
-        return format_html(render(template_name, request=request, **context))
+def csrf(request):
+    return {} if request is None else csrf_(request)
 
-    class Template:
-        def __init__(self, template_string, **kwargs):
-            from jinja2 import Template
-
-            self.template = Template(template_string, **kwargs)
-
-        def render(self, context, request=None):
-            return self.template.render(**context)
-
-    def slugify(s):
-        return s.lower().replace(' ', '-')
-
-    def mark_safe(s):
-        return Markup(s)
+try:
+    from django.template.loader import get_template_from_string
+except ImportError:  # pragma: no cover
+    # Django 1.8+
+    # noinspection PyUnresolvedReferences
+    from django.template import engines
+
+    def get_template_from_string(template_code, origin=None, name=None):
+        del origin, name  # the origin and name parameters seems not to be implemented in django 1.8
+        try:
+            engine = engines['django']
+        except InvalidTemplateEngineError:
+            engine = engines.all()[0]
+
+        return engine.from_string(template_code)
+
+def render_template(request, template, context):
+    """
+    @type request: django.http.HttpRequest
+    @type template: str|django.template.Template|django.template.backends.django.Template
+    @type context: dict
+    """
+    from iommi._web_compat import template_types
+
+    if template is None:
+        return ''
+    elif isinstance(template, str):
+        return mark_safe(render_to_string(template_name=template, context=context, request=request))
+    elif isinstance(template, DjangoLoadedTemplate):
+        return mark_safe(template.render(context=context, request=request))
+    elif isinstance(template, template_types):
+        return mark_safe(template.render(context=RequestContext(request, context)))
+    else:
+        return mark_safe(template.render(context, request))
+
+# except ImportError:  # pragma: no cover This flask support is a work in progress/future plan
+#     from jinja2 import Markup
+#     from flask import render_template as render
+#     from ._web_compat_flask import HttpRequest  # noqa: F401
+#
+#     csrf = None
+#
+#     class HttpResponse:
+#         def __init__(self, content, content_type=None):
+#             from flask import Response
+#
+#             self.r = Response(content, content_type=content_type)
+#
+#         @property
+#         def content(self):
+#             return self.r.get_rows()
+#
+#         @property
+#         def _headers(self):
+#             return {k.lower(): [v] for k, v in self.r.headers._list}
+#
+#     HttpResponseBase = HttpResponse
+#
+#     def format_html(format_string, *args, **kwargs):
+#         return Markup(format_string).format(*args, **kwargs)
+#
+#     class ValidationError(Exception):
+#         def __init__(self, messages):
+#             if isinstance(messages, list):
+#                 self.messages = messages
+#             else:
+#                 self.messages = [messages]
+#
+#     def HttpResponseRedirect(url, code=302):
+#         from flask import redirect
+#
+#         return redirect(url, code=code)
+#
+#     def smart_str(s):
+#         return str(s)
+#
+#     def render_template(request, template, context):
+#         if template is None:
+#             return ''
+#
+#         if isinstance(template, str):
+#             return Markup(render(template, **(context or {})))
+#         else:
+#             return Markup(template.render(context=context, request=request))
+#
+#     def validate_email(s):
+#         if '@' not in s:
+#             raise ValidationError(messages=['Enter a valid email address.'])
+#
+#         return s
+#
+#     class URLValidator:
+#         def __call__(self, string_value):
+#             if '://' not in string_value:
+#                 raise ValidationError('Enter a valid URL.')
+#
+#     def get_template_from_string(s, origin=None, name=None):
+#         return Template(s)
+#
+#     def render_to_string(template_name, context, request=None):
+#         return format_html(render(template_name, request=request, **context))
+#
+#     class Template:
+#         def __init__(self, template_string, **kwargs):
+#             from jinja2 import Template
+#
+#             self.template = Template(template_string, **kwargs)
+#
+#         def render(self, context, request=None):
+#             return self.template.render(**context)
+#
+#     def slugify(s):
+#         return s.lower().replace(' ', '-')
+#
+#     def mark_safe(s):
+#         return Markup(s)
```

### Comparing `iommi-5.8.1/iommi/action.py` & `iommi-5.9.0/iommi/action.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/admin.py` & `iommi-5.9.0/iommi/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,41 +119,14 @@
 class Admin(Page):
     class Meta:
         iommi_style = 'bootstrap'
         table_class = Table
         form_class = Form
         apps = EMPTY
         parts = EMPTY
-        apps__auth_user__include = True
-        apps__auth_group__include = True
-        parts__messages = Messages()
-        parts__list_auth_user = dict(
-            auto__include=['username', 'email', 'first_name', 'last_name', 'is_staff', 'is_active', 'is_superuser'],
-            columns=dict(
-                username__filter=dict(
-                    include=True,
-                    freetext=True,
-                ),
-                email__filter=dict(
-                    include=True,
-                    freetext=True,
-                ),
-                first_name__filter=dict(
-                    include=True,
-                    freetext=True,
-                ),
-                last_name__filter=dict(
-                    include=True,
-                    freetext=True,
-                ),
-                is_staff__filter__include=True,
-                is_active__filter__include=True,
-                is_superuser__filter__include=True,
-            ),
-        )
 
     model: Type[Model] = Refinable()
     instance: Model = Refinable()
     app_name: str = Refinable()
     model_name: str = Refinable()
     operation: str = Refinable()
     table_class: Type[Table] = Refinable()
@@ -171,14 +144,43 @@
                 url=lambda **_: reverse(Auth.change_password), display_name=gettext('Change password')
             ),
             logout=MenuItem(url=lambda **_: reverse(Auth.logout), display_name=gettext('Logout')),
         ),
     )
 
     @read_config
+    @with_defaults(
+        apps__auth_user__include = True,
+        apps__auth_group__include = True,
+        parts__messages = Messages(),
+        parts__list_auth_user = dict(
+            auto__include=['username', 'email', 'first_name', 'last_name', 'is_staff', 'is_active', 'is_superuser'],
+            columns=dict(
+                username__filter=dict(
+                    include=True,
+                    freetext=True,
+                ),
+                email__filter=dict(
+                    include=True,
+                    freetext=True,
+                ),
+                first_name__filter=dict(
+                    include=True,
+                    freetext=True,
+                ),
+                last_name__filter=dict(
+                    include=True,
+                    freetext=True,
+                ),
+                is_staff__filter__include=True,
+                is_active__filter__include=True,
+                is_superuser__filter__include=True,
+            ),
+        ),
+    )
     def __init__(self, parts, apps, **kwargs):
         # Validate apps params
         for k in apps.keys():
             assert (
                 k in joined_app_name_and_model
             ), f'{k} is not a valid app/model key.\n\n' f'Valid keys:\n    ' + '\n    '.join(
                 sorted(joined_app_name_and_model)
```

### Comparing `iommi-5.8.1/iommi/apps.py` & `iommi-5.9.0/iommi/apps.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,7 +39,15 @@
         register_style('bootstrap5', bootstrap5)
         register_style('semantic_ui', semantic_ui)
         register_style('water', water)
         register_style('foundation', foundation)
         register_style('django_admin', django_admin)
         register_style('uikit', uikit)
         register_style('bootstrap_docs', bootstrap_docs)
+
+        from django.contrib.contenttypes.fields import (
+            GenericForeignKey,
+            GenericRelation,
+        )
+        from iommi import register_factory
+        register_factory(GenericRelation, factory=None)
+        register_factory(GenericForeignKey, factory=None)
```

### Comparing `iommi-5.8.1/iommi/asset.py` & `iommi-5.9.0/iommi/asset.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/attrs.py` & `iommi-5.9.0/iommi/attrs.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/base.py` & `iommi-5.9.0/iommi/base.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/datetime_parsing.py` & `iommi-5.9.0/iommi/datetime_parsing.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/debug.py` & `iommi-5.9.0/iommi/debug.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/declarative/__init__.py` & `iommi-5.9.0/iommi/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/declarative/dispatch.py` & `iommi-5.9.0/iommi/declarative/dispatch.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/declarative/namespace.py` & `iommi-5.9.0/iommi/declarative/namespace.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/declarative/util.py` & `iommi-5.9.0/iommi/declarative/util.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/declarative/with_meta.py` & `iommi-5.9.0/iommi/declarative/with_meta.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/docs.py` & `iommi-5.9.0/iommi/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 def generate_api_docs_tests(directory, classes=None):  # pragma: no cover - this is tested by rtd anyway
     """
     Generate test files for declarative APIs
 
     :param directory: directory to write the .py files into
     :param classes: list of classes to generate tests for
     """
-    print(f'generate_api_docs_tests("{directory}")')
     if classes is None:
         classes = get_default_classes()
 
     doc_by_filename = _generate_tests_from_class_docs(classes=classes)  # pragma: no mutate
     for source_filename, filename, doc_generator in doc_by_filename:  # pragma: no mutate
         try:
             if stat(source_filename).st_mtime <= stat(directory / filename).st_mtime:
```

### Comparing `iommi-5.8.1/iommi/edit_table.py` & `iommi-5.9.0/iommi/edit_table.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/endpoint.py` & `iommi-5.9.0/iommi/endpoint.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/error.py` & `iommi-5.9.0/iommi/error.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/evaluate.py` & `iommi-5.9.0/iommi/evaluate.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/form.py` & `iommi-5.9.0/iommi/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     Set,
     Tuple,
     Type,
     Union,
 )
 
 from django.core.exceptions import ObjectDoesNotExist
-from django.db import IntegrityError
+from django.db import (
+    IntegrityError,
+    models,
+)
 from django.db.models import (
     Case,
     IntegerField,
     Model,
     Q,
     QuerySet,
     When,
@@ -181,14 +184,35 @@
         prefix, _, _ = attribute.rpartition('__')
         parts = prefix.split('__')
         for i in range(len(parts)):
             result.add(tuple(parts[: i + 1]))
     return ['__'.join(p) for p in sorted(sorted(result), key=len)]
 
 
+def save_nested_forms(form, request, **_):
+    did_fail = False
+    for nested_form in form.nested_forms.values():
+        for action in nested_form.actions.values():
+            if action.post_handler is None:
+                continue
+            if action.post_handler and action.invoke_callback(action.post_handler) is None:
+                did_fail = True
+
+    if not did_fail:
+        if 'post_save' in form.extra:
+            form.invoke_callback(form.extra.post_save)
+
+        request.method = 'GET'
+
+        redirect_to = form.extra.get('redirect_to', lambda **_: request.POST.get('next', '.'))
+        target = form.invoke_callback(redirect_to)
+        assert isinstance(target, str), 'redirect_to must return a str'
+        return HttpResponseRedirect(target)
+
+
 def create_or_edit_object__post_handler(*, form, is_create, **_):
     if not form.is_valid():
         return
 
     if is_create:
         assert form.instance is None
         form.instance = form.invoke_callback(form.extra.new_instance)
@@ -200,27 +224,31 @@
         for field in values(form.fields):
             # two phase save for creation in django, have to save main object before related stuff
             if not field.extra.get('django_related_field', False):
                 form.apply_field(field=field, instance=form.instance)
 
         with validation_errors_reported_on(form):
             form.instance.validate_unique()
+            if hasattr(form.instance, 'validate_constraints'):
+                form.instance.validate_constraints()
         if not form.is_valid():
             return
 
         # two phase save for creation in django...
         form.invoke_callback(form.extra.pre_save_all_but_related_fields)
         form.instance.save()
         form.invoke_callback(form.extra.on_save_all_but_related_fields)
 
     form.apply(form.instance)
 
     if not is_create:
         with validation_errors_reported_on(form):
             form.instance.validate_unique()
+            if hasattr(form.instance, 'validate_constraints'):
+                form.instance.validate_constraints()
         if not form.is_valid():
             return
 
     attributes = filter(None, [f.attr for f in form.fields.values()])
 
     form.invoke_callback(form.extra.pre_save)
     for prefix in find_unique_prefixes(attributes):
@@ -509,16 +537,16 @@
     input: Fragment = Refinable()
     label: Fragment = Refinable()
     non_editable_input: Fragment = Refinable()
     help: Fragment = Refinable()
 
     is_list: bool = EvaluatedRefinable()
     is_boolean: bool = EvaluatedRefinable()
-    model: Type[Model] = SpecialEvaluatedRefinable()
-    model_field = Refinable()
+    model: Optional[Type[Model]] = SpecialEvaluatedRefinable()
+    model_field : Optional[models.Field] = Refinable()
     model_field_name = Refinable()
 
     editable: bool = EvaluatedRefinable()
     strip_input: bool = EvaluatedRefinable()
 
     choices: Callable[..., List[Any]] = SpecialEvaluatedRefinable()
     choice_id_formatter: Callable[..., str] = Refinable()
```

### Comparing `iommi-5.8.1/iommi/fragment.py` & `iommi-5.9.0/iommi/fragment.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/from_model.py` & `iommi-5.9.0/iommi/from_model.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/live_edit.py` & `iommi-5.9.0/iommi/live_edit.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/de/LC_MESSAGES/django.mo` & `iommi-5.9.0/iommi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/de/LC_MESSAGES/django.po` & `iommi-5.9.0/iommi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/sv/LC_MESSAGES/django.mo` & `iommi-5.9.0/iommi/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/sv/LC_MESSAGES/django.po` & `iommi-5.9.0/iommi/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/zh_Hans/LC_MESSAGES/django.mo` & `iommi-5.9.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/locale/zh_Hans/LC_MESSAGES/django.po` & `iommi-5.9.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/member.py` & `iommi-5.9.0/iommi/member.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/menu.py` & `iommi-5.9.0/iommi/menu.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/page.py` & `iommi-5.9.0/iommi/page.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/part.py` & `iommi-5.9.0/iommi/part.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/path.py` & `iommi-5.9.0/iommi/path.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/profiling.py` & `iommi-5.9.0/iommi/profiling.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/query.py` & `iommi-5.9.0/iommi/query.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/refinable.py` & `iommi-5.9.0/iommi/refinable.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/shortcut.py` & `iommi-5.9.0/iommi/shortcut.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/sort_after.py` & `iommi-5.9.0/iommi/sort_after.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/sql_trace.py` & `iommi-5.9.0/iommi/sql_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
 from iommi.attrs import render_style
 from iommi.thread_locals import (
     get_current_request,
     set_current_request,
 )
 
+def no_coloring(text, color=None, on_color=None, attrs=None):
+    return text
+
 try:
     from termcolor import colored
 except ImportError:
-
-    def colored(text, color=None, on_color=None, attrs=None):
-        return text
+    colored = no_coloring
 
 
 from django.conf import settings
 from django.db.backends import utils as django_db_utils
 
 
 log = logging.getLogger('db')
```

### Comparing `iommi-5.8.1/iommi/struct.py` & `iommi-5.9.0/iommi/struct.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style.py` & `iommi-5.9.0/iommi/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,16 @@
             unregister_style(name)
 
     return _unregister()
 
 
 def unregister_style(name):
     assert name in _styles
+    style = _styles[name]
+    style.name = None
     del _styles[name]
 
 
 def get_global_style(name):
     if isinstance(name, Style):
         return name
     try:
```

### Comparing `iommi-5.8.1/iommi/style_base.py` & `iommi-5.9.0/iommi/style_base.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_bootstrap.py` & `iommi-5.9.0/iommi/style_bootstrap.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_bootstrap5.py` & `iommi-5.9.0/iommi/style_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_bootstrap_docs.py` & `iommi-5.9.0/iommi/style_bootstrap_docs.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_bootstrap_icons.py` & `iommi-5.9.0/iommi/style_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_bulma.py` & `iommi-5.9.0/iommi/style_bulma.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_django_admin.py` & `iommi-5.9.0/iommi/style_django_admin.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_font_awesome_4.py` & `iommi-5.9.0/iommi/style_font_awesome_4.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_foundation.py` & `iommi-5.9.0/iommi/style_foundation.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_semantic_ui.py` & `iommi-5.9.0/iommi/style_semantic_ui.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_test_base.py` & `iommi-5.9.0/iommi/style_test_base.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/style_uikit.py` & `iommi-5.9.0/iommi/style_uikit.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/synthetic_traceback.py` & `iommi-5.9.0/iommi/synthetic_traceback.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/table.py` & `iommi-5.9.0/iommi/table.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/form/actions.html` & `iommi-5.9.0/iommi/templates/iommi/form/actions.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/form/choice_select2.html` & `iommi-5.9.0/iommi/templates/iommi/form/choice_select2.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/form/init_select2.js` & `iommi-5.9.0/iommi/templates/iommi/form/init_select2.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,25 @@
         placeholder: f.attr('data-placeholder'),
         allowClear: true,
         multiple: multiple
     };
     if (endpoint_path) {
         options.ajax = {
             url: function() {
-                return '?' + this.closest('form').serialize();
+                let form = this.closest('form');
+
+                let full_state = form.attr('data-select2-full-state');
+                if (full_state === undefined) {
+                    full_state = "true";
+                }
+                if (full_state === 'true') {
+                    return '?' + form.serialize();
+                } else {
+                    return "";
+                }
             },
             dataType: "json",
             data: function(params) {
                 let result = {
                     page: params.page || 1
                 }
                 result[endpoint_path] = params.term || '';
```

### Comparing `iommi-5.8.1/iommi/templates/iommi/query/advanced.html` & `iommi-5.9.0/iommi/templates/iommi/query/advanced.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/query/ajax_enhance.js` & `iommi-5.9.0/iommi/templates/iommi/query/ajax_enhance.js`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/query/form.html` & `iommi-5.9.0/iommi/templates/iommi/query/form.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/query/form_toggle_script.html` & `iommi-5.9.0/iommi/templates/iommi/query/form_toggle_script.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/table/bootstrap/paginator.html` & `iommi-5.9.0/iommi/templates/iommi/table/bootstrap/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/table/bulma/paginator.html` & `iommi-5.9.0/iommi/templates/iommi/table/bulma/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/table/js_select_all.html` & `iommi-5.9.0/iommi/templates/iommi/table/js_select_all.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/table/paginator.html` & `iommi-5.9.0/iommi/templates/iommi/table/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/templates/iommi/table/semantic_ui/paginator.html` & `iommi-5.9.0/iommi/templates/iommi/table/semantic_ui/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi/traversable.py` & `iommi-5.9.0/iommi/traversable.py`

 * *Files identical despite different names*

### Comparing `iommi-5.8.1/iommi.egg-info/PKG-INFO` & `iommi-5.9.0/iommi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 5.8.1
+Version: 5.9.0
 Summary: iommi is a high level framework built on django
-Home-page: https://github.com/TriOptima/iommi
+Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
-Author-email: anders.hovmoller@trioptima.com
+Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -17,27 +17,24 @@
 
 iommi
 =====
 
 .. image:: https://img.shields.io/discord/773470009795018763?logo=discord&logoColor=fff?label=Discord&color=7389d8
     :target: https://discord.gg/ZyYRYhf7Pd
 
-.. image:: https://github.com/TriOptima/iommi/workflows/tests/badge.svg
-    :target: https://github.com/TriOptima/iommi/actions?query=workflow%3Atests+branch%3Amaster
+.. image:: https://github.com/iommirocks/iommi/workflows/tests/badge.svg
+    :target: https://github.com/iommirocks/iommi/actions?query=workflow%3Atests+branch%3Amaster
 
-.. image:: https://codecov.io/gh/TriOptima/iommi/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/TriOptima/iommi
+.. image:: https://codecov.io/gh/iommirocks/iommi/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/iommirocks/iommi
 
 .. image:: https://readthedocs.org/projects/iommi/badge/?version=latest
     :target: https://docs.iommi.rocks
     :alt: Documentation Status
 
-.. image:: https://repl.it/badge/github/boxed/iommi-repl.it
-    :target: https://repl.it/github/boxed/iommi-repl.it
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 iommi is a toolkit to build web apps faster. It's built on Django but goes a lot further.
 
 It has:
 
@@ -72,15 +69,15 @@
     ]
 
 
 This creates a page with three separate tables, a header and some text:
 
 .. image:: docs/README-screenshot.png
 
-For more examples, see the `examples project <https://github.com/TriOptima/iommi/tree/master/examples/examples>`_.
+For more examples, see the `examples project <https://github.com/iommirocks/iommi/tree/master/examples/examples>`_.
 
 
 Getting started
 ---------------
 
 See `getting started <https://docs.iommi.rocks/en/latest/getting_started.html>`_.
```

### Comparing `iommi-5.8.1/iommi.egg-info/SOURCES.txt` & `iommi-5.9.0/iommi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
+iommi/.DS_Store
 iommi/__init__.py
 iommi/_db_compat.py
 iommi/_web_compat.py
 iommi/_web_compat_flask.py
 iommi/action.py
 iommi/admin.py
 iommi/apps.py
@@ -66,24 +67,31 @@
 iommi.egg-info/requires.txt
 iommi.egg-info/top_level.txt
 iommi/declarative/__init__.py
 iommi/declarative/dispatch.py
 iommi/declarative/namespace.py
 iommi/declarative/util.py
 iommi/declarative/with_meta.py
+iommi/experimental/.DS_Store
 iommi/experimental/__init__.py
 iommi/experimental/edit_table.py
+iommi/locale/.DS_Store
+iommi/locale/de/.DS_Store
 iommi/locale/de/LC_MESSAGES/django.mo
 iommi/locale/de/LC_MESSAGES/django.po
+iommi/locale/sv/.DS_Store
 iommi/locale/sv/LC_MESSAGES/django.mo
 iommi/locale/sv/LC_MESSAGES/django.po
 iommi/locale/zh_Hans/LC_MESSAGES/django.mo
 iommi/locale/zh_Hans/LC_MESSAGES/django.po
+iommi/templates/.DS_Store
+iommi/templates/iommi/.DS_Store
 iommi/templates/iommi/base.html
 iommi/templates/iommi/blank.html
+iommi/templates/iommi/form/.DS_Store
 iommi/templates/iommi/form/actions.html
 iommi/templates/iommi/form/choice.html
 iommi/templates/iommi/form/choice_select2.html
 iommi/templates/iommi/form/form.html
 iommi/templates/iommi/form/heading.html
 iommi/templates/iommi/form/image_row.html
 iommi/templates/iommi/form/init_select2.js
```

### Comparing `iommi-5.8.1/setup.cfg` & `iommi-5.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 universal = 1
 
 [hammett]
 DJANGO_SETTINGS_MODULE = tests.settings
 plugins = 
 	pytest_django
 	pytest_snapshot
+	time_machine
 
 [tool:pytest]
 testpaths = 
 	tests
 	iommi
 	docs
 addopts = --junitxml=testreport.xml --strict -r fEsxXw --no-migrations
```

### Comparing `iommi-5.8.1/setup.py` & `iommi-5.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 #     everything using imp.find_module
 setup(
     name='iommi',
     version=read_version(),
     description='iommi is a high level framework built on django',
     long_description=readme,
     author='Anders Hovmöller',
-    author_email='anders.hovmoller@trioptima.com',
-    url='https://github.com/TriOptima/iommi',
+    author_email='boxed@killingar.net',
+    url='https://github.com/iommirocks/iommi',
     packages=['iommi'],
     include_package_data=True,
     install_requires=['Django >= 3.0'] + read_reqs('requirements.txt'),
     license="BSD",
     zip_safe=False,
     keywords='iommi',
     classifiers=[
```

