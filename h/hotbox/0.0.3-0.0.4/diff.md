# Comparing `tmp/hotbox-0.0.3.tar.gz` & `tmp/hotbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotbox-0.0.3.tar", last modified: Mon Apr  3 03:59:05 2023, max compression
+gzip compressed data, was "hotbox-0.0.4.tar", last modified: Sat Apr  8 18:26:46 2023, max compression
```

## Comparing `hotbox-0.0.3.tar` & `hotbox-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,52 @@
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-03 03:59:05.860316 hotbox-0.0.3/
--rw-r--r--   0 anthony    (501) staff       (20)     1056 2023-03-06 04:40:01.000000 hotbox-0.0.3/LICENSE
--rw-r--r--   0 anthony    (501) staff       (20)      365 2023-04-03 03:59:05.860360 hotbox-0.0.3/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)       29 2023-03-15 02:06:28.000000 hotbox-0.0.3/README.md
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-03 03:59:05.858121 hotbox-0.0.3/hotbox/
--rw-r--r--   0 anthony    (501) staff       (20)       36 2023-04-03 03:57:32.000000 hotbox-0.0.3/hotbox/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     1596 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/api.py
--rw-r--r--   0 anthony    (501) staff       (20)     5188 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/app.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-03 03:59:05.859747 hotbox-0.0.3/hotbox/cli/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.3/hotbox/cli/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)     2354 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/cli/create.py
--rw-r--r--   0 anthony    (501) staff       (20)      683 2023-04-01 20:34:10.000000 hotbox-0.0.3/hotbox/cli/delete.py
--rw-r--r--   0 anthony    (501) staff       (20)      556 2023-04-01 20:34:10.000000 hotbox-0.0.3/hotbox/cli/get.py
--rw-r--r--   0 anthony    (501) staff       (20)      373 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/cli/main.py
--rw-r--r--   0 anthony    (501) staff       (20)      861 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/cli/server.py
--rw-r--r--   0 anthony    (501) staff       (20)      446 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/const.py
--rw-r--r--   0 anthony    (501) staff       (20)     2597 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/ec2.py
--rw-r--r--   0 anthony    (501) staff       (20)      721 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/settings.py
--rw-r--r--   0 anthony    (501) staff       (20)     1387 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/types.py
--rw-r--r--   0 anthony    (501) staff       (20)     1238 2023-04-03 03:26:37.000000 hotbox-0.0.3/hotbox/utils.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-03 03:59:05.858828 hotbox-0.0.3/hotbox.egg-info/
--rw-r--r--   0 anthony    (501) staff       (20)      365 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)      542 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/SOURCES.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/dependency_links.txt
--rw-r--r--   0 anthony    (501) staff       (20)       47 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/entry_points.txt
--rw-r--r--   0 anthony    (501) staff       (20)      285 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/requires.txt
--rw-r--r--   0 anthony    (501) staff       (20)       13 2023-04-03 03:59:05.000000 hotbox-0.0.3/hotbox.egg-info/top_level.txt
--rw-r--r--   0 anthony    (501) staff       (20)     1328 2023-04-03 03:26:37.000000 hotbox-0.0.3/pyproject.toml
--rw-r--r--   0 anthony    (501) staff       (20)      173 2023-04-03 03:59:05.860551 hotbox-0.0.3/setup.cfg
--rw-r--r--   0 anthony    (501) staff       (20)       38 2023-03-06 04:40:01.000000 hotbox-0.0.3/setup.py
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-03 03:59:05.860109 hotbox-0.0.3/tests/
--rw-r--r--   0 anthony    (501) staff       (20)        0 2023-03-06 04:40:01.000000 hotbox-0.0.3/tests/__init__.py
--rw-r--r--   0 anthony    (501) staff       (20)      176 2023-03-06 04:40:01.000000 hotbox-0.0.3/tests/conftest.py
--rw-r--r--   0 anthony    (501) staff       (20)       96 2023-03-14 23:56:36.000000 hotbox-0.0.3/tests/test_version.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.208122 hotbox-0.0.4/
+-rw-r--r--   0 anthony    (501) staff       (20)     1056 2023-03-06 04:40:01.000000 hotbox-0.0.4/LICENSE
+-rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 18:26:46.208175 hotbox-0.0.4/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)     2652 2023-04-08 16:05:40.000000 hotbox-0.0.4/README.md
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.202674 hotbox-0.0.4/hotbox/
+-rw-r--r--   0 anthony    (501) staff       (20)       36 2023-04-08 18:12:14.000000 hotbox-0.0.4/hotbox/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1596 2023-04-06 15:33:42.000000 hotbox-0.0.4/hotbox/api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5087 2023-04-06 04:51:35.000000 hotbox-0.0.4/hotbox/app.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.204791 hotbox-0.0.4/hotbox/cli/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.4/hotbox/cli/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4268 2023-04-08 18:11:53.000000 hotbox-0.0.4/hotbox/cli/create.py
+-rw-r--r--   0 anthony    (501) staff       (20)      572 2023-04-08 17:35:10.000000 hotbox-0.0.4/hotbox/cli/delete.py
+-rw-r--r--   0 anthony    (501) staff       (20)      444 2023-04-06 05:12:36.000000 hotbox-0.0.4/hotbox/cli/get.py
+-rw-r--r--   0 anthony    (501) staff       (20)      523 2023-04-04 02:44:54.000000 hotbox-0.0.4/hotbox/cli/main.py
+-rw-r--r--   0 anthony    (501) staff       (20)      861 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/cli/server.py
+-rw-r--r--   0 anthony    (501) staff       (20)      446 2023-04-08 15:46:03.000000 hotbox-0.0.4/hotbox/const.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2708 2023-04-08 17:09:44.000000 hotbox-0.0.4/hotbox/ec2.py
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2023-04-01 20:34:10.000000 hotbox-0.0.4/hotbox/py.typed
+-rw-r--r--   0 anthony    (501) staff       (20)      721 2023-04-08 16:05:45.000000 hotbox-0.0.4/hotbox/settings.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.205282 hotbox-0.0.4/hotbox/templates/
+-rw-r--r--   0 anthony    (501) staff       (20)     1783 2023-04-08 17:57:54.000000 hotbox-0.0.4/hotbox/templates/ec2_userdata.sh.j2
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.206426 hotbox-0.0.4/hotbox/templates/image/
+-rw-r--r--   0 anthony    (501) staff       (20)      373 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/Dockerfile.j2
+-rw-r--r--   0 anthony    (501) staff       (20)      559 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/entrypoint.j2
+-rw-r--r--   0 anthony    (501) staff       (20)      182 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/inittab
+-rw-r--r--   0 anthony    (501) staff       (20)       31 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/interfaces
+-rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/resolv.conf
+-rw-r--r--   0 anthony    (501) staff       (20)      383 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/image/start.sh.j2
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.199949 hotbox-0.0.4/hotbox/templates/lang/
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.206865 hotbox-0.0.4/hotbox/templates/lang/go/
+-rw-r--r--   0 anthony    (501) staff       (20)       58 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/lang/go/build
+-rw-r--r--   0 anthony    (501) staff       (20)       24 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/lang/go/entrypoint
+-rw-r--r--   0 anthony    (501) staff       (20)       19 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/lang/go/install
+-rw-r--r--   0 anthony    (501) staff       (20)     3491 2023-04-03 03:26:37.000000 hotbox-0.0.4/hotbox/templates/run_app.sh.j2
+-rw-r--r--   0 anthony    (501) staff       (20)     1477 2023-04-08 17:07:45.000000 hotbox-0.0.4/hotbox/types.py
+-rw-r--r--   0 anthony    (501) staff       (20)      808 2023-04-06 05:12:27.000000 hotbox-0.0.4/hotbox/utils.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.203514 hotbox-0.0.4/hotbox.egg-info/
+-rw-r--r--   0 anthony    (501) staff       (20)     2988 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)      978 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        1 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony    (501) staff       (20)       47 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/entry_points.txt
+-rw-r--r--   0 anthony    (501) staff       (20)      378 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/requires.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        7 2023-04-08 18:26:46.000000 hotbox-0.0.4/hotbox.egg-info/top_level.txt
+-rw-r--r--   0 anthony    (501) staff       (20)     1458 2023-04-06 22:03:03.000000 hotbox-0.0.4/pyproject.toml
+-rw-r--r--   0 anthony    (501) staff       (20)      305 2023-04-08 18:26:46.208407 hotbox-0.0.4/setup.cfg
+-rw-r--r--   0 anthony    (501) staff       (20)       38 2023-03-06 04:40:01.000000 hotbox-0.0.4/setup.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-04-08 18:26:46.207894 hotbox-0.0.4/tests/
+-rw-r--r--   0 anthony    (501) staff       (20)     1116 2023-04-06 05:02:03.000000 hotbox-0.0.4/tests/test_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1757 2023-04-06 04:37:20.000000 hotbox-0.0.4/tests/test_app_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)      481 2023-04-06 02:17:13.000000 hotbox-0.0.4/tests/test_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2693 2023-04-06 05:05:00.000000 hotbox-0.0.4/tests/test_ec2_cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)      102 2023-04-06 02:17:21.000000 hotbox-0.0.4/tests/test_version.py
```

### Comparing `hotbox-0.0.3/LICENSE` & `hotbox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.3/hotbox/api.py` & `hotbox-0.0.4/hotbox/api.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.3/hotbox/app.py` & `hotbox-0.0.4/hotbox/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import shutil
-from typing import Dict
 
 import httpx
