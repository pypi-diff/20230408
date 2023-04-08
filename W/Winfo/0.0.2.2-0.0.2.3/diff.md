# Comparing `tmp/Winfo-0.0.2.2.tar.gz` & `tmp/Winfo-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.2.2.tar", last modified: Sat Apr  8 16:21:55 2023, max compression
+gzip compressed data, was "Winfo-0.0.2.3.tar", last modified: Sat Apr  8 17:59:16 2023, max compression
```

## Comparing `Winfo-0.0.2.2.tar` & `Winfo-0.0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.599668 Winfo-0.0.2.2/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5284 2023-04-08 16:21:55.598667 Winfo-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4836 2023-04-08 16:21:08.000000 Winfo-0.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.576144 Winfo-0.0.2.2/Winfo/
--rw-rw-rw-   0        0        0     8286 2023-04-08 14:08:45.000000 Winfo-0.0.2.2/Winfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:21:55.596666 Winfo-0.0.2.2/Winfo.egg-info/
--rw-rw-rw-   0        0        0     5284 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 16:21:55.000000 Winfo-0.0.2.2/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 16:21:55.599668 Winfo-0.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-08 14:43:56.000000 Winfo-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.832026 Winfo-0.0.2.3/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5360 2023-04-08 17:59:16.831026 Winfo-0.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4912 2023-04-08 17:58:30.000000 Winfo-0.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.811397 Winfo-0.0.2.3/Winfo/
+-rw-rw-rw-   0        0        0     8482 2023-04-08 16:41:27.000000 Winfo-0.0.2.3/Winfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.830030 Winfo-0.0.2.3/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     5360 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:59:16.832026 Winfo-0.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-04-08 16:24:31.000000 Winfo-0.0.2.3/setup.py
```

### Comparing `Winfo-0.0.2.2/LICENSE` & `Winfo-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.2/PKG-INFO` & `Winfo-0.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,22 +19,24 @@
 ### Processor Information
 
 - Get Brandname (Name you see in Taskmanager)
 - Get "real" name
 - Get Maximum Clock Speed
 - Get amount of cores
 - Get amount of threads
+- Get Architecture
 
 ```Python
 import Winfo
 
 print("I have an " + Winfo.cpu.getbrandname())
 print("It's real name is " + Winfo.cpu.getrealname())
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
+print("CPU Architecture: " + Winfo.cpu.architecture())
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
 - Get Refresh Rate
```

### Comparing `Winfo-0.0.2.2/README.md` & `Winfo-0.0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 ### Processor Information
 
 - Get Brandname (Name you see in Taskmanager)
 - Get "real" name
 - Get Maximum Clock Speed
 - Get amount of cores
 - Get amount of threads
+- Get Architecture
 
 ```Python
 import Winfo
 
 print("I have an " + Winfo.cpu.getbrandname())
 print("It's real name is " + Winfo.cpu.getrealname())
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
+print("CPU Architecture: " + Winfo.cpu.architecture())
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
 - Get Refresh Rate
```

### Comparing `Winfo-0.0.2.2/Winfo/__init__.py` & `Winfo-0.0.2.3/Winfo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 
   def threads():
     raw = check_output(["wmic", "cpu", "get", "ThreadCount"])
     rawdecoded = raw.decode()
     getthreads = rawdecoded.strip("ThreadCount").rstrip("\n").replace("\n", "")
     return int(getthreads)
   
+  def architecture():
+    raw = check_output(["echo", "%PROCESSOR_ARCHITECTURE%"], shell=True)
+    rawdecoded = raw.decode()
+    cpuarch = rawdecoded.replace("\n", "")
+    return cpuarch
+  
 class gpu:
   def getname():
     raw = check_output(["wmic", "path", "win32_VideoController", "get", "name"])
     rawdecoded = raw.decode()
     getname = rawdecoded.strip("Name").rstrip("\n").replace("\n", "")
     return getname
   def getRefreshRate():
```

### Comparing `Winfo-0.0.2.2/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.2.3/Winfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,22 +19,24 @@
 ### Processor Information
 
 - Get Brandname (Name you see in Taskmanager)
 - Get "real" name
 - Get Maximum Clock Speed
 - Get amount of cores
 - Get amount of threads
+- Get Architecture
 
 ```Python
 import Winfo
 
 print("I have an " + Winfo.cpu.getbrandname())
 print("It's real name is " + Winfo.cpu.getrealname())
 print("This monster works at " + Winfo.cpu.MaxClockSpeed() + " Ghz")
 print("It has" + str(Winfo.cpu.cores()) + " Cores and " + str(Winfo.cpu.threads) + " Threads")
+print("CPU Architecture: " + Winfo.cpu.architecture())
 ```
 
 ### GPU Information
 
 - Get Brandname of GPU
 - Get Refresh Rate
```

### Comparing `Winfo-0.0.2.2/setup.py` & `Winfo-0.0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.2.2",
+    version="0.0.2.3",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

