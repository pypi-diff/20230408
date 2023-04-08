# Comparing `tmp/manifest-ml-0.1.1.tar.gz` & `tmp/manifest-ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.1.tar", last modified: Mon Jan 30 23:54:04 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.2.tar", last modified: Sat Apr  8 21:13:25 2023, max compression
```

## Comparing `manifest-ml-0.1.1.tar` & `manifest-ml-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,62 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.112446 manifest-ml-0.1.1/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)     7994 2023-01-30 23:54:04.112327 manifest-ml-0.1.1/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     7309 2023-01-30 23:48:13.000000 manifest-ml-0.1.1/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.107064 manifest-ml-0.1.1/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      220 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.107587 manifest-ml-0.1.1/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8045 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.108259 manifest-ml-0.1.1/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3905 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    22012 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2583 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1500 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.109384 manifest-ml-0.1.1/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3368 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3825 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.111032 manifest-ml-0.1.1/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3291 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3619 2023-01-30 23:48:04.000000 manifest-ml-0.1.1/manifest/clients/chatgpt.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5087 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3449 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2776 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3411 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3407 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2983 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5153 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1935 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/clients/toma_diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    11568 2023-01-30 23:48:13.000000 manifest-ml-0.1.1/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2180 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6590 2023-01-28 05:51:03.000000 manifest-ml-0.1.1/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4755 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/manifest/session.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-01-30 23:53:10.000000 manifest-ml-0.1.1/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.111729 manifest-ml-0.1.1/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)     7994 2023-01-30 23:54:03.000000 manifest-ml-0.1.1/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1090 2023-01-30 23:54:04.000000 manifest-ml-0.1.1/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-01-30 23:54:03.000000 manifest-ml-0.1.1/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1428 2023-01-30 23:54:04.000000 manifest-ml-0.1.1/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-01-30 23:54:04.000000 manifest-ml-0.1.1/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      759 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-01-30 23:54:04.112490 manifest-ml-0.1.1/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5173 2023-01-30 23:53:55.000000 manifest-ml-0.1.1/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-01-30 23:54:04.112115 manifest-ml-0.1.1/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1733 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-01-27 08:09:04.000000 manifest-ml-0.1.1/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.651185 manifest-ml-0.1.2/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6955 2023-04-08 21:13:25.651064 manifest-ml-0.1.2/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6267 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.643382 manifest-ml-0.1.2/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.643922 manifest-ml-0.1.2/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8339 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.644859 manifest-ml-0.1.2/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3991 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    22438 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2839 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1612 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.646159 manifest-ml-0.1.2/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3420 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3825 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.648139 manifest-ml-0.1.2/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3298 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11662 2023-04-08 20:45:20.000000 manifest-ml-0.1.2/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3458 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2780 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3738 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3424 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3966 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5109 2023-04-08 20:44:48.000000 manifest-ml-0.1.2/manifest/clients/openaichat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5159 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1943 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/toma_diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    17517 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2730 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     7351 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-08 19:58:13.000000 manifest-ml-0.1.2/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.648727 manifest-ml-0.1.2/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6955 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1291 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1557 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      759 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-08 21:13:25.651229 manifest-ml-0.1.2/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5309 2023-04-08 20:03:25.000000 manifest-ml-0.1.2/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.650443 manifest-ml-0.1.2/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6833 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2053 2023-04-08 20:44:48.000000 manifest-ml-0.1.2/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8101 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    25170 2023-04-08 20:44:57.000000 manifest-ml-0.1.2/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5756 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      531 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.650864 manifest-ml-0.1.2/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1733 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.1/LICENSE` & `manifest-ml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/PKG-INFO` & `manifest-ml-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
-Author-email: lorr1@cs.stanford.edu
+Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: app
-Provides-Extra: chatgpt
 Provides-Extra: diffusers
+Provides-Extra: gcp
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
@@ -42,20 +42,14 @@
 ```
 
 Install with diffusion support:
 ```bash
 pip install manifest-ml[diffusers]
 ```
 
-Install with ChatGPT support:
-```bash
-pip install manifest-ml[chatgpt]
-```
-This installs [pyChatGPT](https://github.com/terry3041/pyChatGPT) and uses the ChatGPT session key to start a session. This key must be set as the `CHATGPT_SESSION_KEY` environment variable or passed in with `client_connection`.
-
 Install with HuggingFace local model support:
 ```bash
 pip install manifest-ml[api]
 ```
 
 Dev Install:
 ```bash
@@ -126,32 +120,14 @@
     client_name = "openai",
     cache_name = "redis",
     cache_connection = "localhost:6379"
 )
 ```
 As a hint, if you want to get Redis running, see the `docker run` command below under development.
 
-## Sessions
-Each Manifest run supports a session that, in addition to a global cache, connects to a local SQLite DB to store user query history.
-```python
-manifest = Manifest(
-    client_name = "openai",
-    cache_name = "sqlite",
-    cache_connection = "mycache.sqlite",
-    session_id = "grass_color",
-)
-```
-will start a Manifest session with the session name `grass_color`. This can be helpful for a user to logically keep track of sessions, see interaction history, and resume sessions if desired. If the session id provided is `_default`, we generate a random id for the user.
-
-After a few queries, the user can explore their history
-```python
-manifest.get_last_queries(4)
-```
-will retrieve the last 4 model queries and responses.
-
 ## Running Queries
 Once you have a session open, you can write and develop prompts.
 
 ```python
 result = manifest.run("Hello, my name is Laurel")
 ```
```

