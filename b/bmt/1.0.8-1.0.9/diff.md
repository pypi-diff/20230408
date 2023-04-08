# Comparing `tmp/bmt-1.0.8.tar.gz` & `tmp/bmt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmt-1.0.8.tar", max compression
+gzip compressed data, was "bmt-1.0.9.tar", max compression
```

## Comparing `bmt-1.0.8.tar` & `bmt-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1544 2023-03-30 15:50:46.718203 bmt-1.0.8/LICENSE
--rw-r--r--   0        0        0     1110 2023-03-30 15:50:46.718203 bmt-1.0.8/README.md
--rw-r--r--   0        0        0       31 2023-03-30 15:50:46.718203 bmt-1.0.8/bmt/__init__.py
--rw-r--r--   0        0        0    56700 2023-03-30 15:50:46.718203 bmt-1.0.8/bmt/toolkit.py
--rw-r--r--   0        0        0     3843 2023-03-30 15:50:46.718203 bmt-1.0.8/bmt/utils.py
--rw-r--r--   0        0        0     1617 2023-03-30 15:51:04.706566 bmt-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 bmt-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-04-03 23:19:11.932956 bmt-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1110 2023-04-03 23:19:11.932956 bmt-1.0.9/README.md
+-rw-r--r--   0        0        0       31 2023-04-03 23:19:11.932956 bmt-1.0.9/bmt/__init__.py
+-rw-r--r--   0        0        0    57299 2023-04-03 23:19:11.936956 bmt-1.0.9/bmt/toolkit.py
+-rw-r--r--   0        0        0     3843 2023-04-03 23:19:11.936956 bmt-1.0.9/bmt/utils.py
+-rw-r--r--   0        0        0     1617 2023-04-03 23:19:32.585241 bmt-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 bmt-1.0.9/PKG-INFO
```

### Comparing `bmt-1.0.8/LICENSE` & `bmt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bmt-1.0.8/README.md` & `bmt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bmt-1.0.8/bmt/toolkit.py` & `bmt-1.0.9/bmt/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 )
 from pprint import pprint
 from bmt.utils import format_element, parse_name
 
 Url = str
 Path = str
 
-REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.2.5/biolink-model.yaml"
-PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.5/predicate_mapping.yaml'
-INFORES_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.5/infores_catalog_nodes.tsv'
+REMOTE_PATH = "https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/biolink-model.yaml"
+PREDICATE_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/predicate_mapping.yaml'
+INFORES_MAP = 'https://raw.githubusercontent.com/biolink/biolink-model/v3.2.6/infores_catalog_nodes.tsv'
 
 
 NODE_PROPERTY = "node property"
 ASSOCIATION_SLOT = "association slot"
 RELATED_TO = "related to"
 
 CACHE_SIZE = 1024
@@ -1094,14 +1094,34 @@
         -------
         bool
             That the named element is a valid relation/predicate in Biolink Model
         """
         return RELATED_TO in self.get_ancestors(name, mixin)
 
     @lru_cache(CACHE_SIZE)
+    def get_denormalized_association_slots(self, formatted) -> List[Element]:
+        """
+        Gets all association slots that are denormalized
+
+        Returns
+        -------
+        List[linkml_model.meta.Element]
+            A list of association slots
+
+        """
+        slots = []
+        for k, v in self.view.schema.slots.items():
+            if v.annotations and "denormalized" in v.annotations:
+                if formatted:
+                    slots.append(format_element(v))
+                else:
+                    slots.append(k)
+        return slots
+
+    @lru_cache(CACHE_SIZE)
     def is_translator_canonical_predicate(self, name: str, mixin: bool = True) -> bool:
         """
         Determines whether the given name is the name of a canonical relation/predicate
         in the Biolink Model. An element is a canonical predicate if it descends from
         `RELATED_TO` and is tagged with the annotation 'biolink:canonical_predicate'
 
         Parameters
```

### Comparing `bmt-1.0.8/bmt/utils.py` & `bmt-1.0.9/bmt/utils.py`

 * *Files identical despite different names*

### Comparing `bmt-1.0.8/pyproject.toml` & `bmt-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmt"
-version = "1.0.8"
+version = "1.0.9"
 description = "Biolink Model Toolkit: A Python API for working with the Biolink Model"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "BSD"
 
 readme = "README.md"
 repository = "https://github.com/biolink/biolink-model-toolkit"
 documentation = "https://biolink.github.io/biolink-model-toolkit/"
```

### Comparing `bmt-1.0.8/PKG-INFO` & `bmt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Biolink Model Toolkit: A Python API for working with the Biolink Model
 Home-page: https://github.com/biolink/biolink-model-toolkit
 License: BSD
 Keywords: schema,linked data,data modeling,biolink,api
 Author: Sierra Taylor Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<4.0
```

