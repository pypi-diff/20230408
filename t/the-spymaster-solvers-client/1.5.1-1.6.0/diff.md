# Comparing `tmp/the-spymaster-solvers-client-1.5.1.tar.gz` & `tmp/the-spymaster-solvers-client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-spymaster-solvers-client-1.5.1.tar", last modified: Fri Feb 10 19:38:31 2023, max compression
+gzip compressed data, was "the-spymaster-solvers-client-1.6.0.tar", last modified: Sat Apr  8 20:43:30 2023, max compression
```

## Comparing `the-spymaster-solvers-client-1.5.1.tar` & `the-spymaster-solvers-client-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/
--rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      492 2023-02-10 19:33:46.000000 the-spymaster-solvers-client-1.5.1/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/
--rw-rw-r--   0 akali     (1000) akali     (1000)       60 2022-06-26 22:20:09.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1517 2023-01-27 16:28:55.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/client.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/
--rw-rw-r--   0 akali     (1000) akali     (1000)       93 2022-06-26 22:01:46.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      708 2022-06-26 22:42:36.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      156 2023-02-10 18:30:33.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/errors.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1257 2023-01-27 16:32:45.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/requests.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      735 2023-01-27 16:34:58.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/responses.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-02-10 19:38:31.834615 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-02-10 19:38:31.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      597 2023-02-10 19:38:31.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-02-10 19:38:31.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       68 2023-02-10 19:38:31.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       29 2023-02-10 19:38:31.000000 the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/top_level.txt
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      492 2023-04-08 20:40:54.000000 the-spymaster-solvers-client-1.6.0/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       60 2022-06-26 22:20:09.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1517 2023-01-27 16:28:55.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/client.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/
+-rw-rw-r--   0 akali     (1000) akali     (1000)       93 2022-06-26 22:01:46.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      708 2022-06-26 22:42:36.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      156 2023-02-10 18:30:33.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/errors.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1263 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/requests.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      740 2023-04-08 20:41:50.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/responses.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 20:43:30.190816 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      325 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      597 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       68 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       29 2023-04-08 20:43:30.000000 the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/top_level.txt
```

### Comparing `the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/client.py` & `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/client.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/base.py` & `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/base.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/requests.py` & `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from codenames.game import GameState
+from codenames.game.state import GameState
 from pydantic import BaseModel, root_validator
 
 from .base import ModelIdentifier, Solver
 
 
 class LoadModelsRequest(BaseModel):
     model_identifiers: List[ModelIdentifier] = []
```

### Comparing `the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client/structs/responses.py` & `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client/structs/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from codenames.game import Guess, Hint
+from codenames.game.move import Guess, Hint
 from pydantic import BaseModel
 
 from .base import ModelIdentifier, Solver
 
 
 class BaseResponse(BaseModel):
     pass
```

### Comparing `the-spymaster-solvers-client-1.5.1/the_spymaster_solvers_client.egg-info/SOURCES.txt` & `the-spymaster-solvers-client-1.6.0/the_spymaster_solvers_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

