# Comparing `tmp/buildarr_prowlarr-0.1.0.tar.gz` & `tmp/buildarr_prowlarr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_prowlarr-0.1.0.tar", max compression
+gzip compressed data, was "buildarr_prowlarr-0.1.1.tar", max compression
```

## Comparing `buildarr_prowlarr-0.1.0.tar` & `buildarr_prowlarr-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      975 2023-04-07 23:02:24.120450 buildarr_prowlarr-0.1.0/buildarr_prowlarr/__init__.py
--rw-r--r--   0        0        0     3830 2023-04-07 23:02:24.122466 buildarr_prowlarr-0.1.0/buildarr_prowlarr/api.py
--rw-r--r--   0        0        0     2548 2023-04-07 23:02:24.124461 buildarr_prowlarr-0.1.0/buildarr_prowlarr/cli.py
--rw-r--r--   0        0        0     5261 2023-04-07 23:02:24.125463 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/__init__.py
--rw-r--r--   0        0        0     3913 2023-04-07 23:02:24.126462 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/__init__.py
--rw-r--r--   0        0        0     1055 2023-04-07 23:02:24.127460 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/__init__.py
--rw-r--r--   0        0        0    25850 2023-04-07 23:02:24.130478 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/applications.py
--rw-r--r--   0        0        0     8076 2023-04-07 23:02:24.131474 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/sync_profiles.py
--rw-r--r--   0        0        0    10178 2023-04-07 23:02:24.132464 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/__init__.py
--rw-r--r--   0        0        0     8582 2023-04-07 23:02:24.133475 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/base.py
--rw-r--r--   0        0        0    31803 2023-04-07 23:02:24.135481 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/torrent.py
--rw-r--r--   0        0        0    14416 2023-04-07 23:02:24.136473 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/usenet.py
--rw-r--r--   0        0        0    20465 2023-04-07 23:02:24.137475 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/general.py
--rw-r--r--   0        0        0     2117 2023-04-07 23:02:24.137475 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/__init__.py
--rw-r--r--   0        0        0    30340 2023-04-07 23:02:24.139476 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/indexers.py
--rw-r--r--   0        0        0    15916 2023-04-07 23:02:24.141486 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/proxies.py
--rw-r--r--   0        0        0    42999 2023-04-07 23:02:24.142460 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/notifications.py
--rw-r--r--   0        0        0     3384 2023-04-07 23:02:24.143481 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/tags.py
--rw-r--r--   0        0        0     7231 2023-04-07 23:02:24.144463 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/ui.py
--rw-r--r--   0        0        0     1034 2023-04-07 23:02:24.145467 buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/types.py
--rw-r--r--   0        0        0     1396 2023-04-07 23:02:24.146462 buildarr_prowlarr-0.1.0/buildarr_prowlarr/exceptions.py
--rw-r--r--   0        0        0      950 2023-04-07 23:02:24.147463 buildarr_prowlarr-0.1.0/buildarr_prowlarr/manager.py
--rw-r--r--   0        0        0     1189 2023-04-07 23:02:24.149469 buildarr_prowlarr-0.1.0/buildarr_prowlarr/plugin.py
--rw-r--r--   0        0        0        0 2023-04-07 23:02:24.150469 buildarr_prowlarr-0.1.0/buildarr_prowlarr/py.typed
--rw-r--r--   0        0        0     3841 2023-04-07 23:02:24.152467 buildarr_prowlarr-0.1.0/buildarr_prowlarr/secrets.py
--rw-r--r--   0        0        0     1162 2023-04-07 23:02:24.153475 buildarr_prowlarr-0.1.0/buildarr_prowlarr/types.py
--rw-r--r--   0        0        0     1465 2023-04-07 23:02:24.155467 buildarr_prowlarr-0.1.0/buildarr_prowlarr/util.py
--rw-r--r--   0        0        0    35149 2023-03-26 01:54:36.064607 buildarr_prowlarr-0.1.0/LICENSE
--rw-r--r--   0        0        0     2332 2023-04-07 23:02:24.179463 buildarr_prowlarr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11795 2023-04-07 23:02:24.118925 buildarr_prowlarr-0.1.0/README.md
--rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11795 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/README.md
+-rw-r--r--   0        0        0      975 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/__init__.py
+-rw-r--r--   0        0        0     3830 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/api.py
+-rw-r--r--   0        0        0     2548 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/cli.py
+-rw-r--r--   0        0        0     5261 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/__init__.py
+-rw-r--r--   0        0        0     3913 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/__init__.py
+-rw-r--r--   0        0        0    25596 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/applications.py
+-rw-r--r--   0        0        0     8237 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py
+-rw-r--r--   0        0        0    10178 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/__init__.py
+-rw-r--r--   0        0        0     8611 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/base.py
+-rw-r--r--   0        0        0    32335 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/torrent.py
+-rw-r--r--   0        0        0    14416 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/usenet.py
+-rw-r--r--   0        0        0    20465 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/general.py
+-rw-r--r--   0        0        0     2117 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/__init__.py
+-rw-r--r--   0        0        0    30713 2023-04-08 10:34:37.463080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/indexers.py
+-rw-r--r--   0        0        0    15858 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/proxies.py
+-rw-r--r--   0        0        0    42999 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/notifications.py
+-rw-r--r--   0        0        0     3384 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/tags.py
+-rw-r--r--   0        0        0     7231 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/ui.py
+-rw-r--r--   0        0        0     1034 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/types.py
+-rw-r--r--   0        0        0     1396 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/exceptions.py
+-rw-r--r--   0        0        0      950 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/manager.py
+-rw-r--r--   0        0        0     1189 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/py.typed
+-rw-r--r--   0        0        0     3841 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/secrets.py
+-rw-r--r--   0        0        0     1162 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/types.py
+-rw-r--r--   0        0        0     1465 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/buildarr_prowlarr/util.py
+-rw-r--r--   0        0        0     2332 2023-04-08 10:34:37.467080 buildarr_prowlarr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.1.1/PKG-INFO
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/api.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/api.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/cli.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/applications.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,37 +212,32 @@
         secrets: ProwlarrSecrets,
         remote: Self,
         api_application_schemas: List[prowlarr.ApplicationResource],
         category_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
         api_application: prowlarr.ApplicationResource,
     ) -> bool:
