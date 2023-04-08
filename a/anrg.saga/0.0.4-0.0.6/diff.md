# Comparing `tmp/anrg.saga-0.0.4.tar.gz` & `tmp/anrg.saga-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anrg.saga-0.0.4.tar", last modified: Fri Apr  7 17:17:09 2023, max compression
+gzip compressed data, was "anrg.saga-0.0.6.tar", last modified: Fri Apr  7 21:56:08 2023, max compression
```

## Comparing `anrg.saga-0.0.4.tar` & `anrg.saga-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/
--rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)     1179 2023-04-06 16:54:49.000000 anrg.saga-0.0.4/README.md
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/anrg.saga.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 17:17:09.000000 anrg.saga-0.0.4/anrg.saga.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      636 2023-04-07 17:17:09.000000 anrg.saga-0.0.4/anrg.saga.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-04-07 17:17:09.000000 anrg.saga-0.0.4/anrg.saga.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       57 2023-04-07 17:17:09.000000 anrg.saga-0.0.4/anrg.saga.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        5 2023-04-07 17:17:09.000000 anrg.saga-0.0.4/anrg.saga.egg-info/top_level.txt
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/saga/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:50:26.000000 anrg.saga-0.0.4/saga/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      495 2023-04-05 15:01:34.000000 anrg.saga-0.0.4/saga/base.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/saga/common/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 15:03:21.000000 anrg.saga-0.0.4/saga/common/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2772 2023-04-06 21:26:40.000000 anrg.saga-0.0.4/saga/common/brute_force.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6569 2023-04-05 17:54:25.000000 anrg.saga-0.0.4/saga/common/cpop.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1365 2023-04-05 17:45:20.000000 anrg.saga-0.0.4/saga/common/fastest_node.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6883 2023-04-07 04:02:43.000000 anrg.saga-0.0.4/saga/common/heft.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1544 2023-04-05 14:51:04.000000 anrg.saga-0.0.4/saga/hybrid.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/saga/stochastic/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:55:47.000000 anrg.saga-0.0.4/saga/stochastic/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      848 2023-04-06 16:43:14.000000 anrg.saga-0.0.4/saga/stochastic/improved_sheft.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2579 2023-04-06 16:43:14.000000 anrg.saga-0.0.4/saga/stochastic/mean_heft.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2628 2023-04-05 18:13:26.000000 anrg.saga-0.0.4/saga/stochastic/sheft.py
--rw-r--r--   0 jared     (1000) jared     (1000)     8492 2023-04-07 04:38:10.000000 anrg.saga-0.0.4/saga/stochastic/stoch_heft.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/saga/utils/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:56:02.000000 anrg.saga-0.0.4/saga/utils/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6100 2023-04-07 17:01:19.000000 anrg.saga-0.0.4/saga/utils/draw.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3112 2023-04-07 03:49:33.000000 anrg.saga-0.0.4/saga/utils/random_graphs.py
--rw-r--r--   0 jared     (1000) jared     (1000)     8999 2023-04-07 17:16:53.000000 anrg.saga-0.0.4/saga/utils/random_variable.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4570 2023-04-06 16:43:14.000000 anrg.saga-0.0.4/saga/utils/simulator.py
--rw-r--r--   0 jared     (1000) jared     (1000)     7370 2023-04-05 17:51:50.000000 anrg.saga-0.0.4/saga/utils/tools.py
--rw-r--r--   0 jared     (1000) jared     (1000)       38 2023-04-07 17:17:09.759468 anrg.saga-0.0.4/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)     1078 2023-04-07 17:17:06.000000 anrg.saga-0.0.4/setup.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/
+-rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)     1179 2023-04-06 16:54:49.000000 anrg.saga-0.0.6/README.md
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/anrg.saga.egg-info/
+-rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 21:56:08.000000 anrg.saga-0.0.6/anrg.saga.egg-info/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)      636 2023-04-07 21:56:08.000000 anrg.saga-0.0.6/anrg.saga.egg-info/SOURCES.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-04-07 21:56:08.000000 anrg.saga-0.0.6/anrg.saga.egg-info/dependency_links.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       57 2023-04-07 21:56:08.000000 anrg.saga-0.0.6/anrg.saga.egg-info/requires.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        5 2023-04-07 21:56:08.000000 anrg.saga-0.0.6/anrg.saga.egg-info/top_level.txt
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/saga/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:50:26.000000 anrg.saga-0.0.6/saga/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      495 2023-04-05 15:01:34.000000 anrg.saga-0.0.6/saga/base.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/saga/common/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 15:03:21.000000 anrg.saga-0.0.6/saga/common/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2772 2023-04-06 21:26:40.000000 anrg.saga-0.0.6/saga/common/brute_force.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     6569 2023-04-05 17:54:25.000000 anrg.saga-0.0.6/saga/common/cpop.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     1365 2023-04-05 17:45:20.000000 anrg.saga-0.0.6/saga/common/fastest_node.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     6883 2023-04-07 04:02:43.000000 anrg.saga-0.0.6/saga/common/heft.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     1544 2023-04-05 14:51:04.000000 anrg.saga-0.0.6/saga/hybrid.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/saga/stochastic/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:55:47.000000 anrg.saga-0.0.6/saga/stochastic/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      848 2023-04-06 16:43:14.000000 anrg.saga-0.0.6/saga/stochastic/improved_sheft.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2579 2023-04-06 16:43:14.000000 anrg.saga-0.0.6/saga/stochastic/mean_heft.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2628 2023-04-05 18:13:26.000000 anrg.saga-0.0.6/saga/stochastic/sheft.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     8492 2023-04-07 04:38:10.000000 anrg.saga-0.0.6/saga/stochastic/stoch_heft.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/saga/utils/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:56:02.000000 anrg.saga-0.0.6/saga/utils/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     6196 2023-04-07 21:52:07.000000 anrg.saga-0.0.6/saga/utils/draw.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     3112 2023-04-07 03:49:33.000000 anrg.saga-0.0.6/saga/utils/random_graphs.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     8999 2023-04-07 17:16:53.000000 anrg.saga-0.0.6/saga/utils/random_variable.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     4570 2023-04-06 16:43:14.000000 anrg.saga-0.0.6/saga/utils/simulator.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     7370 2023-04-05 17:51:50.000000 anrg.saga-0.0.6/saga/utils/tools.py
+-rw-r--r--   0 jared     (1000) jared     (1000)       38 2023-04-07 21:56:08.689936 anrg.saga-0.0.6/setup.cfg
+-rw-r--r--   0 jared     (1000) jared     (1000)     1078 2023-04-07 21:54:41.000000 anrg.saga-0.0.6/setup.py
```

### Comparing `anrg.saga-0.0.4/PKG-INFO` & `anrg.saga-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anrg.saga
-Version: 0.0.4
+Version: 0.0.6
 Summary: Collection of schedulers for distributed computing
 Home-page: https://github.com/ANRGUSC/saga
 Author: Jared Coleman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anrg.saga-0.0.4/README.md` & `anrg.saga-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/anrg.saga.egg-info/PKG-INFO` & `anrg.saga-0.0.6/anrg.saga.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anrg.saga
