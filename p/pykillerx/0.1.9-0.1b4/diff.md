# Comparing `tmp/pykillerx-0.1.9.tar.gz` & `tmp/pykillerx-0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykillerx-0.1.9.tar", last modified: Wed Jan 18 07:13:45 2023, max compression
+gzip compressed data, was "pykillerx-0.1b4.tar", last modified: Thu Jan 12 11:01:21 2023, max compression
```

## Comparing `pykillerx-0.1.9.tar` & `pykillerx-0.1b4.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-01-18 07:12:32.000000 pykillerx-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-18 07:12:32.000000 pykillerx-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-18 07:13:45.182834 pykillerx-0.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      469 2023-01-18 07:12:32.000000 pykillerx-0.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/blacklist/
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/blacklist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/blacklist/support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/button/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/button/__init__.py
--rw-r--r--   0 root         (0) root         (0)      133 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/button/button.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/extra/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/extra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/extra/hosted.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/help/
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/help/help.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx/helper/
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/basic.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/data.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/goblok.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/hacking.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/inline.py
--rw-r--r--   0 root         (0) root         (0)      299 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/rendy.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/repo.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-01-18 07:12:32.000000 pykillerx-0.1.9/pykillerx/helper/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 07:13:45.182834 pykillerx-0.1.9/pykillerx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-18 07:13:45.000000 pykillerx-0.1.9/pykillerx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-01-18 07:13:45.000000 pykillerx-0.1.9/pykillerx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 07:13:45.000000 pykillerx-0.1.9/pykillerx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-18 07:13:45.000000 pykillerx-0.1.9/pykillerx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-18 07:13:45.000000 pykillerx-0.1.9/pykillerx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 07:13:45.182834 pykillerx-0.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2930 2023-01-18 07:12:32.000000 pykillerx-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.957553 pykillerx-0.1b4/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-01-12 11:00:45.000000 pykillerx-0.1b4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       26 2023-01-12 11:00:45.000000 pykillerx-0.1b4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-01-12 11:01:21.957553 pykillerx-0.1b4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      469 2023-01-12 11:00:45.000000 pykillerx-0.1b4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx/blacklist/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/blacklist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/blacklist/support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx/button/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/button/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      133 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/button/button.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx/extra/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/extra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/extra/hosted.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx/help/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/help/help.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.957553 pykillerx-0.1b4/pykillerx/helper/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/basic.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/goblok.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/inline.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/rendy.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-01-12 11:00:45.000000 pykillerx-0.1b4/pykillerx/helper/repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-12 11:01:21.953554 pykillerx-0.1b4/pykillerx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-01-12 11:01:21.000000 pykillerx-0.1b4/pykillerx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      607 2023-01-12 11:01:21.000000 pykillerx-0.1b4/pykillerx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-12 11:01:21.000000 pykillerx-0.1b4/pykillerx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-01-12 11:01:21.000000 pykillerx-0.1b4/pykillerx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-01-12 11:01:21.000000 pykillerx-0.1b4/pykillerx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-12 11:01:21.957553 pykillerx-0.1b4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-01-12 11:00:45.000000 pykillerx-0.1b4/setup.py
```

### Comparing `pykillerx-0.1.9/LICENSE` & `pykillerx-0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/PKG-INFO` & `pykillerx-0.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykillerx
-Version: 0.1.9
+Version: 0.1b4
 Summary: KillerX Userbot Pyrogram
 Home-page: https://github.com/TeamKillerX/KillerX-Base
 Author: TeamKillerX
 Author-email: killerx@randydev.my.id
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pykillerx-0.1.9/pykillerx/blacklist/support.py` & `pykillerx-0.1b4/pykillerx/blacklist/support.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx/extra/hosted.py` & `pykillerx-0.1b4/pykillerx/extra/hosted.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx/help/help.py` & `pykillerx-0.1b4/pykillerx/help/help.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx/helper/basic.py` & `pykillerx-0.1b4/pykillerx/helper/basic.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx/helper/goblok.py` & `pykillerx-0.1b4/pykillerx/helper/goblok.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # LU MAU BOKEP GAK ? 🤣
 
-from pyrogram import *
-from pyrogram import Client
-from pyrogram.types import *
-
 bokep = "https://t.me/+R-oIEJKFZ0pkYzgx"
 bocil = ""
 tiktok = ""
 kontol = "kangcopybot"
 
 ANAK_KONTOL = kontol
 ANAK_ANJING = bokep
 
-
+# 
 absen = [
     "**Hadir bang** 😁",
     "**Hadir kak** 😉",
     "**Hadir dong** 😁",
     "**Hadir ganteng** 🥵",
     "**Hadir bro** 😎",
     "**Hadir dick** 🤣",
     "**Hadir kak maap telat** 🥺",
 ]
 
-def hacking():
-    hacking = message.reply_text
-
 blockyou = 1447438514
 
 """
 JANGAN HAPUS DEV && GUA GBAN LU KONTOL
 CREDITS @XTSEA
 """
 memek = [
```

### Comparing `pykillerx-0.1.9/pykillerx/helper/inline.py` & `pykillerx-0.1b4/pykillerx/helper/inline.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx/helper/repo.py` & `pykillerx-0.1b4/pykillerx/helper/repo.py`

 * *Files identical despite different names*

### Comparing `pykillerx-0.1.9/pykillerx.egg-info/PKG-INFO` & `pykillerx-0.1b4/pykillerx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykillerx
-Version: 0.1.9
+Version: 0.1b4
 Summary: KillerX Userbot Pyrogram
 Home-page: https://github.com/TeamKillerX/KillerX-Base
 Author: TeamKillerX
 Author-email: killerx@randydev.my.id
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pykillerx-0.1.9/pykillerx.egg-info/SOURCES.txt` & `pykillerx-0.1b4/pykillerx.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,11 @@
 pykillerx/button/button.py
 pykillerx/extra/__init__.py
 pykillerx/extra/hosted.py
 pykillerx/help/__init__.py
 pykillerx/help/help.py
 pykillerx/helper/__init__.py
 pykillerx/helper/basic.py
-pykillerx/helper/data.py
 pykillerx/helper/goblok.py
-pykillerx/helper/hacking.py
 pykillerx/helper/inline.py
 pykillerx/helper/rendy.py
-pykillerx/helper/repo.py
-pykillerx/helper/tools.py
+pykillerx/helper/repo.py
```

### Comparing `pykillerx-0.1.9/setup.py` & `pykillerx-0.1b4/setup.py`

 * *Files identical despite different names*

