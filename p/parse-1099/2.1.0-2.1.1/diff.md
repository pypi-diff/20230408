# Comparing `tmp/parse_1099-2.1.0.tar.gz` & `tmp/parse_1099-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_1099-2.1.0.tar", last modified: Sat Apr  8 16:30:00 2023, max compression
+gzip compressed data, was "parse_1099-2.1.1.tar", last modified: Sat Apr  8 21:46:47 2023, max compression
```

## Comparing `parse_1099-2.1.0.tar` & `parse_1099-2.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-08 16:29:45.000000 parse_1099-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-08 16:29:45.000000 parse_1099-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-08 16:29:45.000000 parse_1099-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 16:30:00.007226 parse_1099-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-08 16:29:45.000000 parse_1099-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.003226 parse_1099-2.1.0/parse_1099/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/dividends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividend_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividends_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/dividends_repository_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/dividends/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/dividends/v1/dividends_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/pdf_contents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/sales/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/sales_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/sales/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/sales/v1/sales_total.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/subparser_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.007226 parse_1099-2.1.0/parse_1099/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 16:29:45.000000 parse_1099-2.1.0/parse_1099/utilities/csv_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:30:00.003226 parse_1099-2.1.0/parse_1099.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 16:29:59.000000 parse_1099-2.1.0/parse_1099.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 16:29:45.000000 parse_1099-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 16:30:00.007226 parse_1099-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-08 16:29:45.000000 parse_1099-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.620118 parse_1099-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-08 21:46:33.000000 parse_1099-2.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-08 21:46:33.000000 parse_1099-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-08 21:46:33.000000 parse_1099-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 21:46:47.620118 parse_1099-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-08 21:46:33.000000 parse_1099-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.612118 parse_1099-2.1.1/parse_1099/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.616119 parse_1099-2.1.1/parse_1099/dividends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/dividend_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/dividends_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/dividends_repository_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.616119 parse_1099-2.1.1/parse_1099/dividends/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/v1/dividends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/v1/dividends_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/v1/dividends_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/dividends/v1/dividends_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/pdf_contents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.616119 parse_1099-2.1.1/parse_1099/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/sales_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.616119 parse_1099-2.1.1/parse_1099/sales/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/v1/sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/v1/sales_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/sales/v1/sales_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/subparser_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.620118 parse_1099-2.1.1/parse_1099/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 21:46:33.000000 parse_1099-2.1.1/parse_1099/utilities/csv_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:46:47.612118 parse_1099-2.1.1/parse_1099.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 21:46:47.000000 parse_1099-2.1.1/parse_1099.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 21:46:33.000000 parse_1099-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-08 21:46:47.620118 parse_1099-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-08 21:46:33.000000 parse_1099-2.1.1/setup.py
```

### Comparing `parse_1099-2.1.0/LICENSE` & `parse_1099-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/PKG-INFO` & `parse_1099-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_1099
-Version: 2.1.0
+Version: 2.1.1
 Summary: Parses 1099 tax document (1099-B, 1099-INT, 1099-DIV) from PDF into CSV format and performs simple analysis
 Home-page: 
 Author: Andrew Wells, Keun Tae (Kevin) Park
 Author-email: ajwells@uchicago.com, kevin.park1217@gmail.com
 Project-URL: Bug Reports, https://github.com/ajwells256/1099-Parser/issues
 Project-URL: Source, https://github.com/ajwells256/1099-Parser
 Keywords: pdf,csv,parsing,excel,spreadsheet,tax,1099
```

### Comparing `parse_1099-2.1.0/README.md` & `parse_1099-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/dividends/dividend_analyzer.py` & `parse_1099-2.1.1/parse_1099/dividends/dividend_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 from pandas.core.series import Series
 from re import search, compile
 from typing import Union, Tuple
+from locale import atof
 
 from .dividends_interface import DividendsInterface
 from .dividends_repository_interface import DividendsRepositoryInterface
 from .dividends_repository_interface import By
 from .v1.dividends_repository import DividendsRepository
 from .v1.dividends_total import DividendsTotal
 from ..pdf_contents import PDFContents
