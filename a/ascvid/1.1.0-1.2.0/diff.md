# Comparing `tmp/ascvid-1.1.0.tar.gz` & `tmp/ascvid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascvid-1.1.0.tar", last modified: Thu Apr  6 15:56:02 2023, max compression
+gzip compressed data, was "ascvid-1.2.0.tar", last modified: Sat Apr  8 16:30:08 2023, max compression
```

## Comparing `ascvid-1.1.0.tar` & `ascvid-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-06 15:56:02.163287 ascvid-1.1.0/
--rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.1.0/LICENSE
--rw-r--r--   0 adam      (1003) adam      (1003)     2622 2023-04-06 15:56:02.163287 ascvid-1.1.0/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     1789 2023-04-06 10:21:51.000000 ascvid-1.1.0/README.rst
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-06 15:56:02.159953 ascvid-1.1.0/ascvid/
--rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.1.0/ascvid/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.1.0/ascvid/__main__.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1445 2023-04-06 15:39:53.000000 ascvid-1.1.0/ascvid/cli.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1155 2023-04-06 09:10:38.000000 ascvid-1.1.0/ascvid/getcol.py
--rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.1.0/ascvid/logger.py
--rw-r--r--   0 adam      (1003) adam      (1003)     4009 2023-04-06 15:54:31.000000 ascvid-1.1.0/ascvid/player.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-06 15:56:02.163287 ascvid-1.1.0/ascvid.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)     2622 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      312 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       34 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-06 15:56:02.000000 ascvid-1.1.0/ascvid.egg-info/top_level.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-06 15:56:02.163287 ascvid-1.1.0/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)     2810 2023-04-06 15:52:49.000000 ascvid-1.1.0/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/
+-rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.2.0/LICENSE
+-rw-r--r--   0 adam      (1003) adam      (1003)     3354 2023-04-08 16:30:08.449091 ascvid-1.2.0/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     2595 2023-04-08 16:06:12.000000 ascvid-1.2.0/README.rst
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/ascvid/
+-rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.2.0/ascvid/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.2.0/ascvid/__main__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      831 2023-04-07 16:57:03.000000 ascvid-1.2.0/ascvid/audio.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     2845 2023-04-08 09:19:47.000000 ascvid-1.2.0/ascvid/cli.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.2.0/ascvid/getcol.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.2.0/ascvid/logger.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     5234 2023-04-08 09:42:06.000000 ascvid-1.2.0/ascvid/player.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.2.0/ascvid/run_terminal.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.2.0/ascvid/timer.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/ascvid.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3354 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       46 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:30:08.449091 ascvid-1.2.0/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     3536 2023-04-08 16:29:00.000000 ascvid-1.2.0/setup.py
```

### Comparing `ascvid-1.1.0/LICENSE` & `ascvid-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascvid-1.1.0/PKG-INFO` & `ascvid-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.1.0
+Version: 1.2.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Video :: Display
 License-File: LICENSE
 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
-``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on other OS too.
+``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
 
 It requires a Truecolor terminal to work like this. If you are on a stupider terminal, the results will look less realistic.The produced graphics aren't blinking as in other ASCII video players, however, the videos might lag a bit if your terminal is zoomed out.
-``ascvid`` also supports audio! It's a true video player.
+``ascvid`` also supports audio output and pausing your video! It's a true video player.
+
 
 Installation
 ============
 
 .. code-block:: console
    
    python3 -m pip install ascvid
 
 Then you can just run ``ascvid`` and you're good to go.
 
 CLI Options
 ===========
 *NOTE :: --no-truecolor option lags like my brain, so if you are on a stupid terminal, you are better off using --no-color in ASCII mode.*
 .. code-block:: console
-    
-    Usage: python -m ascvid [OPTIONS] FILE
+   
+    Usage: ascvid [OPTIONS] FILE
 
     Options:
-      -H, --hide-cursor   Hide the cursor while playing the video
-      -A, --no-audio      Don't play audio stream
-      -f, --fps TEXT      Number of FPS the video's supposed to run at. If None,
-                          it's determined from the video. If "max", ascvid will
-                          try its best to keep the video from lagging
-      -c, --char TEXT     Character to be used while rendering the video frames
-      -C, --no-color      Don't color output
-      -a, --ascii         Use multiple ASCII characters. Best to be used with
-                          --no-truecolor
-      -T, --no-truecolor  Reduces color palette. Use this flag on more stupid
-                          terminals (windows).
-      -F, --fast          Toggles off resizing each frame individually, rather
-                          resizes the entire video. Use this if the video is
-                          lagging too much.
-      --help              Show this message and exit.
+      -H, --hide-cursor       Hide the cursor while playing the video
+      -A, --no-audio          Don't play audio stream
+      -f, --fps TEXT          Number of FPS the video's supposed to run at. If
+                              None, it's determined from the video. If "max",
+                              ascvid will try its best to keep the video from
+                              lagging
+      -c, --char TEXT         Character to be used while rendering the video
+                              frames
+      -C, --no-color          Don't color output
+      -a, --ascii             Use multiple ASCII characters. Best to be used with
+                              --no-truecolor
+      -T, --no-truecolor      Reduces color palette. Use this flag on more stupid
+                              terminals (windows).
+      -F, --fast              Toggles off resizing each frame individually, rather
+                              resizes the entire video. Use this if the video is
+                              lagging too much.
+      -d, --disable-controls  Disables pausing the video
+      -t, --title TEXT        Sets the title of the video. If not set, file name
+                              will be used instead
+      -h, --hide-title        hides the title
+      -n, --new-window        Opens in a new terminal window
+      -t, --term TEXT         Specify terminal in format '<terminal command> <run
+                              command switch> {}'
+      --help                  Show this message and exit.
+
```

### Comparing `ascvid-1.1.0/README.rst` & `ascvid-1.2.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,51 @@
-.. image:: asc.png
+.. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
-``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it should work on other OS too.
+``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
-.. image:: rick.gif
+.. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
+
+It requires a Truecolor or at least 256-color terminal to work like this. If you are on a stupider terminal, the results will look less realistic.The produced graphics aren't blinking as in other ASCII video players, however, the videos might lag a bit if your terminal is zoomed out.
+``ascvid`` also supports audio output and pausing your video! It's a true video player.
 
-It requires a Truecolor terminal to work like that. If you are using a more stupid terminal, the graphics will look less realistic. The produced graphics aren't blinking as in other ASCII video players, however, the videos might lag a bit if your terminal is zoomed out.
-``ascvid`` also supports audio! It's a true video player.
 
 Installation
 ============
 
 .. code-block:: console
    
    python3 -m pip install ascvid
 
+Then you can just run ``ascvid`` and you're good to go.
+
 CLI Options
 ===========
-
+*NOTE :: --no-truecolor option lags like my brain, so if you are on a stupid terminal, you are better off using --no-color in ASCII mode.*
 .. code-block:: console
-        
+   
     Usage: ascvid [OPTIONS] FILE
 
-        Options:
-          -H, --hide-cursor   Hide the cursor while playing the video
-          -A, --no-audio      Don't play audio stream
-          -f, --fps TEXT      Number of FPS the video's supposed to run at. If None,
-                              it's determined from the video. If "max", ascvid will
-                              try its best to keep the video from lagging
-          -c, --char TEXT     Character to be used while rendering the video frames
-          -C, --no-color      Don't color output
-          -a, --ascii         Use multiple ASCII characters. Best to be used with
+    Options:
+      -H, --hide-cursor       Hide the cursor while playing the video
+      -A, --no-audio          Don't play audio stream
+      -f, --fps TEXT          Number of FPS the video's supposed to run at. If
+                              None, it's determined from the video. If "max",
+                              ascvid will try its best to keep the video from
+                              lagging
+      -c, --char TEXT         Character to be used while rendering the video
+                              frames
+      -C, --no-color          Don't color output
+      -a, --ascii             Use multiple ASCII characters. Best to be used with
                               --no-truecolor
-          -T, --no-truecolor  Reduces color palette. Use this flag on more stupid
+      -T, --no-truecolor      Reduces color palette. Use this flag on more stupid
                               terminals (windows).
-          -F, --fast          Toggles off resizing each frame individually, rather
+      -F, --fast              Toggles off resizing each frame individually, rather
                               resizes the entire video. Use this if the video is
                               lagging too much.
-          --help              Show this message and exit.
+      -d, --disable-controls  Disables pausing the video
+      -t, --title TEXT        Sets the title of the video. If not set, file name
+                              will be used instead
+      -h, --hide-title        hides the title
+      -n, --new-window        Opens in a new terminal window
+      -t, --term TEXT         Specify terminal in format '<terminal command> <run   
+
```

### Comparing `ascvid-1.1.0/ascvid/cli.py` & `ascvid-1.2.0/ascvid/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,52 @@
 from .player import play_vid
