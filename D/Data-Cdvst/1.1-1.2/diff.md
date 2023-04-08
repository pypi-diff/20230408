# Comparing `tmp/Data_Cdvst-1.1.tar.gz` & `tmp/Data_Cdvst-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Data_Cdvst-1.1.tar", last modified: Sat Apr  8 18:27:00 2023, max compression
+gzip compressed data, was "Data_Cdvst-1.2.tar", last modified: Sat Apr  8 20:25:36 2023, max compression
```

## Comparing `Data_Cdvst-1.1.tar` & `Data_Cdvst-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/
-drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.928600 Data_Cdvst-1.1/Data_Cdvst/
--rw-rw-rw-   0        0        0        0 2023-04-08 11:10:24.000000 Data_Cdvst-1.1/Data_Cdvst/Files_Cdvst.py
--rw-rw-rw-   0        0        0     9532 2023-04-08 12:16:08.000000 Data_Cdvst-1.1/Data_Cdvst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/Data_Cdvst.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1385 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-08 12:19:19.000000 Data_Cdvst-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:25:36.067351 Data_Cdvst-1.2/
+drwxrwxrwx   0        0        0        0 2023-04-08 20:25:36.052848 Data_Cdvst-1.2/Data_Cdvst/
+-rw-rw-rw-   0        0        0        0 2023-04-08 11:10:24.000000 Data_Cdvst-1.2/Data_Cdvst/Files_Cdvst.py
+-rw-rw-rw-   0        0        0     9525 2023-04-08 18:50:29.000000 Data_Cdvst-1.2/Data_Cdvst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:25:36.052848 Data_Cdvst-1.2/Data_Cdvst.egg-info/
+-rw-rw-rw-   0        0        0     1385 2023-04-08 20:25:35.000000 Data_Cdvst-1.2/Data_Cdvst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-08 20:25:35.000000 Data_Cdvst-1.2/Data_Cdvst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 20:25:35.000000 Data_Cdvst-1.2/Data_Cdvst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 20:25:35.000000 Data_Cdvst-1.2/Data_Cdvst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1385 2023-04-08 20:25:36.067351 Data_Cdvst-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 20:25:36.067351 Data_Cdvst-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-08 20:24:30.000000 Data_Cdvst-1.2/setup.py
```

### Comparing `Data_Cdvst-1.1/Data_Cdvst/__init__.py` & `Data_Cdvst-1.2/Data_Cdvst/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlite3
 from contextlib import contextmanager
 from sqlite3 import Error
 import time
-from import Files_Cdvst import *
+from Files_Cdvst import *
 
 class Database:
     """
     Eine Singleton-Klasse zum Verwalten von SQLite-Datenbanken.
 
     Beispiel:
```

### Comparing `Data_Cdvst-1.1/Data_Cdvst.egg-info/PKG-INFO` & `Data_Cdvst-1.2/Data_Cdvst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data-Cdvst
-Version: 1.1
+Version: 1.2
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.1/PKG-INFO` & `Data_Cdvst-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data_Cdvst
-Version: 1.1
+Version: 1.2
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.1/README.md` & `Data_Cdvst-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Data_Cdvst-1.1/setup.py` & `Data_Cdvst-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Data_Cdvst',
-    version='1.1',
+    version='1.2',
     description='Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.',
     long_description="""Data_Cdvst ist eine Python-Bibliothek zur einfachen nutzung von Datenbanken undeinfachen umgang mit datenverarbeitugn und -aufnahme. Die Bibliothek bietet Funktionen zum Abspielen von WAV- und MP3-Dateien sowie zur Aufnahme von Audio in einer WAV-Datei. Die Bibliothek umfasst auch eine automatische Spracherkennungsfunktion.
 
 Funktionen:
 - Einfache Datenbank erstellung
 - Einfache Datenbanken Einträge erzeugen
 - Einfahce Datenbanken auslesen
```

