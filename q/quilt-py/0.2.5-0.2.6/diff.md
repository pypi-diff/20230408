# Comparing `tmp/quilt_py-0.2.5.tar.gz` & `tmp/quilt_py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quilt_py-0.2.5.tar", max compression
+gzip compressed data, was "quilt_py-0.2.6.tar", max compression
```

## Comparing `quilt_py-0.2.5.tar` & `quilt_py-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        6 2023-03-01 17:17:36.767217 quilt_py-0.2.5/README.md
--rw-r--r--   0        0        0      622 2023-04-05 14:32:41.284819 quilt_py-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      739 2023-03-29 22:05:11.666467 quilt_py-0.2.5/quilt/__init__.py
--rw-r--r--   0        0        0     1226 2023-03-29 22:20:58.486400 quilt_py-0.2.5/quilt/config.py
--rw-r--r--   0        0        0      161 2023-04-04 23:13:40.240939 quilt_py-0.2.5/quilt/context_base/__init__.py
--rw-r--r--   0        0        0     1413 2023-02-26 20:47:23.221097 quilt_py-0.2.5/quilt/context_base/request_manager.py
--rw-r--r--   0        0        0     4398 2023-04-05 15:07:41.886663 quilt_py-0.2.5/quilt/context_base/user_manager.py
--rw-r--r--   0        0        0      894 2023-02-22 22:13:46.914009 quilt_py-0.2.5/quilt/errors.py
--rw-r--r--   0        0        0        0 2023-02-28 23:17:18.661730 quilt_py-0.2.5/quilt/extensions/__init__.py
--rw-r--r--   0        0        0     2536 2023-03-10 00:23:33.299180 quilt_py-0.2.5/quilt/extensions/calls.py
--rw-r--r--   0        0        0      656 2023-02-28 23:20:38.295883 quilt_py-0.2.5/quilt/extensions/mask_errors.py
--rw-r--r--   0        0        0     5204 2023-03-10 00:23:13.749469 quilt_py-0.2.5/quilt/extensions/sentry.py
--rw-r--r--   0        0        0        0 2023-02-16 01:36:16.094733 quilt_py-0.2.5/quilt/gql_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-02-16 01:36:33.862640 quilt_py-0.2.5/quilt/gql_utils/resolvers/__init__.py
--rw-r--r--   0        0        0     2893 2023-02-16 02:03:41.004130 quilt_py-0.2.5/quilt/gql_utils/resolvers/helpers.py
--rw-r--r--   0        0        0     5538 2023-02-28 22:54:33.007480 quilt_py-0.2.5/quilt/gql_utils/resolvers/hydrate.py
--rw-r--r--   0        0        0     1481 2023-02-28 18:35:05.783183 quilt_py-0.2.5/quilt/gql_utils/resolvers/logic.py
--rw-r--r--   0        0        0     4969 2023-02-28 18:24:17.300741 quilt_py-0.2.5/quilt/gql_utils/resolvers/models.py
--rw-r--r--   0        0        0     3212 2023-03-30 20:14:52.530125 quilt_py-0.2.5/quilt/gql_utils/resolvers/startup.py
--rw-r--r--   0        0        0     2306 2023-02-21 22:15:51.366341 quilt_py-0.2.5/quilt/gql_utils/strawberry_utils.py
--rw-r--r--   0        0        0     2761 2023-02-28 02:30:06.521864 quilt_py-0.2.5/quilt/helpers.py
--rw-r--r--   0        0        0     2483 2023-02-28 23:43:32.442836 quilt_py-0.2.5/quilt/logs.py
--rw-r--r--   0        0        0        0 2023-02-28 23:52:18.384266 quilt_py-0.2.5/quilt/middlewares/__init__.py
--rw-r--r--   0        0        0      705 2023-02-28 23:51:42.871147 quilt_py-0.2.5/quilt/middlewares/main.py
--rw-r--r--   0        0        0      333 2023-03-01 00:15:36.825263 quilt_py-0.2.5/quilt/models/__init__.py
--rw-r--r--   0        0        0      895 2023-02-15 22:59:50.014980 quilt_py-0.2.5/quilt/models/image.py
--rw-r--r--   0        0        0     1215 2023-02-15 22:53:17.404819 quilt_py-0.2.5/quilt/models/input_datetime.py
--rw-r--r--   0        0        0     2106 2023-03-01 00:18:57.093892 quilt_py-0.2.5/quilt/models/location/__init__.py
--rw-r--r--   0        0        0      363 2023-02-28 23:58:20.825046 quilt_py-0.2.5/quilt/models/location/queries.py
--rw-r--r--   0        0        0     2264 2023-03-01 16:20:22.425244 quilt_py-0.2.5/quilt/models/phone_number.py
--rw-r--r--   0        0        0    11199 2023-03-09 21:45:18.322425 quilt_py-0.2.5/quilt/plugins/StrawberryFilters/default_filters.py
--rw-r--r--   0        0        0    10919 2023-03-09 20:06:52.217104 quilt_py-0.2.5/quilt/plugins/StrawberryFilters/generator.py
--rw-r--r--   0        0        0     6440 2023-03-01 17:29:02.000000 quilt_py-0.2.5/quilt/plugins/StrawberryFilters/logic.py
--rw-r--r--   0        0        0     1530 2023-03-10 00:17:35.041938 quilt_py-0.2.5/quilt/plugins/StrawberryFilters/mixins.py
--rw-r--r--   0        0        0       38 2023-02-08 20:08:53.856234 quilt_py-0.2.5/quilt/scalars/__init__.py
--rw-r--r--   0        0        0      265 2023-03-01 00:19:45.027572 quilt_py-0.2.5/quilt/scalars/phone_number.py
--rw-r--r--   0        0        0        0 2023-02-08 20:08:53.841842 quilt_py-0.2.5/quilt/services/auth/__init__.py
--rw-r--r--   0        0        0     1252 2023-02-28 23:13:42.662358 quilt_py-0.2.5/quilt/services/auth/logic.py
--rw-r--r--   0        0        0     1167 2023-02-28 23:08:56.113002 quilt_py-0.2.5/quilt/services/auth/routes.py
--rw-r--r--   0        0        0      230 2023-02-28 23:14:31.585735 quilt_py-0.2.5/quilt/services/auth/tests.py
--rw-r--r--   0        0        0      266 2023-02-28 17:20:20.325597 quilt_py-0.2.5/quilt/types.py
--rw-r--r--   0        0        0      295 2023-02-28 23:25:02.984361 quilt_py-0.2.5/quilt/utils.py
--rw-r--r--   0        0        0     1178 2023-02-21 16:53:32.720011 quilt_py-0.2.5/quilt/vendors/Cloudinary/__init__.py
--rw-r--r--   0        0        0      639 2023-02-08 20:08:37.141779 quilt_py-0.2.5/quilt/vendors/Cloudinary/schemas.py
--rw-r--r--   0        0        0      808 2023-02-16 02:06:37.085257 quilt_py-0.2.5/quilt/vendors/Firebase/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:08:53.856627 quilt_py-0.2.5/quilt/vendors/GooglePlaces/__init__.py
--rw-r--r--   0        0        0     3653 2023-03-01 00:16:13.108728 quilt_py-0.2.5/quilt/vendors/GooglePlaces/main.py
--rw-r--r--   0        0        0      802 2023-03-01 00:01:11.153247 quilt_py-0.2.5/quilt/vendors/GooglePlaces/tests/__init__.py
--rw-r--r--   0        0        0     4431 2023-02-28 23:59:18.353088 quilt_py-0.2.5/quilt/vendors/GooglePlaces/tests/example_response.json
--rw-r--r--   0        0        0     1111 2023-02-16 02:24:02.140992 quilt_py-0.2.5/quilt/vendors/IPInfo/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 21:40:23.708710 quilt_py-0.2.5/quilt/vendors/Sentry/__init__.py
--rw-r--r--   0        0        0     1240 2023-02-21 21:42:43.021407 quilt_py-0.2.5/quilt/vendors/Sentry/context_managers.py
--rw-r--r--   0        0        0      758 2023-02-21 21:22:10.849578 quilt_py-0.2.5/quilt/vendors/Sentry/decorators.py
--rw-r--r--   0        0        0        0 2023-02-16 02:06:06.850816 quilt_py-0.2.5/quilt/vendors/__init__.py
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 quilt_py-0.2.5/setup.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 quilt_py-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-03-01 17:17:36.767217 quilt_py-0.2.6/README.md
+-rw-r--r--   0        0        0      622 2023-04-07 22:02:01.535156 quilt_py-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      739 2023-03-29 22:05:11.666467 quilt_py-0.2.6/quilt/__init__.py
+-rw-r--r--   0        0        0     1226 2023-03-29 22:20:58.486400 quilt_py-0.2.6/quilt/config.py
+-rw-r--r--   0        0        0      161 2023-04-04 23:13:40.240939 quilt_py-0.2.6/quilt/context_base/__init__.py
+-rw-r--r--   0        0        0     1413 2023-02-26 20:47:23.221097 quilt_py-0.2.6/quilt/context_base/request_manager.py
+-rw-r--r--   0        0        0     4901 2023-04-07 22:05:01.665230 quilt_py-0.2.6/quilt/context_base/user_manager.py
+-rw-r--r--   0        0        0      894 2023-02-22 22:13:46.914009 quilt_py-0.2.6/quilt/errors.py
+-rw-r--r--   0        0        0        0 2023-02-28 23:17:18.661730 quilt_py-0.2.6/quilt/extensions/__init__.py
+-rw-r--r--   0        0        0     2536 2023-03-10 00:23:33.299180 quilt_py-0.2.6/quilt/extensions/calls.py
+-rw-r--r--   0        0        0      656 2023-02-28 23:20:38.295883 quilt_py-0.2.6/quilt/extensions/mask_errors.py
+-rw-r--r--   0        0        0     5204 2023-03-10 00:23:13.749469 quilt_py-0.2.6/quilt/extensions/sentry.py
+-rw-r--r--   0        0        0        0 2023-02-16 01:36:16.094733 quilt_py-0.2.6/quilt/gql_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-16 01:36:33.862640 quilt_py-0.2.6/quilt/gql_utils/resolvers/__init__.py
+-rw-r--r--   0        0        0     2893 2023-02-16 02:03:41.004130 quilt_py-0.2.6/quilt/gql_utils/resolvers/helpers.py
+-rw-r--r--   0        0        0     5538 2023-02-28 22:54:33.007480 quilt_py-0.2.6/quilt/gql_utils/resolvers/hydrate.py
+-rw-r--r--   0        0        0     1481 2023-02-28 18:35:05.783183 quilt_py-0.2.6/quilt/gql_utils/resolvers/logic.py
+-rw-r--r--   0        0        0     4969 2023-02-28 18:24:17.300741 quilt_py-0.2.6/quilt/gql_utils/resolvers/models.py
+-rw-r--r--   0        0        0     3212 2023-03-30 20:14:52.530125 quilt_py-0.2.6/quilt/gql_utils/resolvers/startup.py
+-rw-r--r--   0        0        0     2306 2023-02-21 22:15:51.366341 quilt_py-0.2.6/quilt/gql_utils/strawberry_utils.py
+-rw-r--r--   0        0        0     2761 2023-02-28 02:30:06.521864 quilt_py-0.2.6/quilt/helpers.py
+-rw-r--r--   0        0        0     2483 2023-02-28 23:43:32.442836 quilt_py-0.2.6/quilt/logs.py
+-rw-r--r--   0        0        0        0 2023-02-28 23:52:18.384266 quilt_py-0.2.6/quilt/middlewares/__init__.py
+-rw-r--r--   0        0        0      705 2023-02-28 23:51:42.871147 quilt_py-0.2.6/quilt/middlewares/main.py
+-rw-r--r--   0        0        0      333 2023-03-01 00:15:36.825263 quilt_py-0.2.6/quilt/models/__init__.py
+-rw-r--r--   0        0        0      895 2023-02-15 22:59:50.014980 quilt_py-0.2.6/quilt/models/image.py
+-rw-r--r--   0        0        0     1215 2023-02-15 22:53:17.404819 quilt_py-0.2.6/quilt/models/input_datetime.py
+-rw-r--r--   0        0        0     2106 2023-03-01 00:18:57.093892 quilt_py-0.2.6/quilt/models/location/__init__.py
+-rw-r--r--   0        0        0      363 2023-02-28 23:58:20.825046 quilt_py-0.2.6/quilt/models/location/queries.py
+-rw-r--r--   0        0        0     2264 2023-03-01 16:20:22.425244 quilt_py-0.2.6/quilt/models/phone_number.py
+-rw-r--r--   0        0        0    11199 2023-03-09 21:45:18.322425 quilt_py-0.2.6/quilt/plugins/StrawberryFilters/default_filters.py
+-rw-r--r--   0        0        0    10919 2023-03-09 20:06:52.217104 quilt_py-0.2.6/quilt/plugins/StrawberryFilters/generator.py
+-rw-r--r--   0        0        0     6440 2023-03-01 17:29:02.000000 quilt_py-0.2.6/quilt/plugins/StrawberryFilters/logic.py
+-rw-r--r--   0        0        0     1530 2023-03-10 00:17:35.041938 quilt_py-0.2.6/quilt/plugins/StrawberryFilters/mixins.py
+-rw-r--r--   0        0        0       38 2023-02-08 20:08:53.856234 quilt_py-0.2.6/quilt/scalars/__init__.py
+-rw-r--r--   0        0        0      265 2023-03-01 00:19:45.027572 quilt_py-0.2.6/quilt/scalars/phone_number.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:08:53.841842 quilt_py-0.2.6/quilt/services/auth/__init__.py
+-rw-r--r--   0        0        0     1252 2023-02-28 23:13:42.662358 quilt_py-0.2.6/quilt/services/auth/logic.py
+-rw-r--r--   0        0        0     1167 2023-02-28 23:08:56.113002 quilt_py-0.2.6/quilt/services/auth/routes.py
+-rw-r--r--   0        0        0      230 2023-02-28 23:14:31.585735 quilt_py-0.2.6/quilt/services/auth/tests.py
+-rw-r--r--   0        0        0      266 2023-02-28 17:20:20.325597 quilt_py-0.2.6/quilt/types.py
+-rw-r--r--   0        0        0      295 2023-02-28 23:25:02.984361 quilt_py-0.2.6/quilt/utils.py
+-rw-r--r--   0        0        0     1178 2023-02-21 16:53:32.720011 quilt_py-0.2.6/quilt/vendors/Cloudinary/__init__.py
+-rw-r--r--   0        0        0      639 2023-02-08 20:08:37.141779 quilt_py-0.2.6/quilt/vendors/Cloudinary/schemas.py
+-rw-r--r--   0        0        0      808 2023-02-16 02:06:37.085257 quilt_py-0.2.6/quilt/vendors/Firebase/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:08:53.856627 quilt_py-0.2.6/quilt/vendors/GooglePlaces/__init__.py
+-rw-r--r--   0        0        0     3653 2023-03-01 00:16:13.108728 quilt_py-0.2.6/quilt/vendors/GooglePlaces/main.py
+-rw-r--r--   0        0        0      802 2023-03-01 00:01:11.153247 quilt_py-0.2.6/quilt/vendors/GooglePlaces/tests/__init__.py
+-rw-r--r--   0        0        0     4431 2023-02-28 23:59:18.353088 quilt_py-0.2.6/quilt/vendors/GooglePlaces/tests/example_response.json
+-rw-r--r--   0        0        0     1111 2023-02-16 02:24:02.140992 quilt_py-0.2.6/quilt/vendors/IPInfo/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-21 21:40:23.708710 quilt_py-0.2.6/quilt/vendors/Sentry/__init__.py
+-rw-r--r--   0        0        0     1240 2023-02-21 21:42:43.021407 quilt_py-0.2.6/quilt/vendors/Sentry/context_managers.py
+-rw-r--r--   0        0        0      758 2023-02-21 21:22:10.849578 quilt_py-0.2.6/quilt/vendors/Sentry/decorators.py
+-rw-r--r--   0        0        0        0 2023-02-16 02:06:06.850816 quilt_py-0.2.6/quilt/vendors/__init__.py
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 quilt_py-0.2.6/setup.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 quilt_py-0.2.6/PKG-INFO
```

### Comparing `quilt_py-0.2.5/pyproject.toml` & `quilt_py-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quilt-py"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{include = "quilt"}]
 exclude = ["tests/**/*"]
