# Comparing `tmp/plex_sub_downloader-0.2.0.tar.gz` & `tmp/plex_sub_downloader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex_sub_downloader-0.2.0.tar", last modified: Sat Apr  1 21:22:47 2023, max compression
+gzip compressed data, was "plex_sub_downloader-0.2.1.tar", last modified: Sat Apr  8 21:36:34 2023, max compression
```

## Comparing `plex_sub_downloader-0.2.0.tar` & `plex_sub_downloader-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-01 21:22:47.168074 plex_sub_downloader-0.2.0/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2022-07-14 18:31:06.000000 plex_sub_downloader-0.2.0/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     8292 2023-04-01 21:22:47.167478 plex_sub_downloader-0.2.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     7659 2023-04-01 21:22:19.000000 plex_sub_downloader-0.2.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-01 21:22:47.163843 plex_sub_downloader-0.2.0/plex_sub_downloader/
--rw-r--r--   0 michael    (501) staff       (20)    11429 2023-04-01 21:22:19.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/PlexSubDownloader.py
--rw-r--r--   0 michael    (501) staff       (20)     4321 2022-07-06 20:55:25.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/PlexWebhookEvent.py
--rw-r--r--   0 michael    (501) staff       (20)        0 2022-07-01 14:30:10.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1072 2022-07-18 23:07:21.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/config.schema.json
--rw-r--r--   0 michael    (501) staff       (20)     3282 2023-04-01 21:22:19.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/plex_sub_downloader.py
--rw-r--r--   0 michael    (501) staff       (20)     6095 2023-04-01 21:22:19.000000 plex_sub_downloader-0.2.0/plex_sub_downloader/subliminalHelper.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-01 21:22:47.166687 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     8292 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      531 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       85 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       20 2023-04-01 21:22:47.000000 plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     1048 2023-04-01 21:22:19.000000 plex_sub_downloader-0.2.0/pyproject.toml
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-01 21:22:47.168231 plex_sub_downloader-0.2.0/setup.cfg
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 21:36:34.663309 plex_sub_downloader-0.2.1/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2022-07-14 18:31:06.000000 plex_sub_downloader-0.2.1/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     8781 2023-04-08 21:36:34.662717 plex_sub_downloader-0.2.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     8148 2023-04-08 21:32:23.000000 plex_sub_downloader-0.2.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 21:36:34.659960 plex_sub_downloader-0.2.1/plex_sub_downloader/
+-rw-r--r--   0 michael    (501) staff       (20)    13270 2023-04-08 21:32:23.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/PlexSubDownloader.py
+-rw-r--r--   0 michael    (501) staff       (20)     4321 2022-07-06 20:55:25.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/PlexWebhookEvent.py
+-rw-r--r--   0 michael    (501) staff       (20)        0 2022-07-01 14:30:10.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1072 2022-07-18 23:07:21.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/config.schema.json
+-rw-r--r--   0 michael    (501) staff       (20)     3893 2023-04-08 21:32:23.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/plex_sub_downloader.py
+-rw-r--r--   0 michael    (501) staff       (20)     6095 2023-04-08 21:15:12.000000 plex_sub_downloader-0.2.1/plex_sub_downloader/subliminalHelper.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 21:36:34.662203 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     8781 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      531 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       85 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       20 2023-04-08 21:36:34.000000 plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1048 2023-04-08 21:35:56.000000 plex_sub_downloader-0.2.1/pyproject.toml
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-08 21:36:34.663457 plex_sub_downloader-0.2.1/setup.cfg
```

### Comparing `plex_sub_downloader-0.2.0/LICENSE.txt` & `plex_sub_downloader-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plex_sub_downloader-0.2.0/PKG-INFO` & `plex_sub_downloader-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex_sub_downloader
-Version: 0.2.0
+Version: 0.2.1
 Summary: A (hopefully) straightforward cli tool for downloading subtitles for newly added Plex media.
 Author-email: replicatingTrouts <replicatingTrouts@gmail.com>
 Project-URL: Homepage, https://github.com/replicatingTrouts/plex-sub-downloader
 Project-URL: Bug Tracker, https://github.com/replicatingTrouts/plex-sub-downloader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -78,17 +78,17 @@
 ```
 2022-07-16 21:08:38:plex_sub_downloader:INFO - Testing config file '/path/to/config.json'
 2022-07-16 21:08:38:plex_sub_downloader:INFO - config file is valid.
 ```
 
 <br />
 
