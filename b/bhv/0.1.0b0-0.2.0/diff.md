# Comparing `tmp/bhv-0.1.0b0.tar.gz` & `tmp/bhv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.1.0b0.tar", last modified: Wed Apr  5 12:47:52 2023, max compression
+gzip compressed data, was "bhv-0.2.0.tar", last modified: Sat Apr  8 19:21:00 2023, max compression
```

## Comparing `bhv-0.1.0b0.tar` & `bhv-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-05 12:47:52.580226 bhv-0.1.0b0/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1007 2023-04-05 12:47:52.580226 bhv-0.1.0b0/PKG-INFO
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-05 12:47:52.580226 bhv-0.1.0b0/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)      213 2023-04-05 10:59:47.000000 bhv-0.1.0b0/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    10562 2023-04-05 12:45:11.000000 bhv-0.1.0b0/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9571 2023-04-05 12:47:46.000000 bhv-0.1.0b0/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     7088 2023-04-05 12:47:46.000000 bhv-0.1.0b0/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1979 2023-04-01 10:14:38.000000 bhv-0.1.0b0/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6120 2023-04-05 12:47:46.000000 bhv-0.1.0b0/bhv/symbolic.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-05 12:47:52.580226 bhv-0.1.0b0/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1007 2023-04-05 12:47:52.000000 bhv-0.1.0b0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      229 2023-04-05 12:47:52.000000 bhv-0.1.0b0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-05 12:47:52.000000 bhv-0.1.0b0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-05 12:47:52.000000 bhv-0.1.0b0/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-05 12:47:52.000000 bhv-0.1.0b0/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-05 12:47:52.580226 bhv-0.1.0b0/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1332 2023-04-05 12:47:46.000000 bhv-0.1.0b0/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1060 2023-04-08 19:21:00.370536 bhv-0.2.0/PKG-INFO
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.2.0/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    10798 2023-04-07 21:10:32.000000 bhv-0.2.0/bhv/abstract.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     9571 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     7088 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1980 2023-04-07 21:03:27.000000 bhv-0.2.0/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     6120 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/symbolic.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1060 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      229 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       73 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-04-08 19:21:00.370536 bhv-0.2.0/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1331 2023-04-07 21:27:02.000000 bhv-0.2.0/setup.py
```

### Comparing `bhv-0.1.0b0/PKG-INFO` & `bhv-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.1.0b0
+Version: 0.2.0
 Summary: Boolean Hypervectors
+Home-page: UNKNOWN
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
+License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -20,7 +23,8 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
+
```

### Comparing `bhv-0.1.0b0/bhv/abstract.py` & `bhv-0.2.0/bhv/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,32 +135,37 @@
 
     def jaccard(self, other: Self) -> float:
         return 1. - float((self & other).active()) / float((self | other).active() + 1E-7)
 
     def cosine(self, other: Self) -> float:
         return 1 - float((self & other).active()) / float(self.active() * other.active() + 1E-7)**.5
 
-    def std_apart(self, other: Self) -> float:
+    def std_apart(self, other: Self, invert=False) -> float:
         p = 0.5
         n = NormalDist(0, (DIMENSION*p*(1 - p))**.5)
-        return n.zscore(self.hamming(other))
+        estdvs = n.zscore(p*DIMENSION)
+        stdvs = n.zscore(self.hamming(other))
+        return estdvs - stdvs if invert else stdvs
 
     def zscore(self) -> float:
         p = 0.5
         n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
         return n.zscore(self.active())
 
     def pvalue(self) -> float:
         p = 0.5
         n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
         s = n.cdf(self.active())
         return 2.*min(s, 1. - s)
 
-    def sixsigma(self, other: Self) -> bool:
-        return abs(self.std_apart(other)) < 6
+    def related(self, other: Self, stdvs=6) -> bool:
+        return abs(self.std_apart(other)) < stdvs
+
+    def unrelated(self, other: Self, stdvs=6) -> bool:
+        return abs(self.std_apart(other, invert=True)) < stdvs
 
     # Alternative implementations
 
     @classmethod
     def _majority3_select(cls, a: Self, b: Self, c: Self) -> Self:
         # C:  1 0 0 1 0 1 1
```

### Comparing `bhv-0.1.0b0/bhv/np.py` & `bhv-0.2.0/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.1.0b0/bhv/pytorch.py` & `bhv-0.2.0/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.1.0b0/bhv/shared.py` & `bhv-0.2.0/bhv/shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
     from typing import Self
 except ImportError:
-    Self = 'AbstractHV'
+    Self = 'AbstractBHV'
 
 DIMENSION = 8192
 
 from dataclasses import fields, is_dataclass
 from base64 import _urlsafe_encode_translation
 import hashlib
 import binascii
```

### Comparing `bhv-0.1.0b0/bhv/symbolic.py` & `bhv-0.2.0/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.1.0b0/bhv.egg-info/PKG-INFO` & `bhv-0.2.0/bhv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.1.0b0
+Version: 0.2.0
 Summary: Boolean Hypervectors
+Home-page: UNKNOWN
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
+License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -20,7 +23,8 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
+
```

### Comparing `bhv-0.1.0b0/setup.py` & `bhv-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0b'
+VERSION = '0.2.0'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