@@ -26,43 +27,46 @@
     def enable_reporting(self, report_prefix: str):
         self.report_prefix = report_prefix
 
     def get_disqualified_dividends(self, contents: PDFContents) -> "Tuple[Union[list[DividendsInterface], None], Union[DividendsTotal, None]]":
         '''Gets an adjusted list of dividends, or None if there were no disqualifications'''
         # get securities that had qualified dividends
         cusips = DividendAnalyzer.get_securities_with_qualified_dividends(contents.dividends)
+        adjusted_total = None
+        adjusted_dividends = None
 
-        # get sales for those securities and calculate holding period
-        transactions_with_short_holding_periods = DividendAnalyzer.get_securities_with_short_holding_periods(contents.sales, cusips)
-        symbols_with_short_holding_periods = [s.symbol for s in transactions_with_short_holding_periods if s.symbol is not None]
-        cusips_with_short_holding_periods = [s.cusip for s in transactions_with_short_holding_periods if s.symbol is None and s.cusip is not None]
-
-        # fetch dividend information for all securities with holding periods less than 60 days
-        prev_year = datetime.now().year - 1
-        cusip_exdates, cusip_to_symbol_map = self.repository.get_dividend_exdates(By.CUSIP, cusips_with_short_holding_periods, prev_year)
-        symbol_exdates, _ = self.repository.get_dividend_exdates(By.SYMBOL, symbols_with_short_holding_periods, prev_year)
-
-        dividend_exdates = None
-        if (cusip_exdates is not None and symbol_exdates is not None):
-            dividend_exdates = cusip_exdates.append(symbol_exdates)
-        elif (cusip_exdates is not None):
-            dividend_exdates = cusip_exdates
-        elif (symbol_exdates is not None):
-            dividend_exdates = symbol_exdates
-
-        if dividend_exdates is None:
-            raise Exception("Encountered an error while retreiving ex-dividend dates")
-
-        # produce an updated list of dividends
-        cusip_to_symbol_map.update([(s.cusip, s.symbol) for s in transactions_with_short_holding_periods if s.symbol is not None and s.cusip is not None])
+        if len(cusips) > 0:
+            # get sales for those securities and calculate holding period
+            transactions_with_short_holding_periods = DividendAnalyzer.get_securities_with_short_holding_periods(contents.sales, cusips)
+            symbols_with_short_holding_periods = [s.symbol for s in transactions_with_short_holding_periods if s.symbol is not None]
+            cusips_with_short_holding_periods = [s.cusip for s in transactions_with_short_holding_periods if s.symbol is None and s.cusip is not None]
+
+            # fetch dividend information for all securities with holding periods less than 60 days
+            prev_year = datetime.now().year - 1
+            cusip_exdates, cusip_to_symbol_map = self.repository.get_dividend_exdates(By.CUSIP, cusips_with_short_holding_periods, prev_year)
+            symbol_exdates, _ = self.repository.get_dividend_exdates(By.SYMBOL, symbols_with_short_holding_periods, prev_year)
+
+            dividend_exdates = None
+            if (cusip_exdates is not None and symbol_exdates is not None):
+                dividend_exdates = cusip_exdates.append(symbol_exdates)
+            elif (cusip_exdates is not None):
+                dividend_exdates = cusip_exdates
+            elif (symbol_exdates is not None):
+                dividend_exdates = symbol_exdates
+
+            if dividend_exdates is None:
+                raise Exception("Encountered an error while retreiving ex-dividend dates")
+
+            # produce an updated list of dividends
+            cusip_to_symbol_map.update([(s.cusip, s.symbol) for s in transactions_with_short_holding_periods if s.symbol is not None and s.cusip is not None])
+
+            adjusted_dividends = self.get_adjusted_dividends(contents.dividends, transactions_with_short_holding_periods, dividend_exdates, cusip_to_symbol_map)
+            if adjusted_dividends is not None:
+                adjusted_total = DividendsTotal.FromDividends(adjusted_dividends)
 
