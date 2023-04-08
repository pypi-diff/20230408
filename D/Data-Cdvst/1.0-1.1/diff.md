# Comparing `tmp/Data_Cdvst-1.0.tar.gz` & `tmp/Data_Cdvst-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Data_Cdvst-1.0.tar", last modified: Mon Apr  3 22:30:25 2023, max compression
+gzip compressed data, was "Data_Cdvst-1.1.tar", last modified: Sat Apr  8 18:27:00 2023, max compression
```

## Comparing `Data_Cdvst-1.0.tar` & `Data_Cdvst-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 22:30:25.626394 Data_Cdvst-1.0/
-drwxrwxrwx   0        0        0        0 2023-04-03 22:30:25.579931 Data_Cdvst-1.0/Data_Cdvst/
--rw-rw-rw-   0        0        0     8084 2023-04-03 22:09:33.000000 Data_Cdvst-1.0/Data_Cdvst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 22:30:25.623306 Data_Cdvst-1.0/Data_Cdvst.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-04-03 22:30:25.000000 Data_Cdvst-1.0/Data_Cdvst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-03 22:30:25.000000 Data_Cdvst-1.0/Data_Cdvst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 22:30:25.000000 Data_Cdvst-1.0/Data_Cdvst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-03 22:30:25.000000 Data_Cdvst-1.0/Data_Cdvst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1385 2023-04-03 22:30:25.625384 Data_Cdvst-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-03 22:30:25.626394 Data_Cdvst-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-03 22:29:15.000000 Data_Cdvst-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/
+drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.928600 Data_Cdvst-1.1/Data_Cdvst/
+-rw-rw-rw-   0        0        0        0 2023-04-08 11:10:24.000000 Data_Cdvst-1.1/Data_Cdvst/Files_Cdvst.py
+-rw-rw-rw-   0        0        0     9532 2023-04-08 12:16:08.000000 Data_Cdvst-1.1/Data_Cdvst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/Data_Cdvst.egg-info/
+-rw-rw-rw-   0        0        0     1385 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 18:27:00.000000 Data_Cdvst-1.1/Data_Cdvst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1385 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:27:00.951753 Data_Cdvst-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-08 12:19:19.000000 Data_Cdvst-1.1/setup.py
```

### Comparing `Data_Cdvst-1.0/Data_Cdvst/__init__.py` & `Data_Cdvst-1.1/Data_Cdvst/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sqlite3
 from contextlib import contextmanager
 from sqlite3 import Error
 import time
+from import Files_Cdvst import *
 
 class Database:
     """
     Eine Singleton-Klasse zum Verwalten von SQLite-Datenbanken.
 
     Beispiel:
 
@@ -234,14 +235,63 @@
         Schließt die Verbindung zur Datenbank.
 
         """
         if self.conn:
             self.conn.close()
 
 
+
+class ConfigManager:
+    import json
+    import os
+    CONFIG_FILE_PATH = os.path.join(os.path.dirname(__file__), "config.json")
+    DEFAULT_API_KEY = "INSERT_YOUR_API_KEY_HERE"
+
+    @classmethod
+    def load_config(cls):
+        if not os.path.isfile(cls.CONFIG_FILE_PATH):
+            cls.save_config(cls.DEFAULT_API_KEY)
+        with open(cls.CONFIG_FILE_PATH, "r") as f:
+            config = json.load(f)
+        return config
+
+    @classmethod
+    def save_config(cls, api_key):
+        config = {"api_key": api_key}
+        with open(cls.CONFIG_FILE_PATH, "w") as f:
+            json.dump(config, f)
+
+class FavoritesManager:
+    import json
+    import os
+    FAVORITES_FILE_PATH = os.path.join(os.path.dirname(__file__), "favorites.json")
+    DEFAULT_CATEGORIES = {
+        "Category 1": [
+            "Prompt 1",
+            "Prompt 2"
+        ],
+        "Category 2": [
+            "Prompt 3",
+            "Prompt 4"
+        ]
+    }
+
+    @classmethod
+    def load_favorites(cls):
+        if not os.path.isfile(cls.FAVORITES_FILE_PATH):
+            cls.save_favorites(cls.DEFAULT_CATEGORIES)
+        with open(cls.FAVORITES_FILE_PATH, "r") as f:
+            favorites = json.load(f)
+        return favorites
+
+    @classmethod
+    def save_favorites(cls, favorites):
+        with open(cls.FAVORITES_FILE_PATH, "w") as f:
+            json.dump(favorites, f)
+
 if __name__ == "__main__":
     # Beispiel:
     db_path = "example.db"
     db = Database(db_path)
     db.create_table()
     db.add_entry(name="Module Name", description="Description", version="0.1", dirpath=r"F:\users\cdvst\OneDrive\Desktop\Pypi Module\ModuleName")
     entry = db.get_entry(ID=1)
```

### Comparing `Data_Cdvst-1.0/Data_Cdvst.egg-info/PKG-INFO` & `Data_Cdvst-1.1/Data_Cdvst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data-Cdvst
-Version: 1.0
+Version: 1.1
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.0/PKG-INFO` & `Data_Cdvst-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data_Cdvst
-Version: 1.0
+Version: 1.1
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.0/README.md` & `Data_Cdvst-1.1/README.md`

 * *Files identical despite different names*

### Comparing `Data_Cdvst-1.0/setup.py` & `Data_Cdvst-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Data_Cdvst',
-    version='1.0',
+    version='1.1',
     description='Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.',
     long_description="""Data_Cdvst ist eine Python-Bibliothek zur einfachen nutzung von Datenbanken undeinfachen umgang mit datenverarbeitugn und -aufnahme. Die Bibliothek bietet Funktionen zum Abspielen von WAV- und MP3-Dateien sowie zur Aufnahme von Audio in einer WAV-Datei. Die Bibliothek umfasst auch eine automatische Spracherkennungsfunktion.
 
 Funktionen:
 - Einfache Datenbank erstellung
 - Einfache Datenbanken Einträge erzeugen
 - Einfahce Datenbanken auslesen
```

