# Comparing `tmp/spinelibs-0.0.14.tar.gz` & `tmp/spinelibs-0.0.15.tar.gz`

## Comparing `spinelibs-0.0.14.tar` & `spinelibs-0.0.15.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 spinelibs-0.0.14/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/general/GUIDColumn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/general/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/console/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/console/console_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/csv/__init__.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/csv/csv_reader.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/csv/csv_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/sql/__init__.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/sql/sql_reader.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/polars/steps/io/sql/sql_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/console/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/console/console_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/csv/__init__.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/csv/csv_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hdfs/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hdfs/hdfs_reader.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hdfs/hdfs_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hive/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hive/hive_reader.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hive/hive_writer.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/hive/sql_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/jdbc/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/jdbc/jdbc_reader.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/jdbc/jdbc_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/mssql/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/mssql/mssql_reader.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 spinelibs-0.0.14/spinelibs/spark/steps/io/mssql/mssql_writer.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 spinelibs-0.0.14/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 spinelibs-0.0.14/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 spinelibs-0.0.14/README.md
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 spinelibs-0.0.14/pyproject.toml
--rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 spinelibs-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/__init__.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 spinelibs-0.0.15/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/general/GUIDColumn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/general/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/console/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/console/console_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/csv/__init__.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/csv/csv_reader.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/csv/csv_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/sql/__init__.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/sql/sql_reader.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/polars/steps/io/sql/sql_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/console/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/console/console_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/csv/__init__.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/csv/csv_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hdfs/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hdfs/hdfs_reader.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hdfs/hdfs_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hive/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hive/hive_reader.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hive/hive_writer.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/hive/sql_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/jdbc/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/jdbc/jdbc_reader.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/jdbc/jdbc_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/mssql/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/mssql/mssql_reader.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 spinelibs-0.0.15/spinelibs/spark/steps/io/mssql/mssql_writer.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 spinelibs-0.0.15/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 spinelibs-0.0.15/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 spinelibs-0.0.15/README.md
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 spinelibs-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 spinelibs-0.0.15/PKG-INFO
```

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/general/GUIDColumn.py` & `spinelibs-0.0.15/spinelibs/polars/steps/general/GUIDColumn.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/io/console/console_writer.py` & `spinelibs-0.0.15/spinelibs/polars/steps/io/console/console_writer.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/io/csv/csv_reader.py` & `spinelibs-0.0.15/spinelibs/polars/steps/io/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/io/csv/csv_writer.py` & `spinelibs-0.0.15/spinelibs/polars/steps/io/csv/csv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
         self.path = path
         self.sep = sep
         self.batch_size = batch_size
 
     async def process(self, ctx: SpinePolarsContext, df: PolarsDataFrame = None) -> PolarsDataFrame:
         ctx.logger.info(f"Writing CSV to {self.path} with headers={self.headers}")
         writer = df.collect().write_csv if ctx.lazy else df.write_csv
-        writer(self.path, has_header=self.headers, batch_size=self.batch_size, sep=self.sep)
+        writer(self.path, has_header=self.headers, batch_size=self.batch_size, separator=self.sep)
         return df
```

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/io/sql/sql_reader.py` & `spinelibs-0.0.15/spinelibs/polars/steps/io/sql/sql_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/polars/steps/io/sql/sql_writer.py` & `spinelibs-0.0.15/spinelibs/polars/steps/io/sql/sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/csv/csv_reader.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/hdfs/hdfs_reader.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/hdfs/hdfs_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/hdfs/hdfs_writer.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/hdfs/hdfs_writer.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/hive/hive_reader.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/hive/hive_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/hive/hive_writer.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/hive/hive_writer.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/hive/sql_reader.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/hive/sql_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/jdbc/jdbc_reader.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/jdbc/jdbc_reader.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/spinelibs/spark/steps/io/jdbc/jdbc_writer.py` & `spinelibs-0.0.15/spinelibs/spark/steps/io/jdbc/jdbc_writer.py`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/.gitignore` & `spinelibs-0.0.15/.gitignore`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/LICENSE` & `spinelibs-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `spinelibs-0.0.14/pyproject.toml` & `spinelibs-0.0.15/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "spinelibs"
 description = "Libs for spine project"
 
 readme = "README.md"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
     { name = "Shahar Luftig", email = "shaharluftig@gmail.com" },
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
 keywords = ["dataframe", "dag", "core"]
```

### Comparing `spinelibs-0.0.14/PKG-INFO` & `spinelibs-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinelibs
-Version: 0.0.14
+Version: 0.0.15
 Summary: Libs for spine project
 Project-URL: Homepage, https://github.com/shaharluftig/spine
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

