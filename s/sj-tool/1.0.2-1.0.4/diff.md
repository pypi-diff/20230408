# Comparing `tmp/sj_tool-1.0.2-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 10001 bytes, number of entries: 23
+Zip file size: 10265 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
 -rw-rw-rw-  2.0 fat     1710 b- defN 23-Mar-31 04:11 sj_tool/scheduler.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Apr-04 05:43 sj_tool/system.py
 -rw-rw-rw-  2.0 fat      597 b- defN 23-Apr-04 05:43 sj_tool/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:40 sj_tool/db/__init__.py
--rw-rw-rw-  2.0 fat     5667 b- defN 23-Mar-27 02:33 sj_tool/db/mongo.py
--rw-rw-rw-  2.0 fat     2035 b- defN 23-Mar-24 10:52 sj_tool/db/mysql.py
+-rw-rw-rw-  2.0 fat     5626 b- defN 23-Apr-08 09:02 sj_tool/db/mongo.py
+-rw-rw-rw-  2.0 fat     1237 b- defN 23-Apr-08 08:39 sj_tool/db/mysql.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:29 sj_tool/fjsp/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:30 sj_tool/fjsp/entity/__init__.py
--rw-rw-rw-  2.0 fat      442 b- defN 23-Mar-27 11:02 sj_tool/fjsp/entity/job.py
+-rw-rw-rw-  2.0 fat      463 b- defN 23-Apr-08 16:59 sj_tool/fjsp/entity/changeover.py
+-rw-rw-rw-  2.0 fat      663 b- defN 23-Apr-08 16:47 sj_tool/fjsp/entity/job.py
 -rw-rw-rw-  2.0 fat      374 b- defN 23-Mar-27 11:20 sj_tool/fjsp/entity/machine.py
 -rw-rw-rw-  2.0 fat      617 b- defN 23-Mar-27 11:02 sj_tool/fjsp/entity/operation.py
--rw-rw-rw-  2.0 fat       77 b- defN 23-Mar-27 11:20 sj_tool/fjsp/entity/product.py
+-rw-rw-rw-  2.0 fat      109 b- defN 23-Apr-08 16:59 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
--rw-rw-rw-  2.0 fat     1779 b- defN 23-Mar-30 05:51 sj_tool/logger/text_logger.py
--rw-rw-rw-  2.0 fat     2077 b- defN 23-Mar-31 08:22 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      468 b- defN 23-Apr-08 08:01 sj_tool-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 08:01 sj_tool-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-08 08:01 sj_tool-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1797 b- defN 23-Apr-08 08:01 sj_tool-1.0.2.dist-info/RECORD
-23 files, 18929 bytes uncompressed, 7089 bytes compressed:  62.5%
+-rw-rw-rw-  2.0 fat     1866 b- defN 23-Apr-08 12:57 sj_tool/logger/text_logger.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-08 11:50 sj_tool/logger/visual_logger.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1887 b- defN 23-Apr-08 17:05 sj_tool-1.0.4.dist-info/RECORD
+24 files, 18992 bytes uncompressed, 7211 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: sj_tool/fjsp/__init__.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/__init__.py
 Comment: 
 
+Filename: sj_tool/fjsp/entity/changeover.py
+Comment: 
+
 Filename: sj_tool/fjsp/entity/job.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/machine.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/operation.py
@@ -51,20 +54,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.2.dist-info/METADATA
+Filename: sj_tool-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.2.dist-info/WHEEL
+Filename: sj_tool-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.2.dist-info/top_level.txt
+Filename: sj_tool-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.2.dist-info/RECORD
+Filename: sj_tool-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/db/mongo.py

