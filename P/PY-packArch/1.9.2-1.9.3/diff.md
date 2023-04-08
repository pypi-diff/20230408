# Comparing `tmp/PY-packArch-1.9.2.tar.gz` & `tmp/PY-packArch-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PY-packArch-1.9.2.tar", last modified: Thu Mar 16 20:34:19 2023, max compression
+gzip compressed data, was "PY-packArch-1.9.3.tar", last modified: Sat Apr  8 18:18:40 2023, max compression
```

## Comparing `PY-packArch-1.9.2.tar` & `PY-packArch-1.9.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-03-16 20:34:19.631512 PY-packArch-1.9.2/
--rw-r--r--   0 angel     (1000) users      (984)    35149 2023-03-07 00:39:50.000000 PY-packArch-1.9.2/LICENSE
--rw-r--r--   0 angel     (1000) users      (984)    10649 2023-03-16 20:34:19.631512 PY-packArch-1.9.2/PKG-INFO
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-03-16 20:34:19.631512 PY-packArch-1.9.2/PY_packArch.egg-info/
--rw-r--r--   0 angel     (1000) users      (984)    10649 2023-03-16 20:34:19.000000 PY-packArch-1.9.2/PY_packArch.egg-info/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)      184 2023-03-16 20:34:19.000000 PY-packArch-1.9.2/PY_packArch.egg-info/SOURCES.txt
--rw-r--r--   0 angel     (1000) users      (984)        1 2023-03-16 20:34:19.000000 PY-packArch-1.9.2/PY_packArch.egg-info/dependency_links.txt
--rw-r--r--   0 angel     (1000) users      (984)        9 2023-03-16 20:34:19.000000 PY-packArch-1.9.2/PY_packArch.egg-info/top_level.txt
--rw-r--r--   0 angel     (1000) users      (984)     9788 2023-03-16 20:33:20.000000 PY-packArch-1.9.2/README.md
--rw-r--r--   0 angel     (1000) users      (984)     8113 2023-03-16 20:33:26.000000 PY-packArch-1.9.2/packarch.py
--rw-r--r--   0 angel     (1000) users      (984)      848 2023-03-16 20:33:51.000000 PY-packArch-1.9.2/pyproject.toml
--rw-r--r--   0 angel     (1000) users      (984)       38 2023-03-16 20:34:19.631512 PY-packArch-1.9.2/setup.cfg
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/
+-rw-r--r--   0 angel     (1000) users      (984)    35149 2023-03-07 00:39:50.000000 PY-packArch-1.9.3/LICENSE
+-rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/PKG-INFO
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-08 18:18:40.249784 PY-packArch-1.9.3/PY_packArch.egg-info/
+-rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)      184 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/SOURCES.txt
+-rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/dependency_links.txt
+-rw-r--r--   0 angel     (1000) users      (984)        9 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/top_level.txt
+-rw-r--r--   0 angel     (1000) users      (984)     9810 2023-03-16 20:36:50.000000 PY-packArch-1.9.3/README.md
+-rw-r--r--   0 angel     (1000) users      (984)     8087 2023-04-08 18:14:37.000000 PY-packArch-1.9.3/packarch.py
+-rw-r--r--   0 angel     (1000) users      (984)      848 2023-04-08 18:17:31.000000 PY-packArch-1.9.3/pyproject.toml
+-rw-r--r--   0 angel     (1000) users      (984)       38 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/setup.cfg
```

### Comparing `PY-packArch-1.9.2/LICENSE` & `PY-packArch-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PY-packArch-1.9.2/PKG-INFO` & `PY-packArch-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PY-packArch
-Version: 1.9.2
+Version: 1.9.3
 Summary: Small library to manage pacman package manager and install packages from AUR
 Author-email: Tom5521 <mismarttv321@gmail.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/Tom5521/PY-PackArch
 Project-URL: Bug Tracker, https://github.com/Tom5521/PY-PackArch/issues
 Project-URL: Documentation, https://github.com/Tom5521/PY-PackArch/blob/master/README.md
 Project-URL: Download-url, https://github.com/Tom5521/PY-PackArch/archive/refs/heads/master.zip