### Comparing `manifest-ml-0.1.1/README.md` & `manifest-ml-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,14 @@
 ```
 
 Install with diffusion support:
 ```bash
 pip install manifest-ml[diffusers]
 ```
 
-Install with ChatGPT support:
-```bash
-pip install manifest-ml[chatgpt]
-```
-This installs [pyChatGPT](https://github.com/terry3041/pyChatGPT) and uses the ChatGPT session key to start a session. This key must be set as the `CHATGPT_SESSION_KEY` environment variable or passed in with `client_connection`.
-
 Install with HuggingFace local model support:
 ```bash
 pip install manifest-ml[api]
 ```
 
 Dev Install:
 ```bash
@@ -102,32 +96,14 @@
     client_name = "openai",
     cache_name = "redis",
     cache_connection = "localhost:6379"
 )
 ```
 As a hint, if you want to get Redis running, see the `docker run` command below under development.
 
-## Sessions
-Each Manifest run supports a session that, in addition to a global cache, connects to a local SQLite DB to store user query history.
-```python
-manifest = Manifest(
-    client_name = "openai",
-    cache_name = "sqlite",
-    cache_connection = "mycache.sqlite",
-    session_id = "grass_color",
-)
-```
-will start a Manifest session with the session name `grass_color`. This can be helpful for a user to logically keep track of sessions, see interaction history, and resume sessions if desired. If the session id provided is `_default`, we generate a random id for the user.
-
-After a few queries, the user can explore their history
-```python
-manifest.get_last_queries(4)
-```
-will retrieve the last 4 model queries and responses.
-
 ## Running Queries
 Once you have a session open, you can write and develop prompts.
 
 ```python
 result = manifest.run("Hello, my name is Laurel")
 ```
```

### Comparing `manifest-ml-0.1.1/manifest/api/app.py` & `manifest-ml-0.1.2/manifest/api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,18 +169,24 @@
         raise ValueError("Prompt must be a str or list of str")
     try:
         result_gens = []
         for generations in model.generate(prompt, **generation_args):
             result_gens.append(generations)
         if model_type == "diffuser":
             # Assign None logprob as it's not supported in diffusers
-            results = [{"array": r[0], "logprob": None} for r in result_gens]
+            results = [
+                {"array": r[0], "logprob": None, "tokens": None, "token_logprobs": None}
+                for r in result_gens
+            ]
             res_type = "image_generation"
         else:
-            results = [{"text": r[0], "logprob": r[1]} for r in result_gens]
+            results = [
+                {"text": r[0], "logprob": r[1], "tokens": r[2], "token_logprobs": r[3]}
+                for r in result_gens
+            ]
             res_type = "text_completion"
         # transform the result into the openai format
         return Response(
             json.dumps(ModelResponse(results, response_type=res_type).__dict__()),
             status=200,
         )
     except Exception as e:
@@ -228,15 +234,20 @@
 
     if not isinstance(prompt, (str, list)):
         raise ValueError("Prompt must be a str or list of str")
 
     try:
         score_list = model.score_sequence(prompt, **generation_args)
         results = [
-            {"text": prompt if isinstance(prompt, str) else prompt[i], "logprob": r}
+            {
+                "text": prompt if isinstance(prompt, str) else prompt[i],
+                "logprob": r[0],
+                "tokens": r[1],
+                "token_logprobs": r[2],
+            }
             for i, r in enumerate(score_list)
         ]
         # transform the result into the openai format
         return Response(
             json.dumps(
                 ModelResponse(results, response_type="prompt_logit_score").__dict__()
             ),
```

### Comparing `manifest-ml-0.1.1/manifest/api/models/diffuser.py` & `manifest-ml-0.1.2/manifest/api/models/diffuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def get_init_params(self) -> Dict:
         """Return init params to determine what model is being used."""
         return {"model_name": self.model_name, "model_path": self.model_path}
 
     @torch.no_grad()
     def generate(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[Tuple[Any, float]]:
+    ) -> List[Tuple[Any, float, List[int], List[float]]]:
         """
         Generate the prompt from model.
 
         Outputs must be generated text and score, not including prompt.
 
         Args:
             prompt: promt to generate from.
@@ -86,21 +86,21 @@
         Returns:
             list of generated text (list of length 1 for 1 generation).
         """
         # TODO: Is this correct for getting arguments in?
         if isinstance(prompt, str):
             prompt = [prompt]
         result = self.pipeline(prompt, output_type="np.array", **kwargs)
-        # Return None for logprobs
-        return [(im, None) for im in result["images"]]
+        # Return None for logprobs and token logprobs
+        return [(im, None, None, None) for im in result["images"]]
 
     @torch.no_grad()
     def score_sequence(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[float]:
+    ) -> List[Tuple[float, List[int], List[float]]]:
         """
         Score a sequence of choices.
 
         Args:
             prompt (:obj:`str` or :obj:`List[str]`):
                 The prompt to score the choices against.
             **kwargs:
```

### Comparing `manifest-ml-0.1.1/manifest/api/models/huggingface.py` & `manifest-ml-0.1.2/manifest/api/models/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,14 +175,15 @@
             {
                 "generated_text": self.tokenizer.decode(
                     output_seq[-num_generated_tokens:], skip_special_tokens=True
                 ),
                 "logprobs": logits[
                     range(num_generated_tokens), i, output_seq[-num_generated_tokens:]
                 ].tolist(),
+                "tokens": output_seq[-num_generated_tokens:].tolist(),
             }
             for i, output_seq in enumerate(output_dict.sequences)
         ]
         return generated_sequences
 
 
 class HuggingFaceModel(Model):
@@ -543,15 +544,15 @@
             embedding
         """
         pass
 
     @torch.no_grad()
     def generate(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[Tuple[Any, float]]:
+    ) -> List[Tuple[Any, float, List[int], List[float]]]:
         """
         Generate the prompt from model.
 
         Outputs must be generated text and score, not including prompt.
 
         Args:
             prompt: promt to generate from.
@@ -569,23 +570,28 @@
             repetition_penalty=kwargs.get("repetition_penalty"),
             top_k=kwargs.get("top_k"),
             top_p=kwargs.get("top_p"),
             do_sample=kwargs.get("do_sample"),
             num_return_sequences=num_return,
         )
         final_results = [
-            (cast(str, r["generated_text"]), sum(cast(List[float], r["logprobs"])))
+            (
+                cast(str, r["generated_text"]),
+                sum(cast(List[float], r["logprobs"])),
+                cast(List[int], r["tokens"]),
+                cast(List[float], r["logprobs"]),
+            )
             for r in result
         ]
         return final_results
 
     @torch.no_grad()
     def score_sequence(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[float]:
+    ) -> List[Tuple[float, List[int], List[float]]]:
         """
         Score a sequence of choices.
 
         Args:
             prompt (:obj:`str` or :obj:`List[str]`):
                 The prompt to score the choices against.
             **kwargs:
@@ -602,20 +608,24 @@
         )
         encoded_prompt["labels"] = encoded_prompt["input_ids"].clone()
         encoded_prompt = encoded_prompt.to(self.pipeline.device)
         logits = self.pipeline.model(  # type: ignore
             **encoded_prompt,
         ).logits
         # For causal decoders, shift logts and labels
