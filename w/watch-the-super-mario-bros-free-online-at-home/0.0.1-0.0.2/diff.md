# Comparing `tmp/watch-the-super-mario-bros-free-online-at-home-0.0.1.tar.gz` & `tmp/watch-the-super-mario-bros-free-online-at-home-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-the-super-mario-bros-free-online-at-home-0.0.1.tar", last modified: Sat Apr  8 18:10:57 2023, max compression
+gzip compressed data, was "watch-the-super-mario-bros-free-online-at-home-0.0.2.tar", last modified: Sat Apr  8 18:33:40 2023, max compression
```

## Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.1.tar` & `watch-the-super-mario-bros-free-online-at-home-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 18:10:57.388182 watch-the-super-mario-bros-free-online-at-home-0.0.1/
--rw-rw-rw-   0        0        0     1071 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      536 2023-04-08 18:10:57.388182 watch-the-super-mario-bros-free-online-at-home-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14804 2023-04-08 01:21:43.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 18:10:57.371228 watch-the-super-mario-bros-free-online-at-home-0.0.1/mariobros/
--rw-rw-rw-   0        0        0      654 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/mariobros/Area_Fig.py
--rw-rw-rw-   0        0        0        0 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/mariobros/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-08 18:10:57.388182 watch-the-super-mario-bros-free-online-at-home-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-08 18:09:20.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:10:57.387184 watch-the-super-mario-bros-free-online-at-home-0.0.1/watch_the_super_mario_bros_free_online_at_home.egg-info/
--rw-rw-rw-   0        0        0      536 2023-04-08 18:10:57.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/watch_the_super_mario_bros_free_online_at_home.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-08 18:10:57.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/watch_the_super_mario_bros_free_online_at_home.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 18:10:57.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/watch_the_super_mario_bros_free_online_at_home.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-08 18:10:57.000000 watch-the-super-mario-bros-free-online-at-home-0.0.1/watch_the_super_mario_bros_free_online_at_home.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:33:40.448081 watch-the-super-mario-bros-free-online-at-home-0.0.2/
+-rw-rw-rw-   0        0        0     1071 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-04-08 18:33:40.447083 watch-the-super-mario-bros-free-online-at-home-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14804 2023-04-08 01:21:43.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 18:33:40.428170 watch-the-super-mario-bros-free-online-at-home-0.0.2/mariobros/
+-rw-rw-rw-   0        0        0      654 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/mariobros/Area_Fig.py
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/mariobros/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:33:40.448081 watch-the-super-mario-bros-free-online-at-home-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-04-08 18:33:25.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:33:40.446087 watch-the-super-mario-bros-free-online-at-home-0.0.2/watch_the_super_mario_bros_free_online_at_home.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-04-08 18:33:40.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/watch_the_super_mario_bros_free_online_at_home.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-08 18:33:40.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/watch_the_super_mario_bros_free_online_at_home.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:33:40.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/watch_the_super_mario_bros_free_online_at_home.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-08 18:33:40.000000 watch-the-super-mario-bros-free-online-at-home-0.0.2/watch_the_super_mario_bros_free_online_at_home.egg-info/top_level.txt
```

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.1/LICENSE` & `watch-the-super-mario-bros-free-online-at-home-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.1/README.md` & `watch-the-super-mario-bros-free-online-at-home-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.1/mariobros/Area_Fig.py` & `watch-the-super-mario-bros-free-online-at-home-0.0.2/mariobros/Area_Fig.py`

 * *Files identical despite different names*

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.1/setup.py` & `watch-the-super-mario-bros-free-online-at-home-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from setuptools import setup, find_packages
-import codecs
-import os
+from setuptools import setup
+import setuptools
 
-VERSION = '0.0.1'
-DESCRIPTION = 'Watch "The Super Mario Bros. Movie" Free Online At Home'
+# with open("README.md", "r") as fh:
+#    long_description = fh.read()
 
-
-# Setting up
 setup(
+    
+    version='0.0.2',
+    description= 'Watch "The Super Mario Bros. Movie" Free Online At Home',
     name="watch-the-super-mario-bros-free-online-at-home",
-    version=VERSION,
     author="john",
     author_email="john@gmail.com",
+    # long_description=long_description,
     long_description_content_type="text/markdown",
-    long_description= "file: README.md",
-    packages=find_packages(),
+     packages=setuptools.find_packages(),
     install_requires=[],
     keywords=['The super mario bros'],
     classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ]
 )
```

