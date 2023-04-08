# Comparing `tmp/codenames-2.0.1.tar.gz` & `tmp/codenames-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codenames-2.0.1.tar", last modified: Sat Apr  8 15:00:44 2023, max compression
+gzip compressed data, was "codenames-2.0.2.tar", last modified: Sat Apr  8 15:14:35 2023, max compression
```

## Comparing `codenames-2.0.1.tar` & `codenames-2.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.726104 codenames-2.0.1/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 15:00:44.726104 codenames-2.0.1/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-2.0.1/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.718104 codenames-2.0.1/codenames/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-2.0.1/codenames/__init__.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.722104 codenames-2.0.1/codenames/boards/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:47.000000 codenames-2.0.1/codenames/boards/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2010 2023-04-08 14:40:42.000000 codenames-2.0.1/codenames/boards/builder.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-2.0.1/codenames/boards/english.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-2.0.1/codenames/boards/hebrew.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.722104 codenames-2.0.1/codenames/game/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:44.000000 codenames-2.0.1/codenames/game/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1015 2023-04-08 14:33:58.000000 codenames-2.0.1/codenames/game/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4103 2023-04-08 14:42:14.000000 codenames-2.0.1/codenames/game/board.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      928 2023-04-08 14:41:06.000000 codenames-2.0.1/codenames/game/card.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1200 2023-04-08 14:41:15.000000 codenames-2.0.1/codenames/game/color.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-2.0.1/codenames/game/exceptions.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2319 2023-04-08 14:59:45.000000 codenames-2.0.1/codenames/game/move.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2308 2023-04-08 14:41:21.000000 codenames-2.0.1/codenames/game/player.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4773 2023-04-08 14:59:45.000000 codenames-2.0.1/codenames/game/runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      830 2023-04-08 14:40:42.000000 codenames-2.0.1/codenames/game/score.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     9808 2023-04-08 14:59:45.000000 codenames-2.0.1/codenames/game/state.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      452 2023-04-08 14:40:42.000000 codenames-2.0.1/codenames/game/winner.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.722104 codenames-2.0.1/codenames/online/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:49:02.000000 codenames-2.0.1/codenames/online/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    13115 2023-04-08 14:59:45.000000 codenames-2.0.1/codenames/online/online_adapter.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7862 2023-04-08 14:51:10.000000 codenames-2.0.1/codenames/online/online_game_runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1090 2023-04-08 14:50:37.000000 codenames-2.0.1/codenames/online/online_players.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-2.0.1/codenames/online/utils.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.722104 codenames-2.0.1/codenames/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:59:11.000000 codenames-2.0.1/codenames/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)       52 2023-04-08 14:59:44.000000 codenames-2.0.1/codenames/utils/formatting.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.718104 codenames-2.0.1/codenames.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 15:00:44.000000 codenames-2.0.1/codenames.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)     1137 2023-04-08 15:00:44.000000 codenames-2.0.1/codenames.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 15:00:44.000000 codenames-2.0.1/codenames.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      110 2023-04-08 15:00:44.000000 codenames-2.0.1/codenames.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-08 15:00:44.000000 codenames-2.0.1/codenames.egg-info/top_level.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      728 2023-04-08 08:52:53.000000 codenames-2.0.1/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 15:00:44.726104 codenames-2.0.1/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      554 2023-04-08 15:00:16.000000 codenames-2.0.1/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.726104 codenames-2.0.1/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-2.0.1/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1674 2023-04-08 14:23:07.000000 codenames-2.0.1/tests/board_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      750 2023-04-08 14:40:42.000000 codenames-2.0.1/tests/card_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8015 2023-04-08 14:48:49.000000 codenames-2.0.1/tests/flows_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8017 2023-04-08 14:41:21.000000 codenames-2.0.1/tests/game_runner_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7210 2023-04-08 14:48:49.000000 codenames-2.0.1/tests/game_state_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      822 2023-04-08 14:41:21.000000 codenames-2.0.1/tests/player_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      682 2023-04-08 14:40:42.000000 codenames-2.0.1/tests/serialization_test.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:00:44.726104 codenames-2.0.1/tests/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-2.0.1/tests/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3735 2023-04-08 14:40:42.000000 codenames-2.0.1/tests/utils/constants.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-2.0.1/tests/utils/hooks.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2823 2023-04-08 14:41:21.000000 codenames-2.0.1/tests/utils/testing_players.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 15:14:35.287190 codenames-2.0.2/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-2.0.2/README.md
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.283190 codenames-2.0.2/codenames/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-2.0.2/codenames/__init__.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.283190 codenames-2.0.2/codenames/boards/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:47.000000 codenames-2.0.2/codenames/boards/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2010 2023-04-08 14:40:42.000000 codenames-2.0.2/codenames/boards/builder.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-2.0.2/codenames/boards/english.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-2.0.2/codenames/boards/hebrew.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/codenames/game/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:44.000000 codenames-2.0.2/codenames/game/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1015 2023-04-08 14:33:58.000000 codenames-2.0.2/codenames/game/base.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4103 2023-04-08 14:42:14.000000 codenames-2.0.2/codenames/game/board.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      928 2023-04-08 14:41:06.000000 codenames-2.0.2/codenames/game/card.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1200 2023-04-08 14:41:15.000000 codenames-2.0.2/codenames/game/color.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-2.0.2/codenames/game/exceptions.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2319 2023-04-08 14:59:45.000000 codenames-2.0.2/codenames/game/move.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2308 2023-04-08 14:41:21.000000 codenames-2.0.2/codenames/game/player.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     4773 2023-04-08 14:59:45.000000 codenames-2.0.2/codenames/game/runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      830 2023-04-08 14:40:42.000000 codenames-2.0.2/codenames/game/score.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    10106 2023-04-08 15:11:15.000000 codenames-2.0.2/codenames/game/state.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      452 2023-04-08 14:40:42.000000 codenames-2.0.2/codenames/game/winner.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/codenames/online/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:49:02.000000 codenames-2.0.2/codenames/online/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)    13115 2023-04-08 14:59:45.000000 codenames-2.0.2/codenames/online/online_adapter.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7862 2023-04-08 14:51:10.000000 codenames-2.0.2/codenames/online/online_game_runner.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1090 2023-04-08 14:50:37.000000 codenames-2.0.2/codenames/online/online_players.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-2.0.2/codenames/online/utils.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/codenames/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:59:11.000000 codenames-2.0.2/codenames/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)       52 2023-04-08 14:59:44.000000 codenames-2.0.2/codenames/utils/formatting.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.283190 codenames-2.0.2/codenames.egg-info/
+-rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 15:14:35.000000 codenames-2.0.2/codenames.egg-info/PKG-INFO
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1137 2023-04-08 15:14:35.000000 codenames-2.0.2/codenames.egg-info/SOURCES.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 15:14:35.000000 codenames-2.0.2/codenames.egg-info/dependency_links.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      110 2023-04-08 15:14:35.000000 codenames-2.0.2/codenames.egg-info/requires.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-08 15:14:35.000000 codenames-2.0.2/codenames.egg-info/top_level.txt
+-rw-rw-r--   0 akali     (1000) akali     (1000)      728 2023-04-08 08:52:53.000000 codenames-2.0.2/pyproject.toml
+-rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 15:14:35.287190 codenames-2.0.2/setup.cfg
+-rw-rw-r--   0 akali     (1000) akali     (1000)      554 2023-04-08 15:14:21.000000 codenames-2.0.2/setup.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/tests/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-2.0.2/tests/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1674 2023-04-08 14:23:07.000000 codenames-2.0.2/tests/board_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      750 2023-04-08 14:40:42.000000 codenames-2.0.2/tests/card_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8015 2023-04-08 14:48:49.000000 codenames-2.0.2/tests/flows_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     8017 2023-04-08 14:41:21.000000 codenames-2.0.2/tests/game_runner_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     7664 2023-04-08 15:12:37.000000 codenames-2.0.2/tests/game_state_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      822 2023-04-08 14:41:21.000000 codenames-2.0.2/tests/player_test.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)      682 2023-04-08 14:40:42.000000 codenames-2.0.2/tests/serialization_test.py
+drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 15:14:35.287190 codenames-2.0.2/tests/utils/
+-rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-2.0.2/tests/utils/__init__.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     3735 2023-04-08 14:40:42.000000 codenames-2.0.2/tests/utils/constants.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-2.0.2/tests/utils/hooks.py
+-rw-rw-r--   0 akali     (1000) akali     (1000)     2823 2023-04-08 14:41:21.000000 codenames-2.0.2/tests/utils/testing_players.py
```

### Comparing `codenames-2.0.1/PKG-INFO` & `codenames-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 2.0.1
+Version: 2.0.2
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-2.0.1/codenames/boards/builder.py` & `codenames-2.0.2/codenames/boards/builder.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/boards/english.py` & `codenames-2.0.2/codenames/boards/english.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/boards/hebrew.py` & `codenames-2.0.2/codenames/boards/hebrew.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/base.py` & `codenames-2.0.2/codenames/game/base.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/board.py` & `codenames-2.0.2/codenames/game/board.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/card.py` & `codenames-2.0.2/codenames/game/card.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/color.py` & `codenames-2.0.2/codenames/game/color.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/move.py` & `codenames-2.0.2/codenames/game/move.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/player.py` & `codenames-2.0.2/codenames/game/player.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/runner.py` & `codenames-2.0.2/codenames/game/runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/score.py` & `codenames-2.0.2/codenames/game/score.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/game/state.py` & `codenames-2.0.2/codenames/game/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,29 @@
 
 
 class BaseGameState(BaseModel):
     language: str
     board: Board
     score: Score
     current_team_color: TeamColor = TeamColor.BLUE