-        labels_attention_mask = encoded_prompt["attention_mask"].unsqueeze(-1)[
-            ..., 1:, :
-        ]
-        masked_log_probs = (
-            labels_attention_mask.float()
-            * torch.log_softmax(logits.float(), dim=-1)[..., :-1, :]
+        labels_attention_mask = encoded_prompt["attention_mask"].unsqueeze(-1)
+        masked_log_probs = labels_attention_mask.float() * torch.log_softmax(
+            logits.float(), dim=-1
         )
         seq_token_log_probs = torch.gather(
-            masked_log_probs, -1, encoded_prompt["labels"][..., 1:].unsqueeze(-1)
+            masked_log_probs, -1, encoded_prompt["labels"].unsqueeze(-1)
         )
         seq_token_log_probs = seq_token_log_probs.squeeze(dim=-1)
         seq_log_prob = seq_token_log_probs.sum(dim=-1)
-        return seq_log_prob.tolist()
+        return [
+            (seq, tokens, seq_token)
+            for seq, tokens, seq_token in zip(
+                seq_log_prob.tolist(),
+                encoded_prompt["input_ids"].tolist(),
+                seq_token_log_probs.tolist(),
+            )
+        ]
```

### Comparing `manifest-ml-0.1.1/manifest/api/models/model.py` & `manifest-ml-0.1.2/manifest/api/models/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,25 +44,27 @@
     @abstractmethod
     def get_init_params(self) -> Dict:
         """Return init params to determine what model is being used."""
         raise NotImplementedError()
 
     def generate(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[Tuple[Any, float]]:
+    ) -> List[Tuple[Any, float, List[int], List[float]]]:
         """
         Generate the prompt from model.
 
         Outputs must be generated text and score, not including prompt.
 
         Args:
             prompt: promt to generate from.
 
         Returns:
             list of generated text (list of length 1 for 1 generation).
+            Each item is the response, answer logprob, list of tokens,
+            and list of logprobs for each token.
         """
         raise NotImplementedError()
 
     def embed(self, prompt: Union[str, List[str]], **kwargs: Any) -> np.ndarray:
         """
         Compute embedding for prompts.
 
@@ -72,18 +74,21 @@
         Returns:
             embedding
         """
         raise NotImplementedError()
 
     def score_sequence(
         self, prompt: Union[str, List[str]], **kwargs: Any
-    ) -> List[float]:
+    ) -> List[Tuple[float, List[int], List[float]]]:
         """
         Score a sequence of choices.
 
         Args:
             prompt (:obj:`str` or :obj:`List[str]`):
                 The prompt to score the choices against.
             **kwargs:
                 Additional keyword arguments passed along to the :obj:`__call__` method.
+
+        Returns:
+            Tuple of total score, tokens, and probs per token.
         """
         raise NotImplementedError()
