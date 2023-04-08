# Comparing `tmp/qiskit_quaintier-0.2.0.tar.gz` & `tmp/qiskit_quaintier-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_quaintier-0.2.0.tar", last modified: Sat Apr  8 21:50:20 2023, max compression
+gzip compressed data, was "qiskit_quaintier-0.3.0.tar", last modified: Sat Apr  8 21:55:05 2023, max compression
```

## Comparing `qiskit_quaintier-0.2.0.tar` & `qiskit_quaintier-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 21:50:20.099680 qiskit_quaintier-0.2.0/
--rw-r--r--   0 rustam     (501) staff       (20)      336 2023-04-08 21:50:20.099391 qiskit_quaintier-0.2.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_quaintier-0.2.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 21:50:20.098948 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)      336 2023-04-08 21:50:20.000000 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      231 2023-04-08 21:50:20.000000 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-08 21:50:20.000000 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       18 2023-04-08 21:50:20.000000 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       10 2023-04-08 21:50:20.000000 qiskit_quaintier-0.2.0/qiskit_quaintier.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1889 2023-04-08 21:16:12.000000 qiskit_quaintier-0.2.0/quantier.py
--rw-r--r--   0 rustam     (501) staff       (20)       38 2023-04-08 21:50:20.099779 qiskit_quaintier-0.2.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      657 2023-04-08 21:50:03.000000 qiskit_quaintier-0.2.0/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 21:55:05.569632 qiskit_quaintier-0.3.0/
+-rw-r--r--   0 rustam     (501) staff       (20)      336 2023-04-08 21:55:05.569346 qiskit_quaintier-0.3.0/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_quaintier-0.3.0/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 21:55:05.568845 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)      336 2023-04-08 21:55:05.000000 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      231 2023-04-08 21:55:05.000000 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-08 21:55:05.000000 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       18 2023-04-08 21:55:05.000000 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       10 2023-04-08 21:55:05.000000 qiskit_quaintier-0.3.0/qiskit_quaintier.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1889 2023-04-08 21:16:12.000000 qiskit_quaintier-0.3.0/quantier.py
+-rw-r--r--   0 rustam     (501) staff       (20)       38 2023-04-08 21:55:05.569729 qiskit_quaintier-0.3.0/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      657 2023-04-08 21:54:23.000000 qiskit_quaintier-0.3.0/setup.py
```

### Comparing `qiskit_quaintier-0.2.0/quantier.py` & `qiskit_quaintier-0.3.0/quantier.py`

 * *Files identical despite different names*

### Comparing `qiskit_quaintier-0.2.0/setup.py` & `qiskit_quaintier-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qiskit_quaintier",
-    version="0.2.0",
+    version="0.3.0",
     description="A quantum provider for Qiskit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["quaintier"],
     package_dir={"quaintier": "."},
     classifiers=[
         "Programming Language :: Python :: 3",
```

