# Comparing `tmp/mia-accounting-1.0.1.tar.gz` & `tmp/mia-accounting-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.0.1.tar", last modified: Thu Apr  6 00:44:10 2023, max compression
+gzip compressed data, was "mia-accounting-1.1.0.tar", last modified: Sat Apr  8 16:49:29 2023, max compression
```

## Comparing `mia-accounting-1.0.1.tar` & `mia-accounting-1.1.0.tar`

### file list

```diff
@@ -1,287 +1,303 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.537094 mia-accounting-1.0.1/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.0.1/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.0.1/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     7032 2023-04-06 00:44:10.537094 mia-accounting-1.0.1/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     6233 2023-04-06 00:38:39.000000 mia-accounting-1.0.1/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.505095 mia-accounting-1.0.1/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.0.1/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.0.1/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.505095 mia-accounting-1.0.1/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.505095 mia-accounting-1.0.1/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.0.1/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.505095 mia-accounting-1.0.1/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.0.1/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1384 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1626 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1587 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1155 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2227 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-06 00:43:06.000000 mia-accounting-1.0.1/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.0.1/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.0.1/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.0.1/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3977 2023-04-06 00:31:13.000000 mia-accounting-1.0.1/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.0.1/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-06 00:43:06.000000 mia-accounting-1.0.1/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-06 00:44:10.537094 mia-accounting-1.0.1/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.501095 mia-accounting-1.0.1/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     2911 2023-04-05 00:06:20.000000 mia-accounting-1.0.1/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1254 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     5570 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7424 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1296 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2018 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1817 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/base_account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1365 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3286 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6620 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.0.1/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.0.1/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.509095 mia-accounting-1.0.1/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3609 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11070 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19663 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3771 2023-04-05 01:25:10.000000 mia-accounting-1.0.1/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9480 2023-04-04 23:58:41.000000 mia-accounting-1.0.1/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    30277 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1256 2023-04-05 00:04:13.000000 mia-accounting-1.0.1/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2577 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.513095 mia-accounting-1.0.1/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-05 04:27:28.000000 mia-accounting-1.0.1/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-05 04:59:37.000000 mia-accounting-1.0.1/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8009 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8362 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-05 04:56:12.000000 mia-accounting-1.0.1/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.517094 mia-accounting-1.0.1/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6093 2023-04-05 00:14:19.000000 mia-accounting-1.0.1/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1227 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4128 2023-04-04 23:58:21.000000 mia-accounting-1.0.1/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)     9635 2023-04-04 23:55:45.000000 mia-accounting-1.0.1/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.497095 mia-accounting-1.0.1/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.517094 mia-accounting-1.0.1/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    12126 2023-04-05 01:06:22.000000 mia-accounting-1.0.1/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.517094 mia-accounting-1.0.1/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9072 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.0.1/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.497095 mia-accounting-1.0.1/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.517094 mia-accounting-1.0.1/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.521094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3123 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2780 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.525094 mia-accounting-1.0.1/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.0.1/src/accounting/templates/accounting/report/trial-balance.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    43406 2023-04-05 18:34:29.000000 mia-accounting-1.0.1/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.0.1/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.501095 mia-accounting-1.0.1/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    13934 2023-04-05 18:34:36.000000 mia-accounting-1.0.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    47372 2023-04-05 18:34:36.000000 mia-accounting-1.0.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.501095 mia-accounting-1.0.1/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    13934 2023-04-05 18:34:36.000000 mia-accounting-1.0.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    47372 2023-04-05 18:55:17.000000 mia-accounting-1.0.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     7383 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.0.1/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.0.1/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.529094 mia-accounting-1.0.1/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     7032 2023-04-06 00:44:10.000000 mia-accounting-1.0.1/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    10691 2023-04-06 00:44:10.000000 mia-accounting-1.0.1/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-06 00:44:10.000000 mia-accounting-1.0.1/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-06 00:44:10.000000 mia-accounting-1.0.1/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-06 00:44:10.000000 mia-accounting-1.0.1/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.0.1/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    35927 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     5034 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)    27074 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    16847 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   106499 2023-04-04 23:59:18.000000 mia-accounting-1.0.1/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    33566 2023-04-04 09:21:36.000000 mia-accounting-1.0.1/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    16853 2023-04-04 09:21:32.000000 mia-accounting-1.0.1/tests/test_option.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4143 2023-04-04 23:16:14.000000 mia-accounting-1.0.1/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.0.1/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.0.1/tests/test_site/locale.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.0.1/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.0.1/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.0.1/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.0.1/tests/test_site/templates/login.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.0.1/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.0.1/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.501095 mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.501095 mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-06 00:44:10.533094 mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     3792 2023-04-04 09:21:33.000000 mia-accounting-1.0.1/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/tests/testlib_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    13639 2023-04-04 09:21:31.000000 mia-accounting-1.0.1/tests/testlib_offset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.1.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.1.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     6225 2023-04-06 02:00:23.000000 mia-accounting-1.1.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.1.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.1.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.1.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.482895 mia-accounting-1.1.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.1.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1186 2023-04-08 16:40:31.000000 mia-accounting-1.1.0/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-08 16:40:32.000000 mia-accounting-1.1.0/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-08 16:46:46.000000 mia-accounting-1.1.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.1.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.1.0/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.1.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3969 2023-04-06 02:00:11.000000 mia-accounting-1.1.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.1.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-08 16:46:46.000000 mia-accounting-1.1.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     2981 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1254 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5589 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7424 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1296 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2018 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1813 2023-04-06 08:06:37.000000 mia-accounting-1.1.0/src/accounting/base_account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1365 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3286 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6616 2023-04-06 08:06:37.000000 mia-accounting-1.1.0/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.1.0/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.1.0/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.486895 mia-accounting-1.1.0/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.1.0/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9480 2023-04-04 23:58:41.000000 mia-accounting-1.1.0/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.1.0/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.490895 mia-accounting-1.1.0/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.1.0/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8362 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.1.0/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.1.0/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4569 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10748 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.494895 mia-accounting-1.1.0/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.1.0/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.498895 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.502894 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 16:22:08.000000 mia-accounting-1.1.0/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.1.0/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15685 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52091 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15685 2023-04-08 16:37:13.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52091 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.506894 mia-accounting-1.1.0/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.510894 mia-accounting-1.1.0/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.1.0/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.1.0/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.1.0/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.1.0/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.1.0/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.510894 mia-accounting-1.1.0/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11343 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-08 16:49:29.000000 mia-accounting-1.1.0/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.1.0/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    35927 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5034 2023-04-04 09:21:36.000000 mia-accounting-1.1.0/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)    27074 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16847 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   106499 2023-04-04 23:59:18.000000 mia-accounting-1.1.0/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    33566 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    34728 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/test_offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16853 2023-04-04 09:21:32.000000 mia-accounting-1.1.0/tests/test_option.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4143 2023-04-04 23:16:14.000000 mia-accounting-1.1.0/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.1.0/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.1.0/tests/test_site/locale.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.1.0/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.1.0/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.1.0/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.1.0/tests/test_site/templates/login.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.514894 mia-accounting-1.1.0/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.1.0/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.1.0/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.578893 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.478895 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-08 16:49:29.602893 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3792 2023-04-04 09:21:33.000000 mia-accounting-1.1.0/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-04 09:21:31.000000 mia-accounting-1.1.0/tests/testlib_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13639 2023-04-08 16:39:46.000000 mia-accounting-1.1.0/tests/testlib_offset.py
```

### Comparing `mia-accounting-1.0.1/LICENSE` & `mia-accounting-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/MANIFEST.in` & `mia-accounting-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/PKG-INFO` & `mia-accounting-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
@@ -33,30 +33,40 @@
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
-You may try the `live demonstration`_.
-
 
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
 You may also download the from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
+Test Site and Live Demonstration
+================================
+
+You may find a working example in the `test site`_ in the
+`source distribution`_.  It is the simplest website that works with
+*Mia! Accounting*.  It is used in the automatic tests.  It is the same
+code run for `live demonstration`_.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.
 
 The following front-end JavaScript libraries must be loaded.  You may
@@ -173,26 +183,14 @@
         </div>
       </div>
     </nav>
 
 Check your Flask application and see how it works.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application, you may start with the
-test site.
-
-
 Documentation
 =============
 
 Refer to the `documentation on Read the Docs`_.
 
 
 Copyright
@@ -219,23 +217,23 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
+.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
 .. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
-.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
-.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.0.1/README.rst` & `mia-accounting-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,40 @@
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
-You may try the `live demonstration`_.
-
 
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
 You may also download the from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
+Test Site and Live Demonstration
+================================
+
+You may find a working example in the `test site`_ in the
+`source distribution`_.  It is the simplest website that works with
+*Mia! Accounting*.  It is used in the automatic tests.  It is the same
+code run for `live demonstration`_.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.
 
 The following front-end JavaScript libraries must be loaded.  You may
@@ -153,26 +163,14 @@
         </div>
       </div>
     </nav>
 
 Check your Flask application and see how it works.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application, you may start with the
-test site.
-
-
 Documentation
 =============
 
 Refer to the `documentation on Read the Docs`_.
 
 
 Copyright
@@ -199,23 +197,23 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
+.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
 .. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
-.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
-.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.0.1/docs/Makefile` & `mia-accounting-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/make.bat` & `mia-accounting-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.account.rst` & `mia-accounting-1.1.0/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.base_account.rst` & `mia-accounting-1.1.0/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.currency.rst` & `mia-accounting-1.1.0/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.1.0/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.1.0/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.1.0/docs/source/accounting.journal_entry.utils.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,14 @@
 ----------------------------------------------------------
 
 .. automodule:: accounting.journal_entry.utils.description_editor
    :members:
    :undoc-members:
    :show-inheritance:
 
-accounting.journal\_entry.utils.offset\_alias module
-----------------------------------------------------
-
-.. automodule:: accounting.journal_entry.utils.offset_alias
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 accounting.journal\_entry.utils.operators module
 ------------------------------------------------
 
 .. automodule:: accounting.journal_entry.utils.operators
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.0.1/docs/source/accounting.option.rst` & `mia-accounting-1.1.0/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.report.period.rst` & `mia-accounting-1.1.0/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.report.reports.rst` & `mia-accounting-1.1.0/docs/source/accounting.report.reports.rst`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,30 @@
 -----------------------------------------------
 
 .. automodule:: accounting.report.reports.trial_balance
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.report.reports.unapplied module
+------------------------------------------
+
+.. automodule:: accounting.report.reports.unapplied
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+accounting.report.reports.unapplied\_accounts module
+----------------------------------------------------
+
+.. automodule:: accounting.report.reports.unapplied_accounts
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: accounting.report.reports
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.0.1/docs/source/accounting.report.rst` & `mia-accounting-1.1.0/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/accounting.report.utils.rst` & `mia-accounting-1.1.0/docs/source/accounting.report.utils.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,22 @@
 -------------------------------------------
 
 .. automodule:: accounting.report.utils.report_type
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.report.utils.unapplied module
+----------------------------------------
+
+.. automodule:: accounting.report.utils.unapplied
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.report.utils.urls module
 -----------------------------------
 
 .. automodule:: accounting.report.utils.urls
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.0.1/docs/source/accounting.rst` & `mia-accounting-1.1.0/docs/source/accounting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
    accounting.account
    accounting.base_account
    accounting.currency
    accounting.journal_entry
    accounting.option
    accounting.report
+   accounting.unmatched_offset
    accounting.utils
 
 Submodules
 ----------
 
 accounting.forms module
 -----------------------
```

### Comparing `mia-accounting-1.0.1/docs/source/accounting.utils.rst` & `mia-accounting-1.1.0/docs/source/accounting.utils.rst`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,30 @@
 ---------------------------------
 
 .. automodule:: accounting.utils.next_uri
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.utils.offset\_alias module
+-------------------------------------
+
+.. automodule:: accounting.utils.offset_alias
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+accounting.utils.offset\_matcher module
+---------------------------------------
+
+.. automodule:: accounting.utils.offset_matcher
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.utils.options module
 -------------------------------
 
 .. automodule:: accounting.utils.options
    :members:
    :undoc-members:
    :show-inheritance:
@@ -88,14 +104,22 @@
 -----------------------------------
 
 .. automodule:: accounting.utils.strip_text
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.utils.unapplied module
+---------------------------------
+
+.. automodule:: accounting.utils.unapplied
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.utils.user module
 ----------------------------
 
 .. automodule:: accounting.utils.user
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.0.1/docs/source/conf.py` & `mia-accounting-1.1.0/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.0.1'
+release = '1.1.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.0.1/docs/source/examples.rst` & `mia-accounting-1.1.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/history.rst` & `mia-accounting-1.1.0/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/docs/source/intro.rst` & `mia-accounting-1.1.0/docs/source/intro.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,40 @@
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
-You may try the `live demonstration`_.
-
 
 Installation
 ------------
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
 You may also download the from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
+Test Site and Live Demonstration
+--------------------------------
+
+You may find a working example in the `test site`_ in the
+`source distribution`_.  It is the simplest website that works with
+*Mia! Accounting*.  It is used in the automatic tests.  It is the same
+code run for `live demonstration`_.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Prerequisites
 -------------
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.
 
 The following front-end JavaScript libraries must be loaded.  You may
@@ -98,41 +108,29 @@
         </div>
       </div>
     </nav>
 
 Check your Flask application and see how it works.
 
 
-Test Site and Live Demonstration
---------------------------------
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application, you may start with the
-test site.
-
-
 Documentation
 -------------
 
 Refer to the `documentation on Read the Docs`_.
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
+.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
-.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
-.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.0.1/pyproject.toml` & `mia-accounting-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.0.1"
+version = "1.1.0"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.0.1/src/accounting/__init__.py` & `mia-accounting-1.1.0/src/accounting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,8 +84,11 @@
 
     from . import report
     report.init_app(app, url_prefix)
 
     from . import option
     option.init_app(bp)
 
+    from . import unmatched_offset
+    unmatched_offset.init_app(bp)
+
     app.register_blueprint(bp, url_prefix=url_prefix)
