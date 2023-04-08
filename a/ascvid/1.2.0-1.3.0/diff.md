# Comparing `tmp/ascvid-1.2.0.tar.gz` & `tmp/ascvid-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascvid-1.2.0.tar", last modified: Sat Apr  8 16:30:08 2023, max compression
+gzip compressed data, was "ascvid-1.3.0.tar", last modified: Sat Apr  8 16:52:44 2023, max compression
```

## Comparing `ascvid-1.2.0.tar` & `ascvid-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/
--rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.2.0/LICENSE
--rw-r--r--   0 adam      (1003) adam      (1003)     3354 2023-04-08 16:30:08.449091 ascvid-1.2.0/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     2595 2023-04-08 16:06:12.000000 ascvid-1.2.0/README.rst
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/ascvid/
--rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.2.0/ascvid/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.2.0/ascvid/__main__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      831 2023-04-07 16:57:03.000000 ascvid-1.2.0/ascvid/audio.py
--rw-r--r--   0 adam      (1003) adam      (1003)     2845 2023-04-08 09:19:47.000000 ascvid-1.2.0/ascvid/cli.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.2.0/ascvid/getcol.py
--rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.2.0/ascvid/logger.py
--rw-r--r--   0 adam      (1003) adam      (1003)     5234 2023-04-08 09:42:06.000000 ascvid-1.2.0/ascvid/player.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.2.0/ascvid/run_terminal.py
--rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.2.0/ascvid/timer.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:30:08.449091 ascvid-1.2.0/ascvid.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)     3354 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       46 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:30:08.000000 ascvid-1.2.0/ascvid.egg-info/top_level.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:30:08.449091 ascvid-1.2.0/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)     3536 2023-04-08 16:29:00.000000 ascvid-1.2.0/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.634208 ascvid-1.3.0/
+-rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.3.0/LICENSE
+-rw-r--r--   0 adam      (1003) adam      (1003)     3405 2023-04-08 16:52:44.630874 ascvid-1.3.0/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     2660 2023-04-08 16:52:21.000000 ascvid-1.3.0/README.rst
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.630874 ascvid-1.3.0/ascvid/
+-rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.3.0/ascvid/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.3.0/ascvid/__main__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      831 2023-04-07 16:57:03.000000 ascvid-1.3.0/ascvid/audio.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     2933 2023-04-08 16:44:11.000000 ascvid-1.3.0/ascvid/cli.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.3.0/ascvid/getcol.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.3.0/ascvid/logger.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     5278 2023-04-08 16:44:37.000000 ascvid-1.3.0/ascvid/player.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.3.0/ascvid/run_terminal.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.3.0/ascvid/timer.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.630874 ascvid-1.3.0/ascvid.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3405 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       46 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:52:44.634208 ascvid-1.3.0/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     3587 2023-04-08 16:51:52.000000 ascvid-1.3.0/setup.py
```

### Comparing `ascvid-1.2.0/LICENSE` & `ascvid-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/PKG-INFO` & `ascvid-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.2.0
+Version: 1.3.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -65,10 +65,12 @@
       -d, --disable-controls  Disables pausing the video
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
+      -o, --outfile TEXT      Specify output file
+
       --help                  Show this message and exit.
```

### Comparing `ascvid-1.2.0/README.rst` & `ascvid-1.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -43,9 +43,10 @@
                               resizes the entire video. Use this if the video is
                               lagging too much.
       -d, --disable-controls  Disables pausing the video
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
-      -t, --term TEXT         Specify terminal in format '<terminal command> <run   
+      -t, --term TEXT         Specify terminal in format '<terminal command> <run command switch>'
+      -o, --outfile TEXT      Specify output file
```

### Comparing `ascvid-1.2.0/ascvid/audio.py` & `ascvid-1.3.0/ascvid/audio.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/ascvid/cli.py` & `ascvid-1.3.0/ascvid/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 @click.option("--no-truecolor","-T",is_flag=True,default=False,help="Reduces color palette. Use this flag on more stupid terminals (windows).")
 @click.option("--fast","-F",is_flag=True,default=False,help="Toggles off resizing each frame individually, rather resizes the entire video. Use this if the video is lagging too much.")
 @click.option("--disable-controls","-d",is_flag=True,default=False,help="Disables pausing the video")
 @click.option("--title","-t",default=None,help="Sets the title of the video. If not set, file name will be used instead")
 @click.option("--hide-title","-h",default=False,is_flag=True,help="hides the title")
 @click.option("--new-window","-n",is_flag=True,help="Opens in a new terminal window")
 @click.option("--term","-t",default=None,help="Specify terminal in format '<terminal command> <run command switch> {}'")
-def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast,disable_controls,title,hide_title,new_window,term):
+@click.option("--outfile","-o",default=None,help="Specify output file")
+def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast,disable_controls,title,hide_title,new_window,term,outfile):
     if new_window:
         cmd = [sys.executable,"-m","ascvid",file]
         if hide_cursor:
             cmd.extend(["-H"])
         if no_audio:
             cmd.extend(["-A"])
         if fps is not None:
@@ -45,8 +46,8 @@
         run_term(' '.join(cmd),term)
         return
     if fps and fps!="max":
         fps=int(fps)
     play_audio=not no_audio
     colored = not no_color
     truecolor = not no_truecolor
