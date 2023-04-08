# Comparing `tmp/SelSik-0.2.9.tar.gz` & `tmp/SelSik-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SelSik-0.2.9.tar", last modified: Sat Apr  8 19:02:45 2023, max compression
+gzip compressed data, was "SelSik-0.3.0.tar", last modified: Sat Apr  8 19:07:25 2023, max compression
```

## Comparing `SelSik-0.2.9.tar` & `SelSik-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:02:45.688304 SelSik-0.2.9/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-04-08 19:00:19.000000 SelSik-0.2.9/LICENSE
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       26 2023-04-08 19:00:19.000000 SelSik-0.2.9/MANIFEST.in
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2761 2023-04-08 19:02:45.688304 SelSik-0.2.9/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2215 2023-04-08 19:00:19.000000 SelSik-0.2.9/README.md
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:02:45.688304 SelSik-0.2.9/SelSik/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    12999 2023-04-08 19:01:22.000000 SelSik-0.2.9/SelSik/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:02:45.688304 SelSik-0.2.9/SelSik.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2761 2023-04-08 19:02:45.000000 SelSik-0.2.9/SelSik.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      206 2023-04-08 19:02:45.000000 SelSik-0.2.9/SelSik.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-04-08 19:02:45.000000 SelSik-0.2.9/SelSik.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       68 2023-04-08 19:02:45.000000 SelSik-0.2.9/SelSik.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        7 2023-04-08 19:02:45.000000 SelSik-0.2.9/SelSik.egg-info/top_level.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-04-08 19:02:45.688304 SelSik-0.2.9/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1207 2023-04-08 19:02:26.000000 SelSik-0.2.9/setup.py
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:07:25.207165 SelSik-0.3.0/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-04-08 19:00:19.000000 SelSik-0.3.0/LICENSE
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       26 2023-04-08 19:00:19.000000 SelSik-0.3.0/MANIFEST.in
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2761 2023-04-08 19:07:25.207165 SelSik-0.3.0/PKG-INFO
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2215 2023-04-08 19:00:19.000000 SelSik-0.3.0/README.md
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:07:25.207165 SelSik-0.3.0/SelSik/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    13055 2023-04-08 19:07:07.000000 SelSik-0.3.0/SelSik/__init__.py
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-04-08 19:07:25.207165 SelSik-0.3.0/SelSik.egg-info/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2761 2023-04-08 19:07:25.000000 SelSik-0.3.0/SelSik.egg-info/PKG-INFO
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      206 2023-04-08 19:07:25.000000 SelSik-0.3.0/SelSik.egg-info/SOURCES.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-04-08 19:07:25.000000 SelSik-0.3.0/SelSik.egg-info/dependency_links.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       68 2023-04-08 19:07:25.000000 SelSik-0.3.0/SelSik.egg-info/requires.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        7 2023-04-08 19:07:25.000000 SelSik-0.3.0/SelSik.egg-info/top_level.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-04-08 19:07:25.207165 SelSik-0.3.0/setup.cfg
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1207 2023-04-08 19:07:18.000000 SelSik-0.3.0/setup.py
```

### Comparing `SelSik-0.2.9/LICENSE` & `SelSik-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SelSik-0.2.9/PKG-INFO` & `SelSik-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelSik
-Version: 0.2.9
+Version: 0.3.0
 Summary: @KekikAkademi Selenium Kütüphanesi
 Home-page: https://github.com/keyiflerolsun/SelSik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: SelSik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SelSik Version: 0.2.9 Summary: @KekikAkademi
+Metadata-Version: 2.1 Name: SelSik Version: 0.3.0 Summary: @KekikAkademi
 Selenium KÃ¼tÃ¼phanesi Home-page: https://github.com/keyiflerolsun/SelSik
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: SelSik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5
 - Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://www.akashtrehan.com/assets/images/emoji/terminal.png] SelSik
```

### Comparing `SelSik-0.2.9/README.md` & `SelSik-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SelSik-0.2.9/SelSik/__init__.py` & `SelSik-0.3.0/SelSik/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,23 @@
             self.tarayici.execute_cdp_cmd(
                 "Storage.clearDataForOrigin", {
                     "origin"       : "*",
                     "storageTypes" : "all",
                 }
             )
 
-        if self.remote:
-            with suppress(Exception):
-                return self.tarayici.quit()
-
         with suppress(Exception):
             self.tarayici.close()
 
+        with suppress(Exception):
+            self.tarayici.execute_script("window.close();")
+
+        with suppress(Exception):
+            self.tarayici.quit()
+
         if _sistem != "nt":
             with suppress(Exception):
                 Popen("rm -rf /tmp/.com.google.Chrome.*", shell=True)
 
     def __init__(
         self,
         link:str,
```

### Comparing `SelSik-0.2.9/SelSik.egg-info/PKG-INFO` & `SelSik-0.3.0/SelSik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SelSik
-Version: 0.2.9
+Version: 0.3.0
 Summary: @KekikAkademi Selenium Kütüphanesi
 Home-page: https://github.com/keyiflerolsun/SelSik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: SelSik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SelSik Version: 0.2.9 Summary: @KekikAkademi
+Metadata-Version: 2.1 Name: SelSik Version: 0.3.0 Summary: @KekikAkademi
 Selenium KÃ¼tÃ¼phanesi Home-page: https://github.com/keyiflerolsun/SelSik
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: SelSik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5
 - Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://www.akashtrehan.com/assets/images/emoji/terminal.png] SelSik
```

### Comparing `SelSik-0.2.9/setup.py` & `SelSik-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "SelSik",
-    version      = "0.2.9",
+    version      = "0.3.0",
     url          = "https://github.com/keyiflerolsun/SelSik",
     description  = "@KekikAkademi Selenium Kütüphanesi",
     keywords     = ["SelSik", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