-# Running
+# Running the Webhook Listener Thing
 
-To start plex_sub_downloader, run:
+To start plex_sub_downloader in webhook mode, run:
 ```
 plex_sub_downloader --config path/to/config.json start-webhook
 ``` 
 
 Assuming it starts and runs correctly, you should see something like the following:
 ```
  2023-04-01 15:51:01:PlexSubDownloader:INFO - Configuring PlexSubDownloader
@@ -129,24 +129,34 @@
 2022-07-19 14:14:32:PlexSubDownloader:INFO - found 1 for video /path/to/movies/Wild.Wild.West.1999/Wild.Wild.West.1999.mp4
 ```
 
 Congrats! It's probably working?
 
 <br />
 
+# Manually Running for a Specific Video
+
+plex_sub_downloader also has a command for manually checking a Movie, Episode, Season, or Show for missing subtitles.
+Simply run plex_sub_downloader with the `check-video` command option, and pass it the item's metadata key:
+
+```
+plex_sub_downloader --config path/to/config.json check-video /library/metadata/42069
+```
+
 # Command-line Arguments
 
 | Argument | Description |
 | -------- | ----------- |
 | -h, --help | Show this help message and exits |
 | -v, --version | Prints version info and exits |
 | -c CONFIG, --config CONFIG | Config File |
 | -d, --debug | Enable debug logging |
 | configtest | Run validation on config file |
-| start-webhook| Run http webhook server |
+| start-webhook | Run http webhook server |
+| check-video {video key} | Manually check the given video for missing subtitles. |
 
 <br />
 
 # Configuration
 
 | Parameter | Required? | Description |
 | --------- | --------- | ----------- |
