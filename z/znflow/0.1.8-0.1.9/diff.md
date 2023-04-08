# Comparing `tmp/znflow-0.1.8.tar.gz` & `tmp/znflow-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znflow-0.1.8.tar", max compression
+gzip compressed data, was "znflow-0.1.9.tar", max compression
```

## Comparing `znflow-0.1.8.tar` & `znflow-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-03-03 06:50:11.633851 znflow-0.1.8/LICENSE
--rw-r--r--   0        0        0     5183 2023-03-23 12:58:22.279243 znflow-0.1.8/README.md
--rw-r--r--   0        0        0     1066 2023-03-23 12:58:22.279243 znflow-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1023 2023-03-23 10:00:20.744512 znflow-0.1.8/znflow/__init__.py
--rw-r--r--   0        0        0     8337 2023-03-23 12:58:22.289243 znflow-0.1.8/znflow/base.py
--rw-r--r--   0        0        0     5555 2023-03-21 13:36:17.542419 znflow-0.1.8/znflow/graph.py
--rw-r--r--   0        0        0     1055 2023-03-22 17:00:36.335580 znflow-0.1.8/znflow/handler.py
--rw-r--r--   0        0        0     3262 2023-03-22 19:18:09.366497 znflow-0.1.8/znflow/node.py
--rw-r--r--   0        0        0     2760 2023-03-23 12:58:22.299243 znflow-0.1.8/znflow/utils.py
--rw-r--r--   0        0        0      666 2023-02-02 09:31:06.072217 znflow-0.1.8/znflow/visualize.py
--rw-r--r--   0        0        0     5858 1970-01-01 00:00:00.000000 znflow-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-03 06:50:11.633851 znflow-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5183 2023-03-24 11:13:18.708773 znflow-0.1.9/README.md
+-rw-r--r--   0        0        0     1066 2023-03-24 11:13:18.708773 znflow-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1025 2023-03-24 11:13:18.768772 znflow-0.1.9/znflow/__init__.py
+-rw-r--r--   0        0        0     8337 2023-03-24 11:13:18.778772 znflow-0.1.9/znflow/base.py
+-rw-r--r--   0        0        0     3470 2023-03-24 14:53:06.069920 znflow-0.1.9/znflow/combine.py
+-rw-r--r--   0        0        0     5973 2023-03-24 14:50:22.691716 znflow-0.1.9/znflow/graph.py
+-rw-r--r--   0        0        0     1055 2023-03-24 11:13:18.778772 znflow-0.1.9/znflow/handler.py
+-rw-r--r--   0        0        0     3504 2023-03-24 14:50:22.691716 znflow-0.1.9/znflow/node.py
+-rw-r--r--   0        0        0     1983 2023-03-24 11:13:18.788771 znflow-0.1.9/znflow/utils.py
+-rw-r--r--   0        0        0      666 2023-02-02 09:31:06.072217 znflow-0.1.9/znflow/visualize.py
+-rw-r--r--   0        0        0     5858 1970-01-01 00:00:00.000000 znflow-0.1.9/PKG-INFO
```

### Comparing `znflow-0.1.8/LICENSE` & `znflow-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `znflow-0.1.8/README.md` & `znflow-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `znflow-0.1.8/pyproject.toml` & `znflow-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "znflow"
-version = "0.1.8"
+version = "0.1.9"
 description = "A general purpose framework for building and running computational graphs."
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `znflow-0.1.8/znflow/__init__.py` & `znflow-0.1.9/znflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     CombinedConnections,
     Connection,
     FunctionFuture,
     Property,
     disable_graph,
     get_attribute,
 )
+from znflow.combine import combine
 from znflow.graph import DiGraph
 from znflow.node import Node, nodify
-from znflow.utils import combine
 from znflow.visualize import draw
 
 __version__ = importlib.metadata.version(__name__)
 
 __all__ = [
     "DiGraph",
     "Node",
```

### Comparing `znflow-0.1.8/znflow/base.py` & `znflow-0.1.9/znflow/base.py`

 * *Files identical despite different names*

### Comparing `znflow-0.1.8/znflow/graph.py` & `znflow-0.1.9/znflow/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,32 +100,44 @@
             super().add_node(node_for_adding.uuid, value=node_for_adding, **attr)
         else:
             raise ValueError("Only Nodes are supported.")
 
     def add_connections(self, u_of_edge, v_of_edge, **attr):
         log.debug(f"Add edge between {u_of_edge=} and {v_of_edge=}.")
         if isinstance(u_of_edge, Connection) and isinstance(v_of_edge, NodeBaseMixin):