+from httpx import Response
 from jinja2 import Template
 
 from hotbox.const import (
     DEFAULT_IMAGE_TEMPLATE_DIR,
     DEFAULT_LANG_TEMPLATE_DIR,
     DEFAULT_RUN_APP_TEMPLATE_FILEPATH,
 )
@@ -131,15 +131,15 @@
                 app_id=app_id,
                 vcpu_count=vcpu_count,
                 mem_size_mib=mem_size_mib,
             )
         with open(f"{tmpdir}/{app_id}_run_app.sh", "w") as f:
             f.write(template)
 
-    def upload_app_bundle(self, app_id: str, bundle_path: str) -> Dict:
+    def upload_app_bundle(self, app_id: str, bundle_path: str) -> Response:
         response = httpx.post(
             url=env.HOTBOX_API_URL + Routes.create_apps,
             files={
                 "upload_file": (
                     os.path.basename(bundle_path),
                     open(bundle_path, "rb"),
                     "application/gzip",
@@ -147,19 +147,17 @@
                 "create_app_request": (
                     None,
                     json.dumps({"app_id": app_id}),
                     "application/json",
                 ),
             },
         )
-        if not response.status_code == 200:
-            raise Exception(f"Failed to upload app bundle: {response.text}")
-        return response.json()
+        return response
 
-    def unzip_and_run(self, bundle_path: str, app_id: str) -> None:
+    def unzip_and_run(self, bundle_path: str, app_id: str) -> None:  # pragma: no cover
         os.system(f"tar -xzf {bundle_path}")
         os.system(f"chmod +x {app_id}_run_app.sh")
         os.system(f"./{app_id}_run_app.sh &")
         os.remove(bundle_path)
 
 
 app_svc = AppService()
```

### Comparing `hotbox-0.0.3/hotbox/cli/delete.py` & `hotbox-0.0.4/hotbox/cli/delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import json
 from typing import List
 
+import orjson
 from typer import Argument, Option, Typer, echo
 
 from hotbox.ec2 import ec2_svc
-from hotbox.utils import json_serializer
 
 app = Typer(
     name="delete",
     help="Delete resources.",
     no_args_is_help=True,
 )
 
@@ -25,13 +24,8 @@
     ),
     region: str = Option(
         None,
         help="AWS Region.",
     ),
 ) -> None:
     response = ec2_svc.delete(ids, region)
