# Comparing `tmp/keyrock-encryption-2022.12.26.2203.tar.gz` & `tmp/keyrock-encryption-2023.4.8.1838.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-encryption-2022.12.26.2203.tar", last modified: Mon Dec 26 22:03:42 2022, max compression
+gzip compressed data, was "keyrock-encryption-2023.4.8.1838.tar", last modified: Sat Apr  8 18:38:26 2023, max compression
```

## Comparing `keyrock-encryption-2022.12.26.2203.tar` & `keyrock-encryption-2023.4.8.1838.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 22:03:42.226085 keyrock-encryption-2022.12.26.2203/
--rw-r--r--   0 root         (0) root         (0)       72 2022-12-26 22:03:42.226085 keyrock-encryption-2022.12.26.2203/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 22:03:42.222425 keyrock-encryption-2022.12.26.2203/keyrock_encryption/
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-12-26 22:03:27.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 22:03:42.226085 keyrock-encryption-2022.12.26.2203/keyrock_encryption/encryption/
--rw-rw-rw-   0 root         (0) root         (0)       25 2022-12-26 22:03:27.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption/encryption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-12-26 22:03:27.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption/encryption/encryption.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-26 22:03:27.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption/encryption/test_encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 22:03:42.225170 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/
--rw-r--r--   0 root         (0) root         (0)       72 2022-12-26 22:03:42.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2022-12-26 22:03:42.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 22:03:42.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-12-26 22:03:42.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-26 22:03:42.000000 keyrock-encryption-2022.12.26.2203/keyrock_encryption.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-12-26 22:03:27.000000 keyrock-encryption-2022.12.26.2203/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      182 2022-12-26 22:03:42.227000 keyrock-encryption-2022.12.26.2203/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.251128 keyrock-encryption-2023.4.8.1838/keyrock_encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.254128 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/test_encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 18:38:26.253128 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-08 18:38:26.000000 keyrock-encryption-2023.4.8.1838/keyrock_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-08 18:38:10.000000 keyrock-encryption-2023.4.8.1838/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-08 18:38:26.255128 keyrock-encryption-2023.4.8.1838/setup.cfg
```

### Comparing `keyrock-encryption-2022.12.26.2203/keyrock_encryption/encryption/encryption.py` & `keyrock-encryption-2023.4.8.1838/keyrock_encryption/encryption/encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import base64
 import hashlib
 import json
 import re
 import string
 import random
 
-try:
-    from Crypto import Random
-    from Crypto.Cipher import AES
-    from Crypto.Util.Padding import pad, unpad
-except:
-    pass
+from Crypto import Random
+from Crypto.Cipher import AES
+from Crypto.Util.Padding import pad, unpad
 
 from keyrock_core import json_util
 
 
 class AESCipher(object):
     def __init__(self, key):
         self.bs = AES.block_size
```