@@ -13,15 +13,15 @@
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Software Distribution
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1678149263/py-packarch-pypi.png_diqgoq.png" width="1000" height="100" />
+<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1676571071/Captura_de_pantalla_de_2023-02-16_15-08-13_iiarxj.png" width="1000" height="100" />
 
 
 [![CodeFactor](https://www.codefactor.io/repository/github/tom5521/py-packarch/badge)](https://www.codefactor.io/repository/github/tom5521/py-packarch)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Tom5521/PY-pacman)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Tom5521/PY-pacman)
```

### Comparing `PY-packArch-1.9.2/PY_packArch.egg-info/PKG-INFO` & `PY-packArch-1.9.3/PY_packArch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PY-packArch
-Version: 1.9.2
+Version: 1.9.3
 Summary: Small library to manage pacman package manager and install packages from AUR
 Author-email: Tom5521 <mismarttv321@gmail.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/Tom5521/PY-PackArch
 Project-URL: Bug Tracker, https://github.com/Tom5521/PY-PackArch/issues
 Project-URL: Documentation, https://github.com/Tom5521/PY-PackArch/blob/master/README.md
 Project-URL: Download-url, https://github.com/Tom5521/PY-PackArch/archive/refs/heads/master.zip
@@ -13,15 +13,15 @@
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Software Distribution
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1678149263/py-packarch-pypi.png_diqgoq.png" width="1000" height="100" />
+<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1676571071/Captura_de_pantalla_de_2023-02-16_15-08-13_iiarxj.png" width="1000" height="100" />
 
 
 [![CodeFactor](https://www.codefactor.io/repository/github/tom5521/py-packarch/badge)](https://www.codefactor.io/repository/github/tom5521/py-packarch)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Tom5521/PY-pacman)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Tom5521/PY-pacman)
```

### Comparing `PY-packArch-1.9.2/README.md` & `PY-packArch-1.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1678149263/py-packarch-pypi.png_diqgoq.png" width="1000" height="100" />
+<img src="https://res.cloudinary.com/dqjsgmkxo/image/upload/v1676571071/Captura_de_pantalla_de_2023-02-16_15-08-13_iiarxj.png" width="1000" height="100" />
 
 
 [![CodeFactor](https://www.codefactor.io/repository/github/tom5521/py-packarch/badge)](https://www.codefactor.io/repository/github/tom5521/py-packarch)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Tom5521/PY-pacman)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Tom5521/PY-pacman)
```

### Comparing `PY-packArch-1.9.2/packarch.py` & `PY-packArch-1.9.3/packarch.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,19 +222,18 @@
     if cond1 != "":
         options = [""]
         print(words[6], words[4])
         if "o" in cond1:
             options[0] = "Ss"
             if "e" in cond1:
                 options[0] = "Si"
-        else:
-            if "l" in cond1:
-                options[0] = "Qs"
-                if "e" in cond1:
-                    options[0] = "Q"
+        elif "l" in cond1:
+            options[0] = "Qs"
+            if "e" in cond1:
+                options[0] = "Q"
         sys("pacman -" + options[0] + sp + list)
     else:
         sys("pacman -Ss " + list)
 
 
 def clone(link, route="", cond="", command=""):
     for i in link.split():
@@ -266,15 +265,15 @@
 
 def upgrade_me():
     sys("pip install py-packarch --upgrade")
     sys("pip3 install py-packarch --upgrade")
 
 
 def version():
-    print("PY-PackArch \nCreated by Tom5521 \nVersion 1.9.1\nUnder the gpl-3.0 licence")
+    print("PY-PackArch \nCreated by Tom5521 \nVersion 1.9.2\nUnder the gpl-3.0 licence")
 
 
 def info(package):
     sys("pacman -Si " + package)
 
 
 def get_version(packages, cond=""):
@@ -284,9 +283,10 @@
         readata = opendata.read()
         if "h" in cond:
             print(readata.split()[1])
         else:
             print(i + " is in version", (readata.split()[1]))
     sys("rm /tmp/transpaced_data")
 
+
 def manual():
-    sys("firefox https://github.com/Tom5521/PY-PackArch/blob/master/README.md")
+    sys("firefox https://github.com/Tom5521/PY-PackArch/blob/master/README.md")
```

### Comparing `PY-packArch-1.9.2/pyproject.toml` & `PY-packArch-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PY-packArch"
-version = "1.9.2"
+version = "1.9.3"
 authors = [
     { name="Tom5521", email="mismarttv321@gmail.com" },
 ]
 description = "Small library to manage pacman package manager and install packages from AUR"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GPL-3.0"}
```

