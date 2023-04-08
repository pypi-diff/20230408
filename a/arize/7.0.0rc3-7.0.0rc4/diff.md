# Comparing `tmp/arize-7.0.0rc3.tar.gz` & `tmp/arize-7.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kiko/Documents/Arize/arize/sdk/python/logger/dist/.tmp-utjbw9mc/arize-7.0.0rc3.tar", last modified: Wed Apr  5 03:10:06 2023, max compression
+gzip compressed data, was "arize-7.0.0rc4.tar", last modified: Fri Apr  7 22:52:10 2023, max compression
```

## Comparing `arize-7.0.0rc3.tar` & `arize-7.0.0rc4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc3/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc3/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-05 03:10:06.000000 arize-7.0.0rc3/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc3/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-05 03:09:13.000000 arize-7.0.0rc3/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    25743 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2279 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     2351 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      385 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    11458 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    21869 2023-04-05 02:42:05.000000 arize-7.0.0rc3/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    22283 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    59096 2023-04-01 00:42:11.000000 arize-7.0.0rc3/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167320 2023-04-05 02:42:05.000000 arize-7.0.0rc3/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-03-30 21:17:25.000000 arize-7.0.0rc3/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    18696 2023-04-05 02:36:10.000000 arize-7.0.0rc3/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7196 2023-04-05 02:36:10.000000 arize-7.0.0rc3/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-05 03:10:05.000000 arize-7.0.0rc3/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc3/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1561 2023-04-05 03:10:06.000000 arize-7.0.0rc3/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-05 03:10:06.000000 arize-7.0.0rc3/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    43569 2023-03-30 21:17:25.000000 arize-7.0.0rc3/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc3/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.374084 arize-7.0.0rc4/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc4/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc4/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-07 22:52:10.374690 arize-7.0.0rc4/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc4/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.267353 arize-7.0.0rc4/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    25743 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.305116 arize-7.0.0rc4/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.308253 arize-7.0.0rc4/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.326610 arize-7.0.0rc4/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2279 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.328141 arize-7.0.0rc4/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.334591 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    11932 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    21965 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.354679 arize-7.0.0rc4/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.359424 arize-7.0.0rc4/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22704 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    59911 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   167320 2023-04-07 22:16:19.000000 arize-7.0.0rc4/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.369208 arize-7.0.0rc4/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    20830 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7196 2023-04-06 23:45:03.000000 arize-7.0.0rc4/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.276765 arize-7.0.0rc4/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc4/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1561 2023-04-07 22:52:10.377092 arize-7.0.0rc4/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.373013 arize-7.0.0rc4/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    43569 2023-03-30 21:17:25.000000 arize-7.0.0rc4/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc4/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arize-7.0.0rc3/LICENSE.md` & `arize-7.0.0rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/PKG-INFO` & `arize-7.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc3
+Version: 7.0.0rc4
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: MimicExplainer
 Provides-Extra: AutoEmbeddings
 Provides-Extra: LLM_Evaluation
 License-File: LICENSE.md
 
 <div align="center">
```

### Comparing `arize-7.0.0rc3/README.md` & `arize-7.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/api.py` & `arize-7.0.0rc4/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/bounded_executor.py` & `arize-7.0.0rc4/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/bulk_client.py` & `arize-7.0.0rc4/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/bulk_client_shap.py` & `arize-7.0.0rc4/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/client_shap_values.py` & `arize-7.0.0rc4/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/log_client.py` & `arize-7.0.0rc4/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/log_pandas_dataframe.py` & `arize-7.0.0rc4/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/examples/preproduction_client.py` & `arize-7.0.0rc4/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.0rc4/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/base_generators.py` & `arize-7.0.0rc4/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.0rc4/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/models.py` & `arize-7.0.0rc4/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.0rc4/arize/pandas/embeddings/nlp_generators.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,7 +54,40 @@
         logger.info("Generating embedding vectors")
         ds = ds.map(
             lambda batch: self._get_embedding_vector(batch, "cls_token"),
             batched=True,
             batch_size=self.batch_size,
         )
         return cast(pd.DataFrame, ds.to_pandas())["embedding_vector"]
