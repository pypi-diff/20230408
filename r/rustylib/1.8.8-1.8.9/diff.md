# Comparing `tmp/rustylib-1.8.8.tar.gz` & `tmp/rustylib-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustylib-1.8.8.tar", last modified: Sat Apr  8 16:45:40 2023, max compression
+gzip compressed data, was "rustylib-1.8.9.tar", last modified: Sat Apr  8 17:48:46 2023, max compression
```

## Comparing `rustylib-1.8.8.tar` & `rustylib-1.8.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 16:45:40.038476 rustylib-1.8.8/
--rw-rw-rw-   0        0        0     1421 2023-04-08 16:45:40.039505 rustylib-1.8.8/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-04-08 16:42:11.000000 rustylib-1.8.8/README.md
--rw-rw-rw-   0        0        0      140 2023-02-23 18:16:03.000000 rustylib-1.8.8/pyproject.toml
--rw-rw-rw-   0        0        0      666 2023-04-08 16:45:40.043476 rustylib-1.8.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 16:45:39.925477 rustylib-1.8.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 16:45:39.963477 rustylib-1.8.8/src/rustylib/
--rw-rw-rw-   0        0        0      239 2023-02-10 15:07:06.000000 rustylib-1.8.8/src/rustylib/Rcolor.py
--rw-rw-rw-   0        0        0     4507 2023-04-08 16:40:45.000000 rustylib-1.8.8/src/rustylib/Rkon.py
--rw-rw-rw-   0        0        0     4548 2023-04-08 15:13:27.000000 rustylib-1.8.8/src/rustylib/Rmath.py
--rw-rw-rw-   0        0        0     2740 2023-02-19 17:16:23.000000 rustylib-1.8.8/src/rustylib/Rrandom.py
--rw-rw-rw-   0        0        0     1460 2023-02-01 19:47:34.000000 rustylib-1.8.8/src/rustylib/Rrequests.py
--rw-rw-rw-   0        0        0     1771 2023-02-04 10:37:10.000000 rustylib-1.8.8/src/rustylib/Rsugaku.py
--rw-rw-rw-   0        0        0    11830 2023-04-08 16:39:12.000000 rustylib-1.8.8/src/rustylib/Rusty.py
--rw-rw-rw-   0        0        0      475 2023-02-25 16:22:19.000000 rustylib-1.8.8/src/rustylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 16:45:40.033476 rustylib-1.8.8/src/rustylib.egg-info/
--rw-rw-rw-   0        0        0     1421 2023-04-08 16:45:39.000000 rustylib-1.8.8/src/rustylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-08 16:45:39.000000 rustylib-1.8.8/src/rustylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 16:45:39.000000 rustylib-1.8.8/src/rustylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 16:45:39.000000 rustylib-1.8.8/src/rustylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:48:46.161373 rustylib-1.8.9/
+-rw-rw-rw-   0        0        0     1421 2023-04-08 17:48:46.162374 rustylib-1.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-04-08 16:42:11.000000 rustylib-1.8.9/README.md
+-rw-rw-rw-   0        0        0      140 2023-02-23 18:16:03.000000 rustylib-1.8.9/pyproject.toml
+-rw-rw-rw-   0        0        0      666 2023-04-08 17:48:46.173394 rustylib-1.8.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 17:48:45.732851 rustylib-1.8.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 17:48:46.057373 rustylib-1.8.9/src/rustylib/
+-rw-rw-rw-   0        0        0      239 2023-02-10 15:07:06.000000 rustylib-1.8.9/src/rustylib/Rcolor.py
+-rw-rw-rw-   0        0        0     4507 2023-04-08 16:40:45.000000 rustylib-1.8.9/src/rustylib/Rkon.py
+-rw-rw-rw-   0        0        0     4821 2023-04-08 17:35:44.000000 rustylib-1.8.9/src/rustylib/Rmath.py
+-rw-rw-rw-   0        0        0     2740 2023-02-19 17:16:23.000000 rustylib-1.8.9/src/rustylib/Rrandom.py
+-rw-rw-rw-   0        0        0     1460 2023-02-01 19:47:34.000000 rustylib-1.8.9/src/rustylib/Rrequests.py
+-rw-rw-rw-   0        0        0     1771 2023-02-04 10:37:10.000000 rustylib-1.8.9/src/rustylib/Rsugaku.py
+-rw-rw-rw-   0        0        0    11830 2023-04-08 17:47:29.000000 rustylib-1.8.9/src/rustylib/Rusty.py
+-rw-rw-rw-   0        0        0      440 2023-04-08 17:35:12.000000 rustylib-1.8.9/src/rustylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:48:46.151373 rustylib-1.8.9/src/rustylib.egg-info/
+-rw-rw-rw-   0        0        0     1421 2023-04-08 17:48:45.000000 rustylib-1.8.9/src/rustylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-08 17:48:45.000000 rustylib-1.8.9/src/rustylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:48:45.000000 rustylib-1.8.9/src/rustylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-08 17:48:45.000000 rustylib-1.8.9/src/rustylib.egg-info/top_level.txt
```

### Comparing `rustylib-1.8.8/PKG-INFO` & `rustylib-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustylib
-Version: 1.8.8
+Version: 1.8.9
 Summary: A useful python library for everything.
 Home-page: https://github.com/ZeyaTsu/rustylib
 Author: ZeyaTsu
 Project-URL: Bug Tracker, https://github.com/ZeyaTsu/rustylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rustylib-1.8.8/README.md` & `rustylib-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `rustylib-1.8.8/setup.cfg` & `rustylib-1.8.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 7573 7479 6c69 620d 0a76 6572   = rustylib..ver
