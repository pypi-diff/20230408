# Comparing `tmp/pysmells-1.0.4.tar.gz` & `tmp/pysmells-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.4.tar", last modified: Sat Apr  8 00:04:55 2023, max compression
+gzip compressed data, was "pysmells-1.0.5.tar", last modified: Sat Apr  8 17:12:16 2023, max compression
```

## Comparing `pysmells-1.0.4.tar` & `pysmells-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 00:04:55.351087 pysmells-1.0.4/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.4/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)     2114 2023-04-08 00:04:55.350407 pysmells-1.0.4/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.4/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 00:04:55.338337 pysmells-1.0.4/pysmells/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.4/pysmells/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3987 2023-04-07 22:49:21.000000 pysmells-1.0.4/pysmells/analyze.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 00:04:55.348019 pysmells-1.0.4/pysmells.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)     2114 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      261 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-08 00:04:55.000000 pysmells-1.0.4/pysmells.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-08 00:04:55.351380 pysmells-1.0.4/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)     1369 2023-04-08 00:04:46.000000 pysmells-1.0.4/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.945591 pysmells-1.0.5/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.5/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2143 2023-04-08 17:12:16.944827 pysmells-1.0.5/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.5/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.929927 pysmells-1.0.5/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.5/pysmells/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3459 2023-04-08 00:31:24.000000 pysmells-1.0.5/pysmells/analyze.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.942210 pysmells-1.0.5/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2143 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      261 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-08 17:12:16.945993 pysmells-1.0.5/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1398 2023-04-08 17:12:01.000000 pysmells-1.0.5/setup.py
```

### Comparing `pysmells-1.0.4/LICENSE` & `pysmells-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.4/PKG-INFO` & `pysmells-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
-Home-page: https://github.com/yourusername/pysmells
-Author: Marcos Paulo Alves de Sousa
+Home-page: https://github.com/pysmells/pysmells
+Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysmells-1.0.4/README.md` & `pysmells-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.4/pysmells.egg-info/PKG-INFO` & `pysmells-1.0.5/pysmells.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
-Home-page: https://github.com/yourusername/pysmells
-Author: Marcos Paulo Alves de Sousa
+Home-page: https://github.com/pysmells/pysmells
+Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysmells-1.0.4/setup.py` & `pysmells-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pysmells",
-    version="1.0.4",
-    author="Marcos Paulo Alves de Sousa",
+    version="1.0.5",
+    author="Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto",
     author_email="msousa@museu-goeldi.br",
     description="A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/pysmells",
+    url="https://github.com/pysmells/pysmells",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

