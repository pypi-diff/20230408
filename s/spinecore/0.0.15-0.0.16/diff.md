# Comparing `tmp/spinecore-0.0.15.tar.gz` & `tmp/spinecore-0.0.16.tar.gz`

## Comparing `spinecore-0.0.15.tar` & `spinecore-0.0.16.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 spinecore-0.0.15/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/context/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/context/base_context.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/context/polars_context.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/context/spark_context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/graphs.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/IContext.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/IExecutor.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/IStep.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/Logger.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/Workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/metaclasses/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/contract/metaclasses/singleton.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/dataframes/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/dataframes/pandas_dataframe.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/dataframes/polars_dataframe.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/dataframes/spark_dataframe.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/logging/__init__.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/logging/spine_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/steps/__init__.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/steps/polars_step.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/common/helpers/steps/spark_step.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/executors/__init__.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/executors/spine_executor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/executors/workflow_executors/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/executors/workflow_executors/async_workflow_executor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/tests/unit/executors/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/tests/unit/executors/test_spine_executor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/workflows/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 spinecore-0.0.15/spinecore/workflows/dag_workflow.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 spinecore-0.0.15/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 spinecore-0.0.15/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 spinecore-0.0.15/README.md
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 spinecore-0.0.15/pyproject.toml
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 spinecore-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 spinecore-0.0.16/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/context/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/context/base_context.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/context/polars_context.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/context/spark_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/__init__.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/graphs.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/IContext.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/IExecutor.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/IStep.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/Logger.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/Workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/metaclasses/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/contract/metaclasses/singleton.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/dataframes/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/dataframes/pandas_dataframe.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/dataframes/polars_dataframe.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/dataframes/spark_dataframe.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/logging/__init__.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/logging/spine_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/steps/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/steps/polars_step.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/common/helpers/steps/spark_step.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/executors/__init__.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/executors/spine_executor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/executors/workflow_executors/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/executors/workflow_executors/async_workflow_executor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/tests/unit/executors/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/tests/unit/executors/test_spine_executor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/workflows/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 spinecore-0.0.16/spinecore/workflows/dag_workflow.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 spinecore-0.0.16/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 spinecore-0.0.16/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 spinecore-0.0.16/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 spinecore-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 spinecore-0.0.16/PKG-INFO
```

### Comparing `spinecore-0.0.15/spinecore/common/context/base_context.py` & `spinecore-0.0.16/spinecore/common/context/base_context.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/context/polars_context.py` & `spinecore-0.0.16/spinecore/common/context/polars_context.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/context/spark_context.py` & `spinecore-0.0.16/spinecore/common/context/spark_context.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/helpers/graphs.py` & `spinecore-0.0.16/spinecore/common/helpers/graphs.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/helpers/contract/Workflow.py` & `spinecore-0.0.16/spinecore/common/helpers/contract/Workflow.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/helpers/logging/spine_logger.py` & `spinecore-0.0.16/spinecore/common/helpers/logging/spine_logger.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/helpers/steps/polars_step.py` & `spinecore-0.0.16/spinecore/common/helpers/steps/polars_step.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/common/helpers/steps/spark_step.py` & `spinecore-0.0.16/spinecore/common/helpers/steps/spark_step.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/executors/spine_executor.py` & `spinecore-0.0.16/spinecore/executors/spine_executor.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/executors/workflow_executors/async_workflow_executor.py` & `spinecore-0.0.16/spinecore/executors/workflow_executors/async_workflow_executor.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/tests/unit/executors/test_spine_executor.py` & `spinecore-0.0.16/spinecore/tests/unit/executors/test_spine_executor.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/spinecore/workflows/dag_workflow.py` & `spinecore-0.0.16/spinecore/workflows/dag_workflow.py`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/.gitignore` & `spinecore-0.0.16/.gitignore`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/LICENSE` & `spinecore-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `spinecore-0.0.15/pyproject.toml` & `spinecore-0.0.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 [project]
 name = "spinecore"
 description = "The core lib of spine library"
 readme = "README.md"
-version = "0.0.15"
+version = "0.0.16"
 
 authors = [
     { name = "Shahar Luftig", email = "shaharluftig@gmail.com" },
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
@@ -33,13 +33,13 @@
 dependencies = [
     "stringcase ~=1.2.0",
     "matplotlib ~=3.7.1",
     "networkx ~=3.0",
 ]
 
 [project.optional-dependencies]
-polars = ["polars ~=0.16.11", "pyarrow ~=11.0.0", "connectorx ~=0.3.2a2"]
+polars = ["polars ~=0.17.0", "pyarrow ~=11.0.0", "connectorx ~=0.3.2a2"]
 spark = ["pyspark ~=3.2.1"]
 all = ["spinecore[polars]", "spinecore[spark]"]
 
 [project.urls]
 "Homepage" = "https://github.com/shaharluftig/spine"
```

### Comparing `spinecore-0.0.15/PKG-INFO` & `spinecore-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinecore
-Version: 0.0.15
+Version: 0.0.16
 Summary: The core lib of spine library
 Project-URL: Homepage, https://github.com/shaharluftig/spine
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,15 +223,15 @@
 Requires-Dist: networkx~=3.0
 Requires-Dist: stringcase~=1.2.0
 Provides-Extra: all
 Requires-Dist: spinecore[polars]; extra == 'all'
 Requires-Dist: spinecore[spark]; extra == 'all'
 Provides-Extra: polars
 Requires-Dist: connectorx~=0.3.2a2; extra == 'polars'
-Requires-Dist: polars~=0.16.11; extra == 'polars'
+Requires-Dist: polars~=0.17.0; extra == 'polars'
 Requires-Dist: pyarrow~=11.0.0; extra == 'polars'
 Provides-Extra: spark
 Requires-Dist: pyspark~=3.2.1; extra == 'spark'
 Description-Content-Type: text/markdown
 
 # spinecore
```

