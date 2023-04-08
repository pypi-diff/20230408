# Comparing `tmp/hotbox-0.0.7.tar.gz` & `tmp/hotbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotbox-0.0.7.tar", last modified: Sat Apr  8 21:29:50 2023, max compression
+gzip compressed data, was "hotbox-0.0.8.tar", last modified: Sat Apr  8 21:45:12 2023, max compression
```

## Comparing `hotbox-0.0.7.tar` & `hotbox-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.816714 hotbox-0.0.7/
--rw-r--r--   0 anthony    (501) staff       (20)     1056 2023-03-06 04:40:01.000000 hotbox-0.0.7/LICENSE
--rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 21:29:50.816783 hotbox-0.0.7/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)     2652 2023-04-08 16:05:40.000000 hotbox-0.0.7/README.md
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.808792 hotbox-0.0.7/hotbox/
--rw-r--r--   0 anthony    (501) staff       (20)       36 2023-04-08 21:29:35.000000 hotbox-0.0.7/hotbox/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     1596 2023-04-06 15:33:42.000000 hotbox-0.0.7/hotbox/api.py
--rw-r--r--   0 anthony    (501) staff       (20)     5120 2023-04-08 21:27:50.000000 hotbox-0.0.7/hotbox/app.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.812981 hotbox-0.0.7/hotbox/cli/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.7/hotbox/cli/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     4269 2023-04-08 18:39:05.000000 hotbox-0.0.7/hotbox/cli/create.py
--rw-r--r--   0 anthony    (501) staff       (20)      572 2023-04-08 17:35:10.000000 hotbox-0.0.7/hotbox/cli/delete.py
--rw-r--r--   0 anthony    (501) staff       (20)      444 2023-04-06 05:12:36.000000 hotbox-0.0.7/hotbox/cli/get.py
--rw-r--r--   0 anthony    (501) staff       (20)      523 2023-04-04 02:44:54.000000 hotbox-0.0.7/hotbox/cli/main.py
--rw-r--r--   0 anthony    (501) staff       (20)      861 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/cli/server.py
--rw-r--r--   0 anthony    (501) staff       (20)      446 2023-04-08 15:46:03.000000 hotbox-0.0.7/hotbox/const.py
--rw-r--r--   0 anthony    (501) staff       (20)     2657 2023-04-08 19:04:54.000000 hotbox-0.0.7/hotbox/ec2.py
--rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.7/hotbox/py.typed
--rw-r--r--   0 anthony    (501) staff       (20)      721 2023-04-08 16:05:45.000000 hotbox-0.0.7/hotbox/settings.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.813487 hotbox-0.0.7/hotbox/templates/
--rw-r--r--   0 anthony    (501) staff       (20)     1785 2023-04-08 20:34:29.000000 hotbox-0.0.7/hotbox/templates/ec2_userdata.sh.j2
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.814628 hotbox-0.0.7/hotbox/templates/image/
--rw-r--r--   0 anthony    (501) staff       (20)      373 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/Dockerfile.j2
--rw-r--r--   0 anthony    (501) staff       (20)      559 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/entrypoint.j2
--rw-r--r--   0 anthony    (501) staff       (20)      182 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/inittab
--rw-r--r--   0 anthony    (501) staff       (20)       31 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/interfaces
--rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/resolv.conf
--rw-r--r--   0 anthony    (501) staff       (20)      383 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/image/start.sh.j2
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.806316 hotbox-0.0.7/hotbox/templates/lang/
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.815056 hotbox-0.0.7/hotbox/templates/lang/go/
--rw-r--r--   0 anthony    (501) staff       (20)       58 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/lang/go/build
--rw-r--r--   0 anthony    (501) staff       (20)       24 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/lang/go/entrypoint
--rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.7/hotbox/templates/lang/go/install
--rw-r--r--   0 anthony    (501) staff       (20)     4001 2023-04-08 21:13:31.000000 hotbox-0.0.7/hotbox/templates/run_app.sh.j2
--rw-r--r--   0 anthony    (501) staff       (20)     1387 2023-04-08 19:04:51.000000 hotbox-0.0.7/hotbox/types.py
--rw-r--r--   0 anthony    (501) staff       (20)      808 2023-04-06 05:12:27.000000 hotbox-0.0.7/hotbox/utils.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.809602 hotbox-0.0.7/hotbox.egg-info/
--rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)      978 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/SOURCES.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/dependency_links.txt
--rw-r--r--   0 anthony    (501) staff       (20)       47 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/entry_points.txt
--rw-r--r--   0 anthony    (501) staff       (20)      378 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/requires.txt
--rw-r--r--   0 anthony    (501) staff       (20)        7 2023-04-08 21:29:50.000000 hotbox-0.0.7/hotbox.egg-info/top_level.txt
--rw-r--r--   0 anthony    (501) staff       (20)     1458 2023-04-06 22:03:03.000000 hotbox-0.0.7/pyproject.toml
--rw-r--r--   0 anthony    (501) staff       (20)      305 2023-04-08 21:29:50.817050 hotbox-0.0.7/setup.cfg
--rw-r--r--   0 anthony    (501) staff       (20)       38 2023-03-06 04:40:01.000000 hotbox-0.0.7/setup.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:29:50.816500 hotbox-0.0.7/tests/
--rw-r--r--   0 anthony    (501) staff       (20)     1116 2023-04-06 05:02:03.000000 hotbox-0.0.7/tests/test_api.py
--rw-r--r--   0 anthony    (501) staff       (20)     1757 2023-04-06 04:37:20.000000 hotbox-0.0.7/tests/test_app_cli.py
--rw-r--r--   0 anthony    (501) staff       (20)      481 2023-04-06 02:17:13.000000 hotbox-0.0.7/tests/test_cli.py
--rw-r--r--   0 anthony    (501) staff       (20)     2693 2023-04-08 18:36:22.000000 hotbox-0.0.7/tests/test_ec2_cli.py
--rw-r--r--   0 anthony    (501) staff       (20)      102 2023-04-06 02:17:21.000000 hotbox-0.0.7/tests/test_version.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.050187 hotbox-0.0.8/
+-rw-r--r--   0 anthony    (501) staff       (20)     1056 2023-03-06 04:40:01.000000 hotbox-0.0.8/LICENSE
+-rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 21:45:12.050255 hotbox-0.0.8/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)     2652 2023-04-08 16:05:40.000000 hotbox-0.0.8/README.md
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.044910 hotbox-0.0.8/hotbox/
+-rw-r--r--   0 anthony    (501) staff       (20)       36 2023-04-08 21:41:47.000000 hotbox-0.0.8/hotbox/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1596 2023-04-06 15:33:42.000000 hotbox-0.0.8/hotbox/api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5139 2023-04-08 21:41:34.000000 hotbox-0.0.8/hotbox/app.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.046952 hotbox-0.0.8/hotbox/cli/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.8/hotbox/cli/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4269 2023-04-08 18:39:05.000000 hotbox-0.0.8/hotbox/cli/create.py
+-rw-r--r--   0 anthony    (501) staff       (20)      572 2023-04-08 17:35:10.000000 hotbox-0.0.8/hotbox/cli/delete.py
+-rw-r--r--   0 anthony    (501) staff       (20)      444 2023-04-06 05:12:36.000000 hotbox-0.0.8/hotbox/cli/get.py
+-rw-r--r--   0 anthony    (501) staff       (20)      523 2023-04-04 02:44:54.000000 hotbox-0.0.8/hotbox/cli/main.py
+-rw-r--r--   0 anthony    (501) staff       (20)      861 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/cli/server.py
+-rw-r--r--   0 anthony    (501) staff       (20)      446 2023-04-08 15:46:03.000000 hotbox-0.0.8/hotbox/const.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2657 2023-04-08 19:04:54.000000 hotbox-0.0.8/hotbox/ec2.py
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.8/hotbox/py.typed
+-rw-r--r--   0 anthony    (501) staff       (20)      721 2023-04-08 16:05:45.000000 hotbox-0.0.8/hotbox/settings.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.047441 hotbox-0.0.8/hotbox/templates/
+-rw-r--r--   0 anthony    (501) staff       (20)     1785 2023-04-08 21:30:23.000000 hotbox-0.0.8/hotbox/templates/ec2_userdata.sh.j2
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.048502 hotbox-0.0.8/hotbox/templates/image/
+-rw-r--r--   0 anthony    (501) staff       (20)      373 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/Dockerfile.j2
+-rw-r--r--   0 anthony    (501) staff       (20)      559 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/entrypoint.j2
+-rw-r--r--   0 anthony    (501) staff       (20)      182 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/inittab
+-rw-r--r--   0 anthony    (501) staff       (20)       31 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/interfaces
+-rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/resolv.conf
+-rw-r--r--   0 anthony    (501) staff       (20)      383 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/image/start.sh.j2
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.042087 hotbox-0.0.8/hotbox/templates/lang/
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.048972 hotbox-0.0.8/hotbox/templates/lang/go/
+-rw-r--r--   0 anthony    (501) staff       (20)       58 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/lang/go/build
+-rw-r--r--   0 anthony    (501) staff       (20)       24 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/lang/go/entrypoint
+-rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.8/hotbox/templates/lang/go/install
+-rw-r--r--   0 anthony    (501) staff       (20)     4001 2023-04-08 21:13:31.000000 hotbox-0.0.8/hotbox/templates/run_app.sh.j2
+-rw-r--r--   0 anthony    (501) staff       (20)     1387 2023-04-08 19:04:51.000000 hotbox-0.0.8/hotbox/types.py
+-rw-r--r--   0 anthony    (501) staff       (20)      808 2023-04-06 05:12:27.000000 hotbox-0.0.8/hotbox/utils.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.045839 hotbox-0.0.8/hotbox.egg-info/
+-rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)      978 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        1 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony    (501) staff       (20)       47 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/entry_points.txt
+-rw-r--r--   0 anthony    (501) staff       (20)      378 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/requires.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        7 2023-04-08 21:45:12.000000 hotbox-0.0.8/hotbox.egg-info/top_level.txt
+-rw-r--r--   0 anthony    (501) staff       (20)     1458 2023-04-06 22:03:03.000000 hotbox-0.0.8/pyproject.toml
+-rw-r--r--   0 anthony    (501) staff       (20)      305 2023-04-08 21:45:12.050531 hotbox-0.0.8/setup.cfg
+-rw-r--r--   0 anthony    (501) staff       (20)       38 2023-03-06 04:40:01.000000 hotbox-0.0.8/setup.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 21:45:12.049964 hotbox-0.0.8/tests/
+-rw-r--r--   0 anthony    (501) staff       (20)     1116 2023-04-06 05:02:03.000000 hotbox-0.0.8/tests/test_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1757 2023-04-06 04:37:20.000000 hotbox-0.0.8/tests/test_app_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)      481 2023-04-06 02:17:13.000000 hotbox-0.0.8/tests/test_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2693 2023-04-08 18:36:22.000000 hotbox-0.0.8/tests/test_ec2_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)      102 2023-04-06 02:17:21.000000 hotbox-0.0.8/tests/test_version.py
```

### Comparing `hotbox-0.0.7/LICENSE` & `hotbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/PKG-INFO` & `hotbox-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: hotbox
 Author-email: Anthony Corletti <anthcor@gmail.com>
 License: See LICENSE
 Project-URL: Documentation, https://github.com/anthonycorletti/hotbox
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hotbox Version: 0.0.7 Summary: hotbox Author-email:
+Metadata-Version: 2.1 Name: hotbox Version: 0.0.8 Summary: hotbox Author-email:
 Anthony Corletti
 gmail.com> License: See LICENSE Project-URL: Documentation, https://github.com/
 anthonycorletti/hotbox Requires-Python: >=3.10 Description-Content-Type: text/
 markdown Provides-Extra: test Provides-Extra: dev License-File: LICENSE
                                    [hotbox]
    ð Run your code ð¦ on Firecracker MicroVMs ð¥ in the cloud âï¸
                       [Test] [publish] [Coverage] [PyPI]