```

### Comparing `mia-accounting-1.0.1/src/accounting/account/__init__.py` & `mia-accounting-1.1.0/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/account/commands.py` & `mia-accounting-1.1.0/src/accounting/account/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,23 +104,23 @@
 
     :param base_code: The code of the base account.
     :return: True if journal entry line items in the account need offset, or
         False otherwise.
     """
     # Assets
     if base_code[0] == "1":
-        if base_code[:3] in {"113", "114", "118", "184"}:
+        if base_code[:3] in {"113", "114", "118", "184", "186"}:
             return True
-        if base_code in {"1411", "1421", "1431", "1441", "1511", "1521",
-                         "1581", "1611", "1851", ""}:
+        if base_code in {"1286", "1411", "1421", "1431", "1441", "1511",
+                         "1521", "1581", "1611", "1851"}:
             return True
         return False
     # Liabilities
     if base_code[0] == "2":
-        if base_code in {"2111", "2114", "2284", "2293"}:
+        if base_code in {"2111", "2114", "2284", "2293", "2861"}:
             return False
         return True
     # Only assets and liabilities need offset
     return False
 
 
 def __add_accounting_accounts(data: list[AccountData], creator_pk: int)\
```

### Comparing `mia-accounting-1.0.1/src/accounting/account/converters.py` & `mia-accounting-1.1.0/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/account/forms.py` & `mia-accounting-1.1.0/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/account/queries.py` & `mia-accounting-1.1.0/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/account/views.py` & `mia-accounting-1.1.0/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/base_account/__init__.py` & `mia-accounting-1.1.0/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/base_account/commands.py` & `mia-accounting-1.1.0/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/base_account/converters.py` & `mia-accounting-1.1.0/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/base_account/queries.py` & `mia-accounting-1.1.0/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/base_account/views.py` & `mia-accounting-1.1.0/src/accounting/base_account/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 """
 from flask import Blueprint, render_template
 
 from accounting.models import BaseAccount
 from accounting.utils.pagination import Pagination
 from accounting.utils.permission import has_permission, can_view
+from .queries import get_base_account_query
 
 bp: Blueprint = Blueprint("base-account", __name__)
 """The view blueprint for the base account management."""
 
 
 @bp.get("", endpoint="list")
 @has_permission(can_view)
 def list_accounts() -> str:
     """Lists the base accounts.
 
     :return: The account list.
     """
-    from .queries import get_base_account_query
     accounts: list[BaseAccount] = get_base_account_query()
     pagination: Pagination = Pagination[BaseAccount](accounts)
     return render_template("accounting/base-account/list.html",
                            list=pagination.list, pagination=pagination)
 
 
 @bp.get("/<baseAccount:account>", endpoint="detail")
```

### Comparing `mia-accounting-1.0.1/src/accounting/currency/__init__.py` & `mia-accounting-1.1.0/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/currency/commands.py` & `mia-accounting-1.1.0/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/currency/converters.py` & `mia-accounting-1.1.0/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/currency/forms.py` & `mia-accounting-1.1.0/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/currency/queries.py` & `mia-accounting-1.1.0/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/currency/views.py` & `mia-accounting-1.1.0/src/accounting/currency/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 from accounting.utils.cast import s
 from accounting.utils.flash_errors import flash_form_errors
 from accounting.utils.next_uri import inherit_next, or_next
 from accounting.utils.pagination import Pagination
 from accounting.utils.permission import has_permission, can_view, can_edit
 from accounting.utils.user import get_current_user_pk
 from .forms import CurrencyForm
+from .queries import get_currency_query
 
 bp: Blueprint = Blueprint("currency", __name__)
 """The view blueprint for the currency management."""
 api_bp: Blueprint = Blueprint("currency-api", __name__)
 """The view blueprint for the currency management API."""
 
 
 @bp.get("", endpoint="list")
 @has_permission(can_view)
 def list_currencies() -> str:
     """Lists the currencies.
 
     :return: The currency list.
     """
-    from .queries import get_currency_query
     currencies: list[Currency] = get_currency_query()
     pagination: Pagination = Pagination[Currency](currencies)
     return render_template("accounting/currency/list.html",
                            list=pagination.list, pagination=pagination)
 
 
 @bp.get("/create", endpoint="create")
```

### Comparing `mia-accounting-1.0.1/src/accounting/data/base_accounts.csv` & `mia-accounting-1.1.0/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/forms.py` & `mia-accounting-1.1.0/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/converters.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,35 +19,30 @@
 """
 from datetime import date
 
 from flask import abort
 from sqlalchemy.orm import selectinload
 from werkzeug.routing import BaseConverter
 
+from accounting import db
 from accounting.models import JournalEntry, JournalEntryLineItem
 from accounting.utils.journal_entry_types import JournalEntryType
 
 
 class JournalEntryConverter(BaseConverter):
     """The journal entry converter to convert the journal entry ID from and to
     the corresponding journal entry in the routes."""
 
     def to_python(self, value: str) -> JournalEntry:
         """Converts a journal entry ID to a journal entry.
 
         :param value: The journal entry ID.
         :return: The corresponding journal entry.
         """
-        journal_entry: JournalEntry | None = JournalEntry.query\
-            .join(JournalEntryLineItem)\
-            .filter(JournalEntry.id == value)\
-            .options(selectinload(JournalEntry.line_items)
-                     .selectinload(JournalEntryLineItem.offsets)
-                     .selectinload(JournalEntryLineItem.journal_entry))\
-            .first()
+        journal_entry: JournalEntry | None = db.session.get(JournalEntry, value)
         if journal_entry is None:
             abort(404)
         return journal_entry
 
     def to_url(self, value: JournalEntry) -> str:
         """Converts a journal entry to its ID.
```

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/forms/currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,21 @@
 from flask_wtf import FlaskForm
 from wtforms import StringField, ValidationError, FieldList, IntegerField, \
     BooleanField, FormField
 from wtforms.validators import DataRequired
 
 from accounting import db
 from accounting.forms import CurrencyExists
-from accounting.journal_entry.utils.offset_alias import offset_alias
 from accounting.locale import lazy_gettext
 from accounting.models import JournalEntryLineItem
 from accounting.utils.cast import be
+from accounting.utils.offset_alias import offset_alias
 from accounting.utils.strip_text import strip_text
 from .line_item import LineItemForm, CreditLineItemForm, DebitLineItemForm
 
-
 CURRENCY_REQUIRED: DataRequired = DataRequired(
     lazy_gettext("Please select the currency."))
 """The validator to check if the currency code is empty."""
 
 
 class SameCurrencyAsOriginalLineItems:
     """The validator to check if the currency is the same as the
```

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/forms/line_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from wtforms import StringField, ValidationError, DecimalField, IntegerField
 from wtforms.validators import Optional
 
 from accounting import db
 from accounting.forms import ACCOUNT_REQUIRED, AccountExists, IsDebitAccount, \
     IsCreditAccount
 from accounting.locale import lazy_gettext
-from accounting.models import Account, JournalEntryLineItem
+from accounting.models import Account, JournalEntry, JournalEntryLineItem
 from accounting.template_filters import format_amount
 from accounting.utils.cast import be
 from accounting.utils.random_id import new_id
 from accounting.utils.strip_text import strip_text
 from accounting.utils.user import get_current_user_pk
 
 
@@ -123,18 +123,16 @@
 class KeepAccountWhenHavingOffset:
     """The validator to check if the account is the same when having offset."""
 
     def __call__(self, form: FlaskForm, field: StringField) -> None:
         assert isinstance(form, LineItemForm)
         if field.data is None or form.id.data is None:
             return
-        line_item: JournalEntryLineItem | None = db.session\
-            .query(JournalEntryLineItem)\
-            .filter(JournalEntryLineItem.id == form.id.data)\
-            .options(selectinload(JournalEntryLineItem.offsets)).first()
+        line_item: JournalEntryLineItem | None \
+            = db.session.get(JournalEntryLineItem, form.id.data)
         if line_item is None or len(line_item.offsets) == 0:
             return
         if field.data != line_item.account_code:
             raise ValidationError(lazy_gettext(
                 "The account must not be changed when there is offset."))
 
 
@@ -340,22 +338,21 @@
 
         :return: The offsets.
         """
         if not hasattr(self, "__offsets"):
             def get_offsets() -> list[JournalEntryLineItem]:
                 if not self.is_need_offset or self.id.data is None:
                     return []
-                return JournalEntryLineItem.query\
+                return JournalEntryLineItem.query.join(JournalEntry)\
                     .filter(JournalEntryLineItem.original_line_item_id
                             == self.id.data)\
+                    .order_by(JournalEntry.date, JournalEntry.no,
+                              JournalEntryLineItem.no)\
                     .options(selectinload(JournalEntryLineItem.journal_entry),
-                             selectinload(JournalEntryLineItem.account),
-                             selectinload(JournalEntryLineItem.offsets)
-                             .selectinload(
-                                 JournalEntryLineItem.journal_entry)).all()
+                             selectinload(JournalEntryLineItem.account)).all()
             setattr(self, "__offsets", get_offsets())
         return getattr(self, "__offsets")
 
     @property
     def offset_total(self) -> Decimal | None:
         """Returns the total amount of the offsets.
```

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/offset_alias.py` & `mia-accounting-1.1.0/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import sqlalchemy as sa
 from sqlalchemy.orm import selectinload
 
 from accounting import db
 from accounting.models import Account, JournalEntry, JournalEntryLineItem
 from accounting.utils.cast import be
-from .offset_alias import offset_alias
+from accounting.utils.offset_alias import offset_alias
 
 
 def get_selectable_original_line_items(
         line_item_id_on_form: set[int], is_payable: bool,
         is_receivable: bool) -> list[JournalEntryLineItem]:
     """Queries and returns the selectable original line items, with their net
     balances.  The offset amounts of the form is excluded.
```

### Comparing `mia-accounting-1.0.1/src/accounting/journal_entry/views.py` & `mia-accounting-1.1.0/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/locale.py` & `mia-accounting-1.1.0/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/models.py` & `mia-accounting-1.1.0/src/accounting/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,14 +211,33 @@
         """Returns whether the account is a nominal account.
 
         :return: True if the account is a nominal account, or False otherwise.
         """
         return not self.is_real
 
     @property
+    def count(self) -> int:
+        """Returns the number of items in the account.
+
+        :return: The number of items in the account.
+        """
+        if not hasattr(self, "__count"):
+            setattr(self, "__count", 0)
+        return getattr(self, "__count")
+
+    @count.setter
+    def count(self, count: int) -> None:
+        """Sets the number of items in the account.
+
+        :param count: The number of items in the account.
+        :return: None.
+        """
+        setattr(self, "__count", count)
+
+    @property
     def query_values(self) -> list[str]:
         """Returns the values to be queried.
 
         :return: The values to be queried.
         """
         return [self.code, self.title_l10n] + [x.title for x in self.l10n]
 
@@ -656,20 +675,16 @@
     no = db.Column(db.Integer, nullable=False)
     """The line item number under the journal entry and debit or credit."""
     original_line_item_id = db.Column(db.Integer,
                                       db.ForeignKey(id, onupdate="CASCADE"),
                                       nullable=True)
     """The ID of the original line item."""
     original_line_item = db.relationship("JournalEntryLineItem",
-                                         back_populates="offsets",
                                          remote_side=id, passive_deletes=True)
     """The original line item."""
