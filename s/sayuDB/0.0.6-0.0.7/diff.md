# Comparing `tmp/sayuDB-0.0.6.tar.gz` & `tmp/sayuDB-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-0.0.6.tar", last modified: Fri Apr  7 20:05:47 2023, max compression
+gzip compressed data, was "sayuDB-0.0.7.tar", last modified: Sat Apr  8 21:56:34 2023, max compression
```

## Comparing `sayuDB-0.0.6.tar` & `sayuDB-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.797187 sayuDB-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-07 17:42:40.000000 sayuDB-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5890 2023-04-07 20:05:47.793187 sayuDB-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5967 2023-04-07 17:42:40.000000 sayuDB-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.793187 sayuDB-0.0.6/sayuDB/
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-07 17:42:40.000000 sayuDB-0.0.6/sayuDB/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-07 20:04:03.000000 sayuDB-0.0.6/sayuDB/__main__.py
--rw-r--r--   0 root         (0) root         (0)    14085 2023-04-07 19:03:04.000000 sayuDB-0.0.6/sayuDB/processor.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-04-07 19:28:19.000000 sayuDB-0.0.6/sayuDB/remote.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-04-07 20:02:49.000000 sayuDB-0.0.6/sayuDB/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.793187 sayuDB-0.0.6/sayuDB.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5890 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 20:05:47.797187 sayuDB-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6275 2023-04-07 20:04:44.000000 sayuDB-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.620056 sayuDB-0.0.7/
+-rw-rw-rw-   0        0        0     1064 2023-04-08 21:51:28.000000 sayuDB-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6072 2023-04-08 21:56:34.619053 sayuDB-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5767 2023-04-08 21:51:28.000000 sayuDB-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.604652 sayuDB-0.0.7/sayuDB/
+-rw-rw-rw-   0        0        0      635 2023-04-08 21:51:28.000000 sayuDB-0.0.7/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-04-08 21:54:44.000000 sayuDB-0.0.7/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    14630 2023-04-08 21:52:04.000000 sayuDB-0.0.7/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-08 21:52:33.000000 sayuDB-0.0.7/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-04-08 21:52:17.000000 sayuDB-0.0.7/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.619053 sayuDB-0.0.7/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     6072 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 21:56:34.620056 sayuDB-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     6275 2023-04-08 21:53:46.000000 sayuDB-0.0.7/setup.py
```

### Comparing `sayuDB-0.0.6/LICENSE` & `sayuDB-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Arsybai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Arsybai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sayuDB-0.0.6/PKG-INFO` & `sayuDB-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: sayuDB
-Version: 0.0.6
-Summary: Database management system based on python and JSON.
-Home-page: https://github.com/Arsybai/sayuDB
-Author: Arsybai
-Author-email: me@arsybai.com
-License: MIT
-Keywords: database
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
 
 # Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
@@ -39,36 +28,44 @@
 Before you can use sayuDB you need to install it, of course.
 Just clone this repository and place it to your project folder.
 ```shell
 > pip3 install sayuDB
 ```
 for help menu:
 ```shell
-> python3 sayuDB --h
+> python3 -m sayuDB --h
 ```
 
 #### 1.2 Creating database
 The first test to see whether you can access the database server is to try to create a database.
 
 To create a new database, in this example named `myDB`, you use the following funtion:
 ```python
 import sayuDB
 
 # Creating database
 sayuDB.create_database('myDB')
 ```
+
+```shell
+> python3 -m sayuDB create database <database_name>
+```
 You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
 
 If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
 ```python
 import sayuDB
 
 sayuDB.drop_database('myDB')
 ```
 
+```shell
+> python3 -m sayuDB drop database <database_name>
+```
+
 You can import export using:
 ```python
 # Exporting database (must use file name)
 sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
 # Importing database
 sayuDB.import_database(path_='/<path>/filename.ezdb')
 ```
@@ -197,9 +194,7 @@
 Look at the new state of the data:
 ```shell
 name       age  city
 -------  -----  ------------------
 Arsybai     23  Solo, Indonesia
 Moepoi      21  Jakarta, Indonesia
 ```
-
-
```

### Comparing `sayuDB-0.0.6/README.md` & `sayuDB-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
+Metadata-Version: 2.1
+Name: sayuDB
+Version: 0.0.7
+Summary: Database management system based on python and JSON.
+Home-page: https://github.com/Arsybai/sayuDB
+Author: Arsybai
+Author-email: me@arsybai.com
+License: MIT
+Keywords: database
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
@@ -28,44 +38,36 @@
 Before you can use sayuDB you need to install it, of course.
 Just clone this repository and place it to your project folder.
 ```shell
 > pip3 install sayuDB
 ```
 for help menu:
 ```shell
-> python3 -m sayuDB --h
+> python3 sayuDB --h
 ```
 
 #### 1.2 Creating database
 The first test to see whether you can access the database server is to try to create a database.
 
 To create a new database, in this example named `myDB`, you use the following funtion:
 ```python
 import sayuDB
 
 # Creating database
 sayuDB.create_database('myDB')
 ```
