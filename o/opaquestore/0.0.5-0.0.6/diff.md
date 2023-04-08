# Comparing `tmp/opaquestore-0.0.5.tar.gz` & `tmp/opaquestore-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaquestore-0.0.5.tar", last modified: Sun Apr  2 01:34:03 2023, max compression
+gzip compressed data, was "opaquestore-0.0.6.tar", last modified: Sat Apr  8 19:52:59 2023, max compression
```

## Comparing `opaquestore-0.0.5.tar` & `opaquestore-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-02 01:34:03.343090 opaquestore-0.0.5/
--rw-r--r--   0 s         (1000) s         (1000)    35147 2023-03-12 01:33:27.000000 opaquestore-0.0.5/LICENSE
--rw-r--r--   0 s         (1000) s         (1000)       32 2023-03-13 02:12:50.000000 opaquestore-0.0.5/MANIFEST.in
--rw-r--r--   0 s         (1000) s         (1000)     2864 2023-04-02 01:34:03.343090 opaquestore-0.0.5/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)     2355 2023-03-12 19:03:20.000000 opaquestore-0.0.5/README.org
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-02 01:34:03.343090 opaquestore-0.0.5/opaquestore/
--rw-r--r--   0 s         (1000) s         (1000)        1 2023-03-12 18:20:01.000000 opaquestore-0.0.5/opaquestore/__init__.py
--rwxr-xr-x   0 s         (1000) s         (1000)      487 2023-03-12 18:56:42.000000 opaquestore-0.0.5/opaquestore/genkey.py
--rwxr-xr-x   0 s         (1000) s         (1000)     3183 2023-04-02 01:17:05.000000 opaquestore-0.0.5/opaquestore/noiseclient.py
--rwxr-xr-x   0 s         (1000) s         (1000)     5168 2023-04-02 01:16:22.000000 opaquestore-0.0.5/opaquestore/opaquestore.py
--rwxr-xr-x   0 s         (1000) s         (1000)     5741 2023-04-02 01:20:52.000000 opaquestore-0.0.5/opaquestore/server.py
--rwxr-xr-x   0 s         (1000) s         (1000)     2485 2023-04-02 01:18:43.000000 opaquestore-0.0.5/opaquestore/toprf.py
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-02 01:34:03.343090 opaquestore-0.0.5/opaquestore.egg-info/
--rw-r--r--   0 s         (1000) s         (1000)     2864 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)      394 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/SOURCES.txt
--rw-r--r--   0 s         (1000) s         (1000)        1 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/dependency_links.txt
--rw-r--r--   0 s         (1000) s         (1000)       61 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/entry_points.txt
--rw-r--r--   0 s         (1000) s         (1000)       54 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/requires.txt
--rw-r--r--   0 s         (1000) s         (1000)       12 2023-04-02 01:34:03.000000 opaquestore-0.0.5/opaquestore.egg-info/top_level.txt
--rw-r--r--   0 s         (1000) s         (1000)       38 2023-04-02 01:34:03.343090 opaquestore-0.0.5/setup.cfg
--rwxr-xr-x   0 s         (1000) s         (1000)     1441 2023-04-02 01:33:42.000000 opaquestore-0.0.5/setup.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:52:58.999513 opaquestore-0.0.6/
+-rw-r--r--   0 s         (1000) s         (1000)    35147 2023-03-12 01:33:27.000000 opaquestore-0.0.6/LICENSE
+-rw-r--r--   0 s         (1000) s         (1000)       32 2023-03-13 02:12:50.000000 opaquestore-0.0.6/MANIFEST.in
+-rw-r--r--   0 s         (1000) s         (1000)     2864 2023-04-08 19:52:58.999513 opaquestore-0.0.6/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)     2355 2023-03-12 19:03:20.000000 opaquestore-0.0.6/README.org
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:52:58.998513 opaquestore-0.0.6/opaquestore/
+-rw-r--r--   0 s         (1000) s         (1000)        0 2023-04-08 19:49:35.000000 opaquestore-0.0.6/opaquestore/__init__.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     5168 2023-04-08 19:48:55.000000 opaquestore-0.0.6/opaquestore/client.py
+-rwxr-xr-x   0 s         (1000) s         (1000)      487 2023-03-12 18:56:42.000000 opaquestore-0.0.6/opaquestore/genkey.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     3183 2023-04-02 01:17:05.000000 opaquestore-0.0.6/opaquestore/noiseclient.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     5734 2023-04-08 17:10:33.000000 opaquestore-0.0.6/opaquestore/server.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     2485 2023-04-02 01:18:43.000000 opaquestore-0.0.6/opaquestore/toprf.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:52:58.999513 opaquestore-0.0.6/opaquestore.egg-info/
+-rw-r--r--   0 s         (1000) s         (1000)     2864 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)      389 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/SOURCES.txt
+-rw-r--r--   0 s         (1000) s         (1000)        1 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/dependency_links.txt
+-rw-r--r--   0 s         (1000) s         (1000)       56 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/entry_points.txt
+-rw-r--r--   0 s         (1000) s         (1000)       54 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/requires.txt
+-rw-r--r--   0 s         (1000) s         (1000)       12 2023-04-08 19:52:58.000000 opaquestore-0.0.6/opaquestore.egg-info/top_level.txt
+-rw-r--r--   0 s         (1000) s         (1000)       38 2023-04-08 19:52:58.999513 opaquestore-0.0.6/setup.cfg
+-rwxr-xr-x   0 s         (1000) s         (1000)     1436 2023-04-08 19:52:40.000000 opaquestore-0.0.6/setup.py
```

### Comparing `opaquestore-0.0.5/LICENSE` & `opaquestore-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opaquestore-0.0.5/PKG-INFO` & `opaquestore-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaquestore
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Online secret-storage based on the OPAQUE protocol
 Home-page: https://github.com/stef/opaque-store/
 Author: Stefan Marsiske
 Author-email: opaque@ctrlc.hu
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opaquestore-0.0.5/README.org` & `opaquestore-0.0.6/README.org`

 * *Files identical despite different names*

### Comparing `opaquestore-0.0.5/opaquestore/noiseclient.py` & `opaquestore-0.0.6/opaquestore/noiseclient.py`

 * *Files identical despite different names*

### Comparing `opaquestore-0.0.5/opaquestore/opaquestore.py` & `opaquestore-0.0.6/opaquestore/client.py`

 * *Files identical despite different names*

### Comparing `opaquestore-0.0.5/opaquestore/server.py` & `opaquestore-0.0.6/opaquestore/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import socket, sys, os, datetime, os.path, traceback
 import pysodium, opaque
 from dissononce.dh.x25519.keypair import KeyPair
 from dissononce.dh.x25519.public import PublicKey
 from binascii import a2b_base64, b2a_base64
 from klutshnik.utils import getcfg
 from opaquestore import toprf