-        adjusted_dividends = self.get_adjusted_dividends(contents.dividends, transactions_with_short_holding_periods, dividend_exdates, cusip_to_symbol_map)
-        adjusted_total = None
-        if adjusted_dividends is not None:
-            adjusted_total = DividendsTotal.FromDividends(adjusted_dividends)
         return adjusted_dividends, adjusted_total
 
     def get_adjusted_dividends(self, dividends: "list[DividendsInterface]",
                                sales_with_short_holding_periods: "list[SalesInterface]",
                                dividend_exdates: Series, cusip_to_symbol: "dict[str, str]") -> Union["list[DividendsInterface]", None]:
 
         # for each cusip, get all relevant dividends
@@ -89,32 +93,40 @@
                     working_dividend = dividend.copy()
                     adjusted_dividends.append(working_dividend)
 
                     if not dividend.get("transaction_type").startswith("Qualified"):
                         # skip all except the qualified dividends when analyzing for disqualified dividends
                         continue
 
+                    related_dividends = [cusip_div for cusip_div in cusip_dividends
+                                            if dividend.date == cusip_div.date]
+                    
+                    parsed_related_dividend_amounts = [atof(div.get("amount")) for div in related_dividends]
+                    total_dividend_amount = sum([amount for amount in parsed_related_dividend_amounts if amount > 0]) # excludes taxes withheld
+                    qualified_percent = atof(working_dividend.get("amount")) / total_dividend_amount
+
                     exdate = DividendAnalyzer.get_dividend_exdate(
                         working_dividend, cusip_exdates)
                     disqualified_sales = [sale for sale in sales_with_short_holding_periods
                                           if sale.cusip == cusip and
                                           sale.acquired_date <= exdate and exdate <= sale.disposal_date]  # type:ignore since all fields should be populated
 
                     disqualified_sale_count = len(disqualified_sales)
                     if disqualified_sale_count != 0:
                         adjustment_occurred = True
+                        disqualified_shares_count = sum(atof(sale.get("quantity")) for sale in disqualified_sales)
 
                         amount_per_share = cusip_exdates[exdate.date()]
                         disqualified_dividend = working_dividend.disqualify(
-                            disqualified_sale_count, amount_per_share)
+                            disqualified_shares_count, amount_per_share * qualified_percent)
                         adjusted_dividends.append(disqualified_dividend)
 
                         if self.report_prefix is not None:
                             for sale in disqualified_sales:
-                                sale.add_note(f"Disqualifies dividend {working_dividend} with exdate {exdate} and payout ${amount_per_share}")
+                                sale.add_note(f"Disqualifies dividend {dividend} with exdate {exdate}, payout ${amount_per_share} and qualified percentage {round(qualified_percent*100, 1)}%")
                             detailed_report.extend(disqualified_sales)
 
                 if self.report_prefix is not None:
                     qualified_sales = [sale for sale in sales_with_short_holding_periods
                                        if sale.cusip == cusip and sale not in detailed_report]
                     for sale in qualified_sales:
                         sale.add_note("")
```

### Comparing `parse_1099-2.1.0/parse_1099/dividends/dividends_interface.py` & `parse_1099-2.1.1/parse_1099/dividends/dividends_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/dividends/v1/dividends.py` & `parse_1099-2.1.1/parse_1099/dividends/v1/dividends.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         assert(Dividends._quantity_pattern.match(data[3])) # amount
         assert(isinstance(data[4], str)) # transaction_type
         if (include_notes):
             assert(isinstance(data[5], str)) # notes
 
     def disqualify(self, shares_disqualified, share_dividend_amount) -> "DividendsInterface":
         '''Produces a new Dividend of type 'nonqualified dividend' and adjusts this dividend accordingly'''