```

### Comparing `manifest-ml-0.1.1/manifest/api/response.py` & `manifest-ml-0.1.2/manifest/api/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,16 @@
             "object": self.response_type,
             "created": self.created,
             "model": "flask_model",
             "choices": [
                 {
                     key: result[key],
                     "logprob": result["logprob"],
+                    "tokens": result["tokens"],
+                    "token_logprobs": result["token_logprobs"],
                 }
                 if key == "text"
                 else {
                     key: result[key].tolist(),
                     "logprob": result["logprob"],
                 }
                 for result in self.results
```

### Comparing `manifest-ml-0.1.1/manifest/caches/array_cache.py` & `manifest-ml-0.1.2/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/manifest/caches/cache.py` & `manifest-ml-0.1.2/manifest/caches/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,13 @@
 """Cache for queries and responses."""
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Union
+from typing import Any, Dict, Union
 
 from manifest.caches.serializers import ArraySerializer, Serializer
-from manifest.response import Response
-
-RESPONSE_CONSTRUCTORS = {
-    "diffuser": {
-        "generation_key": "choices",
-        "logits_key": "logprobs",
-        "item_key": "array",
-    },
-    "tomadiffuser": {
-        "generation_key": "choices",
-        "logits_key": "logprobs",
-        "item_key": "array",
-    },
-}
+from manifest.response import RESPONSE_CONSTRUCTORS, Response
 
 CACHE_CONSTRUCTOR = {
     "diffuser": ArraySerializer,
     "tomadiffuser": ArraySerializer,
 }
 
 
@@ -97,24 +84,39 @@
         raise NotImplementedError()
 
     @abstractmethod
     def commit(self) -> None:
         """Commit any results."""
         raise NotImplementedError()
 
-    def get(
-        self, request: Dict, overwrite_cache: bool, compute: Callable[[], Dict]
-    ) -> Response:
-        """Get the result of request (by calling compute as needed)."""
+    def get(self, request: Dict) -> Union[Response, None]:
+        """Get the result of request (by calling compute as needed).
+
+        Args:
+            request: request to get.
+            response: response to get.
+
+        Returns:
+            Response object or None if not in cache.
+        """
         key = self.serializer.request_to_key(request)
         cached_response = self.get_key(key)
-        if cached_response and not overwrite_cache:
+        if cached_response:
             cached = True
             response = self.serializer.key_to_response(cached_response)
-        else:
-            # Type Response
-            response = compute()
-            self.set_key(key, self.serializer.response_to_key(response))
-            cached = False
-        return Response(
-            response, cached, request, **RESPONSE_CONSTRUCTORS.get(self.client_name, {})
-        )
+            return Response(
+                response,
+                cached,
+                request,
+                **RESPONSE_CONSTRUCTORS.get(self.client_name, {})
+            )
+        return None
+
+    def set(self, request: Dict, response: Dict) -> None:
+        """Set the value for the key.
+
+        Args:
+            request: request to set.
+            response: response to set.
+        """
+        key = self.serializer.request_to_key(request)
+        self.set_key(key, self.serializer.response_to_key(response))
```

### Comparing `manifest-ml-0.1.1/manifest/caches/noop.py` & `manifest-ml-0.1.2/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/manifest/caches/redis.py` & `manifest-ml-0.1.2/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/manifest/caches/serializers.py` & `manifest-ml-0.1.2/manifest/caches/serializers.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/manifest/caches/sqlite.py` & `manifest-ml-0.1.2/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/manifest/clients/ai21.py` & `manifest-ml-0.1.2/manifest/clients/ai21.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         "engine": ("engine", "j1-large"),
         "temperature": ("temperature", 1.0),
         "max_tokens": ("maxTokens", 10),
         "top_k": ("topKReturn", 0),
         "n": ("numResults", 1),
         "top_p": ("topP", 1.0),
         "stop_sequences": ("stopSequences", []),
-        "client_timeout": ("client_timeout", 60),  # seconds
     }
     REQUEST_CLS = LMRequest
+    NAME = "ai21"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
@@ -90,28 +90,29 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": "ai21", "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
+            request: request
 
         Return:
             response as dict
         """
         return {
             "object": "text_completion",
             "model": getattr(self, "engine"),
             "choices": [
                 {
                     "text": item["data"]["text"],
-                    "logprobs": item["data"]["tokens"],
+                    "token_logprobs": item["data"]["tokens"],
                 }
                 for item in response["completions"]
             ],
         }
```

### Comparing `manifest-ml-0.1.1/manifest/clients/chatgpt.py` & `manifest-ml-0.1.2/manifest/clients/huggingface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,118 @@
-"""Client class."""
+"""Hugging Face client."""
 import logging
-import os
-from typing import Any, Callable, Dict, Optional, Tuple
+from typing import Any, Dict, Optional
 
-from pyChatGPT import ChatGPT
+import requests
 
 from manifest.clients.client import Client
-from manifest.request import LMRequest, Request
+from manifest.request import DEFAULT_REQUEST_KEYS, LMRequest, Request
+from manifest.response import Response
 
 logger = logging.getLogger(__name__)
 
 
-class ChatGPTClient(Client):
-    """ChatGPT Client class."""
+class HuggingFaceClient(Client):
+    """HuggingFace client."""
 
-    # No params for ChatGPT
-    PARAMS: Dict[str, Tuple[str, Any]] = {}
+    # User param -> (client param, default value)
+    PARAMS = {
+        "temperature": ("temperature", 1.0),
+        "max_tokens": ("max_tokens", 10),
+        "n": ("n", 1),
+        "top_p": ("top_p", 1.0),
+        "top_k": ("top_k", 50),
+        "repetition_penalty": ("repetition_penalty", 1.0),
+        "do_sample": ("do_sample", True),
+    }
     REQUEST_CLS = LMRequest
+    NAME = "huggingface"
 
     def connect(
-        self, connection_str: Optional[str], client_args: Dict[str, Any]
+        self,
+        connection_str: Optional[str] = None,
+        client_args: Dict[str, Any] = {},
     ) -> None:
         """
