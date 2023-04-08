# Comparing `tmp/cnd_cr-0.1.0-py3-none-any.whl.zip` & `tmp/cnd_cr-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2267 bytes, number of entries: 8
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-07 18:11 cnd_cr/VERSION
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-07 18:12 cnd_cr/__init__.py
--rw-r--r--  2.0 unx      115 b- defN 23-Apr-07 18:11 cnd_cr/__version__.py
--rw-r--r--  2.0 unx      872 b- defN 23-Apr-07 19:07 cnd_cr/cr.py
--rw-r--r--  2.0 unx      715 b- defN 23-Apr-07 19:22 cnd_cr-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 19:22 cnd_cr-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-07 19:22 cnd_cr-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-07 19:22 cnd_cr-0.1.0.dist-info/RECORD
-8 files, 2482 bytes uncompressed, 1259 bytes compressed:  49.3%
+Zip file size: 2263 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-07 22:32 cnd_cr/VERSION
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-07 22:32 cnd_cr/__init__.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-07 22:32 cnd_cr/__version__.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Apr-07 22:32 cnd_cr/cr.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Apr-07 22:32 cnd_cr-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 22:32 cnd_cr-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-07 22:32 cnd_cr-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-07 22:32 cnd_cr-0.1.1.dist-info/RECORD
+8 files, 2482 bytes uncompressed, 1255 bytes compressed:  49.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cnd_cr/__version__.py
 Comment: 
 
 Filename: cnd_cr/cr.py
 Comment: 
 
-Filename: cnd_cr-0.1.0.dist-info/METADATA
+Filename: cnd_cr-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr-0.1.0.dist-info/WHEEL
+Filename: cnd_cr-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr-0.1.0.dist-info/top_level.txt
+Filename: cnd_cr-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr-0.1.0.dist-info/RECORD
+Filename: cnd_cr-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_cr/VERSION

```diff
@@ -1 +1 @@
-0.1.0
+0.1.1
```

## Comparing `cnd_cr-0.1.0.dist-info/METADATA` & `cnd_cr-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Base for vro Custom Resource
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr.git
```

## Comparing `cnd_cr-0.1.0.dist-info/RECORD` & `cnd_cr-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cnd_cr/VERSION,sha256=atlhOkVXmNbZLl9fOQq0uqcFlryGntaxf1zdKyhjXwY,5
+cnd_cr/VERSION,sha256=Ee4juPwvxhnW6rYnettaUnJhBnrAHM_D4RhX9Vvxi80,5
 cnd_cr/__init__.py,sha256=TFHx8kxKAlkz6Ala0RdN_7mSm7MLMx6GM4GGPylqXTA,98
 cnd_cr/__version__.py,sha256=KJGjSObXd-spicJLTQQHF3fnu5KeoQ7teFYiVvbFW8k,115
 cnd_cr/cr.py,sha256=ynDwvWUTeDXcIcJe5PvFkOxwIjeLXyRam767YGo3wCg,872
-cnd_cr-0.1.0.dist-info/METADATA,sha256=eZ8EBiDV3kPpuwc05r17DokYJpHsbhEy5IlpE7hbL_4,715
-cnd_cr-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cnd_cr-0.1.0.dist-info/top_level.txt,sha256=YQ9GqCX4U_2hOIc4pgC3t5ZvSVTwzD2sLjpqwIvKbRY,7
-cnd_cr-0.1.0.dist-info/RECORD,,
+cnd_cr-0.1.1.dist-info/METADATA,sha256=SxG9CWc97Ql0YbUSOkTsGy0tb3ynq40ctuh1KvwKmCI,715
+cnd_cr-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cnd_cr-0.1.1.dist-info/top_level.txt,sha256=YQ9GqCX4U_2hOIc4pgC3t5ZvSVTwzD2sLjpqwIvKbRY,7
+cnd_cr-0.1.1.dist-info/RECORD,,
```