-
-```shell
-> python3 -m sayuDB create database <database_name>
-```
 You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
 
 If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
 ```python
 import sayuDB
 
 sayuDB.drop_database('myDB')
 ```
 
-```shell
-> python3 -m sayuDB drop database <database_name>
-```
-
 You can import export using:
 ```python
 # Exporting database (must use file name)
 sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
 # Importing database
 sayuDB.import_database(path_='/<path>/filename.ezdb')
 ```
```

### Comparing `sayuDB-0.0.6/sayuDB/__init__.py` & `sayuDB-0.0.7/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.6/sayuDB/__main__.py` & `sayuDB-0.0.7/sayuDB/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except:
     print("Read the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""Invalid commad. get help by
 --h""")
     exit()
 
 if sys.argv[1] == "help" or sys.argv[1] == '--h':
-    print("sayuDB v0.0.6\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
+    print("sayuDB v0.0.7\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""
 [ USERS ]
 Show Users  \t\t: show users
 Create user \t\t: create user <username> <password>
 Remove user \t\t: remove user <username>
 
 [ DATABASE ]
@@ -36,16 +36,14 @@
 Grant user \t\t: grant user <username> <database_name>
 Import Database \t: import database <path_to_ezdb>
 Export Database \t: export database <database_name> <output_path>
 
 [ SERVER ]
 Activate Server \t: activate server <port>
 Deactivate Server \t: deactivate server
-Block IP  \t\t: block ip <ip> (coming soon)
-Unblock IP  \t\t: unblock ip <ip> (coming soon)
 
 if you can't access the server after activate. setup the public access by
 setup public server <server_name> <port>
 leave it with your server public IP in server_name if you don't have domain and the port must be same when you activate
 after that you can acces it within your IP server.
     """)
```

### Comparing `sayuDB-0.0.6/sayuDB/processor.py` & `sayuDB-0.0.7/sayuDB/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,15 @@
         
         the datatypes:
         - str   
         - float
         - int   
         - dict
         """
-        with open(f'{os.path.dirname(__file__)}/datas/{self.database}.ezdb', 'r') as rdb:
-            rdb = eval(rdb.read())
+        rdb = self.openDB()
         if name in rdb:
             print("Table already exist")
         else:
             tables_ = {
                 "name": name,
                 "column": {},
                 "datas":[]
@@ -195,14 +194,28 @@
                         data_[i] = eval(str(contents[idx]))
                 except:
                     print(f"The content typedata invalid at column {i} content {contents[idx]}")
                     sys.exit()
             idx += 1
         db_[table]['datas'].append(data_)
         self.save_table(table, db_)
+
+    def insert_many(self, table:str, col, contents:list):
+        """
+        contents = [
+        ["a"],
+        ["b"]
+        ]
+        """
+        try:
+            contents[0][0]
+            for row in contents:
+                self.insert_row(table, col, row)
+        except:
+            raise Exception("Invalid contents list")
         
     def select_row(self, table: str, col, where=None, order_by=None, as_json=False, limit=None):
         """_summary_
 
         Args:
             table (str): The table name
             col (_type_): The column what you want to show. use * for all column
@@ -296,14 +309,25 @@
                     i[set_col] = set_val
             else:
                 if i[col_] == val_:
                     i[set_col] = set_val
         self.save_table(table, db_)
         return "Column updated"
     
+    def update_row_json(self, table:str, set_:object, where:str):
+        """
+        set_ = {
+        "col1":"data1",
+        "col2":"data2"
+        }
+        """
+        for i in set_:
+            self.update_row(table, f"{i}={set_[i]}", where)
+        return "Column updated"
+    
     def delete_row(self, table: str, where: str):
         db_ = self.openDB()
         if table not in db_:
             sys.exit("Table not found")
         if '=' in where:
             col_ = where.split('=')[0]
             val_ = where.split('=')[1]
```

### Comparing `sayuDB-0.0.6/sayuDB/remote.py` & `sayuDB-0.0.7/sayuDB/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def database_exsistence(self, database:str):
         response = sendRequest(self.host+'/existence', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database})
         if response != 'ok':
             exit(response)
         return True
     
     def commit_database(self, database:str, content):
