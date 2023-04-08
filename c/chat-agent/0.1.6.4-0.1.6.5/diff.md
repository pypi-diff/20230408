# Comparing `tmp/chat_agent-0.1.6.4.tar.gz` & `tmp/chat_agent-0.1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_agent-0.1.6.4.tar", last modified: Sat Apr  8 06:09:59 2023, max compression
+gzip compressed data, was "chat_agent-0.1.6.5.tar", last modified: Sat Apr  8 16:52:22 2023, max compression
```

## Comparing `chat_agent-0.1.6.4.tar` & `chat_agent-0.1.6.5.tar`

### file list

```diff
@@ -1,59 +1,55 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.257326 chat_agent-0.1.6.4/
--rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.4/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 06:09:59.257143 chat_agent-0.1.6.4/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1696 2023-04-05 16:42:52.000000 chat_agent-0.1.6.4/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.249328 chat_agent-0.1.6.4/chat_agent/
--rw-r--r--   0 alex       (501) staff       (20)     2727 2023-04-05 16:35:58.000000 chat_agent-0.1.6.4/chat_agent/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2881 2023-04-03 16:26:46.000000 chat_agent-0.1.6.4/chat_agent/app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.250437 chat_agent-0.1.6.4/chat_agent/base/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.4/chat_agent/base/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3428 2023-04-08 05:50:23.000000 chat_agent-0.1.6.4/chat_agent/base/base_websocket.py
--rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.4/chat_agent/base/singleton.py
--rw-r--r--   0 alex       (501) staff       (20)     1536 2023-04-08 05:26:59.000000 chat_agent-0.1.6.4/chat_agent/base_websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.251128 chat_agent-0.1.6.4/chat_agent/cache/
--rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.4/chat_agent/cache/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.4/chat_agent/cache/cache_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.4/chat_agent/cert.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.251917 chat_agent-0.1.6.4/chat_agent/client/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.4/chat_agent/client/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1042 2023-04-08 02:45:20.000000 chat_agent-0.1.6.4/chat_agent/client/base_web_socket_client.py
--rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.4/chat_agent/client/web_socket_client.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.252152 chat_agent-0.1.6.4/chat_agent/config/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.4/chat_agent/config/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      410 2023-03-31 01:41:44.000000 chat_agent-0.1.6.4/chat_agent/config/config_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.4/chat_agent/favicon.ico
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.252528 chat_agent-0.1.6.4/chat_agent/handler/
--rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.4/chat_agent/handler/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4356 2023-04-05 05:33:47.000000 chat_agent-0.1.6.4/chat_agent/handler/openai_handler.py
--rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.4/chat_agent/key.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.252892 chat_agent-0.1.6.4/chat_agent/logger/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.4/chat_agent/logger/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.4/chat_agent/logger/logger_helper.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.253467 chat_agent-0.1.6.4/chat_agent/logs/
--rw-r--r--   0 alex       (501) staff       (20)     5176 2023-04-08 05:52:04.000000 chat_agent-0.1.6.4/chat_agent/logs/base_websocket.log
--rw-r--r--   0 alex       (501) staff       (20)   111129 2023-04-08 05:52:02.000000 chat_agent-0.1.6.4/chat_agent/logs/chat_agent.handler.openai_handler.log
--rw-r--r--   0 alex       (501) staff       (20)     6129 2023-04-08 05:52:04.000000 chat_agent-0.1.6.4/chat_agent/logs/websocket_app.log
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.253863 chat_agent-0.1.6.4/chat_agent/static/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.254969 chat_agent-0.1.6.4/chat_agent/static/icon/
--rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.4/chat_agent/static/icon/openai.png
--rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.4/chat_agent/static/icon/whale.png
--rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.4/chat_agent/static/index.html
--rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.4/chat_agent/static/websocket_index.html
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.255213 chat_agent-0.1.6.4/chat_agent/test/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.4/chat_agent/test/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.256899 chat_agent-0.1.6.4/chat_agent/util/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.4/chat_agent/util/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.4/chat_agent/util/context.py
--rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.4/chat_agent/util/file.py
--rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.4/chat_agent/util/random.py
--rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.4/chat_agent/util/time.py
--rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.4/chat_agent/util/timeout.py
--rw-r--r--   0 alex       (501) staff       (20)     2956 2023-04-07 05:26:50.000000 chat_agent-0.1.6.4/chat_agent/websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 06:09:59.249963 chat_agent-0.1.6.4/chat_agent.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 06:09:59.000000 chat_agent-0.1.6.4/chat_agent.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1269 2023-04-08 06:09:59.000000 chat_agent-0.1.6.4/chat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-08 06:09:59.000000 chat_agent-0.1.6.4/chat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      269 2023-04-08 06:09:59.000000 chat_agent-0.1.6.4/chat_agent.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2023-04-08 06:09:59.000000 chat_agent-0.1.6.4/chat_agent.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-08 06:09:59.257375 chat_agent-0.1.6.4/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      874 2023-04-08 06:09:14.000000 chat_agent-0.1.6.4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.451400 chat_agent-0.1.6.5/
+-rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.5/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 16:52:22.451130 chat_agent-0.1.6.5/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1696 2023-04-08 16:48:02.000000 chat_agent-0.1.6.5/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.444129 chat_agent-0.1.6.5/chat_agent/
+-rw-r--r--   0 alex       (501) staff       (20)     2755 2023-04-08 16:47:51.000000 chat_agent-0.1.6.5/chat_agent/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2881 2023-04-03 16:26:46.000000 chat_agent-0.1.6.5/chat_agent/app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.445245 chat_agent-0.1.6.5/chat_agent/base/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.5/chat_agent/base/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3843 2023-04-08 16:45:47.000000 chat_agent-0.1.6.5/chat_agent/base/base_websocket.py
+-rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.5/chat_agent/base/singleton.py
+-rw-r--r--   0 alex       (501) staff       (20)     1536 2023-04-08 05:26:59.000000 chat_agent-0.1.6.5/chat_agent/base_websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.445901 chat_agent-0.1.6.5/chat_agent/cache/
+-rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.5/chat_agent/cache/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.5/chat_agent/cache/cache_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/cert.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.446466 chat_agent-0.1.6.5/chat_agent/client/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.5/chat_agent/client/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1055 2023-04-08 16:50:23.000000 chat_agent-0.1.6.5/chat_agent/client/base_web_socket_client.py
+-rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.5/chat_agent/client/web_socket_client.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.446696 chat_agent-0.1.6.5/chat_agent/config/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/config/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      605 2023-04-08 16:45:47.000000 chat_agent-0.1.6.5/chat_agent/config/config_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/favicon.ico
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.447154 chat_agent-0.1.6.5/chat_agent/handler/
+-rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.5/chat_agent/handler/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4356 2023-04-05 05:33:47.000000 chat_agent-0.1.6.5/chat_agent/handler/openai_handler.py
+-rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/key.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.447507 chat_agent-0.1.6.5/chat_agent/logger/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.5/chat_agent/logger/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.5/chat_agent/logger/logger_helper.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.448115 chat_agent-0.1.6.5/chat_agent/static/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.449063 chat_agent-0.1.6.5/chat_agent/static/icon/
+-rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/static/icon/openai.png
+-rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/static/icon/whale.png
+-rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.5/chat_agent/static/index.html
+-rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.5/chat_agent/static/websocket_index.html
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.449283 chat_agent-0.1.6.5/chat_agent/test/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.5/chat_agent/test/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.450927 chat_agent-0.1.6.5/chat_agent/util/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.5/chat_agent/util/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.5/chat_agent/util/context.py
+-rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.5/chat_agent/util/file.py
+-rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.5/chat_agent/util/random.py
+-rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.5/chat_agent/util/time.py
+-rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/util/timeout.py
+-rw-r--r--   0 alex       (501) staff       (20)     2956 2023-04-07 05:26:50.000000 chat_agent-0.1.6.5/chat_agent/websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.444766 chat_agent-0.1.6.5/chat_agent.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1146 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      269 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-08 16:52:22.451448 chat_agent-0.1.6.5/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      874 2023-04-08 16:47:51.000000 chat_agent-0.1.6.5/setup.py
```

### Comparing `chat_agent-0.1.6.4/README.md` & `chat_agent-0.1.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 简单的OpenAI chatGPT代理
 
 ### 安装
 ```
 使用pip安装最新版本，指定到官方pypi源
-pip install chat-agent==0.1.6.3 -i https://pypi.org/simple/
+pip install chat-agent==0.1.6.5 -i https://pypi.org/simple/
 ```
 
 ### 环境变量配置项：
 ```
 必配：
 OPENAI_ORGANIZATION_KEY: openai对应的组织id
 OPENAI_API_KEY: openai分配的api key
```

