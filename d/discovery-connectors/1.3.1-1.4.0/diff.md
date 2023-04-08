# Comparing `tmp/discovery-connectors-1.3.1.tar.gz` & `tmp/discovery-connectors-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-connectors-1.3.1.tar", last modified: Wed Mar 29 15:46:17 2023, max compression
+gzip compressed data, was "discovery-connectors-1.4.0.tar", last modified: Sat Apr  8 20:34:34 2023, max compression
```

## Comparing `discovery-connectors-1.3.1.tar` & `discovery-connectors-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.916379 discovery-connectors-1.3.1/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-03-29 15:46:17.916643 discovery-connectors-1.3.1/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.903206 discovery-connectors-1.3.1/discovery_connectors.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-03-29 15:46:17.000000 discovery-connectors-1.3.1/discovery_connectors.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)      868 2023-03-29 15:46:17.000000 discovery-connectors-1.3.1/discovery_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-03-29 15:46:17.000000 discovery-connectors-1.3.1/discovery_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      195 2023-03-29 15:46:17.000000 discovery-connectors-1.3.1/discovery_connectors.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-03-29 15:46:17.000000 discovery-connectors-1.3.1/discovery_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.903934 discovery-connectors-1.3.1/ds_connectors/
--rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-03-29 15:46:07.000000 discovery-connectors-1.3.1/ds_connectors/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.911006 discovery-connectors-1.3.1/ds_connectors/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.3.1/ds_connectors/handlers/cortex_helpers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/hive_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.3.1/ds_connectors/handlers/mc_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5389 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/mongo_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-03-29 15:44:49.000000 discovery-connectors-1.3.1/ds_connectors/handlers/mysql_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/postgres_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/redis_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15587 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/handlers/s3_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.912194 discovery-connectors-1.3.1/ds_connectors/parsers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/parsers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/ds_connectors/parsers/dsv.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-03-29 15:46:17.917569 discovery-connectors-1.3.1/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2352 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.898444 discovery-connectors-1.3.1/tests/
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.913324 discovery-connectors-1.3.1/tests/aws/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/tests/aws/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/tests/aws/s3_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.914636 discovery-connectors-1.3.1/tests/managed_content/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.3.1/tests/managed_content/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.3.1/tests/managed_content/mc_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-29 15:46:17.915673 discovery-connectors-1.3.1/tests/po1/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.3.1/tests/po1/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.714393 discovery-connectors-1.4.0/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-04-08 20:34:34.714627 discovery-connectors-1.4.0/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.702176 discovery-connectors-1.4.0/discovery_connectors.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)      987 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      195 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.702492 discovery-connectors-1.4.0/ds_connectors/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-08 20:34:13.000000 discovery-connectors-1.4.0/ds_connectors/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.707592 discovery-connectors-1.4.0/ds_connectors/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.0/ds_connectors/handlers/cortex_helpers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/hive_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mc_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5389 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mongo_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mysql_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/postgres_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/redis_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15587 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/s3_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.708329 discovery-connectors-1.4.0/ds_connectors/parsers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/parsers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/parsers/dsv.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-08 20:34:34.715484 discovery-connectors-1.4.0/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2352 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.699294 discovery-connectors-1.4.0/tests/
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.709034 discovery-connectors-1.4.0/tests/aws/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/aws/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/aws/s3_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.709581 discovery-connectors-1.4.0/tests/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.710410 discovery-connectors-1.4.0/tests/managed_content/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.0/tests/managed_content/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.0/tests/managed_content/mc_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.712784 discovery-connectors-1.4.0/tests/mysql/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/mysql/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1221 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/mysql/mongo_handler_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8812 2023-04-08 20:11:13.000000 discovery-connectors-1.4.0/tests/mysql/mysql_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.713753 discovery-connectors-1.4.0/tests/po1/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.3.1/LICENSE.txt` & `discovery-connectors-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/PKG-INFO` & `discovery-connectors-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.3.1
+Version: 1.4.0
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.3.1/discovery_connectors.egg-info/PKG-INFO` & `discovery-connectors-1.4.0/discovery_connectors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.3.1
+Version: 1.4.0
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.3.1/discovery_connectors.egg-info/SOURCES.txt` & `discovery-connectors-1.4.0/discovery_connectors.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,14 @@
 ds_connectors/handlers/postgres_handlers.py
 ds_connectors/handlers/redis_handlers.py
 ds_connectors/handlers/s3_handlers.py
 ds_connectors/parsers/__init__.py
 ds_connectors/parsers/dsv.py
 tests/aws/__init__.py
 tests/aws/s3_handler_test.py
+tests/handlers/__init__.py
 tests/managed_content/__init__.py
 tests/managed_content/mc_handler_test.py
+tests/mysql/__init__.py
+tests/mysql/mongo_handler_test.py
+tests/mysql/mysql_handler_test.py
 tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/cortex_helpers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/cortex_helpers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/hive_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/hive_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/mc_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/mc_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/mongo_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/mongo_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/mysql_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/postgres_handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from aistac.handlers.abstract_handlers import AbstractSourceHandler, ConnectorContract, HandlerFactory