```diff
@@ -32,126 +32,126 @@
 
     Returns:
         返回 pymongo.collection.Collection 对象，代表创建的 MongoDB 集合
     """
     return database[collection_name]
 
 
-def insert_one_doc(collection: pymongo.collection.Collection, doc: Dict) -> InsertOneResult:
+def insert_one(collection: pymongo.collection.Collection, doc: Dict) -> InsertOneResult:
     """
     向 MongoDB 集合中插入一条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要插入文档的 MongoDB 集合
         doc: 要插入的文档数据，一个 Python 字典对象
 
     Returns:
         返回 InsertOneResult 对象，代表插入操作的结果
     """
     return collection.insert_one(doc)
 
 
-def insert_many_docs(collection: pymongo.collection.Collection, docs: List[Dict]) -> InsertManyResult:
+def insert_many(collection: pymongo.collection.Collection, docs: List[Dict]) -> InsertManyResult:
     """
     向 MongoDB 集合中插入多条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要插入文档的 MongoDB 集合
         docs: 要插入的多个文档数据，一个 Python 字典对象的列表
 
     Returns:
         返回 results.InsertManyResult 对象，代表插入操作的结果
     """
     return collection.insert_many(docs)
 
 
-def find_one_doc(collection: pymongo.collection.Collection) -> Dict:
+def find_one(collection: pymongo.collection.Collection) -> Dict:
     """
     查询 MongoDB 集合中的一条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要查询的 MongoDB 集合
 
     Returns:
         返回一个 Python 字典对象，代表查询到的 MongoDB 文档数据
     """
     return collection.find_one()
 
 
-def find_all_docs(collection: pymongo.collection.Collection) -> pymongo.cursor.Cursor:
+def find_all(collection: pymongo.collection.Collection) -> pymongo.cursor.Cursor:
     """
     查询 MongoDB 集合中的所有文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要查询的 MongoDB 集合
 
     Returns:
         返回一个 pymongo.cursor.Cursor 对象，代表查询到的 MongoDB 文档的游标
     """
     return collection.find()
 
 
-def find_docs_by_query(collection: pymongo.collection.Collection, query: Dict) -> pymongo.cursor.Cursor:
+def find_by_query(collection: pymongo.collection.Collection, query: Dict) -> pymongo.cursor.Cursor:
     """
     根据查询条件查询 MongoDB 集合中的文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要查询的 MongoDB 集合
         query: 查询条件，一个 Python 字典对象，例如 {"age": 30}
 
     Returns:
         返回一个 pymongo.cursor.Cursor 对象，代表
     """
     return collection.find(query)
 
 
-def delete_one_doc(collection: pymongo.collection.Collection, query: Dict) -> DeleteResult:
+def delete_one(collection: pymongo.collection.Collection, query: Dict) -> DeleteResult:
     """
     从 MongoDB 集合中删除一条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要删除文档的 MongoDB 集合
         query: 删除条件，一个 Python 字典对象，例如 {"name": "John"}
 
     Returns:
         返回 DeleteResult 对象，代表删除操作的结果
     """
     return collection.delete_one(query)
 
 
-def delete_many_docs(collection: pymongo.collection.Collection, query: Dict) -> DeleteResult:
+def delete_many(collection: pymongo.collection.Collection, query: Dict) -> DeleteResult:
     """
     从 MongoDB 集合中删除多条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要删除文档的 MongoDB 集合
         query: 删除条件，一个 Python 字典对象，例如 {"age": {"$gt": 25}}，若为{}，则删除所有文档
 
     Returns:
         返回 DeleteResult 对象，代表删除操作的结果
     """
     return collection.delete_many(query)
 
 
-def update_one_doc(collection: pymongo.collection.Collection, query: Dict, update: Dict) -> UpdateResult:
+def update_one(collection: pymongo.collection.Collection, query: Dict, update: Dict) -> UpdateResult:
     """
     更新 MongoDB 集合中的一条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要更新文档的 MongoDB 集合
         query: 更新条件，一个 Python 字典对象，例如 {"name": "John"}
         update: 要更新的文档数据，一个 Python 字典对象，例如 {"$set": {"age": 25}}
 
     Returns:
         返回 UpdateResult 对象，代表更新操作的结果
     """
     return collection.update_one(query, update)
 
 
-def update_many_docs(collection: pymongo.collection.Collection, query: Dict, update: Dict) -> UpdateResult:
+def update_many(collection: pymongo.collection.Collection, query: Dict, update: Dict) -> UpdateResult:
     """
     更新 MongoDB 集合中的多条文档
 
     Args:
         collection: pymongo.collection.Collection 对象，代表要更新文档的 MongoDB 集合
         query: 更新条件，一个 Python 字典对象，例如 {"age": {"$lt": 30}}
         update: 要更新的文档数据，一个 Python 字典对象，例如 {"$set": {"age": 30}}
```

## sj_tool/db/mysql.py

