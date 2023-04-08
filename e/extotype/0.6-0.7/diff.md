# Comparing `tmp/extotype-0.6.tar.gz` & `tmp/extotype-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extotype-0.6.tar", last modified: Sat Apr  8 21:35:18 2023, max compression
+gzip compressed data, was "extotype-0.7.tar", last modified: Sat Apr  8 21:40:12 2023, max compression
```

## Comparing `extotype-0.6.tar` & `extotype-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:35:18.446430 extotype-0.6/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:35:18.446430 extotype-0.6/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      435 2023-04-08 01:30:33.000000 extotype-0.6/README.md
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:35:18.446430 extotype-0.6/extotype/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1703 2023-04-08 21:20:17.000000 extotype-0.6/extotype/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:35:18.446430 extotype-0.6/extotype/static/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      777 2023-04-08 00:25:09.000000 extotype-0.6/extotype/static/extotype.js
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:35:18.446430 extotype-0.6/extotype/templates/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      214 2023-04-08 00:26:12.000000 extotype-0.6/extotype/templates/search.html
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:35:18.446430 extotype-0.6/extotype.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:35:18.000000 extotype-0.6/extotype.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      257 2023-04-08 21:35:18.000000 extotype-0.6/extotype.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-08 21:35:18.000000 extotype-0.6/extotype.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      992 2023-04-08 21:35:18.000000 extotype-0.6/extotype.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        9 2023-04-08 21:35:18.000000 extotype-0.6/extotype.egg-info/top_level.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-08 21:35:18.446430 extotype-0.6/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      440 2023-04-08 21:33:35.000000 extotype-0.6/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:40:12.346827 extotype-0.7/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:40:12.346827 extotype-0.7/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      435 2023-04-08 01:30:33.000000 extotype-0.7/README.md
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:40:12.346827 extotype-0.7/extotype/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1602 2023-04-08 21:39:24.000000 extotype-0.7/extotype/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:40:12.346827 extotype-0.7/extotype/static/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      777 2023-04-08 00:25:09.000000 extotype-0.7/extotype/static/extotype.js
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:40:12.346827 extotype-0.7/extotype/templates/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      214 2023-04-08 00:26:12.000000 extotype-0.7/extotype/templates/search.html
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-04-08 21:40:12.346827 extotype-0.7/extotype.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       50 2023-04-08 21:40:12.000000 extotype-0.7/extotype.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      257 2023-04-08 21:40:12.000000 extotype-0.7/extotype.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-04-08 21:40:12.000000 extotype-0.7/extotype.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      992 2023-04-08 21:40:12.000000 extotype-0.7/extotype.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        9 2023-04-08 21:40:12.000000 extotype-0.7/extotype.egg-info/top_level.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-04-08 21:40:12.346827 extotype-0.7/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      440 2023-04-08 21:39:50.000000 extotype-0.7/setup.py
```

### Comparing `extotype-0.6/extotype/__init__.py` & `extotype-0.7/extotype/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import path
 from sphinx.jinja2glue import SphinxFileSystemLoader
 from sphinx.application import Sphinx
 # from docutils import nodes
 # from hashlib import md5
-from llama_index import SimpleDirectoryReader, SimpleNodeParser, GPTSimpleVectorIndex
+from llama_index import GPTSimpleVectorIndex, SimpleDirectoryReader
 
 data = {}
 
 # def generate_embeddings(app, doctree, docname):
 #     data[docname] = {}
 #     for section in doctree.traverse(nodes.section):
 #         text = section.astext()
@@ -26,17 +26,15 @@
     app.builder.templates.loaders.insert(1, SphinxFileSystemLoader(template_dir))
     app.builder.templates.templatepathlen += 1
 
 def generate_index(app, exception):
     if app.builder.name != 'text':
         return
     documents = SimpleDirectoryReader(app.outdir).load_data()
-    parser = SimpleNodeParser()
-    nodes = parser.get_nodes_from_documents(documents)
-    index = GPTSimpleVectorIndex.from_documents(nodes)
+    index = GPTSimpleVectorIndex.from_documents(documents)
     index.save_to_disk(path.join(app.outdir, 'index.json'))
 
 def setup(app):
     app.connect('builder-inited', add_static_dir)
     # app.connect('doctree-resolved', generate_embeddings)
     app.connect('build-finished', generate_index)
     return {
```

### Comparing `extotype-0.6/extotype/static/extotype.js` & `extotype-0.7/extotype/static/extotype.js`

 * *Files identical despite different names*

### Comparing `extotype-0.6/extotype.egg-info/requires.txt` & `extotype-0.7/extotype.egg-info/requires.txt`

 * *Files identical despite different names*