```

### Comparing `plex_sub_downloader-0.2.0/README.md` & `plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: plex-sub-downloader
+Version: 0.2.1
+Summary: A (hopefully) straightforward cli tool for downloading subtitles for newly added Plex media.
+Author-email: replicatingTrouts <replicatingTrouts@gmail.com>
+Project-URL: Homepage, https://github.com/replicatingTrouts/plex-sub-downloader
+Project-URL: Bug Tracker, https://github.com/replicatingTrouts/plex-sub-downloader/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 Plex Sub Downloader
 ===================
 
 
 ## What is it?
 
 This is a command-line tool designed to automate the downloading of subtitles for media on your [Plex Media Server](https://www.plex.tv/). It makes use of [Flask](https://flask.palletsprojects.com/en/2.1.x/) and [Python-PlexAPI](https://github.com/pkkid/python-plexapi) to listen for newly-added media, and [Subliminal](https://github.com/Diaoul/subliminal) to search your favorite subtitle providers.
@@ -64,17 +78,17 @@
 ```
 2022-07-16 21:08:38:plex_sub_downloader:INFO - Testing config file '/path/to/config.json'
 2022-07-16 21:08:38:plex_sub_downloader:INFO - config file is valid.
 ```
 
 <br />
 
-# Running
+# Running the Webhook Listener Thing
 
-To start plex_sub_downloader, run:
+To start plex_sub_downloader in webhook mode, run:
 ```
 plex_sub_downloader --config path/to/config.json start-webhook
 ``` 
 
 Assuming it starts and runs correctly, you should see something like the following:
 ```
  2023-04-01 15:51:01:PlexSubDownloader:INFO - Configuring PlexSubDownloader
@@ -115,24 +129,34 @@
 2022-07-19 14:14:32:PlexSubDownloader:INFO - found 1 for video /path/to/movies/Wild.Wild.West.1999/Wild.Wild.West.1999.mp4
 ```
 
 Congrats! It's probably working?
 
 <br />
 
+# Manually Running for a Specific Video
+
+plex_sub_downloader also has a command for manually checking a Movie, Episode, Season, or Show for missing subtitles.
+Simply run plex_sub_downloader with the `check-video` command option, and pass it the item's metadata key:
+
+```
+plex_sub_downloader --config path/to/config.json check-video /library/metadata/42069
+```
+
 # Command-line Arguments
 
 | Argument | Description |
 | -------- | ----------- |
 | -h, --help | Show this help message and exits |
 | -v, --version | Prints version info and exits |
 | -c CONFIG, --config CONFIG | Config File |
 | -d, --debug | Enable debug logging |
 | configtest | Run validation on config file |
-| start-webhook| Run http webhook server |
+| start-webhook | Run http webhook server |
+| check-video {video key} | Manually check the given video for missing subtitles. |
 
 <br />
 
 # Configuration
 
 | Parameter | Required? | Description |
 | --------- | --------- | ----------- |
```

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader/PlexSubDownloader.py` & `plex_sub_downloader-0.2.1/plex_sub_downloader/PlexSubDownloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,107 +57,154 @@
         Retrieves the relevent item from Plex and searches for subtitles.
         :param PlexWebhookEvent event:
         """
         log.info("Handling library.new event")
         log.info(f'Title: {event.Metadata.title}, type: {event.Metadata.type}, section: {event.Metadata.librarySectionTitle}')
         
         video = self.getVideoItemFromEvent(event)
+        if video is None:
+            log.info("Video referenced in event could not be retrieved.")
+            return
+        
+        self.handleDownloadingVideoSubtitles(video)
+
+    def manuallyCheckVideoSubtitles(self, video_key):
+        """Manually check video for missing subtitles, and try to download missing subs.
+        """
 
+        video = self.getVideoItem(video_key)
+        if video is None:
+            log.info(f"Video with key {video_key} could not be retrieved.")
+            return 
+        self.handleDownloadingVideoSubtitles(video)
+
+    def handleDownloadingVideoSubtitles(self, video):
         missingVideos = self.getVidsMissingSubtitles([video])
         log.info("Found " + str(len(missingVideos)) + " videos missing subtitles")
         log.info([f'{video.title}, {video.key}' for video in missingVideos])
         if len(missingVideos) > 0:
             subtitles = self.downloadSubtitlesForVideos(missingVideos)
 
             if self.subtitle_destination == "metadata":
                 self.uploadSubtitlesToMetadata(missingVideos, subtitles)
             else:
                 self.sub.save_subtitles(subtitles)
         else:
             log.info("No subtitles to download, doing nothing!")
-
+        
     def getVideoItemFromEvent(self, event):
          # if Metadata.type == "show", then the metadata key looks like
         # `/library/metadata/45533/children`, which doesn't return what we actually want
         # when we call fetchItem
         key = event.Metadata.key
+        return self.getVideoItem(key)
+    
+    def getVideoItem(self, key):
         key = key.replace("/children", "")
-        video = self.plexServer.fetchItem(ekey=key)
-        video.reload()
-        return video
-
+        try:
+            video = self.plexServer.fetchItem(ekey=key)
+            video.reload()
+            return video
+        except Exception as e:
+            log.error(f'Error while trying to retrieve video with key {key}')
+            log.error(e)
+            return None
+    
 
     def getVidsMissingSubtitles(self,videos):
         """Search the given list of videos for ones that don't already have subtitles.
         For videos of type 'season' or 'show', this will search through all of the episodes
         as well.
         :param list videos: list of plexapi.video.Video objects.
         :return: list of Video objects that don't have any subtitles.
         """
 
         vidsMissingSubs = []
         for v in videos:
             if v.type == 'movie' or v.type == 'episode':
-                if self.checkVideoForSubtitles(v) == False:
+                if self.isVideoMissingSubtitles(v):
                     vidsMissingSubs.append(v)
                 
             elif v.type == 'season' or v.type == 'show':
                 eps = v.episodes()
                 for e in eps:
                     e.reload()
-                    if self.checkVideoForSubtitles(e) == False:
+                    if self.isVideoMissingSubtitles(e):
                         vidsMissingSubs.append(e)
 
         return vidsMissingSubs
 
-    def checkVideoForSubtitles(self, video):
-        """Checks the given video for subtitles by retrieving the SubtitleStreams.
-        Checks against the list of languages provided in config['languages']. If _any_ 
-        language isn't found, this will return False.
+    def isVideoMissingSubtitles(self, video):
+        """Checks the given video to see if it's missing subtitles for any of the languages defined in config['languages'].
         :param video: plexapi.video.Video object
-        :return: boolean, True if the video has subtitles for every requested language, False otherwise
+        :return: boolean, False if the video has subtitles for every requested language, True otherwise
         """
+
+        missingSubtitles = self.getMissingSubtitleLanguages(video)
+        return len(missingSubtitles) > 0
+    
+    def getMissingSubtitleLanguages(self, video):
+        """Compares the existing subtitle languages on the video to the languages requested based on config['languages'],
+        and returns requested languages that aren't already present.
+        :param video: plexapi.video.Video object
+        :return: array of language codes
+        """
+        requestedLanguages = self.config['languages'].copy()
+
+        existingSubtitleLanguages = self.getVideoSubtitleLanguageCodes(video)
         
-        languagesNotFound = self.config['languages']
+        for languageCode in existingSubtitleLanguages:
+            if languageCode in requestedLanguages:
+                requestedLanguages.remove(languageCode)
+        log.info(f'Video {video.title} {video.key} is missing {len(requestedLanguages)} subtitle languages:')
+        log.info(f'{requestedLanguages}')
 
+        return requestedLanguages
+
+    def getVideoSubtitleLanguageCodes(self, video):
+        """Gets the language codes for any SubtitleStreams on the given video.
+        :param video: plexapi.video.Video object
+        :return: array of language codes
+        """
         subs = video.subtitleStreams()
-        log.debug(f'Found {len(subs)} subtitles for video {video.title} {video.key}')
+        log.info(f'Found {len(subs)} subtitles for video {video.title} {video.key}')
+        languageCodes = []
         for sub in subs:
-            log.debug(f'subtitle {sub.displayTitle} language code:{sub.languageCode}, format: {sub.format}, forced: {sub.forced}')
-            if sub.languageCode in languagesNotFound:
-                languagesNotFound.remove(sub.languageCode)
-        
-        return len(languagesNotFound) == 0
+            log.info(f'subtitle {sub.displayTitle} language code:{sub.languageCode}, format: {sub.format}, forced: {sub.forced}')
+            languageCodes.append(sub.languageCode)
         
+        return languageCodes
+
+
     def downloadSubtitlesForVideos(self, videos):
         """Attempts to download subtitles for the given list of videos.
         :param list videos: list of plexapi.video.Video objects.
         :return: dict[subliminal.video.Video, list[subliminal.subtitle.Subtitle]]
         """
 
-        log.info("Downloading subtitles for " + str(len(videos)) + " videos")
+        log.info(f"Downloading subtitles for {len(videos)} videos:")
         log.info([video.title for video in videos])
         subtitles = self.sub.search_videos(videos)
         return subtitles
 
 
-    def uploadSubtitlesToMetadata(self, plexVideos, subtitles):
+    def uploadSubtitlesToMetadata(self, plexVideos, subtitleDict):
         """Saves the subtitles to Plex.
         :param list plexVideos: list of plexapi.video.Video objects.
         :param dict subtitles: dict of dict[subliminal.video.Video, list[subliminal.subtitle.Subtitle]]
         """
 
         log.info("Saving subtitles to Plex metadata")
         tempdir = tempfile.gettempdir()
         for video in plexVideos:
             mediaPart = video.media[0].parts[0]
             filepath = video.media[0].parts[0].file
-            for subVideo, subtitles in subtitles.items():
+            for subVideo, subtitles in subtitleDict.items():
                 if subVideo.name == filepath:
-                    log.info(f'found {len(subtitles)} for video {subVideo.name}')
+                    log.debug(f'found {len(subtitles)} subtitles for video {subVideo.name}')
 
                     savedSubtitlePaths = self.sub.save_subtitle(subVideo, subtitles, destination=tempdir)
                     for subtitlePath in savedSubtitlePaths:
                         log.debug(f'Uploading subtitles \'{subtitlePath}\' to video {video.title} {video.key}')
                         originalDefault = None 
                         existingSubs = video.subtitleStreams();
                         for sub in existingSubs:
```

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader/PlexWebhookEvent.py` & `plex_sub_downloader-0.2.1/plex_sub_downloader/PlexWebhookEvent.py`

 * *Files identical despite different names*

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader/config.schema.json` & `plex_sub_downloader-0.2.1/plex_sub_downloader/config.schema.json`

 * *Files identical despite different names*

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader/subliminalHelper.py` & `plex_sub_downloader-0.2.1/plex_sub_downloader/subliminalHelper.py`

 * *Files identical despite different names*

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/PKG-INFO` & `plex_sub_downloader-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: plex-sub-downloader
-Version: 0.2.0
-Summary: A (hopefully) straightforward cli tool for downloading subtitles for newly added Plex media.
-Author-email: replicatingTrouts <replicatingTrouts@gmail.com>
-Project-URL: Homepage, https://github.com/replicatingTrouts/plex-sub-downloader
-Project-URL: Bug Tracker, https://github.com/replicatingTrouts/plex-sub-downloader/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 Plex Sub Downloader
 ===================
 
 
 ## What is it?
 
 This is a command-line tool designed to automate the downloading of subtitles for media on your [Plex Media Server](https://www.plex.tv/). It makes use of [Flask](https://flask.palletsprojects.com/en/2.1.x/) and [Python-PlexAPI](https://github.com/pkkid/python-plexapi) to listen for newly-added media, and [Subliminal](https://github.com/Diaoul/subliminal) to search your favorite subtitle providers.
@@ -78,17 +64,17 @@
 ```
 2022-07-16 21:08:38:plex_sub_downloader:INFO - Testing config file '/path/to/config.json'
 2022-07-16 21:08:38:plex_sub_downloader:INFO - config file is valid.
 ```
 
 <br />
 
-# Running
+# Running the Webhook Listener Thing
 
-To start plex_sub_downloader, run:
+To start plex_sub_downloader in webhook mode, run:
 ```
 plex_sub_downloader --config path/to/config.json start-webhook
 ``` 
 
 Assuming it starts and runs correctly, you should see something like the following:
 ```
  2023-04-01 15:51:01:PlexSubDownloader:INFO - Configuring PlexSubDownloader
@@ -129,24 +115,34 @@
 2022-07-19 14:14:32:PlexSubDownloader:INFO - found 1 for video /path/to/movies/Wild.Wild.West.1999/Wild.Wild.West.1999.mp4
 ```
 
 Congrats! It's probably working?
 
 <br />
 
+# Manually Running for a Specific Video
+
+plex_sub_downloader also has a command for manually checking a Movie, Episode, Season, or Show for missing subtitles.
+Simply run plex_sub_downloader with the `check-video` command option, and pass it the item's metadata key:
+
+```
+plex_sub_downloader --config path/to/config.json check-video /library/metadata/42069
+```
+
 # Command-line Arguments
 
 | Argument | Description |
 | -------- | ----------- |
 | -h, --help | Show this help message and exits |
 | -v, --version | Prints version info and exits |
 | -c CONFIG, --config CONFIG | Config File |
 | -d, --debug | Enable debug logging |
 | configtest | Run validation on config file |
-| start-webhook| Run http webhook server |
+| start-webhook | Run http webhook server |
+| check-video {video key} | Manually check the given video for missing subtitles. |
 
 <br />
 
 # Configuration
 
 | Parameter | Required? | Description |
 | --------- | --------- | ----------- |
```

### Comparing `plex_sub_downloader-0.2.0/plex_sub_downloader.egg-info/SOURCES.txt` & `plex_sub_downloader-0.2.1/plex_sub_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plex_sub_downloader-0.2.0/pyproject.toml` & `plex_sub_downloader-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["plex_sub_downloader*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.schema.json"]
 
 [project]
 name = "plex_sub_downloader"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="replicatingTrouts", email="replicatingTrouts@gmail.com" },
 ]
 description = "A (hopefully) straightforward cli tool for downloading subtitles for newly added Plex media."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