-    offsets = db.relationship("JournalEntryLineItem",
-                              back_populates="original_line_item")
-    """The offset items."""
     currency_code = db.Column(db.String,
                               db.ForeignKey(Currency.code, onupdate="CASCADE"),
                               nullable=False)
     """The currency code."""
     currency = db.relationship(Currency, back_populates="line_items")
     """The currency."""
     account_id = db.Column(db.Integer,
@@ -704,36 +719,36 @@
         """Returns the account code.
 
         :return: The account code.
         """
         return self.account.code
 
     @property
-    def debit(self) -> Decimal | None:
-        """Returns the debit amount.
-
-        :return: The debit amount, or None if this is not a debit line item.
-        """
-        return self.amount if self.is_debit else None
-
-    @property
     def is_need_offset(self) -> bool:
         """Returns whether the line item needs offset.
 
         :return: True if the line item needs offset, or False otherwise.
         """
         if not self.account.is_need_offset:
             return False
         if self.account.base_code[0] == "1" and not self.is_debit:
             return False
         if self.account.base_code[0] == "2" and self.is_debit:
             return False
         return True
 
     @property
+    def debit(self) -> Decimal | None:
+        """Returns the debit amount.
+
+        :return: The debit amount, or None if this is not a debit line item.
+        """
+        return self.amount if self.is_debit else None
+
+    @property
     def credit(self) -> Decimal | None:
         """Returns the credit amount.
 
         :return: The credit amount, or None if this is not a credit line item.
         """
         return None if self.is_debit else self.amount
 
@@ -755,14 +770,48 @@
 
         :param net_balance: The net balance.
         :return: None.
         """
         setattr(self, "__net_balance", net_balance)
 
     @property
+    def offsets(self) -> list[t.Self]:
+        """Returns the offset items.
+
+        :return: The offset items.
+        """
+        if not hasattr(self, "__offsets"):
+            cls: t.Type[t.Self] = self.__class__
+            offsets: list[t.Self] = cls.query.join(JournalEntry)\
+                .filter(JournalEntryLineItem.original_line_item_id == self.id)\
+                .order_by(JournalEntry.date, JournalEntry.no,
+                          cls.is_debit, cls.no).all()
+            setattr(self, "__offsets", offsets)
+        return getattr(self, "__offsets")
+
+    @property
+    def match(self) -> t.Self | None:
+        """Returns the match of the line item.
+
+        :return: The match of the line item.
+        """
+        if not hasattr(self, "__match"):
+            setattr(self, "__match", None)
+        return getattr(self, "__match")
+
+    @match.setter
+    def match(self, match: t.Self) -> None:
+        """Sets the match of the line item.
+
+        :param match: The matcho of the line item.
+        :return: None.
+        """
+        setattr(self, "__match", match)
+
+    @property
     def query_values(self) -> list[str]:
         """Returns the values to be queried.
 
         :return: The values to be queried.
         """
         def format_amount(value: Decimal) -> str:
             whole: int = int(value)
```

### Comparing `mia-accounting-1.0.1/src/accounting/option/__init__.py` & `mia-accounting-1.1.0/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/option/forms.py` & `mia-accounting-1.1.0/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/option/views.py` & `mia-accounting-1.1.0/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/__init__.py` & `mia-accounting-1.1.0/src/accounting/report/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,13 +23,15 @@
 def init_app(app: Flask, url_prefix: str) -> None:
     """Initialize the application.
 
     :param app: The Flask application.
     :param url_prefix: The URL prefix of the accounting application.
     :return: None.
     """
-    from .converters import PeriodConverter, IncomeExpensesAccountConverter
+    from .converters import PeriodConverter, CurrentAccountConverter, \
+        NeedOffsetAccountConverter
     app.url_map.converters["period"] = PeriodConverter
-    app.url_map.converters["ieAccount"] = IncomeExpensesAccountConverter
+    app.url_map.converters["currentAccount"] = CurrentAccountConverter
+    app.url_map.converters["needOffsetAccount"] = NeedOffsetAccountConverter
 
     from .views import bp as report_bp
     app.register_blueprint(report_bp, url_prefix=url_prefix)
```

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/__init__.py` & `mia-accounting-1.1.0/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/chooser.py` & `mia-accounting-1.1.0/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/description.py` & `mia-accounting-1.1.0/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/month_end.py` & `mia-accounting-1.1.0/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/parser.py` & `mia-accounting-1.1.0/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/period.py` & `mia-accounting-1.1.0/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.1.0/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/period/specification.py` & `mia-accounting-1.1.0/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/__init__.py` & `mia-accounting-1.1.0/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.1.0/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.1.0/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.1.0/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/journal.py` & `mia-accounting-1.1.0/src/accounting/report/reports/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,16 @@
                  description: str | None,
                  debit: str | Decimal | None,
                  credit: str | Decimal | None,
                  note: str | None):
         """Constructs a row in the CSV.
 
         :param journal_entry_date: The journal entry date.
+        :param currency: The currency.
+        :param account: The account.
         :param description: The description.
         :param debit: The debit amount.
         :param credit: The credit amount.
         :param note: The note.
         """
         self.date: str | date = journal_entry_date
         """The date."""
@@ -112,14 +114,15 @@
 
     def __init__(self, period: Period,
                  pagination: Pagination[JournalEntryLineItem],
                  line_items: list[JournalEntryLineItem]):
         """Constructs the HTML page parameters.
 
         :param period: The period.
+        :param pagination: The pagination.
         :param line_items: The line items.
         """
         self.period: Period = period
         """The period."""
         self.pagination: Pagination[JournalEntryLineItem] = pagination
         """The pagination."""
         self.line_items: list[JournalEntryLineItem] = line_items
```

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/ledger.py` & `mia-accounting-1.1.0/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/search.py` & `mia-accounting-1.1.0/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.1.0/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/template_filters.py` & `mia-accounting-1.1.0/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/__init__.py` & `mia-accounting-1.1.0/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.1.0/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/base_report.py` & `mia-accounting-1.1.0/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.1.0/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/option_link.py` & `mia-accounting-1.1.0/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.1.0/src/accounting/report/utils/report_chooser.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accounting.models import Currency, Account
 from accounting.report.period import Period, get_period
 from accounting.template_globals import default_currency_code
 from accounting.utils.current_account import CurrentAccount
 from .option_link import OptionLink
 from .report_type import ReportType
 from .urls import journal_url, ledger_url, income_expenses_url, \
-    trial_balance_url, income_statement_url, balance_sheet_url
+    trial_balance_url, income_statement_url, balance_sheet_url, unapplied_url
 
 
 class ReportChooser:
     """The report chooser."""
 
     def __init__(self, active_report: ReportType,
                  period: Period | None = None,
@@ -70,14 +70,15 @@
         """Whether the current report is the search page."""
         self.__reports.append(self.__income_expenses)
         self.__reports.append(self.__ledger)
         self.__reports.append(self.__journal)
         self.__reports.append(self.__trial_balance)
         self.__reports.append(self.__income_statement)
         self.__reports.append(self.__balance_sheet)
+        self.__reports.append(self.__unapplied)
         for report in self.__reports:
             if report.is_active:
                 self.current_report = report.title
         if self.is_search:
             self.current_report = gettext("Search")
 
     @property
@@ -147,13 +148,30 @@
         :return: The balance sheet.
         """
         return OptionLink(gettext("Balance Sheet"),
                           balance_sheet_url(self.__currency, self.__period),
                           self.__active_report == ReportType.BALANCE_SHEET,
                           fa_icon="fa-solid fa-scale-balanced")
 
+    @property
+    def __unapplied(self) -> OptionLink:
+        """Returns the unapplied original line items.
+
+        :return: The unapplied original line items.
+        """
+        account: Account = self.__account
+        if not account.is_need_offset:
+            return OptionLink(gettext("Unapplied Original Line Items"),
+                              unapplied_url(None),
+                              self.__active_report == ReportType.UNAPPLIED,
+                              fa_icon="fa-solid fa-link-slash")
+        return OptionLink(gettext("Unapplied Original Line Items"),
+                          unapplied_url(account),
+                          self.__active_report == ReportType.UNAPPLIED,
+                          fa_icon="fa-solid fa-link-slash")
+
     def __iter__(self) -> t.Iterator[OptionLink]:
         """Returns the iteration of the reports.
 
         :return: The iteration of the reports.
         """
         return iter(self.__reports)
```

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/report_type.py` & `mia-accounting-1.1.0/src/accounting/report/utils/report_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,9 +30,11 @@
     """The income and expenses log."""
     TRIAL_BALANCE: str = "trial-balance"
     """The trial balance."""
     INCOME_STATEMENT: str = "income-statement"
     """The income statement."""
     BALANCE_SHEET: str = "balance-sheet"
     """The balance sheet."""
+    UNAPPLIED: str = "unapplied"
+    """The unapplied original line items."""
     SEARCH: str = "search"
     """The search."""
```

### Comparing `mia-accounting-1.0.1/src/accounting/report/utils/urls.py` & `mia-accounting-1.1.0/src/accounting/report/utils/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,7 +112,19 @@
     :return: The URL of the balance sheet.
     """
     if period.is_default:
         return url_for("accounting-report.balance-sheet-default",
                        currency=currency)
     return url_for("accounting-report.balance-sheet",
                    currency=currency, period=period)
+
+
+def unapplied_url(account: Account | None) -> str:
+    """Returns the URL of the unapplied original line items.
+
+    :param account: The account, or None to list the accounts with unapplied
+        original line items.
+    :return: The URL of the unapplied original line items.
+    """
+    if account is None:
+        return url_for("accounting-report.unapplied-default")
+    return url_for("accounting-report.unapplied", account=account)
```

### Comparing `mia-accounting-1.0.1/src/accounting/report/views.py` & `mia-accounting-1.1.0/src/accounting/report/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from accounting.report.period import Period, get_period
 from accounting.template_globals import default_currency_code
 from accounting.utils.current_account import CurrentAccount
 from accounting.utils.options import options
 from accounting.utils.permission import has_permission, can_view
 from .reports import Journal, Ledger, IncomeExpenses, TrialBalance, \
     IncomeStatement, BalanceSheet, Search
+from .reports.unapplied import UnappliedOriginalLineItems
+from .reports.unapplied_accounts import AccountsWithUnappliedOriginalLineItems
 from .template_filters import format_amount
 
 bp: Blueprint = Blueprint("accounting-report", __name__)
 """The view blueprint for the reports."""
 bp.add_app_template_filter(format_amount, "accounting_report_format_amount")
 
 
@@ -120,31 +122,30 @@
     """
     report: Ledger = Ledger(currency, account, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
-@bp.get("income-expenses/<currency:currency>/<ieAccount:account>",
+@bp.get("income-expenses/<currency:currency>/<currentAccount:account>",
         endpoint="income-expenses-default")
 @has_permission(can_view)
 def get_default_income_expenses(currency: Currency, account: CurrentAccount) \
         -> str | Response:
     """Returns the income and expenses log in the default period.
 
     :param currency: The currency.
     :param account: The account.
     :return: The income and expenses log in the default period.
     """
     return __get_income_expenses(currency, account, get_period())
 
 
-@bp.get(
-    "income-expenses/<currency:currency>/<ieAccount:account>/<period:period>",
-    endpoint="income-expenses")
+@bp.get("income-expenses/<currency:currency>/<currentAccount:account>/"
+        "<period:period>", endpoint="income-expenses")
 @has_permission(can_view)
 def get_income_expenses(currency: Currency, account: CurrentAccount,
                         period: Period) -> str | Response:
     """Returns the income and expenses log.
 
     :param currency: The currency.
     :param account: The account.
@@ -282,14 +283,42 @@
     """
     report: BalanceSheet = BalanceSheet(currency, period)
     if "as" in request.args and request.args["as"] == "csv":
         return report.csv()
     return report.html()
 
 
+@bp.get("unapplied", endpoint="unapplied-default")
+@has_permission(can_view)
+def get_default_unapplied() -> str | Response:
+    """Returns the accounts with unapplied original line items.
+
+    :return: The accounts with unapplied original line items.
+    """
+    report: AccountsWithUnappliedOriginalLineItems \
+        = AccountsWithUnappliedOriginalLineItems()
+    if "as" in request.args and request.args["as"] == "csv":
+        return report.csv()
+    return report.html()
+
+
+@bp.get("unapplied/<needOffsetAccount:account>", endpoint="unapplied")
+@has_permission(can_view)
+def get_unapplied(account: Account) -> str | Response:
+    """Returns the unapplied original line items.
+
+    :param account: The Account.
+    :return: The unapplied original line items.
+    """
+    report: UnappliedOriginalLineItems = UnappliedOriginalLineItems(account)
+    if "as" in request.args and request.args["as"] == "csv":
+        return report.csv()
+    return report.html()
+
+
 @bp.get("search", endpoint="search")
 @has_permission(can_view)
 def search() -> str | Response:
     """Returns the search result.
 
     :return: The search result.
     """
```

### Comparing `mia-accounting-1.0.1/src/accounting/static/css/style.css` & `mia-accounting-1.1.0/src/accounting/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -205,19 +205,31 @@
 }
 .accounting-report-table .accounting-amount {
     text-align: right;
 }
 .accounting-report-table-body .accounting-amount {
     font-style: italic;
 }
+.accounting-report-table-body .accounting-report-table-row {
+    background-color: #f8f9fa;
+}
 .accounting-report-table-body .accounting-report-table-row:nth-child(2n+1) {
-    background-color: #f2f2f2;
+    background-color: #ecedee;
 }
 .accounting-report-table-body .accounting-report-table-row:hover {
-    background-color: rgba(0, 0, 0, 0.075);
+    background-color: #e5e6e7;
+}
+.accounting-report-table-body .accounting-report-table-row-danger {
+    background-color: #f8d7da;
+}
+.accounting-report-table-body .accounting-report-table-row-danger:nth-child(2n+1) {
+    background-color: #eccccf;
+}
+.accounting-report-table-body .accounting-report-table-row-danger:hover {
+    background-color: #e5c7ca;
 }
 .accounting-journal-table .accounting-report-table-row {
     grid-template-columns: 1fr 1fr 2fr 4fr 1fr 1fr;
 }
 .accounting-ledger-real-table .accounting-report-table-row {
     grid-template-columns: 1fr 4fr 1fr 1fr 1fr;
 }
@@ -305,14 +317,24 @@
 }
 .accounting-balance-sheet-account {
     margin-left: 0.5rem;
 }
 .accounting-balance-sheet-total .accounting-amount, .accounting-balance-sheet-subtotal, .accounting-amount {
     font-style: italic;
 }
+.accounting-unapplied-table .accounting-report-table-row {
+    grid-template-columns: 1fr 1fr 5fr 1fr 1fr;
+}
+.accounting-unapplied-account-table .accounting-report-table-row {
+    display: flex;
+    justify-content: space-between;
+}
+.accounting-unapplied-account-table .accounting-report-table-header .accounting-report-table-row {
+    display: block;
+}
 
 /* The accounting report */
 .accounting-mobile-journal-credit {
     padding-left: 1rem;
 }
 
 /* The description editor */
@@ -339,14 +361,20 @@
 .accounting-recurring-description-template-illustration p {
     margin: 0.2rem 0;
 }
 .accounting-recurring-description-template-illustration ul {
     margin: 0;
 }
 
+/* The unmatched offsets */
+.accounting-unmatched-offset-pair-list {
+    height: 20rem;
+    overflow-y: scroll;
+}
+
 /* The Material Design text field (floating form control in Bootstrap) */
 .accounting-material-text-field {
     position: relative;
     min-height: calc(3.5rem + 2px);
     padding-top: 1.625rem;
 }
 .accounting-material-text-field > .form-label {
```

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/account-form.js` & `mia-accounting-1.1.0/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/account-order.js` & `mia-accounting-1.1.0/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/currency-form.js` & `mia-accounting-1.1.0/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/description-editor.js` & `mia-accounting-1.1.0/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.1.0/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -119,15 +119,15 @@
             if (option.isMatched(this.#isShowMore, codesInUse, this.#query.value)) {
                 option.setShown(true);
                 isAnyMatched = true;
             } else {
                 option.setShown(false);
             }
         }
-        if (!isAnyMatched) {
+        if (!isAnyMatched && this.#isShowMore) {
             this.#optionList.classList.add("d-none");
             this.#queryNoResult.classList.remove("d-none");
         } else {
             this.#optionList.classList.remove("d-none");
             this.#queryNoResult.classList.add("d-none");
         }
     }
```

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.1.0/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.1.0/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/option-form.js` & `mia-accounting-1.1.0/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.1.0/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.1.0/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/template_filters.py` & `mia-accounting-1.1.0/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/template_globals.py` & `mia-accounting-1.1.0/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/base.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/include/nav.html`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,20 @@
       </li>
       <li>
         <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.currency.") %} active {% endif %}" href="{{ url_for("accounting.currency.list") }}">
           <i class="fa-solid fa-money-bill-wave"></i>
           {{ A_("Currencies") }}
         </a>
       </li>
+      <li>
+        <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.unmatched-offset.") %} active {% endif %}" href="{{ url_for("accounting.unmatched-offset.dashboard") }}">
+          <i class="fa-solid fa-link-slash"></i>
+          {{ A_("Unmatched Offsets") }}
+        </a>
+      </li>
       {% if accounting_can_admin() %}
         <li>
           <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.option.") %} active {% endif %}" href="{{ url_for("accounting.option.detail") }}">
             <i class="fa-solid fa-gear"></i>
             {{ A_("Settings") }}
           </a>
         </li>
```

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,18 @@
                       <a href="{{ url_for("accounting.journal-entry.detail", journal_entry=offset.journal_entry)|accounting_append_next }}">
                         {{ offset.journal_entry.date|accounting_format_date }} {{ offset.amount|accounting_format_amount }}
                       </a>
                     </li>
                   {% endfor %}
                 </ul>
               </div>
-              {% if line_item.balance %}
+              {% if line_item.net_balance %}
                 <div class="d-flex justify-content-between">
                   <div>{{ A_("Net balance") }}</div>
-                  <div>{{ line_item.balance|accounting_format_amount }}</div>
+                  <div>{{ line_item.net_balance|accounting_format_amount }}</div>
                 </div>
               {% else %}
                 <div class="d-flex justify-content-between">
                   <div>{{ A_("Fully offset") }}</div>
                 </div>
               {% endif %}
             {% else %}
```

#### html2text {}

```diff
@@ -22,17 +22,17 @@
 {{ A_("Offsets") }}
     * {% for offset in line_item.offsets %}
     * journal-entry.detail",
       journal_entry=offset.journal_entry)|accounting_append_next }}"> {
       { offset.journal_entry.date|accounting_format_date }} {
       { offset.amount|accounting_format_amount }}
 {% endfor %}
