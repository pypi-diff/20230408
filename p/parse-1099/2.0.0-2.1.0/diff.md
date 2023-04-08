# Comparing `tmp/parse_1099-2.0.0.tar.gz` & `tmp/parse_1099-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_1099-2.0.0.tar", last modified: Sat Apr  8 06:27:27 2023, max compression
+gzip compressed data, was "parse_1099-2.1.0.tar", last modified: Sat Apr  8 16:30:00 2023, max compression
```

## Comparing `parse_1099-2.0.0.tar` & `parse_1099-2.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.578236 parse_1099-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-08 06:27:12.000000 parse_1099-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-08 06:27:12.000000 parse_1099-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-08 06:27:12.000000 parse_1099-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 06:27:27.578236 parse_1099-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-08 06:27:12.000000 parse_1099-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.574236 parse_1099-2.0.0/parse_1099/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.574236 parse_1099-2.0.0/parse_1099/dividends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/dividend_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/dividends_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/dividends_repository_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.578236 parse_1099-2.0.0/parse_1099/dividends/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/v1/dividends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/v1/dividends_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/v1/dividends_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/dividends/v1/dividends_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/pdf_contents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.578236 parse_1099-2.0.0/parse_1099/sales/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/sales_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.578236 parse_1099-2.0.0/parse_1099/sales/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/v1/sales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/v1/sales_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/sales/v1/sales_total.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/subparser_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.578236 parse_1099-2.0.0/parse_1099/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 06:27:12.000000 parse_1099-2.0.0/parse_1099/utilities/csv_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 06:27:27.574236 parse_1099-2.0.0/parse_1099.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 06:27:27.000000 parse_1099-2.0.0/parse_1099.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 06:27:12.000000 parse_1099-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 06:27:27.578236 parse_1099-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-08 06:27:12.000000 parse_1099-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-08 16:29:45.000000 parse_1099-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-08 16:29:45.000000 parse_1099-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-08 16:29:45.000000 parse_1099-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 16:30:00.007226 parse_1099-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-08 16:29:45.000000 parse_1099-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.003226 parse_1099-2.1.0/parse_1099/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/dividends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividend_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividends_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividends_repository_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/dividends/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/pdf_contents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/sales_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/sales/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/subparser_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/utilities/csv_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.003226 parse_1099-2.1.0/parse_1099.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 16:29:45.000000 parse_1099-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 16:30:00.007226 parse_1099-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-08 16:29:45.000000 parse_1099-2.1.0/setup.py
```

### Comparing `parse_1099-2.0.0/CHANGELOG.md` & `parse_1099-2.1.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-# v2.0.0
-## Added
+
+## [2.1.0] 2023-04-08
+### Changed
+- Added short-hand flags for the existing command line parameters.
+
+## [2.0.0] 2023-04-07
+### Added
 - Added search functionality for ex dividend dates.
 - Added parsing of dividends.
 - Added analysis of dividends and sales to determine whether qualified dividends need to be considered nonqualified.
 
-## Changed
+### Changed
 - Downgraded python version requirement to `>= 3.6` for ease of use on ubuntu.
 - Renamed tool to `parse_1099` to reflect that it's not specific to Robinhood.
 
-# v1.0.1
+## [1.0.1]
 - Updated README.md to utilize `pip install rh_1099`
 - Updated setup.py to bump Python version requirement to `>= 3.8`
 
-# v1.0.0
+## [1.0.0]
 - Initial release
```

### Comparing `parse_1099-2.0.0/LICENSE` & `parse_1099-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/PKG-INFO` & `parse_1099-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_1099
-Version: 2.0.0
+Version: 2.1.0
 Summary: Parses 1099 tax document (1099-B, 1099-INT, 1099-DIV) from PDF into CSV format and performs simple analysis
 Home-page: 
 Author: Andrew Wells, Keun Tae (Kevin) Park
 Author-email: ajwells@uchicago.com, kevin.park1217@gmail.com
 Project-URL: Bug Reports, https://github.com/ajwells256/1099-Parser/issues
 Project-URL: Source, https://github.com/ajwells256/1099-Parser
 Keywords: pdf,csv,parsing,excel,spreadsheet,tax,1099
```

### Comparing `parse_1099-2.0.0/README.md` & `parse_1099-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/dividends/dividend_analyzer.py` & `parse_1099-2.1.0/parse_1099/dividends/dividend_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,14 @@
                                           if sale.cusip == cusip and
                                           sale.acquired_date <= exdate and exdate <= sale.disposal_date]  # type:ignore since all fields should be populated
 
                     disqualified_sale_count = len(disqualified_sales)
                     if disqualified_sale_count != 0:
                         adjustment_occurred = True
 
