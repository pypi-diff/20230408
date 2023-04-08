# Comparing `tmp/netunicorn-connector-salt-0.3.1.tar.gz` & `tmp/netunicorn-connector-salt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.1.tar", last modified: Fri Apr  7 21:47:54 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.2.tar", last modified: Fri Apr  7 21:58:19 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.1.tar` & `netunicorn-connector-salt-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.1/LICENSE` & `netunicorn-connector-salt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.1/PKG-INFO` & `netunicorn-connector-salt-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.1
+Version: 0.3.2
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.1/README.md` & `netunicorn-connector-salt-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.1/pyproject.toml` & `netunicorn-connector-salt-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,33 +198,33 @@
             self.logger.debug(
                 f"Deployment of executor {deployment.executor_id} to node {deployment.node} successful, no commands to execute"
             )
             return {deployment.executor_id: Success(None)}
 
         try:
             # consequent, not in parallel
-            results = [
-                await (
-                    await self.session.post(
-                        self.runpoint,
-                        json={
-                            "client": "local",
-                            "tgt": deployment.node.name,
-                            "fun": "cmd.run",
-                            "arg": [command],
-                            "username": self.username,
-                            "password": self.password,
-                            "eauth": self.eauth,
-                            "full_return": True,
-                        },
-                    ).json()
-                )
-                .get("return", [{}])[0]
-                for command in deployment.environment_definition.commands
-            ]
+            results = []
+            for command in deployment.environment_definition.commands:
+                async with self.session.post(
+                    self.runpoint,
+                    json={
+                        "client": "local",
+                        "tgt": deployment.node.name,
+                        "fun": "cmd.run",
+                        "arg": [command],
+                        "username": self.username,
+                        "password": self.password,
+                        "eauth": self.eauth,
+                        "full_return": True,
+                    },
+                ) as response:
+                    salt_return = await response.json()
+                    self.logger.debug(salt_return)
+                    salt_return = salt_return.get("return", [{}])[0]
+                    results.append(salt_return)
         except Exception as e:
             self.logger.error(
                 f"Exception during deployment of executor {deployment.executor_id}, node {deployment.node}: {e}"
             )
             results = [e]
         self.logger.debug(
             f"Deployment of executor {deployment.executor_id} to node {deployment.node}, result: {results}"
```

### Comparing `netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.1
+Version: 0.3.2
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

