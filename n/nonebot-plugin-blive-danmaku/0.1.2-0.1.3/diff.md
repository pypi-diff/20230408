# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.2.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.2.tar` & `nonebot_plugin_blive_danmaku-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.2/LICENSE
--rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       67 2023-04-07 19:00:18.585303 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0     2837 2023-04-07 19:41:42.478829 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/pusher.py
--rw-r--r--   0        0        0     1407 2023-04-07 18:48:25.619184 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_add.py
--rw-r--r--   0        0        0     1396 2023-04-07 18:49:55.897456 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_delete.py
--rw-r--r--   0        0        0      916 2023-04-07 18:53:16.447915 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_list.py
--rw-r--r--   0        0        0      829 2023-04-07 18:52:14.308552 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_off.py
--rw-r--r--   0        0        0      820 2023-04-07 18:50:57.288389 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_on.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     1953 2023-04-07 19:33:48.683619 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3289 2023-04-07 19:01:53.281128 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      950 2023-04-07 19:51:23.975973 nonebot_plugin_blive_danmaku-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    59274 2023-04-07 19:51:27.937112 nonebot_plugin_blive_danmaku-0.1.2/README.md
--rw-r--r--   0        0        0    60383 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.3/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       67 2023-04-07 19:00:18.585303 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0     3111 2023-04-08 17:55:07.052693 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/pusher.py
+-rw-r--r--   0        0        0     1407 2023-04-07 18:48:25.619184 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_add.py
+-rw-r--r--   0        0        0     1396 2023-04-07 18:49:55.897456 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_delete.py
+-rw-r--r--   0        0        0      916 2023-04-07 18:53:16.447915 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_list.py
+-rw-r--r--   0        0        0      829 2023-04-07 18:52:14.308552 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_off.py
+-rw-r--r--   0        0        0      820 2023-04-07 18:50:57.288389 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_on.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     1953 2023-04-07 19:33:48.683619 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3752 2023-04-08 17:54:45.409318 nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-08 19:06:24.287928 nonebot_plugin_blive_danmaku-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1738 2023-04-08 19:03:48.106577 nonebot_plugin_blive_danmaku-0.1.3/README.md
+-rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/pusher.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/pusher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import time
 import asyncio
-from bilireq.live import get_rooms_info_by_uids
-from ..utils import send_msg
+from bilireq.live import get_rooms_info_by_uids, get_room_info_by_id
+from ..utils import send_msg, get_timespan, get_time_difference
 from ..blivedm import blivedm
 from ..database import Db as db
 from nonebot.log import logger
-from nonebot import require
+from nonebot import require, get_driver
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 
 class ClientModel:
     def __init__(self, room_id):
         self.uid=""
         self.name=""
+        self.live_time=0
         self.client=blivedm.BLiveClient(room_id)
 
 
 clients = []
 
 
 @scheduler.scheduled_job(
@@ -38,19 +39,21 @@
     for uid, info in res.items():
         new_status = 0 if info["live_status"] == 2 else info["live_status"]
         index = [x for x in clients if x.uid == uid]
         if not index:
             if new_status:
                 logger.info(f'{info["uname"]}开播了，连接直播间')
                 room_id = info["short_id"] if info["short_id"] else info["room_id"]
+                room_info = await get_room_info_by_id(room_id, reqtype="web")
                 model = ClientModel(room_id)
                 model.client.add_handler(handler)
                 model.client.start()
                 model.uid=uid
                 model.name=info["uname"]
+                model.live_time=get_timespan(room_info["live_time"])
                 clients.append(model)
         else:
             if new_status == 0:
                 model = index[0]
                 client = model.client
                 try:
                     asyncio.gather(client.join())
@@ -64,13 +67,14 @@
     async def _on_danmaku(self, client: blivedm.BLiveClient, message: blivedm.DanmakuMessage):
         if(message.msg.startswith("#路灯")):
             subs = await db.get_subs(uid=client.room_owner_uid)
             if not subs:
                 return
             for sub in subs:
                 index = [x for x in clients if x.uid == str(sub.uid)]
-                logger.info(index)
                 model = index[0]
                 logger.info(f'{model.name}的直播间收到路灯：{message.uname} -> {message.msg}')
+                dt = get_time_difference(model.live_time)
                 datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-                msg = f'【{model.name}】 在 {datetime} 收到了 {message.uname} 发来的路灯【{message.msg.replace("#路灯","", 1).strip()}】'
+                msg = f'【{model.name}】 在 {datetime}({dt}) 收到了 {message.uname} 发来的路灯【{message.msg.replace("#路灯","", 1).strip()}】'
                 await send_msg(bot_id=sub.bot_id,send_type=sub.type,type_id=sub.type_id,message=msg)
+
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_add.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_list.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_off.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_on.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/command/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.3/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import nonebot
+import time
 from pathlib import Path
 from typing import Union
-import nonebot
 from nonebot import require
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
     Bot,
@@ -88,7 +89,23 @@
     return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
 
 
 def on_startup():
     if not Path(get_path()).is_dir():
             Path(get_path()).mkdir(parents=True)
 
+def get_timespan(time_str):
+    """字符串转时间戳"""
+    time_array = time.strptime(time_str,"%Y-%m-%d %H:%M:%S")
+    res = int(time.mktime(time_array))
+    return res
+
+
+def get_time_difference(live_time: int):
+    """计算开播时间到当前时间的时间差"""
+    now = int(time.time())
+    sub = now - live_time
+    m, s = divmod(sub, 60)
+    h, m = divmod(m, 60)
+    dt = ("%02d:%02d:%02d" % (h, m, s))
+    return dt
+
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.2/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.2"
+version = "0.1.3"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