-            assert u_of_edge.uuid in self, f"'{u_of_edge.uuid=}' not in '{self=}'"
-            assert v_of_edge.uuid in self, f"'{v_of_edge.uuid=}' not in '{self=}'"
+            if u_of_edge.uuid not in self:
+                raise ValueError(
+                    f"The source node (uuid={u_of_edge.uuid}, connection={u_of_edge}) is"
+                    " not in the graph."
+                )
+            if (
+                v_of_edge.uuid not in self
+            ):  # this might be impossible to reach. Let me know if you found a way.
+                raise ValueError(
+                    f"The target node (uuid={v_of_edge.uuid}, connection={v_of_edge}) is"
+                    " not in the graph."
+                )
+
             # TODO what if 'v_attr' is a list/dict/... that contains multiple connections?
             #  Is this relevant? We could do `v_attr.<dict_key>` or `v_attr.<list_index>`
             #  See test_node.test_ListConnection and test_node.test_DictionaryConnection
             self.add_edge(
                 u_of_edge.uuid,
                 v_of_edge.uuid,
                 u_attr=u_of_edge.attribute,
                 **attr,
             )
         else:
             raise ValueError("Only Connections and Nodes are supported.")
 
     def get_sorted_nodes(self):
         all_pipelines = []
-        for stage in self.reverse():
-            all_pipelines += nx.dfs_postorder_nodes(self.reverse(), stage)
+        reverse = self.reverse(copy=False)
+        for stage in reverse:
+            all_pipelines += nx.dfs_postorder_nodes(reverse, stage)
         return list(dict.fromkeys(all_pipelines))  # remove duplicates but keep order
 
     def run(self):
         for node_uuid in self.get_sorted_nodes():
             node = self.nodes[node_uuid]["value"]
             # update connectors
             self._update_node_attributes(node, handler.UpdateConnectors())
```

### Comparing `znflow-0.1.8/znflow/handler.py` & `znflow-0.1.9/znflow/handler.py`

 * *Files identical despite different names*

### Comparing `znflow-0.1.8/znflow/node.py` & `znflow-0.1.9/znflow/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,28 @@
 )
 
 
 def _mark_init_in_construction(cls):
     if "__init__" in dir(cls):
 
         def wrap_init(func):
+            if getattr(func, "_already_wrapped", False):
+                # if the function is already wrapped, return it
+                #  TODO this is solving the error but not the root cause
+                return func
+
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 cls._in_construction = True
                 value = func(*args, **kwargs)
                 cls._in_construction = False
                 return value
 
+            wrapper._already_wrapped = True
+
             return wrapper
 
         cls.__init__ = wrap_init(cls.__init__)
     return cls
 
 
 class Node(NodeBaseMixin):
@@ -54,24 +61,24 @@
         # Connect the Node to the Grap
         graph = get_graph()
         if graph is not empty:
             graph.add_node(instance)
         return instance
 
     def __getattribute__(self, item):
-        if item == "_graph_":
+        if item.startswith("_"):
             return super().__getattribute__(item)
         if self._graph_ not in [empty, None]:
             with disable_graph():
                 if item not in set(dir(self)):
                     raise AttributeError(
                         f"'{self.__class__.__name__}' object has no attribute '{item}'"
                     )
 
-            if item not in type(self)._protected_ and not item.startswith("_"):
+            if item not in type(self)._protected_:
                 if self._in_construction:
                     return super().__getattribute__(item)
                 return Connection(instance=self, attribute=item)
         return super().__getattribute__(item)
 
     def __setattr__(self, item, value) -> None:
         super().__setattr__(item, value)
```

### Comparing `znflow-0.1.8/znflow/utils.py` & `znflow-0.1.9/znflow/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -61,36 +61,7 @@
         """Handle a set."""
         return {self._handle(x, **kwargs) for x in value}
 
     @_handle.register
     def _(self, value: dict, **kwargs) -> dict:
         """Handle a dict."""
         return {key: self._handle(val, **kwargs) for key, val in value.items()}
-
-
-def combine(*args, attribute=None):
-    """Combine Node outputs which are lists into a single flat list.
-
-    Attributes
-    ----------
-    args : list of Node instances
-    attribute : str, default=None
-        If not None, the attribute of the Node instance is gathered.
-
-    Examples
-    --------
-    The following are all allowed:
-    >>> combine([a, b, c])
-    >>> combine(a, b, c)
-    >>> combine([a, b, c], attribute="outs")
-    >>> combine(a, b, c, attribute="outs")
-
-    Returns
-    -------
-    CombinedConnections:
-        A combined connections object.
-    """
-    if len(args) == 1 and isinstance(args[0], (list, tuple)):
-        args = args[0]
-    if attribute is None:
-        return sum(args, [])
-    return sum(map(lambda x: getattr(x, attribute), args), [])
```

### Comparing `znflow-0.1.8/znflow/visualize.py` & `znflow-0.1.9/znflow/visualize.py`

 * *Files identical despite different names*

### Comparing `znflow-0.1.8/PKG-INFO` & `znflow-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: znflow
-Version: 0.1.8
+Version: 0.1.9
 Summary: A general purpose framework for building and running computational graphs.
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