-{% if line_item.balance %}
+{% if line_item.net_balance %}
 {{ A_("Net balance") }}
-{{ line_item.balance|accounting_format_amount }}
+{{ line_item.net_balance|accounting_format_amount }}
 {% else %}
 {{ A_("Fully offset") }}
 {% endif %} {% else %}
 {{ A_("Unmatched") }}
 {% endif %}
 {% endif %}
 {{ line_item.amount|accounting_format_amount }}
```

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/detail.html`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,19 @@
   </a>
 </div>
 
 <table class="table table-striped table-hover table-light" aria-label="{{ A_("Settings") }}">
 <tbody>
 <tr>
   <th scope="row">{{ A_("Default Currency") }}</th>
-  <td>{{ obj.default_currency_text }}</td>
+  <td>{{ obj.default_currency }}</td>
 </tr>
 <tr>
   <th scope="row">{{ A_("Default Account for the Income and Expenses Log") }}</th>
-  <td>{{ obj.default_ie_account_code_text }}</td>
+  <td>{{ obj.default_ie_account }}</td>
 </tr>
 </tbody>
 </table>
 
 <h2>{{ A_("Recurring Expense") }}</h2>
 
 {% if obj.recurring.expenses %}
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/22 #} {%
 extends "accounting/base.html" %} {% block header %}{% block title %}{{ A_
 ("Settings") }}{% endblock %}{% endblock %} {% block content %}
 option.edit")|accounting_inherit_next }}">  {{ A_("Edit") }}
 option.edit")|accounting_inherit_next }}">
 ) }}">
 {{ A_("Default Currency") }}
-{{ obj.default_currency_text }}
+{{ obj.default_currency }}
 {{ A_("Default Account for the Income and Expenses Log") }}
-{{ obj.default_ie_account_code_text }}
+{{ obj.default_ie_account }}
 ***** {{ A_("Recurring Expense") }} *****
 {% if obj.recurring.expenses %}
     * {% for recurring_item in obj.recurring.expenses %}
     * {{ recurring_item.account_text }}
       {{ recurring_item.name }}
       {{ recurring_item.description_template }}
     * {% endfor %}
```

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.1.0/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/translations/accounting.pot` & `mia-accounting-1.1.0/src/accounting/translations/accounting.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
+"POT-Creation-Date: 2023-04-09 00:22+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -29,30 +29,30 @@
 msgid "The currency does not exist."
 msgstr ""
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr ""
 
-#: src/accounting/models.py:562
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:565
+#: src/accounting/models.py:584
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:566
+#: src/accounting/models.py:585
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:699
+#: src/accounting/models.py:714
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr ""
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -199,32 +199,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr ""
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:40
+#: src/accounting/journal_entry/forms/currency.py:39
 msgid "Please select the currency."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:63
+#: src/accounting/journal_entry/forms/currency.py:62
 msgid "The currency must be the same as the original line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:90
+#: src/accounting/journal_entry/forms/currency.py:89
 msgid "The currency must not be changed when there is offset."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:99
+#: src/accounting/journal_entry/forms/currency.py:98
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:112
+#: src/accounting/journal_entry/forms/currency.py:111
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr ""
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -265,50 +265,50 @@
 msgid "The original line item cannot be an offset item."
 msgstr ""
 
 #: src/accounting/journal_entry/forms/line_item.py:119
 msgid "The account must be the same as the original line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:137
+#: src/accounting/journal_entry/forms/line_item.py:135
 msgid "The account must not be changed when there is offset."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:153
+#: src/accounting/journal_entry/forms/line_item.py:151
 msgid "A payable line item cannot start from debit."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:169
+#: src/accounting/journal_entry/forms/line_item.py:167
 msgid "A receivable line item cannot start from credit."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:180
+#: src/accounting/journal_entry/forms/line_item.py:178
 #: src/accounting/static/js/journal-entry-line-item-editor.js:436
 msgid "Please fill in a positive amount."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:222
+#: src/accounting/journal_entry/forms/line_item.py:220
 #: src/accounting/static/js/journal-entry-line-item-editor.js:442
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:243
+#: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:416
+#: src/accounting/journal_entry/forms/line_item.py:413
 msgid "This account is not for debit line items."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:468
+#: src/accounting/journal_entry/forms/line_item.py:465
 msgid "This account is not for credit line items."
 msgstr ""
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr ""
 
@@ -436,47 +436,52 @@
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:50
 msgid "Date"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unapplied_accounts.py:109
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:55
 msgid "Account"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:408
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
+#: src/accounting/templates/accounting/report/unapplied.html:52
 msgid "Description"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr ""
@@ -490,15 +495,15 @@
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 msgid "Balance"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:410
-#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:228
@@ -522,52 +527,72 @@
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/income-statement.html:55
+#: src/accounting/templates/accounting/report/unapplied.html:53
 msgid "Amount"
 msgstr ""
 
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
+#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr ""
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:56
 msgid "Debit"
 msgstr ""
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
 #: src/accounting/templates/accounting/report/trial-balance.html:57
 msgid "Credit"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:81
+#: src/accounting/report/reports/unapplied.py:121
+#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/templates/accounting/include/nav.html:39
+msgid "Accounts"
+msgstr ""
+
+#: src/accounting/report/reports/unapplied.py:139
+#: src/accounting/templates/accounting/report/unapplied.html:54
+msgid "Net Balance"
+msgstr ""
+
+#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+msgid "Count"
+msgstr ""
+
+#: src/accounting/report/utils/report_chooser.py:82
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -575,38 +600,43 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:92
+#: src/accounting/report/utils/report_chooser.py:93
 msgid "Income and Expenses Log"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:105
+#: src/accounting/report/utils/report_chooser.py:106
 msgid "Ledger"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:117
+#: src/accounting/report/utils/report_chooser.py:118
 msgid "Journal"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:127
+#: src/accounting/report/utils/report_chooser.py:128
 msgid "Trial Balance"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:138
+#: src/accounting/report/utils/report_chooser.py:139
 msgid "Income Statement"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:149
+#: src/accounting/report/utils/report_chooser.py:150
 msgid "Balance Sheet"
 msgstr ""
 
+#: src/accounting/report/utils/report_chooser.py:163
+#: src/accounting/report/utils/report_chooser.py:167
+msgid "Unapplied Original Line Items"
+msgstr ""
+
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr ""
 
 #: src/accounting/static/js/description-editor.js:951
 #: src/accounting/static/js/description-editor.js:1129
 msgid "Please fill in the tag."
@@ -720,14 +750,15 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -760,14 +791,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
+#: src/accounting/templates/accounting/unmatched-offset/list.html:54
 msgid "Close"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr ""
 
@@ -777,21 +809,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:70
 msgid "Cancel"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
+#: src/accounting/templates/accounting/unmatched-offset/list.html:71
 msgid "Confirm"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -843,14 +877,18 @@
 #: src/accounting/templates/accounting/report/balance-sheet.html:110
 #: src/accounting/templates/accounting/report/income-expenses.html:113
 #: src/accounting/templates/accounting/report/income-statement.html:96
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
 #: src/accounting/templates/accounting/report/trial-balance.html:82
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:98
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:104
 msgid "There is no data."
 msgstr ""
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr ""
@@ -932,27 +970,28 @@
 msgid "Accounting"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/nav.html:33
 msgid "Reports"
 msgstr ""
 
-#: src/accounting/templates/accounting/include/nav.html:39
-msgid "Accounts"
-msgstr ""
-
 #: src/accounting/templates/accounting/include/nav.html:45
 msgid "Base Accounts"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr ""
 
-#: src/accounting/templates/accounting/include/nav.html:58
+#: src/accounting/templates/accounting/include/nav.html:57
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
+msgid "Unmatched Offsets"
+msgstr ""
+
+#: src/accounting/templates/accounting/include/nav.html:64
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1204,14 +1243,29 @@
 
 #: src/accounting/templates/accounting/report/trial-balance.html:29
 #: src/accounting/templates/accounting/report/trial-balance.html:49
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr ""
 
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
+msgid "Accounts with Unapplied Original Line Items"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/unapplied.html:28
+#, python-format
+msgid "Unapplied Original Line Items of %(account)s"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/unapplied.html:65
+#, python-format
+msgid "Can match %(offset)s"
+msgstr ""
+
 #: src/accounting/templates/accounting/report/include/period-chooser.html:26
 msgid "Period Chooser"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:34
 msgid "Month"
 msgstr ""
@@ -1237,14 +1291,73 @@
 msgstr ""
 
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
 msgid "Download"
 msgstr ""
 
+#: src/accounting/templates/accounting/unmatched-offset/list.html:24
+#, python-format
+msgid "Unmatched Offsets in %(account)s"
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:28
+msgid "Toolbar"
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:41
+msgid "Match"
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:53
+msgid "Confirm Match Offsets"
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:57
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:81
+#, python-format
+msgid ""
+"%(matches)s unapplied original line items out of %(total)s can match with"
+" their offsets."
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:83
+#, python-format
+msgid "%(total)s unapplied original line items without matching offsets."
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:85
+msgid "Go to unapplied original line items."
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:87
+msgid "All original line items are fully offset."
+msgstr ""
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:98
+#, python-format
+msgid "Can match %(item)s"
+msgstr ""
+
+#: src/accounting/unmatched_offset/views.py:71
+msgid "No more offset to match automatically."
+msgstr ""
+
+#: src/accounting/unmatched_offset/views.py:77
+#, python-format
+msgid "Matches %(matches)s from %(total)s unapplied line items."
+msgstr ""
+
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr ""
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
 msgid "Previous"
```

### Comparing `mia-accounting-1.0.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.0.0\n"
+"Project-Id-Version: mia-accounting 1.1.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
-"PO-Revision-Date: 2023-04-06 02:34+0800\n"
+"POT-Creation-Date: 2023-04-09 00:22+0800\n"
+"PO-Revision-Date: 2023-04-09 00:37+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,14 +18,22 @@
 
 msgid "%(currency)s Settings"
 msgstr "%(currency)s设置"
 
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
+msgid ""
+"%(matches)s unapplied original line items out of %(total)s can match with "
+"their offsets."
+msgstr "%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
+
+msgid "%(total)s unapplied original line items without matching offsets."
+msgstr "%(total)s 笔未抵销原始分录，无法自动配对抵销。"
+
 msgid "(Unknown)"
 msgstr "（不明）"
 
 msgid "A nominal account does not need offset."
 msgstr "虚科目不需抵销。"
 
 msgid "A payable line item cannot start from debit."
@@ -42,14 +50,17 @@
 
 msgid "Accounting"
 msgstr "记帐"
 
 msgid "Accounts"
 msgstr "科目"
 
+msgid "Accounts with Unapplied Original Line Items"
+msgstr "有未抵销原始分录的科目"
+
 msgid "Add a New Account"
 msgstr "添加科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "添加现金支出传票"
 
 msgid "Add a New Cash Receipt Journal Entry"
@@ -60,14 +71,17 @@
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "添加转帐传票"
 
 msgid "All"
 msgstr "全部"
 
+msgid "All original line items are fully offset."
+msgstr "原始分录已全部抵销。"
+
 msgid "Amount"
 msgstr "金额"
 
 msgid "Annotation"
 msgstr "注记"
 
 msgid "April"
@@ -105,14 +119,20 @@
 
 msgid "Brought forward"
 msgstr "前期转入"
 
 msgid "Bus"
 msgstr "公车"
 
+msgid "Can match %(item)s"
+msgstr "可抵销 %(item)s"
+
+msgid "Can match %(offset)s"
+msgstr "可抵销 %(offset)s"
+
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Cash Disbursement"
 msgstr "现金支出"
 
 msgid "Cash Disbursement Journal Entry#%(id)s"
@@ -147,17 +167,23 @@
 
 msgid "Confirm Delete Currency"
 msgstr "确认删除货币"
 
 msgid "Confirm Delete Journal Entry"
 msgstr "确认删除传票"
 
+msgid "Confirm Match Offsets"
+msgstr "确认抵销"
+
 msgid "Content"
 msgstr "内容"
 
+msgid "Count"
+msgstr "数量"
+
 msgid "Created"
 msgstr "建档"
 
 msgid "Credit"
 msgstr "贷方"
 
 msgid "Currencies"
@@ -204,14 +230,22 @@
 
 msgid "Do you really want to delete this currency?"
 msgstr "你确定要删掉这个货币吗？"
 
 msgid "Do you really want to delete this journal entry?"
 msgstr "你确定要删掉这张传票吗？"
 
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr ""
+"你确定要抵销下列原始分录与抵销分录吗？结果无法复原。请先备份数据库，并仔细核"
+"对抵销分录是否正确。"
+
 msgid "Download"
 msgstr "下载"
 
 msgid "Edit"
 msgstr "编辑"
 
 msgid "Editing %(journal_entry)s"
@@ -231,14 +265,17 @@
 
 msgid "Fully offset"
 msgstr "全部抵销"
 
 msgid "General"
 msgstr "一般"
 
+msgid "Go to unapplied original line items."
+msgstr "查阅未抵销原始分录。"
+
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "损益表"
 
 msgid "Income Statement of %(currency)s %(period)s"
@@ -291,14 +328,20 @@
 
 msgid "Line items with offset cannot be deleted."
 msgstr "无法删除抵销过的分录。"
 
 msgid "March"
 msgstr "三月"
 
+msgid "Match"
+msgstr "抵销"
+
+msgid "Matches %(matches)s from %(total)s unapplied line items."
+msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches) 笔。"
+
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
 
 msgid "More…"
@@ -306,24 +349,30 @@
 
 msgid "Name"
 msgstr "名称"
 
 msgid "Needs Offset"
 msgstr "需抵销"
 
+msgid "Net Balance"
+msgstr "净额"
+
 msgid "Net balance"
 msgstr "净额"
 
 msgid "New"
 msgstr "添加"
 
 msgctxt "Pagination|"
 msgid "Next"
 msgstr "下一页"
 
+msgid "No more offset to match automatically."
+msgstr "无法自动配对抵销。"
+
 msgid "Note"
 msgstr "备注"
 
 msgid "November"
 msgstr "十一月"
 
 msgid "October"
@@ -652,14 +701,17 @@
 
 msgid "Today"
 msgstr "今天"
 
 msgid "Tomorrow"
 msgstr "明天"
 
+msgid "Toolbar"
+msgstr "工具列"
+
 msgid "Total"
 msgstr "合计"
 
 msgid "Transfer"
 msgstr "转帐"
 
 msgid "Transfer Journal Entry#%(id)s"
