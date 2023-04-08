# Comparing `tmp/gif2ascii-0.1.3.tar.gz` & `tmp/gif2ascii-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif2ascii-0.1.3.tar", last modified: Sat Apr  8 13:48:23 2023, max compression
+gzip compressed data, was "gif2ascii-0.1.4.tar", last modified: Sat Apr  8 16:59:06 2023, max compression
```

## Comparing `gif2ascii-0.1.3.tar` & `gif2ascii-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 13:48:23.720858 gif2ascii-0.1.3/
--rw-r--r--   0 shbhit     (501) staff       (20)     1216 2023-04-08 13:48:23.719395 gif2ascii-0.1.3/PKG-INFO
--rw-r--r--   0 shbhit     (501) staff       (20)      739 2023-04-08 11:21:22.000000 gif2ascii-0.1.3/README.md
-drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 13:48:23.701696 gif2ascii-0.1.3/gif2ascii/
--rw-r--r--   0 shbhit     (501) staff       (20)     4570 2023-04-08 13:44:55.000000 gif2ascii-0.1.3/gif2ascii/GifAscii.py
--rw-r--r--   0 shbhit     (501) staff       (20)       40 2023-04-08 09:41:46.000000 gif2ascii-0.1.3/gif2ascii/__init__.py
--rw-r--r--   0 shbhit     (501) staff       (20)     1481 2023-04-08 13:47:28.000000 gif2ascii-0.1.3/gif2ascii/__main__.py
--rw-r--r--   0 shbhit     (501) staff       (20)     1156 2023-04-08 08:33:03.000000 gif2ascii-0.1.3/gif2ascii/clear.py
-drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 13:48:23.715778 gif2ascii-0.1.3/gif2ascii.egg-info/
--rw-r--r--   0 shbhit     (501) staff       (20)     1216 2023-04-08 13:48:23.000000 gif2ascii-0.1.3/gif2ascii.egg-info/PKG-INFO
--rw-r--r--   0 shbhit     (501) staff       (20)      267 2023-04-08 13:48:23.000000 gif2ascii-0.1.3/gif2ascii.egg-info/SOURCES.txt
--rw-r--r--   0 shbhit     (501) staff       (20)        1 2023-04-08 13:48:23.000000 gif2ascii-0.1.3/gif2ascii.egg-info/dependency_links.txt
--rw-r--r--   0 shbhit     (501) staff       (20)       16 2023-04-08 13:48:23.000000 gif2ascii-0.1.3/gif2ascii.egg-info/requires.txt
--rw-r--r--   0 shbhit     (501) staff       (20)       10 2023-04-08 13:48:23.000000 gif2ascii-0.1.3/gif2ascii.egg-info/top_level.txt
--rw-r--r--   0 shbhit     (501) staff       (20)       38 2023-04-08 13:48:23.720986 gif2ascii-0.1.3/setup.cfg
--rw-r--r--   0 shbhit     (501) staff       (20)     1018 2023-04-08 13:48:20.000000 gif2ascii-0.1.3/setup.py
+drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 16:59:06.505242 gif2ascii-0.1.4/
+-rw-r--r--   0 shbhit     (501) staff       (20)     1889 2023-04-08 16:59:06.504188 gif2ascii-0.1.4/PKG-INFO
+-rw-r--r--   0 shbhit     (501) staff       (20)     1351 2023-04-08 16:55:56.000000 gif2ascii-0.1.4/README.md
+drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 16:59:06.490640 gif2ascii-0.1.4/gif2ascii/
+-rw-r--r--   0 shbhit     (501) staff       (20)     4570 2023-04-08 13:44:55.000000 gif2ascii-0.1.4/gif2ascii/GifAscii.py
+-rw-r--r--   0 shbhit     (501) staff       (20)       40 2023-04-08 09:41:46.000000 gif2ascii-0.1.4/gif2ascii/__init__.py
+-rw-r--r--   0 shbhit     (501) staff       (20)     1481 2023-04-08 13:54:12.000000 gif2ascii-0.1.4/gif2ascii/__main__.py
+-rw-r--r--   0 shbhit     (501) staff       (20)     1156 2023-04-08 08:33:03.000000 gif2ascii-0.1.4/gif2ascii/clear.py
+drwxr-xr-x   0 shbhit     (501) staff       (20)        0 2023-04-08 16:59:06.502119 gif2ascii-0.1.4/gif2ascii.egg-info/
+-rw-r--r--   0 shbhit     (501) staff       (20)     1889 2023-04-08 16:59:06.000000 gif2ascii-0.1.4/gif2ascii.egg-info/PKG-INFO
+-rw-r--r--   0 shbhit     (501) staff       (20)      267 2023-04-08 16:59:06.000000 gif2ascii-0.1.4/gif2ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 shbhit     (501) staff       (20)        1 2023-04-08 16:59:06.000000 gif2ascii-0.1.4/gif2ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 shbhit     (501) staff       (20)       16 2023-04-08 16:59:06.000000 gif2ascii-0.1.4/gif2ascii.egg-info/requires.txt
+-rw-r--r--   0 shbhit     (501) staff       (20)       10 2023-04-08 16:59:06.000000 gif2ascii-0.1.4/gif2ascii.egg-info/top_level.txt
+-rw-r--r--   0 shbhit     (501) staff       (20)       38 2023-04-08 16:59:06.505335 gif2ascii-0.1.4/setup.cfg
+-rw-r--r--   0 shbhit     (501) staff       (20)     1104 2023-04-08 16:58:19.000000 gif2ascii-0.1.4/setup.py
```

### Comparing `gif2ascii-0.1.3/gif2ascii/GifAscii.py` & `gif2ascii-0.1.4/gif2ascii/GifAscii.py`

 * *Files identical despite different names*

### Comparing `gif2ascii-0.1.3/gif2ascii/__main__.py` & `gif2ascii-0.1.4/gif2ascii/__main__.py`

 * *Files identical despite different names*

### Comparing `gif2ascii-0.1.3/gif2ascii/clear.py` & `gif2ascii-0.1.4/gif2ascii/clear.py`

 * *Files identical despite different names*

### Comparing `gif2ascii-0.1.3/setup.py` & `gif2ascii-0.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Gif to ASCII'
 LONG_DESCRIPTION = 'Converts Gifs and Images to Colorful ASCII'
 
 # Setting up
 setup(
     name="gif2ascii",
     version=VERSION,
@@ -19,14 +19,17 @@
     author_email="<shobhitbhosure7@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['Pillow', 'argparse'],
     keywords=['python', 'ascii gif', 'terminal gif', 'ascii art', 'terminal art'],
+    project_urls={
+        'Source': "https://github.com/shobhit99/gif2ascii/"
+    },
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

