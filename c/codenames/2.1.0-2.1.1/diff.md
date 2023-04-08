# Comparing `tmp/codenames-2.1.0.tar.gz` & `tmp/codenames-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codenames-2.1.0.tar", last modified: Sat Apr  8 21:43:22 2023, max compression
+gzip compressed data, was "codenames-2.1.1.tar", last modified: Sat Apr  8 21:49:22 2023, max compression
```

## Comparing `codenames-2.1.0.tar` & `codenames-2.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.349290 codenames-2.1.0/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:43:22.349290 codenames-2.1.0/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-2.1.0/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-2.1.0/codenames/__init__.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames/boards/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:47.000000 codenames-2.1.0/codenames/boards/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2010 2023-04-08 14:40:42.000000 codenames-2.1.0/codenames/boards/builder.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-2.1.0/codenames/boards/english.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-2.1.0/codenames/boards/hebrew.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames/game/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:44.000000 codenames-2.1.0/codenames/game/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1015 2023-04-08 14:33:58.000000 codenames-2.1.0/codenames/game/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4103 2023-04-08 14:42:14.000000 codenames-2.1.0/codenames/game/board.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      928 2023-04-08 14:41:06.000000 codenames-2.1.0/codenames/game/card.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1200 2023-04-08 14:41:15.000000 codenames-2.1.0/codenames/game/color.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-2.1.0/codenames/game/exceptions.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2319 2023-04-08 14:59:45.000000 codenames-2.1.0/codenames/game/move.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2710 2023-04-08 21:36:30.000000 codenames-2.1.0/codenames/game/player.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     5041 2023-04-08 21:41:55.000000 codenames-2.1.0/codenames/game/runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      830 2023-04-08 14:40:42.000000 codenames-2.1.0/codenames/game/score.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    10106 2023-04-08 15:11:15.000000 codenames-2.1.0/codenames/game/state.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      452 2023-04-08 14:40:42.000000 codenames-2.1.0/codenames/game/winner.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames/online/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:49:02.000000 codenames-2.1.0/codenames/online/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    13115 2023-04-08 14:59:45.000000 codenames-2.1.0/codenames/online/online_adapter.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7862 2023-04-08 14:51:10.000000 codenames-2.1.0/codenames/online/online_game_runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1090 2023-04-08 14:50:37.000000 codenames-2.1.0/codenames/online/online_players.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-2.1.0/codenames/online/utils.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:59:11.000000 codenames-2.1.0/codenames/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      281 2023-04-08 21:36:52.000000 codenames-2.1.0/codenames/utils/formatting.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.345289 codenames-2.1.0/codenames.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:43:22.000000 codenames-2.1.0/codenames.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)     1137 2023-04-08 21:43:22.000000 codenames-2.1.0/codenames.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 21:43:22.000000 codenames-2.1.0/codenames.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      110 2023-04-08 21:43:22.000000 codenames-2.1.0/codenames.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-08 21:43:22.000000 codenames-2.1.0/codenames.egg-info/top_level.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      728 2023-04-08 08:52:53.000000 codenames-2.1.0/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 21:43:22.349290 codenames-2.1.0/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      554 2023-04-08 21:43:01.000000 codenames-2.1.0/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.349290 codenames-2.1.0/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-2.1.0/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1674 2023-04-08 14:23:07.000000 codenames-2.1.0/tests/board_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      750 2023-04-08 14:40:42.000000 codenames-2.1.0/tests/card_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8015 2023-04-08 14:48:49.000000 codenames-2.1.0/tests/flows_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8668 2023-04-08 21:41:54.000000 codenames-2.1.0/tests/game_runner_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7664 2023-04-08 15:12:37.000000 codenames-2.1.0/tests/game_state_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      805 2023-04-08 21:36:49.000000 codenames-2.1.0/tests/player_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      682 2023-04-08 14:40:42.000000 codenames-2.1.0/tests/serialization_test.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:43:22.349290 codenames-2.1.0/tests/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-2.1.0/tests/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3735 2023-04-08 14:40:42.000000 codenames-2.1.0/tests/utils/constants.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-2.1.0/tests/utils/hooks.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2823 2023-04-08 14:41:21.000000 codenames-2.1.0/tests/utils/testing_players.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.972485 codenames-2.1.1/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:49:22.972485 codenames-2.1.1/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-2.1.1/README.md
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/__init__.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames/boards/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:47.000000 codenames-2.1.1/codenames/boards/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2010 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/boards/builder.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/boards/english.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/boards/hebrew.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/game/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:44.000000 codenames-2.1.1/codenames/game/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1015 2023-04-08 14:33:58.000000 codenames-2.1.1/codenames/game/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4103 2023-04-08 14:42:14.000000 codenames-2.1.1/codenames/game/board.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      928 2023-04-08 14:41:06.000000 codenames-2.1.1/codenames/game/card.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1200 2023-04-08 14:41:15.000000 codenames-2.1.1/codenames/game/color.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/game/exceptions.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2319 2023-04-08 21:46:43.000000 codenames-2.1.1/codenames/game/move.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2710 2023-04-08 21:36:30.000000 codenames-2.1.1/codenames/game/player.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     5041 2023-04-08 21:41:55.000000 codenames-2.1.1/codenames/game/runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      830 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/game/score.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    10106 2023-04-08 15:11:15.000000 codenames-2.1.1/codenames/game/state.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      452 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/game/winner.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/online/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:49:02.000000 codenames-2.1.1/codenames/online/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    13115 2023-04-08 14:59:45.000000 codenames-2.1.1/codenames/online/online_adapter.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7862 2023-04-08 14:51:10.000000 codenames-2.1.1/codenames/online/online_game_runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1090 2023-04-08 14:50:37.000000 codenames-2.1.1/codenames/online/online_players.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/online/utils.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:59:11.000000 codenames-2.1.1/codenames/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      281 2023-04-08 21:36:52.000000 codenames-2.1.1/codenames/utils/formatting.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1137 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      110 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/top_level.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      728 2023-04-08 08:52:53.000000 codenames-2.1.1/pyproject.toml
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 21:49:22.972485 codenames-2.1.1/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      554 2023-04-08 21:49:00.000000 codenames-2.1.1/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/tests/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-2.1.1/tests/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1674 2023-04-08 14:23:07.000000 codenames-2.1.1/tests/board_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      750 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/card_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8015 2023-04-08 14:48:49.000000 codenames-2.1.1/tests/flows_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8668 2023-04-08 21:41:54.000000 codenames-2.1.1/tests/game_runner_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7664 2023-04-08 15:12:37.000000 codenames-2.1.1/tests/game_state_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      805 2023-04-08 21:36:49.000000 codenames-2.1.1/tests/player_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      682 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/serialization_test.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/tests/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-2.1.1/tests/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     3735 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/utils/constants.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-2.1.1/tests/utils/hooks.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2823 2023-04-08 14:41:21.000000 codenames-2.1.1/tests/utils/testing_players.py
```

### Comparing `codenames-2.1.0/PKG-INFO` & `codenames-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 2.1.0
+Version: 2.1.1
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-2.1.0/codenames/boards/builder.py` & `codenames-2.1.1/codenames/boards/builder.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/boards/english.py` & `codenames-2.1.1/codenames/boards/english.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/boards/hebrew.py` & `codenames-2.1.1/codenames/boards/hebrew.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/base.py` & `codenames-2.1.1/codenames/game/base.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/board.py` & `codenames-2.1.1/codenames/game/board.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/card.py` & `codenames-2.1.1/codenames/game/card.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/color.py` & `codenames-2.1.1/codenames/game/color.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/move.py` & `codenames-2.1.1/codenames/game/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 class GivenGuess(BaseModel):
     given_hint: GivenHint
     guessed_card: Card
 
     def __str__(self) -> str:
-        result = "Correct!" if self.correct else "Wrong!"
+        result = "correct!" if self.correct else "wrong!"
         return f"'{self.guessed_card}', {result}"
 
     @property
     def correct(self) -> bool:
         return self.team.as_card_color == self.guessed_card.color
 
     def dict(self, *args, **kwargs) -> dict:
```

### Comparing `codenames-2.1.0/codenames/game/player.py` & `codenames-2.1.1/codenames/game/player.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/runner.py` & `codenames-2.1.1/codenames/game/runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/score.py` & `codenames-2.1.1/codenames/game/score.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/game/state.py` & `codenames-2.1.1/codenames/game/state.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/online/online_adapter.py` & `codenames-2.1.1/codenames/online/online_adapter.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/online/online_game_runner.py` & `codenames-2.1.1/codenames/online/online_game_runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/online/online_players.py` & `codenames-2.1.1/codenames/online/online_players.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames/online/utils.py` & `codenames-2.1.1/codenames/online/utils.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/codenames.egg-info/PKG-INFO` & `codenames-2.1.1/codenames.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 2.1.0
+Version: 2.1.1
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-2.1.0/codenames.egg-info/SOURCES.txt` & `codenames-2.1.1/codenames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/pyproject.toml` & `codenames-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/setup.py` & `codenames-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "beautifultable~=1.0",
 ]
 WEB_DEPS = ["selenium~=4.1"]
 ALL_DEPS = BASE_DEPS + WEB_DEPS
 
 setup(
     name="codenames",
-    version="2.1.0",
+    version="2.1.1",
     description="Codenames board game logic implementation in python.",
     author="Asaf Kali",
     author_email="akali93@gmail.com",
     url="https://github.com/asaf-kali/codenames",
     install_requires=BASE_DEPS,
     extras_require={
         "all": ALL_DEPS,
```

### Comparing `codenames-2.1.0/tests/board_test.py` & `codenames-2.1.1/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/card_test.py` & `codenames-2.1.1/tests/card_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/flows_test.py` & `codenames-2.1.1/tests/flows_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/game_runner_test.py` & `codenames-2.1.1/tests/game_runner_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/game_state_test.py` & `codenames-2.1.1/tests/game_state_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/player_test.py` & `codenames-2.1.1/tests/player_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/serialization_test.py` & `codenames-2.1.1/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/utils/constants.py` & `codenames-2.1.1/tests/utils/constants.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/utils/hooks.py` & `codenames-2.1.1/tests/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.0/tests/utils/testing_players.py` & `codenames-2.1.1/tests/utils/testing_players.py`

 * *Files identical despite different names*

