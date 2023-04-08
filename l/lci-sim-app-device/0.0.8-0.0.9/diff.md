# Comparing `tmp/lci-sim-app-device-0.0.8.tar.gz` & `tmp/lci-sim-app-device-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lci-sim-app-device-0.0.8.tar", last modified: Sat Oct 29 23:14:20 2022, max compression
+gzip compressed data, was "dist/lci-sim-app-device-0.0.9.tar", last modified: Sat Oct 29 23:25:25 2022, max compression
```

## Comparing `lci-sim-app-device-0.0.8.tar` & `lci-sim-app-device-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/
--rw-r--r--   0 pi        (1000) pi        (1000)     1167 2022-10-29 23:14:14.000000 lci-sim-app-device-0.0.8/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/
--rw-r--r--   0 pi        (1000) pi        (1000)     1737 2022-10-29 20:52:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1674 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/run-old-method.py
--rw-r--r--   0 pi        (1000) pi        (1000)       36 2022-10-29 22:19:01.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:38:55.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1227 2022-10-29 21:19:57.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Reader.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/
--rw-r--r--   0 pi        (1000) pi        (1000)      464 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/UTF16.py
--rw-r--r--   0 pi        (1000) pi        (1000)      863 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/SystemInfo.py
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:43:00.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1318 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/ErrorLogger.py
--rw-r--r--   0 pi        (1000) pi        (1000)       98 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/RestartProgram.py
--rw-r--r--   0 pi        (1000) pi        (1000)      208 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/modification_date.py
--rw-r--r--   0 pi        (1000) pi        (1000)      590 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/MD5Sum.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6792 2022-10-29 21:17:53.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Web.py
--rw-r--r--   0 pi        (1000) pi        (1000)      372 2022-10-29 21:21:35.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/APN.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5306 2022-10-29 21:17:28.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SocketClient.py
--rw-r--r--   0 pi        (1000) pi        (1000)       32 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/Device.py
--rw-r--r--   0 pi        (1000) pi        (1000)      627 2022-10-29 19:21:33.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/LaunchArguments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2074 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SQL.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:42:46.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10666 2022-10-29 21:20:47.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/SerialReader.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4938 2022-10-29 21:21:08.000000 lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/AppHandler.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      981 2022-10-29 23:14:19.000000 lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-10-29 23:14:19.000000 lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2022-10-29 23:14:19.000000 lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      487 2022-10-29 23:14:19.000000 lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      487 2022-10-29 23:14:20.000000 lci-sim-app-device-0.0.8/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1209 2022-10-29 23:25:20.000000 lci-sim-app-device-0.0.9/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/setup.cfg
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1737 2022-10-29 20:52:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1674 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/run-old-method.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       36 2022-10-29 22:19:01.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:38:55.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1227 2022-10-29 21:19:57.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Reader.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/
+-rw-r--r--   0 pi        (1000) pi        (1000)      464 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/UTF16.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      863 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/SystemInfo.py
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:43:00.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1318 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/ErrorLogger.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       98 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/RestartProgram.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      208 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/modification_date.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      590 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/MD5Sum.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6792 2022-10-29 21:17:53.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Web.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      372 2022-10-29 21:21:35.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/APN.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5306 2022-10-29 21:17:28.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SocketClient.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       32 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/Device.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      627 2022-10-29 19:21:33.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/LaunchArguments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2074 2022-10-26 17:56:42.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SQL.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-10-29 22:42:46.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10666 2022-10-29 21:20:47.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/SerialReader.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4938 2022-10-29 21:21:08.000000 lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/AppHandler.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      981 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      487 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      487 2022-10-29 23:25:25.000000 lci-sim-app-device-0.0.9/PKG-INFO
```

### Comparing `lci-sim-app-device-0.0.8/setup.py` & `lci-sim-app-device-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'Sim App Device package'
 LONG_DESCRIPTION = 'Software to run, e.g. on a raspberry pi, to communicate with the SIM800 overlay and connect to the sim-app.ovh controller. Details can be found at https://sim-app.ovh or github.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="lci-sim-app-device", 
@@ -22,9 +22,10 @@
             #"Development Status :: 3 - Alpha",
             #"Intended Audience :: Education",
             "Programming Language :: Python :: 3",
             #"Operating System :: MacOS :: MacOS X",
             #"Operating System :: Microsoft :: Windows",
         ],
 
-        include_package_data=True
+        include_package_data=True,
+        package_dir={'Assets': 'Assets'}
 )
```

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/__main__.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/__main__.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/run-old-method.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/run-old-method.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/Reader.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/Reader.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/SystemInfo.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/ErrorLogger.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/ErrorLogger.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/Utils/MD5Sum.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/Utils/MD5Sum.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/Web.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/Web.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/SocketClient.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/SocketClient.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/LaunchArguments.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/LaunchArguments.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/SQL.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/SQL.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/SerialReader.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/SerialReader.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci-sim-app-device/App/SIM800/AppHandler.py` & `lci-sim-app-device-0.0.9/lci-sim-app-device/App/SIM800/AppHandler.py`

 * *Files identical despite different names*

### Comparing `lci-sim-app-device-0.0.8/lci_sim_app_device.egg-info/SOURCES.txt` & `lci-sim-app-device-0.0.9/lci_sim_app_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

