# Comparing `tmp/keyrock-encryption-2023.4.8.1838.tar.gz` & `tmp/keyrock-encryption-2023.4.8.1854.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-encryption-2023.4.8.1838.tar", last modified: Sat Apr  8 18:38:26 2023, max compression
+gzip compressed data, was "keyrock-encryption-2023.4.8.1854.tar", last modified: Sat Apr  8 18:54:09 2023, max compression
```

## Comparing `keyrock-encryption-2023.4.8.1838.tar` & `keyrock-encryption-2023.4.8.1854.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.251128 keyrock-encryption-2023.4.8.1838/keyrock_encryption/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/encryption.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/test_encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.253128 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-08 18:38:26.255128 keyrock-encryption-2023.4.8.1838/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.665588 keyrock-encryption-2023.4.8.1854/keyrock_encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.668588 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/test_encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:54:09.667588 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-08 18:54:09.000000 keyrock-encryption-2023.4.8.1854/keyrock_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:53:52.000000 keyrock-encryption-2023.4.8.1854/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-08 18:54:09.669588 keyrock-encryption-2023.4.8.1854/setup.cfg
```

### Comparing `keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/encryption.py` & `keyrock-encryption-2023.4.8.1854/keyrock_encryption/encryption/encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import base64
 import hashlib
 import json
 import re
 import string
 import random
 
-from Crypto import Random
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import pad, unpad
+try:
+    from Crypto import Random
+    from Crypto.Cipher import AES
+    from Crypto.Util.Padding import pad, unpad
+except:
+    pass
 
 from keyrock_core import json_util
 
 
 class AESCipher(object):
     def __init__(self, key):
         self.bs = AES.block_size
```

