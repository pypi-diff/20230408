# Comparing `tmp/wiu-0.0.7.tar.gz` & `tmp/wiu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiu-0.0.7.tar", last modified: Sat Apr  8 17:43:46 2023, max compression
+gzip compressed data, was "wiu-0.0.8.tar", last modified: Sat Apr  8 17:49:38 2023, max compression
```

## Comparing `wiu-0.0.7.tar` & `wiu-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:43:46.862309 wiu-0.0.7/
--rw-rw-rw-   0        0        0     1096 2023-04-07 16:59:44.000000 wiu-0.0.7/LICENCE
--rw-rw-rw-   0        0        0      957 2023-04-08 17:43:46.861311 wiu-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-04-08 00:38:12.000000 wiu-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 17:43:46.862309 wiu-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      527 2023-04-08 17:43:42.000000 wiu-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:43:46.811352 wiu-0.0.7/wiu/
--rw-rw-rw-   0        0        0       66 2023-04-08 05:58:55.000000 wiu-0.0.7/wiu/__init__.py
--rw-rw-rw-   0        0        0     1932 2023-04-08 17:43:06.000000 wiu-0.0.7/wiu/calculator.py
--rw-rw-rw-   0        0        0      377 2023-04-08 05:52:36.000000 wiu-0.0.7/wiu/message.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:43:46.858313 wiu-0.0.7/wiu.egg-info/
--rw-rw-rw-   0        0        0      957 2023-04-08 17:43:46.000000 wiu-0.0.7/wiu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-04-08 17:43:46.000000 wiu-0.0.7/wiu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:43:46.000000 wiu-0.0.7/wiu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-08 17:43:46.000000 wiu-0.0.7/wiu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:49:38.890268 wiu-0.0.8/
+-rw-rw-rw-   0        0        0     1096 2023-04-07 16:59:44.000000 wiu-0.0.8/LICENCE
+-rw-rw-rw-   0        0        0      957 2023-04-08 17:49:38.889269 wiu-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-04-08 00:38:12.000000 wiu-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:49:38.907253 wiu-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      527 2023-04-08 17:49:31.000000 wiu-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:49:38.858296 wiu-0.0.8/wiu/
+-rw-rw-rw-   0        0        0       66 2023-04-08 05:58:55.000000 wiu-0.0.8/wiu/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-04-08 17:49:15.000000 wiu-0.0.8/wiu/calculator.py
+-rw-rw-rw-   0        0        0      377 2023-04-08 05:52:36.000000 wiu-0.0.8/wiu/message.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:49:38.886273 wiu-0.0.8/wiu.egg-info/
+-rw-rw-rw-   0        0        0      957 2023-04-08 17:49:38.000000 wiu-0.0.8/wiu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-04-08 17:49:38.000000 wiu-0.0.8/wiu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:49:38.000000 wiu-0.0.8/wiu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-08 17:49:38.000000 wiu-0.0.8/wiu.egg-info/top_level.txt
```

### Comparing `wiu-0.0.7/LICENCE` & `wiu-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `wiu-0.0.7/PKG-INFO` & `wiu-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiu
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library made to practice and improve programming and english skills during our university.
 Home-page: UNKNOWN
 Author: Iuri Torres & João Witor
 Author-email: iuri.t1000@gmail.com
 License: MIT License
 Keywords: wiu
 Platform: UNKNOWN
```

### Comparing `wiu-0.0.7/README.md` & `wiu-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wiu-0.0.7/setup.py` & `wiu-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as file:
     readme = file.read()
 
 setup(
     name='wiu',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT License',
     author='Iuri Torres & João Witor',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='iuri.t1000@gmail.com',
     keywords='wiu',
     description=u'A library made to practice and improve programming and english skills during our university.',
```

### Comparing `wiu-0.0.7/wiu/calculator.py` & `wiu-0.0.8/wiu/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return accumulated
 
         except IndexError:
             Message.send_error("You can't pass an empty list")
 
 
     # CALC AVERAGE OF A LIST OF NUMBERS
-    def calcAverage(array: list[int|float]) -> int|float:
+    def average(array: list[int|float]) -> int|float:
         try:   
             average = sum(array) / len(array)
 
             if '.0' in str(average):
                 average = int( str(average).replace('.0', '') )
 
             return average
```

### Comparing `wiu-0.0.7/wiu.egg-info/PKG-INFO` & `wiu-0.0.8/wiu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiu
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library made to practice and improve programming and english skills during our university.
 Home-page: UNKNOWN
 Author: Iuri Torres & João Witor
 Author-email: iuri.t1000@gmail.com
 License: MIT License
 Keywords: wiu
 Platform: UNKNOWN
```

