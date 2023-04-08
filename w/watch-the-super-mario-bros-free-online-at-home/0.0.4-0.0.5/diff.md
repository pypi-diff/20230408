# Comparing `tmp/watch-the-super-mario-bros-free-online-at-home-0.0.4.tar.gz` & `tmp/watch-the-super-mario-bros-free-online-at-home-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-the-super-mario-bros-free-online-at-home-0.0.4.tar", last modified: Sat Apr  8 20:49:28 2023, max compression
+gzip compressed data, was "watch-the-super-mario-bros-free-online-at-home-0.0.5.tar", last modified: Sat Apr  8 21:13:17 2023, max compression
```

## Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.4.tar` & `watch-the-super-mario-bros-free-online-at-home-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 20:49:28.199199 watch-the-super-mario-bros-free-online-at-home-0.0.4/
--rw-rw-rw-   0        0        0     1069 2023-04-08 20:47:15.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      572 2023-04-08 20:49:28.199199 watch-the-super-mario-bros-free-online-at-home-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    14206 2023-04-08 20:35:07.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 20:49:28.175210 watch-the-super-mario-bros-free-online-at-home-0.0.4/mariobros/
--rw-rw-rw-   0        0        0      654 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/mariobros/Area_Fig.py
--rw-rw-rw-   0        0        0        0 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/mariobros/__init__.py
--rw-rw-rw-   0        0        0       86 2023-04-08 20:49:28.202188 watch-the-super-mario-bros-free-online-at-home-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-04-08 20:46:31.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:49:28.197201 watch-the-super-mario-bros-free-online-at-home-0.0.4/watch_the_super_mario_bros_free_online_at_home.egg-info/
--rw-rw-rw-   0        0        0      572 2023-04-08 20:49:28.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/watch_the_super_mario_bros_free_online_at_home.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-08 20:49:28.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/watch_the_super_mario_bros_free_online_at_home.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 20:49:28.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/watch_the_super_mario_bros_free_online_at_home.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-08 20:49:28.000000 watch-the-super-mario-bros-free-online-at-home-0.0.4/watch_the_super_mario_bros_free_online_at_home.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 21:13:17.188605 watch-the-super-mario-bros-free-online-at-home-0.0.5/
+-rw-rw-rw-   0        0        0     1069 2023-04-08 20:47:15.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    14890 2023-04-08 21:13:17.189602 watch-the-super-mario-bros-free-online-at-home-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14206 2023-04-08 20:35:07.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 21:13:17.170653 watch-the-super-mario-bros-free-online-at-home-0.0.5/mariobros/
+-rw-rw-rw-   0        0        0      654 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/mariobros/Area_Fig.py
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:11:49.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/mariobros/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-08 21:13:17.196584 watch-the-super-mario-bros-free-online-at-home-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1247 2023-04-08 21:12:55.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 21:13:17.188605 watch-the-super-mario-bros-free-online-at-home-0.0.5/watch_the_super_mario_bros_free_online_at_home.egg-info/
+-rw-rw-rw-   0        0        0    14890 2023-04-08 21:13:17.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/watch_the_super_mario_bros_free_online_at_home.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-04-08 21:13:17.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/watch_the_super_mario_bros_free_online_at_home.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 21:13:17.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/watch_the_super_mario_bros_free_online_at_home.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-08 21:13:17.000000 watch-the-super-mario-bros-free-online-at-home-0.0.5/watch_the_super_mario_bros_free_online_at_home.egg-info/top_level.txt
```

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.4/LICENSE.txt` & `watch-the-super-mario-bros-free-online-at-home-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.4/README.md` & `watch-the-super-mario-bros-free-online-at-home-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `watch-the-super-mario-bros-free-online-at-home-0.0.4/mariobros/Area_Fig.py` & `watch-the-super-mario-bros-free-online-at-home-0.0.5/mariobros/Area_Fig.py`

 * *Files identical despite different names*

