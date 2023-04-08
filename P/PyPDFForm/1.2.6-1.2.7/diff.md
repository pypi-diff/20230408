# Comparing `tmp/PyPDFForm-1.2.6.tar.gz` & `tmp/PyPDFForm-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.6.tar", last modified: Fri Apr  7 19:13:04 2023, max compression
+gzip compressed data, was "PyPDFForm-1.2.7.tar", last modified: Sat Apr  8 16:18:06 2023, max compression
```

## Comparing `PyPDFForm-1.2.6.tar` & `PyPDFForm-1.2.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:06.553081 PyPDFForm-1.2.7/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 16:18:06.000000 PyPDFForm-1.2.7/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:18:06.557081 PyPDFForm-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 16:17:50.000000 PyPDFForm-1.2.7/setup.py
```

### Comparing `PyPDFForm-1.2.6/LICENSE` & `PyPDFForm-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PKG-INFO` & `PyPDFForm-1.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.6
+Version: 1.2.7
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,18 +32,17 @@
 Install using [pip](https://pip.pypa.io/en/stable/):
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
+![Check out the GitHub repository for a live demo if you can't see it here.](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
-![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
-
-A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
+A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
 
 PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join(
@@ -68,15 +67,15 @@
             },
         )
         .read()
     )
 ```
 
 After running the above code snippet you can find `output.pdf` at the location you specified, 
-and it should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_filled.pdf).
+and it should look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_filled.pdf).
 
 ## Documentation
 
 [Examples](https://github.com/chinapandaman/PyPDFForm/blob/master/docs/examples.md)
 
 ## How to Contribute
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.6 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.7 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
@@ -11,28 +11,29 @@
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
-en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
-form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
-master/pdf_samples/sample_template.pdf). Download it and try: ```python import
-os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
-os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
-Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
-= os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
-you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
-as output: output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill(
-{ "test": "test_1", "check": True, "test_2": "test_2", "check_2": False,
-"test_3": "test_3", "check_3": True, }, ) .read() ) ``` After running the above
-code snippet you can find `output.pdf` at the location you specified, and it
-should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/
+en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
+out the GitHub repository for a live demo if you can't see it here.](https://
+github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF form can
+be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/
+pdf_samples/sample_template.pdf). Download it and try: ```python import os from
+PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join
+( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) # Change this to
+where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM = os.path.join
+( os.path.expanduser("~"), "output.pdf" ) # Change this to where you wish to
+put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+") as output:
+output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill( { "test":
+"test_1", "check": True, "test_2": "test_2", "check_2": False, "test_3":
+"test_3", "check_3": True, }, ) .read() ) ``` After running the above code
+snippet you can find `output.pdf` at the location you specified, and it should
+look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/
 pdf_samples/sample_filled.pdf). ## Documentation [Examples](https://github.com/
 chinapandaman/PyPDFForm/blob/master/docs/examples.md) ## How to Contribute If
 you wish to improve this library, there is one specific way you can contribute
 on top of the usual open source project norms such as issues and pull requests.
 It is difficult to make sure that the library supports all the PDF form
 creating tools out there. So if you run into a case where the library does not
 work for certain PDF forms created by certain tools, feel free to open an issue
```

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/constants.py` & `PyPDFForm-1.2.7/PyPDFForm/core/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/filler.py` & `PyPDFForm-1.2.7/PyPDFForm/core/filler.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/font.py` & `PyPDFForm-1.2.7/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/image.py` & `PyPDFForm-1.2.7/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/patterns.py` & `PyPDFForm-1.2.7/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/template.py` & `PyPDFForm-1.2.7/PyPDFForm/core/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/utils.py` & `PyPDFForm-1.2.7/PyPDFForm/core/utils.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/core/watermark.py` & `PyPDFForm-1.2.7/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/element.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/template.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/middleware/text.py` & `PyPDFForm-1.2.7/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm/wrapper.py` & `PyPDFForm-1.2.7/PyPDFForm/wrapper.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.2.7/PyPDFForm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.6
+Version: 1.2.7
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,18 +32,17 @@
 Install using [pip](https://pip.pypa.io/en/stable/):
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
+![Check out the GitHub repository for a live demo if you can't see it here.](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
-![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
-
-A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
+A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
 
 PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join(
@@ -68,15 +67,15 @@
             },
         )
         .read()
     )
 ```
 
 After running the above code snippet you can find `output.pdf` at the location you specified, 
-and it should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_filled.pdf).
+and it should look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_filled.pdf).
 
 ## Documentation
 
 [Examples](https://github.com/chinapandaman/PyPDFForm/blob/master/docs/examples.md)
 
 ## How to Contribute
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.6 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.7 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
@@ -11,28 +11,29 @@
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
-en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
-form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
-master/pdf_samples/sample_template.pdf). Download it and try: ```python import
-os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
-os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
-Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
-= os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
-you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
-as output: output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill(
-{ "test": "test_1", "check": True, "test_2": "test_2", "check_2": False,
-"test_3": "test_3", "check_3": True, }, ) .read() ) ``` After running the above
-code snippet you can find `output.pdf` at the location you specified, and it
-should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/
+en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
+out the GitHub repository for a live demo if you can't see it here.](https://
+github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF form can
+be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/
+pdf_samples/sample_template.pdf). Download it and try: ```python import os from
+PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join
+( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) # Change this to
+where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM = os.path.join
+( os.path.expanduser("~"), "output.pdf" ) # Change this to where you wish to
+put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+") as output:
+output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill( { "test":
+"test_1", "check": True, "test_2": "test_2", "check_2": False, "test_3":
+"test_3", "check_3": True, }, ) .read() ) ``` After running the above code
+snippet you can find `output.pdf` at the location you specified, and it should
+look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/
 pdf_samples/sample_filled.pdf). ## Documentation [Examples](https://github.com/
 chinapandaman/PyPDFForm/blob/master/docs/examples.md) ## How to Contribute If
 you wish to improve this library, there is one specific way you can contribute
 on top of the usual open source project norms such as issues and pull requests.
 It is difficult to make sure that the library supports all the PDF form
 creating tools out there. So if you run into a case where the library does not
 work for certain PDF forms created by certain tools, feel free to open an issue
```

