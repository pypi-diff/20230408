# Comparing `tmp/pynarrator-0.0.1.5.tar.gz` & `tmp/pynarrator-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynarrator-0.0.1.5.tar", last modified: Sun Apr  2 11:33:56 2023, max compression
+gzip compressed data, was "pynarrator-0.0.1.6.tar", last modified: Sat Apr  8 18:47:57 2023, max compression
```

## Comparing `pynarrator-0.0.1.5.tar` & `pynarrator-0.0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-02 11:33:56.212890 pynarrator-0.0.1.5/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.5/LICENSE
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1254 2023-04-02 11:33:56.212777 pynarrator-0.0.1.5/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      482 2023-04-02 11:29:50.000000 pynarrator-0.0.1.5/README.md
--rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-02 11:33:56.212938 pynarrator-0.0.1.5/setup.cfg
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-02 11:33:37.000000 pynarrator-0.0.1.5/setup.py
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-02 11:33:56.211148 pynarrator-0.0.1.5/src/
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-02 11:33:56.212359 pynarrator-0.0.1.5/src/pynarrator.egg-info/
--rw-r--r--   0 denisabdullin   (501) staff       (20)     1254 2023-04-02 11:33:56.000000 pynarrator-0.0.1.5/src/pynarrator.egg-info/PKG-INFO
--rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-02 11:33:56.000000 pynarrator-0.0.1.5/src/pynarrator.egg-info/SOURCES.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-02 11:33:56.000000 pynarrator-0.0.1.5/src/pynarrator.egg-info/dependency_links.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-02 11:33:56.000000 pynarrator-0.0.1.5/src/pynarrator.egg-info/requires.txt
--rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-02 11:33:56.000000 pynarrator-0.0.1.5/src/pynarrator.egg-info/top_level.txt
-drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-02 11:33:56.212480 pynarrator-0.0.1.5/tests/
--rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.5/tests/test_narrate_descriptive.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.693501 pynarrator-0.0.1.6/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1071 2023-03-01 20:23:53.000000 pynarrator-0.0.1.6/LICENSE
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1684 2023-04-08 18:47:57.693376 pynarrator-0.0.1.6/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      968 2023-04-08 18:46:26.000000 pynarrator-0.0.1.6/README.md
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       38 2023-04-08 18:47:57.693537 pynarrator-0.0.1.6/setup.cfg
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1166 2023-04-08 18:47:16.000000 pynarrator-0.0.1.6/setup.py
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.691683 pynarrator-0.0.1.6/src/
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.692869 pynarrator-0.0.1.6/src/pynarrator.egg-info/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)     1684 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/PKG-INFO
+-rw-r--r--   0 denisabdullin   (501) staff       (20)      249 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/SOURCES.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)        1 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/dependency_links.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       55 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/requires.txt
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       43 2023-04-08 18:47:57.000000 pynarrator-0.0.1.6/src/pynarrator.egg-info/top_level.txt
+drwxr-xr-x   0 denisabdullin   (501) staff       (20)        0 2023-04-08 18:47:57.692989 pynarrator-0.0.1.6/tests/
+-rw-r--r--   0 denisabdullin   (501) staff       (20)       68 2023-03-02 10:10:10.000000 pynarrator-0.0.1.6/tests/test_narrate_descriptive.py
```

### Comparing `pynarrator-0.0.1.5/LICENSE` & `pynarrator-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynarrator-0.0.1.5/PKG-INFO` & `pynarrator-0.0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Template-based NLG framework for creating text narratives out of data
-Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
-License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pynarrator
-Template-based NLG framework for creating text narratives out of data
+ Template-based NLG framework for creating text narratives out of data
 
-## Installation
+ ## Installation
 
-You can install the package from pip:
+ You can install the package from pip:
 
-```bash
-pip3 install pynarrator
+ ```bash
+ pip3 install pynarrator
+ ```
+
+ ```python
+ import os
+ from pynarrator import narrate_descriptive, read_data
 ```
 
-## Usage
+## Basic Usage
 
-Import the package functions and create a data frame.
+pynarrator has a range of functions for creating template-based narratives and also embedded data set that you can use by calling `read_data()`
 
 ```python
-from pynarrator import narrate_descriptive, read_data
+sales = read_data()
+narrative = narrate_descriptive(sales, measure = 'Sales', dimensions = ['Region', 'Product'], coverage = 0.5)
+```
 
-df = read_data()
+## Chat GPT
+
+```python
+ from pynarrator import gpt_get_completions, enhance_narrative, translate_narrative, summarize_narrative
+```
 
-df.head()
+```python
+enhance_narrative(narrative)
 ```
 
-Now create descriptive narratives from your data
 ```python
-narrate_descriptive(df, measure = 'Sales', dimensions = ['Region', 'Product'])
+enhance_narrative(narrative, language = 'Spanish')
 ```
 
+```python
+summarize_narrative(narrative)
+```
 
+Complete documentation is available at the [narrator](https://denisabd.github.io/narrator/) package website
```

### Comparing `pynarrator-0.0.1.5/setup.py` & `pynarrator-0.0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open('README.md', 'r') as fh:
    long_description = fh.read()
   
 setup(
   name = 'pynarrator',
-  version = '0.0.1.5',
+  version = '0.0.1.6',
   author = 'Denis Abdullin',
   author_email = 'denisabdullincz@gmail.com',
   description = 'Template-based NLG framework for creating text narratives out of data',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   py_modules = [
     'narrate_descriptive',
```

### Comparing `pynarrator-0.0.1.5/src/pynarrator.egg-info/PKG-INFO` & `pynarrator-0.0.1.6/src/pynarrator.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 Metadata-Version: 2.1
 Name: pynarrator
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Template-based NLG framework for creating text narratives out of data
-Home-page: UNKNOWN
 Author: Denis Abdullin
 Author-email: denisabdullincz@gmail.com
-License: UNKNOWN
 Keywords: python,nlg,template,chatgpt
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pynarrator
-Template-based NLG framework for creating text narratives out of data
+ Template-based NLG framework for creating text narratives out of data
 
-## Installation
+ ## Installation
 
-You can install the package from pip:
+ You can install the package from pip:
 
-```bash
-pip3 install pynarrator
+ ```bash
+ pip3 install pynarrator
+ ```
+
+ ```python
+ import os
+ from pynarrator import narrate_descriptive, read_data
 ```
 
-## Usage
+## Basic Usage
 
-Import the package functions and create a data frame.
+pynarrator has a range of functions for creating template-based narratives and also embedded data set that you can use by calling `read_data()`
 
 ```python
-from pynarrator import narrate_descriptive, read_data
+sales = read_data()
+narrative = narrate_descriptive(sales, measure = 'Sales', dimensions = ['Region', 'Product'], coverage = 0.5)
+```
 
-df = read_data()
+## Chat GPT
+
+```python
+ from pynarrator import gpt_get_completions, enhance_narrative, translate_narrative, summarize_narrative
+```
 
-df.head()
+```python
+enhance_narrative(narrative)
 ```
 
-Now create descriptive narratives from your data
 ```python
-narrate_descriptive(df, measure = 'Sales', dimensions = ['Region', 'Product'])
+enhance_narrative(narrative, language = 'Spanish')
 ```
 
+```python
+summarize_narrative(narrative)
+```
 
+Complete documentation is available at the [narrator](https://denisabd.github.io/narrator/) package website
```

