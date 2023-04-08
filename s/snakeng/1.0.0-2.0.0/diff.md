# Comparing `tmp/snakeng-1.0.0-py3-none-any.whl.zip` & `tmp/snakeng-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13556 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       22 b- defN 23-Mar-31 03:34 snakeng/__init__.py
--rw-rw-rw-  2.0 fat     4684 b- defN 23-Mar-31 03:28 snakeng/__main__.py
--rw-rw-rw-  2.0 fat    18058 b- defN 23-Mar-31 03:30 snakeng/snake.py
--rw-rw-rw-  2.0 fat    10761 b- defN 23-Mar-31 03:37 snakeng-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6261 b- defN 23-Mar-31 03:37 snakeng-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-31 03:37 snakeng-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-31 03:37 snakeng-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      610 b- defN 23-Mar-31 03:37 snakeng-1.0.0.dist-info/RECORD
-8 files, 40496 bytes uncompressed, 12500 bytes compressed:  69.1%
+Zip file size: 13550 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-08 18:21 snakeng/__init__.py
+-rw-rw-rw-  2.0 fat     4644 b- defN 23-Mar-31 04:30 snakeng/__main__.py
+-rw-rw-rw-  2.0 fat    18130 b- defN 23-Apr-08 18:16 snakeng/snake.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-Apr-08 18:32 snakeng-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6202 b- defN 23-Apr-08 18:32 snakeng-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 18:32 snakeng-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-08 18:32 snakeng-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      610 b- defN 23-Apr-08 18:32 snakeng-2.0.0.dist-info/RECORD
+8 files, 40469 bytes uncompressed, 12494 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: snakeng/__main__.py
 Comment: 
 
 Filename: snakeng/snake.py
 Comment: 
 
-Filename: snakeng-1.0.0.dist-info/LICENSE
+Filename: snakeng-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: snakeng-1.0.0.dist-info/METADATA
+Filename: snakeng-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: snakeng-1.0.0.dist-info/WHEEL
+Filename: snakeng-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: snakeng-1.0.0.dist-info/top_level.txt
+Filename: snakeng-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: snakeng-1.0.0.dist-info/RECORD
+Filename: snakeng-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## snakeng/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "2.0.0"
```

## snakeng/__main__.py

```diff
@@ -8,36 +8,27 @@
 import keyboard
 
 from snakeng.snake import SnakeGame, Speed, Direction
 
 scheduler = sched.scheduler(time.time, time.sleep)
 
 runtime_data = {
-    'last_direction': None,
     'paused': False,
     'scheduler_event': None
 }
 
 dirmap = {'up': Direction.UP, 'down': Direction.DOWN, 'left': Direction.LEFT, 'right': Direction.RIGHT}
 speedmap = {'slow': Speed.SLOW, 'medium': Speed.MEDIUM, 'fast': Speed.FAST, 'faster': Speed.FASTER}
 
-def keypress_event(e):
-    newdir = dirmap.get(e.name, None)
-    if newdir is None:
-        if e.name == 'p':
-            runtime_data['paused'] = not runtime_data['paused']
-    else:
-        runtime_data['last_direction'] = newdir
-
 
 def process_frame(game, frame_time):
     runtime_data["scheduler_event"] = scheduler.enterabs(time.time() + frame_time, 0, process_frame, argument=(game, frame_time))
 
     if not runtime_data['paused']:
-        new_state = game.process(runtime_data['last_direction'])
+        new_state = game.process()
         new_state_string = new_state.to_string()
         sys.stdout.write("\033[2J\n" + new_state_string)
         sys.stdout.flush()
 
         if new_state.dead:
             scheduler.cancel(runtime_data["scheduler_event"])
 
@@ -83,14 +74,23 @@
                      apples_disappear=not args.permanent_apples, apple_disappear_ticks=args.apple_ticks)
 
     if args.input_file is not None:
         with open(args.input_file, 'r') as fh:
             game.deserialize(json.load(fh))
 
     frame_time = 1.0 / float(args.fps)