### Comparing `chat_agent-0.1.6.4/chat_agent/__init__.py` & `chat_agent-0.1.6.5/chat_agent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 CHAT_AGENT_HTTPS_DEFAULT = False
 CHAT_AGENT_SSL_CERT_FILE_FULL_PATH_DEFAULT = 'cert.pem'
 CHAT_AGENT_SSL_KEY_FILE_FULL_PATH_DEFAULT = 'key.pem'
 CHAT_AGENT_STATIC_PATH_DEFAULT = 'static'
 CHAT_AGENT_TIMEOUT_DEFAULT = 30
 
 CHAT_AGENT_HOST = config_helper.get_config_from_env(CHAT_AGENT_HOST_KEY, CHAT_AGENT_HOST_DEFAULT)
-CHAT_AGENT_PORT = config_helper.get_config_from_env(CHAT_AGENT_PORT_KEY, CHAT_AGENT_PORT_DEFAULT)
-CHAT_AGENT_HTTPS_PORT = config_helper.get_config_from_env(CHAT_AGENT_HTTPS_PORT_KEY, CHAT_AGENT_HTTPS_PORT_DEFAULT)
-CHAT_AGENT_WEBSOCKET_PORT = config_helper.get_config_from_env(CHAT_AGENT_WEBSOCKET_PORT_KEY,
-                                                              CHAT_AGENT_WEBSOCKET_PORT_DEFAULT)
-CHAT_AGENT_WEBSOCKET_WSS_PORT = config_helper.get_config_from_env(CHAT_AGENT_WEBSOCKET_WSS_PORT_KEY,
-                                                                  CHAT_AGENT_WEBSOCKET_WSS_PORT_DEFAULT)
+CHAT_AGENT_PORT = config_helper.get_int_config_from_env(CHAT_AGENT_PORT_KEY, CHAT_AGENT_PORT_DEFAULT)
+CHAT_AGENT_HTTPS_PORT = config_helper.get_int_config_from_env(CHAT_AGENT_HTTPS_PORT_KEY, CHAT_AGENT_HTTPS_PORT_DEFAULT)
+CHAT_AGENT_WEBSOCKET_PORT = config_helper.get_int_config_from_env(CHAT_AGENT_WEBSOCKET_PORT_KEY,
+                                                                  CHAT_AGENT_WEBSOCKET_PORT_DEFAULT)
+CHAT_AGENT_WEBSOCKET_WSS_PORT = config_helper.get_int_config_from_env(CHAT_AGENT_WEBSOCKET_WSS_PORT_KEY,
+                                                                      CHAT_AGENT_WEBSOCKET_WSS_PORT_DEFAULT)
 CHAT_AGENT_SECRET_KEY = config_helper.get_config_from_env(CHAT_AGENT_SECRET_KEY, CHAT_AGENT_SECRET_KEY_DEFAULT)
 CHAT_AGENT_HTTPS = config_helper.get_boolean_config_from_env(CHAT_AGENT_HTTPS_KEY, CHAT_AGENT_HTTPS_DEFAULT)
 CHAT_AGENT_SSL_CERT_FILE_FULL_PATH = config_helper.get_config_from_env(CHAT_AGENT_SSL_CERT_FILE_FULL_PATH_KEY,
                                                                        CHAT_AGENT_SSL_CERT_FILE_FULL_PATH_DEFAULT)
 CHAT_AGENT_SSL_KEY_FILE_FULL_PATH = config_helper.get_config_from_env(CHAT_AGENT_SSL_KEY_FILE_FULL_PATH_KEY,
                                                                       CHAT_AGENT_SSL_KEY_FILE_FULL_PATH_DEFAULT)
 CHAT_AGENT_STATIC_PATH = config_helper.get_config_from_env(CHAT_AGENT_STATIC_PATH_KEY, CHAT_AGENT_STATIC_PATH_DEFAULT)
