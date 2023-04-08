# Comparing `tmp/subete-0.9.2.tar.gz` & `tmp/subete-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subete-0.9.2.tar", last modified: Fri Apr 29 16:25:05 2022, max compression
+gzip compressed data, was "subete-0.9.3.tar", last modified: Fri Apr 29 18:09:38 2022, max compression
```

## Comparing `subete-0.9.2.tar` & `subete-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 16:25:05.794714 subete-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-29 16:24:51.000000 subete-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-04-29 16:25:05.794714 subete-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-29 16:24:51.000000 subete-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-29 16:24:51.000000 subete-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-29 16:25:05.798715 subete-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-04-29 16:24:51.000000 subete-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 16:25:05.794714 subete-0.9.2/subete/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-04-29 16:24:51.000000 subete-0.9.2/subete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34070 2022-04-29 16:24:51.000000 subete-0.9.2/subete/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 16:25:05.794714 subete-0.9.2/subete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-04-29 16:25:05.000000 subete-0.9.2/subete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-04-29 16:25:05.000000 subete-0.9.2/subete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 16:25:05.000000 subete-0.9.2/subete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-29 16:25:05.000000 subete-0.9.2/subete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-29 16:25:05.000000 subete-0.9.2/subete.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 18:09:38.493127 subete-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-29 18:09:20.000000 subete-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-04-29 18:09:38.493127 subete-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-29 18:09:20.000000 subete-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-29 18:09:20.000000 subete-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-29 18:09:38.493127 subete-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-04-29 18:09:20.000000 subete-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 18:09:38.489127 subete-0.9.3/subete/
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2022-04-29 18:09:20.000000 subete-0.9.3/subete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34369 2022-04-29 18:09:20.000000 subete-0.9.3/subete/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 18:09:38.489127 subete-0.9.3/subete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-04-29 18:09:37.000000 subete-0.9.3/subete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-04-29 18:09:38.000000 subete-0.9.3/subete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 18:09:37.000000 subete-0.9.3/subete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-29 18:09:38.000000 subete-0.9.3/subete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-29 18:09:38.000000 subete-0.9.3/subete.egg-info/top_level.txt
```

### Comparing `subete-0.9.2/LICENSE` & `subete-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subete-0.9.2/PKG-INFO` & `subete-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: subete
-Version: 0.9.2
+Version: 0.9.3
 Summary: The Sample Programs API in Python
 Home-page: https://github.com/TheRenegadeCoder/subete
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Subete
 
 Subete is a Python library for interacting with the Sample Programs
 repository. It works by cloning the repository and analyzing its
```

### Comparing `subete-0.9.2/setup.py` & `subete-0.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     print("WARNING: sphinx not available")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 MAJOR = 0
 MINOR = 9
-PATCH = 2
+PATCH = 3
 
 name = "subete"
 version = f"{MAJOR}.{MINOR}"
 release = f"{MAJOR}.{MINOR}.{PATCH}"
 setuptools.setup(
     name=name,
     version=release,
     author="The Renegade Coder",
     author_email="jeremy.grifski@therenegadecoder.com",
     description="The Sample Programs API in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheRenegadeCoder/subete",
     packages=setuptools.find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
         "PyYAML>=5",
         "GitPython>=3"
     ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

### Comparing `subete-0.9.2/subete/__init__.py` & `subete-0.9.3/subete/__init__.py`

 * *Files identical despite different names*

### Comparing `subete-0.9.2/subete/repo.py` & `subete-0.9.3/subete/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,16 +215,16 @@
         to point at archive (for historical purposes). This is normally
         a non-issue if the directory is generated using Git, but can be more
         annoying if the user provides a source. 
 
         :return: a path to the documentation directory
         """
         if not source_dir:
-            return os.path.join(self._temp_dir.name, "docs", "docs")
-        return os.path.join(source_dir, os.pardir, "docs", "docs")
+            return os.path.join(self._temp_dir.name, "docs", "sources")
+        return os.path.join(source_dir, os.pardir, "docs", "sources")
 
 
 class LanguageCollection:
     """
     An object representing a collection of sample programs files for a particular programming language.
 
     :param str name: the name of the language (e.g., python)
@@ -821,15 +821,15 @@
     """
     An object representing a Project in the Sample Programs repo.
 
     :param str name: the name of the project in its pathlike form (e.g., hello-world) 
     """
 
     def __init__(self, name: str):
-        self._name: str = name
+        self._name: str = Project._generate_name(name)
         self._requirements_url: str = self._generate_requirements_url()
 
     def __str__(self) -> str:
         logger.info(f"Generating name from {self._name}")
         return (
             self._name.replace("-", " ").title() 
             if len(self._name) > 3 
@@ -895,11 +895,20 @@
         """
         A helper method for generating the expected requirements URL 
         for this sample program.
 
         :return: the expected requirements URL 
         """
         doc_url_base = "https://sampleprograms.io/projects"
-        if "export" in self.pathlike_name() or "import" in self.pathlike_name():
-            return f"{doc_url_base}/import-export"
-        else:
-            return f"{doc_url_base}/{self.pathlike_name()}"
+        return f"{doc_url_base}/{self.pathlike_name()}"
+
+    @staticmethod
+    def _generate_name(name: str) -> str:
+        """
+        Creates the project name from some input string.
+
+        :param str name: the name of the project in its pathlike form (e.g., hello-world)
+        :return: the name of the project in its pathlike form (e.g., hello-world)
+        """
+        if "export" in name or "import" in name:
+            return "import-export"
+        return name
```

### Comparing `subete-0.9.2/subete.egg-info/PKG-INFO` & `subete-0.9.3/subete.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: subete
-Version: 0.9.2
+Version: 0.9.3
 Summary: The Sample Programs API in Python
 Home-page: https://github.com/TheRenegadeCoder/subete
 Author: The Renegade Coder
 Author-email: jeremy.grifski@therenegadecoder.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Subete
 
 Subete is a Python library for interacting with the Sample Programs
 repository. It works by cloning the repository and analyzing its
```

