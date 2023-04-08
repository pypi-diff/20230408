# Comparing `tmp/SteamPlayerCharts-0.2-py3-none-any.whl.zip` & `tmp/SteamPlayerCharts-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,7 @@
-Zip file size: 1546 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat     1185 b- defN 23-Apr-07 22:58 SteamPlayerCharts-0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 22:58 SteamPlayerCharts-0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-07 22:58 SteamPlayerCharts-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      329 b- defN 23-Apr-07 22:58 SteamPlayerCharts-0.2.dist-info/RECORD
-4 files, 1611 bytes uncompressed, 900 bytes compressed:  44.1%
+Zip file size: 2308 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1253 b- defN 23-Apr-07 20:19 SteamCharts.py
+-rw-rw-rw-  2.0 fat     1208 b- defN 23-Apr-07 23:21 SteamPlayerCharts-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 23:21 SteamPlayerCharts-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-07 23:21 SteamPlayerCharts-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      409 b- defN 23-Apr-07 23:21 SteamPlayerCharts-0.2.1.dist-info/RECORD
+5 files, 2974 bytes uncompressed, 1542 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
-Filename: SteamPlayerCharts-0.2.dist-info/METADATA
+Filename: SteamCharts.py
 Comment: 
 
-Filename: SteamPlayerCharts-0.2.dist-info/WHEEL
+Filename: SteamPlayerCharts-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: SteamPlayerCharts-0.2.dist-info/top_level.txt
+Filename: SteamPlayerCharts-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: SteamPlayerCharts-0.2.dist-info/RECORD
+Filename: SteamPlayerCharts-0.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: SteamPlayerCharts-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `SteamPlayerCharts-0.2.dist-info/METADATA` & `SteamPlayerCharts-0.2.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SteamPlayerCharts
-Version: 0.2
+Version: 0.2.1
 Summary: A Python wrapper for SteamCharts
 Author: Serpensin
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: beautifulsoup4
 
 # SteamCharts
@@ -16,15 +16,15 @@
 
 `pip install SteamPlayerCharts`
 
 
 ## Example
 ```python
 import asyncio
-import SteamCharts
+import SteamPlayerCharts as SteamCharts
 
 async def main():
 	steamgameID = "4000"
 	player_count = await SteamCharts.playercount(steamgameID)
 	print(player_count)
 	try:
 		current_players = player_count['Current Players']
```

