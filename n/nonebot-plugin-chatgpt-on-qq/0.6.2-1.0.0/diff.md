# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-0.6.2.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-0.6.2.tar", last modified: Wed Mar 22 09:16:24 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.0.0.tar", last modified: Sat Apr  8 19:16:16 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2.tar` & `nonebot-plugin-chatgpt-on-qq-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 09:16:24.749189 nonebot-plugin-chatgpt-on-qq-0.6.2/
--rw-rw-rw-   0        0        0      769 2023-03-22 09:16:24.747209 nonebot-plugin-chatgpt-on-qq-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 09:16:24.728634 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    12548 2023-03-22 09:12:42.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3630 2023-03-15 12:15:37.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      358 2023-03-22 09:12:42.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     7255 2023-03-22 09:15:34.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     1969 2023-03-15 12:15:37.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/main.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:16:24.744233 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      769 2023-03-22 09:16:24.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-03-22 09:16:24.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 09:16:24.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-03-22 09:16:24.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-03-22 09:16:24.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 09:16:24.749189 nonebot-plugin-chatgpt-on-qq-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-03-22 09:15:57.000000 nonebot-plugin-chatgpt-on-qq-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.534462 nonebot-plugin-chatgpt-on-qq-1.0.0/
+-rw-rw-rw-   0        0        0      769 2023-04-08 19:16:16.532461 nonebot-plugin-chatgpt-on-qq-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.517738 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    12548 2023-03-22 09:12:42.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     3819 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
+-rw-rw-rw-   0        0        0      423 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0     7253 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/conversation.py
+-rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     1969 2023-03-15 12:15:37.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/main.py
+drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.528967 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      769 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 19:16:16.534462 nonebot-plugin-chatgpt-on-qq-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-08 19:15:49.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 0.6.2
+Version: 1.0.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,24 @@
 from .config import Config
 from .custom_errors import OverMaxTokenLengthError, NoResponseError, NoApiKeyError
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
 
 # ENCODER = tiktoken.get_encoding("gpt2")
 MAX_TOKEN = 4000
-MODEL = "gpt-3.5-turbo"
+
+if plugin_config.model_name:
+    MODEL = plugin_config.model_name
+else:
+    MODEL = "gpt-3.5-turbo"
+
+if plugin_config.temperature:
+    TEMPERATURE = plugin_config.temperature
+else:
+    TEMPERATURE = 0.5
 
 
 class PromptManager:
     def __init__(self,  basic_prompt, history_max: int) -> None:
         self.history: List[Dict[str, str]] = basic_prompt
         self.history_max = history_max
         self.basic_len = len(basic_prompt)
@@ -52,40 +61,40 @@
         except UnicodeEncodeError:
             jsonStr = json.dumps(self.history, ensure_ascii=True)
         return jsonStr
 
 
 class ChatGPTBot:
     def __init__(self, api_key: str, basic_prompt, history_max: int) -> None:
-        if api_key is not "NoKey":
+        if api_key:
             openai.api_key = api_key
         else:
             raise NoApiKeyError("未设置ApiKey")
         self.prompt_manager = PromptManager(
             basic_prompt=basic_prompt, history_max=history_max)
         self.talk_count = 0
 
     async def ask(
         self,
         user_input: str,
-        temperature: float = 0.5,
+        temperature: float = TEMPERATURE
     ) -> Dict:
 
         try:
             completion = await self._get_completion(user_input, temperature)
             await self._process_completion(completion=completion)
             return completion["choices"][0]["message"]["content"]
         except:
             self.prompt_manager.history.pop()
             raise ConnectionError
 
     async def _get_completion(
             self,
             user_input: str,
-            temperature: float = 0.5
+            temperature: float = TEMPERATURE
     ):
 
         return await openai.ChatCompletion.acreate(
             model=MODEL,
             messages=self.prompt_manager.construct_prompt(user_input),
             temperature=temperature,
             max_tokens=1000
```

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/conversation.py` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 from .config import Config
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
 # 设置代理
 proxy = plugin_config.openai_proxy
 api_base = plugin_config.openai_api_base
 
-if proxy == None:
-    logger.error("请设置代理!")
+if not proxy:
+    logger.warning("插件未设置代理。")
 elif proxy=="NoError":
     pass
 else:
     openai.proxy = {'http': f"http://{proxy}", 'https': f'http://{proxy}'}
-if api_base != None:
+if api_base:
     openai.api_base = api_base
 
 # 设置保存路径
 START_TIME = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
 SAVE_PATH: Path = plugin_config.history_save_path.joinpath(START_TIME)
 # 设置管理员
 ADMIN = plugin_config.admin
```

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq/main.py` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/main.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 0.6.2
+Version: 1.0.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt` & `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-0.6.2/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='0.6.2',
+    version='1.0.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

