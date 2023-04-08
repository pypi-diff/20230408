# Comparing `tmp/burst-3.1.7.tar.gz` & `tmp/burst-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/burst-3.1.7.tar", last modified: Tue Nov 12 11:38:26 2019, max compression
+gzip compressed data, was "dist/burst-3.1.9.tar", last modified: Sat Nov 23 03:47:40 2019, max compression
```

## Comparing `burst-3.1.7.tar` & `burst-3.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/
--rw-r--r--   0 dantezhu   (501) staff       (20)      259 2019-11-12 11:38:26.000000 burst-3.1.7/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)     5488 2018-05-16 13:12:11.000000 burst-3.1.7/README.md
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/
--rw-r--r--   0 dantezhu   (501) staff       (20)      157 2019-11-12 11:38:05.000000 burst-3.1.7/burst/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)    11639 2019-08-14 03:36:51.000000 burst-3.1.7/burst/bin/burstctl
--rw-r--r--   0 dantezhu   (501) staff       (20)      564 2019-08-14 03:31:53.000000 burst-3.1.7/burst/blueprint.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4139 2019-08-14 03:31:53.000000 burst-3.1.7/burst/burst.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/master/
--rw-r--r--   0 dantezhu   (501) staff       (20)       28 2019-08-14 03:31:53.000000 burst-3.1.7/burst/master/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)    10917 2019-11-12 11:36:59.000000 burst-3.1.7/burst/master/master.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/proxy/
--rw-r--r--   0 dantezhu   (501) staff       (20)       26 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/proxy/connection/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     5682 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/admin_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4408 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/client_tcp_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2687 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/client_udp_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      788 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/master_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4675 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/connection/worker_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1669 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/group_queue.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     5404 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/proxy.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2390 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/reload_helper.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1486 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/stat_counter.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      405 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/task_container.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7253 2019-08-14 03:31:53.000000 burst-3.1.7/burst/proxy/task_dispatcher.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/share/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:54.000000 burst-3.1.7/burst/share/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7763 2019-08-14 03:31:53.000000 burst-3.1.7/burst/share/config.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3378 2019-08-14 03:31:53.000000 burst-3.1.7/burst/share/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       85 2019-08-14 03:31:53.000000 burst-3.1.7/burst/share/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4389 2019-08-14 03:31:54.000000 burst-3.1.7/burst/share/mixins.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1218 2019-08-14 03:31:54.000000 burst-3.1.7/burst/share/task.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1212 2019-08-14 03:31:54.000000 burst-3.1.7/burst/share/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst/worker/
--rw-r--r--   0 dantezhu   (501) staff       (20)       28 2019-08-14 03:31:54.000000 burst-3.1.7/burst/worker/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     6754 2019-11-12 11:36:59.000000 burst-3.1.7/burst/worker/connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3608 2019-08-14 03:31:54.000000 burst-3.1.7/burst/worker/request.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2365 2019-11-12 11:36:59.000000 burst-3.1.7/burst/worker/worker.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      259 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)     1013 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-06-20 08:00:46.000000 burst-3.1.7/burst.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       41 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2019-11-12 11:38:26.000000 burst-3.1.7/burst.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2019-11-12 11:38:26.000000 burst-3.1.7/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      529 2019-11-12 11:38:05.000000 burst-3.1.7/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      259 2019-11-23 03:47:40.000000 burst-3.1.9/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)     5488 2018-05-16 13:12:11.000000 burst-3.1.9/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      157 2019-11-23 03:47:19.000000 burst-3.1.9/burst/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)    11639 2019-08-14 03:36:51.000000 burst-3.1.9/burst/bin/burstctl
+-rw-r--r--   0 dantezhu   (501) staff       (20)      564 2019-08-14 03:31:53.000000 burst-3.1.9/burst/blueprint.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4139 2019-08-14 03:31:53.000000 burst-3.1.9/burst/burst.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/master/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       28 2019-08-14 03:31:53.000000 burst-3.1.9/burst/master/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)    10917 2019-11-12 11:36:59.000000 burst-3.1.9/burst/master/master.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/proxy/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       26 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/proxy/connection/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     5682 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/admin_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4408 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/client_tcp_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2687 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/client_udp_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      788 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/master_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4675 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/connection/worker_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1669 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/group_queue.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     5404 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/proxy.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2390 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/reload_helper.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1486 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/stat_counter.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      405 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/task_container.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7253 2019-08-14 03:31:53.000000 burst-3.1.9/burst/proxy/task_dispatcher.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/share/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:54.000000 burst-3.1.9/burst/share/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7763 2019-08-14 03:31:53.000000 burst-3.1.9/burst/share/config.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3378 2019-08-14 03:31:53.000000 burst-3.1.9/burst/share/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       85 2019-08-14 03:31:53.000000 burst-3.1.9/burst/share/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4383 2019-11-23 03:30:16.000000 burst-3.1.9/burst/share/mixins.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1218 2019-08-14 03:31:54.000000 burst-3.1.9/burst/share/task.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1212 2019-08-14 03:31:54.000000 burst-3.1.9/burst/share/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst/worker/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       28 2019-08-14 03:31:54.000000 burst-3.1.9/burst/worker/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6750 2019-11-23 03:30:16.000000 burst-3.1.9/burst/worker/connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3608 2019-08-14 03:31:54.000000 burst-3.1.9/burst/worker/request.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2367 2019-11-23 03:30:16.000000 burst-3.1.9/burst/worker/worker.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      259 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1013 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2016-06-20 08:00:46.000000 burst-3.1.9/burst.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       41 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2019-11-23 03:47:40.000000 burst-3.1.9/burst.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       38 2019-11-23 03:47:40.000000 burst-3.1.9/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      529 2019-11-23 03:47:23.000000 burst-3.1.9/setup.py
```

### Comparing `burst-3.1.7/README.md` & `burst-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/bin/burstctl` & `burst-3.1.9/burst/bin/burstctl`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/blueprint.py` & `burst-3.1.9/burst/blueprint.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/burst.py` & `burst-3.1.9/burst/burst.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/master/master.py` & `burst-3.1.9/burst/master/master.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/connection/admin_connection.py` & `burst-3.1.9/burst/proxy/connection/admin_connection.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/connection/client_tcp_connection.py` & `burst-3.1.9/burst/proxy/connection/client_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/connection/client_udp_connection.py` & `burst-3.1.9/burst/proxy/connection/client_udp_connection.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/connection/master_connection.py` & `burst-3.1.9/burst/proxy/connection/master_connection.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/connection/worker_connection.py` & `burst-3.1.9/burst/proxy/connection/worker_connection.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/group_queue.py` & `burst-3.1.9/burst/proxy/group_queue.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/proxy.py` & `burst-3.1.9/burst/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/reload_helper.py` & `burst-3.1.9/burst/proxy/reload_helper.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/stat_counter.py` & `burst-3.1.9/burst/proxy/stat_counter.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/proxy/task_dispatcher.py` & `burst-3.1.9/burst/proxy/task_dispatcher.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/share/config.py` & `burst-3.1.9/burst/share/config.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/share/constants.py` & `burst-3.1.9/burst/share/constants.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/share/mixins.py` & `burst-3.1.9/burst/share/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 class AppEventsMixin(object):
     events = None
 
     def __init__(self):
         self.events = Events()
 
     @_reg_event_handler
-    def create_worker(self, f):
+    def start_worker(self, f):
         """
         创建worker
         f(worker)
         """
 
     @_reg_event_handler
-    def create_conn(self, f):
+    def open_conn(self, f):
         """
         worker连接建立后
         f(conn)
         """
 
     @_reg_event_handler
     def before_first_request(self, f):
@@ -139,22 +139,22 @@
     def after_request(self, f):
         """
         执行完route对应的view_func后
         f(request, exc)
         """
 
     @_reg_event_handler
-    def create_app_worker(self, f):
+    def start_app_worker(self, f):
         """
         创建worker
         f(worker)
         """
 
     @_reg_event_handler
-    def create_app_conn(self, f):
+    def open_app_conn(self, f):
         """
         worker连接建立后
         f(conn)
         """
 
     @_reg_event_handler
     def before_app_first_request(self, f):
```

