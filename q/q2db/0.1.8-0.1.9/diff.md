# Comparing `tmp/q2db-0.1.8.tar.gz` & `tmp/q2db-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2db-0.1.8.tar", max compression
+gzip compressed data, was "q2db-0.1.9.tar", max compression
```

## Comparing `q2db-0.1.8.tar` & `q2db-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3399 2022-06-23 21:06:07.570486 q2db-0.1.8/README.md
--rw-r--r--   0        0        0      521 2022-07-19 16:08:12.261716 q2db-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       37 2022-07-01 09:35:16.794537 q2db-0.1.8/q2db/__init__.py
--rw-r--r--   0        0        0    16008 2022-07-19 16:07:39.474597 q2db-0.1.8/q2db/cursor.py
--rw-r--r--   0        0        0    29886 2022-07-19 15:49:28.816604 q2db-0.1.8/q2db/db.py
--rw-r--r--   0        0        0     7486 2022-07-14 15:03:04.627959 q2db-0.1.8/q2db/schema.py
--rw-r--r--   0        0        0      948 2021-10-28 15:19:40.483890 q2db-0.1.8/q2db/utils.py
--rw-r--r--   0        0        0       22 2022-07-19 16:08:13.065690 q2db-0.1.8/q2db/version.py
--rw-r--r--   0        0        0     4203 2022-07-19 16:08:13.863000 q2db-0.1.8/setup.py
--rw-r--r--   0        0        0     4005 2022-07-19 16:08:13.863566 q2db-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3399 2022-06-23 21:06:07.570486 q2db-0.1.9/README.md
+-rw-r--r--   0        0        0      521 2022-07-19 16:22:35.010294 q2db-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-07-01 09:35:16.794537 q2db-0.1.9/q2db/__init__.py
+-rw-r--r--   0        0        0    15772 2022-07-19 16:22:13.054978 q2db-0.1.9/q2db/cursor.py
+-rw-r--r--   0        0        0    29882 2022-07-19 16:22:25.814483 q2db-0.1.9/q2db/db.py
+-rw-r--r--   0        0        0     7486 2022-07-14 15:03:04.627959 q2db-0.1.9/q2db/schema.py
+-rw-r--r--   0        0        0      948 2021-10-28 15:19:40.483890 q2db-0.1.9/q2db/utils.py
+-rw-r--r--   0        0        0       22 2022-07-19 16:22:35.745932 q2db-0.1.9/q2db/version.py
+-rw-r--r--   0        0        0     4203 2022-07-19 16:22:36.781141 q2db-0.1.9/setup.py
+-rw-r--r--   0        0        0     4005 2022-07-19 16:22:36.781632 q2db-0.1.9/PKG-INFO
```

### Comparing `q2db-0.1.8/README.md` & `q2db-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `q2db-0.1.8/pyproject.toml` & `q2db-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2db"
-version = "0.1.8"
+version = "0.1.9"
 description = "python DB API wrapper (MySQL, PostgreSQL, SQLite)"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.black]
 line-length = 110
```

### Comparing `q2db-0.1.8/q2db/cursor.py` & `q2db-0.1.9/q2db/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,37 +280,35 @@
     def import_json(self, file, tick_callback=None):
         """read json from file or file-like object
         ;param file: str or file-like object
         """
         if self.table_name:
             read_from = self._prepare_import(file)
             rows = json.load(read_from)
-            for x in rows:
-                self.insert(x, refresh=False)
-                tick_callback() if tick_callback else None
-                if self.last_sql_error():
-                    raise Exception("Import error")
-            self.refresh()
+            self.import_rows(rows, tick_callback)
 
     def import_csv(self, file, tick_callback=None):
         """read csv from file or file-like object
         ;param file: str or file-like object
         """
         if self.table_name:
             read_from = self._prepare_import(file)
             rows = csv.DictReader(read_from, dialect="excel")