+
+    def keypress_event(e):
+        newdir = dirmap.get(e.name, None)
+        if newdir is None:
+            if e.name == 'p':
+                runtime_data['paused'] = not runtime_data['paused']
+        else:
+            game.direction_input(newdir)
+
     keyboard.on_press(keypress_event)
 
     try:
         process_frame(game, frame_time)
         scheduler.run()
     except KeyboardInterrupt:
         if args.output_file:
```

## snakeng/snake.py

```diff
@@ -154,15 +154,15 @@
         for i in range(len(chunk[:-1])):
             x = chunk[i][0]
             y = chunk[i][1]
             nextx = chunk[i + 1][0]
             nexty = chunk[i + 1][1]
 
             newps = _draw_line(Position(x=x, y=y), Position(x=nextx, y=nexty))
-            if ret and (newps[0] == ret[-1]) and (len(newps) > 2):
+            if ret and (newps[0] == ret[-1]) and (len(newps) > 1):
                 newps.pop(0)
 
             ret.extend(newps)
 
     return ret
 
 
@@ -182,65 +182,67 @@
     :ivar fixed_speed: If True, snake speed does not change relative to snake size
     :ivar int score: Number of apples the snake has collected
     :ivar apple_position: Position object representing the current position of \
         the apple, or None if there is no apple.
     :ivar bool dead: True if the snake has died
     :ivar bool apples_disappear: If True, apples will disappear after a fixed period \
         of time if not collected. If False, apples will stay forever until collected.
-    :ivar int apple_disappear_ticks: specifies number of frames before apple disappears. \
-        If set to None, a sane default will be used.
+    :ivar int apple_disappear_ticks: specifies number of frames before apple disappears.
+    :ivar int apple_ticks: Number of ticks elapsed for current apple.
     """
     area_width: int = 120
     area_height: int = 120
     snake_segments: List = field(default_factory=lambda: [])
     snake_direction: int = Direction.UP
     snake_speed: int = Speed.SLOW
     fixed_speed: bool = False
     score: int = 0
     apple_position: Position = None
     dead: bool = False
     apples_disappear: bool = True
     apple_disappear_ticks: int = None
+    apple_ticks: int = 0
 
     def serialize(self):
         """
         Serialize the instance to a dict suitable for use with json.dump
 
         :return: serialized data as a dict
         :rtype: dict
         """
         return {
             'area_width': self.area_width,
             'area_height': self.area_height,
             'snake_segments': _serialize_snake_positions(self.snake_segments),
             'snake_direction': self.snake_direction,
-            'score': self.score,
             'apple_position': self.apple_position.serialize(),
             'snake_speed': self.snake_speed,
             'fixed_speed': self.fixed_speed,
             'apples_disappear': self.apples_disappear,
-            'apple_disappear_ticks': self.apple_disappear_ticks
+            'apple_disappear_ticks': self.apple_disappear_ticks,
+            'apple_ticks': self.apple_ticks
         }
 
     def deserialize(self, attrs):
         """
         Load the instance with values from a serialized dict
 
         :param dict attrs: dict containing instance values
         """
         self.area_width = attrs['area_width']
         self.area_height = attrs['area_height']
         self.snake_segments = _deserialize_snake_positions(attrs['snake_segments'])
         self.snake_direction = attrs['snake_direction']
-        self.score = attrs['score']
+        self.score = len(self.snake_segments) - 1
         self.apple_position = Position().deserialize(attrs['apple_position'])
         self.snake_speed = attrs['snake_speed']
         self.fixed_speed = attrs['fixed_speed']
         self.apples_disappear = attrs['apples_disappear']
         self.apple_disappear_ticks = attrs['apple_disappear_ticks']
+        self.apple_ticks = attrs['apple_ticks']
         return self
 
     def to_string(self, frame_corner_char='+', frame_horiz_char='-', frame_vert_char='|',
                   snake_head_left_char='<', snake_head_right_char='>', snake_head_up_char='^',
                   snake_head_down_char='v', snake_body_char='#', apple_char='@', space_char=' '):
         """
         Convert the instance to an ASCII string representing the current game state
@@ -346,20 +348,18 @@
         self.snake_move_ticks = 0
         self.queued_moves = []
 
         self.table = [[0 for _ in range(width)] for _ in range(height)]
         self.table[head_pos.y][head_pos.x] = 1
 
         if apple_disappear_ticks is None:
-            self.state.apple_disappear_ticks = max(width, height)
+            self.state.apple_disappear_ticks = max(width, height) * 3
         else:
             self.state.apple_disappear_ticks = apple_disappear_ticks
 
-        self.apple_ticks = 0
-
         if fixed_speed is not None:
             self.state.fixed_speed = True
             self.state.snake_speed = fixed_speed
 
     def deserialize(self, game_state):
         """
         Deserialize a saved game state from a dict and populate this instance with it
@@ -376,14 +376,20 @@
         Serialize the current game state to a dict suitable for json.dump
 
         :return: serialized game state as dict
         :rtype: dict
         """
         return self.state.serialize()
 
+    def direction_input(self, direction):
+        """
+        Provide a new directional input to the game
+        """
+        self.queued_moves.append(direction)
+
     def _new_apple_position(self):
         ret = self.state.snake_segments[-1]
         while ret in self.state.snake_segments:
             xval = random.randrange(1, self.state.area_width - 2)
             yval = random.randrange(1, self.state.area_height - 2)
             ret = Position(x=xval, y=yval)
 
@@ -404,17 +410,18 @@
 
     def _new_head(self):
         if self.snake_move_ticks < self.state.snake_speed:
             return None
 
         while self.queued_moves:
             new_direction = self.queued_moves.pop(0)
-            if new_direction != self.state.snake_direction:
-                self.state.snake_direction = new_direction
-                break
+            if (new_direction != self.state.snake_direction):
+                if not self._opposite_dirs(new_direction, self.state.snake_direction):
+                    self.state.snake_direction = new_direction
+                    break
 
         xadd, yadd = _MOVEMAP[self.state.snake_direction]
         self.snake_move_ticks = 0
         curr_head = self.state.snake_segments[-1]
         newx = curr_head.x + xadd
         newy = curr_head.y + yadd
 
@@ -440,61 +447,55 @@
         if (Direction.UP in dirs) and (Direction.DOWN in dirs):
             return True
         elif (Direction.LEFT in dirs) and (Direction.RIGHT in dirs):
             return True
 
         return False
 
-    def process(self, direction_input=None):
+    def process(self):
         """
         Process a single frame of the game, and return the new game state
 
-        :param SnakeGameInput direction_input: direction key currently being pressed, if any
-
         :return: New game state
         :rtype: SnakeGameState
         """
         if self.state.dead:
             return
 
-        if direction_input is not None:
-            if not self._opposite_dirs(direction_input, self.state.snake_direction):
-                self.queued_moves.append(direction_input)
-
         # Handle adding a new head segment in the current direction
         new_head = self._new_head()
 
         self.snake_move_ticks += 1
 
+        if self.state.apples_disappear:
+            if self.state.apple_ticks >= self.state.apple_disappear_ticks:
+                self.state.apple_position = self._new_apple_position()
+                self.state.apple_ticks = 0
+
+            self.state.apple_ticks += 1
+
         if new_head is None:
             return self.state
 
         if self.table[new_head.y][new_head.x] == 1:
             # Snake has hit itself
             self.state.dead = True
 
         self.state.snake_segments.append(new_head)
         self.table[new_head.y][new_head.x] = 1
 
         # Check if hit apple, delete apple and increment score if so
         if new_head == self.state.apple_position:
             self.state.apple_position = self._new_apple_position()
-            self.apple_ticks = 0
+            self.state.apple_ticks = 0
             self.state.score += 1
         else:
             tail = self.state.snake_segments.pop(0)
             self.table[tail.y][tail.x] = 0
 
-        if self.state.apples_disappear:
-            if self.apple_ticks >= self.state.apple_disappear_ticks:
-                self.state.apple_position = self._new_apple_position()
-                self.apple_ticks = 0
-
-            self.apple_ticks += 1
-
         # Check if we crossed a score threshold
         if not self.state.fixed_speed:
             if self.state.snake_speed == Speed.SLOW:
                 if self.state.score >= SLOW_SCORE_THRESHOLD:
                     self.state.snake_speed = Speed.MEDIUM
             elif self.state.snake_speed == Speed.MEDIUM:
                 if self.state.score >= MEDIUM_SCORE_THRESHOLD:
```

## Comparing `snakeng-1.0.0.dist-info/LICENSE` & `snakeng-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `snakeng-1.0.0.dist-info/METADATA` & `snakeng-2.0.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakeng
-Version: 1.0.0
+Version: 2.0.0
 Summary: Easy-to-use snake game engine. Quickly implement snake for anything!
 Home-page: http://github.com/eriknyquist/snakeng
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://eriknyquist.github.io/snakeng
 Project-URL: Issues, https://github.com/eriknyquist/snakeng/issues
@@ -59,32 +59,32 @@
 .. code:: python
 
     import sys
     import time
     import keyboard
     from snakeng.snake import SnakeGame, Direction
 
-    last_direction = Direction.DOWN
     dirmap = {'up': Direction.UP, 'down': Direction.DOWN, 'left': Direction.LEFT, 'right': Direction.RIGHT}
 
+    game = SnakeGame()                 # Create game instance
+
     def keypress_event(e):
-        global last_direction
         new_direction = dirmap.get(e.name, None)
         if new_direction is not None:
-            last_direction = new_direction
+            game.direction_input(new_direction)
 
     keyboard.on_press(keypress_event)  # Register callback function to save last keypress
-    game = SnakeGame()                 # Create game instance
 
     while True:
-        new_state = game.process(last_direction)               # Produce new frame
+        new_state = game.process()                             # Produce new frame
         sys.stdout.write("\033[2J\n" + new_state.to_string())  # Clear terminal screen and print new game state
         sys.stdout.flush()                                     # Flush output
         time.sleep(0.05)
 
+
 Sample command-line (ASCII) implementation
 -------------------------------------------
 
 Additionally, a sample terminal-based implementation of a snake game is provided,
 which can be accessed by running ``snakeng`` as a module:
 
 ::
```

## Comparing `snakeng-1.0.0.dist-info/RECORD` & `snakeng-2.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-snakeng/__init__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-snakeng/__main__.py,sha256=H3z7zg5BnU66Toa7zfHptHcf9y7DoEjc7mUlc7BU2mc,4684
-snakeng/snake.py,sha256=AFRpf0Qmzg7yHPSXxF4vSK7OI0BMAMjON6vgfkqdW-w,18058
-snakeng-1.0.0.dist-info/LICENSE,sha256=TnXSlu6RXKQvvwOoFbWv--MAdwOfsuLVHilmQGOJLE0,10761
-snakeng-1.0.0.dist-info/METADATA,sha256=gCJAuRWRHqgHnE9yKnhSYeNgn2GuHFUF7kfcyoDkXsI,6261
-snakeng-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-snakeng-1.0.0.dist-info/top_level.txt,sha256=oBJqdggtCvjEQxNzZJr7HnwlTiGQUZvjD55-VOgS25E,8
-snakeng-1.0.0.dist-info/RECORD,,
+snakeng/__init__.py,sha256=_7OlQdbVkK4jad0CLdpI0grT-zEAb-qgFmH5mFzDXiA,22
+snakeng/__main__.py,sha256=H5FCi7ADO9tdJOzjmUMV65Jjsbb-7xovBa-TnWBh6ns,4644
+snakeng/snake.py,sha256=7shD2hAS-QFD5iRyFNnD4PyWAcNeBupxVqXflYhaql8,18130
+snakeng-2.0.0.dist-info/LICENSE,sha256=TnXSlu6RXKQvvwOoFbWv--MAdwOfsuLVHilmQGOJLE0,10761
+snakeng-2.0.0.dist-info/METADATA,sha256=X69LfQmrBhkxVn3h0PKd-HnnKCxFbWj7kNdOxKYD1bI,6202
+snakeng-2.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+snakeng-2.0.0.dist-info/top_level.txt,sha256=oBJqdggtCvjEQxNzZJr7HnwlTiGQUZvjD55-VOgS25E,8
+snakeng-2.0.0.dist-info/RECORD,,
```