-        Connect to ChatGPT.
-
-        We use https://github.com/terry3041/pyChatGPT.
+        Connect to the HuggingFace url.
 
         Arsg:
             connection_str: connection string.
             client_args: client arguments.
         """
-        self.session_key = os.environ.get("CHATGPT_SESSION_KEY", connection_str)
-        if self.session_key is None:
-            raise ValueError(
-                "ChatGPT session key not set. Set CHATGPT_SESSION_KEY environment "
-                "variable or pass through `client_connection`. "
-                "For details, see https://github.com/terry3041/pyChatGPT "
-                "and go through instructions for getting a session key."
-            )
-        self.host = None
+        if not connection_str:
+            raise ValueError("Must provide connection string")
+        self.host = connection_str.rstrip("/")
         for key in self.PARAMS:
             setattr(self, key, client_args.pop(key, self.PARAMS[key][1]))
-        self._chat_session = ChatGPT(self.session_key, verbose=False)
 
     def close(self) -> None:
         """Close the client."""
-        self._chat_session = None
-
-    def clear_conversations(self) -> None:
-        """Clear conversations.
-
-        Only works for ChatGPT.
-        """
-        self._chat_session.clear_conversations()
+        pass
 
     def get_generation_url(self) -> str:
         """Get generation URL."""
-        return ""
+        return self.host + "/completions"
 
     def get_generation_header(self) -> Dict[str, str]:
         """
         Get generation header.
 
         Returns:
             header.
         """
         return {}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
-        return False
+        return True
 
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "chatgpt", "engine": "chatgpt"}
+        res = requests.post(self.host + "/params")
+        return res.json()
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def get_score_prompt_request(
+        self,
+        request: Request,
+    ) -> Response:
         """
-        Format response to dict.
-
-        Args:
-            response: response
-
-        Return:
-            response as dict
-        """
-        return {
-            "model": "chatgpt",
-            "choices": [
-                {
-                    "text": response["message"],
-                }
-            ],
-        }
-
-    def get_request(self, request: Request) -> Tuple[Callable[[], Dict], Dict]:
-        """
-        Get request string function.
+        Get the logit score of the prompt via a forward pass of the model.
 
         Args:
             request: request.
 
         Returns:
             request function that takes no input.
             request parameters as dict.
         """
-        if isinstance(request.prompt, list):
-            raise ValueError("ChatGPT does not support batch inference.")
-
-        prompt = str(request.prompt)
-        request_params = request.to_dict(self.PARAMS)
-
-        def _run_completion() -> Dict:
-            try:
-                res = self._chat_session.send_message(prompt)
-            except Exception as e:
-                logger.error(f"ChatGPT error {e}.")
-                raise e
-            return self.format_response(res)
-
-        return _run_completion, request_params
+        request_params = self.get_request_params(request)
+        retry_timeout = request_params.pop("client_timeout")
+        for key in DEFAULT_REQUEST_KEYS:
+            request_params.pop(key, None)
+        # Do not add params like we do with request as the model isn't sampling
+        request_params = {"prompt": request.prompt}
+
+        post_str = self.host + "/score_sequence"
+        try:
+            res = requests.post(
+                post_str,
+                json=request_params,
+                timeout=retry_timeout,
+            )
+            res.raise_for_status()
+        except requests.Timeout as e:
+            logger.error("HF request timed out. Increase client_timeout.")
+            raise e
+        except requests.exceptions.HTTPError as e:
+            logger.error(res.text)
+            raise e
+        response_dict = res.json()
+        return Response(response_dict, cached=False, request_params=request_params)
```

### Comparing `manifest-ml-0.1.1/manifest/clients/cohere.py` & `manifest-ml-0.1.2/manifest/clients/cohere.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         "temperature": ("temperature", 0.75),
         "n": ("num_generations", 1),
         "top_k": ("k", 0),
         "top_p": ("p", 0.75),
         "frequency_penalty": ("frequency_penalty", 0.0),
         "presence_penalty": ("presence_penalty", 0.0),
         "stop_sequences": ("stop_sequences", None),
-        "client_timeout": ("client_timeout", 60),  # seconds
     }
     REQUEST_CLS = LMRequest
+    NAME = "cohere"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
@@ -89,29 +89,30 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": "cohere", "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
+            request: request
 
         Return:
             response as dict
         """
         return {
             "object": "text_completion",
             "model": getattr(self, "engine"),
             "choices": [
                 {
                     "text": item["text"],
                     "text_logprob": item.get("likelihood", None),
-                    "logprobs": item.get("token_likelihoods", None),
+                    "token_logprobs": item.get("token_likelihoods", None),
                 }
                 for item in response["generations"]
             ],
         }
```

### Comparing `manifest-ml-0.1.1/manifest/clients/diffuser.py` & `manifest-ml-0.1.2/manifest/clients/diffuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     PARAMS = {
         "num_inference_steps": ("num_inference_steps", 50),
         "height": ("height", 512),
         "width": ("width", 512),
         "n": ("num_images_per_prompt", 1),
         "guidance_scale": ("guidance_scale", 7.5),
         "eta": ("eta", 0.0),
-        "client_timeout": ("client_timeout", 120),  # seconds
     }
     REQUEST_CLS = DiffusionRequest
+    NAME = "diffuser"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
@@ -81,20 +81,21 @@
 
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params")
         return res.json()
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
+            request: request
 
         Return:
             response as dict
         """
         # Convert array to np.array
         for choice in response["choices"]:
             choice["array"] = self.to_numpy(np.array(choice["array"]))
```

### Comparing `manifest-ml-0.1.1/manifest/clients/dummy.py` & `manifest-ml-0.1.2/manifest/clients/dummy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Dummy client."""
 import logging
-from typing import Any, Callable, Dict, Optional, Tuple
+from typing import Any, Dict, Optional
 
 from manifest.clients.client import Client
 from manifest.request import LMRequest, Request
+from manifest.response import Response
 
 logger = logging.getLogger(__name__)
 
 
 class DummyClient(Client):
     """Dummy client."""
 
     # User param -> (client param, default value)
     PARAMS = {
         "n": ("num_results", 1),
     }
     REQUEST_CLS = LMRequest