+from .run_terminal import run_term 
 import click
-
+import sys
 @click.command()
 @click.argument("file")
 @click.option("--hide-cursor","-H",default=False,is_flag=True,help="Hide the cursor while playing the video")
 @click.option("--no-audio","-A",is_flag=True,default=False,help="Don't play audio stream")
 @click.option("--fps","-f",default=None,help="Number of FPS the video's supposed to run at. If None, it's determined from the video. If \"max\", ascvid will try its best to keep the video from lagging")
 @click.option("--char","-c",default='\u2588',type=str,help="Character to be used while rendering the video frames")
 @click.option("--no-color","-C",default=False,is_flag=True,help="Don't color output")
 @click.option("--ascii","-a",is_flag=True,default=False,help="Use multiple ASCII characters. Best to be used with --no-truecolor")
 @click.option("--no-truecolor","-T",is_flag=True,default=False,help="Reduces color palette. Use this flag on more stupid terminals (windows).")
 @click.option("--fast","-F",is_flag=True,default=False,help="Toggles off resizing each frame individually, rather resizes the entire video. Use this if the video is lagging too much.")
-def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast):
+@click.option("--disable-controls","-d",is_flag=True,default=False,help="Disables pausing the video")
+@click.option("--title","-t",default=None,help="Sets the title of the video. If not set, file name will be used instead")
+@click.option("--hide-title","-h",default=False,is_flag=True,help="hides the title")
+@click.option("--new-window","-n",is_flag=True,help="Opens in a new terminal window")
+@click.option("--term","-t",default=None,help="Specify terminal in format '<terminal command> <run command switch> {}'")
+def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast,disable_controls,title,hide_title,new_window,term):
+    if new_window:
+        cmd = [sys.executable,"-m","ascvid",file]
+        if hide_cursor:
+            cmd.extend(["-H"])
+        if no_audio:
+            cmd.extend(["-A"])
+        if fps is not None:
+            cmd.extend(["-f"])
+            cmd.extend([f"{fps}"])
+        cmd.extend(["-c",f"{char}"])
+        if no_color:
+            cmd.extend(["-C"])
+        if ascii:
+            cmd.extend(["-a"])
+        if no_truecolor:
+            cmd.extend(["-T"])
+        if fast:
+            cmd.extend(["-F"])
+        if disable_controls:
+            cmd.extend(["-d"])
+        if title is not None:
+            cmd.extend(["-t",f"{title}"])
+        if hide_title:
+            cmd.extend(["-h"])
+        run_term(' '.join(cmd),term)
+        return
     if fps and fps!="max":
         fps=int(fps)
     play_audio=not no_audio
     colored = not no_color
     truecolor = not no_truecolor
-    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast)
+    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast,disable_controls,title,not hide_title)
```

### Comparing `ascvid-1.1.0/ascvid/getcol.py` & `ascvid-1.2.0/ascvid/getcol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import colorama
 from math import sqrt
-import numpy as np
+import colorsys
 colorama.init()
 #### Please note that these colors might display differently on other terminals