-        disqualification_amount = shares_disqualified * share_dividend_amount
+        disqualification_amount = round(shares_disqualified * share_dividend_amount, 2)
         dividend_data = [self.get("security"), self.get("cusip"), \
                 self.get("transaction_date"), str(disqualification_amount), "Nonqualified dividend"]
         if self.include_notes:
             dividend_data.append(self.get("notes"))
 
         disqualified_dividend = Dividends(dividend_data, self.include_notes, disqualified = True)
 
@@ -60,15 +60,15 @@
         new_qualified_amount = parsed_amount - disqualification_amount
         assert(new_qualified_amount > 0)
         self.data[amount_idx] = str(new_qualified_amount)
 
         return disqualified_dividend
 
     def copy(self) -> "DividendsInterface":
-        return Dividends(self.data, self.include_notes)
+        return Dividends(self.data.copy(), self.include_notes)
 
     @staticmethod
     def parse(raw_data: "list[str]", include_notes: bool) -> "list[Dividends]":
         transx: list[Dividends] = []
         assert(isinstance(raw_data, list))
         if not raw_data: return transx  # empty list
 
@@ -180,11 +180,21 @@
         subtotals = {}
         while cursor < len(raw_data):
             if Dividends._subtotal_pattern.match(raw_data[cursor]) \
                     and Dividends._quantity_pattern.match(raw_data[cursor-1]):
                 subtotal_amount = atof(raw_data[cursor-1])
                 subtotals[raw_data[cursor]] = subtotal_amount
             cursor += 1
+
+        total_title = "Total Dividends & distributions"
+        tax_exempt_title = "Total Tax-exempt dividends"
+        foreign_tax_withheld_title = "Total Foreign tax withheld"
+        if total_title not in subtotals:
+            subtotals[total_title] = 0
+        if tax_exempt_title not in subtotals:
+            subtotals[tax_exempt_title] = 0
+        if foreign_tax_withheld_title not in subtotals:
+            subtotals[foreign_tax_withheld_title] = 0
         
         return DividendsTotal(subtotals["Total Dividends & distributions"], \
             tax_exempt=subtotals["Total Tax-exempt dividends"], \
             foreign_tax_withheld=subtotals["Total Foreign tax withheld"])
```

### Comparing `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_parser.py` & `parse_1099-2.1.1/parse_1099/dividends/v1/dividends_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from ...subparser_interface import SubparserInterface
 from ...pdf_contents import PDFContents
 from .dividends import Dividends
 
 
 class DividendsParser(SubparserInterface):
 
+    _transaction_type_pattern = compile(".*(dividend|withheld).*")
+
     def __init__(self, pdf_file, include_dividend_notes: bool = False):
         super().__init__(pdf_file)
         self.include_notes = include_dividend_notes
 
     def process(self, show_progress: bool, pdf_contents: PDFContents) -> PDFContents:
         indicator_str = "Detail for Dividends and Distributions"
         num_pages = len(self.pages)
@@ -32,21 +34,25 @@
                     continue
 
                 def get_next_security_index(strings, start_idx = 0) -> Union[int, None]:
                     for i in range(start_idx, len(strings)-1):
                         if Dividends._security_pattern.match(strings[i]) and Dividends._cusip_pattern.match(strings[i+1]):
                             return i
 
+                # robinhood header can look like a security header since their account ids are the same form as CUSIPs
+                # endeavor to pass over these false matches by advancing at least as far as the title, which in the current version gets beyond the robinhood account string
+                header_title_idx = strings.index(indicator_str)
                 prev_header_idx: int = -1
-                security_header_idx = get_next_security_index(strings)
+                security_header_idx = get_next_security_index(strings, header_title_idx+1)
                 while security_header_idx:
                     # fix multi-line securities names. Not ideal, could improve
                     if (security_header_idx > 0 and \
                         Dividends._security_pattern.match(strings[security_header_idx-1]) and \
-                        not Dividends._subtotal_pattern.match(strings[security_header_idx-1])):
+                        not Dividends._subtotal_pattern.match(strings[security_header_idx-1]) and \
+                        not DividendsParser._transaction_type_pattern.match(strings[security_header_idx-1])): # in the case where there's just one dividend for a security, there isn't a subtotal
                         strings[security_header_idx] = f"{strings[security_header_idx-1]} {strings[security_header_idx]}"
 
                     # case: this isn't the first header on the page
                     if prev_header_idx >= 0:
                         # action: previous security is finished, parse its range of lines into a Sales
                         security_dividends_lines = dangling_lines + strings[prev_header_idx:security_header_idx]
                         dangling_lines = []
