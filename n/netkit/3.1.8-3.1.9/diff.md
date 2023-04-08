# Comparing `tmp/netkit-3.1.8.tar.gz` & `tmp/netkit-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netkit-3.1.8.tar", last modified: Fri May 22 02:37:57 2020, max compression
+gzip compressed data, was "dist/netkit-3.1.9.tar", last modified: Fri Jul  3 13:23:13 2020, max compression
```

## Comparing `netkit-3.1.8.tar` & `netkit-3.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-22 02:37:57.000000 netkit-3.1.8/
--rw-r--r--   0 dantezhu   (501) staff       (20)      262 2020-05-22 02:37:57.000000 netkit-3.1.8/PKG-INFO
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit/
--rw-r--r--   0 dantezhu   (501) staff       (20)       22 2020-05-22 02:28:56.000000 netkit-3.1.8/netkit/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     5761 2020-05-15 08:35:05.000000 netkit-3.1.8/netkit/box.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit/contrib/
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:35:08.000000 netkit-3.1.8/netkit/contrib/__init__.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     2818 2020-05-22 02:28:29.000000 netkit-3.1.8/netkit/contrib/tcp_client.py
--rw-r--r--   0 dantezhu   (501) staff       (20)       54 2019-08-14 03:35:08.000000 netkit-3.1.8/netkit/log.py
--rw-r--r--   0 dantezhu   (501) staff       (20)    13763 2020-05-06 03:53:14.000000 netkit-3.1.8/netkit/stream.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      427 2019-08-14 03:46:18.000000 netkit-3.1.8/netkit/utils.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      262 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      264 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        7 2020-05-22 02:37:57.000000 netkit-3.1.8/netkit.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-05-22 02:37:57.000000 netkit-3.1.8/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      413 2020-05-22 02:28:56.000000 netkit-3.1.8/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-03 13:23:13.000000 netkit-3.1.9/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      262 2020-07-03 13:23:13.000000 netkit-3.1.9/PKG-INFO
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-03 13:23:13.000000 netkit-3.1.9/netkit/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       22 2020-07-03 13:22:56.000000 netkit-3.1.9/netkit/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     6038 2020-07-03 13:22:30.000000 netkit-3.1.9/netkit/box.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-03 13:23:13.000000 netkit-3.1.9/netkit/contrib/
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2019-08-14 03:35:08.000000 netkit-3.1.9/netkit/contrib/__init__.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     2818 2020-05-22 02:28:29.000000 netkit-3.1.9/netkit/contrib/tcp_client.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)       54 2019-08-14 03:35:08.000000 netkit-3.1.9/netkit/log.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)    13763 2020-05-06 03:53:14.000000 netkit-3.1.9/netkit/stream.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      427 2019-08-14 03:46:18.000000 netkit-3.1.9/netkit/utils.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2020-07-03 13:23:13.000000 netkit-3.1.9/netkit.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      262 2020-07-03 13:23:12.000000 netkit-3.1.9/netkit.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      264 2020-07-03 13:23:12.000000 netkit-3.1.9/netkit.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2020-07-03 13:23:12.000000 netkit-3.1.9/netkit.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        7 2020-07-03 13:23:12.000000 netkit-3.1.9/netkit.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       38 2020-07-03 13:23:13.000000 netkit-3.1.9/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      413 2020-07-03 13:22:55.000000 netkit-3.1.9/setup.py
```

### Comparing `netkit-3.1.8/netkit/box.py` & `netkit-3.1.9/netkit/box.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,38 +26,51 @@
     """
 
     # 继承时可修改
     header_attrs = HEADER_ATTRS
     # 网络字节序. 继承时可修改
     header_fmt_type = '!'
 
-    header_fmt = None
-    header_len = None
+    _header_fmt = None
+    _header_len = None
 
     # 如果调用unpack成功的话，会置为True
     unpack_done = None
 
     # 仅支持bytes类型
     _body = None
 
     def __init__(self, init_data=None):
-        self.header_fmt = self.header_fmt_type + ''.join(value[0] for value in self.header_attrs.values())
-        self.header_len = struct.calcsize(self.header_fmt)
-
         self.unpack_done = False
 
         for k, v in self.header_attrs.items():
             setattr(self, k, v[1])
         self.body = b''
 
         if init_data and isinstance(init_data, dict):
             for k, v in init_data.items():
                 setattr(self, k, v)
 
     @property
+    def header_fmt(self):
+        cls = type(self)
+        if cls._header_fmt is None:
+            cls._header_fmt = self.header_fmt_type + ''.join(value[0] for value in self.header_attrs.values())
+
+        return cls._header_fmt
+
+    @property
+    def header_len(self):
+        cls = type(self)
+        if cls._header_len is None:
+            cls._header_len = struct.calcsize(self.header_fmt)
+
+        return cls._header_len
+
+    @property
     def body(self):
         return self._body
 
     @body.setter
     def body(self, value):
         """
         如果传入的不是bytes类型，就强制转换成bytes类型
```

### Comparing `netkit-3.1.8/netkit/contrib/tcp_client.py` & `netkit-3.1.9/netkit/contrib/tcp_client.py`

 * *Files identical despite different names*

### Comparing `netkit-3.1.8/netkit/stream.py` & `netkit-3.1.9/netkit/stream.py`

 * *Files identical despite different names*