@@ -670,17 +722,29 @@
 
 msgid "Trial Balance"
 msgstr "试算表"
 
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
+msgid "Unapplied Original Line Items"
+msgstr "未抵销原始分录"
+
+msgid "Unapplied Original Line Items of %(account)s"
+msgstr "%(account)s未抵销原始分录"
+
 msgid "Unmatched"
 msgstr "未抵销"
 
+msgid "Unmatched Offsets"
+msgstr "遗漏的抵销分录"
+
+msgid "Unmatched Offsets in %(account)s"
+msgstr "%(account)s遗漏的抵销分录"
+
 msgid "Updated"
 msgstr "更新"
 
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水费{last_bimonthly_number}月"
 
 msgid "Year"
```

### Comparing `mia-accounting-1.0.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.1.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.0.0\n"
+"Project-Id-Version: mia-accounting 1.1.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
-"PO-Revision-Date: 2023-04-06 02:34+0800\n"
+"POT-Creation-Date: 2023-04-09 00:22+0800\n"
+"PO-Revision-Date: 2023-04-09 00:37+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -31,30 +31,30 @@
 msgid "The currency does not exist."
 msgstr "没有这个货币。"
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr "没有这个科目。"
 
-#: src/accounting/models.py:562
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr "现金支出传票#%(id)s"
 
-#: src/accounting/models.py:565
+#: src/accounting/models.py:584
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr "现金收入传票#%(id)s"
 
-#: src/accounting/models.py:566
+#: src/accounting/models.py:585
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "转帐传票#%(id)s"
 
-#: src/accounting/models.py:699
+#: src/accounting/models.py:714
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -201,32 +201,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr "传票不可删除。"
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr "传票删掉了"
 
-#: src/accounting/journal_entry/forms/currency.py:40
+#: src/accounting/journal_entry/forms/currency.py:39
 msgid "Please select the currency."
 msgstr "请选择货币。"
 
-#: src/accounting/journal_entry/forms/currency.py:63
+#: src/accounting/journal_entry/forms/currency.py:62
 msgid "The currency must be the same as the original line item."
 msgstr "货币需和原始分录相同。"
 
-#: src/accounting/journal_entry/forms/currency.py:90
+#: src/accounting/journal_entry/forms/currency.py:89
 msgid "The currency must not be changed when there is offset."
 msgstr "抵销过不可变更货币。"
 
-#: src/accounting/journal_entry/forms/currency.py:99
+#: src/accounting/journal_entry/forms/currency.py:98
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr "请加上分录。"
 
-#: src/accounting/journal_entry/forms/currency.py:112
+#: src/accounting/journal_entry/forms/currency.py:111
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方贷方合计不符。 "
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -267,50 +267,50 @@
 msgid "The original line item cannot be an offset item."
 msgstr "原始分录不可以是抵销分录。"
 
 #: src/accounting/journal_entry/forms/line_item.py:119
 msgid "The account must be the same as the original line item."
 msgstr "科目需和原始分录相同。"
 
-#: src/accounting/journal_entry/forms/line_item.py:137
+#: src/accounting/journal_entry/forms/line_item.py:135
 msgid "The account must not be changed when there is offset."
 msgstr "抵销过不可变更科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:153
+#: src/accounting/journal_entry/forms/line_item.py:151
 msgid "A payable line item cannot start from debit."
 msgstr "不可由借方新建应付款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:169
+#: src/accounting/journal_entry/forms/line_item.py:167
 msgid "A receivable line item cannot start from credit."
 msgstr "不可由贷方新建应收款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:180
+#: src/accounting/journal_entry/forms/line_item.py:178
 #: src/accounting/static/js/journal-entry-line-item-editor.js:436
 msgid "Please fill in a positive amount."
 msgstr "金额请填正数。"
 
-#: src/accounting/journal_entry/forms/line_item.py:222
+#: src/accounting/journal_entry/forms/line_item.py:220
 #: src/accounting/static/js/journal-entry-line-item-editor.js:442
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr "金额不可超过原始分录净额 %(balance)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:243
+#: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金额不可低于抵销总额 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:416
+#: src/accounting/journal_entry/forms/line_item.py:413
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:468
+#: src/accounting/journal_entry/forms/line_item.py:465
 msgid "This account is not for credit line items."
 msgstr "科目不是贷方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "这不是流动科目。"
 
@@ -438,47 +438,52 @@
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr "前期转入"
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:50
 msgid "Date"
 msgstr "日期"
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unapplied_accounts.py:109
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:55
 msgid "Account"
 msgstr "科目"
 
 #: src/accounting/report/reports/income_expenses.py:408
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
+#: src/accounting/templates/accounting/report/unapplied.html:52
 msgid "Description"
 msgstr "摘要"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
@@ -492,15 +497,15 @@
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 msgid "Balance"
 msgstr "余额"
 
 #: src/accounting/report/reports/income_expenses.py:410
-#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr "备注"
 
 #: src/accounting/report/reports/income_statement.py:228
@@ -524,52 +529,72 @@
 msgstr "税后净利"
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr "本期损益"
 
 #: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/income-statement.html:55
+#: src/accounting/templates/accounting/report/unapplied.html:53
 msgid "Amount"
 msgstr "金额"
 
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
+#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr "货币"
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:56
 msgid "Debit"
 msgstr "借方"
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
 #: src/accounting/templates/accounting/report/trial-balance.html:57
 msgid "Credit"
 msgstr "贷方"
 
-#: src/accounting/report/utils/report_chooser.py:81
+#: src/accounting/report/reports/unapplied.py:121
+#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/templates/accounting/include/nav.html:39
+msgid "Accounts"
+msgstr "科目"
+
+#: src/accounting/report/reports/unapplied.py:139
+#: src/accounting/templates/accounting/report/unapplied.html:54
+msgid "Net Balance"
+msgstr "净额"
+
+#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+msgid "Count"
+msgstr "数量"
+
+#: src/accounting/report/utils/report_chooser.py:82
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -577,38 +602,43 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr "搜索"
 
-#: src/accounting/report/utils/report_chooser.py:92
+#: src/accounting/report/utils/report_chooser.py:93
 msgid "Income and Expenses Log"
 msgstr "收支帐"
 
-#: src/accounting/report/utils/report_chooser.py:105
+#: src/accounting/report/utils/report_chooser.py:106
 msgid "Ledger"
 msgstr "分类帐"
 
-#: src/accounting/report/utils/report_chooser.py:117
+#: src/accounting/report/utils/report_chooser.py:118
 msgid "Journal"
 msgstr "日记簿"
 
-#: src/accounting/report/utils/report_chooser.py:127
+#: src/accounting/report/utils/report_chooser.py:128
 msgid "Trial Balance"
 msgstr "试算表"
 
-#: src/accounting/report/utils/report_chooser.py:138
+#: src/accounting/report/utils/report_chooser.py:139
 msgid "Income Statement"
 msgstr "损益表"
 
-#: src/accounting/report/utils/report_chooser.py:149
+#: src/accounting/report/utils/report_chooser.py:150
 msgid "Balance Sheet"
 msgstr "资产负债表"
 
+#: src/accounting/report/utils/report_chooser.py:163
+#: src/accounting/report/utils/report_chooser.py:167
+msgid "Unapplied Original Line Items"
+msgstr "未抵销原始分录"
+
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr "请填上标题。"
 
 #: src/accounting/static/js/description-editor.js:951
 #: src/accounting/static/js/description-editor.js:1129
 msgid "Please fill in the tag."
@@ -722,14 +752,15 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr "回上页"
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -762,14 +793,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
+#: src/accounting/templates/accounting/unmatched-offset/list.html:54
 msgid "Close"
 msgstr "关闭"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你确定要删掉这个科目吗？"
 
@@ -779,21 +811,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:70
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
+#: src/accounting/templates/accounting/unmatched-offset/list.html:71
 msgid "Confirm"
 msgstr "确定"
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -845,14 +879,18 @@
 #: src/accounting/templates/accounting/report/balance-sheet.html:110
 #: src/accounting/templates/accounting/report/income-expenses.html:113
 #: src/accounting/templates/accounting/report/income-statement.html:96
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
 #: src/accounting/templates/accounting/report/trial-balance.html:82
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:98
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:104
 msgid "There is no data."
 msgstr "没有数据。"
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
@@ -934,27 +972,28 @@
 msgid "Accounting"
 msgstr "记帐"
 
 #: src/accounting/templates/accounting/include/nav.html:33
 msgid "Reports"
 msgstr "报表"
 
-#: src/accounting/templates/accounting/include/nav.html:39
-msgid "Accounts"
-msgstr "科目"
-
 #: src/accounting/templates/accounting/include/nav.html:45
 msgid "Base Accounts"
 msgstr "基本科目"
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr "货币"
 
-#: src/accounting/templates/accounting/include/nav.html:58
+#: src/accounting/templates/accounting/include/nav.html:57
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
+msgid "Unmatched Offsets"
+msgstr "遗漏的抵销分录"
+
+#: src/accounting/templates/accounting/include/nav.html:64
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr "设置"
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1206,14 +1245,29 @@
 
 #: src/accounting/templates/accounting/report/trial-balance.html:29
 #: src/accounting/templates/accounting/report/trial-balance.html:49
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:41x
+msgid "Accounts with Unapplied Original Line Items"
+msgstr "有未抵销原始分录的科目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:28
+#, python-format
+msgid "Unapplied Original Line Items of %(account)s"
+msgstr "%(account)s未抵销原始分录"
+
+#: src/accounting/templates/accounting/report/unapplied.html:65
+#, python-format
+msgid "Can match %(offset)s"
+msgstr "可抵销 %(offset)s"
+
 #: src/accounting/templates/accounting/report/include/period-chooser.html:26
 msgid "Period Chooser"
 msgstr "选择日期范围"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:34
 msgid "Month"
 msgstr "月"
@@ -1239,14 +1293,74 @@
 msgstr "期间"
 
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
 msgid "Download"
 msgstr "下载"
 
+#: src/accounting/templates/accounting/unmatched-offset/list.html:24
+#, python-format
+msgid "Unmatched Offsets in %(account)s"
+msgstr "%(account)s遗漏的抵销分录"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:28
+msgid "Toolbar"
+msgstr "工具列"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:41
+msgid "Match"
+msgstr "抵销"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:53
+msgid "Confirm Match Offsets"
+msgstr "确认抵销"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:57
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr "你确定要抵销下列原始分录与抵销分录吗？结果无法复原。请先备份数据库，并仔细核对抵销分录是否正确。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:81
+#, python-format
+msgid ""
+"%(matches)s unapplied original line items out of %(total)s can match with"
+" their offsets."
+msgstr ""
+"%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:83
+#, python-format
+msgid "%(total)s unapplied original line items without matching offsets."
+msgstr "%(total)s 笔未抵销原始分录，无法自动配对抵销。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:85
+msgid "Go to unapplied original line items."
+msgstr "查阅未抵销原始分录。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:87
+msgid "All original line items are fully offset."
+msgstr "原始分录已全部抵销。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:98
+#, python-format
+msgid "Can match %(item)s"
+msgstr "可抵销 %(item)s"
+
+#: src/accounting/unmatched_offset/views.py:71
+msgid "No more offset to match automatically."
+msgstr "无法自动配对抵销。"
+
+#: src/accounting/unmatched_offset/views.py:77
+#, python-format
+msgid "Matches %(matches)s from %(total)s unapplied line items."
+msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches) 笔。"
+
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流动资产与负债"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
 msgid "Previous"
```

### Comparing `mia-accounting-1.0.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.0.0\n"
+"Project-Id-Version: mia-accounting 1.1.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
-"PO-Revision-Date: 2023-04-06 02:34+0800\n"
+"POT-Creation-Date: 2023-04-09 00:22+0800\n"
+"PO-Revision-Date: 2023-04-09 00:37+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,14 +18,22 @@
 
 msgid "%(currency)s Settings"
 msgstr "%(currency)s設定"
 
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
+msgid ""
+"%(matches)s unapplied original line items out of %(total)s can match with "
+"their offsets."
+msgstr "%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
+
+msgid "%(total)s unapplied original line items without matching offsets."
+msgstr "%(total)s 筆未抵銷原始分錄，無法自動配對抵銷。"
+
 msgid "(Unknown)"
 msgstr "（不明）"
 
 msgid "A nominal account does not need offset."
 msgstr "虛科目不需抵銷。"
 
 msgid "A payable line item cannot start from debit."
@@ -42,14 +50,17 @@
 
 msgid "Accounting"
 msgstr "記帳"
 
 msgid "Accounts"
 msgstr "科目"
 
+msgid "Accounts with Unapplied Original Line Items"
+msgstr "有未抵銷原始分錄的科目"
+
 msgid "Add a New Account"
 msgstr "新增科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "新增現金支出傳票"
 
 msgid "Add a New Cash Receipt Journal Entry"
@@ -60,14 +71,17 @@
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "新增轉帳傳票"
 
 msgid "All"
 msgstr "全部"
 
+msgid "All original line items are fully offset."
+msgstr "原始分錄已全部抵銷。"
+
 msgid "Amount"
 msgstr "金額"
 
 msgid "Annotation"
 msgstr "註記"
 
 msgid "April"
@@ -105,14 +119,20 @@
 
 msgid "Brought forward"
 msgstr "前期轉入"
 
 msgid "Bus"
 msgstr "公車"
 
+msgid "Can match %(item)s"
+msgstr "可抵銷 %(item)s"
+
+msgid "Can match %(offset)s"
+msgstr "可抵銷 %(offset)s"
+
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Cash Disbursement"
 msgstr "現金支出"
 
 msgid "Cash Disbursement Journal Entry#%(id)s"
@@ -147,17 +167,23 @@
 
 msgid "Confirm Delete Currency"
 msgstr "確認刪除貨幣"
 
 msgid "Confirm Delete Journal Entry"
 msgstr "確認刪除傳票"
 
+msgid "Confirm Match Offsets"
+msgstr "確認抵銷"
+
 msgid "Content"
 msgstr "內容"
 
+msgid "Count"
+msgstr "數量"
+
 msgid "Created"
 msgstr "建檔"
 
 msgid "Credit"
 msgstr "貸方"
 
 msgid "Currencies"
@@ -204,14 +230,22 @@
 
 msgid "Do you really want to delete this currency?"
 msgstr "你確定要刪掉這個貨幣嗎？"
 
 msgid "Do you really want to delete this journal entry?"
 msgstr "你確定要刪掉這張傳票嗎？"
 
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr ""
+"你確定要抵銷下列原始分錄與抵銷分錄嗎？結果無法復原。請先備份資料庫，並仔細核"
+"對抵銷分錄是否正確。"
+
 msgid "Download"
 msgstr "下載"
 
 msgid "Edit"
 msgstr "編輯"
 
 msgid "Editing %(journal_entry)s"