-Version: 0.0.4
+Version: 0.0.6
 Summary: Collection of schedulers for distributed computing
 Home-page: https://github.com/ANRGUSC/saga
 Author: Jared Coleman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anrg.saga-0.0.4/anrg.saga.egg-info/SOURCES.txt` & `anrg.saga-0.0.6/anrg.saga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/common/brute_force.py` & `anrg.saga-0.0.6/saga/common/brute_force.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/common/cpop.py` & `anrg.saga-0.0.6/saga/common/cpop.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/common/fastest_node.py` & `anrg.saga-0.0.6/saga/common/fastest_node.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/common/heft.py` & `anrg.saga-0.0.6/saga/common/heft.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/hybrid.py` & `anrg.saga-0.0.6/saga/hybrid.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/stochastic/improved_sheft.py` & `anrg.saga-0.0.6/saga/stochastic/improved_sheft.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/stochastic/mean_heft.py` & `anrg.saga-0.0.6/saga/stochastic/mean_heft.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/stochastic/sheft.py` & `anrg.saga-0.0.6/saga/stochastic/sheft.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/stochastic/stoch_heft.py` & `anrg.saga-0.0.6/saga/stochastic/stoch_heft.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/utils/draw.py` & `anrg.saga-0.0.6/saga/utils/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,14 @@
             formatted_graph.nodes[node]["weight"] = formatted_graph.nodes[node]["weight"].mean()
     for edge in formatted_graph.edges:
         formatted_graph.edges[edge]["label"] = formatted_graph.edges[edge]["weight"]
         if isinstance(formatted_graph.edges[edge]["weight"], RandomVariable):
             formatted_graph.edges[edge]["weight"] = formatted_graph.edges[edge]["weight"].mean()
     return formatted_graph
 
