# Comparing `tmp/mastodon_to_sqlite-0.1.1.tar.gz` & `tmp/mastodon_to_sqlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastodon_to_sqlite-0.1.1.tar", max compression
+gzip compressed data, was "mastodon_to_sqlite-0.2.0.tar", max compression
```

## Comparing `mastodon_to_sqlite-0.1.1.tar` & `mastodon_to_sqlite-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1231 2022-12-26 19:18:52.352953 mastodon_to_sqlite-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-12-22 17:17:52.956053 mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/__init__.py
--rw-r--r--   0        0        0     4551 2023-03-12 06:23:21.347147 mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/cli.py
--rw-r--r--   0        0        0     2862 2023-03-12 06:23:41.822021 mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/client.py
--rw-r--r--   0        0        0     6218 2023-03-12 06:34:06.187761 mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/service.py
--rw-r--r--   0        0        0      916 2023-03-12 06:36:25.756207 mastodon_to_sqlite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 mastodon_to_sqlite-0.1.1/setup.py
--rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 mastodon_to_sqlite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1553 2023-04-08 18:39:58.835837 mastodon_to_sqlite-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 18:39:58.835837 mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     6897 2023-04-08 18:39:58.839837 mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/cli.py
+-rw-r--r--   0        0        0     3180 2023-04-08 18:39:58.839837 mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/client.py
+-rw-r--r--   0        0        0     8400 2023-04-08 18:39:58.839837 mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/service.py
+-rw-r--r--   0        0        0      916 2023-04-08 18:39:58.839837 mastodon_to_sqlite-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 mastodon_to_sqlite-0.2.0/PKG-INFO
```

### Comparing `mastodon_to_sqlite-0.1.1/README.md` & `mastodon_to_sqlite-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # mastodon-to-sqlite
 
 Save data from Mastodon to a SQLite database.
 
 ## Install
 
 ```console
-foo@bar:~$ pip install -e git+https://github.com/myles/mastodon-to-sqlite.git#egg=mastodon-to-sqlite
+foo@bar:~$ pip install mastodon-to-sqlite
 ```
 
 ## Authentication
 
 First you will need to create an application on your Mastodon server. You
 can find that on your Mastodon serer.
 
@@ -48,7 +48,26 @@
 
 The `statuses` command will retrieve all the details about your Mastodon 
 statuses.
 
 ```console
 foo@bar:~$ mastodon-to-sqlite statuses mastodon.db
 ```
+
+## Retrieving Mastodon bookmarks
+
+The `bookmarks` command will retrieve all the details about your Mastodon
+bookmarks.
+
+```console
+foo@bar:~$ mastodon-to-sqlite bookmarks mastodon.db
+```
+
+
+## Retrieving Mastodon favourites
+
+The `favourites` command will retrieve all the details about your Mastodon
+favourites.
+
+```console
+foo@bar:~$ mastodon-to-sqlite favourites mastodon.db
+```
```

### Comparing `mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/client.py` & `mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,7 +77,17 @@
     ) -> Generator[Tuple[PreparedRequest, Response], None, None]:
         return self.request_paginated("GET", f"accounts/{account_id}/following")
 
     def accounts_statuses(
         self, account_id: str
     ) -> Generator[Tuple[PreparedRequest, Response], None, None]:
         return self.request_paginated("GET", f"accounts/{account_id}/statuses")
+
+    def bookmarks(
+        self,
+    ) -> Generator[Tuple[PreparedRequest, Response], None, None]:
+        return self.request_paginated("GET", "bookmarks")
+
+    def favourites(
+        self,
+    ) -> Generator[Tuple[PreparedRequest, Response], None, None]:
+        return self.request_paginated("GET", "favourites")
```

### Comparing `mastodon_to_sqlite-0.1.1/mastodon_to_sqlite/service.py` & `mastodon_to_sqlite-0.2.0/mastodon_to_sqlite/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -74,14 +74,37 @@
         )
         statuses_table.enable_fts(["content"], create_triggers=True)
 
     statuses_indexes = {tuple(i.columns) for i in statuses_table.indexes}
     if ("account_id",) not in statuses_indexes:
         statuses_table.create_index(["account_id"])
 
+    status_activities_table = get_table("status_activities", db=db)
+    if status_activities_table.exists() is False:
+        status_activities_table.create(
+            columns={
+                "account_id": int,
+                "activity": str,  # favourited, bookmarked
+                "status_id": int,
+            },
+            pk=("account_id", "activity", "status_id"),
+            foreign_keys=(
+                ("account_id", "accounts", "id"),
+                ("status_id", "statuses", "id"),
+            ),
+        )
+
+    status_activities_indexes = {
+        tuple(i.columns) for i in status_activities_table.indexes
+    }
+    if ("account_id", "activity") not in status_activities_indexes:
+        status_activities_table.create_index(["account_id", "activity"])
+    if ("status_id", "activity") not in status_activities_indexes:
+        status_activities_table.create_index(["status_id", "activity"])
+
 
 def get_client(auth_file_path: str) -> MastodonClient:
     """
     Returns a fully authenticated MastodonClient.
     """
     with Path(auth_file_path).absolute().open() as file_obj:
         raw_auth = file_obj.read()
