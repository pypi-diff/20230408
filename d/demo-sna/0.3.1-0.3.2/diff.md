# Comparing `tmp/demo_sna-0.3.1.tar.gz` & `tmp/demo_sna-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demo_sna-0.3.1.tar", last modified: Sat Apr  8 20:14:30 2023, max compression
+gzip compressed data, was "demo_sna-0.3.2.tar", last modified: Sat Apr  8 20:28:38 2023, max compression
```

## Comparing `demo_sna-0.3.1.tar` & `demo_sna-0.3.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.367965 demo_sna-0.3.1/
--rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3619 2023-03-28 19:17:05.000000 demo_sna-0.3.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-03-28 19:17:05.000000 demo_sna-0.3.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-03-28 19:17:05.000000 demo_sna-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1113 2023-04-08 20:14:30.369105 demo_sna-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-03-29 10:28:31.000000 demo_sna-0.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.284368 demo_sna-0.3.1/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 demo_sna-0.3.1/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.296199 demo_sna-0.3.1/demo_sna/
--rw-rw-rw-   0        0        0      130 2023-03-28 19:17:05.000000 demo_sna-0.3.1/demo_sna/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-03-28 11:35:04.000000 demo_sna-0.3.1/demo_sna/aned.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.309724 demo_sna-0.3.1/demo_sna/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.1/demo_sna/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.312202 demo_sna-0.3.1/demo_sna/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.1/demo_sna/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-04-01 08:52:56.000000 demo_sna-0.3.1/demo_sna/arabiner/bin/infer.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.317388 demo_sna-0.3.1/demo_sna/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.1/demo_sna/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-03-29 20:22:54.000000 demo_sna-0.3.1/demo_sna/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 demo_sna-0.3.1/demo_sna/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0      446 2023-03-28 19:17:05.000000 demo_sna-0.3.1/demo_sna/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.320494 demo_sna-0.3.1/demo_sna/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 demo_sna-0.3.1/demo_sna/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7430 2023-04-08 19:52:51.000000 demo_sna-0.3.1/demo_sna/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.333049 demo_sna-0.3.1/demo_sna/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 demo_sna-0.3.1/demo_sna/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 demo_sna-0.3.1/demo_sna/morph/charsets.py
--rw-rw-rw-   0        0        0     2803 2023-04-08 19:53:06.000000 demo_sna-0.3.1/demo_sna/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0    14406 2023-04-08 20:13:56.000000 demo_sna-0.3.1/demo_sna/morph/morph_tagger.py
--rw-rw-rw-   0        0        0      197 2023-04-01 20:15:05.000000 demo_sna-0.3.1/demo_sna/morph/serializers.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 demo_sna-0.3.1/demo_sna/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-08 19:53:07.000000 demo_sna-0.3.1/demo_sna/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0     6053 2023-04-05 20:55:34.000000 demo_sna-0.3.1/demo_sna/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.343263 demo_sna-0.3.1/demo_sna/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 demo_sna-0.3.1/demo_sna/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 demo_sna-0.3.1/demo_sna/salma/implication.py
--rw-rw-rw-   0        0        0      513 2023-04-08 09:06:50.000000 demo_sna-0.3.1/demo_sna/salma/tokenizers_words.py
--rw-rw-rw-   0        0        0    17930 2023-02-26 06:10:53.000000 demo_sna-0.3.1/demo_sna/salma/views.py
--rw-rw-rw-   0        0        0     7710 2023-04-06 11:49:15.000000 demo_sna-0.3.1/demo_sna/salma/wsd.py
--rw-rw-rw-   0        0        0     1089 2023-04-01 19:55:10.000000 demo_sna-0.3.1/demo_sna/wsd.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.307721 demo_sna-0.3.1/demo_sna.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-08 20:14:30.000000 demo_sna-0.3.1/demo_sna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2023-04-08 20:14:30.000000 demo_sna-0.3.1/demo_sna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 20:14:30.000000 demo_sna-0.3.1/demo_sna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-08 20:14:30.000000 demo_sna-0.3.1/demo_sna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-08 20:11:58.000000 demo_sna-0.3.1/demo_sna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-08 20:14:30.000000 demo_sna-0.3.1/demo_sna.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.363966 demo_sna-0.3.1/docs/
--rw-rw-rw-   0        0        0      625 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/authors.rst
--rw-rw-rw-   0        0        0     4907 2023-04-08 19:52:39.000000 demo_sna-0.3.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/history.rst
--rw-rw-rw-   0        0        0      321 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/index.rst
--rw-rw-rw-   0        0        0     1145 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/readme.rst
--rw-rw-rw-   0        0        0       70 2023-03-28 19:17:05.000000 demo_sna-0.3.1/docs/usage.rst
--rw-rw-rw-   0        0        0      399 2023-04-08 20:14:30.370814 demo_sna-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-08 20:14:22.000000 demo_sna-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:14:30.367427 demo_sna-0.3.1/tests/
--rw-rw-rw-   0        0        0       35 2023-03-28 19:17:05.000000 demo_sna-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0      397 2023-04-08 19:53:09.000000 demo_sna-0.3.1/tests/test_demo.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.616115 demo_sna-0.3.2/
+-rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3619 2023-03-28 19:17:05.000000 demo_sna-0.3.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-03-28 19:17:05.000000 demo_sna-0.3.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-03-28 19:17:05.000000 demo_sna-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1113 2023-04-08 20:28:38.617248 demo_sna-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-03-29 10:28:31.000000 demo_sna-0.3.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.524824 demo_sna-0.3.2/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 demo_sna-0.3.2/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.535514 demo_sna-0.3.2/demo_sna/
+-rw-rw-rw-   0        0        0      130 2023-03-28 19:17:05.000000 demo_sna-0.3.2/demo_sna/__init__.py
+-rw-rw-rw-   0        0        0     1671 2023-03-28 11:35:04.000000 demo_sna-0.3.2/demo_sna/aned.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.549804 demo_sna-0.3.2/demo_sna/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.2/demo_sna/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.552124 demo_sna-0.3.2/demo_sna/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.2/demo_sna/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-04-01 08:52:56.000000 demo_sna-0.3.2/demo_sna/arabiner/bin/infer.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.557255 demo_sna-0.3.2/demo_sna/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 demo_sna-0.3.2/demo_sna/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-03-29 20:22:54.000000 demo_sna-0.3.2/demo_sna/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 demo_sna-0.3.2/demo_sna/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0      446 2023-03-28 19:17:05.000000 demo_sna-0.3.2/demo_sna/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.562297 demo_sna-0.3.2/demo_sna/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 demo_sna-0.3.2/demo_sna/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7430 2023-04-08 19:52:51.000000 demo_sna-0.3.2/demo_sna/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.576933 demo_sna-0.3.2/demo_sna/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 demo_sna-0.3.2/demo_sna/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 demo_sna-0.3.2/demo_sna/morph/charsets.py
+-rw-rw-rw-   0        0        0     2803 2023-04-08 19:53:06.000000 demo_sna-0.3.2/demo_sna/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0    14406 2023-04-08 20:13:56.000000 demo_sna-0.3.2/demo_sna/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0      197 2023-04-01 20:15:05.000000 demo_sna-0.3.2/demo_sna/morph/serializers.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 demo_sna-0.3.2/demo_sna/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-08 19:53:07.000000 demo_sna-0.3.2/demo_sna/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0     6053 2023-04-05 20:55:34.000000 demo_sna-0.3.2/demo_sna/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.588649 demo_sna-0.3.2/demo_sna/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 demo_sna-0.3.2/demo_sna/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 demo_sna-0.3.2/demo_sna/salma/implication.py
+-rw-rw-rw-   0        0        0      513 2023-04-08 09:06:50.000000 demo_sna-0.3.2/demo_sna/salma/tokenizers_words.py
+-rw-rw-rw-   0        0        0    17930 2023-02-26 06:10:53.000000 demo_sna-0.3.2/demo_sna/salma/views.py
+-rw-rw-rw-   0        0        0     7710 2023-04-06 11:49:15.000000 demo_sna-0.3.2/demo_sna/salma/wsd.py
+-rw-rw-rw-   0        0        0     1089 2023-04-01 19:55:10.000000 demo_sna-0.3.2/demo_sna/wsd.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.546772 demo_sna-0.3.2/demo_sna.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-08 20:28:38.000000 demo_sna-0.3.2/demo_sna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-04-08 20:28:38.000000 demo_sna-0.3.2/demo_sna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 20:28:38.000000 demo_sna-0.3.2/demo_sna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-08 20:28:38.000000 demo_sna-0.3.2/demo_sna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-08 20:11:58.000000 demo_sna-0.3.2/demo_sna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-08 20:28:38.000000 demo_sna-0.3.2/demo_sna.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.607983 demo_sna-0.3.2/docs/
+-rw-rw-rw-   0        0        0      625 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     4907 2023-04-08 19:52:39.000000 demo_sna-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/history.rst
+-rw-rw-rw-   0        0        0      321 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1145 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       70 2023-03-28 19:17:05.000000 demo_sna-0.3.2/docs/usage.rst
+-rw-rw-rw-   0        0        0      399 2023-04-08 20:28:38.618246 demo_sna-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-04-08 20:28:31.000000 demo_sna-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 20:28:38.614043 demo_sna-0.3.2/tests/
+-rw-rw-rw-   0        0        0       35 2023-03-28 19:17:05.000000 demo_sna-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-04-08 19:53:09.000000 demo_sna-0.3.2/tests/test_demo.py
```

### Comparing `demo_sna-0.3.1/CONTRIBUTING.rst` & `demo_sna-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/LICENSE` & `demo_sna-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/PKG-INFO` & `demo_sna-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demo_sna
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/demo
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: demo_sna
 Requires-Python: >=3.10