@@ -231,14 +265,17 @@
 
 msgid "Fully offset"
 msgstr "全部抵銷"
 
 msgid "General"
 msgstr "一般"
 
+msgid "Go to unapplied original line items."
+msgstr "查閱未抵銷原始分錄。"
+
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "損益表"
 
 msgid "Income Statement of %(currency)s %(period)s"
@@ -291,14 +328,20 @@
 
 msgid "Line items with offset cannot be deleted."
 msgstr "無法刪除抵銷過的分錄。"
 
 msgid "March"
 msgstr "三月"
 
+msgid "Match"
+msgstr "抵銷"
+
+msgid "Matches %(matches)s from %(total)s unapplied line items."
+msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches) 筆。"
+
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
 
 msgid "More…"
@@ -306,24 +349,30 @@
 
 msgid "Name"
 msgstr "名稱"
 
 msgid "Needs Offset"
 msgstr "需抵銷"
 
+msgid "Net Balance"
+msgstr "淨額"
+
 msgid "Net balance"
 msgstr "淨額"
 
 msgid "New"
 msgstr "新增"
 
 msgctxt "Pagination|"
 msgid "Next"
 msgstr "下一頁"
 
+msgid "No more offset to match automatically."
+msgstr "無法自動配對抵銷。"
+
 msgid "Note"
 msgstr "備註"
 
 msgid "November"
 msgstr "十一月"
 
 msgid "October"
@@ -652,14 +701,17 @@
 
 msgid "Today"
 msgstr "今天"
 
 msgid "Tomorrow"
 msgstr "明天"
 
+msgid "Toolbar"
+msgstr "工具列"
+
 msgid "Total"
 msgstr "合計"
 
 msgid "Transfer"
 msgstr "轉帳"
 
 msgid "Transfer Journal Entry#%(id)s"
@@ -670,17 +722,29 @@
 
 msgid "Trial Balance"
 msgstr "試算表"
 
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
+msgid "Unapplied Original Line Items"
+msgstr "未抵銷原始分錄"
+
+msgid "Unapplied Original Line Items of %(account)s"
+msgstr "%(account)s未抵銷原始分錄"
+
 msgid "Unmatched"
 msgstr "未抵銷"
 
+msgid "Unmatched Offsets"
+msgstr "遺漏的抵銷分錄"
+
+msgid "Unmatched Offsets in %(account)s"
+msgstr "%(account)s遺漏的抵銷分錄"
+
 msgid "Updated"
 msgstr "更新"
 
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水費{last_bimonthly_number}月"
 
 msgid "Year"
```

### Comparing `mia-accounting-1.0.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.1.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.0.0\n"
+"Project-Id-Version: mia-accounting 1.1.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-06 02:34+0800\n"
-"PO-Revision-Date: 2023-04-06 02:34+0800\n"
+"POT-Creation-Date: 2023-04-09 00:22+0800\n"
+"PO-Revision-Date: 2023-04-09 00:37+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -31,30 +31,30 @@
 msgid "The currency does not exist."
 msgstr "沒有這個貨幣。"
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr "沒有這個科目。"
 
-#: src/accounting/models.py:562
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr "現金支出傳票#%(id)s"
 
-#: src/accounting/models.py:565
+#: src/accounting/models.py:584
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr "現金收入傳票#%(id)s"
 
-#: src/accounting/models.py:566
+#: src/accounting/models.py:585
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "轉帳傳票#%(id)s"
 
-#: src/accounting/models.py:699
+#: src/accounting/models.py:714
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -201,32 +201,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr "傳票不可刪除。"
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr "傳票刪掉了"
 
-#: src/accounting/journal_entry/forms/currency.py:40
+#: src/accounting/journal_entry/forms/currency.py:39
 msgid "Please select the currency."
 msgstr "請選擇貨幣。"
 
-#: src/accounting/journal_entry/forms/currency.py:63
+#: src/accounting/journal_entry/forms/currency.py:62
 msgid "The currency must be the same as the original line item."
 msgstr "貨幣需和原始分錄相同。"
 
-#: src/accounting/journal_entry/forms/currency.py:90
+#: src/accounting/journal_entry/forms/currency.py:89
 msgid "The currency must not be changed when there is offset."
 msgstr "抵銷過不可變更貨幣。"
 
-#: src/accounting/journal_entry/forms/currency.py:99
+#: src/accounting/journal_entry/forms/currency.py:98
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr "請加上分錄。"
 
-#: src/accounting/journal_entry/forms/currency.py:112
+#: src/accounting/journal_entry/forms/currency.py:111
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方貸方合計不符。 "
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -267,50 +267,50 @@
 msgid "The original line item cannot be an offset item."
 msgstr "原始分錄不可以是抵銷分錄。"
 
 #: src/accounting/journal_entry/forms/line_item.py:119
 msgid "The account must be the same as the original line item."
 msgstr "科目需和原始分錄相同。"
 
-#: src/accounting/journal_entry/forms/line_item.py:137
+#: src/accounting/journal_entry/forms/line_item.py:135
 msgid "The account must not be changed when there is offset."
 msgstr "抵銷過不可變更科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:153
+#: src/accounting/journal_entry/forms/line_item.py:151
 msgid "A payable line item cannot start from debit."
 msgstr "不可由借方新建應付款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:169
+#: src/accounting/journal_entry/forms/line_item.py:167
 msgid "A receivable line item cannot start from credit."
 msgstr "不可由貸方新建應收款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:180
+#: src/accounting/journal_entry/forms/line_item.py:178
 #: src/accounting/static/js/journal-entry-line-item-editor.js:436
 msgid "Please fill in a positive amount."
 msgstr "金額請填正數。"
 
-#: src/accounting/journal_entry/forms/line_item.py:222
+#: src/accounting/journal_entry/forms/line_item.py:220
 #: src/accounting/static/js/journal-entry-line-item-editor.js:442
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr "金額不可超過原始分錄凈額 %(balance)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:243
+#: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金額不可低於抵銷總額 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:416
+#: src/accounting/journal_entry/forms/line_item.py:413
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:468
+#: src/accounting/journal_entry/forms/line_item.py:465
 msgid "This account is not for credit line items."
 msgstr "科目不是貸方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "這不是流動科目。"
 
@@ -438,47 +438,52 @@
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr "前期轉入"
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:50
 msgid "Date"
 msgstr "日期"
 
 #: src/accounting/report/reports/income_expenses.py:407
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unapplied_accounts.py:109
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:55
 msgid "Account"
 msgstr "科目"
 
 #: src/accounting/report/reports/income_expenses.py:408
-#: src/accounting/report/reports/journal.py:156
+#: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
+#: src/accounting/templates/accounting/report/unapplied.html:52
 msgid "Description"
 msgstr "摘要"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
@@ -492,15 +497,15 @@
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 msgid "Balance"
 msgstr "餘額"
 
 #: src/accounting/report/reports/income_expenses.py:410
-#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr "備註"
 
 #: src/accounting/report/reports/income_statement.py:228
@@ -524,52 +529,72 @@
 msgstr "稅後淨利"
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr "本期損益"
 
 #: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/unapplied.py:138
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/income-statement.html:55
+#: src/accounting/templates/accounting/report/unapplied.html:53
 msgid "Amount"
 msgstr "金額"
 
-#: src/accounting/report/reports/journal.py:155
+#: src/accounting/report/reports/journal.py:158
+#: src/accounting/report/reports/unapplied.py:137
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
+#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr "貨幣"
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:56
 msgid "Debit"
 msgstr "借方"
 
-#: src/accounting/report/reports/journal.py:157
+#: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
 #: src/accounting/templates/accounting/report/trial-balance.html:57
 msgid "Credit"
 msgstr "貸方"
 
-#: src/accounting/report/utils/report_chooser.py:81
+#: src/accounting/report/reports/unapplied.py:121
+#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/templates/accounting/include/nav.html:39
+msgid "Accounts"
+msgstr "科目"
+
+#: src/accounting/report/reports/unapplied.py:139
+#: src/accounting/templates/accounting/report/unapplied.html:54
+msgid "Net Balance"
+msgstr "淨額"
+
+#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+msgid "Count"
+msgstr "數量"
+
+#: src/accounting/report/utils/report_chooser.py:82
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -577,38 +602,43 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr "搜尋"
 
-#: src/accounting/report/utils/report_chooser.py:92
+#: src/accounting/report/utils/report_chooser.py:93
 msgid "Income and Expenses Log"
 msgstr "收支帳"
 
-#: src/accounting/report/utils/report_chooser.py:105
+#: src/accounting/report/utils/report_chooser.py:106
 msgid "Ledger"
 msgstr "分類帳"
 
-#: src/accounting/report/utils/report_chooser.py:117
+#: src/accounting/report/utils/report_chooser.py:118
 msgid "Journal"
 msgstr "日記簿"
 
-#: src/accounting/report/utils/report_chooser.py:127
+#: src/accounting/report/utils/report_chooser.py:128
 msgid "Trial Balance"
 msgstr "試算表"
 
-#: src/accounting/report/utils/report_chooser.py:138
+#: src/accounting/report/utils/report_chooser.py:139
 msgid "Income Statement"
 msgstr "損益表"
 
-#: src/accounting/report/utils/report_chooser.py:149
+#: src/accounting/report/utils/report_chooser.py:150
 msgid "Balance Sheet"
 msgstr "資產負債表"
 
+#: src/accounting/report/utils/report_chooser.py:163
+#: src/accounting/report/utils/report_chooser.py:167
+msgid "Unapplied Original Line Items"
+msgstr "未抵銷原始分錄"
+
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr "請填上標題。"
 
 #: src/accounting/static/js/description-editor.js:951
 #: src/accounting/static/js/description-editor.js:1129
 msgid "Please fill in the tag."
@@ -722,14 +752,15 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr "回上頁"
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -762,14 +793,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
+#: src/accounting/templates/accounting/unmatched-offset/list.html:54
 msgid "Close"
 msgstr "關閉"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你確定要刪掉這個科目嗎？"
 
@@ -779,21 +811,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:70
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
+#: src/accounting/templates/accounting/unmatched-offset/list.html:71
 msgid "Confirm"
 msgstr "確定"
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -845,14 +879,18 @@
 #: src/accounting/templates/accounting/report/balance-sheet.html:110
 #: src/accounting/templates/accounting/report/income-expenses.html:113
 #: src/accounting/templates/accounting/report/income-statement.html:96
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
 #: src/accounting/templates/accounting/report/trial-balance.html:82
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:98
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
+#: src/accounting/templates/accounting/unmatched-offset/list.html:104
 msgid "There is no data."
 msgstr "沒有資料。"
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
@@ -934,27 +972,28 @@
 msgid "Accounting"
 msgstr "記帳"
 
 #: src/accounting/templates/accounting/include/nav.html:33
 msgid "Reports"
 msgstr "報表"
 
-#: src/accounting/templates/accounting/include/nav.html:39
-msgid "Accounts"
-msgstr "科目"
-
 #: src/accounting/templates/accounting/include/nav.html:45
 msgid "Base Accounts"
 msgstr "基本科目"
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr "貨幣"
 
-#: src/accounting/templates/accounting/include/nav.html:58
+#: src/accounting/templates/accounting/include/nav.html:57
+#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
+msgid "Unmatched Offsets"
+msgstr "遺漏的抵銷分錄"
+
+#: src/accounting/templates/accounting/include/nav.html:64
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr "設定"
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1206,14 +1245,29 @@
 
 #: src/accounting/templates/accounting/report/trial-balance.html:29
 #: src/accounting/templates/accounting/report/trial-balance.html:49
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:41x
+msgid "Accounts with Unapplied Original Line Items"
+msgstr "有未抵銷原始分錄的科目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:28
+#, python-format
+msgid "Unapplied Original Line Items of %(account)s"
+msgstr "%(account)s未抵銷原始分錄"
+
+#: src/accounting/templates/accounting/report/unapplied.html:65
+#, python-format
+msgid "Can match %(offset)s"
+msgstr "可抵銷 %(offset)s"
+
 #: src/accounting/templates/accounting/report/include/period-chooser.html:26
 msgid "Period Chooser"
 msgstr "選擇日期範圍"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:34
 msgid "Month"
 msgstr "月"
@@ -1239,14 +1293,74 @@
 msgstr "期間"
 
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
 msgid "Download"
 msgstr "下載"
 
+#: src/accounting/templates/accounting/unmatched-offset/list.html:24
+#, python-format
+msgid "Unmatched Offsets in %(account)s"
+msgstr "%(account)s遺漏的抵銷分錄"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:28
+msgid "Toolbar"
+msgstr "工具列"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:36
+#: src/accounting/templates/accounting/unmatched-offset/list.html:41
+msgid "Match"
+msgstr "抵銷"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:53
+msgid "Confirm Match Offsets"
+msgstr "確認抵銷"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:57
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr "你確定要抵銷下列原始分錄與抵銷分錄嗎？結果無法復原。請先備份資料庫，並仔細核對抵銷分錄是否正確。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:81
+#, python-format
+msgid ""
+"%(matches)s unapplied original line items out of %(total)s can match with"
+" their offsets."
+msgstr ""
+"%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:83
+#, python-format
+msgid "%(total)s unapplied original line items without matching offsets."
+msgstr "%(total)s 筆未抵銷原始分錄，無法自動配對抵銷。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:85
+msgid "Go to unapplied original line items."
+msgstr "查閱未抵銷原始分錄。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:87
+msgid "All original line items are fully offset."
+msgstr "原始分錄已全部抵銷。"
+
+#: src/accounting/templates/accounting/unmatched-offset/list.html:98
+#, python-format
+msgid "Can match %(item)s"
+msgstr "可抵銷 %(item)s"
+
+#: src/accounting/unmatched_offset/views.py:71
+msgid "No more offset to match automatically."
+msgstr "無法自動配對抵銷。"
+
+#: src/accounting/unmatched_offset/views.py:77
+#, python-format
+msgid "Matches %(matches)s from %(total)s unapplied line items."
+msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches) 筆。"
+
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流動資產與負債"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
 msgid "Previous"
```

### Comparing `mia-accounting-1.0.1/src/accounting/utils/__init__.py` & `mia-accounting-1.1.0/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/cast.py` & `mia-accounting-1.1.0/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/current_account.py` & `mia-accounting-1.1.0/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/flash_errors.py` & `mia-accounting-1.1.0/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.1.0/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/next_uri.py` & `mia-accounting-1.1.0/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/options.py` & `mia-accounting-1.1.0/src/accounting/utils/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,20 +95,20 @@
 
         :param value: The default currency code.
         :return: None.
         """
         self.__set_option("default_currency_code", value)
 
     @property
-    def default_currency_text(self) -> str:
-        """Returns the text of the default currency code.
+    def default_currency(self) -> Currency:
+        """Returns the default currency.
 
-        :return: The text of the default currency code.
+        :return: The default currency.
         """