-CHAT_AGENT_TIMEOUT = config_helper.get_config_from_env(CHAT_AGENT_TIMEOUT_KEY, CHAT_AGENT_TIMEOUT_DEFAULT)
+CHAT_AGENT_TIMEOUT = config_helper.get_int_config_from_env(CHAT_AGENT_TIMEOUT_KEY, CHAT_AGENT_TIMEOUT_DEFAULT)
```

### Comparing `chat_agent-0.1.6.4/chat_agent/app.py` & `chat_agent-0.1.6.5/chat_agent/app.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/base/base_websocket.py` & `chat_agent-0.1.6.5/chat_agent/base/base_websocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+from collections import OrderedDict
 
 from geventwebsocket import WebSocketServer, WebSocketApplication, Resource
+from geventwebsocket.handler import WebSocketHandler
 
 from chat_agent.base.singleton import Singleton
 from chat_agent.logger.logger_helper import get_logger
 from chat_agent.util.context import get_thread_context
 from chat_agent.util.random import get_random_md5
 
 logger = get_logger('base_websocket')
@@ -54,14 +56,22 @@
     context = get_thread_context()
     if 'socket' not in context:
         return None
     socket = context['socket']
     return socket.remote_addr
 
 
+class CustomWebSocketHandler(WebSocketHandler):
+    def handle_one_response(self):
+        try:
+            super(CustomWebSocketHandler, self).handle_one_response()
+        except Exception as e:
+            logger.error("捕获到异常：{}".format(e))
+
+
 @Singleton
 class BaseWebSocketServer:
 
     def __init__(self, *args, **kwargs):
         self.sockets = {}
         self.handlers = {}
 