-        response = sendRequest(self.host+'/commit', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database, 'content':str(encode_base64(content))}, 'POST')
+        response = sendRequest(self.host+'/commit', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database, 'content':encode_base64(str(content))}, 'POST')
         if response != 'ok':
             exit(response)
         return True
     
     def pull_database(self, database:str):
         response = sendRequest(self.host+'/pull', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database})
         return json.loads(response)
```

### Comparing `sayuDB-0.0.6/sayuDB/server.py` & `sayuDB-0.0.7/sayuDB/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     with open('config.json', 'w')as wconf:
         json.dump(config(), wconf, indent=4)
     return
 
 def checkAuth():
     username = decode_base64(request.form['username'])
     password = decode_base64(request.form['password'])
-    if username not in user:
+    if username not in user():
         return "User not found"
     if password != user()[username]['password']:
         return "Invalid credentials"
     if username == 'root':
         return "Action rejected"
     return True
 
@@ -78,28 +78,28 @@
         return "Database not found in server"
     return 'ok'
     
 @app.route('/commit', methods=['POST'])
 def commit():
     username = decode_base64(request.form['username'])
     database = request.form['database']
-    content = json.load(decode_base64(request.form['content']))
+    content = decode_base64(request.form['content'])
     if not checkAuth():
         return "Authorization rejected"
     if not hasAccess(username, database):
         return "Database not found in server"
-    sayuDB.sayuDB(database).save_db(content)
+    sayuDB.sayuDB(database).save_db(eval(content))
     return 'ok'
 
 @app.route('/pull')
 def pull():
     username = decode_base64(request.form['username'])
     database = request.form['database']
     if not checkAuth():
         return "Authorization rejected"
     if not hasAccess(username, database):
         return "Database not found in server"
-    return sayuDB.sayuDB(database).openDB()
+    return jsonify(sayuDB.sayuDB(database).openDB())
 
 
 if __name__ == "__main__":
     app.run(debug=True, port=int(sys.argv[1]), host='0.0.0.0')