-00000020: 7369 6f6e 203d 2031 2e38 2e38 0d0a 6175  sion = 1.8.8..au
+00000020: 7369 6f6e 203d 2031 2e38 2e39 0d0a 6175  sion = 1.8.9..au
 00000030: 7468 6f72 203d 205a 6579 6154 7375 0d0a  thor = ZeyaTsu..
 00000040: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000050: 7573 6566 756c 2070 7974 686f 6e20 6c69  useful python li
 00000060: 6272 6172 7920 666f 7220 6576 6572 7974  brary for everyt
 00000070: 6869 6e67 2e0d 0a6c 6f6e 675f 6465 7363  hing...long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
```

### Comparing `rustylib-1.8.8/src/rustylib/Rkon.py` & `rustylib-1.8.9/src/rustylib/Rkon.py`

 * *Files identical despite different names*

### Comparing `rustylib-1.8.8/src/rustylib/Rmath.py` & `rustylib-1.8.9/src/rustylib/Rmath.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,24 @@
         num = number
         while increment > 0:
             num *= increment
             increment-=1
         if number == 0:
             return 1
         return num
+    
+    def sumi(seq, i=0):
+        total = 0
+        if isinstance(seq, (list, tuple)):
+            for num in seq[i:]:
+                total += num
+            return total
+        else:
+            print("Rusty Error - seq can be either a tuple or a list.")
+
         
     pi = 3.1415926535897932384626433832795028841971693993751058209749445923078164062862089986280348253421170679821480865132823066470938446095505822317253594081284811174502841027019385211055596446229489549303819644288109756659334461284756482337867831652712019091456485669234603486104543266482133936072602491412737245870066063155881748815209209628292540917153643678925903600113305305488204665213841469519415116094330572703657595919530921861173819326117931051185480744623799627495673518857527248912279381830119491298336733624406566430860213949463952247371907021798609437027705392171762931767523846748184676694051320005681271452635608277857713427577896091736371787214684409012249534301465495853710507922796892589235420199561121290219608640344181598136297747713099605187072113499999983729780499510597317328160963185950244594553469083026425223082533446850352619311881710100031378387528865875332083814206171776691473035982534904287554687311595628638823537875937519577818577805321712268066130019278766111959092164201989
 
 class Object():
     def __init__(self):
         self.x = 0
         self.y = 0
```

### Comparing `rustylib-1.8.8/src/rustylib/Rrandom.py` & `rustylib-1.8.9/src/rustylib/Rrandom.py`

 * *Files identical despite different names*

### Comparing `rustylib-1.8.8/src/rustylib/Rrequests.py` & `rustylib-1.8.9/src/rustylib/Rrequests.py`

 * *Files identical despite different names*

### Comparing `rustylib-1.8.8/src/rustylib/Rsugaku.py` & `rustylib-1.8.9/src/rustylib/Rsugaku.py`

 * *Files identical despite different names*

### Comparing `rustylib-1.8.8/src/rustylib/Rusty.py` & `rustylib-1.8.9/src/rustylib/Rusty.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             if analysis[indx] == wanted:
                 valueRETURN = analysis[indx]
                 found.append(valueRETURN)
         return len(found)
 
     def pkginfo():
         NAME = 'rustylib'
-        VERSION = '1.8.8'
+        VERSION = '1.8.9'
         cache = []
         web = Request("https://raw.githubusercontent.com/ZeyaTsu/rustylib/main/Rpkg_info.json")
         res = web.send()
         if res == True:
             cache.append(NAME)
             cache.append(web.get("name"))
             cache.append(VERSION)
```

### Comparing `rustylib-1.8.8/src/rustylib.egg-info/PKG-INFO` & `rustylib-1.8.9/src/rustylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustylib
-Version: 1.8.8
+Version: 1.8.9
 Summary: A useful python library for everything.
 Home-page: https://github.com/ZeyaTsu/rustylib
 Author: ZeyaTsu
 Project-URL: Bug Tracker, https://github.com/ZeyaTsu/rustylib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