-COLORS = {
+_COLORS = {
     (0, 0, 0): colorama.Fore.BLACK,
     (128, 0, 0): colorama.Fore.RED,
     (0, 128, 0): colorama.Fore.GREEN,
     (128, 128, 0): colorama.Fore.YELLOW,
     (0, 0, 128): colorama.Fore.BLUE,
     (128, 0, 128): colorama.Fore.MAGENTA,
     (0, 128, 128): colorama.Fore.CYAN,
@@ -17,15 +17,15 @@
     (0, 255, 0): colorama.Fore.LIGHTGREEN_EX,
     (255, 255, 0): colorama.Fore.LIGHTYELLOW_EX,
     (0, 255, 255): colorama.Fore.LIGHTCYAN_EX,
     (255, 0, 255): colorama.Fore.LIGHTMAGENTA_EX,
     (255, 255, 255): colorama.Fore.LIGHTWHITE_EX,
 
 }
-COLKEYS=list(COLORS.keys())
+COLORS = {colorsys.rgb_to_hsv(*k):v for k,v in _COLORS.items()}
+def calc_dist(col1,col2):
+    return 2*abs(col1[0] - col2[0])+ abs(col1[1]-col2[1])+ abs(col1[2]-col2[2])
 def closest_color(color):
-    colors = np.array(COLKEYS)
-    color = np.array(color)
-    distances = np.sqrt(np.sum((colors-color)**2,axis=1))
-    index_of_smallest = np.where(distances==np.amin(distances))
-    smallest_distance = colors[index_of_smallest]
-    return COLORS[tuple(smallest_distance.tolist()[0])]
+    color=colorsys.rgb_to_hsv(*color)
+    min_d=min(COLORS,key=lambda d:calc_dist(color,d))
+    return COLORS[min_d]
+
```

### Comparing `ascvid-1.1.0/ascvid/logger.py` & `ascvid-1.2.0/ascvid/logger.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.1.0/ascvid/player.py` & `ascvid-1.2.0/ascvid/player.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,19 +2,40 @@
 from math import sqrt
 import moviepy.editor as mp
 import sys
 import os
 import time
 import cursor
 import threading
+import getkey
+import queue
 from .getcol import closest_color
 from .logger import print_error,print_warning
-CHARS = ' .\'`^",:;Il!i><~+_-?][}{1)(|\\/tfjrxnuvczXYUJCLQ0OZmwqpdbkhao*#MW&8%B@$'
+from . import audio
+CHARS = ' .\'`^",:;Il!i><~+_-?][}{1)(|\\/tfjrxnuvczXYUJCLQ0OZmwqpdbkhao*#MW&8%B@$\u2591\u2592\u2593\u2588'
 CLOSEST_CACHE = {}
 CHAR_CACHE = {}
+def fqget(q):
+    if q.empty():
+        return
+    return q.get()
+def _getchar(color):
+    if color in CHAR_CACHE:
+        return CHAR_CACHE[color]
+    brightness=round(get_brightness(color))
+    charindex=int((brightness/255)*(len(CHARS)-1))
+    char=CHARS[charindex]
+    CHAR_CACHE[color]=char
+    return char
+
+def check_paused(q):
+    def check():
+        while True:
+            q.put(getkey.getkey())
+    return check
 def closest(col):
     global CLOSEST_CACHE
     if col in CLOSEST_CACHE:
         return CLOSEST_CACHE[col]
     cl=closest_color(col)
     CLOSEST_CACHE[col]=cl
     return cl
@@ -22,22 +43,14 @@
     if sys.platform=="win32":
         os.system("cls")
     else:
         os.system("clear")
 def get_brightness(col):
     R,G,B=col
     return sqrt(0.299 * R**2 + 0.587 * G**2 + 0.114 * B**2)
-def _getchar(color):
-    if color in CHAR_CACHE:
-        return CHAR_CACHE[color]
-    brightness=round(get_brightness(color))
-    charindex=int((brightness/255)*(len(CHARS)-1))
-    char=CHARS[charindex]
-    CHAR_CACHE[color]=char
-    return char
 
 def get_character(color,colored,truecolor):
     r,g,b=color
     brightness=round(get_brightness(color))
     charindex=int((brightness/255)*(len(CHARS)-1))
     character=CHARS[charindex]
     if colored:
@@ -49,19 +62,20 @@
     if use_ascii:
         return get_character(color,colored,truecolor)
     if truecolor:
         r,g,b=color
         return f"\x1b[38;2;{r};{g};{b}m{char}"
     return f"{closest(color)}{char}"
 
-def show_frame(fr,char,colored,truecolor,use_ascii,resize):
+def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit):
     ts=os.get_terminal_size()
     tw=ts.columns
     th=ts.lines
-
+    if hast:
+        th-=1
     sys.stdout.write('\033[H')
     sys.stdout.flush()
     d=Image.fromarray(fr)
     if resize:
         dh=d.height//2
         wd=d.width/tw
         hd=dh/th
@@ -82,30 +96,41 @@
     for y in range(d.height):
         line=''
         for x in range(d.width):
             r,g,b,*foo=pix[x,y]
             line+=get_pixel((r,g,b),colored,truecolor,use_ascii,char)
         lines.append(line+'\x1b[0m')
     clear()
+    if hast:
+        print(tit)
     print('\n'.join(lines),end="")
 def mkpos(a):
     if a<0:
         return 0
     return a
-def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False):
+def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False,disable_controls=False,title=None,show_title=True):
+    if title is None:
+        title=file
+
     vid=mp.VideoFileClip(file)