-        return str(db.session.get(Currency, self.default_currency_code))
+        return db.session.get(Currency, self.default_currency_code)
 
     @property
     def default_ie_account_code(self) -> str:
         """Returns the default account code for the income and expenses log.
 
         :return: The default account code for the income and expenses log.
         """
@@ -120,29 +120,18 @@
 
         :param value: The default account code for the income and expenses log.
         :return: None.
         """
         self.__set_option("default_ie_account", value)
 
     @property
-    def default_ie_account_code_text(self) -> str:
-        """Returns the text of the default currency code.
-
-        :return: The text of the default currency code.
-        """
-        code: str = self.default_ie_account_code
-        if code == CurrentAccount.CURRENT_AL_CODE:
-            return str(CurrentAccount.current_assets_and_liabilities())
-        return str(CurrentAccount(Account.find_by_code(code)))
-
-    @property
     def default_ie_account(self) -> CurrentAccount:
-        """Returns the default account code for the income and expenses log.
+        """Returns the default account for the income and expenses log.
 
-        :return: The default account code for the income and expenses log.
+        :return: The default account for the income and expenses log.
         """
         if self.default_ie_account_code \
                 == CurrentAccount.CURRENT_AL_CODE:
             return CurrentAccount.current_assets_and_liabilities()
         return CurrentAccount(
             Account.find_by_code(self.default_ie_account_code))
```

### Comparing `mia-accounting-1.0.1/src/accounting/utils/pagination.py` & `mia-accounting-1.1.0/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/permission.py` & `mia-accounting-1.1.0/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/query.py` & `mia-accounting-1.1.0/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/random_id.py` & `mia-accounting-1.1.0/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/strip_text.py` & `mia-accounting-1.1.0/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/accounting/utils/user.py` & `mia-accounting-1.1.0/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.1.0/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
@@ -33,30 +33,40 @@
 * Trial balance
 * Income statement
 * Balance sheet
 
 In addition, *Mia! Accounting* tracks offsets for unpaid payables and
 receivables.
 
-You may try the `live demonstration`_.
-
 
 Installation
 ============
 
 Install *Mia! Accounting* with ``pip``:
 
 ::
 
     pip install mia-accounting
 
 You may also download the from the `PyPI project page`_ or the
 `release page`_ on the `Git repository`_.
 
 
+Test Site and Live Demonstration
+================================
+
+You may find a working example in the `test site`_ in the
+`source distribution`_.  It is the simplest website that works with
+*Mia! Accounting*.  It is used in the automatic tests.  It is the same
+code run for `live demonstration`_.
+
+If you do not have a running Flask application or do not know how to
+start one, you may start with the test site.
+
+
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
 The primary key of the user data model must be integer.
 
 The following front-end JavaScript libraries must be loaded.  You may
@@ -173,26 +183,14 @@
         </div>
       </div>
     </nav>
 
 Check your Flask application and see how it works.
 
 
-Test Site and Live Demonstration
-================================
-
-You may find a working example in the `test site`_ in the
-`source distribution`_.  It is the simplest website that works with
-*Mia! Accounting*.  It is used in the automatic tests.  It is the same
-code run for `live demonstration`_.
-
-If you do not have a running Flask application, you may start with the
-test site.
-
-
 Documentation
 =============
 
 Refer to the `documentation on Read the Docs`_.
 
 
 Copyright
@@ -219,23 +217,23 @@
 | imacat
 | imacat@mail.imacat.idv.tw
 | 2023/1/27
 
 
 .. _Flask: https://flask.palletsprojects.com
 .. _double-entry bookkeeping: https://en.wikipedia.org/wiki/Double-entry_bookkeeping
+.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
+.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _live demonstration: https://accounting.imacat.idv.tw
 .. _PyPI project page: https://pypi.org/project/mia-accounting
 .. _release page: https://github.com/imacat/mia-accounting/releases
 .. _Git repository: https://github.com/imacat/mia-accounting
 .. _CDN: https://en.wikipedia.org/wiki/Content_delivery_network
 .. _Bootstrap: https://getbootstrap.com
 .. _FontAwesome: https://fontawesome.com
 .. _Decimal.js: https://mikemcl.github.io/decimal.js
 .. _Tempus-Dominus: https://getdatepicker.com
 .. _UserUtilityInterface: https://mia-accounting.readthedocs.io/en/latest/accounting.utils.html#accounting.utils.user.UserUtilityInterface
 .. _init_app: https://mia-accounting.readthedocs.io/en/latest/accounting.html#accounting.init_app
 .. _flask_sqlalchemy.SQLAlchemy.create_all: https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/api/#flask_sqlalchemy.SQLAlchemy.create_all
 .. _Bootstrap navigation bar: https://getbootstrap.com/docs/5.3/components/navbar/
-.. _test site: https://github.com/imacat/mia-accounting/tree/main/tests/test_site
-.. _source distribution: https://pypi.org/project/mia-accounting/#files
 .. _documentation on Read the Docs: https://mia-accounting.readthedocs.io
```

### Comparing `mia-accounting-1.0.1/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.1.0/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/source/accounting.journal_entry.utils.rst
 docs/source/accounting.option.rst
 docs/source/accounting.report.period.rst
 docs/source/accounting.report.reports.rst
 docs/source/accounting.report.rst
 docs/source/accounting.report.utils.rst
 docs/source/accounting.rst
+docs/source/accounting.unmatched_offset.rst
 docs/source/accounting.utils.rst
 docs/source/conf.py
 docs/source/examples.rst
 docs/source/history.rst
 docs/source/index.rst
 docs/source/intro.rst
 docs/source/modules.rst
@@ -58,15 +59,14 @@
 src/accounting/journal_entry/forms/currency.py
 src/accounting/journal_entry/forms/journal_entry.py
 src/accounting/journal_entry/forms/line_item.py
 src/accounting/journal_entry/forms/reorder.py
 src/accounting/journal_entry/utils/__init__.py
 src/accounting/journal_entry/utils/account_option.py
 src/accounting/journal_entry/utils/description_editor.py
-src/accounting/journal_entry/utils/offset_alias.py
 src/accounting/journal_entry/utils/operators.py
 src/accounting/journal_entry/utils/original_line_items.py
 src/accounting/option/__init__.py
 src/accounting/option/forms.py
 src/accounting/option/views.py
 src/accounting/report/__init__.py
 src/accounting/report/converters.py
@@ -84,21 +84,24 @@
 src/accounting/report/reports/balance_sheet.py
 src/accounting/report/reports/income_expenses.py
 src/accounting/report/reports/income_statement.py
 src/accounting/report/reports/journal.py
 src/accounting/report/reports/ledger.py
 src/accounting/report/reports/search.py
 src/accounting/report/reports/trial_balance.py
+src/accounting/report/reports/unapplied.py
+src/accounting/report/reports/unapplied_accounts.py
 src/accounting/report/utils/__init__.py
 src/accounting/report/utils/base_page_params.py
 src/accounting/report/utils/base_report.py
 src/accounting/report/utils/csv_export.py
 src/accounting/report/utils/option_link.py
 src/accounting/report/utils/report_chooser.py
 src/accounting/report/utils/report_type.py
+src/accounting/report/utils/unapplied.py
 src/accounting/report/utils/urls.py
 src/accounting/static/css/style.css
 src/accounting/static/js/account-form.js
 src/accounting/static/js/account-order.js
 src/accounting/static/js/currency-form.js
 src/accounting/static/js/description-editor.js
 src/accounting/static/js/drag-and-drop-reorder.js
@@ -162,55 +165,66 @@
 src/accounting/templates/accounting/report/balance-sheet.html
 src/accounting/templates/accounting/report/income-expenses.html
 src/accounting/templates/accounting/report/income-statement.html
 src/accounting/templates/accounting/report/journal.html
 src/accounting/templates/accounting/report/ledger.html
 src/accounting/templates/accounting/report/search.html
 src/accounting/templates/accounting/report/trial-balance.html
+src/accounting/templates/accounting/report/unapplied-accounts.html
+src/accounting/templates/accounting/report/unapplied.html
 src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
 src/accounting/templates/accounting/report/include/balance-sheet-section.html
 src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
 src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
 src/accounting/templates/accounting/report/include/ledger-row-desktop.html
 src/accounting/templates/accounting/report/include/ledger-row-mobile.html
 src/accounting/templates/accounting/report/include/period-chooser.html
 src/accounting/templates/accounting/report/include/search-modal.html
 src/accounting/templates/accounting/report/include/toolbar-buttons.html
+src/accounting/templates/accounting/unmatched-offset/dashboard.html
+src/accounting/templates/accounting/unmatched-offset/list.html
 src/accounting/translations/accounting.pot
 src/accounting/translations/babel.cfg
 src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
 src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
 src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
 src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+src/accounting/unmatched_offset/__init__.py
+src/accounting/unmatched_offset/queries.py
+src/accounting/unmatched_offset/views.py
 src/accounting/utils/__init__.py
 src/accounting/utils/cast.py
 src/accounting/utils/current_account.py
 src/accounting/utils/flash_errors.py
 src/accounting/utils/journal_entry_types.py
 src/accounting/utils/next_uri.py
+src/accounting/utils/offset_alias.py
+src/accounting/utils/offset_matcher.py
 src/accounting/utils/options.py
 src/accounting/utils/pagination.py
 src/accounting/utils/permission.py
 src/accounting/utils/query.py
 src/accounting/utils/random_id.py
 src/accounting/utils/strip_text.py
+src/accounting/utils/unapplied.py
 src/accounting/utils/user.py
 src/mia_accounting.egg-info/PKG-INFO
 src/mia_accounting.egg-info/SOURCES.txt
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
 tests/babel-utils.py
 tests/test_account.py
 tests/test_base_account.py
 tests/test_currency.py
 tests/test_description_editor.py
 tests/test_journal_entry.py
 tests/test_offset.py
+tests/test_offset_matcher.py
 tests/test_option.py
 tests/test_utils.py
 tests/testlib.py
 tests/testlib_journal_entry.py
 tests/testlib_offset.py
 tests/test_site/__init__.py
 tests/test_site/auth.py
```

### Comparing `mia-accounting-1.0.1/tests/babel-utils-test-site.py` & `mia-accounting-1.1.0/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/babel-utils.py` & `mia-accounting-1.1.0/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_account.py` & `mia-accounting-1.1.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_base_account.py` & `mia-accounting-1.1.0/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_currency.py` & `mia-accounting-1.1.0/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_description_editor.py` & `mia-accounting-1.1.0/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_journal_entry.py` & `mia-accounting-1.1.0/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_offset.py` & `mia-accounting-1.1.0/tests/test_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,42 +77,42 @@
         create_uri: str = f"{PREFIX}/create/receipt?next=%2F_next"
         store_uri: str = f"{PREFIX}/store/receipt"
         form: dict[str, str]
         old_amount: Decimal
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.e_r_or3d.journal_entry.days, [CurrencyData(
+            self.data.l_r_or3d.journal_entry.days, [CurrencyData(
                 "USD",
                 [],
                 [JournalEntryLineItemData(
                     Accounts.RECEIVABLE,
-                    self.data.e_r_or1d.description, "300",
-                    original_line_item=self.data.e_r_or1d),
+                    self.data.l_r_or1d.description, "300",
+                    original_line_item=self.data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
-                     self.data.e_r_or1d.description, "100",
-                     original_line_item=self.data.e_r_or1d),
+                     self.data.l_r_or1d.description, "100",
+                     original_line_item=self.data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
-                     self.data.e_r_or3d.description, "100",
-                     original_line_item=self.data.e_r_or3d)])])
+                     self.data.l_r_or3d.description, "100",
+                     original_line_item=self.data.l_r_or3d)])])
 
         # Non-existing original line item ID
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.e_p_or1c.id
-        form["currency-1-credit-1-account_code"] = self.data.e_p_or1c.account
+            = self.data.l_p_or1c.id
+        form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
         with self.app.app_context():
@@ -127,16 +127,16 @@
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.e_p_of1d.id
-        form["currency-1-credit-1-account_code"] = self.data.e_p_of1d.account
+            = self.data.l_p_of1d.id
+        form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-code"] = "EUR"
@@ -191,21 +191,21 @@
 
     def test_edit_receivable_offset(self) -> None:
         """Tests to edit the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account
-        journal_entry_data: JournalEntryData = self.data.v_r_of2
+        journal_entry_data: JournalEntryData = self.data.j_r_of2
         edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.v_r_or2.days
+        journal_entry_data.days = self.data.j_r_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("600")
 
         # Non-existing original line item ID
         form = journal_entry_data.update_form(self.csrf_token)
@@ -213,16 +213,16 @@
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.e_p_or1c.id
-        form["currency-1-credit-1-account_code"] = self.data.e_p_or1c.account
+            = self.data.l_p_or1c.id
+        form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The original line item does not need offset
@@ -238,16 +238,16 @@
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-credit-1-original_line_item_id"] \
-            = self.data.e_p_of1d.id
-        form["currency-1-credit-1-account_code"] = self.data.e_p_of1d.account
+            = self.data.l_p_of1d.id
+        form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-code"] = "EUR"
@@ -304,21 +304,21 @@
 
     def test_edit_receivable_original_line_item(self) -> None:
         """Tests to edit the receivable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
-        journal_entry_data: JournalEntryData = self.data.v_r_or1
+        journal_entry_data: JournalEntryData = self.data.j_r_or1
         edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.v_r_of1.days
+        journal_entry_data.days = self.data.j_r_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("3.4")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("3.4")
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
@@ -384,15 +384,15 @@
         # The original line item is always before the offset item, even when
         # they happen in the same day.
         with self.app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
             journal_entry_of: JournalEntry | None = db.session.get(
-                JournalEntry, self.data.v_r_of1.id)
+                JournalEntry, self.data.j_r_of1.id)
             self.assertIsNotNone(journal_entry_of)
             self.assertEqual(journal_entry_or.date, journal_entry_of.date)
             self.assertLess(journal_entry_or.no, journal_entry_of.no)
 
     def test_add_payable_offset(self) -> None:
         """Tests to add the payable offset.
 
@@ -401,42 +401,42 @@
         from accounting.models import Account, JournalEntry
         create_uri: str = f"{PREFIX}/create/disbursement?next=%2F_next"
         store_uri: str = f"{PREFIX}/store/disbursement"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.e_p_or3c.journal_entry.days, [CurrencyData(
+            self.data.l_p_or3c.journal_entry.days, [CurrencyData(
                 "USD",
                 [JournalEntryLineItemData(
                     Accounts.PAYABLE,
-                    self.data.e_p_or1c.description, "500",
-                    original_line_item=self.data.e_p_or1c),
+                    self.data.l_p_or1c.description, "500",
+                    original_line_item=self.data.l_p_or1c),
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
-                     self.data.e_p_or1c.description, "300",
-                     original_line_item=self.data.e_p_or1c),
+                     self.data.l_p_or1c.description, "300",
+                     original_line_item=self.data.l_p_or1c),
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
-                     self.data.e_p_or3c.description, "120",
-                     original_line_item=self.data.e_p_or3c)],
+                     self.data.l_p_or3c.description, "120",
+                     original_line_item=self.data.l_p_or3c)],
                 [])])
 
         # Non-existing original line item ID
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.e_r_or1d.id
-        form["currency-1-debit-1-account_code"] = self.data.e_r_or1d.account
+            = self.data.l_r_or1d.id
+        form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
         with self.app.app_context():
@@ -451,16 +451,16 @@
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.e_r_of1c.id
-        form["currency-1-debit-1-account_code"] = self.data.e_r_of1c.account
+            = self.data.l_r_of1c.id
+        form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
         form = journal_entry_data.new_form(self.csrf_token)
         form["currency-1-code"] = "EUR"
@@ -515,21 +515,21 @@
 
     def test_edit_payable_offset(self) -> None:
         """Tests to edit the payable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