-    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast,disable_controls,title,not hide_title)
+    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast,disable_controls,title,not hide_title,outfile)
```

### Comparing `ascvid-1.2.0/ascvid/getcol.py` & `ascvid-1.3.0/ascvid/getcol.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/ascvid/logger.py` & `ascvid-1.3.0/ascvid/logger.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/ascvid/player.py` & `ascvid-1.3.0/ascvid/player.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,16 @@
 def closest(col):
     global CLOSEST_CACHE
     if col in CLOSEST_CACHE:
         return CLOSEST_CACHE[col]
     cl=closest_color(col)
     CLOSEST_CACHE[col]=cl
     return cl
-def clear():
-    if sys.platform=="win32":
-        os.system("cls")
-    else:
-        os.system("clear")
+def clear(out):
+    out.write("\x1b[H\x1b[2J\x1b[3J")
 def get_brightness(col):
     R,G,B=col
     return sqrt(0.299 * R**2 + 0.587 * G**2 + 0.114 * B**2)
 
 def get_character(color,colored,truecolor):
     r,g,b=color
     brightness=round(get_brightness(color))
@@ -62,22 +59,22 @@
     if use_ascii:
         return get_character(color,colored,truecolor)
     if truecolor:
         r,g,b=color
         return f"\x1b[38;2;{r};{g};{b}m{char}"
     return f"{closest(color)}{char}"
 
-def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit):
+def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit,out):
     ts=os.get_terminal_size()
     tw=ts.columns
     th=ts.lines
     if hast:
         th-=1
-    sys.stdout.write('\033[H')
-    sys.stdout.flush()
+    out.write('\033[H')
+    out.flush()
     d=Image.fromarray(fr)
     if resize:
         dh=d.height//2
         wd=d.width/tw
         hd=dh/th
         scale=1
         if wd>1 and hd>1 and wd>=hd:
@@ -95,23 +92,27 @@
 
     for y in range(d.height):
         line=''
         for x in range(d.width):
             r,g,b,*foo=pix[x,y]
             line+=get_pixel((r,g,b),colored,truecolor,use_ascii,char)
         lines.append(line+'\x1b[0m')
-    clear()
+    clear(out)
     if hast:
-        print(tit)
-    print('\n'.join(lines),end="")
+        print(tit,file=out)
+    print('\n'.join(lines),end="",file=out)
 def mkpos(a):
     if a<0:
         return 0
     return a
-def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False,disable_controls=False,title=None,show_title=True):
+def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False,disable_controls=False,title=None,show_title=True,out=None):
+    if out is None:
+        out=sys.stdout
+    else:
+        out=open(out,"w")
     if title is None:
         title=file
 
     vid=mp.VideoFileClip(file)
     q=queue.Queue()
     settings=None
     if sys.platform.lower().startswith("linux"):
@@ -153,36 +154,36 @@
         cursor.hide()
     if play_audio and vid.audio is not None:
         audio_stream=audio.Audio(vid)
         audio_stream.play()
     if not disable_controls:
         check_thread=threading.Thread(target=check_paused(q),daemon=True)
         check_thread.start()
-    clear()
+    clear(out)
     try: 
         for frame in vid.iter_frames():
 
             if not disable_controls:
                 resp=fqget(q)
                 if resp==" ":
                     if audio_stream is not None:
                         audio_stream.pause()
                     while q.get()!=" ":
                         pass
                     if audio_stream is not None:
                         audio_stream.resume()
             t=time.time()
-            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title)
+            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title,out)
             if fps!="max":
                 time.sleep(mkpos(1/fps-(time.time()-t)))
     finally:
         cursor.show()
-        sys.stdout.write("\x1b[0m")
-        sys.stdout.flush()
+        out.write("\x1b[0m")
+        out.flush()
         if settings is not None:
             time.sleep(0.2)
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, settings)
 
-        clear()
+        clear(out)
```

### Comparing `ascvid-1.2.0/ascvid/run_terminal.py` & `ascvid-1.3.0/ascvid/run_terminal.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/ascvid/timer.py` & `ascvid-1.3.0/ascvid/timer.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.2.0/ascvid.egg-info/PKG-INFO` & `ascvid-1.3.0/ascvid.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.2.0
+Version: 1.3.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -65,10 +65,12 @@
       -d, --disable-controls  Disables pausing the video
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
+      -o, --outfile TEXT      Specify output file
+
       --help                  Show this message and exit.
```

### Comparing `ascvid-1.2.0/setup.py` & `ascvid-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name="ascvid",version="1.2.0",description="ASCII Video player.", long_description=
+setuptools.setup(name="ascvid",version="1.3.0",description="ASCII Video player.", long_description=
                  """
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
 ``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
@@ -49,14 +49,16 @@
       -d, --disable-controls  Disables pausing the video
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
+      -o, --outfile TEXT      Specify output file
+
       --help                  Show this message and exit.
    
     """,
                  install_requires=["pillow","moviepy","cursor","numpy","click","sounddevice"],
                  packages=["ascvid"],
                  classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: Microsoft :: Windows","Operating System :: POSIX :: Linux","Operating System :: Unix","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
```

