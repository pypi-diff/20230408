# Comparing `tmp/speechkit-2.2.1.tar.gz` & `tmp/speechkit-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechkit-2.2.1.tar", last modified: Tue Apr  4 23:25:43 2023, max compression
+gzip compressed data, was "speechkit-2.2.2.tar", last modified: Sat Apr  8 18:18:18 2023, max compression
```

## Comparing `speechkit-2.2.1.tar` & `speechkit-2.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.757861 speechkit-2.2.1/
--rw-r--r--   0 tikhon     (501) staff       (20)     1075 2021-07-25 21:54:31.000000 speechkit-2.2.1/LICENSE.txt
--rw-r--r--   0 tikhon     (501) staff       (20)     5983 2023-04-04 23:25:43.758035 speechkit-2.2.1/PKG-INFO
--rw-r--r--   0 tikhon     (501) staff       (20)     4865 2023-03-16 12:17:40.000000 speechkit-2.2.1/README.md
--rw-r--r--   0 tikhon     (501) staff       (20)      105 2021-07-25 21:54:31.000000 speechkit-2.2.1/pyproject.toml
--rw-r--r--   0 tikhon     (501) staff       (20)     1236 2023-04-04 23:25:43.759028 speechkit-2.2.1/setup.cfg
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.731195 speechkit-2.2.1/src/
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.736065 speechkit-2.2.1/src/speechkit/
--rw-r--r--   0 tikhon     (501) staff       (20)      520 2023-04-04 22:50:08.000000 speechkit-2.2.1/src/speechkit/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)    14491 2022-05-17 12:56:09.000000 speechkit-2.2.1/src/speechkit/_auth.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.739027 speechkit-2.2.1/src/speechkit/_recognition/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-07 17:17:00.000000 speechkit-2.2.1/src/speechkit/_recognition/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.739791 speechkit-2.2.1/src/speechkit/_recognition/google/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:17:36.000000 speechkit-2.2.1/src/speechkit/_recognition/google/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.742116 speechkit-2.2.1/src/speechkit/_recognition/google/api/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:17:51.000000 speechkit-2.2.1/src/speechkit/_recognition/google/api/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)     2165 2021-08-08 11:04:14.000000 speechkit-2.2.1/src/speechkit/_recognition/google/api/annotations_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)      159 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 tikhon     (501) staff       (20)    10493 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/google/api/http_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)      159 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.743037 speechkit-2.2.1/src/speechkit/_recognition/google/rpc/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:18:03.000000 speechkit-2.2.1/src/speechkit/_recognition/google/rpc/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)     3432 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/google/rpc/status_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)      159 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/google/rpc/status_pb2_grpc.py
--rw-r--r--   0 tikhon     (501) staff       (20)     8106 2021-08-11 19:36:36.000000 speechkit-2.2.1/src/speechkit/_recognition/streaming_recognition.py
--rw-r--r--   0 tikhon     (501) staff       (20)    15580 2023-04-04 22:41:37.000000 speechkit-2.2.1/src/speechkit/_recognition/sync_recognition.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.743359 speechkit-2.2.1/src/speechkit/_recognition/yandex/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:19:33.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.743590 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:18:18.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.743826 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:18:29.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.744056 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:18:39.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/__init__.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.746017 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:18:48.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)    33603 2021-08-08 11:03:51.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)     5030 2021-08-08 11:04:38.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.748732 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/api/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:19:06.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/api/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)     3633 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/api/operation_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)      159 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/api/operation_pb2_grpc.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.750953 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/operation/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2021-08-08 23:19:17.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/operation/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)     7861 2021-08-08 11:04:26.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2.py
--rw-r--r--   0 tikhon     (501) staff       (20)      159 2021-08-07 23:57:39.000000 speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2_grpc.py
--rw-r--r--   0 tikhon     (501) staff       (20)     6708 2021-08-08 15:55:54.000000 speechkit-2.2.1/src/speechkit/_synthesis.py
--rw-r--r--   0 tikhon     (501) staff       (20)      345 2021-08-08 14:51:17.000000 speechkit-2.2.1/src/speechkit/auth.py
--rw-r--r--   0 tikhon     (501) staff       (20)      518 2021-08-08 15:51:28.000000 speechkit-2.2.1/src/speechkit/exceptions.py
--rw-r--r--   0 tikhon     (501) staff       (20)     1025 2021-08-08 15:51:28.000000 speechkit-2.2.1/src/speechkit/utils.py
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.737843 speechkit-2.2.1/src/speechkit.egg-info/
--rw-r--r--   0 tikhon     (501) staff       (20)     5983 2023-04-04 23:25:43.000000 speechkit-2.2.1/src/speechkit.egg-info/PKG-INFO
--rw-r--r--   0 tikhon     (501) staff       (20)     2054 2023-04-04 23:25:43.000000 speechkit-2.2.1/src/speechkit.egg-info/SOURCES.txt
--rw-r--r--   0 tikhon     (501) staff       (20)        1 2023-04-04 23:25:43.000000 speechkit-2.2.1/src/speechkit.egg-info/dependency_links.txt
--rw-r--r--   0 tikhon     (501) staff       (20)       79 2023-04-04 23:25:43.000000 speechkit-2.2.1/src/speechkit.egg-info/requires.txt
--rw-r--r--   0 tikhon     (501) staff       (20)       16 2023-04-04 23:25:43.000000 speechkit-2.2.1/src/speechkit.egg-info/top_level.txt
-drwxr-xr-x   0 tikhon     (501) staff       (20)        0 2023-04-04 23:25:43.757273 speechkit-2.2.1/src/tests/
--rw-r--r--   0 tikhon     (501) staff       (20)        0 2022-04-27 22:19:03.000000 speechkit-2.2.1/src/tests/__init__.py
--rw-r--r--   0 tikhon     (501) staff       (20)     3894 2022-05-13 12:26:40.000000 speechkit-2.2.1/src/tests/test_auth.py
--rw-r--r--   0 tikhon     (501) staff       (20)      849 2022-04-27 22:19:03.000000 speechkit-2.2.1/src/tests/test_exceptions.py
--rw-r--r--   0 tikhon     (501) staff       (20)    27634 2023-03-16 12:06:07.000000 speechkit-2.2.1/src/tests/test_long_audio_recognition.py
--rw-r--r--   0 tikhon     (501) staff       (20)    26357 2022-05-13 12:05:23.000000 speechkit-2.2.1/src/tests/test_short_audio_recognition.py
--rw-r--r--   0 tikhon     (501) staff       (20)     1572 2022-04-27 22:19:03.000000 speechkit-2.2.1/src/tests/test_speech_synthesis.py
--rw-r--r--   0 tikhon     (501) staff       (20)     1727 2022-05-13 12:05:23.000000 speechkit-2.2.1/src/tests/test_streaming_recognition.py
--rw-r--r--   0 tikhon     (501) staff       (20)      860 2022-05-13 12:33:14.000000 speechkit-2.2.1/src/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.424963 speechkit-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-08 18:18:09.000000 speechkit-2.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-08 18:18:18.424963 speechkit-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-08 18:18:09.000000 speechkit-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-08 18:18:09.000000 speechkit-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-08 18:18:18.424963 speechkit-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.416963 speechkit-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/google/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/api/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/rpc/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/google/rpc/status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/streaming_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/sync_recognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33603 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/api/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/api/operation_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/operation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/speechkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.420963 speechkit-2.2.2/src/speechkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-08 18:18:18.000000 speechkit-2.2.2/src/speechkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-08 18:18:18.000000 speechkit-2.2.2/src/speechkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:18:18.000000 speechkit-2.2.2/src/speechkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-08 18:18:18.000000 speechkit-2.2.2/src/speechkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 18:18:18.000000 speechkit-2.2.2/src/speechkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:18.424963 speechkit-2.2.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27634 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_long_audio_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26357 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_short_audio_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_speech_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_streaming_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-08 18:18:09.000000 speechkit-2.2.2/src/tests/test_utils.py
```

### Comparing `speechkit-2.2.1/LICENSE.txt` & `speechkit-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/PKG-INFO` & `speechkit-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechkit
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python SDK for Yandex Speechkit API.
 Home-page: https://github.com/TikhonP/yandex-speechkit-lib-python
 Author: Tikhon Petrishchev
 Author-email: tikhon.petrishchev@gmail.com
 Project-URL: Bug Tracker, https://github.com/TikhonP/yandex-speechkit-lib-python/issues
 Project-URL: Documentation, https://yandex-speechkit-lib-python.readthedocs.io/en/latest/index.html
 Project-URL: GitHub, https://github.com/TikhonP/yandex-speechkit-lib-python
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center">
```

### Comparing `speechkit-2.2.1/README.md` & `speechkit-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/setup.cfg` & `speechkit-2.2.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = speechkit
-version = 2.2.1
+version = 2.2.2
 author = Tikhon Petrishchev
 author_email = tikhon.petrishchev@gmail.com
 description = Python SDK for Yandex Speechkit API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TikhonP/yandex-speechkit-lib-python
 project_urls = 
