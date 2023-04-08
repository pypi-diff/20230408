# Comparing `tmp/sinacor_negs-0.0.2.tar.gz` & `tmp/sinacor_negs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinacor_negs-0.0.2.tar", last modified: Sat Apr  8 20:31:11 2023, max compression
+gzip compressed data, was "sinacor_negs-0.0.3.tar", last modified: Sat Apr  8 20:54:54 2023, max compression
```

## Comparing `sinacor_negs-0.0.2.tar` & `sinacor_negs-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 20:31:11.539207 sinacor_negs-0.0.2/
--rw-rw-rw-   0        0        0     1099 2023-04-08 18:19:42.000000 sinacor_negs-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1201 2023-04-08 20:31:11.538210 sinacor_negs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-04-08 19:15:57.000000 sinacor_negs-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 20:31:11.540206 sinacor_negs-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      942 2023-04-08 20:30:52.000000 sinacor_negs-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:31:11.526242 sinacor_negs-0.0.2/sinacor_negs/
--rw-rw-rw-   0        0        0        0 2023-04-08 20:17:48.000000 sinacor_negs-0.0.2/sinacor_negs/__init__.py
--rw-rw-rw-   0        0        0     4610 2023-04-08 19:51:38.000000 sinacor_negs-0.0.2/sinacor_negs/sinacor_negs.py
--rw-rw-rw-   0        0        0      166 2023-04-08 18:47:29.000000 sinacor_negs-0.0.2/sinacor_negs/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:31:11.536216 sinacor_negs-0.0.2/sinacor_negs.egg-info/
--rw-rw-rw-   0        0        0     1201 2023-04-08 20:31:11.000000 sinacor_negs-0.0.2/sinacor_negs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-08 20:31:11.000000 sinacor_negs-0.0.2/sinacor_negs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 20:31:11.000000 sinacor_negs-0.0.2/sinacor_negs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-08 20:31:11.000000 sinacor_negs-0.0.2/sinacor_negs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-08 20:31:11.000000 sinacor_negs-0.0.2/sinacor_negs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.945923 sinacor_negs-0.0.3/
+-rw-rw-rw-   0        0        0     1099 2023-04-08 18:19:42.000000 sinacor_negs-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      605 2023-04-08 20:54:54.944925 sinacor_negs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-04-08 20:52:11.000000 sinacor_negs-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 20:54:54.945923 sinacor_negs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-08 20:53:35.000000 sinacor_negs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.934952 sinacor_negs-0.0.3/sinacor_negs/
+-rw-rw-rw-   0        0        0       39 2023-04-08 20:54:25.000000 sinacor_negs-0.0.3/sinacor_negs/__init__.py
+-rw-rw-rw-   0        0        0     4611 2023-04-08 20:54:26.000000 sinacor_negs-0.0.3/sinacor_negs/sinacor_negs.py
+-rw-rw-rw-   0        0        0      166 2023-04-08 20:54:51.000000 sinacor_negs-0.0.3/sinacor_negs/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.942929 sinacor_negs-0.0.3/sinacor_negs.egg-info/
+-rw-rw-rw-   0        0        0      605 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/top_level.txt
```

### Comparing `sinacor_negs-0.0.2/LICENSE.txt` & `sinacor_negs-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.0.2/README.md` & `sinacor_negs-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Como usar
 ```python
 import sinacor_negs as snegs
 
 negs_txt_path = 'sample//negs.txt'
 
-negs = snegs.read_negs_txt(negs_sample_path)
+negs = snegs.read_negs_txt(negs_txt_path)
 
 '''
 negs.header -> dataframe do header.
 negs.negs -> dataframe do negs (todos os negócios).
 negs.trailer -> dataframe do trailer.
 '''
```

### Comparing `sinacor_negs-0.0.2/setup.py` & `sinacor_negs-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="sinacor_negs",
-    version="0.0.2",
+    version="0.0.3",
     author="Renan Moretto Pereira",
     author_email="renan_morettopereira@hotmail.com",
     description="Leitor do arquivo NEGS da bolsa",
-    long_description_content_type="text/markdown",
-    long_description=long_description,
     license="MIT",
     packages=find_packages(),
     install_requires=["pandas>=2.0.0", "numpy>=1.24.2"],
     keywords=["python", "sinacor", "negs", "bolsa", "b3"],
     url="https://github.com/renanmoretto/sinacor_negs",
     classifiers=[
         "Development Status :: 1 - Planning",
```

### Comparing `sinacor_negs-0.0.2/sinacor_negs/sinacor_negs.py` & `sinacor_negs-0.0.3/sinacor_negs/sinacor_negs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 
 from dataclasses import dataclass
 
-from utils import drop_left_zeros_df
+from .utils import drop_left_zeros_df
 
 @dataclass
 class Negs:
     header: pd.DataFrame()
     negs: pd.DataFrame()
     trailer: pd.DataFrame()
     account_more_than_seven_digits: bool
```