```

### Comparing `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_repository.py` & `parse_1099-2.1.1/parse_1099/dividends/v1/dividends_repository.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/dividends/v1/dividends_total.py` & `parse_1099-2.1.1/parse_1099/dividends/v1/dividends_total.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/main.py` & `parse_1099-2.1.1/parse_1099/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             if not args.disable_dividend_analysis:
                 dividend_analyzer = DividendAnalyzer()
                 if args.analysis_report:
                     dividend_analyzer.enable_reporting(args.csv)
                 adjusted_dividends, adjusted_total = dividend_analyzer.get_disqualified_dividends(contents)
                 if adjusted_dividends is not None:
                     assert(adjusted_total is not None) # this should never be none if there are dividends
-                    print(f"Analyzed dividends and determinded that ${adjusted_total.disqualified} of qualified dividends should be considered nonqualified due to short holding periods around the ex-dividend date")
+                    report = "For more details, see the sales_with_short_holding_periods report." if args.analysis_report else "For more details, use the --analysis-report flag."
+                    print(f">>> Analyzed dividends and determinded that ${adjusted_total.disqualified:.2f} of qualified dividends should be considered nonqualified due to \
+                          short holding periods around the ex-dividend date. The disqualification is reflected in the adjusted_dividends csv. {report}")
                     adjusted_dividends_csv = f"{args.csv}_adjusted_dividends.csv"
                     csv_writer.write_to_csv(adjusted_dividends_csv, adjusted_dividends)
 
-                    print(adjusted_total)
+                    if args.validate:
+                        print(adjusted_total)
     else:
         print(f">>> No data to save to file")
```

### Comparing `parse_1099-2.1.0/parse_1099/parser.py` & `parse_1099-2.1.1/parse_1099/parser.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/pdf_contents.py` & `parse_1099-2.1.1/parse_1099/pdf_contents.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/sales/sales_interface.py` & `parse_1099-2.1.1/parse_1099/sales/sales_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/sales/v1/sales.py` & `parse_1099-2.1.1/parse_1099/sales/v1/sales.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/sales/v1/sales_parser.py` & `parse_1099-2.1.1/parse_1099/sales/v1/sales_parser.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/sales/v1/sales_total.py` & `parse_1099-2.1.1/parse_1099/sales/v1/sales_total.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/subparser_interface.py` & `parse_1099-2.1.1/parse_1099/subparser_interface.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099/utilities/csv_writer.py` & `parse_1099-2.1.1/parse_1099/utilities/csv_writer.py`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/parse_1099.egg-info/PKG-INFO` & `parse_1099-2.1.1/parse_1099.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-1099
-Version: 2.1.0
+Version: 2.1.1
 Summary: Parses 1099 tax document (1099-B, 1099-INT, 1099-DIV) from PDF into CSV format and performs simple analysis
 Home-page: 
 Author: Andrew Wells, Keun Tae (Kevin) Park
 Author-email: ajwells@uchicago.com, kevin.park1217@gmail.com
 Project-URL: Bug Reports, https://github.com/ajwells256/1099-Parser/issues
 Project-URL: Source, https://github.com/ajwells256/1099-Parser
 Keywords: pdf,csv,parsing,excel,spreadsheet,tax,1099
```

### Comparing `parse_1099-2.1.0/parse_1099.egg-info/SOURCES.txt` & `parse_1099-2.1.1/parse_1099.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parse_1099-2.1.0/setup.py` & `parse_1099-2.1.1/setup.py`

 * *Files identical despite different names*