+
+
+class EmbeddingGeneratorForNLPSummarization(NLPEmbeddingGenerator):
+    def __init__(self, model_name: str = "distilbert-base-uncased", **kwargs):
+        super(EmbeddingGeneratorForNLPSummarization, self).__init__(
+            use_case=UseCases.NLP.SUMMARIZATION,
+            model_name=model_name,
+            **kwargs,
+        )
+
+    def generate_embeddings(
+        self,
+        text_col: pd.Series,
+    ) -> pd.Series:
+        """
+        Obtain embedding vectors from your text data using pre-trained large language models.
+
+        :param text_col: a pandas Series containing the different pieces of text.
+        :return: a pandas Series containing the embedding vectors.
+        """
+        if not isinstance(text_col, pd.Series):
+            raise TypeError("text_col must be a pandas Series")
+
+        ds = Dataset.from_dict({"text": text_col})
+
+        ds.set_transform(partial(self.tokenize, text_feat_name="text"))
+        logger.info("Generating embedding vectors")
+        ds = ds.map(
+            lambda batch: self._get_embedding_vector(batch, "avg_token"),
+            batched=True,
+            batch_size=self.batch_size,
+        )
+        return cast(pd.DataFrame, ds.to_pandas())["embedding_vector"]
```

### Comparing `arize-7.0.0rc3/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.0rc4/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Optional
 
 import pandas as pd
+from arize.utils.logging import logger
 from tqdm.auto import tqdm
 
 from .constants import IMPORT_ERROR_MESSAGE
 
 try:
     import evaluate
 except ImportError:
@@ -35,15 +36,17 @@
             for each translation.
         max_order (int, optional):  Maximum n-gram order to use when computing BLEU score. Defaults to 4.
         smooth (bool, optional): Whether or not to apply Lin et al. 2004 smoothing. Defaults to False.
 
     Returns:
         List[float]: BLEU scores
     """
+    logger.info("Loading metric: bleu")
     bleu = evaluate.load("bleu")
+    logger.info("Computing bleu scores")
     return [
         bleu.compute(
             predictions=[preds], references=[refs], max_order=max_order, smooth=smooth
         )[  # type:ignore
             "bleu"
         ]
         for (preds, refs) in tqdm(
@@ -89,15 +92,17 @@
             to False.
         use_effective_order (bool, optional): If True, stops including n-gram orders for which precision is 0.
             This should be True, if sentence-level BLEU will be computed. Defaults to False.
 
     Returns:
         List[float]: SacreBLEU scores
     """
+    logger.info("Loading metric: sacrebleu")
     s_bleu = evaluate.load("sacrebleu")