@@ -17,14 +17,15 @@
 	Natural Language :: English
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
 	boto3
```

### Comparing `speechkit-2.2.1/src/speechkit/__init__.py` & `speechkit-2.2.2/src/speechkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 speechkit
 Python SDK for using Yandex Speech recognition and synthesis.
 """
 
 __author__ = 'Tikhon Petrishchev'
-__version__ = '2.2.1'
+__version__ = '2.2.2'
 
 from speechkit._auth import Session
 from speechkit._recognition.streaming_recognition import DataStreamingRecognition
 from speechkit._recognition.sync_recognition import ShortAudioRecognition, RecognitionLongAudio
 from speechkit._synthesis import SpeechSynthesis
 
 __all__ = ['Session', 'SpeechSynthesis', 'ShortAudioRecognition', 'RecognitionLongAudio', 'DataStreamingRecognition']
```

### Comparing `speechkit-2.2.1/src/speechkit/_auth.py` & `speechkit-2.2.2/src/speechkit/_auth.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/google/api/annotations_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/google/api/http_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/google/rpc/status_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/streaming_recognition.py` & `speechkit-2.2.2/src/speechkit/_recognition/streaming_recognition.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/sync_recognition.py` & `speechkit-2.2.2/src/speechkit/_recognition/sync_recognition.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py` & `speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/api/operation_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/api/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2.py` & `speechkit-2.2.2/src/speechkit/_recognition/yandex/cloud/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/_synthesis.py` & `speechkit-2.2.2/src/speechkit/_synthesis.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/exceptions.py` & `speechkit-2.2.2/src/speechkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit/utils.py` & `speechkit-2.2.2/src/speechkit/utils.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/speechkit.egg-info/PKG-INFO` & `speechkit-2.2.2/src/speechkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechkit
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python SDK for Yandex Speechkit API.
 Home-page: https://github.com/TikhonP/yandex-speechkit-lib-python
 Author: Tikhon Petrishchev
 Author-email: tikhon.petrishchev@gmail.com
 Project-URL: Bug Tracker, https://github.com/TikhonP/yandex-speechkit-lib-python/issues
 Project-URL: Documentation, https://yandex-speechkit-lib-python.readthedocs.io/en/latest/index.html
 Project-URL: GitHub, https://github.com/TikhonP/yandex-speechkit-lib-python
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center">
```

### Comparing `speechkit-2.2.1/src/speechkit.egg-info/SOURCES.txt` & `speechkit-2.2.2/src/speechkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_auth.py` & `speechkit-2.2.2/src/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_exceptions.py` & `speechkit-2.2.2/src/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_long_audio_recognition.py` & `speechkit-2.2.2/src/tests/test_long_audio_recognition.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_short_audio_recognition.py` & `speechkit-2.2.2/src/tests/test_short_audio_recognition.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_speech_synthesis.py` & `speechkit-2.2.2/src/tests/test_speech_synthesis.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_streaming_recognition.py` & `speechkit-2.2.2/src/tests/test_streaming_recognition.py`

 * *Files identical despite different names*

### Comparing `speechkit-2.2.1/src/tests/test_utils.py` & `speechkit-2.2.2/src/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 
     def invalid_session_from_api_key(self):
         session = Session.from_api_key('api_key', 'sdsas')
         with self.assertRaises(ValueError):
             list_of_service_accounts(session)
 
     def invalid_session_no_folder_id(self):
-        session = Session.from_yandex_passport_oauth_token(api_key)
+        api_key = os.environ.get('YANDEX_OAUTH')
+        session = Session.from_api_key(api_key)
         with self.assertRaises(ValueError):
             list_of_service_accounts(session)
```