@@ -99,19 +109,23 @@
             return handler
 
         return decorator
 
     def start(self, host: str = '0.0.0.0', port: int = 9080):
         WebSocketServer(
             (host, port),
-            Resource({'/': BaseWebSocket})
+            Resource(OrderedDict([('/', BaseWebSocket)])),
+            handler_class=CustomWebSocketHandler
         ).serve_forever()
 
 
 if __name__ == '__main__':
     server = BaseWebSocketServer()
 
+
     @server.on("websocket_chat")
     def say_hello(data):
         logger.debug('receive message,', data)
         send_message("websocket_chat", "nice to meet you")
+
+
     server.start()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chat_agent-0.1.6.4/chat_agent/base_websocket_app.py` & `chat_agent-0.1.6.5/chat_agent/base_websocket_app.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/cache/cache_helper.py` & `chat_agent-0.1.6.5/chat_agent/cache/cache_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/cert.pem` & `chat_agent-0.1.6.5/chat_agent/cert.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/client/base_web_socket_client.py` & `chat_agent-0.1.6.5/chat_agent/client/base_web_socket_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print("Received message: {}".format(message))
 
 
 def on_error(ws, error):
     print("Error occurred: {}".format(error))
 
 
-def on_close(ws):
+def on_close(ws, status, msg):
     print("WebSocket connection closed")
 
 
 def on_open(ws):
     print("WebSocket connection opened")
 
     def run():
```

### Comparing `chat_agent-0.1.6.4/chat_agent/client/web_socket_client.py` & `chat_agent-0.1.6.5/chat_agent/client/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/favicon.ico` & `chat_agent-0.1.6.5/chat_agent/favicon.ico`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/handler/__init__.py` & `chat_agent-0.1.6.5/chat_agent/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/handler/openai_handler.py` & `chat_agent-0.1.6.5/chat_agent/handler/openai_handler.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/key.pem` & `chat_agent-0.1.6.5/chat_agent/key.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/logger/logger_helper.py` & `chat_agent-0.1.6.5/chat_agent/logger/logger_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/static/icon/openai.png` & `chat_agent-0.1.6.5/chat_agent/static/icon/openai.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/static/icon/whale.png` & `chat_agent-0.1.6.5/chat_agent/static/icon/whale.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/static/index.html` & `chat_agent-0.1.6.5/chat_agent/static/index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/static/websocket_index.html` & `chat_agent-0.1.6.5/chat_agent/static/websocket_index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/util/context.py` & `chat_agent-0.1.6.5/chat_agent/util/context.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/util/timeout.py` & `chat_agent-0.1.6.5/chat_agent/util/timeout.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent/websocket_app.py` & `chat_agent-0.1.6.5/chat_agent/websocket_app.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.4/chat_agent.egg-info/SOURCES.txt` & `chat_agent-0.1.6.5/chat_agent.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 chat_agent/client/web_socket_client.py
 chat_agent/config/__init__.py
 chat_agent/config/config_helper.py
 chat_agent/handler/__init__.py
 chat_agent/handler/openai_handler.py
 chat_agent/logger/__init__.py
 chat_agent/logger/logger_helper.py
-chat_agent/logs/base_websocket.log
-chat_agent/logs/chat_agent.handler.openai_handler.log
-chat_agent/logs/websocket_app.log
 chat_agent/static/index.html
 chat_agent/static/websocket_index.html
 chat_agent/static/icon/openai.png
 chat_agent/static/icon/whale.png
 chat_agent/test/__init__.py
 chat_agent/util/__init__.py
 chat_agent/util/context.py
```

### Comparing `chat_agent-0.1.6.4/setup.py` & `chat_agent-0.1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chat_agent",
-    version="0.1.6.4",
+    version="0.1.6.5",
     packages=find_packages(),
     zip_sage=False,
     include_package_data=True,
     install_requires=[
         'setuptools~=63.4.1',
         'flask~=2.2.2',
         'flask_cors~=3.0.10',
```