+    NAME = "dummy"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
@@ -63,15 +65,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"engine": "dummy"}
 
-    def get_request(self, request: Request) -> Tuple[Callable[[], Dict], Dict]:
+    def run_request(self, request: Request) -> Response:
         """
         Get request string function.
 
         Args:
             request: request.
 
         Returns:
@@ -80,27 +82,40 @@
         """
         if isinstance(request.prompt, list):
             num_results = len(request.prompt)
         else:
             num_results = 1
         request_params = request.to_dict(self.PARAMS)
 
-        def _run_completion() -> Dict:
-            return {
-                "choices": [{"text": "hello"}]
-                * int(request_params["num_results"])
-                * num_results
-            }
+        response_dict = {
+            "choices": [{"text": "hello"}]
+            * int(request_params["num_results"])
+            * num_results,
+            "usage": [{"prompt_tokens": 1, "completion_tokens": 1, "total_tokens": 2}]
+            * int(request_params["num_results"])
+            * num_results,
+        }
+        return Response(response_dict, False, request_params)
 
-        return _run_completion, request_params
+    async def arun_batch_request(self, request: Request) -> Response:
+        """
+        Get async request string function.
+
+        Args:
+            request: request.
+
+        Returns:
+            response.
+        """
+        return self.run_request(request)
 
     def get_score_prompt_request(
         self,
         request: Request,
-    ) -> Tuple[Callable[[], Dict], Dict]:
+    ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
 
         Args:
             request: request.
 
         Returns:
@@ -109,21 +124,19 @@
         """
         if isinstance(request.prompt, list):
             num_results = len(request.prompt)
         else:
             num_results = 1
         request_params = {"prompt": request.prompt}
 
-        def _run_completion() -> Dict:
-            return {
-                "choices": [
-                    {
-                        "text": request.prompt
-                        if isinstance(request.prompt, str)
-                        else request.prompt[i],
-                        "logprob": 0.3,
-                    }
-                    for i in range(num_results)
-                ]
-            }
-
-        return _run_completion, request_params
+        response_dict = {
+            "choices": [
+                {
+                    "text": request.prompt
+                    if isinstance(request.prompt, str)
+                    else request.prompt[i],
+                    "logprob": 0.3,
+                }
+                for i in range(num_results)
+            ]
+        }
+        return Response(response_dict, False, request_params)
```

### Comparing `manifest-ml-0.1.1/manifest/clients/toma.py` & `manifest-ml-0.1.2/manifest/clients/toma.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         "temperature": ("temperature", 0.1),
         "max_tokens": ("max_tokens", 32),
         # n is depricated with new API but will come back online soon
         # "n": ("n", 1),
         "top_p": ("top_p", 0.9),
         "top_k": ("top_k", 40),
         "stop_sequences": ("stop", []),
-        "client_timeout": ("client_timeout", 120),  # seconds
     }
     REQUEST_CLS = LMRequest
+    NAME = "toma"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
@@ -139,27 +139,28 @@
             now = datetime.now(mod_time.tzinfo)
             heartbeats[mod["name"]] = {
                 "last_ping": (now - mod_time).total_seconds(),
                 "expected_runtime": mod["expected_runtime"],
             }
         return heartbeats
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
+            request: request
 
         Return:
             response as dict
         """
         return {
             "model": getattr(self, "engine"),
             "choices": [
                 {
                     "text": item["text"],
-                    # "logprobs": [],
+                    # "token_logprobs": [],
                 }
                 for item in response["output"]["choices"]
             ],
         }
```

### Comparing `manifest-ml-0.1.1/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.2/manifest/clients/toma_diffuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,36 +26,37 @@
     PARAMS = {
         "engine": ("model", "StableDiffusion"),
         "num_inference_steps": ("steps", 50),
         "height": ("height", 512),
         "width": ("width", 512),
         "n": ("n", 1),
         "guidance_scale": ("guidance_scale", 7.5),
-        "client_timeout": ("client_timeout", 120),  # seconds
     }
     REQUEST_CLS = DiffusionRequest  # type: ignore
+    NAME = "tomadiffuser"
 
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": "tomadiffuser", "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict) -> Dict[str, Any]:
+    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
+            request: request
 
         Return:
             response as dict
         """
         return {
             "model": getattr(self, "engine"),
             "choices": [
```

### Comparing `manifest-ml-0.1.1/manifest/request.py` & `manifest-ml-0.1.2/manifest/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 """Request object."""
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from pydantic import BaseModel
 
+NOT_CACHE_KEYS = {"client_timeout", "batch_size"}
+DEFAULT_REQUEST_KEYS = {
+    "client_timeout": ("client_timeout", 60),  # seconds
+    "batch_size": ("batch_size", 1),
+    "run_id": ("run_id", None),
+    "request_type": ("request_type", None),
+}
+
 
 class Request(BaseModel):
     """Request object."""
 
     # Prompt
     prompt: Union[str, List[str]] = ""
 
     # Engine
     engine: str = "text-ada-001"
 
     # Number completions
     n: int = 1
 
     # Timeout
-    client_timeout: int = 60
+    client_timeout: int = 120
+
+    # Run id used to repeat run with same parameters
+    run_id: Optional[str] = None
+
+    # Batch size for async batch run
+    batch_size: int = 8
+
+    # Request type None is for completion. Used to scoring prompt
+    request_type: str = None
 
     def to_dict(
         self, allowable_keys: Dict[str, Tuple[str, Any]] = None, add_prompt: bool = True
     ) -> Dict[str, Any]:
         """
         Convert request to a dictionary.
 