+    q=queue.Queue()
+    settings=None
+    if sys.platform.lower().startswith("linux"):
+        import tty
+        import termios
+        settings=termios.tcgetattr(sys.stdin)
+
     if fast:
         frame_count=int(vid.fps*vid.duration)
         if frame_count>=10000:
             response=print_warning(f"{file!r} has {frame_count} frames.",ask="Are you sure you want to resize them all at once [y*]")
             if response!="y":
                 sys.exit(1)
         tw=os.get_terminal_size().columns
         th=os.get_terminal_size().lines
-
         vh=vid.h
         vw=vid.w
         dh=vh//2
         wd=vw-tw
         hd=dh-th
         scale=1
         if wd>0 and hd>0 and wd>=hd:
@@ -119,25 +144,45 @@
 
         vid=vid.resize((int(vw*scale),int(dh*scale)))
 
     fps = fps or vid.fps
     if fps!=vid.fps and fps!="max":
         vid=vid.set_fps(fps)
     process=None
+    audio_stream=None
     if hide_cursor:
         cursor.hide()
     if play_audio and vid.audio is not None:
-        thread=threading.Thread(target=vid.audio.preview,daemon=True)
-        thread.start()
+        audio_stream=audio.Audio(vid)
+        audio_stream.play()
+    if not disable_controls:
+        check_thread=threading.Thread(target=check_paused(q),daemon=True)
+        check_thread.start()
     clear()
-    try:
+    try: 
         for frame in vid.iter_frames():
+
+            if not disable_controls:
+                resp=fqget(q)
+                if resp==" ":
+                    if audio_stream is not None:
+                        audio_stream.pause()
+                    while q.get()!=" ":
+                        pass
+                    if audio_stream is not None:
+                        audio_stream.resume()
             t=time.time()
-            show_frame(frame,char,colored,truecolor,use_ascii,not fast)
+            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title)
             if fps!="max":
                 time.sleep(mkpos(1/fps-(time.time()-t)))
     finally:
         cursor.show()
         sys.stdout.write("\x1b[0m")
         sys.stdout.flush()
+        if settings is not None:
+            time.sleep(0.2)
+            termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, settings)
+
         clear()
-            
+
+           
+
```

### Comparing `ascvid-1.1.0/ascvid.egg-info/PKG-INFO` & `ascvid-1.2.0/ascvid.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.1.0
+Version: 1.2.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia :: Video :: Display
 License-File: LICENSE
 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
-``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on other OS too.
+``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
 
 It requires a Truecolor terminal to work like this. If you are on a stupider terminal, the results will look less realistic.The produced graphics aren't blinking as in other ASCII video players, however, the videos might lag a bit if your terminal is zoomed out.
-``ascvid`` also supports audio! It's a true video player.
+``ascvid`` also supports audio output and pausing your video! It's a true video player.
+
 
 Installation
 ============
 
 .. code-block:: console
    
    python3 -m pip install ascvid
 
 Then you can just run ``ascvid`` and you're good to go.
 
 CLI Options
 ===========
 *NOTE :: --no-truecolor option lags like my brain, so if you are on a stupid terminal, you are better off using --no-color in ASCII mode.*
 .. code-block:: console
-    
-    Usage: python -m ascvid [OPTIONS] FILE
+   
+    Usage: ascvid [OPTIONS] FILE
 
     Options:
-      -H, --hide-cursor   Hide the cursor while playing the video
-      -A, --no-audio      Don't play audio stream
-      -f, --fps TEXT      Number of FPS the video's supposed to run at. If None,
-                          it's determined from the video. If "max", ascvid will
-                          try its best to keep the video from lagging
-      -c, --char TEXT     Character to be used while rendering the video frames
-      -C, --no-color      Don't color output
-      -a, --ascii         Use multiple ASCII characters. Best to be used with
-                          --no-truecolor
-      -T, --no-truecolor  Reduces color palette. Use this flag on more stupid
-                          terminals (windows).
-      -F, --fast          Toggles off resizing each frame individually, rather
-                          resizes the entire video. Use this if the video is
-                          lagging too much.
-      --help              Show this message and exit.
+      -H, --hide-cursor       Hide the cursor while playing the video
+      -A, --no-audio          Don't play audio stream
+      -f, --fps TEXT          Number of FPS the video's supposed to run at. If
+                              None, it's determined from the video. If "max",
+                              ascvid will try its best to keep the video from
+                              lagging
+      -c, --char TEXT         Character to be used while rendering the video
+                              frames
+      -C, --no-color          Don't color output
+      -a, --ascii             Use multiple ASCII characters. Best to be used with
+                              --no-truecolor
+      -T, --no-truecolor      Reduces color palette. Use this flag on more stupid
+                              terminals (windows).
+      -F, --fast              Toggles off resizing each frame individually, rather
+                              resizes the entire video. Use this if the video is
+                              lagging too much.
+      -d, --disable-controls  Disables pausing the video
+      -t, --title TEXT        Sets the title of the video. If not set, file name
+                              will be used instead
+      -h, --hide-title        hides the title
+      -n, --new-window        Opens in a new terminal window
+      -t, --term TEXT         Specify terminal in format '<terminal command> <run
+                              command switch> {}'
+      --help                  Show this message and exit.
+
```

### Comparing `ascvid-1.1.0/setup.py` & `ascvid-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 import setuptools
 
