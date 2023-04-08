# Comparing `tmp/almapiwrapper-0.8.6.tar.gz` & `tmp/almapiwrapper-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almapiwrapper-0.8.6.tar", last modified: Mon Nov  7 14:43:35 2022, max compression
+gzip compressed data, was "almapiwrapper-0.9.0.tar", last modified: Tue Nov 22 21:36:37 2022, max compression
```

## Comparing `almapiwrapper-0.8.6.tar` & `almapiwrapper-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.421255 almapiwrapper-0.8.6/
--rw-rw-rw-   0        0        0     1194 2022-11-07 14:43:35.420754 almapiwrapper-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      601 2022-11-07 14:43:04.000000 almapiwrapper-0.8.6/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.232732 almapiwrapper-0.8.6/almapiwrapper/
--rw-rw-rw-   0        0        0       99 2022-08-22 12:37:35.000000 almapiwrapper-0.8.6/almapiwrapper/__init__.py
--rw-rw-rw-   0        0        0     2671 2022-08-29 19:46:38.000000 almapiwrapper-0.8.6/almapiwrapper/apikeys.py
--rw-rw-rw-   0        0        0      832 2022-06-24 23:16:52.000000 almapiwrapper-0.8.6/almapiwrapper/configlog.py
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.309174 almapiwrapper-0.8.6/almapiwrapper/inventory/
--rw-rw-rw-   0        0        0      100 2022-09-05 10:07:10.000000 almapiwrapper-0.8.6/almapiwrapper/inventory/__init__.py
--rw-rw-rw-   0        0        0    16881 2022-09-12 09:05:07.000000 almapiwrapper-0.8.6/almapiwrapper/inventory/bib.py
--rw-rw-rw-   0        0        0    13722 2022-10-18 13:59:54.000000 almapiwrapper-0.8.6/almapiwrapper/inventory/holding.py
--rw-rw-rw-   0        0        0    15549 2022-09-14 08:50:03.000000 almapiwrapper-0.8.6/almapiwrapper/inventory/item.py
--rw-rw-rw-   0        0        0    12627 2022-09-14 08:48:25.000000 almapiwrapper-0.8.6/almapiwrapper/record.py
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.372584 almapiwrapper-0.8.6/almapiwrapper/users/
--rw-rw-rw-   0        0        0      124 2022-10-04 17:27:12.000000 almapiwrapper-0.8.6/almapiwrapper/users/__init__.py
--rw-rw-rw-   0        0        0     6439 2022-10-18 13:29:58.000000 almapiwrapper-0.8.6/almapiwrapper/users/fee.py
--rw-rw-rw-   0        0        0    11445 2022-11-07 12:49:08.000000 almapiwrapper-0.8.6/almapiwrapper/users/user.py
--rw-rw-rw-   0        0        0     4985 2022-11-07 12:34:59.000000 almapiwrapper-0.8.6/almapiwrapper/users/utils.py
--rw-rw-rw-   0        0        0       23 2022-11-07 12:43:15.000000 almapiwrapper-0.8.6/almapiwrapper/version.py
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.255190 almapiwrapper-0.8.6/almapiwrapper.egg-info/
--rw-rw-rw-   0        0        0     1194 2022-11-07 14:43:35.000000 almapiwrapper-0.8.6/almapiwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2022-11-07 14:43:35.000000 almapiwrapper-0.8.6/almapiwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 14:43:35.000000 almapiwrapper-0.8.6/almapiwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-11-07 14:43:35.000000 almapiwrapper-0.8.6/almapiwrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-06-21 19:29:40.000000 almapiwrapper-0.8.6/licence.txt
--rw-rw-rw-   0        0        0      584 2022-11-07 14:43:04.000000 almapiwrapper-0.8.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-07 14:43:35.421255 almapiwrapper-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      528 2022-11-07 14:38:31.000000 almapiwrapper-0.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-07 14:43:35.419116 almapiwrapper-0.8.6/test/
--rw-rw-rw-   0        0        0        0 2022-06-18 17:18:02.000000 almapiwrapper-0.8.6/test/__init__.py
--rw-rw-rw-   0        0        0    11264 2022-10-18 14:03:04.000000 almapiwrapper-0.8.6/test/test_bib.py
--rw-rw-rw-   0        0        0     1433 2022-10-04 17:27:12.000000 almapiwrapper-0.8.6/test/test_fee.py
--rw-rw-rw-   0        0        0     1364 2022-10-04 17:27:12.000000 almapiwrapper-0.8.6/test/test_fetchusers.py
--rw-rw-rw-   0        0        0     3432 2022-07-15 13:02:20.000000 almapiwrapper-0.8.6/test/test_user.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.849223 almapiwrapper-0.9.0/
+-rw-rw-rw-   0        0        0     1195 2022-11-22 21:36:37.849223 almapiwrapper-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2022-11-22 21:35:56.000000 almapiwrapper-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.629928 almapiwrapper-0.9.0/almapiwrapper/
+-rw-rw-rw-   0        0        0       99 2022-08-22 12:37:35.000000 almapiwrapper-0.9.0/almapiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     2671 2022-08-29 19:46:38.000000 almapiwrapper-0.9.0/almapiwrapper/apikeys.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.691946 almapiwrapper-0.9.0/almapiwrapper/config/
+-rw-rw-rw-   0        0        0       28 2022-11-22 21:19:23.000000 almapiwrapper-0.9.0/almapiwrapper/config/__init__.py
+-rw-rw-rw-   0        0        0     4229 2022-11-22 21:19:23.000000 almapiwrapper-0.9.0/almapiwrapper/config/recset.py
+-rw-rw-rw-   0        0        0      832 2022-06-24 23:16:52.000000 almapiwrapper-0.9.0/almapiwrapper/configlog.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.724360 almapiwrapper-0.9.0/almapiwrapper/inventory/
+-rw-rw-rw-   0        0        0      100 2022-09-05 10:07:10.000000 almapiwrapper-0.9.0/almapiwrapper/inventory/__init__.py
+-rw-rw-rw-   0        0        0    16881 2022-09-12 09:05:07.000000 almapiwrapper-0.9.0/almapiwrapper/inventory/bib.py
+-rw-rw-rw-   0        0        0    13722 2022-11-22 21:18:48.000000 almapiwrapper-0.9.0/almapiwrapper/inventory/holding.py
+-rw-rw-rw-   0        0        0    15549 2022-09-14 08:50:03.000000 almapiwrapper-0.9.0/almapiwrapper/inventory/item.py
+-rw-rw-rw-   0        0        0    12627 2022-09-14 08:48:25.000000 almapiwrapper-0.9.0/almapiwrapper/record.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.756280 almapiwrapper-0.9.0/almapiwrapper/users/
+-rw-rw-rw-   0        0        0      124 2022-10-04 17:27:12.000000 almapiwrapper-0.9.0/almapiwrapper/users/__init__.py
+-rw-rw-rw-   0        0        0     6417 2022-11-22 21:19:23.000000 almapiwrapper-0.9.0/almapiwrapper/users/fee.py
+-rw-rw-rw-   0        0        0    11445 2022-11-22 21:18:48.000000 almapiwrapper-0.9.0/almapiwrapper/users/user.py
+-rw-rw-rw-   0        0        0     4985 2022-11-22 21:18:48.000000 almapiwrapper-0.9.0/almapiwrapper/users/utils.py
+-rw-rw-rw-   0        0        0       23 2022-11-22 21:24:11.000000 almapiwrapper-0.9.0/almapiwrapper/version.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.676209 almapiwrapper-0.9.0/almapiwrapper.egg-info/
+-rw-rw-rw-   0        0        0     1195 2022-11-22 21:36:37.000000 almapiwrapper-0.9.0/almapiwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2022-11-22 21:36:37.000000 almapiwrapper-0.9.0/almapiwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-22 21:36:37.000000 almapiwrapper-0.9.0/almapiwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2022-11-22 21:36:37.000000 almapiwrapper-0.9.0/almapiwrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-06-21 19:29:40.000000 almapiwrapper-0.9.0/licence.txt
+-rw-rw-rw-   0        0        0      585 2022-11-22 21:35:56.000000 almapiwrapper-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-11-22 21:36:37.849223 almapiwrapper-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      528 2022-11-22 21:18:48.000000 almapiwrapper-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-22 21:36:37.849223 almapiwrapper-0.9.0/test/
+-rw-rw-rw-   0        0        0        0 2022-06-18 17:18:02.000000 almapiwrapper-0.9.0/test/__init__.py
+-rw-rw-rw-   0        0        0    11264 2022-11-22 21:18:48.000000 almapiwrapper-0.9.0/test/test_bib.py
+-rw-rw-rw-   0        0        0     1236 2022-11-22 21:19:23.000000 almapiwrapper-0.9.0/test/test_config.py
+-rw-rw-rw-   0        0        0     1433 2022-10-04 17:27:12.000000 almapiwrapper-0.9.0/test/test_fee.py
+-rw-rw-rw-   0        0        0     1364 2022-10-04 17:27:12.000000 almapiwrapper-0.9.0/test/test_fetchusers.py
+-rw-rw-rw-   0        0        0     3432 2022-07-15 13:02:20.000000 almapiwrapper-0.9.0/test/test_user.py
```

### Comparing `almapiwrapper-0.8.6/PKG-INFO` & `almapiwrapper-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: almapiwrapper
-Version: 0.8.6
+Version: 0.9.0
 Summary: This python module is a tool to use Alma APIs. it manages the logs and the backup of the records.