+    current_player_role: PlayerRole = PlayerRole.HINTER
     given_hints: List[GivenHint] = []
     given_guesses: List[GivenGuess] = []
 
     class Config:
         abstract = True
 
-    @cached_property
+    @property
     def moves(self) -> List[Move]:
-        return get_moves(given_hints=self.given_hints, given_guesses=self.given_guesses)
+        return get_moves(
+            given_hints=self.given_hints, given_guesses=self.given_guesses, current_turn=self.current_player_role
+        )
 
 
 class GameState(BaseGameState):
-    current_player_role: PlayerRole = PlayerRole.HINTER
     left_guesses: int = 0
     bonus_given: bool = False
     winner: Optional[Winner] = None
     raw_hints: List[Hint] = []
 
     @root_validator(pre=True)
     def init_score(cls, values: dict) -> dict:  # pylint: disable=no-self-argument
@@ -73,25 +75,27 @@
     @property
     def hinter_state(self) -> "HinterGameState":
         return HinterGameState(
             language=self.language,
             board=self.board,
             score=self.score,
             current_team_color=self.current_team_color,
+            current_player_role=self.current_player_role,
             given_hints=self.given_hints,
             given_guesses=self.given_guesses,
         )
 
     @property
     def guesser_state(self) -> "GuesserGameState":
         return GuesserGameState(
             language=self.language,
             board=self.board.censured,
             score=self.score,
             current_team_color=self.current_team_color,
+            current_player_role=self.current_player_role,
             given_hints=self.given_hints,
             given_guesses=self.given_guesses,
             left_guesses=self.left_guesses,
             bonus_given=self.bonus_given,
         )
 
     @property