@@ -78,14 +95,17 @@
     # Penalize frequency
     frequency_penalty: float = 0
 
 
 class DiffusionRequest(Request):
     """Diffusion Model Request object."""
 
+    # Request type
+    request_type: str = "diffusion"
+
     # Number of steps
     num_inference_steps: int = 50
 
     # Height of image
     height: int = 512
 
     # Width of image
```

### Comparing `manifest-ml-0.1.1/manifest/response.py` & `manifest-ml-0.1.2/manifest/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 """Client response."""
 import json
 from typing import Any, Dict, List, Union
 
 import numpy as np
 
+RESPONSE_CONSTRUCTORS = {
+    "diffuser": {
+        "logits_key": "token_logprobs",
+        "item_key": "array",
+    },
+    "tomadiffuser": {
+        "logits_key": "token_logprobs",
+        "item_key": "array",
+    },
+}
+
 
 class NumpyArrayEncoder(json.JSONEncoder):
     """Numpy array encoder."""
 
     def default(self, obj: Any) -> str:
         """Encode numpy array."""
         if isinstance(obj, np.ndarray):
@@ -16,20 +27,21 @@
 
 
 class Response:
     """Response class."""
 
     def __init__(
         self,
-        response: Dict,
+        response: Dict,  # TODO: make pydantic model
         cached: bool,
-        request_params: Dict,
+        request_params: Dict,  # TODO: use request pydantic model
         generation_key: str = "choices",
-        logits_key: str = "logprobs",
+        logits_key: str = "token_logprobs",
         item_key: str = "text",
+        usage_key: str = "usage",
     ):
         """
         Initialize response.
 
         Args:
             response: response dict.
             cached: whether response is cached.
@@ -37,43 +49,54 @@
             generation_key: key for generation results.
             logits_key: key for logits.
             item_key: key for item in the generations.
         """
         self.generation_key = generation_key
         self.logits_key = logits_key
         self.item_key = item_key
+        self.usage_key = usage_key
         self.item_dtype = None
         if isinstance(response, dict):
             self._response = response
         else:
             raise ValueError(f"Response must be dict. Response is\n{response}.")
         if (
             (self.generation_key not in self._response)
             or (not isinstance(self._response[self.generation_key], list))
             or (len(self._response[self.generation_key]) <= 0)
         ):
             raise ValueError(
                 "Response must be serialized to a dict with a nonempty"
                 f" list of choices. Response is\n{self._response}."
             )
+        # Turn off usage if it is not in response
+        if self.usage_key not in self._response:
+            self.usage_key = None
+        else:
+            if not isinstance(self._response[self.usage_key], list):
+                raise ValueError(
+                    "Response must be a list with usage dicts, one per choice."
+                    f" Response is\n{self._response}."
+                )
+
         if self.item_key not in self._response[self.generation_key][0]:
             raise ValueError(
                 "Response must be serialized to a dict with a "
                 f"list of choices with {self.item_key} field"
             )
         if (
             self.logits_key in self._response[self.generation_key][0]
             and self._response[self.generation_key][0][self.logits_key]
         ):
             if not isinstance(
                 self._response[self.generation_key][0][self.logits_key], list
             ):
                 raise ValueError(
-                    "Response must be serialized to a dict with a "
-                    "list of choices with logprobs field"
+                    f"{self.logits_key} must be a list of items "
+                    "one for each token in the choice."
                 )
         if isinstance(
             self._response[self.generation_key][0][self.item_key], np.ndarray
         ):
             self.item_dtype = str(
                 self._response[self.generation_key][0][self.item_key].dtype
             )
```

### Comparing `manifest-ml-0.1.1/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.2/manifest_ml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
-Author-email: lorr1@cs.stanford.edu
+Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: api
 Provides-Extra: app
-Provides-Extra: chatgpt
 Provides-Extra: diffusers
+Provides-Extra: gcp
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
@@ -42,20 +42,14 @@
 ```
 
 Install with diffusion support:
 ```bash
 pip install manifest-ml[diffusers]
 ```
 
-Install with ChatGPT support:
-```bash
-pip install manifest-ml[chatgpt]
-```
-This installs [pyChatGPT](https://github.com/terry3041/pyChatGPT) and uses the ChatGPT session key to start a session. This key must be set as the `CHATGPT_SESSION_KEY` environment variable or passed in with `client_connection`.
-
 Install with HuggingFace local model support:
 ```bash
 pip install manifest-ml[api]
 ```
 
 Dev Install:
 ```bash
@@ -126,32 +120,14 @@
     client_name = "openai",
     cache_name = "redis",
     cache_connection = "localhost:6379"
 )
 ```
 As a hint, if you want to get Redis running, see the `docker run` command below under development.
 
-## Sessions
-Each Manifest run supports a session that, in addition to a global cache, connects to a local SQLite DB to store user query history.
-```python
-manifest = Manifest(
-    client_name = "openai",
-    cache_name = "sqlite",
-    cache_connection = "mycache.sqlite",
-    session_id = "grass_color",
-)
-```
-will start a Manifest session with the session name `grass_color`. This can be helpful for a user to logically keep track of sessions, see interaction history, and resume sessions if desired. If the session id provided is `_default`, we generate a random id for the user.
-
-After a few queries, the user can explore their history
-```python
-manifest.get_last_queries(4)
-```
-will retrieve the last 4 model queries and responses.
-
 ## Running Queries
 Once you have a session open, you can write and develop prompts.
 
 ```python
 result = manifest.run("Hello, my name is Laurel")
 ```
```

