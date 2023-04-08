# Comparing `tmp/Winfo-0.0.2.1.tar.gz` & `tmp/Winfo-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.2.1.tar", last modified: Sat Apr  8 14:14:12 2023, max compression
+gzip compressed data, was "Winfo-0.0.2.2.tar", last modified: Sat Apr  8 16:21:55 2023, max compression
```

## Comparing `Winfo-0.0.2.1.tar` & `Winfo-0.0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 14:14:12.511966 Winfo-0.0.2.1/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.1/LICENSE
--rw-rw-rw-   0        0        0     5264 2023-04-08 14:14:12.510967 Winfo-0.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4816 2023-04-08 14:10:53.000000 Winfo-0.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 14:14:12.497967 Winfo-0.0.2.1/Winfo/
--rw-rw-rw-   0        0        0     8286 2023-04-08 14:08:45.000000 Winfo-0.0.2.1/Winfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:14:12.509966 Winfo-0.0.2.1/Winfo.egg-info/
--rw-rw-rw-   0        0        0     5264 2023-04-08 14:14:12.000000 Winfo-0.0.2.1/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-08 14:14:12.000000 Winfo-0.0.2.1/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 14:14:12.000000 Winfo-0.0.2.1/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 14:14:12.000000 Winfo-0.0.2.1/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 14:14:12.511966 Winfo-0.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-08 14:13:35.000000 Winfo-0.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.599668 Winfo-0.0.2.2/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     5284 2023-04-08 16:21:55.598667 Winfo-0.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4836 2023-04-08 16:21:08.000000 Winfo-0.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.576144 Winfo-0.0.2.2/Winfo/
+-rw-rw-rw-   0        0        0     8286 2023-04-08 14:08:45.000000 Winfo-0.0.2.2/Winfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.596666 Winfo-0.0.2.2/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     5284 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 16:21:55.599668 Winfo-0.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-04-08 14:43:56.000000 Winfo-0.0.2.2/setup.py
```

### Comparing `Winfo-0.0.2.1/LICENSE` & `Winfo-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.1/PKG-INFO` & `Winfo-0.0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -32,14 +32,15 @@
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
+- Get Refresh Rate
 
 ```Python
 import Winfo
 
 print("My GPU is the " + Winfo.gpu.getname())
 print("I like my " + Winfo.gpu.getRefreshRate() + " Hz")
 ```
```

### Comparing `Winfo-0.0.2.1/README.md` & `Winfo-0.0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
+- Get Refresh Rate
 
 ```Python
 import Winfo
 
 print("My GPU is the " + Winfo.gpu.getname())
 print("I like my " + Winfo.gpu.getRefreshRate() + " Hz")
 ```
```

### Comparing `Winfo-0.0.2.1/Winfo/__init__.py` & `Winfo-0.0.2.2/Winfo/__init__.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.1/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.2.2/Winfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -32,14 +32,15 @@
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
+- Get Refresh Rate
 
 ```Python
 import Winfo
 
 print("My GPU is the " + Winfo.gpu.getname())
 print("I like my " + Winfo.gpu.getRefreshRate() + " Hz")
 ```
```

### Comparing `Winfo-0.0.2.1/setup.py` & `Winfo-0.0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.2.1",
+    version="0.0.2.2",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