```

### Comparing `hotbox-0.0.7/README.md` & `hotbox-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/api.py` & `hotbox-0.0.8/hotbox/api.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/app.py` & `hotbox-0.0.8/hotbox/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
                     "application/json",
                 ),
             },
         )
         return response
 
     def unzip_and_run(self, bundle_path: str, app_id: str) -> None:  # pragma: no cover
-        os.system(f"tar -xzf {bundle_path}")
-        os.system(f"chmod +x {app_id}_run_app.sh")
         # TODO: uncomment this
-        # os.system(f"./{app_id}_run_app.sh")
+        # os.system(f"tar -xzf {bundle_path}")
+        # os.system(f"chmod +x {app_id}_run_app.sh")
+        # os.system(f"./{app_id}_run_app.sh &")
         # os.remove(bundle_path)
+        pass
 
 
 app_svc = AppService()
```

### Comparing `hotbox-0.0.7/hotbox/cli/create.py` & `hotbox-0.0.8/hotbox/cli/create.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/cli/delete.py` & `hotbox-0.0.8/hotbox/cli/delete.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/cli/main.py` & `hotbox-0.0.8/hotbox/cli/main.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/cli/server.py` & `hotbox-0.0.8/hotbox/cli/server.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/ec2.py` & `hotbox-0.0.8/hotbox/ec2.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/settings.py` & `hotbox-0.0.8/hotbox/settings.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/templates/ec2_userdata.sh.j2` & `hotbox-0.0.8/hotbox/templates/ec2_userdata.sh.j2`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/templates/image/entrypoint.j2` & `hotbox-0.0.8/hotbox/templates/image/entrypoint.j2`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/templates/run_app.sh.j2` & `hotbox-0.0.8/hotbox/templates/run_app.sh.j2`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/types.py` & `hotbox-0.0.8/hotbox/types.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox/utils.py` & `hotbox-0.0.8/hotbox/utils.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/hotbox.egg-info/PKG-INFO` & `hotbox-0.0.8/hotbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: hotbox
 Author-email: Anthony Corletti <anthcor@gmail.com>
 License: See LICENSE
 Project-URL: Documentation, https://github.com/anthonycorletti/hotbox
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hotbox Version: 0.0.7 Summary: hotbox Author-email:
+Metadata-Version: 2.1 Name: hotbox Version: 0.0.8 Summary: hotbox Author-email:
 Anthony Corletti
 gmail.com> License: See LICENSE Project-URL: Documentation, https://github.com/
 anthonycorletti/hotbox Requires-Python: >=3.10 Description-Content-Type: text/
 markdown Provides-Extra: test Provides-Extra: dev License-File: LICENSE
                                    [hotbox]
    ð Run your code ð¦ on Firecracker MicroVMs ð¥ in the cloud âï¸
                       [Test] [publish] [Coverage] [PyPI]
```

### Comparing `hotbox-0.0.7/hotbox.egg-info/SOURCES.txt` & `hotbox-0.0.8/hotbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/pyproject.toml` & `hotbox-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/tests/test_api.py` & `hotbox-0.0.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/tests/test_app_cli.py` & `hotbox-0.0.8/tests/test_app_cli.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.7/tests/test_ec2_cli.py` & `hotbox-0.0.8/tests/test_ec2_cli.py`

 * *Files identical despite different names*

