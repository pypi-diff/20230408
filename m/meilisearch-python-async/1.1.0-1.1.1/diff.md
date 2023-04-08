# Comparing `tmp/meilisearch_python_async-1.1.0.tar.gz` & `tmp/meilisearch_python_async-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.1.0.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.1.1.tar", max compression
```

## Comparing `meilisearch_python_async-1.1.0.tar` & `meilisearch_python_async-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/LICENSE
--rw-r--r--   0        0        0     4641 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/README.md
--rw-r--r--   0        0        0       73 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2538 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0    22123 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     1886 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    86427 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      789 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    10993 2023-04-03 10:52:08.830309 meilisearch_python_async-1.1.0/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2138 2023-04-03 10:52:08.834309 meilisearch_python_async-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-07 22:06:54.234997 meilisearch_python_async-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4641 2023-04-07 22:06:54.234997 meilisearch_python_async-1.1.1/README.md
+-rw-r--r--   0        0        0       73 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2538 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0    22123 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     1886 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    86427 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    10993 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2138 2023-04-07 22:06:54.238996 meilisearch_python_async-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.1.1/PKG-INFO
```

### Comparing `meilisearch_python_async-1.1.0/LICENSE` & `meilisearch_python_async-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/README.md` & `meilisearch_python_async-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/client.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/index.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/models/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from camel_converter.pydantic_base import CamelBase
 from pydantic import Field
 
 
 class TaskId(CamelBase):
     uid: int
 
 
 class TaskStatus(TaskId):
-    index_uids: Optional[List[str]] = None
+    index_uid: Optional[str] = None
     status: str
     task_type: Union[str, Dict[str, Any]] = Field(..., alias="type")
     details: Optional[Dict[str, Any]]
     error: Optional[Dict[str, Any]]
     canceled_by: Optional[int]
     duration: Optional[str]
     enqueued_at: datetime
     started_at: Optional[datetime]
     finished_at: Optional[datetime]
 
 
 class TaskInfo(CamelBase):
     task_uid: int
-    index_uids: Optional[List[str]] = None
+    index_uid: Optional[str] = None
     status: str
     task_type: Union[str, Dict[str, Any]] = Field(..., alias="type")
     enqueued_at: datetime
```

### Comparing `meilisearch_python_async-1.1.0/meilisearch_python_async/task.py` & `meilisearch_python_async-1.1.1/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.1.0/pyproject.toml` & `meilisearch_python_async-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.1.0/PKG-INFO` & `meilisearch_python_async-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
```

