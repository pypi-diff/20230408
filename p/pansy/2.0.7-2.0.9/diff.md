# Comparing `tmp/pansy-2.0.7.tar.gz` & `tmp/pansy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pansy-2.0.7.tar", last modified: Fri Mar 13 09:22:16 2020, max compression
+gzip compressed data, was "dist/pansy-2.0.9.tar", last modified: Sun Mar 15 16:25:01 2020, max compression
```

## Comparing `pansy-2.0.7.tar` & `pansy-2.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/
--rw-r--r--   0 dantezhu   (501) staff       (20)      227 2020-03-13 09:22:16.000000 pansy-2.0.7/PKG-INFO
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/
--rw-r--r--   0 dantezhu   (501) staff       (20)      147 2020-03-13 09:21:53.000000 pansy-2.0.7/pansy/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      564 2020-03-11 12:42:33.000000 pansy-2.0.7/pansy/blueprint.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/contrib/
--rw-r--r--   0 dantezhu   (501) staff       (20)       44 2020-03-13 08:54:52.000000 pansy-2.0.7/pansy/contrib/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/contrib/token/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-03-13 08:54:52.000000 pansy-2.0.7/pansy/contrib/token/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1666 2020-03-13 08:54:52.000000 pansy-2.0.7/pansy/contrib/token/easy_aes.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2930 2020-03-13 09:19:28.000000 pansy-2.0.7/pansy/contrib/token/token_helper.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/master/
--rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/master/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3516 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/master/master.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3111 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/pansy.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/proto/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-08-14 03:03:00.000000 pansy-2.0.7/pansy/proto/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4658 2019-08-22 04:55:33.000000 pansy-2.0.7/pansy/proto/pansy_pb2.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/share/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 pansy-2.0.7/pansy/share/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7822 2019-08-14 03:38:47.000000 pansy-2.0.7/pansy/share/config.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1078 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/share/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       83 2019-01-04 14:57:08.000000 pansy-2.0.7/pansy/share/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4641 2020-03-11 12:42:33.000000 pansy-2.0.7/pansy/share/mixins.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1367 2019-08-14 03:38:48.000000 pansy-2.0.7/pansy/share/task.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1141 2019-08-14 03:38:48.000000 pansy-2.0.7/pansy/share/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/station/
--rw-r--r--   0 dantezhu   (501) staff       (20)       29 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/station/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2652 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/station/station.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/trigger/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 pansy-2.0.7/pansy/trigger/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4812 2020-03-11 12:42:33.000000 pansy-2.0.7/pansy/trigger/client.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      965 2019-08-14 03:38:49.000000 pansy-2.0.7/pansy/trigger/trigger.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy/worker/
--rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/worker/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3789 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/worker/connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3043 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/worker/request.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     8024 2020-03-11 13:04:31.000000 pansy-2.0.7/pansy/worker/worker.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      227 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      833 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-01-04 15:31:47.000000 pansy-2.0.7/pansy.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       59 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2020-03-13 09:22:16.000000 pansy-2.0.7/pansy.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-03-13 09:22:16.000000 pansy-2.0.7/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      482 2020-03-13 09:21:53.000000 pansy-2.0.7/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      227 2020-03-15 16:25:01.000000 pansy-2.0.9/PKG-INFO
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      147 2020-03-15 16:24:23.000000 pansy-2.0.9/pansy/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      564 2020-03-11 12:42:33.000000 pansy-2.0.9/pansy/blueprint.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/contrib/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       44 2020-03-13 08:54:52.000000 pansy-2.0.9/pansy/contrib/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/contrib/token/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2020-03-13 08:54:52.000000 pansy-2.0.9/pansy/contrib/token/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1666 2020-03-13 08:54:52.000000 pansy-2.0.9/pansy/contrib/token/easy_aes.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2930 2020-03-13 09:19:28.000000 pansy-2.0.9/pansy/contrib/token/token_helper.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/master/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/master/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3516 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/master/master.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3166 2020-03-15 16:24:14.000000 pansy-2.0.9/pansy/pansy.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/proto/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-08-14 03:03:00.000000 pansy-2.0.9/pansy/proto/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4658 2019-08-22 04:55:33.000000 pansy-2.0.9/pansy/proto/pansy_pb2.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/share/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 pansy-2.0.9/pansy/share/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7822 2019-08-14 03:38:47.000000 pansy-2.0.9/pansy/share/config.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1162 2020-03-15 16:24:14.000000 pansy-2.0.9/pansy/share/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       83 2019-01-04 14:57:08.000000 pansy-2.0.9/pansy/share/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4641 2020-03-11 12:42:33.000000 pansy-2.0.9/pansy/share/mixins.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1367 2019-08-14 03:38:48.000000 pansy-2.0.9/pansy/share/task.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1141 2019-08-14 03:38:48.000000 pansy-2.0.9/pansy/share/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/station/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       29 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/station/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2652 2020-03-15 16:24:14.000000 pansy-2.0.9/pansy/station/station.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/trigger/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 pansy-2.0.9/pansy/trigger/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4812 2020-03-11 12:42:33.000000 pansy-2.0.9/pansy/trigger/client.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      965 2019-08-14 03:38:49.000000 pansy-2.0.9/pansy/trigger/trigger.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy/worker/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/worker/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3789 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/worker/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3043 2020-03-11 13:04:31.000000 pansy-2.0.9/pansy/worker/request.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     8083 2020-03-15 16:24:14.000000 pansy-2.0.9/pansy/worker/worker.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-03-15 16:25:01.000000 pansy-2.0.9/pansy.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      227 2020-03-15 16:25:00.000000 pansy-2.0.9/pansy.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      833 2020-03-15 16:25:00.000000 pansy-2.0.9/pansy.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-03-15 16:25:00.000000 pansy-2.0.9/pansy.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-01-04 15:31:47.000000 pansy-2.0.9/pansy.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       59 2020-03-15 16:25:00.000000 pansy-2.0.9/pansy.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2020-03-15 16:25:00.000000 pansy-2.0.9/pansy.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-03-15 16:25:01.000000 pansy-2.0.9/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      482 2020-03-15 16:24:20.000000 pansy-2.0.9/setup.py
```

### Comparing `pansy-2.0.7/pansy/blueprint.py` & `pansy-2.0.9/pansy/blueprint.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/contrib/token/easy_aes.py` & `pansy-2.0.9/pansy/contrib/token/easy_aes.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/contrib/token/token_helper.py` & `pansy-2.0.9/pansy/contrib/token/token_helper.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/master/master.py` & `pansy-2.0.9/pansy/master/master.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/pansy.py` & `pansy-2.0.9/pansy/pansy.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                                    get_converter=import_module_or_string)
     debug = ConfigAttribute('DEBUG')
 
     conn_timeout = ConfigAttribute('CONN_TIMEOUT')
     reconnect_interval = ConfigAttribute('RECONNECT_INTERVAL')
     stop_timeout = ConfigAttribute('STOP_TIMEOUT')
     work_timeout = ConfigAttribute('WORK_TIMEOUT')
