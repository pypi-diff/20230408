# Comparing `tmp/RP-DataBase-1.1.0.tar.gz` & `tmp/RP-DataBase-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RP-DataBase-1.1.0.tar", last modified: Sat Apr  8 16:33:57 2023, max compression
+gzip compressed data, was "RP-DataBase-1.1.1.tar", last modified: Sat Apr  8 16:45:45 2023, max compression
```

## Comparing `RP-DataBase-1.1.0.tar` & `RP-DataBase-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/
--rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/PKG-INFO
-drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/RPDB/
--rw-r--r--   0 hsn       (1000) hsn       (1000)        0 2023-04-08 15:24:42.000000 RP-DataBase-1.1.0/RPDB/__init__.py
--rw-r--r--   0 hsn       (1000) hsn       (1000)     9750 2023-04-08 16:26:05.000000 RP-DataBase-1.1.0/RPDB/database.py
-drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/RP_DataBase.egg-info/
--rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/PKG-INFO
--rw-r--r--   0 hsn       (1000) hsn       (1000)      182 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/SOURCES.txt
--rw-r--r--   0 hsn       (1000) hsn       (1000)        1 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/dependency_links.txt
--rw-r--r--   0 hsn       (1000) hsn       (1000)        5 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/top_level.txt
--rw-r--r--   0 hsn       (1000) hsn       (1000)       38 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/setup.cfg
--rw-r--r--   0 hsn       (1000) hsn       (1000)      269 2023-04-08 16:33:31.000000 RP-DataBase-1.1.0/setup.py
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:45:45.956950 RP-DataBase-1.1.1/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:45:45.956950 RP-DataBase-1.1.1/PKG-INFO
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:45:45.956950 RP-DataBase-1.1.1/RPDB/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        0 2023-04-08 15:24:42.000000 RP-DataBase-1.1.1/RPDB/__init__.py
+-rw-r--r--   0 hsn       (1000) hsn       (1000)     9791 2023-04-08 16:45:43.000000 RP-DataBase-1.1.1/RPDB/database.py
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:45:45.956950 RP-DataBase-1.1.1/RP_DataBase.egg-info/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:45:45.000000 RP-DataBase-1.1.1/RP_DataBase.egg-info/PKG-INFO
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      182 2023-04-08 16:45:45.000000 RP-DataBase-1.1.1/RP_DataBase.egg-info/SOURCES.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        1 2023-04-08 16:45:45.000000 RP-DataBase-1.1.1/RP_DataBase.egg-info/dependency_links.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        5 2023-04-08 16:45:45.000000 RP-DataBase-1.1.1/RP_DataBase.egg-info/top_level.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)       38 2023-04-08 16:45:45.956950 RP-DataBase-1.1.1/setup.cfg
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      269 2023-04-08 16:45:43.000000 RP-DataBase-1.1.1/setup.py
```

### Comparing `RP-DataBase-1.1.0/RPDB/database.py` & `RP-DataBase-1.1.1/RPDB/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,16 +240,19 @@
         if os.path.exists(os.path.join(self.path, 'slices', self.get_key_hash(key))):
             os.remove(os.path.join(self.path, 'slices', self.get_key_hash(key)))
 
             self.keys.remove(key)
         self.lock.release()
 
     def close(self):
-        self.lock.acquire()
         self.already_dump = True
+        self.dump()
+
+    def dump(self):
+        self.lock.acquire()
         with open(os.path.join(self.path, 'all.keys'), 'w', encoding='utf8') as f:
             json.dump({'keys': list(self.keys)}, f)
         with open(os.path.join(self.path, 'meta.json'), 'w', encoding='utf8') as f:
             json.dump(self.meta, f)
         self.lock.release()
 
     def __del__(self):
```

