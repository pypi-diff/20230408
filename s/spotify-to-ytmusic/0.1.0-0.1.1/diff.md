# Comparing `tmp/spotify_to_ytmusic-0.1.0.tar.gz` & `tmp/spotify_to_ytmusic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.1.0.tar", last modified: Sat Apr  8 14:12:01 2023, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.1.1.tar", last modified: Sat Apr  8 18:53:20 2023, max compression
```

## Comparing `spotify_to_ytmusic-0.1.0.tar` & `spotify_to_ytmusic-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.726717 spotify_to_ytmusic-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.722717 spotify_to_ytmusic-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.722717 spotify_to_ytmusic-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-08 14:12:01.726717 spotify_to_ytmusic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:12:01.726717 spotify_to_ytmusic-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.722717 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.726717 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-08 14:12:01.000000 spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:12:01.726717 spotify_to_ytmusic-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 14:11:51.000000 spotify_to_ytmusic-0.1.0/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.520875 spotify_to_ytmusic-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.508875 spotify_to_ytmusic-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.512875 spotify_to_ytmusic-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:53:20.520875 spotify_to_ytmusic-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-08 18:53:20.000000 spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:20.516875 spotify_to_ytmusic-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:53:09.000000 spotify_to_ytmusic-0.1.1/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.1.0/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.1.1/.github/workflows/coverage.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     - uses: actions/checkout@master
     - name: Setup Python
       uses: actions/setup-python@master
       with:
         python-version: 3.x
     - name: Generate coverage report
       env:
-        HEADERS_AUTH: ${{ secrets.HEADERS_AUTH }}
-        TEST_CFG: ${{ secrets.TEST_CFG }}
+        SETTINGS_INI: ${{ secrets.SETTINGS_INI }}
       run: |
         pip install -e .
         pip install coverage
         cat <<< "$SETTINGS_INI" > spotify_to_ytmusic/settings.ini
         coverage run
         coverage xml
     - name: Upload coverage to Codecov
```

### Comparing `spotify_to_ytmusic-0.1.0/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.1.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/.gitignore` & `spotify_to_ytmusic-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/LICENSE` & `spotify_to_ytmusic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/PKG-INFO` & `spotify_to_ytmusic-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,29 +24,34 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/sigma67/spotify_to_ytmusic
 Project-URL: repository, https://github.com/sigma67/spotify_to_ytmusic
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 spotify_to_ytmusic
-############################################
+####################
+
 .. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://badges.gitter.im/sigma67/spotify_to_ytmusic.svg
-   :alt: Ask questions at https://gitter.im/sigma67/spotify_to_ytmusic
-   :target: https://gitter.im/sigma67/spotify_to_ytmusic
+.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+   :alt: Ask questions at Discussions
+   :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
 .. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
 .. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
```

### Comparing `spotify_to_ytmusic-0.1.0/README.rst` & `spotify_to_ytmusic-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 spotify_to_ytmusic
-############################################
+####################
+
 .. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://badges.gitter.im/sigma67/spotify_to_ytmusic.svg
-   :alt: Ask questions at https://gitter.im/sigma67/spotify_to_ytmusic
-   :target: https://gitter.im/sigma67/spotify_to_ytmusic
+.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+   :alt: Ask questions at Discussions
+   :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
 .. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
 .. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
```

### Comparing `spotify_to_ytmusic-0.1.0/pyproject.toml` & `spotify_to_ytmusic-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 name = "spotify_to_ytmusic"
 description = "Transfer Spotify playlists to YouTube Music"
 requires-python = ">=3.8"
 authors=[{name = "sigma67", email= "ytmusicapi@gmail.com"}]
 license={file="LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "ytmusicapi",
-    "spotipy"
+    "ytmusicapi>=1.0",
+    "spotipy>=2.23.0"
 ]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
-dev = ['pre-commit', 'flake8', 'yapf', 'coverage', 'sphinx', 'sphinx-rtd-theme']
+dev = ['black', 'isort', 'coverage']
 
 [project.scripts]
 spotify_to_ytmusic = "spotify_to_ytmusic.main:main"
 
 [project.urls]
 homepage = "https://github.com/sigma67/spotify_to_ytmusic"
 repository = "https://github.com/sigma67/spotify_to_ytmusic"