@@ -247,15 +251,15 @@
 
 def _determine_first_team(board: Board) -> TeamColor:
     if len(board.blue_cards) >= len(board.red_cards):
         return TeamColor.BLUE
     return TeamColor.RED
 
 
-def get_moves(given_hints: List[GivenHint], given_guesses: List[GivenGuess]) -> List[Move]:
+def get_moves(given_hints: List[GivenHint], given_guesses: List[GivenGuess], current_turn: PlayerRole) -> List[Move]:
     guesses_by_hints = get_guesses_by_hints(given_hints=given_hints, given_guesses=given_guesses)
     moves: List[Move] = []
     for hint, guesses in guesses_by_hints.items():
         hint_move = HintMove(given_hint=hint)
         moves.append(hint_move)
         for guess in guesses:
             guess_move = GuessMove(given_guess=guess)
@@ -265,15 +269,19 @@
             continue
         if len(guesses) < hint.card_amount + 1:
             last_guess = guesses[-1]
             if last_guess.correct:
                 moves.append(PassMove(team=hint.team_color))
     if not moves:
         return moves
-    # TODO: Determine if last pass move should be removed.
+    last_move = moves[-1]
+    if not isinstance(last_move, PassMove):
+        return moves
+    if current_turn == PlayerRole.GUESSER:
+        moves = moves[:-1]
     return moves
 
 
 def get_guesses_by_hints(
     given_hints: List[GivenHint], given_guesses: List[GivenGuess]
 ) -> Dict[GivenHint, List[GivenGuess]]:
     guesses_by_hints: Dict[GivenHint, List[GivenGuess]] = {}
