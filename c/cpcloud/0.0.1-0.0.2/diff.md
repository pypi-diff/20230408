# Comparing `tmp/cpcloud-0.0.1-py3-none-any.whl.zip` & `tmp/cpcloud-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6988 bytes, number of entries: 7
--rwxr-xr-x  2.0 unx     7838 b- defN 23-Apr-08 16:50 cpcloud-0.0.1.data/scripts/cpcloud
--rwxr-xr-x  2.0 unx     7838 b- defN 23-Apr-08 16:50 cpcloud-0.0.1.data/scripts/cpcloud.py
--rw-r--r--  2.0 unx     1077 b- defN 23-Apr-08 17:31 cpcloud-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      574 b- defN 23-Apr-08 17:31 cpcloud-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 17:31 cpcloud-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-08 17:31 cpcloud-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 23-Apr-08 17:31 cpcloud-0.0.1.dist-info/RECORD
-7 files, 17989 bytes uncompressed, 5974 bytes compressed:  66.8%
+Zip file size: 6967 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx     7809 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.data/scripts/cpcloud
+-rwxr-xr-x  2.0 unx     7809 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.data/scripts/cpcloud.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      574 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      569 b- defN 23-Apr-08 17:34 cpcloud-0.0.2.dist-info/RECORD
+7 files, 17931 bytes uncompressed, 5953 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: cpcloud-0.0.1.data/scripts/cpcloud
+Filename: cpcloud-0.0.2.data/scripts/cpcloud
 Comment: 
 
-Filename: cpcloud-0.0.1.data/scripts/cpcloud.py
+Filename: cpcloud-0.0.2.data/scripts/cpcloud.py
 Comment: 
 
-Filename: cpcloud-0.0.1.dist-info/LICENSE
+Filename: cpcloud-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: cpcloud-0.0.1.dist-info/METADATA
+Filename: cpcloud-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cpcloud-0.0.1.dist-info/WHEEL
+Filename: cpcloud-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cpcloud-0.0.1.dist-info/top_level.txt
+Filename: cpcloud-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cpcloud-0.0.1.dist-info/RECORD
+Filename: cpcloud-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cpcloud-0.0.1.data/scripts/cpcloud` & `cpcloud-0.0.2.data/scripts/cpcloud`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+#!python
 import os
 
 import argparse
 from tqdm import tqdm
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 from googleapiclient.http import MediaIoBaseDownload
 
 from mimetypes import guess_type
 
-# If modifying these scopes, delete the file token.json.
+VERSION = "0.0.2"
+
 SCOPES = [
     "https://www.googleapis.com/auth/drive",
     "https://www.googleapis.com/auth/drive.appdata",
     "https://www.googleapis.com/auth/drive.file",
 ]
 
 credentials = {
@@ -226,15 +228,15 @@
         files = get_files(directory_id, service)
 
         for file in files:
             download_file(file.get("id"), file.get("name"), service)
 
 
 def get_version():
-    return "0.0.1"
+    return VERSION
 
 
 def command_selector(command, **args):
     commands = {"send": send_files, "receive": receive_files, "version": get_version}
 
     command_fnc = commands.get(command, invalid_command)
```

## Comparing `cpcloud-0.0.1.data/scripts/cpcloud.py` & `cpcloud-0.0.2.data/scripts/cpcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+#!python
 import os
 
 import argparse
 from tqdm import tqdm
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 from googleapiclient.http import MediaIoBaseDownload
 
 from mimetypes import guess_type
 
-# If modifying these scopes, delete the file token.json.
+VERSION = "0.0.2"
+
 SCOPES = [
     "https://www.googleapis.com/auth/drive",
     "https://www.googleapis.com/auth/drive.appdata",
     "https://www.googleapis.com/auth/drive.file",
 ]
 
 credentials = {
@@ -226,15 +228,15 @@
         files = get_files(directory_id, service)
 
         for file in files:
             download_file(file.get("id"), file.get("name"), service)
 
 
 def get_version():
-    return "0.0.1"
+    return VERSION
 
 
 def command_selector(command, **args):
     commands = {"send": send_files, "receive": receive_files, "version": get_version}
 
     command_fnc = commands.get(command, invalid_command)
```

## Comparing `cpcloud-0.0.1.dist-info/LICENSE` & `cpcloud-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpcloud-0.0.1.dist-info/METADATA` & `cpcloud-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpcloud
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple tool to copy files using Google Drive.
 Author: Edzon Sanchez
 Author-email: edzon.sanchez@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `cpcloud-0.0.1.dist-info/RECORD` & `cpcloud-0.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-cpcloud-0.0.1.data/scripts/cpcloud,sha256=AJ9yhZBODIK5J2UHTmUVHTeDTXPREcySyCr2gRMaVKs,7838
-cpcloud-0.0.1.data/scripts/cpcloud.py,sha256=AJ9yhZBODIK5J2UHTmUVHTeDTXPREcySyCr2gRMaVKs,7838
-cpcloud-0.0.1.dist-info/LICENSE,sha256=79ZW7nvt3_m-GgF2a0S-2kLIJ9LnjMOEtlqoTlKLkyk,1077
-cpcloud-0.0.1.dist-info/METADATA,sha256=FFwWVlo_rq6MTC0Lq_jbn_Np2KkqeYAXcMmF7sOAn5A,574
-cpcloud-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cpcloud-0.0.1.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-cpcloud-0.0.1.dist-info/RECORD,,
+cpcloud-0.0.2.data/scripts/cpcloud,sha256=-MvmMmCZU1OfZj-ye1UOIE0rWis89lC-OnTYx_7jUuE,7809
+cpcloud-0.0.2.data/scripts/cpcloud.py,sha256=-MvmMmCZU1OfZj-ye1UOIE0rWis89lC-OnTYx_7jUuE,7809
+cpcloud-0.0.2.dist-info/LICENSE,sha256=79ZW7nvt3_m-GgF2a0S-2kLIJ9LnjMOEtlqoTlKLkyk,1077
+cpcloud-0.0.2.dist-info/METADATA,sha256=E9gZuefAnpRdpIYWRrrBpN0V4NhCwuoO77gE7WmqstY,574
+cpcloud-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cpcloud-0.0.2.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+cpcloud-0.0.2.dist-info/RECORD,,
```