+    tasks_max_size = ConfigAttribute('TASKS_MAX_SIZE')
 
     ############################## configurable end   ##############################
 
     config = None
 
     master = None
     blueprints = None
```

### Comparing `pansy-2.0.7/pansy/proto/pansy_pb2.py` & `pansy-2.0.9/pansy/proto/pansy_pb2.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/share/config.py` & `pansy-2.0.9/pansy/share/config.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/share/constants.py` & `pansy-2.0.9/pansy/share/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,8 +42,11 @@
     # 重连等待时间。worker和client都在用
     'RECONNECT_INTERVAL': 1,
 
     'STOP_TIMEOUT': None,
 
     # 处理task超时(秒). 超过后会打印fatal日志. None 代表永不超时
     'WORK_TIMEOUT': None,
+
+    # 等待处理的tasks的最大值。<=0代表无限
+    'TASKS_MAX_SIZE': -1,
 }
```

### Comparing `pansy-2.0.7/pansy/share/mixins.py` & `pansy-2.0.9/pansy/share/mixins.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/share/task.py` & `pansy-2.0.9/pansy/share/task.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/share/utils.py` & `pansy-2.0.9/pansy/share/utils.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/station/station.py` & `pansy-2.0.9/pansy/station/station.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     enabled = True
     got_keyboard_interrupt = False
 
     worker_threads = None
 
     def __init__(self, app, room_id_begin, room_id_end):
         self.app = app
-        self.worker_threads = list()
         self.room_id_begin = room_id_begin
         self.room_id_end = room_id_end
+        self.worker_threads = list()
 
     def run(self):
         setproctitle.setproctitle(self.app.make_proc_name(
             'station:%s-%s' % (self.room_id_begin, self.room_id_end)
         ))
         self._handle_signals()
```

### Comparing `pansy-2.0.7/pansy/trigger/client.py` & `pansy-2.0.9/pansy/trigger/client.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/trigger/trigger.py` & `pansy-2.0.9/pansy/trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/worker/connection.py` & `pansy-2.0.9/pansy/worker/connection.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/worker/request.py` & `pansy-2.0.9/pansy/worker/request.py`

 * *Files identical despite different names*

### Comparing `pansy-2.0.7/pansy/worker/worker.py` & `pansy-2.0.9/pansy/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,19 @@
     # 业务可以通过clock来设置schedule
     clock = None
 
     # 工作进展
     work_progress = None
 
     def __init__(self, station, room_id):
-        self.task_queue = queue.Queue()
         self.station = station
         self.room_id = room_id
 
+        self.task_queue = queue.Queue(self.app.tasks_max_size)
+
         self.conn = self.connection_class(
             self,
             (self.app.host, self.app.port),
             self.app.conn_timeout
         )
 
         self.clock = Clock()
@@ -80,15 +81,15 @@
                 # 说明已经没有了
                 break
             except KeyboardInterrupt:
                 # 原样抛出
                 raise
             except:
                 # 说明出问题了
-                logger.error('exc occur.', exc_info=True)
+                logger.error('exc occur. worker: %s', self, exc_info=True)
                 break
             finally:
                 block = False
 
         for task in task_list:
             if task is None:
                 # 通过传入None来中断block
@@ -183,15 +184,15 @@
             True: 成功
             False: 失败
         """
         try:
             self.task_queue.put_nowait(task)
             return True
         except:
-            logger.error('exc occur. task: %r', task, exc_info=True)
+            logger.error('exc occur. worker: %s, task: %s', self, task, exc_info=True)
             return False
 
     @property
     def app(self):
         return self.station.app
 
     @property
```

### Comparing `pansy-2.0.7/pansy.egg-info/SOURCES.txt` & `pansy-2.0.9/pansy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