-setuptools.setup(name="ascvid",version="1.1.0",description="ASCII Video player.", long_description=
+setuptools.setup(name="ascvid",version="1.2.0",description="ASCII Video player.", long_description=
                  """
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
-``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on other OS too.
+``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
 
 It requires a Truecolor terminal to work like this. If you are on a stupider terminal, the results will look less realistic.The produced graphics aren't blinking as in other ASCII video players, however, the videos might lag a bit if your terminal is zoomed out.
-``ascvid`` also supports audio! It's a true video player.
+``ascvid`` also supports audio output and pausing your video! It's a true video player.
+
 
 Installation
 ============
 
 .. code-block:: console
    
    python3 -m pip install ascvid
 
 Then you can just run ``ascvid`` and you're good to go.
 
 CLI Options
 ===========
 *NOTE :: --no-truecolor option lags like my brain, so if you are on a stupid terminal, you are better off using --no-color in ASCII mode.*
 .. code-block:: console
-    
-    Usage: python -m ascvid [OPTIONS] FILE
+   
+    Usage: ascvid [OPTIONS] FILE
 
     Options:
-      -H, --hide-cursor   Hide the cursor while playing the video
-      -A, --no-audio      Don't play audio stream
-      -f, --fps TEXT      Number of FPS the video's supposed to run at. If None,
-                          it's determined from the video. If "max", ascvid will
-                          try its best to keep the video from lagging
-      -c, --char TEXT     Character to be used while rendering the video frames
-      -C, --no-color      Don't color output
-      -a, --ascii         Use multiple ASCII characters. Best to be used with
-                          --no-truecolor
-      -T, --no-truecolor  Reduces color palette. Use this flag on more stupid
-                          terminals (windows).
-      -F, --fast          Toggles off resizing each frame individually, rather
-                          resizes the entire video. Use this if the video is
-                          lagging too much.
-      --help              Show this message and exit.
+      -H, --hide-cursor       Hide the cursor while playing the video
+      -A, --no-audio          Don't play audio stream
+      -f, --fps TEXT          Number of FPS the video's supposed to run at. If
+                              None, it's determined from the video. If "max",
+                              ascvid will try its best to keep the video from
+                              lagging
+      -c, --char TEXT         Character to be used while rendering the video
+                              frames
+      -C, --no-color          Don't color output
+      -a, --ascii             Use multiple ASCII characters. Best to be used with
+                              --no-truecolor
+      -T, --no-truecolor      Reduces color palette. Use this flag on more stupid
+                              terminals (windows).
+      -F, --fast              Toggles off resizing each frame individually, rather
+                              resizes the entire video. Use this if the video is
+                              lagging too much.
+      -d, --disable-controls  Disables pausing the video
+      -t, --title TEXT        Sets the title of the video. If not set, file name
+                              will be used instead
+      -h, --hide-title        hides the title
+      -n, --new-window        Opens in a new terminal window
+      -t, --term TEXT         Specify terminal in format '<terminal command> <run
+                              command switch> {}'
+      --help                  Show this message and exit.
+   
     """,
-                 install_requires=["pillow","moviepy","cursor","numpy","click"],
+                 install_requires=["pillow","moviepy","cursor","numpy","click","sounddevice"],
                  packages=["ascvid"],
-                 classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: OS Independent","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
+                 classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: Microsoft :: Windows","Operating System :: POSIX :: Linux","Operating System :: Unix","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
```