@@ -202,17 +225,20 @@
 def transformer_status(status: Dict[str, Any]):
     """
     Transformer a Mastodon status, so it can be safely saved to the SQLite
     database.
     """
     account = status.pop("account")
 
-    to_remove = [
-        k for k in status.keys() if k not in ("id", "created_at", "content")
-    ]
+    to_keep = (
+        "id",
+        "created_at",
+        "content",
+    )
+    to_remove = [k for k in status.keys() if k not in to_keep]
     for key in to_remove:
         del status[key]
 
     status["account_id"] = account["id"]
 
 
 def save_statuses(db: Database, statuses: List[Dict[str, Any]]):
@@ -222,7 +248,53 @@
     build_database(db)
     statuses_table = get_table("statuses", db=db)
 
     for status in statuses:
         transformer_status(status)
 
     statuses_table.upsert_all(statuses, pk="id")
+
+
+def get_bookmarks(
+    account_id: str, client: MastodonClient
+) -> Generator[List[Dict[str, Any]], None, None]:
+    """
+    Get authenticated account's bookmarks.
+    """
+    for request, response in client.bookmarks():
+        yield response.json()
+
+
+def get_favourites(
+    account_id: str, client: MastodonClient
+) -> Generator[List[Dict[str, Any]], None, None]:
+    """
+    Get authenticated account's favourites.
+    """
+    for request, response in client.favourites():
+        yield response.json()
+
+
+def save_activities(type: str, db: Database, statuses: List[Dict[str, Any]]):
+    """
+    Save Mastodon activities to the SQLite database.
+    """
+    build_database(db)
+    statuses_table = get_table("statuses", db=db)
+    status_activities_table = get_table("status_activities", db=db)
+
+    for status in statuses:
+        transformer_status(status)
+
+    statuses_table.upsert_all(statuses, pk="id")
+
+    status_activities_table.upsert_all(
+        (
+            {
+                "account_id": status["account_id"],
+                "activity": type,
+                "status_id": status["id"],
+            }
+            for status in statuses
+        ),
+        pk=("account_id", "activity", "status_id"),
+    )
```

### Comparing `mastodon_to_sqlite-0.1.1/pyproject.toml` & `mastodon_to_sqlite-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mastodon-to-sqlite"
-version = "0.1.1"
+version = "0.2.0"
 description = "Save data from Mastodon to a SQLite database"
 authors = ["Myles Braithwaite <me@mylesbraithwaite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/myles/mastodon-to-sqlite"
 keywords = ["mastodon", "sqlite", "dogsheep"]
```

### Comparing `mastodon_to_sqlite-0.1.1/PKG-INFO` & `mastodon_to_sqlite-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastodon-to-sqlite
-Version: 0.1.1
+Version: 0.2.0
 Summary: Save data from Mastodon to a SQLite database
 Home-page: https://github.com/myles/mastodon-to-sqlite
 License: Apache-2.0
 Keywords: mastodon,sqlite,dogsheep
 Author: Myles Braithwaite
 Author-email: me@mylesbraithwaite.com
 Requires-Python: >=3.9,<4.0
@@ -22,15 +22,15 @@
 # mastodon-to-sqlite
 
 Save data from Mastodon to a SQLite database.
 
 ## Install
 
 ```console
-foo@bar:~$ pip install -e git+https://github.com/myles/mastodon-to-sqlite.git#egg=mastodon-to-sqlite
+foo@bar:~$ pip install mastodon-to-sqlite
 ```
 
 ## Authentication
 
 First you will need to create an application on your Mastodon server. You
 can find that on your Mastodon serer.
 
@@ -70,7 +70,26 @@
 The `statuses` command will retrieve all the details about your Mastodon 
 statuses.
 
 ```console
 foo@bar:~$ mastodon-to-sqlite statuses mastodon.db
 ```
 
+## Retrieving Mastodon bookmarks
+
+The `bookmarks` command will retrieve all the details about your Mastodon
+bookmarks.
+
+```console
+foo@bar:~$ mastodon-to-sqlite bookmarks mastodon.db
+```
+
+
+## Retrieving Mastodon favourites
+
+The `favourites` command will retrieve all the details about your Mastodon
+favourites.
+
+```console
+foo@bar:~$ mastodon-to-sqlite favourites mastodon.db
+```
+
```

