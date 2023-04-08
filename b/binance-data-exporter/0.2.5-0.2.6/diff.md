# Comparing `tmp/binance_data_exporter-0.2.5.tar.gz` & `tmp/binance_data_exporter-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_data_exporter-0.2.5.tar", last modified: Sat Apr  8 16:36:38 2023, max compression
+gzip compressed data, was "binance_data_exporter-0.2.6.tar", last modified: Sat Apr  8 16:48:11 2023, max compression
```

## Comparing `binance_data_exporter-0.2.5.tar` & `binance_data_exporter-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 16:36:38.978729 binance_data_exporter-0.2.5/
--rw-rw-rw-   0        0        0     4563 2023-04-08 16:36:38.977733 binance_data_exporter-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4308 2023-04-08 14:33:42.000000 binance_data_exporter-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 16:36:38.952726 binance_data_exporter-0.2.5/binance_data_exporter/
--rw-rw-rw-   0        0        0        0 2023-04-08 16:08:49.000000 binance_data_exporter-0.2.5/binance_data_exporter/__init__.py
--rw-rw-rw-   0        0        0     9361 2023-04-08 16:35:44.000000 binance_data_exporter-0.2.5/binance_data_exporter/binance_data_exporter.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:36:38.974728 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-08 16:36:38.000000 binance_data_exporter-0.2.5/binance_data_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 16:36:38.978729 binance_data_exporter-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-04-08 16:36:08.000000 binance_data_exporter-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:48:11.969740 binance_data_exporter-0.2.6/
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:48:11.968745 binance_data_exporter-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4308 2023-04-08 14:33:42.000000 binance_data_exporter-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 16:48:11.937577 binance_data_exporter-0.2.6/binance_data_exporter/
+-rw-rw-rw-   0        0        0        0 2023-04-08 16:08:49.000000 binance_data_exporter-0.2.6/binance_data_exporter/__init__.py
+-rw-rw-rw-   0        0        0     9365 2023-04-08 16:47:13.000000 binance_data_exporter-0.2.6/binance_data_exporter/binance_data_exporter.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:48:11.966786 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-08 16:48:11.000000 binance_data_exporter-0.2.6/binance_data_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 16:48:11.969740 binance_data_exporter-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-04-08 16:47:58.000000 binance_data_exporter-0.2.6/setup.py
```

### Comparing `binance_data_exporter-0.2.5/PKG-INFO` & `binance_data_exporter-0.2.6/binance_data_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: binance_data_exporter
-Version: 0.2.5
+Name: binance-data-exporter
+Version: 0.2.6
 Summary: A tool for exporting in JSON the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Exporter
```

### Comparing `binance_data_exporter-0.2.5/README.md` & `binance_data_exporter-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `binance_data_exporter-0.2.5/binance_data_exporter/binance_data_exporter.py` & `binance_data_exporter-0.2.6/binance_data_exporter/binance_data_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         elif opt in ("-o", "--output_folder"):
             OUTPUT_FOLDER = arg
 
 
 # ------------------------------------------------------------------------------ #
 #                               * MAIN *                                         #
 # ------------------------------------------------------------------------------ #
-def main(argv=None) -> None:
+def main(argv=sys.argv) -> None:
     """
     Main function
     param argv: The command line arguments
     """
     
     if argv is not None: parse_command_line_args(argv)
     data = request_data()
```

### Comparing `binance_data_exporter-0.2.5/binance_data_exporter.egg-info/PKG-INFO` & `binance_data_exporter-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: binance-data-exporter
-Version: 0.2.5
+Name: binance_data_exporter
+Version: 0.2.6
 Summary: A tool for exporting in JSON the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Exporter
```

### Comparing `binance_data_exporter-0.2.5/setup.py` & `binance_data_exporter-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='binance_data_exporter',
-    version='0.2.5',  # current_version
+    version='0.2.6',  # current_version
     description='A tool for exporting in JSON the historical data of a symbol from Binance',
     author='zestones',
     author_email='idrissbenguezzou@gmail.com',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'binance_data_exporter=binance_data_exporter.binance_data_exporter:main [argv]'
```

