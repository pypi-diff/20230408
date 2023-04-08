# Comparing `tmp/casambi_bt-0.1.2-py3-none-any.whl.zip` & `tmp/casambi_bt-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27149 bytes, number of entries: 17
+Zip file size: 27151 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      229 b- defN 23-Apr-07 15:31 CasambiBt/__init__.py
 -rw-r--r--  2.0 unx      828 b- defN 23-Feb-21 11:39 CasambiBt/_cache.py
 -rw-r--r--  2.0 unx    15829 b- defN 23-Apr-08 08:34 CasambiBt/_casambi.py
 -rw-r--r--  2.0 unx    17487 b- defN 23-Apr-07 18:55 CasambiBt/_client.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Feb-21 11:37 CasambiBt/_constants.py
 -rw-r--r--  2.0 unx     1144 b- defN 23-Feb-21 11:54 CasambiBt/_discover.py
 -rw-r--r--  2.0 unx     3831 b- defN 23-Apr-07 15:24 CasambiBt/_encryption.py
 -rw-r--r--  2.0 unx     2389 b- defN 23-Apr-07 15:30 CasambiBt/_keystore.py
 -rw-r--r--  2.0 unx    11958 b- defN 23-Apr-08 08:35 CasambiBt/_network.py
--rw-r--r--  2.0 unx      824 b- defN 23-Apr-07 17:08 CasambiBt/_operation.py
+-rw-r--r--  2.0 unx      826 b- defN 23-Apr-08 18:44 CasambiBt/_operation.py
 -rw-r--r--  2.0 unx    13496 b- defN 23-Apr-07 15:31 CasambiBt/_unit.py
 -rw-r--r--  2.0 unx     1551 b- defN 23-Apr-07 15:46 CasambiBt/errors.py
--rw-r--r--  2.0 unx    11341 b- defN 23-Apr-08 09:00 casambi_bt-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2076 b- defN 23-Apr-08 09:00 casambi_bt-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 09:00 casambi_bt-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-08 09:00 casambi_bt-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1339 b- defN 23-Apr-08 09:00 casambi_bt-0.1.2.dist-info/RECORD
-17 files, 84618 bytes uncompressed, 24981 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    11341 b- defN 23-Apr-08 18:47 casambi_bt-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2076 b- defN 23-Apr-08 18:47 casambi_bt-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 18:47 casambi_bt-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-08 18:47 casambi_bt-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1339 b- defN 23-Apr-08 18:47 casambi_bt-0.1.3.dist-info/RECORD
+17 files, 84620 bytes uncompressed, 24983 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: CasambiBt/_unit.py
 Comment: 
 
 Filename: CasambiBt/errors.py
 Comment: 
 
-Filename: casambi_bt-0.1.2.dist-info/LICENSE
+Filename: casambi_bt-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: casambi_bt-0.1.2.dist-info/METADATA
+Filename: casambi_bt-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: casambi_bt-0.1.2.dist-info/WHEEL
+Filename: casambi_bt-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: casambi_bt-0.1.2.dist-info/top_level.txt
+Filename: casambi_bt-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: casambi_bt-0.1.2.dist-info/RECORD
+Filename: casambi_bt-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CasambiBt/_operation.py

```diff
@@ -21,14 +21,14 @@
     def prepareOperation(self, op: OpCode, target: int, payload: bytes) -> bytes:
         if len(payload) > 63:
             raise ValueError("Payload too long")
 
         flags = (self.lifetime & 15) << 11 | len(payload)
 
         # Ensure that origin can't overflow.
-        # TODO: Check that signed is actually correct here.
+        # TODO: Check that unsigned is actually correct here.
         packet = struct.pack(
-            ">hbhhh", flags, op, self.origin & (2**15 - 1), target, 0
+            ">HBHHH", flags, op, self.origin & (2**16 - 1), target, 0
         )
         self.origin += 1
 
         return packet + payload
```

## Comparing `casambi_bt-0.1.2.dist-info/LICENSE` & `casambi_bt-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `casambi_bt-0.1.2.dist-info/METADATA` & `casambi_bt-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casambi-bt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A minimal, unofficial implementation of a bluetooth client for casambi devices
 Home-page: https://github.com/lkempf/casambi-bt
 Author: lkempf
 Author-email: pypi@lukas-kempf.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

## Comparing `casambi_bt-0.1.2.dist-info/RECORD` & `casambi_bt-0.1.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 CasambiBt/_casambi.py,sha256=w0I2KOEOUbvyf8BYuoq-SDNT8W5cOksGE8imFDHCe_s,15829
 CasambiBt/_client.py,sha256=ngmsOEMMgNpry5dn28Mrp2Maq1cYpcTnDIsp1Y9RnPU,17487
 CasambiBt/_constants.py,sha256=r3Egb7xCM5Gq8csnVss4gOlXVvnj0uUS4nqKzbBy1FM,194
 CasambiBt/_discover.py,sha256=v11ucqWHsPOZXjMCrJIaldEsY3BmY3ekVmMnlcuQB4U,1144
 CasambiBt/_encryption.py,sha256=CLcoOOrggQqhJbnr_emBnEnkizpWDvb_0yFnitq4_FM,3831
 CasambiBt/_keystore.py,sha256=OMGf7zjc3U658cnmQ141lTZFROPLnJ3Bwbg51X30SsI,2389
 CasambiBt/_network.py,sha256=AEgFm4SyYU0s6GQx3AWUn33YIKVedn4j46EK1vX1f00,11958
-CasambiBt/_operation.py,sha256=9Wr9c_kHiDc46G5un4KG0HWo5lGdWxiERO1XyxYKaIA,824
+CasambiBt/_operation.py,sha256=P1AdpGjY4FIoGYgcsO6IdRuxQfxaYGGWh94rwj06FnY,826
 CasambiBt/_unit.py,sha256=JB22f3pQh5GIEVksCrcmeFgYjuyjSsYwhG3leQ28R5Q,13496
 CasambiBt/errors.py,sha256=6Kz9JgpIs4FTOYqtHKQc-Cj3ybzRWYaDulqPw0DXL7Y,1551
-casambi_bt-0.1.2.dist-info/LICENSE,sha256=TAIIitFxpxEDi6Iju7foW4TDQmWvC-IhLVLhl67jKmQ,11341
-casambi_bt-0.1.2.dist-info/METADATA,sha256=meL_dtMAPvYsoGMdYVmWSy6PDfdlh4JB2zYijyh6tMA,2076
-casambi_bt-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-casambi_bt-0.1.2.dist-info/top_level.txt,sha256=uNbqLjtecFosoFzpGAC89-5icikWODKI8rOjbi8v_sA,10
-casambi_bt-0.1.2.dist-info/RECORD,,
+casambi_bt-0.1.3.dist-info/LICENSE,sha256=TAIIitFxpxEDi6Iju7foW4TDQmWvC-IhLVLhl67jKmQ,11341
+casambi_bt-0.1.3.dist-info/METADATA,sha256=HIr122fVC2HxqA2z3w41McCFjzi7I3BfDeQ847_aH0o,2076
+casambi_bt-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+casambi_bt-0.1.3.dist-info/top_level.txt,sha256=uNbqLjtecFosoFzpGAC89-5icikWODKI8rOjbi8v_sA,10
+casambi_bt-0.1.3.dist-info/RECORD,,
```