-from opaquestore.noiseclient import NoiseWrapperServer
+from opaquestore import noiseclient
 
 config = None
 
 CREATE   =b'\x00'
 GET      =b'\x66'
 EXOP     =b'\xE0' # unimplemented
 
@@ -163,15 +163,15 @@
 
             while(len(kids)>config['max_kids']):
                 pid, status = os.waitpid(0,0)
                 kids.remove(pid)
 
             pid=os.fork()
             if pid==0:
-              conn = NoiseWrapperServer(conn, config['noise_key'])
+              conn = noiseclient.NoiseWrapperServer(conn, config['noise_key'])
               try:
                 handler(conn)
               except:
                 print("fail")
                 raise
               finally:
                 try: conn.shutdown(socket.SHUT_RDWR)
```

### Comparing `opaquestore-0.0.5/opaquestore/toprf.py` & `opaquestore-0.0.6/opaquestore/toprf.py`

 * *Files identical despite different names*

### Comparing `opaquestore-0.0.5/opaquestore.egg-info/PKG-INFO` & `opaquestore-0.0.6/opaquestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaquestore
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Online secret-storage based on the OPAQUE protocol
 Home-page: https://github.com/stef/opaque-store/
 Author: Stefan Marsiske
 Author-email: opaque@ctrlc.hu
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opaquestore-0.0.5/setup.py` & `opaquestore-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name = 'opaquestore',
-      version = '0.0.5',
+      version = '0.0.6',
       description = 'Simple Online secret-storage based on the OPAQUE protocol',
       license = "GPLv3",
       author = 'Stefan Marsiske',
       author_email = 'opaque@ctrlc.hu',
       url = 'https://github.com/stef/opaque-store/',
       long_description=read('README.org'),
       long_description_content_type="text/markdown",
@@ -29,11 +29,11 @@
       classifiers = ["Development Status :: 4 - Beta",
                      "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
                      "Topic :: Security :: Cryptography",
                      "Topic :: Security",
                      ],
       entry_points = {
           'console_scripts': [
-              'opaquestore = opaquestore.opaquestore:main'
+              'opaquestore = opaquestore.client:main'
           ],
       },
 )
```

