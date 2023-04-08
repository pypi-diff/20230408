# Comparing `tmp/moonglaive-0.0.5.tar.gz` & `tmp/moonglaive-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moonglaive-0.0.5.tar", last modified: Sat Apr  8 16:45:26 2023, max compression
+gzip compressed data, was "dist/moonglaive-0.0.6.tar", last modified: Sat Apr  8 16:47:41 2023, max compression
```

## Comparing `moonglaive-0.0.5.tar` & `moonglaive-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:45:26.000000 moonglaive-0.0.5/
--rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:45:26.000000 moonglaive-0.0.5/PKG-INFO
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/
--rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      433 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)       89 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       11 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)     1074 2023-02-23 18:06:50.000000 moonglaive-0.0.5/LICENSE
--rw-r--r--   0 user       (502) staff       (20)       60 2023-02-23 18:06:50.000000 moonglaive-0.0.5/README.md
--rw-r--r--   0 user       (502) staff       (20)     1011 2023-04-08 16:44:58.000000 moonglaive-0.0.5/setup.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive/
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive/platforms/
--rw-r--r--   0 user       (502) staff       (20)      909 2023-04-08 16:45:08.000000 moonglaive-0.0.5/moonglaive/platforms/sherlock.py
--rw-r--r--   0 user       (502) staff       (20)     1223 2023-04-08 16:45:06.000000 moonglaive-0.0.5/moonglaive/platforms/code4rena.py
--rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:28.000000 moonglaive-0.0.5/moonglaive/platforms/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4039 2023-04-08 16:45:02.000000 moonglaive-0.0.5/moonglaive/platforms/base.py
--rwxr-xr-x   0 user       (502) staff       (20)      158 2023-04-08 16:21:54.000000 moonglaive-0.0.5/moonglaive/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)     1480 2023-04-08 16:45:19.000000 moonglaive-0.0.5/moonglaive/__main__.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:45:26.000000 moonglaive-0.0.5/moonglaive/services/
--rw-r--r--   0 user       (502) staff       (20)     1446 2023-03-04 05:16:49.000000 moonglaive-0.0.5/moonglaive/services/discord.py
--rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:32.000000 moonglaive-0.0.5/moonglaive/services/__init__.py
--rw-r--r--   0 user       (502) staff       (20)       38 2023-04-08 16:45:26.000000 moonglaive-0.0.5/setup.cfg
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/
+-rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:47:41.000000 moonglaive-0.0.6/PKG-INFO
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      433 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)       89 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       11 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)     1074 2023-02-23 18:06:50.000000 moonglaive-0.0.6/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)       60 2023-02-23 18:06:50.000000 moonglaive-0.0.6/README.md
+-rw-r--r--   0 user       (502) staff       (20)     1011 2023-04-08 16:47:32.000000 moonglaive-0.0.6/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/platforms/
+-rw-r--r--   0 user       (502) staff       (20)      920 2023-04-08 16:47:25.000000 moonglaive-0.0.6/moonglaive/platforms/sherlock.py
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-08 16:47:24.000000 moonglaive-0.0.6/moonglaive/platforms/code4rena.py
+-rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:28.000000 moonglaive-0.0.6/moonglaive/platforms/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4050 2023-04-08 16:47:28.000000 moonglaive-0.0.6/moonglaive/platforms/base.py
+-rwxr-xr-x   0 user       (502) staff       (20)      158 2023-04-08 16:21:54.000000 moonglaive-0.0.6/moonglaive/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)     1502 2023-04-08 16:47:21.000000 moonglaive-0.0.6/moonglaive/__main__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/services/
+-rw-r--r--   0 user       (502) staff       (20)     1446 2023-03-04 05:16:49.000000 moonglaive-0.0.6/moonglaive/services/discord.py
+-rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:32.000000 moonglaive-0.0.6/moonglaive/services/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-04-08 16:47:41.000000 moonglaive-0.0.6/setup.cfg
```

### Comparing `moonglaive-0.0.5/PKG-INFO` & `moonglaive-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: moonglaive
-Version: 0.0.5
+Version: 0.0.6
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `moonglaive-0.0.5/moonglaive.egg-info/PKG-INFO` & `moonglaive-0.0.6/moonglaive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: moonglaive
-Version: 0.0.5
+Version: 0.0.6
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `moonglaive-0.0.5/LICENSE` & `moonglaive-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.5/setup.py` & `moonglaive-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moonglaive',
-    version='0.0.5',
+    version='0.0.6',
     description='Three-bladed weapon of the night elf Sentinels',
     url='https://github.com/MalfurionWhitehat/moonglaive',
     author='MalfurionWhitehat',
     author_email='MalfurionWhitehat@proton.me',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `moonglaive-0.0.5/moonglaive/platforms/sherlock.py` & `moonglaive-0.0.6/moonglaive/platforms/sherlock.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 import requests
 
-from platforms.base import Base
+from moonglaive.platforms.base import Base
 
 
 class Sherlock(Base):
     discord_guild_id = '812037309376495636'
 
     def __init__(self, discord_authorization: str):
         super().__init__(discord_authorization)
```

### Comparing `moonglaive-0.0.5/moonglaive/platforms/code4rena.py` & `moonglaive-0.0.6/moonglaive/platforms/code4rena.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List
 import requests
 from dateutil import parser as date
 from re import sub
 from decimal import Decimal
 
-from platforms.base import Base
+from moonglaive.platforms.base import Base
 
 
 class Code4rena(Base):
     discord_guild_id = '810916927919620096'
 
     def __init__(self, discord_authorization: str):
         super().__init__(discord_authorization)
```

### Comparing `moonglaive-0.0.5/moonglaive/platforms/base.py` & `moonglaive-0.0.6/moonglaive/platforms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import Dict
 from datetime import datetime
 from fuzzywuzzy import fuzz
 
-from services.discord import Channel, Discord
+from moonglaive.services.discord import Channel, Discord
 
 
 class Base():
     discord_guild_id = None
     discord = None
     channels = []
```

### Comparing `moonglaive-0.0.5/moonglaive/__main__.py` & `moonglaive-0.0.6/moonglaive/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from tabulate import tabulate
 
-from platforms.code4rena import Code4rena
-from platforms.sherlock import Sherlock
+from moonglaive.platforms.code4rena import Code4rena
+from moonglaive.platforms.sherlock import Sherlock
 
 parser = argparse.ArgumentParser(
     description='Three-bladed weapon of the night elf Sentinels.')
 parser.add_argument('--active', help='Active audit contests',
                     action=argparse.BooleanOptionalAction)
 parser.add_argument('--upcoming', help='Upcoming audit contests',
                     action=argparse.BooleanOptionalAction)
```

### Comparing `moonglaive-0.0.5/moonglaive/services/discord.py` & `moonglaive-0.0.6/moonglaive/services/discord.py`

 * *Files identical despite different names*