```diff
@@ -1,73 +1,41 @@
-import os
 from playhouse.pool import PooledMySQLDatabase
-from peewee import Model, CharField, IntegerField, MySQLDatabase
 
 
 # 定义数据库连接池
-def create_connection_pool(database, max_connections=8, stale_timeout=300, **kwargs):
-    return PooledMySQLDatabase(database, max_connections=max_connections, stale_timeout=stale_timeout, **kwargs)
-
-
-db = PooledMySQLDatabase(
-    "mydatabase",
-    max_connections=8,
-    stale_timeout=300,
-    user="myusername",
-    password="mypassword",
-    host="localhost",
-    port=3306,
-)
+def create_connection_pool(database, user, password, host, port=3306, max_connections=8, stale_timeout=300, **kwargs):
+    return PooledMySQLDatabase(
+        database,
+        user=user,
+        password=password,
+        host=host,
+        port=port,
+        max_connections=max_connections,
+        stale_timeout=stale_timeout,
+        **kwargs
+    )
 
 
 # 定义通用增删改查函数
-def create_record(model_class, **kwargs):
+def create_record(db, model_class, **kwargs):
     with db.atomic():
         record = model_class.create(**kwargs)
         return record.id
 
 
-def update_record(model_class, record_id, **kwargs):
+def update_record(db, model_class, record_id, **kwargs):
     with db.atomic():
         query = model_class.update(**kwargs).where(model_class.id == record_id)
         return query.execute()
 
 
-def delete_record(model_class, record_id):
+def delete_record(db, model_class, record_id):
     with db.atomic():
         query = model_class.delete().where(model_class.id == record_id)
         return query.execute()
 
 
-def get_records(model_class, *select_fields, **where):
+def get_records(db, model_class, *select_fields, **where):
     query = model_class.select(*select_fields)
     for key, value in where.items():
         query = query.where(getattr(model_class, key) == value)
     return query
-
-
-# 使用通用函数操作 User 模型类
-class User(Model):
-    name = CharField()
-    email = CharField(unique=True)
-    password = CharField()
-
-    class Meta:
-        database = db
-        table_name = "users"
-
-
-# 插入数据
-user_id = create_record(User, name="Alice", email="alice@example.com", password="password")
-
-# 查询数据
-users = get_records(User, User.id, User.name, User.email, User.password, name="Alice")
-for user in users:
-    print(user.id, user.name, user.email, user.password)
-
-# 更新数据
-updated = update_record(User, user_id, name="Bob", password="new_password")
-print(updated)
-
-# 删除数据
-deleted = delete_record(User, user_id)
-print(deleted)
```

## sj_tool/fjsp/entity/job.py

```diff
@@ -1,18 +1,20 @@
 import pandas as pd
 
 
 class BaseJob(object):
-    def __init__(self, job_id: str, MAD: str, STD: str, demand: float):
+    def __init__(self, job_id: str, product_code, arrival_time: str, ots_time: str, demand: float):
         """
 
         :param job_id:
-        :param MAD:
-        :param STD:
-        :param demand:
+        :param product_code: 产品编码
+        :param arrival_time: job到达时间，即最早可开始时间
+        :param ots_time: 截止时间
+        :param demand: 需求量
         """
         self.id = job_id
-        self.MAD = pd.to_datetime(MAD)
-        self.STD = pd.to_datetime(STD)
+        self.product_code = product_code
+        self.arrival_time = pd.to_datetime(arrival_time)
+        self.ots_time = pd.to_datetime(ots_time)
         self.demand = demand
         self.start_operations = []
         self.operations = []
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## sj_tool/fjsp/entity/product.py

```diff
@@ -1,3 +1,4 @@
 class Product(object):
-    def __init__(self, idx):
+    def __init__(self, idx, name):
         self.id = idx
+        self.name = name
```

## sj_tool/logger/text_logger.py

```diff
@@ -35,17 +35,17 @@
     CRITICAL = "CRITICAL"
 
 
 def init(level: str, filepath=None, max_filesize=None, replace=False) -> loguru.logger:
     """
     初始化日志框架
     :param level: 最低的日志level，如LogLevel.INFO
-    :param filepath:
-    :param max_filesize:
-    :param replace:
+    :param filepath: 日志文件路径
+    :param max_filesize: 最大文件大小
+    :param replace: 是否替换已有文件（如果文件存在）
     :return:
     """
     logger.remove()
     logger.add(sys.stdout, level=level)
     if filepath is not None:
         if replace:
             os.remove(filepath)
```

## sj_tool/logger/visual_logger.py

```diff
@@ -1,37 +1,37 @@
 import wave
 import numpy as np
 
-from typing import Optional, List
+from typing import List, Union
 from visualdl import LogWriter
 from tensorboardX import SummaryWriter
 
 
 class VisualLogger(object):
     def __init__(self, logdir, use_visualdl=True):
         self.writer = LogWriter(logdir) if use_visualdl else SummaryWriter(logdir)
 
-    def add_scalar(self, tag: str, value: Optional[str, int, float], step: int):
+    def add_scalar(self, tag: str, value: Union[str, int, float], step: int):
         self.writer.add_scalar(tag, value, step)
 
     def add_image(self, tag: str, img: np.ndarray, step: int):
         self.writer.add_image(tag=tag, img=img, step=step)
 
     def add_audio(self, tag: str, audio_path: str, step: int):
         _, audio_data = self._read_audio_data(audio_path)
         self.writer.add_audio(tag=tag, audio_array=audio_data, step=step, sample_rate=8000)
 
