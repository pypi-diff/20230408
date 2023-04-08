# Comparing `tmp/data_augmentation_GASPLN-0.1.5.tar.gz` & `tmp/data_augmentation_GASPLN-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_augmentation_GASPLN-0.1.5.tar", last modified: Thu Apr  6 12:41:58 2023, max compression
+gzip compressed data, was "data_augmentation_GASPLN-0.1.6.tar", last modified: Sat Apr  8 17:00:08 2023, max compression
```

## Comparing `data_augmentation_GASPLN-0.1.5.tar` & `data_augmentation_GASPLN-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:58.470900 data_augmentation_GASPLN-0.1.5/
--rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-04-06 12:41:58.470900 data_augmentation_GASPLN-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2135 2023-04-06 12:38:34.000000 data_augmentation_GASPLN-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:58.457901 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/
--rw-rw-rw-   0        0        0        0 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:58.463901 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/data/
--rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
--rw-rw-rw-   0        0        0     2606 2023-04-06 12:41:21.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:58.462900 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-06 12:41:58.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-04-06 12:41:58.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 12:41:58.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-06 12:41:58.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-06 12:41:58.000000 data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-06 12:41:58.471900 data_augmentation_GASPLN-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-06 12:41:14.000000 data_augmentation_GASPLN-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.488831 data_augmentation_GASPLN-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-04-08 17:00:08.488831 data_augmentation_GASPLN-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2462 2023-04-08 16:59:37.000000 data_augmentation_GASPLN-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.467715 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/
+-rw-rw-rw-   0        0        0        0 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.474717 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/
+-rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
+-rw-rw-rw-   0        0        0     3141 2023-04-08 16:34:07.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.474717 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-08 17:00:08.489831 data_augmentation_GASPLN-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-08 16:59:32.000000 data_augmentation_GASPLN-0.1.6/setup.py
```

### Comparing `data_augmentation_GASPLN-0.1.5/LICENSE` & `data_augmentation_GASPLN-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.5/README.md` & `data_augmentation_GASPLN-0.1.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 The first parameter is the text to be augmented, and the second parameter is the percentage of words to be replaced by synonyms (by default, and in this example, 50% of the words in the text).
 
 ### Back Translation
 
 The `back_translation()` function can be used for back translation. Here's an example:
 
 ```python
-da.back_translation("Data augmentation é uma técnica de aprendizado de máquina que aumenta o número de dados de treinamento, alterando os dados existentes de alguma forma a fim de criar novos dados.", 2)
+da.back_translation('Data augmentation é uma técnica de aprendizado de máquina que aumenta o número de dados de treinamento, alterando os dados existentes em conjuntos de dados de treinamento.', languages=['en', 'es', 'ru'], translator='google')
 ```
 
-The first parameter is the text to be augmented, and the second parameter is the number of translations to be performed. Currently, two options are available for the second parameter, 1 or 2, where:
+- The `first parameter` is the text to be augmented;
+- The `second parameter` is a list of languages to be used for back translation (by default it translates to English, Spanish and back to Portuguese*)
+    * It is not necessary to include Portuguese in the list of languages, as the text will be translated to Portuguese at the end of the process;
+- The `third parameter` is the translator to be used (by default it uses Google Translate).
 
-- 1 = Portuguese > English > Portuguese
-- 2 = Portuguese > Spanish > English > Portuguese
+A list of the available languages and translators can be found [here](https://pypi.org/project/translators/#supported-languages).
```

### Comparing `data_augmentation_GASPLN-0.1.5/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet` & `data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.5/setup.py` & `data_augmentation_GASPLN-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_augmentation_GASPLN',
-    version='0.1.5',
+    version='0.1.6',
     author='Artur Melchiori Cerri',
     author_email='arturmelchiori@gmail.com',
     description='Data augmentation for Portuguese language',
     install_requires=[
         "spacy",
         "nltk",
         "pandas",
```

