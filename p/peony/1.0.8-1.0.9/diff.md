# Comparing `tmp/peony-1.0.8.tar.gz` & `tmp/peony-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/peony-1.0.8.tar", last modified: Wed May 20 02:25:10 2020, max compression
+gzip compressed data, was "dist/peony-1.0.9.tar", last modified: Wed May 20 02:39:11 2020, max compression
```

## Comparing `peony-1.0.8.tar` & `peony-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/
--rw-r--r--   0 dantezhu   (501) staff       (20)      229 2020-05-20 02:25:10.000000 peony-1.0.8/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)     1017 2020-05-19 06:54:11.000000 peony-1.0.8/README.md
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/
--rw-r--r--   0 dantezhu   (501) staff       (20)      157 2020-05-20 02:24:47.000000 peony-1.0.8/peony/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/bin/
--rwxr-xr-x   0 dantezhu   (501) staff       (20)     7424 2020-05-19 11:31:22.000000 peony-1.0.8/peony/bin/peonyctl
--rw-r--r--   0 dantezhu   (501) staff       (20)      564 2020-03-11 12:42:33.000000 peony-1.0.8/peony/blueprint.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/master/
--rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 peony-1.0.8/peony/master/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     4990 2020-05-20 01:56:17.000000 peony-1.0.8/peony/master/master.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2409 2020-05-20 01:56:17.000000 peony-1.0.8/peony/master/task_queue_manager.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3180 2020-05-20 01:44:26.000000 peony-1.0.8/peony/peony.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/proxy/
--rw-r--r--   0 dantezhu   (501) staff       (20)       26 2019-08-14 03:31:53.000000 peony-1.0.8/peony/proxy/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/proxy/connection/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:53.000000 peony-1.0.8/peony/proxy/connection/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3738 2020-05-19 11:31:09.000000 peony-1.0.8/peony/proxy/connection/admin_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3966 2020-05-20 01:45:07.000000 peony-1.0.8/peony/proxy/connection/client_tcp_connection.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2758 2020-05-19 08:33:30.000000 peony-1.0.8/peony/proxy/proxy.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      654 2020-05-19 11:31:26.000000 peony-1.0.8/peony/proxy/stat_counter.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/share/
--rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 peony-1.0.8/peony/share/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7822 2019-08-14 03:38:47.000000 peony-1.0.8/peony/share/config.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1438 2020-05-20 01:56:36.000000 peony-1.0.8/peony/share/constants.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       84 2020-05-19 02:23:53.000000 peony-1.0.8/peony/share/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     3437 2020-05-19 07:50:35.000000 peony-1.0.8/peony/share/mixins.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     1381 2020-05-19 08:28:56.000000 peony-1.0.8/peony/share/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony/worker/
--rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 peony-1.0.8/peony/worker/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2375 2020-05-19 08:52:22.000000 peony-1.0.8/peony/worker/request.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7814 2020-05-19 09:33:40.000000 peony-1.0.8/peony/worker/worker.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      229 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      748 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-05-18 09:25:59.000000 peony-1.0.8/peony.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       54 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        6 2020-05-20 02:25:10.000000 peony-1.0.8/peony.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-05-20 02:25:10.000000 peony-1.0.8/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      511 2020-05-20 02:24:50.000000 peony-1.0.8/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      229 2020-05-20 02:39:11.000000 peony-1.0.9/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1017 2020-05-19 06:54:11.000000 peony-1.0.9/README.md
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      157 2020-05-20 02:38:38.000000 peony-1.0.9/peony/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/bin/
+-rwxr-xr-x   0 dantezhu   (501) staff       (20)     7424 2020-05-19 11:31:22.000000 peony-1.0.9/peony/bin/peonyctl
+-rw-r--r--   0 dantezhu   (501) staff       (20)      564 2020-03-11 12:42:33.000000 peony-1.0.9/peony/blueprint.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/master/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 peony-1.0.9/peony/master/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     4964 2020-05-20 02:35:50.000000 peony-1.0.9/peony/master/master.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2409 2020-05-20 01:56:17.000000 peony-1.0.9/peony/master/task_queue_manager.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3180 2020-05-20 01:44:26.000000 peony-1.0.9/peony/peony.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/proxy/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       26 2019-08-14 03:31:53.000000 peony-1.0.9/peony/proxy/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/proxy/connection/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:31:53.000000 peony-1.0.9/peony/proxy/connection/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3684 2020-05-20 02:35:27.000000 peony-1.0.9/peony/proxy/connection/admin_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3790 2020-05-20 02:35:22.000000 peony-1.0.9/peony/proxy/connection/client_tcp_connection.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2758 2020-05-19 08:33:30.000000 peony-1.0.9/peony/proxy/proxy.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      654 2020-05-19 11:31:26.000000 peony-1.0.9/peony/proxy/stat_counter.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/share/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        0 2019-01-04 14:57:08.000000 peony-1.0.9/peony/share/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7822 2019-08-14 03:38:47.000000 peony-1.0.9/peony/share/config.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1438 2020-05-20 01:56:36.000000 peony-1.0.9/peony/share/constants.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       84 2020-05-19 02:23:53.000000 peony-1.0.9/peony/share/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     3437 2020-05-19 07:50:35.000000 peony-1.0.9/peony/share/mixins.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     1381 2020-05-19 08:28:56.000000 peony-1.0.9/peony/share/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony/worker/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       27 2020-03-11 13:04:31.000000 peony-1.0.9/peony/worker/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2375 2020-05-19 08:52:22.000000 peony-1.0.9/peony/worker/request.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7814 2020-05-19 09:33:40.000000 peony-1.0.9/peony/worker/worker.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      229 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      748 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-05-18 09:25:59.000000 peony-1.0.9/peony.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       54 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        6 2020-05-20 02:39:11.000000 peony-1.0.9/peony.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-05-20 02:39:11.000000 peony-1.0.9/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      511 2020-05-20 02:38:34.000000 peony-1.0.9/setup.py
```

### Comparing `peony-1.0.8/README.md` & `peony-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/bin/peonyctl` & `peony-1.0.9/peony/bin/peonyctl`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/blueprint.py` & `peony-1.0.9/peony/blueprint.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/master/master.py` & `peony-1.0.9/peony/master/master.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,13 @@
             """
             self.stop_all()
 
         # INT为强制结束
         signal.signal(signal.SIGINT, stop_handler)
         # TERM为安全结束
         signal.signal(signal.SIGTERM, stop_handler)
-        # HUP为热更新
         signal.signal(signal.SIGHUP, signal.SIG_IGN)
 
     def __repr__(self):
         return '<%s name: %s>' % (
             type(self).__name__, self.app.name
         )
```