-Author-email: Raphael Rey <raphael.rey@slsp.ch>
+Author-email: Raphaël Rey <raphael.rey@slsp.ch>
 Project-URL: Homepage, https://github.com/Swiss-Library-Service-Platform/almapiwrapper
 Project-URL: Bug Tracker, https://github.com/Swiss-Library-Service-Platform/almapiwrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: licence.txt
@@ -16,14 +16,14 @@
 **********************************
 
 This python module is a tool to use Alma APIs. it manages the logs and the
 backup of the records.
 
 * Author: Raphaël Rey (raphael.rey@slsp.ch)
 * Year: 2022
-* Version: 0.8.6
+* Version: 0.9.0
 * License: GNU General Public License v3.0
 * `Documentation <https://almapi-wrapper.readthedocs.io/en/latest/>`_
 
 .. |doc| image:: https://readthedocs.org/projects/almapi-wrapper/badge/?version=latest
     :target: https://almapi-wrapper.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `almapiwrapper-0.8.6/README.rst` & `almapiwrapper-0.9.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 **********************************
 
 This python module is a tool to use Alma APIs. it manages the logs and the
 backup of the records.
 
 * Author: Raphaël Rey (raphael.rey@slsp.ch)
 * Year: 2022
-* Version: 0.8.6
+* Version: 0.9.0
 * License: GNU General Public License v3.0
 * `Documentation <https://almapi-wrapper.readthedocs.io/en/latest/>`_
 
 .. |doc| image:: https://readthedocs.org/projects/almapi-wrapper/badge/?version=latest
     :target: https://almapi-wrapper.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `almapiwrapper-0.8.6/almapiwrapper/apikeys.py` & `almapiwrapper-0.9.0/almapiwrapper/apikeys.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/configlog.py` & `almapiwrapper-0.9.0/almapiwrapper/configlog.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/inventory/bib.py` & `almapiwrapper-0.9.0/almapiwrapper/inventory/bib.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/inventory/holding.py` & `almapiwrapper-0.9.0/almapiwrapper/inventory/holding.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/inventory/item.py` & `almapiwrapper-0.9.0/almapiwrapper/inventory/item.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/record.py` & `almapiwrapper-0.9.0/almapiwrapper/record.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/users/fee.py` & `almapiwrapper-0.9.0/almapiwrapper/users/fee.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class Fee(Record):
     """Class representing a Users fee
 
     :cvar api_base_url_users: url of the user api
     :ivar fee_id: id of the fee
     :ivar primary_id: primary_id of the user
-    :ivar zone: initial value: zone where the user should be created
+    :ivar zone: initial value: zone of the fee
     :ivar env: initial value: environment of the entity: 'P' for production and 'S' for sandbox
     :ivar user: :class:`almapiwrapper.users.User` either primary_id of the user or the user itself must be provided
     :ivar data: :class:`almapiwrapper.record.JsonData` with fee data"""
 
     api_base_url_users: ClassVar[str] = 'https://api-eu.hosted.exlibrisgroup.com/almaws/v1/users'
 
     def __init__(self,
```

### Comparing `almapiwrapper-0.8.6/almapiwrapper/users/user.py` & `almapiwrapper-0.9.0/almapiwrapper/users/user.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper/users/utils.py` & `almapiwrapper-0.9.0/almapiwrapper/users/utils.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/almapiwrapper.egg-info/PKG-INFO` & `almapiwrapper-0.9.0/almapiwrapper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: almapiwrapper
-Version: 0.8.6
+Version: 0.9.0
 Summary: This python module is a tool to use Alma APIs. it manages the logs and the backup of the records.
-Author-email: Raphael Rey <raphael.rey@slsp.ch>
+Author-email: Raphaël Rey <raphael.rey@slsp.ch>
 Project-URL: Homepage, https://github.com/Swiss-Library-Service-Platform/almapiwrapper
 Project-URL: Bug Tracker, https://github.com/Swiss-Library-Service-Platform/almapiwrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: licence.txt
@@ -16,14 +16,14 @@
 **********************************
 
 This python module is a tool to use Alma APIs. it manages the logs and the
 backup of the records.
 
 * Author: Raphaël Rey (raphael.rey@slsp.ch)
 * Year: 2022
-* Version: 0.8.6
+* Version: 0.9.0
 * License: GNU General Public License v3.0
 * `Documentation <https://almapi-wrapper.readthedocs.io/en/latest/>`_
 
 .. |doc| image:: https://readthedocs.org/projects/almapi-wrapper/badge/?version=latest
     :target: https://almapi-wrapper.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `almapiwrapper-0.8.6/almapiwrapper.egg-info/SOURCES.txt` & `almapiwrapper-0.9.0/almapiwrapper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 almapiwrapper/configlog.py
 almapiwrapper/record.py
 almapiwrapper/version.py
 almapiwrapper.egg-info/PKG-INFO
 almapiwrapper.egg-info/SOURCES.txt
 almapiwrapper.egg-info/dependency_links.txt
 almapiwrapper.egg-info/top_level.txt
+almapiwrapper/config/__init__.py
+almapiwrapper/config/recset.py
 almapiwrapper/inventory/__init__.py
 almapiwrapper/inventory/bib.py
 almapiwrapper/inventory/holding.py
 almapiwrapper/inventory/item.py
 almapiwrapper/users/__init__.py
 almapiwrapper/users/fee.py
 almapiwrapper/users/user.py
 almapiwrapper/users/utils.py
 test/__init__.py
 test/test_bib.py
+test/test_config.py
 test/test_fee.py
 test/test_fetchusers.py
 test/test_user.py
```

### Comparing `almapiwrapper-0.8.6/licence.txt` & `almapiwrapper-0.9.0/licence.txt`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/pyproject.toml` & `almapiwrapper-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "almapiwrapper"
-version = "0.8.6"
+version = "0.9.0"
 authors = [
-  { name="Raphael Rey", email="raphael.rey@slsp.ch" },
+  { name="Raphaël Rey", email="raphael.rey@slsp.ch" },
 ]
 description = "This python module is a tool to use Alma APIs. it manages the logs and the backup of the records."
 readme = "readme.rst"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `almapiwrapper-0.8.6/setup.py` & `almapiwrapper-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/test/test_bib.py` & `almapiwrapper-0.9.0/test/test_bib.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/test/test_fee.py` & `almapiwrapper-0.9.0/test/test_fee.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/test/test_fetchusers.py` & `almapiwrapper-0.9.0/test/test_fetchusers.py`

 * *Files identical despite different names*

### Comparing `almapiwrapper-0.8.6/test/test_user.py` & `almapiwrapper-0.9.0/test/test_user.py`

 * *Files identical despite different names*