### Comparing `manifest-ml-0.1.1/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.2/manifest_ml.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 numpy>=1.20.0
 pydantic>=1.9.0
 redis>=4.3.1
 requests>=2.27.1
+aiohttp>=3.8.0
 sqlitedict>=2.0.0
+tenacity>=8.2.0
+tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
-python-dotenv>=0.20.0
 deepspeed>=0.7.0
-pep8-naming>=0.12.1
-types-redis>=4.2.6
-nbsphinx>=0.8.0
-diffusers>=0.6.0
+types-setuptools>=57.4.17
+fastapi>=0.70.0
+types-protobuf>=3.19.21
 sphinx-rtd-theme>=0.5.1
+sqlalchemy
+autopep8>=1.6.0
+docformatter>=1.4
+types-python-dateutil>=2.8.16
+recommonmark>=0.7.1
+uvicorn>=0.18.0
+diffusers>=0.6.0
+pg8000
+pre-commit>=2.14.0
+isort>=5.9.3
+flake8>=4.0.0
+nbsphinx>=0.8.0
 transformers<4.26.0,>=4.20.0
-pytest>=7.0.0
+black>=22.3.0
 mypy>=0.950
+twine
+types-PyYAML>=6.0.7
 types-requests>=2.27.29
+pep8-naming>=0.12.1
+accelerate>=0.10.0
+torch>=1.8.0
+python-dotenv>=0.20.0
 Flask>=2.1.2
-fastapi>=0.70.0
+types-xxhash>=3.0.0
+flake8-docstrings>=1.6.0
+cloud-sql-python-connector[pg8000]>=1.0.0
+pytest-cov>=3.0.0
 pillow>=9.0.0
-types-setuptools>=57.4.17
-torch>=1.8.0
-types-PyYAML>=6.0.7
-twine
-isort>=5.9.3
 types-pillow>=9.0.0
-uvicorn>=0.18.0
-accelerate>=0.10.0
-pytest-cov>=3.0.0
-flake8-docstrings>=1.6.0
-types-xxhash>=3.0.0
-pyChatGPT>=0.4.3
-types-protobuf>=3.19.21
-docformatter>=1.4
-pre-commit>=2.14.0
+pytest>=7.0.0
+types-redis>=4.2.6
 sphinx-autobuild
-black>=22.3.0
-flake8>=4.0.0
-types-python-dateutil>=2.8.16
-recommonmark>=0.7.1
-autopep8>=1.6.0
 
 [api]
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
 accelerate>=0.10.0
 transformers<4.26.0,>=4.20.0
 torch>=1.8.0
 
 [app]
 fastapi>=0.70.0
 uvicorn>=0.18.0
 
-[chatgpt]
-pyChatGPT>=0.4.3
-
 [dev]
 autopep8>=1.6.0
 black>=22.3.0
 isort>=5.9.3
 flake8>=4.0.0
 flake8-docstrings>=1.6.0
 mypy>=0.950
@@ -82,7 +84,12 @@
 types-pillow>=9.0.0
 types-xxhash>=3.0.0
 sphinx-autobuild
 twine
 
 [diffusers]
 pillow>=9.0.0
+
+[gcp]
+pg8000
+cloud-sql-python-connector[pg8000]>=1.0.0
+sqlalchemy
```

### Comparing `manifest-ml-0.1.1/pyproject.toml` & `manifest-ml-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/setup.py` & `manifest-ml-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,29 @@
 with open(ver_path) as ver_file:
     exec(ver_file.read(), main_ns)
 
 # Package meta-data.
 NAME = "manifest-ml"
 DESCRIPTION = "Manifest for Prompting Foundation Models."
 URL = "https://github.com/HazyResearch/manifest"
-EMAIL = "lorr1@cs.stanford.edu"
+EMAIL = "laurel.orr@numbersstation.ai"
 AUTHOR = "Laurel Orr"
 REQUIRES_PYTHON = ">=3.8.0"
 VERSION = main_ns["__version__"]
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "numpy>=1.20.0",
     "pydantic>=1.9.0",
     "redis>=4.3.1",
     "requests>=2.27.1",
+    "aiohttp>=3.8.0",
     "sqlitedict>=2.0.0",
+    "tenacity>=8.2.0",
+    "tiktoken>=0.3.0",
     "xxhash>=3.0.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     "api": [
         "deepspeed>=0.7.0",
@@ -46,20 +49,22 @@
         "transformers>=4.20.0,<4.26.0",
         "torch>=1.8.0",
     ],
     "app": [
         "fastapi>=0.70.0",
         "uvicorn>=0.18.0",
     ],
-    "chatgpt": [
-        "pyChatGPT>=0.4.3",
-    ],
     "diffusers": [
         "pillow>=9.0.0",
     ],
+    "gcp": [
+        "pg8000",
+        "cloud-sql-python-connector[pg8000]>=1.0.0",
+        "sqlalchemy",
+    ],
     "dev": [
         "autopep8>=1.6.0",
         "black>=22.3.0",
         "isort>=5.9.3",
         "flake8>=4.0.0",
         "flake8-docstrings>=1.6.0",
         "mypy>=0.950",
```

### Comparing `manifest-ml-0.1.1/web_app/main.py` & `manifest-ml-0.1.2/web_app/main.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.1/web_app/schemas.py` & `manifest-ml-0.1.2/web_app/schemas.py`

 * *Files identical despite different names*