### Comparing `peony-1.0.8/peony/master/task_queue_manager.py` & `peony-1.0.9/peony/master/task_queue_manager.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/peony.py` & `peony-1.0.9/peony/peony.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/proxy/connection/admin_connection.py` & `peony-1.0.9/peony/proxy/connection/admin_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,14 @@
     def buildProtocol(self, addr):
         return AdminConnection(self, addr)
 
 
 class AdminConnection(Protocol):
     _read_buffer = None
 
-    # 客户端IP的数字
-    _client_ip_num = None
-
     def __init__(self, factory, address):
         self.factory = factory
         self.address = address
         self._read_buffer = b''
 
     def dataReceived(self, data):
         """
```

### Comparing `peony-1.0.8/peony/proxy/connection/client_tcp_connection.py` & `peony-1.0.9/peony/proxy/connection/client_tcp_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,36 +15,28 @@
     def buildProtocol(self, addr):
         return ClientConnection(self, addr)
 
 
 class ClientConnection(Protocol):
     _read_buffer = None
 
-    # 客户端IP的数字
-    _client_ip_num = None
-
-    # 客户端IP是否IPV6
-    _ipv6 = None
-
     # 过期timer
     _expire_timer = None
 
     def __init__(self, factory, address):
         # address: IPv4Address
         self.factory = factory
         self.address = address
         self._read_buffer = b''
 
     def connectionMade(self):
         self.transport.setTcpNoDelay(True)
 
         self.factory.proxy.stat_counter.clients += 1
 
-        self._client_ip_num, self._ipv6 = ip_str_to_bin(self.address.host)
-
         self._set_expire_callback()
 
     def connectionLost(self, reason=connectionDone):
         self._clear_expire_callback()
 
         self.factory.proxy.stat_counter.clients -= 1
```

### Comparing `peony-1.0.8/peony/proxy/proxy.py` & `peony-1.0.9/peony/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/proxy/stat_counter.py` & `peony-1.0.9/peony/proxy/stat_counter.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/share/config.py` & `peony-1.0.9/peony/share/config.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/share/constants.py` & `peony-1.0.9/peony/share/constants.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/share/mixins.py` & `peony-1.0.9/peony/share/mixins.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/share/utils.py` & `peony-1.0.9/peony/share/utils.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/worker/request.py` & `peony-1.0.9/peony/worker/request.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony/worker/worker.py` & `peony-1.0.9/peony/worker/worker.py`

 * *Files identical despite different names*

### Comparing `peony-1.0.8/peony.egg-info/SOURCES.txt` & `peony-1.0.9/peony.egg-info/SOURCES.txt`

 * *Files identical despite different names*