### Comparing `burst-3.1.7/burst/share/task.py` & `burst-3.1.9/burst/share/task.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/share/utils.py` & `burst-3.1.9/burst/share/utils.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/worker/connection.py` & `burst-3.1.9/burst/worker/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         try:
             self.client.connect()
         except KeyboardInterrupt as e:
             raise e
         except:
             return False
         else:
-            self.worker.app.events.create_conn(self)
+            self.worker.app.events.open_conn(self)
             for bp in self.worker.app.blueprints:
-                bp.events.create_app_conn(self)
+                bp.events.open_app_conn(self)
 
             return True
 
     def write(self, data):
         """
         发送数据    True: 成功   else: 失败
         """
```

### Comparing `burst-3.1.7/burst/worker/request.py` & `burst-3.1.9/burst/worker/request.py`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/burst/worker/worker.py` & `burst-3.1.9/burst/worker/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def run(self):
         setproctitle.setproctitle(self.app.make_proc_name(
             '%s:%s' % (self.type, self.group_id)
         ))
 
         self._handle_proc_signals()
-        self._on_worker_run()
+        self._on_worker_start()
 
         try:
             address = os.path.join(
                 self.app.config['IPC_ADDRESS_DIRECTORY'],
                 self.app.config['WORKER_ADDRESS_TPL'] % self.group_id
             )
             conn = self.connection_class(self, address, self.app.config['WORKER_CONN_TIMEOUT'])
@@ -48,18 +48,18 @@
         except KeyboardInterrupt:
             pass
         except:
             logger.error('exc occur. worker: %s', self, exc_info=True)
         finally:
             self._on_worker_stop()
 
-    def _on_worker_run(self):
-        self.app.events.create_worker(self)
+    def _on_worker_start(self):
+        self.app.events.start_worker(self)
         for bp in self.app.blueprints:
-            bp.events.create_app_worker(self)
+            bp.events.start_app_worker(self)
 
     def _on_worker_stop(self):
         for bp in self.app.blueprints:
             bp.events.stop_app_worker(self)
         self.app.events.stop_worker(self)
 
     def _handle_proc_signals(self):
```

### Comparing `burst-3.1.7/burst.egg-info/SOURCES.txt` & `burst-3.1.9/burst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burst-3.1.7/setup.py` & `burst-3.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='burst',
-    version='3.1.7',
+    version='3.1.9',
     zip_safe=False,
     platforms='any',
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
     python_requires='>=3',
     scripts=['burst/bin/burstctl'],
     install_requires=['setproctitle', 'twisted', 'events', 'netkit', 'click'],
     url='https://github.com/dantezhu/burst',
```