```

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/controllers.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,29 +29,29 @@
         count = count + 1
         try:
             playlist = spotify.getSpotifyPlaylist(p["external_urls"]["spotify"])
             videoIds = ytmusic.search_songs(playlist["tracks"])
             playlist_id = ytmusic.create_playlist(
                 p["name"],
                 p["description"],
-                "PUBLIC" if args.public else "PRIVATE",
+                "PUBLIC" if p['public'] else "PRIVATE",
                 videoIds,
             )
             print(playlist_id)
         except Exception as ex:
             print(f"Could not transfer playlist {p['name']}. {str(ex)}")
 
 
 def create(args):
     spotify, ytmusic = _init()
     date = ""
     if args.date:
         date = " " + datetime.today().strftime("%m/%d/%Y")
 
-    playlist = _get_spotify_playlist(args.playlist)
+    playlist = _get_spotify_playlist(spotify, args.playlist)
     name = args.name + date if args.name else playlist["name"] + date
     info = playlist["description"] if (args.info is None) else args.info
     videoIds = ytmusic.search_songs(playlist["tracks"])
     playlistId = ytmusic.create_playlist(
         name, info, "PUBLIC" if args.public else "PRIVATE", videoIds
     )
 
@@ -59,18 +59,19 @@
         f"Success: created playlist {name}\n"
         f"https://music.youtube.com/playlist?list={playlistId}"
     )
 
 
 def update(args):
     spotify, ytmusic = _init()
-    playlist = _get_spotify_playlist(args.playlist)
+    playlist = _get_spotify_playlist(spotify, args.playlist)
     playlistId = ytmusic.get_playlist_id(args.name)
     videoIds = ytmusic.search_songs(playlist["tracks"])
-    ytmusic.remove_songs(playlistId)
+    if not args.append:
+        ytmusic.remove_songs(playlistId)
     ytmusic.add_playlist_items(playlistId, videoIds)
 
 
 def remove(args):
     ytmusic = YTMusicTransfer()
     ytmusic.remove_playlists(args.pattern)
```

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,23 @@
     parser = argparse.ArgumentParser(description="Transfer spotify playlists to YouTube Music.")
 
     subparsers = parser.add_subparsers(help="Provide a subcommand", dest="command", required=True)
     setup_parser = subparsers.add_parser("setup", help="Set up credentials")
     setup_parser.set_defaults(func=controllers.setup)
     setup_parser.add_argument("--file", type=Path, help="Optional path to a settings.ini file")
 
-    playlist_creator = argparse.ArgumentParser(add_help=False)
-    playlist_creator.add_argument(
-        "-p",
-        "--public",
-        action="store_true",
-        help="Make created playlist public. Default: private",
-    )
+    spotify_playlist = argparse.ArgumentParser(add_help=False)
+    spotify_playlist.add_argument("playlist", type=str, help="Provide a playlist Spotify link.")
 
     create_parser = subparsers.add_parser(
         "create",
         help="Create a new playlist on YouTube Music.",
-        parents=[playlist_creator],
+        parents=[spotify_playlist],
     )
     create_parser.set_defaults(func=controllers.create)
-    create_parser.add_argument("playlist", type=str, help="Provide a playlist Spotify link.")
     create_parser.add_argument(
         "-d",
         "--date",
         action="store_true",
         help="Append the current date to the playlist name",
     )
     create_parser.add_argument(
@@ -41,18 +35,25 @@
     )
     create_parser.add_argument(
         "-n",
         "--name",
         type=str,
         help="Provide a name for the YouTube Music playlist. Default: Spotify playlist name",
     )
+    create_parser.add_argument(
+        "-p",
+        "--public",
+        action="store_true",
+        help="Make created playlist public. Default: private",
+    )
 
     update_parser = subparsers.add_parser(
         "update",
         help="Delete all entries in the provided Google Play Music playlist and update the playlist with entries from the Spotify playlist.",
+        parents=[spotify_playlist],
     )
     update_parser.set_defaults(func=controllers.update)
     update_parser.add_argument(
         "name", type=str, help="The name of the YouTube Music playlist to update."
     )
     update_parser.add_argument(
         "--append", help="Do not delete items, append to target playlist instead"
@@ -62,18 +63,17 @@
         "remove", help="Remove playlists with specified regex pattern."
     )
     remove_parser.set_defaults(func=controllers.remove)
     remove_parser.add_argument("pattern", help="regex pattern")
 
     all_parser = subparsers.add_parser(
         "all",
-        help="Transfer all public playlists of the specified user (Spotify User ID).",
-        parents=[playlist_creator],
+        help="Transfer all public playlists of the specified user (Spotify User ID)."
     )
-    update_parser.add_argument(
+    all_parser.add_argument(
         "user", type=str, help="Spotify userid of the specified user."
     )
     all_parser.set_defaults(func=controllers.all)
 
     return parser.parse_args(args)
```

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/match.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/match.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/spotify.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic/ytmusic.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     def create_playlist(self, name, info, privacy="PRIVATE", tracks=None):
         return self.api.create_playlist(name, info, privacy, video_ids=tracks)
 
     def search_songs(self, tracks):
         videoIds = []
         songs = list(tracks)
         notFound = list()
+        print("Searching YouTube...")
         for i, song in enumerate(songs):
             name = re.sub(r" \(feat.*\..+\)", "", song["name"])
             query = song["artist"] + " " + name
             query = query.replace(" &", "")
             result = self.api.search(query)
             if len(result) == 0:
                 notFound.append(query)
             else:
                 targetSong = get_best_fit_song_id(result, song)
                 if targetSong is None:
                     notFound.append(query)
                 else:
                     videoIds.append(targetSong)
 
-            print("Searching YouTube...")
             if i > 0 and i % 10 == 0:
                 print(f"YouTube tracks: {i}/{len(songs)}")
 
         with open(path + "noresults_youtube.txt", "w", encoding="utf-8") as f:
             f.write("\n".join(notFound))
             f.write("\n")
             f.close()
```

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-to-ytmusic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,29 +24,34 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/sigma67/spotify_to_ytmusic
 Project-URL: repository, https://github.com/sigma67/spotify_to_ytmusic
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 spotify_to_ytmusic
-############################################
+####################
+
 .. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://badges.gitter.im/sigma67/spotify_to_ytmusic.svg
-   :alt: Ask questions at https://gitter.im/sigma67/spotify_to_ytmusic
-   :target: https://gitter.im/sigma67/spotify_to_ytmusic
+.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+   :alt: Ask questions at Discussions
+   :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
 .. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
 .. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
```

### Comparing `spotify_to_ytmusic-0.1.0/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.1.1/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

