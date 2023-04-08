# Comparing `tmp/spark_quality_rules_tools-0.2.1.tar.gz` & `tmp/spark_quality_rules_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.1.tar", last modified: Sat Oct 22 17:33:12 2022, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.2.2.tar", last modified: Fri Apr  7 23:30:08 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.1.tar` & `spark_quality_rules_tools-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.571555 spark_quality_rules_tools-0.2.1/
--rw-rw-rw-   0        0        0     1092 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      155 2022-07-28 23:32:51.000000 spark_quality_rules_tools-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4481 2022-10-22 17:33:12.571555 spark_quality_rules_tools-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3672 2022-10-17 12:27:14.000000 spark_quality_rules_tools-0.2.1/README.md
--rw-rw-rw-   0        0        0       86 2022-10-22 17:33:12.587146 spark_quality_rules_tools-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1258 2022-10-22 17:32:32.000000 spark_quality_rules_tools-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.524649 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2263 2022-10-20 17:02:45.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.540274 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    31605 2022-10-20 17:02:45.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.555898 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      216 2022-07-24 23:59:58.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2472 2022-07-12 20:46:27.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/dataframe.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.555898 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/external/
--rw-rw-rw-   0        0        0    71803 2022-10-17 12:27:14.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/external/folder_process.png
--rw-rw-rw-   0        0        0     1056 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/memory.py
--rw-rw-rw-   0        0        0     2113 2022-07-28 23:32:51.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.571555 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-07-28 16:09:02.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    17801 2022-10-22 17:32:32.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     2894 2022-10-21 21:13:53.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.571555 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/templates/table.html
-drwxrwxrwx   0        0        0        0 2022-10-22 17:33:12.540274 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4481 2022-10-22 17:33:12.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2022-10-22 17:33:12.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-22 17:33:12.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2022-10-22 17:33:12.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2022-10-22 17:33:12.000000 spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.014212 spark_quality_rules_tools-0.2.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      155 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4481 2023-04-07 23:30:08.014212 spark_quality_rules_tools-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3672 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-07 23:30:08.015210 spark_quality_rules_tools-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-04-07 23:29:06.000000 spark_quality_rules_tools-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.934192 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2263 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.963199 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    31605 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.994205 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      216 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2472 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.999207 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/
+-rw-rw-rw-   0        0        0    71803 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/folder_process.png
+-rw-rw-rw-   0        0        0     1056 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/memory.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.008208 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    17801 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     2894 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:08.013210 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/table.html
+drwxrwxrwx   0        0        0        0 2023-04-07 23:30:07.955196 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4481 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-07 23:30:07.000000 spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.1/LICENSE` & `spark_quality_rules_tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/PKG-INFO` & `spark_quality_rules_tools-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 Keywords: spark,dq,rules,hammurabies
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spark_quality_rules_tools-0.2.1/README.md` & `spark_quality_rules_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/setup.py` & `spark_quality_rules_tools-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.1',
+    version='0.2.2',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/dataframe.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/external/folder_process.png` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/external/folder_process.png`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/memory.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools/utils/templates/table.html` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 Keywords: spark,dq,rules,hammurabies
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spark_quality_rules_tools-0.2.1/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.2.2/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

