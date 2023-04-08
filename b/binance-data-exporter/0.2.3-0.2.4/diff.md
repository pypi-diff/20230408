# Comparing `tmp/binance_data_exporter-0.2.3.tar.gz` & `tmp/binance_data_exporter-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_data_exporter-0.2.3.tar", last modified: Sat Apr  8 16:09:52 2023, max compression
+gzip compressed data, was "binance_data_exporter-0.2.4.tar", last modified: Sat Apr  8 16:31:45 2023, max compression
```

## Comparing `binance_data_exporter-0.2.3.tar` & `binance_data_exporter-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.189442 binance_data_exporter-0.2.3/
--rw-rw-rw-   0        0        0       32 2023-04-08 16:07:11.000000 binance_data_exporter-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4563 2023-04-08 16:09:52.188459 binance_data_exporter-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4308 2023-04-08 14:33:42.000000 binance_data_exporter-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.104440 binance_data_exporter-0.2.3/binance_data_exporter/
--rw-rw-rw-   0        0        0        0 2023-04-08 16:08:49.000000 binance_data_exporter-0.2.3/binance_data_exporter/__init__.py
--rw-rw-rw-   0        0        0     9242 2023-04-08 14:37:53.000000 binance_data_exporter-0.2.3/binance_data_exporter/binance_data_exporter.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:09:52.181452 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-08 16:09:52.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-08 16:09:51.000000 binance_data_exporter-0.2.3/binance_data_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 16:09:52.189442 binance_data_exporter-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-04-08 16:09:38.000000 binance_data_exporter-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:31:45.534859 binance_data_exporter-0.2.4/
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:31:45.533852 binance_data_exporter-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4308 2023-04-08 14:33:42.000000 binance_data_exporter-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 16:31:45.499852 binance_data_exporter-0.2.4/binance_data_exporter/
+-rw-rw-rw-   0        0        0        0 2023-04-08 16:08:49.000000 binance_data_exporter-0.2.4/binance_data_exporter/__init__.py
+-rw-rw-rw-   0        0        0     9242 2023-04-08 14:37:53.000000 binance_data_exporter-0.2.4/binance_data_exporter/binance_data_exporter.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:31:45.531870 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-08 16:31:45.000000 binance_data_exporter-0.2.4/binance_data_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 16:31:45.534859 binance_data_exporter-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-04-08 16:31:25.000000 binance_data_exporter-0.2.4/setup.py
```

### Comparing `binance_data_exporter-0.2.3/PKG-INFO` & `binance_data_exporter-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance_data_exporter
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for exporting in JSON the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Exporter
```

### Comparing `binance_data_exporter-0.2.3/README.md` & `binance_data_exporter-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `binance_data_exporter-0.2.3/binance_data_exporter/binance_data_exporter.py` & `binance_data_exporter-0.2.4/binance_data_exporter/binance_data_exporter.py`

 * *Files identical despite different names*

### Comparing `binance_data_exporter-0.2.3/binance_data_exporter.egg-info/PKG-INFO` & `binance_data_exporter-0.2.4/binance_data_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-data-exporter
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for exporting in JSON the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Exporter
```

### Comparing `binance_data_exporter-0.2.3/setup.py` & `binance_data_exporter-0.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='binance_data_exporter',
-    version='0.2.3',  # current_version
+    version='0.2.4',  # current_version
     description='A tool for exporting in JSON the historical data of a symbol from Binance',
     author='zestones',
     author_email='idrissbenguezzou@gmail.com',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'binance_data_exporter=binance_data_exporter:main'
+            'binance_data_exporter=binance_data_exporter.binance_data_exporter:main'
         ]
     },
     install_requires=[
         'requests',
         'colorama',
         'tabulate',
     ],
```