```

### Comparing `sayuDB-0.0.6/sayuDB.egg-info/PKG-INFO` & `sayuDB-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,205 +1,212 @@
-Metadata-Version: 2.1
-Name: sayuDB
-Version: 0.0.6
-Summary: Database management system based on python and JSON.
-Home-page: https://github.com/Arsybai/sayuDB
-Author: Arsybai
-Author-email: me@arsybai.com
-License: MIT
-Keywords: database
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Documentation
-
-##### Table of content
-###### Preface
-1. [What is sayuDB](#1_What_is_sayuDB_18)
-
-###### Tutorial
-1. [Getting Started](#1-getting-started)
-- 1.1 [Installation](#11-installation)
-- 1.2 [Creating database](#12-creating-database)
-- 1.3 [Creating a New Table](#13-creating-a-new-table)
-- 1.4 [Populating a table with rows](#14-pupulating-a-table-with-rows)
-- 1.5 [Querying a Table](#15-querying-a-table)
-- 1.6 [Updates](#updates)
-- 1.7 [Deletion](#17-deletion)
-
----
-# Preface
-### 1. What is sayuDB
-sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
-It supports a large part of the SQL standard feature
-
-# Tutorial
-### 1. Getting Started
-#### 1.1 Installation
-Before you can use sayuDB you need to install it, of course.
-Just clone this repository and place it to your project folder.
-```shell
-> pip3 install sayuDB
-```
-for help menu:
-```shell
-> python3 sayuDB --h
-```
-
-#### 1.2 Creating database
-The first test to see whether you can access the database server is to try to create a database.
-
-To create a new database, in this example named `myDB`, you use the following funtion:
-```python
-import sayuDB
-
-# Creating database
-sayuDB.create_database('myDB')
-```
-You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
-
-If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
-```python
-import sayuDB
-
-sayuDB.drop_database('myDB')
-```
-
-You can import export using:
-```python
-# Exporting database (must use file name)
-sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
-# Importing database
-sayuDB.import_database(path_='/<path>/filename.ezdb')
-```
-
-#### 1.3 Creating a New Table
-You can create a new table by specifying the table name, along with all column names and their types:
-
-you must define the database first with:
-```python
-import sayuDB
-
-db = sayuDB.sayuDB(database='myDB')
-```
-
-then
-```python
-db.create_table('people', [
-    ['name','str'],
-    ['age','int'],
-    ['city','str']
-])
-```
-sayuDB currenly support data types `str`,`int`,`float`,`dict`
-
-If you want to show the table, using this following function:
-```python
-db.show_table(name='people')
-```
-it will returned as printed table:
-```shell
-name    column    datas
-------  --------  -------
-```
-
-Finally, it should be mentioned that if you don't need a table any longer or want to recreate it differently you can remove it using the following function:
-```python
-db.drop_table(name='people')
-```
-
-#### 1.4 Populating a Table With Rows
-The `insert_row` function is used to populate a table with rows:
-```python
-db.insert_row(table='people', col='name,age,city', contents=['Arsybai', 23, 'Solo, Indonesia'])
-```
-_You can also use col as list. EX `['name','age','city']`_
-
-### 1.5 Querying a Table
-To retrieve data from a table, the table is queried. An `select_row` funtion is used to do this. The funtion is divided into a select list (the part that lists the columns to be returned), a table list (the part that lists the tables from which to retrieve the data), and an optional qualification (the part that specifies any restrictions). For example, to retrieve all the rows of table `people`, type:
-```python
-data = db.select_row(table='people', col='*')
-print(data)
-```
-Here `*` is a shorthand for “all columns”. So the same result would be had with:
-```python
-db.select_row(table='people', col='name,age,city')
-```
-The output should be:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Ataro       25  Bekasi, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-
-If you want the output is json, use `as_json=True`:
-```python
-data = db.select_row(table='people', col='*', as_json=True)
-print(data)
-```
-
-A query can be “qualified” by adding a `where` clause that specifies which rows are wanted:
-```python
-data = db.select_row(table='people', col='*', where='age=23')
-print(data)
-```
-you can also use ` contain ` for specific column that contain some value:
-```python
-data = db.select_row(table='people', col='*', where='age contain 23')
-print(data)
-```
-Result:
-```shell
-name       age  city
--------  -----  ---------------
-Arsybai     23  Solo, Indonesia
-```
-
-You can request that the results of a query be returned in sorted order:
-```python
-data = db.select_row(table='people', col='*', order_by='age|asc')
-print(data)
-```
-_The order should be `asc` or `desc`_
-
-Result:
-```shell
-name       age  city
--------  -----  ------------------
-Moepoi      21  Jakarta, Indonesia
-Arsybai     23  Solo, Indonesia
-Ataro       25  Bekasi, Indonesia
-```
-
-#### Updates
-You can update existing rows using the `update_row`.
-as example I want to set `Ataro` age to `26`:
-```python
-db.update_row(table='people', set_='age=26', where='name=Ataro')
-```
-Look at the new state of the data:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Ataro       26  Bekasi, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-
-#### Deletion
-Rows can be removed from a table using the `delete_row`:
-```python
-db.delete_row(table='people', where='name=Ataro')
-```
-
-Look at the new state of the data:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-
-
+import setuptools
+
+setuptools.setup(
+    name="sayuDB",
+    version="0.0.7",
+    author="Arsybai",
+    description="Database management system based on python and JSON.",
+    packages=["sayuDB"],
+    license="MIT",
+    author_email="me@arsybai.com",
+    url="https://github.com/Arsybai/sayuDB",
+    keywords=[
+        'database',
+    ],
+    install_requires=[
+    'requests',
+    'tabulate',
+    'flask'
+    ],
+    long_description_content_type="text/markdown",
+    long_description="""# Documentation
+
+##### Table of content
+###### Preface
+1. [What is sayuDB](#1_What_is_sayuDB_18)
+
+###### Tutorial
+1. [Getting Started](#1-getting-started)
+- 1.1 [Installation](#11-installation)
+- 1.2 [Creating database](#12-creating-database)
+- 1.3 [Creating a New Table](#13-creating-a-new-table)
+- 1.4 [Populating a table with rows](#14-pupulating-a-table-with-rows)
+- 1.5 [Querying a Table](#15-querying-a-table)
+- 1.6 [Updates](#updates)
+- 1.7 [Deletion](#17-deletion)
+
+---
+# Preface
+### 1. What is sayuDB
+sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
+It supports a large part of the SQL standard feature
+
+# Tutorial
+### 1. Getting Started
+#### 1.1 Installation
+Before you can use sayuDB you need to install it, of course.
+Just clone this repository and place it to your project folder.
+```shell
+> pip3 install sayuDB
+```
+for help menu:
+```shell
+> python3 sayuDB --h
+```
+
+#### 1.2 Creating database
+The first test to see whether you can access the database server is to try to create a database.
+
+To create a new database, in this example named `myDB`, you use the following funtion:
+```python
+import sayuDB
+
+# Creating database
+sayuDB.create_database('myDB')
+```
+You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
+
+If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
+```python
+import sayuDB
+
+sayuDB.drop_database('myDB')
+```
+
+You can import export using:
+```python
+# Exporting database (must use file name)
+sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
+# Importing database
+sayuDB.import_database(path_='/<path>/filename.ezdb')
+```
+
+#### 1.3 Creating a New Table
+You can create a new table by specifying the table name, along with all column names and their types:
+
+you must define the database first with:
+```python
+import sayuDB
+
+db = sayuDB.sayuDB(database='myDB')
+```
+
+then
+```python
+db.create_table('people', [
+    ['name','str'],
+    ['age','int'],
+    ['city','str']
+])
+```
+sayuDB currenly support data types `str`,`int`,`float`,`dict`
+
+If you want to show the table, using this following function:
+```python
+db.show_table(name='people')
+```
+it will returned as printed table:
+```shell
+name    column    datas
+------  --------  -------
+```
+
+Finally, it should be mentioned that if you don't need a table any longer or want to recreate it differently you can remove it using the following function:
+```python
+db.drop_table(name='people')
+```
+
+#### 1.4 Populating a Table With Rows
+The `insert_row` function is used to populate a table with rows:
+```python
+db.insert_row(table='people', col='name,age,city', contents=['Arsybai', 23, 'Solo, Indonesia'])
+```
+_You can also use col as list. EX `['name','age','city']`_
+
+### 1.5 Querying a Table
+To retrieve data from a table, the table is queried. An `select_row` funtion is used to do this. The funtion is divided into a select list (the part that lists the columns to be returned), a table list (the part that lists the tables from which to retrieve the data), and an optional qualification (the part that specifies any restrictions). For example, to retrieve all the rows of table `people`, type:
+```python
+data = db.select_row(table='people', col='*')
+print(data)
+```
+Here `*` is a shorthand for “all columns”. So the same result would be had with:
+```python
+db.select_row(table='people', col='name,age,city')
+```
+The output should be:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Ataro       25  Bekasi, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+
+If you want the output is json, use `as_json=True`:
+```python
+data = db.select_row(table='people', col='*', as_json=True)
+print(data)
+```
+
+A query can be “qualified” by adding a `where` clause that specifies which rows are wanted:
+```python
+data = db.select_row(table='people', col='*', where='age=23')
+print(data)
+```
+you can also use ` contain ` for specific column that contain some value:
+```python
+data = db.select_row(table='people', col='*', where='age contain 23')
+print(data)
+```
+Result:
+```shell
+name       age  city
+-------  -----  ---------------
+Arsybai     23  Solo, Indonesia
+```
+
+You can request that the results of a query be returned in sorted order:
+```python
+data = db.select_row(table='people', col='*', order_by='age|asc')
+print(data)
+```
+_The order should be `asc` or `desc`_
+
+Result:
+```shell
+name       age  city
+-------  -----  ------------------
+Moepoi      21  Jakarta, Indonesia
+Arsybai     23  Solo, Indonesia
+Ataro       25  Bekasi, Indonesia
+```
+
+#### Updates
+You can update existing rows using the `update_row`.
+as example I want to set `Ataro` age to `26`:
+```python
+db.update_row(table='people', set_='age=26', where='name=Ataro')
+```
+Look at the new state of the data:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Ataro       26  Bekasi, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+
+#### Deletion
+Rows can be removed from a table using the `delete_row`:
+```python
+db.delete_row(table='people', where='name=Ataro')
+```
+
+Look at the new state of the data:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+"""
+)
```

### Comparing `sayuDB-0.0.6/setup.py` & `sayuDB-0.0.7/sayuDB.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-import setuptools
+Metadata-Version: 2.1
+Name: sayuDB
+Version: 0.0.7
+Summary: Database management system based on python and JSON.
+Home-page: https://github.com/Arsybai/sayuDB
+Author: Arsybai
+Author-email: me@arsybai.com
+License: MIT
+Keywords: database
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-setuptools.setup(
-    name="sayuDB",
-    version="0.0.6",
-    author="Arsybai",
-    description="Database management system based on python and JSON.",
-    packages=["sayuDB"],
-    license="MIT",
-    author_email="me@arsybai.com",
-    url="https://github.com/Arsybai/sayuDB",
-    keywords=[
-        'database',
-    ],
-    install_requires=[
-    'requests',
-    'tabulate',
-    'flask'
-    ],
-    long_description_content_type="text/markdown",
-    long_description="""# Documentation
+# Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
 ###### Tutorial
 1. [Getting Started](#1-getting-started)
@@ -204,9 +196,7 @@
 Look at the new state of the data:
 ```shell
 name       age  city
 -------  -----  ------------------
 Arsybai     23  Solo, Indonesia
 Moepoi      21  Jakarta, Indonesia
 ```
-"""
-)
```

