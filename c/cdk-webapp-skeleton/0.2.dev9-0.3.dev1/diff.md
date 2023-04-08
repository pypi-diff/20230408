# Comparing `tmp/cdk_webapp_skeleton-0.2.dev9.tar.gz` & `tmp/cdk_webapp_skeleton-0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.2.dev9.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.3.dev1.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.2.dev9.tar` & `cdk_webapp_skeleton-0.3.dev1.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0       41 2023-03-04 17:24:38.946983 cdk_webapp_skeleton-0.2.dev9/README.md
--rw-r--r--   0        0        0      140 2023-03-05 17:48:38.904797 cdk_webapp_skeleton-0.2.dev9/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     1372 2023-03-05 19:02:17.362554 cdk_webapp_skeleton-0.2.dev9/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0      974 2023-03-05 16:39:22.989325 cdk_webapp_skeleton-0.2.dev9/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.2.dev9/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0      492 2023-03-05 19:03:08.623047 cdk_webapp_skeleton-0.2.dev9/pyproject.toml
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.2.dev9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-18 20:08:26.095902 cdk_webapp_skeleton-0.3.dev1/README.md
+-rw-r--r--   0        0        0      357 2023-03-19 05:12:26.210544 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-06 04:54:06.784822 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     1498 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     1909 2023-03-11 14:21:41.833987 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4717 2023-03-19 05:12:26.218545 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-03-05 18:01:24.075619 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     2906 2023-04-08 16:25:59.200667 cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0      593 2023-04-08 16:25:51.192530 cdk_webapp_skeleton-0.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.3.dev1/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.2.dev9/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.3.dev1/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import aws_cdk as cdk
-from aws_cdk import (
-    pipelines as pipelines,
-    aws_codebuild as codebuild,
-    aws_s3 as s3,
-)
+from aws_cdk import aws_codebuild as codebuild
+from aws_cdk import aws_s3 as s3
+from aws_cdk import pipelines as pipelines
 from constructs import Construct
 
 from .branch_config import BranchConfig
 
 
 class BranchCICDPipeline(Construct):
     def __init__(self, scope: Construct, branch_config: BranchConfig):
@@ -19,26 +17,31 @@
             removal_policy=cdk.RemovalPolicy.DESTROY,
             auto_delete_objects=True,
         )
 
         synth_step = pipelines.ShellStep(
             "Synth",
             input=branch_config.source,
-            env={"BRANCH": branch_config.branch_name, },
-            commands=["./synth.sh"]
+            env={
+                "BRANCH": branch_config.branch_name,
+            },
+            commands=["./synth.sh"],
         )
 
         self.cdk_pipeline = pipelines.CodePipeline(
             scope,
             "Pipeline",  # Pipeline name gets the stack name prepended
             synth=synth_step,
             code_build_defaults=pipelines.CodeBuildOptions(
                 build_environment=codebuild.BuildEnvironment(
                     compute_type=codebuild.ComputeType.SMALL
                 ),
                 cache=codebuild.Cache.bucket(cache_bucket),
             ),
-            cross_account_keys=False
+            cross_account_keys=False,
         )
 
     def add_stage(self, stage: cdk.Stage) -> pipelines.StageDeployment:
         return self.cdk_pipeline.add_stage(stage)
+
+    def build_pipeline(self):
+        self.cdk_pipeline.build_pipeline()
```

### Comparing `cdk_webapp_skeleton-0.2.dev9/PKG-INFO` & `cdk_webapp_skeleton-0.3.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.2.dev9
+Version: 0.3.dev1
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-cdk-lib (>=2.67.0,<3.0.0)
+Requires-Dist: cloudcomponents-cdk-static-website (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-Needs `synth.sh` at project root folder.
```