-    def add_histogram(self, tag: str, values: Optional[np.ndarray, List], step: int):
+    def add_histogram(self, tag: str, values: Union[np.ndarray, List], step: int):
         self.writer.add_histogram(tag=tag, values=values, step=step, buckets=10)
 
     def add_pr_curve(
         self,
         tag: str,
-        labels: Optional[np.ndarray, List],
-        predictions: Optional[np.ndarray, List],
+        labels: Union[np.ndarray, List],
+        predictions: Union[np.ndarray, List],
         step: int,
         num_thresholds,
     ):
         self.writer.add_pr_curve(
             tag=tag, labels=labels, predictions=predictions, step=step, num_thresholds=num_thresholds
         )
```

## Comparing `sj_tool-1.0.2.dist-info/RECORD` & `sj_tool-1.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 sj_tool/email_sender.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/file.py,sha256=NsbZm_9UGni8CKoZEL9mMFwX7u2R2DXA-HtuUS1iaPw,155
 sj_tool/json.py,sha256=yG7paERY6nUtF51kz5ZXp396TKT-UgIyb0teAXeKD5Q,313
 sj_tool/scheduler.py,sha256=dZJdlvgWuDurNro3ZZ1dgA6qqoqCLSGFzPekS0Tkkx0,1710
 sj_tool/system.py,sha256=xQxxnAKZ8yW8LJZlw0MhpRyQ_p1LnqwlKnuwgiFdqgI,245
 sj_tool/util.py,sha256=cFqbYbJ_NzqG2OeEF8IFrV7wjsDcULZmOa7UgatZF84,597
 sj_tool/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/db/mongo.py,sha256=nV5lx0JndkhVfIJKb2TPkWFxKon8d_mtQhTRDuiWs-g,5667
-sj_tool/db/mysql.py,sha256=BQ2SSoUej6qCHthE6i1UvViOZqWYxnuT06RXxjDKEno,2035
+sj_tool/db/mongo.py,sha256=oUDrhYV_sOq8M9KNFK_QDExCWQ070T1nksp8XzGtDs4,5626
+sj_tool/db/mysql.py,sha256=o9tidq_q9TkDbJXUb6KTMf9O9cJMZeL3rCsADCmroBQ,1237
 sj_tool/fjsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/fjsp/entity/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/fjsp/entity/job.py,sha256=43WfIwh1xFQeaZcf0dTJCnl2UMt5xoDVeIKX7Hm8q1U,442
+sj_tool/fjsp/entity/changeover.py,sha256=LKGrTW1pppF8zEP6fOXBYYmUa2hjtkpoN73OkGI65p0,463
+sj_tool/fjsp/entity/job.py,sha256=v3Co8jowTkjtDihATSsScKFjl9vwXxqKxuMIzm9M6-g,663
 sj_tool/fjsp/entity/machine.py,sha256=F0IDbnE-Jp5h6EaTmZ19PIOxLDtZIvtPyUgC3-nFDK0,374
 sj_tool/fjsp/entity/operation.py,sha256=JL3pza2IeJIvGwru5ieWSdwvN8DWHGR7XIr1TW2gPdQ,617
-sj_tool/fjsp/entity/product.py,sha256=JLiw5pWGzR7vqU9HtneTjaqB1sbmoQzzs4YMGOwhjes,77
+sj_tool/fjsp/entity/product.py,sha256=YTYKXvDH0D6AkOhyONP47POeOidHzSLgLmiXWNXnR6k,109
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/logger/text_logger.py,sha256=RutgGq2e0ZCX7I9f6cNLDeDYryZij7feaXgWy-6JWGA,1779
-sj_tool/logger/visual_logger.py,sha256=1LT4eUg_sgxnDlW1kcNvzhCOeng16AoJsyVDEI_ZzPg,2077
-sj_tool-1.0.2.dist-info/METADATA,sha256=o0EI_ym90K3Lo0P0VCOp6-8LccCrJJLU9QP1T-pomj8,468
-sj_tool-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.2.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.2.dist-info/RECORD,,
+sj_tool/logger/text_logger.py,sha256=hNPAxGVOsL46q-9cd-o-S7WV3CL52vlhD7HWKRAeh2Y,1866
+sj_tool/logger/visual_logger.py,sha256=7X73d7-xHmG2JDiUtFWRVBiNXb8mp91T4nX_sBB1wbc,2062
+sj_tool-1.0.4.dist-info/METADATA,sha256=WP9CsV4Q-NFUlq-1MsUMjqIbGM31MP0yCoF4Ff-E7Bk,492
+sj_tool-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.4.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.4.dist-info/RECORD,,
```