### Comparing `PyPDFForm-1.2.6/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.2.7/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.6/README.md` & `PyPDFForm-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 Install using [pip](https://pip.pypa.io/en/stable/):
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
+![Check out the GitHub repository for a live demo if you can't see it here.](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
-![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
-
-A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
+A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
 
 PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join(
@@ -55,15 +54,15 @@
             },
         )
         .read()
     )
 ```
 
 After running the above code snippet you can find `output.pdf` at the location you specified, 
-and it should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_filled.pdf).
+and it should look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/pdf_samples/sample_filled.pdf).
 
 ## Documentation
 
 [Examples](https://github.com/chinapandaman/PyPDFForm/blob/master/docs/examples.md)
 
 ## How to Contribute
```

#### html2text {}

```diff
@@ -5,28 +5,29 @@
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
-en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
-form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
-master/pdf_samples/sample_template.pdf). Download it and try: ```python import
-os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
-os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
-Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
-= os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
-you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
-as output: output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill(
-{ "test": "test_1", "check": True, "test_2": "test_2", "check_2": False,
-"test_3": "test_3", "check_3": True, }, ) .read() ) ``` After running the above
-code snippet you can find `output.pdf` at the location you specified, and it
-should look like [this](https://github.com/chinapandaman/PyPDFForm/blob/master/
+en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
+out the GitHub repository for a live demo if you can't see it here.](https://
+github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF form can
+be found [here](https://github.com/chinapandaman/PyPDFForm/raw/master/
+pdf_samples/sample_template.pdf). Download it and try: ```python import os from
+PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM = os.path.join
+( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) # Change this to
+where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM = os.path.join
+( os.path.expanduser("~"), "output.pdf" ) # Change this to where you wish to
+put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+") as output:
+output.write( PyPDFForm(PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM) .fill( { "test":
+"test_1", "check": True, "test_2": "test_2", "check_2": False, "test_3":
+"test_3", "check_3": True, }, ) .read() ) ``` After running the above code
+snippet you can find `output.pdf` at the location you specified, and it should
+look like [this](https://github.com/chinapandaman/PyPDFForm/raw/master/
 pdf_samples/sample_filled.pdf). ## Documentation [Examples](https://github.com/
 chinapandaman/PyPDFForm/blob/master/docs/examples.md) ## How to Contribute If
 you wish to improve this library, there is one specific way you can contribute
 on top of the usual open source project norms such as issues and pull requests.
 It is difficult to make sure that the library supports all the PDF form
 creating tools out there. So if you run into a case where the library does not
 work for certain PDF forms created by certain tools, feel free to open an issue
```

### Comparing `PyPDFForm-1.2.6/setup.py` & `PyPDFForm-1.2.7/setup.py`

 * *Files identical despite different names*