```

### Comparing `demo_sna-0.3.1/README.rst` & `demo_sna-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/data/my_data.pickle` & `demo_sna-0.3.2/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/aned.py` & `demo_sna-0.3.2/demo_sna/aned.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/arabiner/bin/infer.py` & `demo_sna-0.3.2/demo_sna/arabiner/bin/infer.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/arabiner/utils/data.py` & `demo_sna-0.3.2/demo_sna/arabiner/utils/data.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/arabiner/utils/helpers.py` & `demo_sna-0.3.2/demo_sna/arabiner/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/jaccard/jaccardFunction.py` & `demo_sna-0.3.2/demo_sna/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/morph/charsets.py` & `demo_sna-0.3.2/demo_sna/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/morph/lemmatizeSentence.py` & `demo_sna-0.3.2/demo_sna/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/morph/morph_tagger.py` & `demo_sna-0.3.2/demo_sna/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/morph/tokenizers_words.py` & `demo_sna-0.3.2/demo_sna/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/parser.py` & `demo_sna-0.3.2/demo_sna/parser.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/salma/implication.py` & `demo_sna-0.3.2/demo_sna/salma/implication.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/salma/tokenizers_words.py` & `demo_sna-0.3.2/demo_sna/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/salma/views.py` & `demo_sna-0.3.2/demo_sna/salma/views.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/salma/wsd.py` & `demo_sna-0.3.2/demo_sna/salma/wsd.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna/wsd.py` & `demo_sna-0.3.2/demo_sna/wsd.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/demo_sna.egg-info/PKG-INFO` & `demo_sna-0.3.2/demo_sna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demo-sna
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/demo
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: demo_sna
 Requires-Python: >=3.10
```

### Comparing `demo_sna-0.3.1/demo_sna.egg-info/SOURCES.txt` & `demo_sna-0.3.2/demo_sna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/docs/Makefile` & `demo_sna-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/docs/conf.py` & `demo_sna-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/docs/installation.rst` & `demo_sna-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/docs/make.bat` & `demo_sna-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.1/setup.py` & `demo_sna-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,10 +60,10 @@
     include_package_data=True,
     keywords='demo_sna',
     name='demo_sna',
     packages=find_packages(include=['demo_sna', 'demo_sna.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/demo',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,    
 )
```

