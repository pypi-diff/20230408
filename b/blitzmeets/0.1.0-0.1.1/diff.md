# Comparing `tmp/blitzmeets-0.1.0.tar.gz` & `tmp/blitzmeets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blitzmeets-0.1.0.tar", last modified: Sat Apr  8 17:03:37 2023, max compression
+gzip compressed data, was "blitzmeets-0.1.1.tar", last modified: Sat Apr  8 17:12:36 2023, max compression
```

## Comparing `blitzmeets-0.1.0.tar` & `blitzmeets-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:03:37.493617 blitzmeets-0.1.0/
--rw-rw-rw-   0        0        0     1163 2023-04-08 17:03:37.492031 blitzmeets-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-04-08 17:01:49.000000 blitzmeets-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 17:03:37.461809 blitzmeets-0.1.0/blitzmeets/
--rw-rw-rw-   0        0        0       30 2023-04-08 17:00:29.000000 blitzmeets-0.1.0/blitzmeets/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-08 16:39:47.000000 blitzmeets-0.1.0/blitzmeets/client.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:03:37.490546 blitzmeets-0.1.0/blitzmeets.egg-info/
--rw-rw-rw-   0        0        0     1163 2023-04-08 17:03:37.000000 blitzmeets-0.1.0/blitzmeets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-08 17:03:37.000000 blitzmeets-0.1.0/blitzmeets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:03:37.000000 blitzmeets-0.1.0/blitzmeets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-08 17:03:37.000000 blitzmeets-0.1.0/blitzmeets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 17:03:37.000000 blitzmeets-0.1.0/blitzmeets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 17:03:37.493617 blitzmeets-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-04-08 16:39:09.000000 blitzmeets-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:12:36.823165 blitzmeets-0.1.1/
+-rw-rw-rw-   0        0        0     1163 2023-04-08 17:12:36.823165 blitzmeets-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-04-08 17:01:49.000000 blitzmeets-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 17:12:36.800284 blitzmeets-0.1.1/blitzmeets/
+-rw-rw-rw-   0        0        0       30 2023-04-08 17:00:29.000000 blitzmeets-0.1.1/blitzmeets/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-04-08 17:11:55.000000 blitzmeets-0.1.1/blitzmeets/client.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:12:36.821092 blitzmeets-0.1.1/blitzmeets.egg-info/
+-rw-rw-rw-   0        0        0     1163 2023-04-08 17:12:36.000000 blitzmeets-0.1.1/blitzmeets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-08 17:12:36.000000 blitzmeets-0.1.1/blitzmeets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:12:36.000000 blitzmeets-0.1.1/blitzmeets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-08 17:12:36.000000 blitzmeets-0.1.1/blitzmeets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-08 17:12:36.000000 blitzmeets-0.1.1/blitzmeets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:12:36.824610 blitzmeets-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      940 2023-04-08 17:12:13.000000 blitzmeets-0.1.1/setup.py
```

### Comparing `blitzmeets-0.1.0/PKG-INFO` & `blitzmeets-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blitzmeets
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility to create virtual meetings programatically
 Home-page: https://github.com/BliyzJB/BlitzMeets
 Author: Your Name
 Author-email: youremail@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blitzmeets-0.1.0/blitzmeets/client.py` & `blitzmeets-0.1.1/blitzmeets/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from io import BytesIO
 import qrcode
 
 class MeetClient:
     def __init__(self) -> None:
         self.base_url = "https://brie.fi/ng"
 
-    def create_meet(self):
+    def create_meet(self) -> str:
         unique_id = token_hex(4)
         return f"{self.base_url}/{unique_id[:3:]}-{unique_id[3:6]}-{unique_id[6:]}"
 
-    def create_qr_code(self):
+    def create_qr_code(self) -> bytes:
         meet_link = self.create_meet()
         qr = qrcode.QRCode(version=1, box_size=10, border=4)
         qr.add_data(meet_link)
         qr.make(fit=True)
         img = qr.make_image(fill_color="black", back_color="white")
         with BytesIO() as buffer:
             img.save(buffer, format="png")
```

### Comparing `blitzmeets-0.1.0/blitzmeets.egg-info/PKG-INFO` & `blitzmeets-0.1.1/blitzmeets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blitzmeets
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility to create virtual meetings programatically
 Home-page: https://github.com/BliyzJB/BlitzMeets
 Author: Your Name
 Author-email: youremail@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blitzmeets-0.1.0/setup.py` & `blitzmeets-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='blitzmeets',
-    version='0.1.0',
+    version='0.1.1',
     description='A utility to create virtual meetings programatically',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Your Name',
     author_email='youremail@example.com',
     url='https://github.com/BliyzJB/BlitzMeets',
     packages=find_packages(),
```