-        api_schema = self._get_api_schema(api_application_schemas)
-        changed, updated_attrs = self.get_update_remote_attrs(
+        changed, set_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
             remote_map=self._get_base_remote_map(category_ids, tag_ids) + self._remote_map,
+            set_unchanged=True,
         )
         if changed:
+            if "fields" in set_attrs:
+                field_values: Dict[str, Any] = {
+                    field["name"]: field["value"] for field in set_attrs["fields"]
+                }
+                set_attrs["fields"] = [
+                    {**f, "value": field_values[f["name"]]}
+                    for f in self._get_api_schema(api_application_schemas)["fields"]
+                ]
+            remote_attrs = {**api_application.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
-                application_api = prowlarr.ApplicationApi(api_client)
-                if "fields" in updated_attrs:
-                    field_values: Dict[str, Any] = {
-                        field["name"]: field["value"] for field in updated_attrs["fields"]
-                    }
-                    updated_attrs["fields"] = [
-                        (
-                            {**f, "value": field_values[f["name"]]}
-                            if f["name"] in field_values
-                            else f
-                        )
-                        for f in api_schema["fields"]
-                    ]
-                remote_attrs = {**api_application.to_dict(), **updated_attrs}
-                application_api.update_applications(
+                prowlarr.ApplicationApi(api_client).update_applications(
                     id=str(api_application.id),
                     application_resource=prowlarr.ApplicationResource.from_dict(remote_attrs),
                 )
             return True
         return False
 
     def _delete_remote(self, tree: str, secrets: ProwlarrSecrets, application_id: int) -> None:
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/apps/sync_profiles.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,22 @@
     def _update_remote(
         self,
         tree: str,
         secrets: ProwlarrSecrets,
         remote: Self,
         api_profile: prowlarr.AppProfileResource,
     ) -> bool:
-        changed, updated_attrs = self.get_update_remote_attrs(
+        changed, set_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
             remote_map=self._remote_map,
+            set_unchanged=True,
         )
         if changed:
-            remote_attrs = {**api_profile.to_dict(), **updated_attrs}
+            remote_attrs = {**api_profile.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
                 prowlarr.AppProfileApi(api_client).update_app_profile(
                     id=str(api_profile.id),
                     app_profile_resource=prowlarr.AppProfileResource.from_dict(remote_attrs),
                 )
             return True
         return False
@@ -178,15 +179,18 @@
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
         # Track whether or not any changes have been made on the remote instance.
         changed = False
         # Pull API objects and metadata required during the update operation.
         with prowlarr_api_client(secrets=secrets) as api_client:
-            api_profiles = prowlarr.AppProfileApi(api_client).list_app_profile()
+            api_profiles: Dict[str, prowlarr.AppProfileResource] = {
+                api_profile.name: api_profile
+                for api_profile in prowlarr.AppProfileApi(api_client).list_app_profile()
+            }
         # Compare local definitions to their remote equivalent.
         # If a local definition does not exist on the remote, create it.
         # If it does exist on the remote, attempt an an in-place modification,
         # and set the `changed` flag if modifications were made.
         for profile_name, profile in self.definitions.items():
             profile_tree = f"{tree}.definitions[{repr(profile_name)}]"
             if profile_name not in remote.definitions:
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/base.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,33 +204,36 @@
         secrets: ProwlarrSecrets,
         remote: Self,
         api_downloadclient_schemas: List[prowlarr.DownloadClientResource],
         category_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
         api_downloadclient: prowlarr.DownloadClientResource,
     ) -> bool:
-        changed, updated_attrs = self.get_update_remote_attrs(
+        changed, set_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
             remote_map=self._get_base_remote_map(category_ids, tag_ids) + self._remote_map,
+            set_unchanged=True,
         )
         if changed:
-            if "fields" in updated_attrs:
+            if "fields" in set_attrs:
                 field_values: Dict[str, Any] = {
-                    field["name"]: field["value"] for field in updated_attrs["fields"]
+                    field["name"]: field["value"] for field in set_attrs["fields"]
                 }
-                updated_attrs["fields"] = [
-                    ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
+                set_attrs["fields"] = [
+                    {**f, "value": field_values[f["name"]]}
                     for f in self._get_api_schema(api_downloadclient_schemas)["fields"]
                 ]
-            remote_attrs = {**api_downloadclient.to_dict(), **updated_attrs}
+            remote_attrs = {**api_downloadclient.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
-                prowlarr.IndexerProxyApi(api_client).update_indexer_proxy(
+                prowlarr.DownloadClientApi(api_client).update_download_client(
                     id=str(api_downloadclient.id),
-                    indexer_proxy_resource=prowlarr.IndexerProxyResource.from_dict(remote_attrs),
+                    download_client_resource=prowlarr.DownloadClientResource.from_dict(
+                        remote_attrs,
+                    ),
                 )
             return True
         return False
 
     def _delete_remote(
         self,
         tree: str,
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/torrent.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/torrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 Prowlarr plugin torrent download client definitions.
 """
 
 
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Dict, List, Literal, Mapping, Optional, Set
+from typing import Any, Dict, List, Literal, Mapping, Optional, Set
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, BaseIntEnum, NonEmptyStr, Password, Port
+from pydantic import validator
 
 from ....types import LowerCaseNonEmptyStr
 from .base import DownloadClient
 
 logger = getLogger(__name__)
 
 
@@ -1059,14 +1060,29 @@
             "directory",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
         ("client_priority", "priority", {"is_field": True}),
         ("add_paused", "addPaused", {"is_field": True}),
     ]
 
+    @validator("directory")
+    def category_directory_mutual_exclusion(
+        cls,
+        value: Optional[str],
+        values: Mapping[str, Any],
+    ) -> Optional[str]:
+        directory = value
+        category: Optional[str] = values.get("category", None)
+        if directory and category:
+            raise ValueError(
+                "'directory' and 'category' are mutually exclusive "
+                "on a Transmission/Vuze download client",
+            )
+        return directory
+
 
 class TransmissionDownloadClient(TransmissionDownloadClientBase):
     """
     Tramsmission download client.
     """
 
     type: Literal["transmission"] = "transmission"
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/download_clients/usenet.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/download_clients/usenet.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/general.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/general.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/__init__.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/indexers.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/indexers.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,27 +211,34 @@
                 raise ValueError(f"field '{name}' defined in both 'fields' and 'secret_fields'")
         return secret_fields
 
     def _get_api_schema(
         self,
         api_indexer_schemas: List[prowlarr.IndexerResource],
     ) -> Dict[str, Any]:
-        return {
-            k: v
-            for k, v in (
-                next(
-                    api_schema
-                    for api_schema in api_indexer_schemas
-                    if api_schema.definition_name.lower() == self.type.lower()
+        try:
+            return {
+                k: v
+                for k, v in (
+                    next(
+                        api_schema
+                        for api_schema in api_indexer_schemas
+                        if api_schema.definition_name.lower() == self.type.lower()
+                    )
+                    .to_dict()
+                    .items()
                 )
-                .to_dict()
-                .items()
-            )
-            if k not in ["id", "name", "added"]
-        }
+                if k not in ["id", "name", "added"]
+            }
+        except StopIteration:
+            expected_types = ", ".join(repr(s.definition_name.lower()) for s in api_indexer_schemas)
+            raise ValueError(
+                f"Invalid 'type' value for indexer '{self.type}' "
+                f"(expected one of: {expected_types})",
+            ) from None
 
     @classmethod
     def _from_remote(
         cls,
         sync_profile_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
         remote_attrs: Mapping[str, Any],
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/indexers/proxies.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/indexers/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,30 +141,30 @@
         tree: str,
         secrets: ProwlarrSecrets,
         remote: Self,
         api_proxy_schemas: List[prowlarr.IndexerProxyResource],
         tag_ids: Mapping[str, int],
         api_proxy: prowlarr.IndexerProxyResource,
     ) -> bool:
-        api_schema = self._get_api_schema(api_proxy_schemas)
-        changed, updated_attrs = self.get_update_remote_attrs(
+        changed, set_attrs = self.get_update_remote_attrs(
             tree=tree,
             remote=remote,
             remote_map=self._get_base_remote_map(tag_ids) + self._remote_map,
+            set_unchanged=True,
         )
         if changed:
-            if "fields" in updated_attrs:
+            if "fields" in set_attrs:
                 field_values: Dict[str, Any] = {
-                    field["name"]: field["value"] for field in updated_attrs["fields"]
+                    field["name"]: field["value"] for field in set_attrs["fields"]
                 }
-                updated_attrs["fields"] = [
-                    ({**f, "value": field_values[f["name"]]} if f["name"] in field_values else f)
-                    for f in api_schema["fields"]
+                set_attrs["fields"] = [
+                    {**f, "value": field_values[f["name"]]}
+                    for f in self._get_api_schema(api_proxy_schemas)["fields"]
                 ]
-            remote_attrs = {**api_proxy.to_dict(), **updated_attrs}
+            remote_attrs = {**api_proxy.to_dict(), **set_attrs}
             with prowlarr_api_client(secrets=secrets) as api_client:
                 prowlarr.IndexerProxyApi(api_client).update_indexer_proxy(
                     id=str(api_proxy.id),
                     indexer_proxy_resource=prowlarr.IndexerProxyResource.from_dict(remote_attrs),
                 )
             return True
         return False
```

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/notifications.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/notifications.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/tags.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/tags.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/settings/ui.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/settings/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/config/types.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/exceptions.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/manager.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/plugin.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/secrets.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/types.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/buildarr_prowlarr/util.py` & `buildarr_prowlarr-0.1.1/buildarr_prowlarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/LICENSE` & `buildarr_prowlarr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/pyproject.toml` & `buildarr_prowlarr-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-prowlarr"
-version = "0.1.0"
+version = "0.1.1"
 description = "Prowlarr indexer manager plugin for Buildarr"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io/plugins/sonarr"
 repository = "https://github.com/buildarr/buildarr-sonarr"
 documentation = "https://buildarr.github.io/plugins/sonarr"
 keywords = [
@@ -40,15 +40,15 @@
 [tool.poetry.plugins."buildarr.plugins"]
 "prowlarr" = "buildarr_prowlarr.plugin:ProwlarrPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 prowlarr-py = ">=0.3.2,<0.4.0"
 buildarr = ">=0.4.0,<0.5.0"
-buildarr-sonarr = {version = ">=0.4.0", optional = true}
+buildarr-sonarr = {version = ">=0.4.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 mypy = "1.2.0"
 types-requests = "2.28.11.17"
 mkdocs = "1.4.2"
 mkdocstrings = {extras = ["python"], version = "0.21.2"}
```

### Comparing `buildarr_prowlarr-0.1.0/README.md` & `buildarr_prowlarr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.1.0/PKG-INFO` & `buildarr_prowlarr-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-prowlarr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prowlarr indexer manager plugin for Buildarr
 Home-page: https://buildarr.github.io/plugins/sonarr
 License: GPL-3.0-or-later
 Keywords: buildarr,prowlarr,lazylibrarian,lidarr,mylar,radarr,readarr,sonarr,whisparr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
 Provides-Extra: sonarr
 Requires-Dist: buildarr (>=0.4.0,<0.5.0)
-Requires-Dist: buildarr-sonarr (>=0.4.0) ; extra == "sonarr"
+Requires-Dist: buildarr-sonarr (>=0.4.1) ; extra == "sonarr"
 Requires-Dist: prowlarr-py (>=0.3.2,<0.4.0)
 Project-URL: Documentation, https://buildarr.github.io/plugins/sonarr
 Project-URL: Repository, https://github.com/buildarr/buildarr-sonarr
 Description-Content-Type: text/markdown
 
 # Buildarr Prowlarr Plugin
```