-                        # todo - lookup dividend per share
                         amount_per_share = cusip_exdates[exdate.date()]
                         disqualified_dividend = working_dividend.disqualify(
                             disqualified_sale_count, amount_per_share)
                         adjusted_dividends.append(disqualified_dividend)
 
                         if self.report_prefix is not None:
                             for sale in disqualified_sales:
```

### Comparing `parse_1099-2.0.0/parse_1099/dividends/dividends_interface.py` & `parse_1099-2.1.0/parse_1099/dividends/dividends_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/dividends/v1/dividends.py` & `parse_1099-2.1.0/parse_1099/dividends/v1/dividends.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/dividends/v1/dividends_parser.py` & `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_parser.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/dividends/v1/dividends_repository.py` & `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_repository.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/dividends/v1/dividends_total.py` & `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_total.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/main.py` & `parse_1099-2.1.0/parse_1099/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         return arg
 
 
 def main():
     arg_parser = argparse.ArgumentParser(
         prog='parse_1099',
         description='1099 Tax Document Parser')
-    arg_parser.add_argument('--pdf', required=True, dest='pdf_path',
+    arg_parser.add_argument('-i', '--pdf', required=True, dest='pdf_path',
                         help='Input path to the 1099 PDF document', metavar="FILE",
                         type=lambda x: is_valid_file(arg_parser, x))
-    arg_parser.add_argument('--csv', metavar="PREFIX", help='Output path (and prefix) of the parsed CSVs. For example, ./directory/output will produce ./directory/output_sales.csv and ./directory/output_dividends.csv')
-    arg_parser.add_argument('--silent', action='store_true', help='Hide progress bar')
-    arg_parser.add_argument('--validate', action='store_true', help='Print total values for validation')
-    arg_parser.add_argument("--include-dividend-notes", action='store_true', help="Include the 'notes' column in the dividend output csv")
-    arg_parser.add_argument("--disable-dividend-analysis", action='store_true', help="Disable analysis of qualified dividend holding periods")
-    arg_parser.add_argument("--analysis-report", action='store_true', help="Produce a detailed report from the qualified dividends analysis.")
+    arg_parser.add_argument('-o', '--csv', metavar="PREFIX", help='Output path (and prefix) of the parsed CSVs. For example, ./directory/output will produce ./directory/output_sales.csv and ./directory/output_dividends.csv')
+    arg_parser.add_argument('-s', '--silent', action='store_true', help='Hide progress bar')
+    arg_parser.add_argument('-v', '--validate', action='store_true', help='Print total values for validation')
+    arg_parser.add_argument('-n', "--include-dividend-notes", action='store_true', help="Include the 'notes' column in the dividend output csv")
+    arg_parser.add_argument('-d', "--disable-dividend-analysis", action='store_true', help="Disable analysis of qualified dividend holding periods")
+    arg_parser.add_argument('-r', "--analysis-report", action='store_true', help="Produce a detailed report from the qualified dividends analysis.")
 
     args = arg_parser.parse_args()
     if not args.csv:
         args.csv = 'output'
 
 
     parser = Parser(args.pdf_path, args.include_dividend_notes)
```

### Comparing `parse_1099-2.0.0/parse_1099/parser.py` & `parse_1099-2.1.0/parse_1099/parser.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/pdf_contents.py` & `parse_1099-2.1.0/parse_1099/pdf_contents.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/sales/sales_interface.py` & `parse_1099-2.1.0/parse_1099/sales/sales_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/sales/v1/sales.py` & `parse_1099-2.1.0/parse_1099/sales/v1/sales.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/sales/v1/sales_parser.py` & `parse_1099-2.1.0/parse_1099/sales/v1/sales_parser.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/sales/v1/sales_total.py` & `parse_1099-2.1.0/parse_1099/sales/v1/sales_total.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/subparser_interface.py` & `parse_1099-2.1.0/parse_1099/subparser_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099/utilities/csv_writer.py` & `parse_1099-2.1.0/parse_1099/utilities/csv_writer.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/parse_1099.egg-info/PKG-INFO` & `parse_1099-2.1.0/parse_1099.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-1099
-Version: 2.0.0
+Version: 2.1.0
 Summary: Parses 1099 tax document (1099-B, 1099-INT, 1099-DIV) from PDF into CSV format and performs simple analysis
 Home-page: 
 Author: Andrew Wells, Keun Tae (Kevin) Park
 Author-email: ajwells@uchicago.com, kevin.park1217@gmail.com
 Project-URL: Bug Reports, https://github.com/ajwells256/1099-Parser/issues
 Project-URL: Source, https://github.com/ajwells256/1099-Parser
 Keywords: pdf,csv,parsing,excel,spreadsheet,tax,1099
```

### Comparing `parse_1099-2.0.0/parse_1099.egg-info/SOURCES.txt` & `parse_1099-2.1.0/parse_1099.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parse_1099-2.0.0/setup.py` & `parse_1099-2.1.0/setup.py`

 * *Files identical despite different names*