-            # self.q2_db.connection.execute("begin transaction")
-            for x in rows:
-                self.insert(x, refresh=False)
-                # self.q2_db._cursor(f"delete from {self.table_name}")
-                tick_callback() if tick_callback else None
-                if self.last_sql_error():
-                    raise Exception(f"Import error: {self.last_sql_error()}, {self.last_sql()}")
-            self.refresh()
-            # self.q2_db.connection.execute("commit")
+            self.import_rows(rows, tick_callback)
+
+    def import_rows(self, rows, tick_callback=None):
+        self.transaction()
+        for x in rows:
+            self.insert(x, refresh=False)
+            tick_callback() if tick_callback else None
+            if self.last_sql_error():
+                self.rollback()
+                raise Exception(f"Import error: {self.last_sql_error()}, {self.last_sql()}")
+        self.commit()
+        self.refresh()
 
     def _prepare_export(self, file, tick_callback=None):
         rez = []
         for x in self.records():
             rez.append(x)
             tick_callback() if tick_callback else None
 
@@ -355,18 +353,18 @@
             where_clause = f" where {where_clause}"
         return f"""select
                         name
                         , type as datatype
                         , `notnull` as nn
                         , `dflt_value` as `default`
                         , case when pk = 1 then '*' else ' ' end as pk
-                        , (SELECT "*" 
-                            FROM sqlite_master 
+                        , (SELECT "*"
+                            FROM sqlite_master
                             WHERE tbl_name="{table_name}"
-                                and ww.pk=1 
+                                and ww.pk=1
                                 and sql LIKE "%AUTOINCREMENT%"
                             ) as ai
                     from PRAGMA_table_info("{table_name}") ww
                     {where_clause}
                     """
 
 
@@ -384,15 +382,15 @@
     @staticmethod
     def get_table_columns_sql(table_name="", where_clause="", database_name=""):
         if where_clause:
             where_clause = f" and {where_clause}"
         return f"""select
                         column_name as name
                         , data_type as datatype
-                        , column_type 
+                        , column_type
                         , case when character_maximum_length<>0
                                 then character_maximum_length
                                 else numeric_precision
                         end as datalen
                         , numeric_scale as datadec
                         , column_key
                         , case when column_key = 'PRI' then '*' else ' ' end as pk
```

### Comparing `q2db-0.1.8/q2db/db.py` & `q2db-0.1.9/q2db/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,18 +359,18 @@
             elif self.db_engine_name == "sqlite3":
                 _column_definition["autoincrement"] = "AUTOINCREMENT"
             elif self.db_engine_name == "postgresql":
                 _column_definition["datatype"] = ""
                 _column_definition["primarykey"] = ""
                 _column_definition["autoincrement"] = "SERIAL PRIMARY KEY"
 
-        sql_column_text = """ {escape_char}{column}{escape_char} 
+        sql_column_text = """ {escape_char}{column}{escape_char}
                                 {datatype} {size}
-                                {primarykey} 
-                                {autoincrement} 
+                                {primarykey}
+                                {autoincrement}
                                 {default}""".format(
             **_column_definition
         )
         table = column_definition["table"]
 
         if table in self.get_tables(table):
             sql_cmd = f"ALTER TABLE {table} ADD {sql_column_text}"
@@ -532,15 +532,15 @@
                 if is_string_data:
                     primary_key_value = record.get(x, "")
                 else:
                     primary_key_value = int_(record.get(x, 0))
                 while (
                     self.cursor(
                         sql=f"""select {self.escape_char}{x}{self.escape_char}
-                                from {table_name} 
+                                from {table_name}
                                 where {self.escape_char}{x}{self.escape_char}='{primary_key_value}'
                             """
                     ).row_count()
                     > 0
                 ):
                     if is_string_data:
                         primary_key_value += "_"