-from common import standardize_instance
-
 def draw_task_graph(task_graph: nx.DiGraph, 
                     ax: Optional[plt.Axes] = None,
                     schedule: Optional[Dict[Hashable, List[Task]]] = None) -> plt.Axes:
     """Draws a task graph
 
     Args:
         task_graph: Task graph
@@ -49,18 +47,20 @@
         
     task_graph = format_graph(task_graph.copy())
     pos = nx.nx_agraph.graphviz_layout(task_graph, prog="dot")
 
     colors = {}
     if schedule is not None:
         tasks = {task.name: task for node, tasks in schedule.items() for task in tasks}
-        network_nodes = {task.node for node, tasks in schedule.items() for task in tasks}
-        network_node_idx = {node: i for i, node in enumerate(sorted(network_nodes))}
+        network_nodes = set(schedule.keys())
+
         cmap = plt.get_cmap("tab20", len(network_nodes))
-        colors = {node: cmap(idx) for node, idx in network_node_idx.items()}
+        sorted_nodes = sorted(network_nodes)
+        sorted_colors = [cmap(i) for i in range(len(network_nodes))]
+        colors = {node: color for node, color in zip(sorted_nodes, sorted_colors)}
 
     nx.draw_networkx_nodes(
         task_graph, pos=pos, ax=ax,
         node_size=100,
         node_color="white",
         edgecolors="black",
         linewidths=2,
@@ -97,15 +97,14 @@
             (u, v): f"{task_graph.edges[(u, v)]['label']:.2f}"
             for u, v in task_graph.edges
         }
     )
 
     return ax
 
-
 def draw_network(network: nx.Graph, ax: Optional[plt.Axes] = None) -> plt.Axes:
     """Draws a network
 
     Args:
         network: Network
         ax: Axes to draw on
     """
@@ -114,22 +113,25 @@
 
     # don't drdaw self loops
     network = format_graph(network.copy())
     network.remove_edges_from(nx.selfloop_edges(network))
 
     # use same colors as task graph
     cmap = plt.get_cmap("tab20", len(network.nodes))
-    node_idx = {node: i for i, node in enumerate(sorted(network.nodes))}
-    colors = [cmap(idx) for node, idx in node_idx.items()]
+    sorted_nodes = sorted(network.nodes)
+    sorted_colors = [cmap(i) for i in range(len(network.nodes))]
+    node_colors = {node: color for node, color in zip(sorted_nodes, sorted_colors)}
+    colors = [node_colors[node] for node in sorted_nodes]
     
     # spring layout
     pos = nx.spring_layout(network)
     # draw network nodes with black border and white fill
     nx.draw_networkx_nodes(
         network, pos=pos, ax=ax,
+        nodelist=sorted_nodes,
         node_color=colors,
         edgecolors="black",
         node_size=3000
     )
 
     # draw network edges
     nx.draw_networkx_edges(
```

### Comparing `anrg.saga-0.0.4/saga/utils/random_graphs.py` & `anrg.saga-0.0.6/saga/utils/random_graphs.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/utils/random_variable.py` & `anrg.saga-0.0.6/saga/utils/random_variable.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/utils/simulator.py` & `anrg.saga-0.0.6/saga/utils/simulator.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/saga/utils/tools.py` & `anrg.saga-0.0.6/saga/utils/tools.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.4/setup.py` & `anrg.saga-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 thisdir = pathlib.Path(__file__).parent.absolute()
 
 long_description = (thisdir / "README.md").read_text()
 
 setup(
     name='anrg.saga',
-    version='0.0.4',
+    version='0.0.6',
     description='Collection of schedulers for distributed computing',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ANRGUSC/saga',
     author='Jared Coleman',
     packages=find_packages(),
     classifiers=[
```