```

### Comparing `quilt_py-0.2.5/quilt/__init__.py` & `quilt_py-0.2.6/quilt/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/config.py` & `quilt_py-0.2.6/quilt/config.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/context_base/request_manager.py` & `quilt_py-0.2.6/quilt/context_base/request_manager.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/context_base/user_manager.py` & `quilt_py-0.2.6/quilt/context_base/user_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,32 +108,47 @@
     async def get(
         self,
         given_resolver: T.Optional[UserResolverType] = None,
         *,
         refresh: T.Optional[bool] = False,
         include_properties: T.Optional[bool] = True,
         include_permissions: T.Optional[bool] = True,
-        gerror: T.Optional[bool] = True,
         client: T.Optional[AsyncIOClient] = None,
     ) -> UserType | None:
         if refresh:
             self._user = UNSET
         if self._user is not UNSET:
             return self._user
         if not self.auth_id:
             return None
         resolver = given_resolver or self.default_resolver_function()
         if include_properties:
             self.default_include_properties_function(resolver)
         if include_permissions:
             resolver.include_fields("permissions")
-        func = resolver.gerror if gerror else resolver.get
+        self._user = await resolver.get(
+            **{self.auth_id_field_name: self.auth_id, "client": client}
+        )
+        return self._user
+
+    async def gerror(
+        self,
+        given_resolver: T.Optional[UserResolverType] = None,
+        *,
+        refresh: T.Optional[bool] = False,
+        include_properties: T.Optional[bool] = True,
+        include_permissions: T.Optional[bool] = True,
+        client: T.Optional[AsyncIOClient] = None,
+    ) -> UserType | None:
         try:
-            self._user = await func(
-                **{self.auth_id_field_name: self.auth_id, "client": client}
+            return await self.get(
+                given_resolver=given_resolver,
+                refresh=refresh,
+                include_properties=include_properties,
+                include_permissions=include_permissions,
+                client=client,
             )
         except edge_orm.ResolverException:
             raise UserManagerException("Please create an account to access.")
-        return self._user
 
     def set(self, user: UserType | None) -> None:
         self._user = user
```

### Comparing `quilt_py-0.2.5/quilt/errors.py` & `quilt_py-0.2.6/quilt/errors.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/extensions/calls.py` & `quilt_py-0.2.6/quilt/extensions/calls.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/extensions/mask_errors.py` & `quilt_py-0.2.6/quilt/extensions/mask_errors.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/extensions/sentry.py` & `quilt_py-0.2.6/quilt/extensions/sentry.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/resolvers/helpers.py` & `quilt_py-0.2.6/quilt/gql_utils/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/resolvers/hydrate.py` & `quilt_py-0.2.6/quilt/gql_utils/resolvers/hydrate.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/resolvers/logic.py` & `quilt_py-0.2.6/quilt/gql_utils/resolvers/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/resolvers/models.py` & `quilt_py-0.2.6/quilt/gql_utils/resolvers/models.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/resolvers/startup.py` & `quilt_py-0.2.6/quilt/gql_utils/resolvers/startup.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/gql_utils/strawberry_utils.py` & `quilt_py-0.2.6/quilt/gql_utils/strawberry_utils.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/helpers.py` & `quilt_py-0.2.6/quilt/helpers.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/logs.py` & `quilt_py-0.2.6/quilt/logs.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/middlewares/main.py` & `quilt_py-0.2.6/quilt/middlewares/main.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/models/image.py` & `quilt_py-0.2.6/quilt/models/image.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/models/input_datetime.py` & `quilt_py-0.2.6/quilt/models/input_datetime.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/models/location/__init__.py` & `quilt_py-0.2.6/quilt/models/location/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/models/phone_number.py` & `quilt_py-0.2.6/quilt/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/plugins/StrawberryFilters/default_filters.py` & `quilt_py-0.2.6/quilt/plugins/StrawberryFilters/default_filters.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/plugins/StrawberryFilters/generator.py` & `quilt_py-0.2.6/quilt/plugins/StrawberryFilters/generator.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/plugins/StrawberryFilters/logic.py` & `quilt_py-0.2.6/quilt/plugins/StrawberryFilters/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/plugins/StrawberryFilters/mixins.py` & `quilt_py-0.2.6/quilt/plugins/StrawberryFilters/mixins.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/services/auth/logic.py` & `quilt_py-0.2.6/quilt/services/auth/logic.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/services/auth/routes.py` & `quilt_py-0.2.6/quilt/services/auth/routes.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/Cloudinary/__init__.py` & `quilt_py-0.2.6/quilt/vendors/Cloudinary/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/Cloudinary/schemas.py` & `quilt_py-0.2.6/quilt/vendors/Cloudinary/schemas.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/Firebase/__init__.py` & `quilt_py-0.2.6/quilt/vendors/Firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/GooglePlaces/main.py` & `quilt_py-0.2.6/quilt/vendors/GooglePlaces/main.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/GooglePlaces/tests/__init__.py` & `quilt_py-0.2.6/quilt/vendors/GooglePlaces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/GooglePlaces/tests/example_response.json` & `quilt_py-0.2.6/quilt/vendors/GooglePlaces/tests/example_response.json`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/IPInfo/__init__.py` & `quilt_py-0.2.6/quilt/vendors/IPInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/Sentry/context_managers.py` & `quilt_py-0.2.6/quilt/vendors/Sentry/context_managers.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/quilt/vendors/Sentry/decorators.py` & `quilt_py-0.2.6/quilt/vendors/Sentry/decorators.py`

 * *Files identical despite different names*

### Comparing `quilt_py-0.2.5/setup.py` & `quilt_py-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'phonenumbers',
  'pydantic[email]',
  'sentry-sdk[httpx,pure-eval]>=1.15,<2.0',
  'strawberry-graphql']
 
 setup_kwargs = {
     'name': 'quilt-py',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': '',
     'long_description': 'hello!',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quilt_py-0.2.5/PKG-INFO` & `quilt_py-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt-py
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: devtools
```

