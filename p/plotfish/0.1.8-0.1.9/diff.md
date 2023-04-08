# Comparing `tmp/plotfish-0.1.8.tar.gz` & `tmp/plotfish-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotfish-0.1.8.tar", max compression
+gzip compressed data, was "plotfish-0.1.9.tar", max compression
```

## Comparing `plotfish-0.1.8.tar` & `plotfish-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3685 2023-04-07 23:12:07.526328 plotfish-0.1.8/plotfish/__init__.py
--rw-r--r--   0        0        0      439 2023-04-07 23:12:21.794545 plotfish-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      665 2023-04-07 23:12:35.366793 plotfish-0.1.8/setup.py
--rw-r--r--   0        0        0      424 2023-04-07 23:12:35.367029 plotfish-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3684 2023-04-07 23:35:23.946517 plotfish-0.1.9/plotfish/__init__.py
+-rw-r--r--   0        0        0      439 2023-04-07 23:35:29.986628 plotfish-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      665 2023-04-07 23:35:57.449425 plotfish-0.1.9/setup.py
+-rw-r--r--   0        0        0      424 2023-04-07 23:35:57.449624 plotfish-0.1.9/PKG-INFO
```

### Comparing `plotfish-0.1.8/plotfish/__init__.py` & `plotfish-0.1.9/plotfish/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,14 @@
             timestamp = timestamp.replace(tzinfo=timezone.utc).timestamp()
         elif isinstance(timestamp, int):
             timestamp = float(timestamp)
         elif timestamp is None:
             timestamp = time.time()
 
         socket.emit("recordDatapoints", (name, [[timestamp, value, None]]))
-
-        # TODO [critical]: Remove this after moving to REST
-        socket.disconnect()
     except Exception as err:
         logger.error(
             "Ran into error while recording datapoint for plot `%s`: %s", name, err
         )
 
 
 def line(
@@ -136,7 +133,12 @@
 
 
 def increment(
     name: str,
     timestamp: Optional[TimestampLike] = None,
 ) -> None:
     _record_datapoint(name, 1, timestamp, metadata={"type": PlotType.Counter})
+
+
+# I feel like this shouldn't be necessary
+def quit() -> None:
+    socket.disconnect()
```

### Comparing `plotfish-0.1.8/setup.py` & `plotfish-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['python-socketio>=5.7.2,<6.0.0',
  'requests>=2.28.2,<3.0.0',
  'websocket-client>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'plotfish',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python SDK for Plotfish.',
     'long_description': None,
     'author': 'The Fisherman',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