```

### Comparing `codenames-2.0.1/codenames/online/online_adapter.py` & `codenames-2.0.2/codenames/online/online_adapter.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/online/online_game_runner.py` & `codenames-2.0.2/codenames/online/online_game_runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/online/online_players.py` & `codenames-2.0.2/codenames/online/online_players.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames/online/utils.py` & `codenames-2.0.2/codenames/online/utils.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/codenames.egg-info/PKG-INFO` & `codenames-2.0.2/codenames.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codenames
-Version: 2.0.1
+Version: 2.0.2
 Summary: Codenames board game logic implementation in python.
 Home-page: https://github.com/asaf-kali/codenames
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `codenames-2.0.1/codenames.egg-info/SOURCES.txt` & `codenames-2.0.2/codenames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/pyproject.toml` & `codenames-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/setup.py` & `codenames-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "beautifultable~=1.0",
 ]
 WEB_DEPS = ["selenium~=4.1"]
 ALL_DEPS = BASE_DEPS + WEB_DEPS
 
 setup(
     name="codenames",
-    version="2.0.1",
+    version="2.0.2",
     description="Codenames board game logic implementation in python.",
     author="Asaf Kali",
     author_email="akali93@gmail.com",
     url="https://github.com/asaf-kali/codenames",
     install_requires=BASE_DEPS,
     extras_require={
         "all": ALL_DEPS,
```

### Comparing `codenames-2.0.1/tests/board_test.py` & `codenames-2.0.2/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/card_test.py` & `codenames-2.0.2/tests/card_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/flows_test.py` & `codenames-2.0.2/tests/flows_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/game_runner_test.py` & `codenames-2.0.2/tests/game_runner_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/game_state_test.py` & `codenames-2.0.2/tests/game_state_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,73 +27,85 @@
     return constants.board_10()
 
 
 def test_game_state_flow(board_10: Board):
     game_state = build_game_state(language="en", board=board_10)
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.HINTER
+    assert game_state.moves == []
 
     # Round 1 - blue team
     game_state.process_hint(Hint(word="Hint 1", card_amount=2))
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 2
+    assert len(game_state.moves) == 1
 
     game_state.process_guess(Guess(card_index=0))  # Blue - Correct
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 1
     assert game_state.bonus_given is False
+    assert len(game_state.moves) == 2
 
     game_state.process_guess(Guess(card_index=1))  # Blue - Correct
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 1
     assert game_state.bonus_given is True
+    assert len(game_state.moves) == 3
 
     with pytest.raises(InvalidGuess):  # Card already guessed
         game_state.process_guess(Guess(card_index=1))
 
     game_state.process_guess(Guess(card_index=PASS_GUESS))  # Pass
     assert game_state.current_team_color == TeamColor.RED
     assert game_state.current_player_role == PlayerRole.HINTER
     assert game_state.left_guesses == 0
+    assert len(game_state.moves) == 4
 
     # Round 2 - red team
     game_state.process_hint(Hint(word="Hint 2", card_amount=1))
     assert game_state.current_team_color == TeamColor.RED
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 1
+    assert len(game_state.moves) == 5
 
     game_state.process_guess(Guess(card_index=4))  # Red - Correct
     assert game_state.current_team_color == TeamColor.RED
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 1
     assert game_state.bonus_given is True
+    assert len(game_state.moves) == 6
 
     game_state.process_guess(Guess(card_index=5))  # Red - Correct
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.HINTER
+    assert len(game_state.moves) == 7
 
     with pytest.raises(InvalidTurn):  # It's not the guesser's turn
         game_state.process_guess(Guess(card_index=8))
 
     # Round 3 - blue team
     game_state.process_hint(Hint(word="Hint 3", card_amount=2))
     assert game_state.current_team_color == TeamColor.BLUE
     assert game_state.current_player_role == PlayerRole.GUESSER
     assert game_state.left_guesses == 2
+    assert len(game_state.moves) == 8
 
     game_state.process_guess(Guess(card_index=PASS_GUESS))
     assert game_state.current_team_color == TeamColor.RED
     assert game_state.current_player_role == PlayerRole.HINTER
+    assert len(game_state.moves) == 9
 
     # Round 4 - red team
     game_state.process_hint(Hint(word="Hint 4", card_amount=2))
+    assert len(game_state.moves) == 10
     game_state.process_guess(Guess(card_index=9))  # Black - Game over
+    assert len(game_state.moves) == 11
     assert game_state.winner == Winner(team_color=TeamColor.BLUE, reason=WinningReason.OPPONENT_HIT_BLACK)
 
     with pytest.raises(InvalidTurn):  # Game is over
         game_state.process_hint(Hint(word="E", card_amount=1))
     with pytest.raises(InvalidTurn):  # Game is over
         game_state.process_guess(Guess(card_index=8))
```

### Comparing `codenames-2.0.1/tests/player_test.py` & `codenames-2.0.2/tests/player_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/serialization_test.py` & `codenames-2.0.2/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/utils/constants.py` & `codenames-2.0.2/tests/utils/constants.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/utils/hooks.py` & `codenames-2.0.2/tests/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `codenames-2.0.1/tests/utils/testing_players.py` & `codenames-2.0.2/tests/utils/testing_players.py`

 * *Files identical despite different names*