```

### Comparing `q2db-0.1.8/q2db/schema.py` & `q2db-0.1.9/q2db/schema.py`

 * *Files identical despite different names*

### Comparing `q2db-0.1.8/q2db/utils.py` & `q2db-0.1.9/q2db/utils.py`

 * *Files identical despite different names*

### Comparing `q2db-0.1.8/setup.py` & `q2db-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mysql-connector-python>=8.0.29,<9.0.0', 'psycopg2-binary>=2.9.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'q2db',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'python DB API wrapper (MySQL, PostgreSQL, SQLite)',
     'long_description': '[![Python application](https://github.com/AndreiPuchko/q2db/actions/workflows/main.yml/badge.svg)](https://github.com/AndreiPuchko/q2db/actions/workflows/main.yml)\n# The light Python DB API wrapper with some ORM functions (MySQL, PostgreSQL, SQLite)\n## Quick start (run demo files)\n## - in docker:\n```bash\ngit clone https://github.com/AndreiPuchko/q2db && cd q2db/database.docker\n./up.sh\n./down.sh\n```  \n## - on your system:\n```bash\npip install q2db\ngit clone https://github.com/AndreiPuchko/q2db && cd q2db\n# sqlite:\npython3 ./demo/demo.py\n# mysql and postgresql:\npip install mysql-connector-python psycopg2-binary\npushd database.docker && docker-compose up -d && popd\npython3 ./demo/demo_mysql.py\npython3 ./demo/demo_postgresql.py\npushd database.docker && docker-compose down -v && popd\n```\n# Features:\n ---\n## Connect\n```python\nfrom q2db.db import Q2Db\n\ndatabase_sqlite = Q2Db("sqlite3", database_name=":memory:")\n# or just\ndatabase_sqlite = Q2Db()\n\n\ndatabase_mysql = Q2Db(\n    "mysql",\n    user="root",\n    password="q2test"\n    host="0.0.0.0",\n    port="3308",\n    database_name="q2test",\n)\n# or just\ndatabase_mysql = Q2Db(url="mysql://root:q2test@0.0.0.0:3308/q2test")\n\ndatabase_postgresql = Q2Db(\n    "postgresql",\n    user="q2user",\n    password="q2test"\n    host="0.0.0.0",\n    port=5432,\n    database_name="q2test1",\n)\n```\n---\n## Define & migrate database schema (ADD COLUMN only).\n```python\nq2db.schema import Q2DbSchema\n\nschema = Q2DbSchema()\n\nschema.add(table="topic_table", column="uid", datatype="int", datalen=9, pk=True)\nschema.add(table="topic_table", column="name", datatype="varchar", datalen=100)\n\nschema.add(table="message_table", column="uid", datatype="int", datalen=9, pk=True)\nschema.add(table="message_table", column="message", datatype="varchar", datalen=100)\nschema.add(\n    table="message_table",\n    column="parent_uid",\n    to_table="topic_table",\n    to_column="uid",\n    related="name"\n)\n\ndatabase.set_schema(schema)\n```\n---\n## INSERT, UPDATE, DELETE\n```python\ndatabase.insert("topic_table", {"name": "topic 0"})\ndatabase.insert("topic_table", {"name": "topic 1"})\ndatabase.insert("topic_table", {"name": "topic 2"})\ndatabase.insert("topic_table", {"name": "topic 3"})\n\ndatabase.insert("message_table", {"message": "Message 0 in 0", "parent_uid": 0})\ndatabase.insert("message_table", {"message": "Message 1 in 0", "parent_uid": 0})\ndatabase.insert("message_table", {"message": "Message 0 in 1", "parent_uid": 1})\ndatabase.insert("message_table", {"message": "Message 1 in 1", "parent_uid": 1})\n\n# this returns False because there is no value 2 in topic_table.id - schema works!\ndatabase.insert("message_table", {"message": "Message 1 in 1", "parent_uid": 2})\n\n\ndatabase.delete("message_table", {"uid": 2})\n\ndatabase.update("message_table", {"uid": 0, "message": "updated message"})\n```\n---\n## Cursor\n```python\ncursor = database.cursor(table_name="topic_table")\ncursor = database.cursor(\n    table_name="topic_table",\n    where=" name like \'%2%\'",\n    order="name desc"\n)\ncursor.insert({"name": "insert record via cursor"})\ncursor.delete({"uid": 2})\ncursor.update({"uid": 0, "message": "updated message"})\n\ncursor = database.cursor(sql="select name from topic_table")\n\nfor x in cursor.records():\n    print(x)\n    print(cursor.r.name)\n\ncursor.record(0)[\'name\']\ncursor.row_count()\ncursor.first()\ncursor.last()\ncursor.next()\ncursor.prev()\ncursor.bof()\ncursor.eof()\n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `q2db-0.1.8/PKG-INFO` & `q2db-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2db
-Version: 0.1.8
+Version: 0.1.9
 Summary: python DB API wrapper (MySQL, PostgreSQL, SQLite)
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