-    echo(
-        json.dumps(
-            response,
-            default=json_serializer,
-        )
-    )
+    echo(orjson.dumps(response))
```

### Comparing `hotbox-0.0.3/hotbox/cli/server.py` & `hotbox-0.0.4/hotbox/cli/server.py`

 * *Files identical despite different names*

### Comparing `hotbox-0.0.3/hotbox/ec2.py` & `hotbox-0.0.4/hotbox/ec2.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 from jinja2 import Template
 
 from hotbox.const import DEFAULT_USERDATA_TEMPLATE_FILEPATH
 from hotbox.types import Ec2Spec
 
 
 class Ec2Service:
-    def __init__(self) -> None:
-        self.aws_client = boto3.client
+    def ec2_client(self, region_name: str) -> boto3.client:
+        return boto3.client("ec2", region_name=region_name)  # pragma: no cover
 
     def get_image_id(
         self,
-        client: boto3.client,
+        ec2_client: boto3.client,
         name: str = "ubuntu/images/hvm-ssd/ubuntu-bionic-18.04-arm64-*",
         virtualization_type: str = "hvm",
         architecture: str = "arm64",
         root_device_type: str = "ebs",
         owner_id: str = "099720109477",
     ) -> str:
         filters = [
             {"Name": "name", "Values": [name]},
             {"Name": "virtualization-type", "Values": [virtualization_type]},
             {"Name": "architecture", "Values": [architecture]},
             {"Name": "root-device-type", "Values": [root_device_type]},
             {"Name": "owner-id", "Values": [owner_id]},
         ]
-        images = client.describe_images(Filters=filters)
+        images = ec2_client.describe_images(Filters=filters)
         images_sorted = sorted(
             images["Images"],
             key=lambda x: x["CreationDate"],
             reverse=True,
         )
         return images_sorted[0]["ImageId"]
 
@@ -42,30 +42,31 @@
     ) -> str:
         if userdata_template_filepath is None:
             userdata_template_filepath = DEFAULT_USERDATA_TEMPLATE_FILEPATH
         with open(userdata_template_filepath) as f:
             return Template(f.read()).render(firecracker_version=firecracker_version)
 
     def create(self, spec: Ec2Spec, firecracker_version: str) -> Dict:
