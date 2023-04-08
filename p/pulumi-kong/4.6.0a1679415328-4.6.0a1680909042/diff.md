# Comparing `tmp/pulumi_kong-4.6.0a1679415328.tar.gz` & `tmp/pulumi_kong-4.6.0a1680909042.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kong-4.6.0a1679415328.tar", last modified: Tue Mar 21 16:28:59 2023, max compression
+gzip compressed data, was "pulumi_kong-4.6.0a1680909042.tar", last modified: Fri Apr  7 23:20:27 2023, max compression
```

## Comparing `pulumi_kong-4.6.0a1679415328.tar` & `pulumi_kong-4.6.0a1680909042.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:59.372289 pulumi_kong-4.6.0a1679415328/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-21 16:28:59.372289 pulumi_kong-4.6.0a1679415328/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:59.368289 pulumi_kong-4.6.0a1679415328/pulumi_kong/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:59.368289 pulumi_kong-4.6.0a1679415328/pulumi_kong/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_key_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14562 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54615 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/target.py
--rw-r--r--   0 runner    (1001) docker     (123)    73091 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong/upstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:28:59.368289 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 16:28:59.372289 pulumi_kong-4.6.0a1679415328/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-21 16:28:59.000000 pulumi_kong-4.6.0a1679415328/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/pulumi_kong/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/pulumi_kong/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_key_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14562 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54615 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73091 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong/upstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:20:27.018556 pulumi_kong-4.6.0a1680909042/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-07 23:20:26.000000 pulumi_kong-4.6.0a1680909042/setup.py
```

### Comparing `pulumi_kong-4.6.0a1679415328/PKG-INFO` & `pulumi_kong-4.6.0a1680909042/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1679415328
+Version: 4.6.0a1680909042
 Summary: A Pulumi package for creating and managing Kong resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi kong
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1679415328/README.md` & `pulumi_kong-4.6.0a1680909042/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/__init__.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/_inputs.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/_utilities.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/certificate.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/config/vars.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_acl.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_basic_auth.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_jwt_auth.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_key_auth.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_key_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/consumer_oauth2.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/consumer_oauth2.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/outputs.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/plugin.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/provider.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/route.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/service.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/target.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/target.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong/upstream.py` & `pulumi_kong-4.6.0a1680909042/pulumi_kong/upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/PKG-INFO` & `pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-kong
-Version: 4.6.0a1679415328
+Version: 4.6.0a1680909042
 Summary: A Pulumi package for creating and managing Kong resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi kong
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1679415328/pulumi_kong.egg-info/SOURCES.txt` & `pulumi_kong-4.6.0a1680909042/pulumi_kong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1679415328/setup.py` & `pulumi_kong-4.6.0a1680909042/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.6.0a1679415328"
-PLUGIN_VERSION = "4.6.0-alpha.1679415328+5679c7b3"
+VERSION = "4.6.0a1680909042"
+PLUGIN_VERSION = "4.6.0-alpha.1680909042+079aa03c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'kong', PLUGIN_VERSION])
         except OSError as error:
```