-import pandas as pd
 
 __author__ = 'Johan Gielstra'
 
 
-class MySQLSourceHandler(AbstractSourceHandler):
-    """ A MySQL Source Handler"""
+class PostgresSourceHandler(AbstractSourceHandler):
+    """ A Postgres Source Handler"""
 
     def __init__(self, connector_contract: ConnectorContract):
-        """ initialise the Handler passing the source_contract dictionary """
+        """ initialise the Hander passing the source_contract dictionary """
         # required module import
-        self.pymysql = HandlerFactory.get_module('pymysql')
+        self.psycopg2 = HandlerFactory.get_module('psycopg2')
         super().__init__(connector_contract)
-        self._host, self._port, self._database, self._user, self._password, self._query = self.__get_connector_details()
         self._file_state = 0
         self._changed_flag = True
 
     def supported_types(self) -> list:
         """ The source types supported with this module"""
-        return ['jdbc', 'mysql']
+        return ['postgresql', 'postgres']
 
     def exists(self) -> bool:
         return True
 
     def has_changed(self) -> bool:
         """ returns if the file has been modified"""
         # TODO: Add in change logic here
@@ -41,57 +39,44 @@
         """ returns the canonical dataset based on the source contract
             The canonical in this instance is a dictionary that has the headers as the key and then
             the ordered list of values for that header
         """
         conn = None
         if not isinstance(self.connector_contract, ConnectorContract):
             raise ValueError("The Connector Contract is not valid")
-
+        database = self.connector_contract.path[1:]
+        host = self.connector_contract.hostname
+        connector_type = self.connector_contract.schema
+        # jdbc url ?? nicer than individual parameters
+        query = self.connector_contract.kwargs.get('query')
+        user = self.connector_contract.username
+        password = self.connector_contract.password
+        port = self.connector_contract.port or '5432'
+        if connector_type.lower() not in self.supported_types():
+            raise ValueError("The source type '{}' is not supported. see supported_types()".format(connector_type))
         try:
-            conn = self.pymysql.connect(host=self._host,
-                                         user=self._user,
-                                         password=self._password,
-                                         database=self._database,
-                                         port=int(self._port))
-            if "query" in kwargs:
-                self._query = kwargs.get("query")
-
-            with conn.cursor() as cursor:
-                cursor.execute(self._query)
-                result = cursor.fetchall()
-                df = pd.DataFrame(result)
-                return df
-        except (Exception, self.pymysql.Error) as error:
+            conn = self.psycopg2.connect(database=database, host=host, port=port, user=user, password=password)
+            cur = conn.cursor()
+            cur.execute(query)
+            colnames = [desc[0] for desc in cur.description]
+            rtn_dict = {}
+            row = cur.fetchone()  # look into fetchMany versus 1-1
+            """
+            {
+                "col1" = [1,2,3],
+                "col2" = ["a","b","c"]
+            }
+            """
+            while row is not None:
+                for idx, col in enumerate(colnames):
+                    if col not in rtn_dict:
+                        rtn_dict[col] = []
+                    rtn_dict.get(col).append(row[idx])
+                row = cur.fetchone()
+            cur.close()
+            return rtn_dict
+        except (Exception, self.psycopg2.DatabaseError) as error:
             print(error)
         finally:
             if conn is not None:
                 conn.close()
                 print('Database connection closed.')
-
-    def __get_connector_details(self):
-        """
-        gets connector details like host, port, username, password, etc from uri
-        sample uri: "jdbc:mysql://root:password@localhost:3306/database"
-        """
-        connector_type = self.connector_contract.schema
-        path = self.connector_contract.path
-
-        url_splits = path.split("//")
-        credentials_str = url_splits[1].split("@")[0]
-        rest_of_uri_str = url_splits[1].split("@")[1]
-
-        # gets credentials from uri
-        username = credentials_str.split(":")[0]
-        password = credentials_str.split(":")[1]
-
-        # gets host details
-        host = rest_of_uri_str.split(":")[0]
-        port = rest_of_uri_str.split(":")[1].split("/")[0]
-        database = rest_of_uri_str.split(":")[1].split("/")[1].split("?")[0]
-
-        params = ""
-        if "?" in rest_of_uri_str:
-            params = rest_of_uri_str.split(":")[1].split("/")[1].split("?")[1]
-        query = self.connector_contract.kwargs.get('query')
-        if connector_type.lower() not in self.supported_types():
-            raise ValueError("The source type '{}' is not supported. see supported_types()".format(connector_type))
-        return host, port, database, username, password, query
```

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/redis_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/redis_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/handlers/s3_handlers.py` & `discovery-connectors-1.4.0/ds_connectors/handlers/s3_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/ds_connectors/parsers/dsv.py` & `discovery-connectors-1.4.0/ds_connectors/parsers/dsv.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/setup.py` & `discovery-connectors-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/tests/aws/s3_handler_test.py` & `discovery-connectors-1.4.0/tests/aws/s3_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.3.1/tests/managed_content/mc_handler_test.py` & `discovery-connectors-1.4.0/tests/managed_content/mc_handler_test.py`

 * *Files identical despite different names*