-        ec2_client = self.aws_client("ec2", region_name=spec.region)
+        ec2_client = self.ec2_client(region_name=spec.region)
         return ec2_client.run_instances(
-            ImageId=self.get_image_id(client=ec2_client),
+            ImageId=self.get_image_id(ec2_client=ec2_client),
             KeyName=spec.key_name,
             InstanceType=spec.instance_type,
             MinCount=spec.min_count,
             MaxCount=spec.max_count,
             Monitoring=spec.monitoring_enabled,
             SecurityGroupIds=spec.security_group_ids,
             BlockDeviceMappings=spec.block_device_mappings,
+            MetadataOptions=spec.metadata_options,
             UserData=self._template_userdata(firecracker_version=firecracker_version),
         )
 
     def get(self, region: str) -> Dict:
-        ec2_client = self.aws_client("ec2", region_name=region)
+        ec2_client = self.ec2_client(region_name=region)
         return ec2_client.describe_instances()
 
     def delete(self, ids: List[str], region: str) -> Dict:
-        ec2_client = self.aws_client("ec2", region_name=region)
+        ec2_client = self.ec2_client(region_name=region)
         return ec2_client.terminate_instances(InstanceIds=ids)
 
 
 ec2_svc = Ec2Service()
```

### Comparing `hotbox-0.0.3/hotbox/settings.py` & `hotbox-0.0.4/hotbox/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pydantic import BaseSettings, Field
 
 
 class _Env(BaseSettings):
     HOTBOX_API_URL: str = Field(
         "http://localhost:8420/api/v0",
         env="HOTBOX_API_URL",
-        description="Hotbox API URL",
+        description="hotbox API URL",
     )
 
     class Config:
         env_file = ".env.local"
         env_file_encoding = "utf-8"
```

### Comparing `hotbox-0.0.3/hotbox/types.py` & `hotbox-0.0.4/hotbox/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 class Language(str, Enum):
     go = "go"
     # python = "py"
 
 
 @unique
 class Image(str, Enum):
-    """Image is the name of the Docker image to use for Hotbox."""
+    """Image is the name of the Docker image to use for hotbox."""
 
     go = "golang:1.20"
     # python = "python:3.11-slim"
 
 
 class Routes(str, Enum):
     create_apps = "/apps"
 
 
 @unique
 class Ec2MetalType(str, Enum):
-    """Ec2MetalType is the type of EC2 instance to use for Hotbox."""
+    """Ec2MetalType is the type of EC2 instance to use for hotbox."""
 
     a1_metal = "a1.metal"
     i3_metal = "i3.metal"
     g4dn_metal = "g4dn.metal"
 
 
 class HotboxSpec(BaseModel):
@@ -45,14 +45,17 @@
     security_group_ids: List[str]
     instance_type: Ec2MetalType = Ec2MetalType.a1_metal
     min_count: int = 1
     max_count: int = 1
     monitoring_enabled: Dict[str, Any] = {
         "Enabled": False,
     }
+    metadata_options: Dict[str, Any] = {
+        "InstanceMetadataTags": "enabled",
+    }
     block_device_mappings: List[Dict[str, Any]] = [
         {
             "DeviceName": "/dev/xvda",
             "Ebs": {
                 "DeleteOnTermination": True,
                 "VolumeSize": 8,
                 "VolumeType": "gp2",
```

### Comparing `hotbox-0.0.3/pyproject.toml` & `hotbox-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,33 +19,38 @@
     "pydantic >=1.8.2",
     "rich >=10.12.0",
     "jinja2 >=3.0.2",
     "python-multipart >=0.0.5",
     "uvicorn >=0.15.0",
     "httpx >=0.21.1",
     "python-dotenv >=0.19.1",
+    "orjson >=3.6.4",
 ]
 [[project.authors]]
 name = "Anthony Corletti"
 email = "anthcor@gmail.com"
 
 [project.scripts]
 hotbox = "hotbox.cli.main:app"
 
 [project.optional-dependencies]
 test = [
     "pytest >=6.2.5",
+    "pytest-asyncio >=0.20.3",
     "coverage >=6.1.1",
     "pytest-cov >=3.0.0",
 ]
 dev = [
     "mypy <1.1.1", # https://github.com/pydantic/pydantic/issues/5190
     "black >=21.10b0",
     "ruff >=0.0.98",
     "pre-commit >=2.17.0",
+    "mkdocs>=1.4.2",
+    "mdx-include>=1.4.2",
+    "mkdocs-material>=9.1.5",
 ]
 
 [project.urls]
 Documentation = "https://github.com/anthonycorletti/hotbox"
 
 [tool.setuptools.dynamic]
 version = {attr = "hotbox.__version__"}
```

