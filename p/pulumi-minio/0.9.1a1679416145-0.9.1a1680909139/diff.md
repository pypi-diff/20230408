# Comparing `tmp/pulumi_minio-0.9.1a1679416145.tar.gz` & `tmp/pulumi_minio-0.9.1a1680909139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_minio-0.9.1a1679416145.tar", last modified: Tue Mar 21 16:40:36 2023, max compression
+gzip compressed data, was "pulumi_minio-0.9.1a1680909139.tar", last modified: Fri Apr  7 23:24:38 2023, max compression
```

## Comparing `pulumi_minio-0.9.1a1679416145.tar` & `pulumi_minio-0.9.1a1680909139.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/pulumi_minio/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/pulumi_minio/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/get_iam_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_user_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_user_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/ilm_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 16:40:36.000000 pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 16:40:36.151320 pulumi_minio-0.9.1a1679416145/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-21 16:40:35.000000 pulumi_minio-0.9.1a1679416145/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:38.763461 pulumi_minio-0.9.1a1680909139/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-07 23:24:38.763461 pulumi_minio-0.9.1a1680909139/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:38.759461 pulumi_minio-0.9.1a1680909139/pulumi_minio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:38.763461 pulumi_minio-0.9.1a1680909139/pulumi_minio/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/get_iam_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_user_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_user_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/ilm_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:38.763461 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:24:38.763461 pulumi_minio-0.9.1a1680909139/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-07 23:24:38.000000 pulumi_minio-0.9.1a1680909139/setup.py
```

### Comparing `pulumi_minio-0.9.1a1679416145/PKG-INFO` & `pulumi_minio-0.9.1a1680909139/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_minio
-Version: 0.9.1a1679416145
+Version: 0.9.1a1680909139
 Summary: A Pulumi package for creating and managing minio cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-minio
 Keywords: pulumi minio
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_minio-0.9.1a1679416145/README.md` & `pulumi_minio-0.9.1a1680909139/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/__init__.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/_inputs.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/_utilities.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/config/vars.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/get_iam_policy_document.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/get_iam_policy_document.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_membership.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_policy.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_policy_attachment.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_group_user_attachment.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_group_user_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_policy.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_service_account.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_user.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/iam_user_policy_attachment.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/iam_user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/ilm_policy.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/ilm_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/outputs.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/provider.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_notification.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_policy.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_bucket_versioning.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio/s3_object.py` & `pulumi_minio-0.9.1a1680909139/pulumi_minio/s3_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/PKG-INFO` & `pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-minio
-Version: 0.9.1a1679416145
+Version: 0.9.1a1680909139
 Summary: A Pulumi package for creating and managing minio cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-minio
 Keywords: pulumi minio
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_minio-0.9.1a1679416145/pulumi_minio.egg-info/SOURCES.txt` & `pulumi_minio-0.9.1a1680909139/pulumi_minio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_minio-0.9.1a1679416145/setup.py` & `pulumi_minio-0.9.1a1680909139/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.1a1679416145"
-PLUGIN_VERSION = "0.9.1-alpha.1679416145+f58cea54"
+VERSION = "0.9.1a1680909139"
+PLUGIN_VERSION = "0.9.1-alpha.1680909139+9a3d02c8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'minio', PLUGIN_VERSION])
         except OSError as error:
```