+    logger.info("Computing sacrebleu scores")
     return [
         s_bleu.compute(
             predictions=[preds],
             references=[refs],
             smooth_method=smooth_method,
             smooth_value=smooth_value,
             lowercase=lowercase,
@@ -138,15 +143,17 @@
             for each translation.
         min_len (int, optional): The minimum order of n-gram this function should extract. Defaults to 1.
         max_len (int, optional): The maximum order of n-gram this function should extract. Defaults to 4.
 
     Returns:
         List[float]: google-BLEU scores
     """
+    logger.info("Loading metric: google_bleu")
     g_bleu = evaluate.load("google_bleu")
+    logger.info("Computing google_bleu scores")
     return [
         g_bleu.compute(predictions=[preds], references=[refs])["google_bleu"]  # type:ignore
         for (preds, refs) in tqdm(zip(response_col, references_col), total=len(response_col))
     ]
 
 
 # ROUGE
@@ -180,15 +187,17 @@
         use_stemmer (bool, optional): If True, uses Porter stemmer to strip word suffixes. Defaults to False.
 
     Returns:
         Dict[str, List[float]]: The output is a dictionary with one entry for each rouge type in the input
             list rouge_types.
     """
     data: Dict[str, List[float]] = {k: [0] * len(response_col) for k in rouge_types}
+    logger.info("Loading metric: rouge")
     rouge = evaluate.load("rouge")
+    logger.info("Computing rouge scores")
     for idx, (preds, refs) in tqdm(
         enumerate(zip(response_col, references_col)),
         total=len(response_col),
     ):
         r: Dict[str, float] = rouge.compute(
             predictions=[preds],
             references=[refs],
@@ -228,15 +237,17 @@
         beta (float, optional): Parameter for controlling shape of penalty as a function of fragmentation.
             Default is 3.
         gamma (float, optional): The relative weight assigned to fragmentation penalty. Default is 0.5.
 
     Returns:
         List[float]: METEOR scores
     """
+    logger.info("Loading metric: meteor")
     meteor = evaluate.load("meteor")
+    logger.info("Computing meteor scores")
     return [
         meteor.compute(
             predictions=[preds], references=[refs], alpha=alpha, beta=beta, gamma=gamma
         )[  # type:ignore
             "meteor"
         ]
         for (preds, refs) in tqdm(zip(response_col, references_col), total=len(response_col))
```

### Comparing `arize-7.0.0rc3/arize/pandas/logger.py` & `arize-7.0.0rc4/arize/pandas/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,14 +98,25 @@
         shap_values_column_names attribute in the Schema, this module will not run. Defaults to
         False.
         :param timeout (float, optional): You can stop waiting for a response after a given number
         of seconds with the timeout parameter. Defaults to None.
         :param verbose: (bool, optional) = When set to true, info messages are printed. Defaults to
         False.
         """
+        # Warning for when prediction_id is not provided by the user and we generate the default
+        # prediction ids
+        if schema.prediction_id_column_name is None:
+            logger.warning(
+                "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
+                "if not provided by the user, allowing referencing and joining with actuals."
+            )
+        # Warning for when prediction_label is not provided and we generate default prediction
+        # labels for GENERATIVE_LLM models
+        if model_type == ModelTypes.GENERATIVE_LLM:
+            self._generative_model_warnings(dataframe, schema)
 
         if verbose:
             logger.info("Performing required validation.")
         errors = Validator.validate_required_checks(
             dataframe=dataframe,
             model_id=model_id,
             schema=schema,
@@ -442,54 +453,32 @@
             )
 
     def _add_default_prediction_label_column(self, df: pd.DataFrame) -> pd.DataFrame:
         df["default_prediction_label"] = [1] * len(df)
         return df
 
     def _remove_extraneous_columns(self, df: pd.DataFrame, schema: Schema) -> pd.DataFrame:
-        cols_to_keep = set()
-
-        for field in schema.__dataclass_fields__:
-            if field.endswith("column_name"):
-                col = getattr(schema, field)
-                if col is not None:
-                    cols_to_keep.add(col)
-
-        if schema.feature_column_names is not None:
-            for col in schema.feature_column_names:
-                cols_to_keep.add(col)
-
-        if schema.embedding_feature_column_names is not None:
-            for emb_col_names in schema.embedding_feature_column_names.values():
-                cols_to_keep.add(emb_col_names.vector_column_name)
-                if emb_col_names.data_column_name is not None:
-                    cols_to_keep.add(emb_col_names.data_column_name)
-                if emb_col_names.link_to_data_column_name is not None:
-                    cols_to_keep.add(emb_col_names.link_to_data_column_name)
-
-        if schema.tag_column_names is not None:
-            for col in schema.tag_column_names:
-                cols_to_keep.add(col)
+        return df[df.columns.intersection(schema.get_used_columns())]
 
-        if schema.shap_values_column_names is not None:
-            for col in schema.shap_values_column_names.values():
-                cols_to_keep.add(col)
-
-        if schema.object_detection_prediction_column_names is not None:
-            for col in schema.object_detection_prediction_column_names:
-                cols_to_keep.add(col)
-
-        if schema.object_detection_actual_column_names is not None:
-            for col in schema.object_detection_actual_column_names:
-                cols_to_keep.add(col)
-
-        if schema.prompt_column_names is not None:
-            cols_to_keep.add(schema.prompt_column_names.vector_column_name)
-            if schema.prompt_column_names.data_column_name is not None:
-                cols_to_keep.add(schema.prompt_column_names.data_column_name)
-
-        if schema.response_column_names is not None:
-            cols_to_keep.add(schema.response_column_names.vector_column_name)
-            if schema.response_column_names.data_column_name is not None:
-                cols_to_keep.add(schema.response_column_names.data_column_name)
-
-        return df[df.columns.intersection(cols_to_keep)]
+    def _generative_model_warnings(self, df: pd.DataFrame, schema: Schema):
+        # Warning for when prediction_label_column_name is not provided
+        if schema.prediction_label_column_name is None:
+            logger.warning(
+                "prediction_label_column_name was not provided, a default prediction label equal "
+                "to 1 will be set for GENERATIVE_LLM models."
+            )
+            # Warning for when actual_label is also not provided
+            if schema.actual_label_column_name is None:
+                logger.warning(
+                    "actual_label_column_name was not provided. Some metrics that require actual labels, "
+                    "e.g. correctness or accuracy, may not be computed."
+                )
+            # Warning for when default prediction labels are 0/1 but actual_labels are not
+            elif not df[schema.actual_label_column_name].isin([0, 1]).all():
+                logger.warning(
+                    f"actual labels in the {schema.actual_label_column_name} column do not follow the "
+                    "standard, i.e. 1/0, used for the prediction label (defaulted to 1). Some "
+                    "metrics that require actual labels, e.g. correctness or accuracy, may not "
+                    "be computed accurately. Consider providing a prediction_label_column_name "
+                    "column containing the positive class from the values in the "
+                    f"{schema.actual_label_column_name} column."
+                )
```

### Comparing `arize-7.0.0rc3/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.0rc4/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/pandas/validation/errors.py` & `arize-7.0.0rc4/arize/pandas/validation/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,28 @@
         return (
             f"Cannot use 'object_detection_prediction_column_names' or "
             f"'object_detection_actual_column_names' for {self.invalid_model_type} model "
             f"type. They are only allowed for ModelTypes.OBJECT_DETECTION models"
         )
 
 
+class DuplicateColumnsInDataframe(ValidationError):
+    def __repr__(self) -> str:
+        return "Duplicate_Columns_In_Dataframe"
+
+    def __init__(self, cols: Iterable) -> None:
+        self.duplicate_cols = cols
+
+    def error_message(self) -> str:
+        return (
+            "The following columns are present in the schema and have duplicates in the dataframe: "
+            f"{self.duplicate_cols}. "
+        )
+
+
 # -----------
 # Type checks
 # -----------
 
 
 class InvalidType(ValidationError):
     def __repr__(self) -> str:
```

### Comparing `arize-7.0.0rc3/arize/pandas/validation/validator.py` & `arize-7.0.0rc4/arize/pandas/validation/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         general_checks = chain(
             Validator._check_invalid_model_id(model_id),
             Validator._check_invalid_model_version(model_version),
             Validator._check_invalid_model_type(model_type),
             Validator._check_invalid_environment(environment),
             Validator._check_invalid_batch_id(batch_id, environment),
             Validator._check_missing_columns(dataframe, schema),
+            Validator._check_dataframe_for_duplicate_columns(schema, dataframe),
             Validator._check_invalid_shap_suffix(schema),
             # model mapping checks
             Validator._check_model_type_and_metrics(model_type, metric_families, schema),
         )
 
         if model_type in NUMERIC_MODEL_TYPES:
             num_checks = chain(
@@ -618,14 +619,28 @@
             schema.prediction_group_id_column_name,
             schema.rank_column_name,
         )
         if any(col is None for col in required):
             return [err.MissingRequiredColumnsForRankingModel()]
         return []
 
+    @staticmethod
+    def _check_dataframe_for_duplicate_columns(
+        schema: Schema, dataframe: pd.DataFrame
+    ) -> List[err.DuplicateColumnsInDataframe]:
+        # Get the columns used in the schema
+        schema_col_used = schema.get_used_columns()
+        # Get the duplicated column names from the dataframe
+        df_duplicate_cols = dataframe.loc[:, dataframe.columns.duplicated()].columns.to_list()
+        # These are the duplicated columns from the dataframe that are referred to by the schema
+        schema_duplicate_cols = [col for col in df_duplicate_cols if col in schema_col_used]
+        if schema_duplicate_cols:
+            return [err.DuplicateColumnsInDataframe(schema_duplicate_cols)]
+        return []
+
     # -----------
     # Type checks
     # -----------
 
     @staticmethod
     def _check_type_prediction_id(
         schema: Schema, column_types: Dict[str, Any]
```

### Comparing `arize-7.0.0rc3/arize/public_pb2.py` & `arize-7.0.0rc4/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/utils/logging.py` & `arize-7.0.0rc4/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/utils/model_mapping.json` & `arize-7.0.0rc4/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize/utils/types.py` & `arize-7.0.0rc4/arize/utils/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import asdict, dataclass
 from dataclasses import replace as dataclass_replace
 from enum import Enum, unique
-from typing import Dict, List, NamedTuple, Optional, Sequence, TypeVar, Union
+from typing import Dict, List, NamedTuple, Optional, Sequence, Set, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
 
 @unique
 class ModelTypes(Enum):
@@ -442,13 +442,61 @@
 
     def replace(self, **changes):
         return dataclass_replace(self, **changes)
 
     def asdict(self) -> Dict[str, str]:
         return asdict(self)
 
+    def get_used_columns(self) -> Set[str]:
+        columns_used = set()
+
+        for field in self.__dataclass_fields__:
+            if field.endswith("column_name"):
+                col = getattr(self, field)
+                if col is not None:
+                    columns_used.add(col)
+
+        if self.feature_column_names is not None:
+            for col in self.feature_column_names:
+                columns_used.add(col)
+        if self.embedding_feature_column_names is not None:
+            for emb_col_names in self.embedding_feature_column_names.values():
+                columns_used.add(emb_col_names.vector_column_name)
+                if emb_col_names.data_column_name is not None:
+                    columns_used.add(emb_col_names.data_column_name)
+                if emb_col_names.link_to_data_column_name is not None:
+                    columns_used.add(emb_col_names.link_to_data_column_name)
+
+        if self.tag_column_names is not None:
+            for col in self.tag_column_names:
+                columns_used.add(col)
+
+        if self.shap_values_column_names is not None:
+            for col in self.shap_values_column_names.values():
+                columns_used.add(col)
+
+        if self.object_detection_prediction_column_names is not None:
+            for col in self.object_detection_prediction_column_names:
+                columns_used.add(col)
+
+        if self.object_detection_actual_column_names is not None:
+            for col in self.object_detection_actual_column_names:
+                columns_used.add(col)
+
+        if self.prompt_column_names is not None:
+            columns_used.add(self.prompt_column_names.vector_column_name)
+            if self.prompt_column_names.data_column_name is not None:
+                columns_used.add(self.prompt_column_names.data_column_name)
+
+        if self.response_column_names is not None:
+            columns_used.add(self.response_column_names.vector_column_name)
+            if self.response_column_names.data_column_name is not None:
+                columns_used.add(self.response_column_names.data_column_name)
+
+        return columns_used
+
 
 T = TypeVar("T", bound=type)
 
 
 def is_list_of(lst: Sequence[object], tp: T) -> bool:
     return isinstance(lst, list) and all(isinstance(x, tp) for x in lst)
```

### Comparing `arize-7.0.0rc3/arize/utils/utils.py` & `arize-7.0.0rc4/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/arize.egg-info/PKG-INFO` & `arize-7.0.0rc4/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc3
+Version: 7.0.0rc4
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: MimicExplainer
 Provides-Extra: AutoEmbeddings
 Provides-Extra: LLM_Evaluation
 License-File: LICENSE.md
 
 <div align="center">
```

### Comparing `arize-7.0.0rc3/arize.egg-info/SOURCES.txt` & `arize-7.0.0rc4/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/setup.cfg` & `arize-7.0.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	Topic :: System :: Logging
 	Topic :: System :: Monitoring
 keywords = arize
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	requests_futures==1.0.0
 	googleapis_common_protos~=1.51
 	protobuf~=3.12
 	pandas>=0.25.3,<2
 	pyarrow>=5.0.0
 
@@ -45,16 +45,16 @@
 	interpret>=0.2.7,<1
 	interpret-community>=0.22.0,<1
 	lightgbm>=2.2.3,<3.3.4
 AutoEmbeddings = 
 	transformers>=4.25, <5
 	tokenizers>=0.13, <1
 	datasets>=2.8, <3
-	torch>=1.13, <2
-	Pillow>=9.0.0, <10
+	torch>=1.13, <3
+	Pillow>=8.4.0, <10
 LLM_Evaluation = 
 	nltk>=3.0.0, <4
 	sacrebleu>=2.3.1, <3
 	rouge-score>=0.1.2, <1
 	evaluate>=0.3, <1
 
 [options.packages.find]
```

### Comparing `arize-7.0.0rc3/tests/test_api.py` & `arize-7.0.0rc4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc3/tests/test_utils.py` & `arize-7.0.0rc4/tests/test_utils.py`

 * *Files identical despite different names*

