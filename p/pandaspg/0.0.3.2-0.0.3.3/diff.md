# Comparing `tmp/pandaspg-0.0.3.2.tar.gz` & `tmp/pandaspg-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandaspg-0.0.3.2.tar", last modified: Fri Apr  7 23:38:52 2023, max compression
+gzip compressed data, was "pandaspg-0.0.3.3.tar", last modified: Sat Apr  8 00:07:52 2023, max compression
```

## Comparing `pandaspg-0.0.3.2.tar` & `pandaspg-0.0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-07 23:38:52.031132 pandaspg-0.0.3.2/
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     1073 2023-04-07 20:28:54.000000 pandaspg-0.0.3.2/LICENSE
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4639 2023-04-07 23:38:52.031132 pandaspg-0.0.3.2/PKG-INFO
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     3986 2023-04-07 23:35:46.000000 pandaspg-0.0.3.2/README.md
-drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-07 23:38:52.031132 pandaspg-0.0.3.2/pandaspg/
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      242 2023-04-07 19:39:47.000000 pandaspg-0.0.3.2/pandaspg/__init__.py
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4763 2023-04-07 21:38:22.000000 pandaspg-0.0.3.2/pandaspg/main.py
-drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-07 23:38:52.031132 pandaspg-0.0.3.2/pandaspg.egg-info/
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4639 2023-04-07 23:38:52.000000 pandaspg-0.0.3.2/pandaspg.egg-info/PKG-INFO
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      198 2023-04-07 23:38:52.000000 pandaspg-0.0.3.2/pandaspg.egg-info/SOURCES.txt
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)        1 2023-04-07 23:38:52.000000 pandaspg-0.0.3.2/pandaspg.egg-info/dependency_links.txt
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)        9 2023-04-07 23:38:52.000000 pandaspg-0.0.3.2/pandaspg.egg-info/top_level.txt
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      725 2023-04-07 23:38:00.000000 pandaspg-0.0.3.2/pyproject.toml
--rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)       38 2023-04-07 23:38:52.031132 pandaspg-0.0.3.2/setup.cfg
+drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-08 00:07:52.973373 pandaspg-0.0.3.3/
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     1073 2023-04-07 20:28:54.000000 pandaspg-0.0.3.3/LICENSE
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4639 2023-04-08 00:07:52.970040 pandaspg-0.0.3.3/PKG-INFO
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     3986 2023-04-07 23:35:46.000000 pandaspg-0.0.3.3/README.md
+drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-08 00:07:52.970040 pandaspg-0.0.3.3/pandaspg/
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      242 2023-04-07 19:39:47.000000 pandaspg-0.0.3.3/pandaspg/__init__.py
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4850 2023-04-07 23:47:59.000000 pandaspg-0.0.3.3/pandaspg/main.py
+drwxr-xr-x   0 adolfoj   (1000) adolfoj   (1000)        0 2023-04-08 00:07:52.970040 pandaspg-0.0.3.3/pandaspg.egg-info/
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)     4639 2023-04-08 00:07:52.000000 pandaspg-0.0.3.3/pandaspg.egg-info/PKG-INFO
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      198 2023-04-08 00:07:52.000000 pandaspg-0.0.3.3/pandaspg.egg-info/SOURCES.txt
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)        1 2023-04-08 00:07:52.000000 pandaspg-0.0.3.3/pandaspg.egg-info/dependency_links.txt
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)        9 2023-04-08 00:07:52.000000 pandaspg-0.0.3.3/pandaspg.egg-info/top_level.txt
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)      725 2023-04-07 23:59:02.000000 pandaspg-0.0.3.3/pyproject.toml
+-rw-r--r--   0 adolfoj   (1000) adolfoj   (1000)       38 2023-04-08 00:07:52.973373 pandaspg-0.0.3.3/setup.cfg
```

### Comparing `pandaspg-0.0.3.2/LICENSE` & `pandaspg-0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandaspg-0.0.3.2/PKG-INFO` & `pandaspg-0.0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandaspg
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: This library contains several functions that allow you to migrate data from a CSV file or Pandas Dataframe into a PostgreSQL database using the libraries Psycopg2 and Pandas
 Author-email: Adolfo Jimenez <adolfoj@protonmail.com>
 Project-URL: Homepage, https://github.com/eadwulf/pandaspg
 Project-URL: Bug Tracker, https://github.com/eadwulf/pandaspg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandaspg-0.0.3.2/README.md` & `pandaspg-0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pandaspg-0.0.3.2/pandaspg/main.py` & `pandaspg-0.0.3.3/pandaspg/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,18 @@
     True if a table was created successfully, False otherwise
     """
 
     cursor = connection.cursor()
 
     # Generate the SQL command to create the table
     command = f"CREATE TABLE {table_name} ("
-    command += "id SERIAL PRIMARY KEY, "
+
+    # Define the primary key field if needed
+    if field_dict.get('id') is None:
+        command += "id SERIAL PRIMARY KEY, "
 
     for field, datatype in field_dict.items():
         command += f"{field} {datatype} NULL, "
 
     # Remove the last comma and space from the command
     command = command[:-2]
```

### Comparing `pandaspg-0.0.3.2/pandaspg.egg-info/PKG-INFO` & `pandaspg-0.0.3.3/pandaspg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandaspg
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: This library contains several functions that allow you to migrate data from a CSV file or Pandas Dataframe into a PostgreSQL database using the libraries Psycopg2 and Pandas
 Author-email: Adolfo Jimenez <adolfoj@protonmail.com>
 Project-URL: Homepage, https://github.com/eadwulf/pandaspg
 Project-URL: Bug Tracker, https://github.com/eadwulf/pandaspg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandaspg-0.0.3.2/pyproject.toml` & `pandaspg-0.0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pandaspg"
-version = "0.0.3.2"
+version = "0.0.3.3"
 authors = [
   { name="Adolfo Jimenez", email="adolfoj@protonmail.com" },
 ]
 description = "This library contains several functions that allow you to migrate data from a CSV file or Pandas Dataframe into a PostgreSQL database using the libraries Psycopg2 and Pandas"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

