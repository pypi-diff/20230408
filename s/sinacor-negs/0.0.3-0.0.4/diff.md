# Comparing `tmp/sinacor_negs-0.0.3.tar.gz` & `tmp/sinacor_negs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinacor_negs-0.0.3.tar", last modified: Sat Apr  8 20:54:54 2023, max compression
+gzip compressed data, was "sinacor_negs-0.0.4.tar", last modified: Sat Apr  8 21:21:05 2023, max compression
```

## Comparing `sinacor_negs-0.0.3.tar` & `sinacor_negs-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.945923 sinacor_negs-0.0.3/
--rw-rw-rw-   0        0        0     1099 2023-04-08 18:19:42.000000 sinacor_negs-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      605 2023-04-08 20:54:54.944925 sinacor_negs-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-04-08 20:52:11.000000 sinacor_negs-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 20:54:54.945923 sinacor_negs-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-08 20:53:35.000000 sinacor_negs-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.934952 sinacor_negs-0.0.3/sinacor_negs/
--rw-rw-rw-   0        0        0       39 2023-04-08 20:54:25.000000 sinacor_negs-0.0.3/sinacor_negs/__init__.py
--rw-rw-rw-   0        0        0     4611 2023-04-08 20:54:26.000000 sinacor_negs-0.0.3/sinacor_negs/sinacor_negs.py
--rw-rw-rw-   0        0        0      166 2023-04-08 20:54:51.000000 sinacor_negs-0.0.3/sinacor_negs/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:54:54.942929 sinacor_negs-0.0.3/sinacor_negs.egg-info/
--rw-rw-rw-   0        0        0      605 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-08 20:54:54.000000 sinacor_negs-0.0.3/sinacor_negs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 21:21:05.628200 sinacor_negs-0.0.4/
+-rw-rw-rw-   0        0        0     1099 2023-04-08 18:19:42.000000 sinacor_negs-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1175 2023-04-08 21:21:05.627202 sinacor_negs-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-04-08 21:18:38.000000 sinacor_negs-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 21:21:05.628200 sinacor_negs-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-08 21:19:02.000000 sinacor_negs-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:21:05.615234 sinacor_negs-0.0.4/sinacor_negs/
+-rw-rw-rw-   0        0        0       39 2023-04-08 20:54:25.000000 sinacor_negs-0.0.4/sinacor_negs/__init__.py
+-rw-rw-rw-   0        0        0     4611 2023-04-08 20:54:26.000000 sinacor_negs-0.0.4/sinacor_negs/sinacor_negs.py
+-rw-rw-rw-   0        0        0      166 2023-04-08 20:59:42.000000 sinacor_negs-0.0.4/sinacor_negs/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:21:05.625208 sinacor_negs-0.0.4/sinacor_negs.egg-info/
+-rw-rw-rw-   0        0        0     1175 2023-04-08 21:21:05.000000 sinacor_negs-0.0.4/sinacor_negs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-08 21:21:05.000000 sinacor_negs-0.0.4/sinacor_negs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 21:21:05.000000 sinacor_negs-0.0.4/sinacor_negs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-08 21:21:05.000000 sinacor_negs-0.0.4/sinacor_negs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-08 21:21:05.000000 sinacor_negs-0.0.4/sinacor_negs.egg-info/top_level.txt
```

### Comparing `sinacor_negs-0.0.3/LICENSE.txt` & `sinacor_negs-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sinacor_negs-0.0.3/README.md` & `sinacor_negs-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # sinacor_negs
-'sinacor_negs' é uma lib feita para facilitar a leitura de arquivos negs.txt da bolsa (B3/Sinacor). A lib foi feita utilizando pandas e retorna os dados em forma de DataFrames (pandas).
+'sinacor_negs' é uma lib feita para facilitar a leitura de arquivos negs.txt da bolsa (B3/Sinacor). A lib foi feita utilizando pandas e retorna os dados em forma de DataFrames.
 
 ## Instalação
 `pip install sinacor_negs`
 
 ## Como usar
 ```python
 import sinacor_negs as snegs
 
 negs_txt_path = 'sample//negs.txt'
 
 negs = snegs.read_negs_txt(negs_txt_path)
 
-'''
-negs.header -> dataframe do header.
-negs.negs -> dataframe do negs (todos os negócios).
-negs.trailer -> dataframe do trailer.
-'''
-
+# negs.header -> dataframe do header.
+# negs.negs -> dataframe do negs (todos os negócios).
+# negs.trailer -> dataframe do trailer.
 ```
```

### Comparing `sinacor_negs-0.0.3/sinacor_negs/sinacor_negs.py` & `sinacor_negs-0.0.4/sinacor_negs/sinacor_negs.py`

 * *Files identical despite different names*