-        journal_entry_data: JournalEntryData = self.data.v_p_of2
+        journal_entry_data: JournalEntryData = self.data.j_p_of2
         edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.v_p_or2.days
+        journal_entry_data.days = self.data.j_p_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("900")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("900")
 
         # Non-existing original line item ID
         form = journal_entry_data.update_form(self.csrf_token)
@@ -537,16 +537,16 @@
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.e_r_or1d.id
-        form["currency-1-debit-1-account_code"] = self.data.e_r_or1d.account
+            = self.data.l_r_or1d.id
+        form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The original line item does not need offset
@@ -562,16 +562,16 @@
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-debit-1-original_line_item_id"] \
-            = self.data.e_r_of1c.id
-        form["currency-1-debit-1-account_code"] = self.data.e_r_of1c.account
+            = self.data.l_r_of1c.id
+        form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
         form["currency-1-code"] = "EUR"
@@ -632,21 +632,21 @@
 
     def test_edit_payable_original_line_item(self) -> None:
         """Tests to edit the payable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
-        journal_entry_data: JournalEntryData = self.data.v_p_or1
+        journal_entry_data: JournalEntryData = self.data.j_p_or1
         edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.v_p_of1.days
+        journal_entry_data.days = self.data.j_p_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("0.9")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("0.9")
 
         # Not the same currency
         form = journal_entry_data.update_form(self.csrf_token)
@@ -712,11 +712,11 @@
         # The original line item is always before the offset item, even when
         # they happen in the same day
         with self.app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
             journal_entry_of: JournalEntry | None = db.session.get(
-                JournalEntry, self.data.v_p_of1.id)
+                JournalEntry, self.data.j_p_of1.id)
             self.assertIsNotNone(journal_entry_of)
             self.assertEqual(journal_entry_or.date, journal_entry_of.date)
             self.assertLess(journal_entry_or.no, journal_entry_of.no)
```

### Comparing `mia-accounting-1.0.1/tests/test_option.py` & `mia-accounting-1.1.0/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/__init__.py` & `mia-accounting-1.1.0/tests/test_site/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/auth.py` & `mia-accounting-1.1.0/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/locale.py` & `mia-accounting-1.1.0/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/static/favicon.svg` & `mia-accounting-1.1.0/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/templates/base.html` & `mia-accounting-1.1.0/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/templates/home.html` & `mia-accounting-1.1.0/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/templates/login.html` & `mia-accounting-1.1.0/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/translations/messages.pot` & `mia-accounting-1.1.0/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.1.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.1.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/test_utils.py` & `mia-accounting-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/testlib.py` & `mia-accounting-1.1.0/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/testlib_journal_entry.py` & `mia-accounting-1.1.0/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.0.1/tests/testlib_offset.py` & `mia-accounting-1.1.0/tests/testlib_offset.py`

 * *Files 20% similar despite different names*

```diff
@@ -185,110 +185,110 @@
             :param credit: The credit account code.
             :return: The debit line item and credit line item.
             """
             return JournalEntryLineItemData(debit, description, amount),\
                 JournalEntryLineItemData(credit, description, amount)
 
         # Receivable original line items
-        self.e_r_or1d, self.e_r_or1c = couple(
+        self.l_r_or1d, self.l_r_or1c = couple(
             "Accountant", "1200", Accounts.RECEIVABLE, Accounts.SERVICE)
-        self.e_r_or2d, self.e_r_or2c = couple(
+        self.l_r_or2d, self.l_r_or2c = couple(
             "Toy", "600", Accounts.RECEIVABLE, Accounts.SALES)
-        self.e_r_or3d, self.e_r_or3c = couple(
+        self.l_r_or3d, self.l_r_or3c = couple(
             "Noodles", "100", Accounts.RECEIVABLE, Accounts.SALES)
-        self.e_r_or4d, self.e_r_or4c = couple(
+        self.l_r_or4d, self.l_r_or4c = couple(
             "Interest", "3.4", Accounts.RECEIVABLE, Accounts.INTEREST)
 
         # Payable original line items
-        self.e_p_or1d, self.e_p_or1c = couple(
+        self.l_p_or1d, self.l_p_or1c = couple(
             "Airplane", "2000", Accounts.TRAVEL, Accounts.PAYABLE)
-        self.e_p_or2d, self.e_p_or2c = couple(
+        self.l_p_or2d, self.l_p_or2c = couple(
             "Phone", "900", Accounts.OFFICE, Accounts.PAYABLE)
-        self.e_p_or3d, self.e_p_or3c = couple(
+        self.l_p_or3d, self.l_p_or3c = couple(
             "Steak", "120", Accounts.MEAL, Accounts.PAYABLE)
-        self.e_p_or4d, self.e_p_or4c = couple(
+        self.l_p_or4d, self.l_p_or4c = couple(
             "Envelop", "0.9", Accounts.OFFICE, Accounts.PAYABLE)
 
         # Original journal entries
-        self.v_r_or1: JournalEntryData = JournalEntryData(
-            50, [CurrencyData("USD", [self.e_r_or1d, self.e_r_or4d],
-                              [self.e_r_or1c, self.e_r_or4c])])
-        self.v_r_or2: JournalEntryData = JournalEntryData(
-            30, [CurrencyData("USD", [self.e_r_or2d, self.e_r_or3d],
-                              [self.e_r_or2c, self.e_r_or3c])])
-        self.v_p_or1: JournalEntryData = JournalEntryData(
-            40, [CurrencyData("USD", [self.e_p_or1d, self.e_p_or4d],
-                              [self.e_p_or1c, self.e_p_or4c])])
-        self.v_p_or2: JournalEntryData = JournalEntryData(
-            20, [CurrencyData("USD", [self.e_p_or2d, self.e_p_or3d],
-                              [self.e_p_or2c, self.e_p_or3c])])
-
-        self.__add_journal_entry(self.v_r_or1)
-        self.__add_journal_entry(self.v_r_or2)
-        self.__add_journal_entry(self.v_p_or1)
-        self.__add_journal_entry(self.v_p_or2)
+        self.j_r_or1: JournalEntryData = JournalEntryData(
+            50, [CurrencyData("USD", [self.l_r_or1d, self.l_r_or4d],
+                              [self.l_r_or1c, self.l_r_or4c])])
+        self.j_r_or2: JournalEntryData = JournalEntryData(
+            30, [CurrencyData("USD", [self.l_r_or2d, self.l_r_or3d],
+                              [self.l_r_or2c, self.l_r_or3c])])
+        self.j_p_or1: JournalEntryData = JournalEntryData(
+            40, [CurrencyData("USD", [self.l_p_or1d, self.l_p_or4d],
+                              [self.l_p_or1c, self.l_p_or4c])])
+        self.j_p_or2: JournalEntryData = JournalEntryData(
+            20, [CurrencyData("USD", [self.l_p_or2d, self.l_p_or3d],
+                              [self.l_p_or2c, self.l_p_or3c])])
+
+        self.__add_journal_entry(self.j_r_or1)
+        self.__add_journal_entry(self.j_r_or2)
+        self.__add_journal_entry(self.j_p_or1)
+        self.__add_journal_entry(self.j_p_or2)
 
         # Receivable offset items
-        self.e_r_of1d, self.e_r_of1c = couple(
+        self.l_r_of1d, self.l_r_of1c = couple(
             "Accountant", "500", Accounts.CASH, Accounts.RECEIVABLE)
-        self.e_r_of1c.original_line_item = self.e_r_or1d
-        self.e_r_of2d, self.e_r_of2c = couple(
+        self.l_r_of1c.original_line_item = self.l_r_or1d
+        self.l_r_of2d, self.l_r_of2c = couple(
             "Accountant", "200", Accounts.CASH, Accounts.RECEIVABLE)
-        self.e_r_of2c.original_line_item = self.e_r_or1d
-        self.e_r_of3d, self.e_r_of3c = couple(
+        self.l_r_of2c.original_line_item = self.l_r_or1d
+        self.l_r_of3d, self.l_r_of3c = couple(
             "Accountant", "100", Accounts.CASH, Accounts.RECEIVABLE)
-        self.e_r_of3c.original_line_item = self.e_r_or1d
-        self.e_r_of4d, self.e_r_of4c = couple(
+        self.l_r_of3c.original_line_item = self.l_r_or1d
+        self.l_r_of4d, self.l_r_of4c = couple(
             "Toy", "240", Accounts.CASH, Accounts.RECEIVABLE)
-        self.e_r_of4c.original_line_item = self.e_r_or2d
-        self.e_r_of5d, self.e_r_of5c = couple(
+        self.l_r_of4c.original_line_item = self.l_r_or2d
+        self.l_r_of5d, self.l_r_of5c = couple(
             "Interest", "3.4", Accounts.CASH, Accounts.RECEIVABLE)
-        self.e_r_of5c.original_line_item = self.e_r_or4d
+        self.l_r_of5c.original_line_item = self.l_r_or4d
 
         # Payable offset items
-        self.e_p_of1d, self.e_p_of1c = couple(
+        self.l_p_of1d, self.l_p_of1c = couple(
             "Airplane", "800", Accounts.PAYABLE, Accounts.CASH)
-        self.e_p_of1d.original_line_item = self.e_p_or1c
-        self.e_p_of2d, self.e_p_of2c = couple(
+        self.l_p_of1d.original_line_item = self.l_p_or1c
+        self.l_p_of2d, self.l_p_of2c = couple(
             "Airplane", "300", Accounts.PAYABLE, Accounts.CASH)
-        self.e_p_of2d.original_line_item = self.e_p_or1c
-        self.e_p_of3d, self.e_p_of3c = couple(
+        self.l_p_of2d.original_line_item = self.l_p_or1c
+        self.l_p_of3d, self.l_p_of3c = couple(
             "Airplane", "100", Accounts.PAYABLE, Accounts.CASH)
-        self.e_p_of3d.original_line_item = self.e_p_or1c
-        self.e_p_of4d, self.e_p_of4c = couple(
+        self.l_p_of3d.original_line_item = self.l_p_or1c
+        self.l_p_of4d, self.l_p_of4c = couple(
             "Phone", "400", Accounts.PAYABLE, Accounts.CASH)
-        self.e_p_of4d.original_line_item = self.e_p_or2c
-        self.e_p_of5d, self.e_p_of5c = couple(
+        self.l_p_of4d.original_line_item = self.l_p_or2c
+        self.l_p_of5d, self.l_p_of5c = couple(
             "Envelop", "0.9", Accounts.PAYABLE, Accounts.CASH)
-        self.e_p_of5d.original_line_item = self.e_p_or4c
+        self.l_p_of5d.original_line_item = self.l_p_or4c
 
         # Offset journal entries
-        self.v_r_of1: JournalEntryData = JournalEntryData(
-            25, [CurrencyData("USD", [self.e_r_of1d], [self.e_r_of1c])])
-        self.v_r_of2: JournalEntryData = JournalEntryData(
+        self.j_r_of1: JournalEntryData = JournalEntryData(
+            25, [CurrencyData("USD", [self.l_r_of1d], [self.l_r_of1c])])
+        self.j_r_of2: JournalEntryData = JournalEntryData(
             20, [CurrencyData("USD",
-                              [self.e_r_of2d, self.e_r_of3d, self.e_r_of4d],
-                              [self.e_r_of2c, self.e_r_of3c, self.e_r_of4c])])
-        self.v_r_of3: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.e_r_of5d], [self.e_r_of5c])])
-        self.v_p_of1: JournalEntryData = JournalEntryData(
-            15, [CurrencyData("USD", [self.e_p_of1d], [self.e_p_of1c])])
-        self.v_p_of2: JournalEntryData = JournalEntryData(
+                              [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
+                              [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
+        self.j_r_of3: JournalEntryData = JournalEntryData(
+            15, [CurrencyData("USD", [self.l_r_of5d], [self.l_r_of5c])])
+        self.j_p_of1: JournalEntryData = JournalEntryData(
+            15, [CurrencyData("USD", [self.l_p_of1d], [self.l_p_of1c])])
+        self.j_p_of2: JournalEntryData = JournalEntryData(
             10, [CurrencyData("USD",
-                              [self.e_p_of2d, self.e_p_of3d, self.e_p_of4d],
-                              [self.e_p_of2c, self.e_p_of3c, self.e_p_of4c])])
-        self.v_p_of3: JournalEntryData = JournalEntryData(
-            5, [CurrencyData("USD", [self.e_p_of5d], [self.e_p_of5c])])
-
-        self.__add_journal_entry(self.v_r_of1)
-        self.__add_journal_entry(self.v_r_of2)
-        self.__add_journal_entry(self.v_r_of3)
-        self.__add_journal_entry(self.v_p_of1)
-        self.__add_journal_entry(self.v_p_of2)
-        self.__add_journal_entry(self.v_p_of3)
+                              [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
+                              [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
+        self.j_p_of3: JournalEntryData = JournalEntryData(
+            5, [CurrencyData("USD", [self.l_p_of5d], [self.l_p_of5c])])
+
+        self.__add_journal_entry(self.j_r_of1)
+        self.__add_journal_entry(self.j_r_of2)
+        self.__add_journal_entry(self.j_r_of3)
+        self.__add_journal_entry(self.j_p_of1)
+        self.__add_journal_entry(self.j_p_of2)
+        self.__add_journal_entry(self.j_p_of3)
 
     def __add_journal_entry(self, journal_entry_data: JournalEntryData) \
             -> None:
         """Adds a journal entry.
 
         :param journal_entry_data: The journal entry data.
         :return: None.
```

