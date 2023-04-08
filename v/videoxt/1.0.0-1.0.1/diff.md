# Comparing `tmp/videoxt-1.0.0.tar.gz` & `tmp/videoxt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videoxt-1.0.0.tar", last modified: Sun Apr  2 02:35:48 2023, max compression
+gzip compressed data, was "videoxt-1.0.1.tar", last modified: Sat Apr  8 18:23:57 2023, max compression
```

## Comparing `videoxt-1.0.0.tar` & `videoxt-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 02:35:48.816769 videoxt-1.0.0/
--rw-rw-rw-   0        0        0     1093 2023-03-04 04:21:35.000000 videoxt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    12937 2023-04-02 02:35:48.816769 videoxt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    12178 2023-04-02 02:31:47.000000 videoxt-1.0.0/README.md
--rw-rw-rw-   0        0        0     1067 2023-04-02 02:35:48.819770 videoxt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-24 20:43:32.000000 videoxt-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 02:35:48.701770 videoxt-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-05 19:38:31.000000 videoxt-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-03-14 03:10:31.000000 videoxt-1.0.0/tests/utils_test.py
--rw-rw-rw-   0        0        0    23911 2023-03-31 01:36:07.000000 videoxt-1.0.0/tests/validators_test.py
-drwxrwxrwx   0        0        0        0 2023-04-02 02:35:48.750769 videoxt-1.0.0/videoxt/
--rw-rw-rw-   0        0        0      154 2023-03-31 01:40:22.000000 videoxt-1.0.0/videoxt/__init__.py
--rw-rw-rw-   0        0        0     8942 2023-04-02 02:26:05.000000 videoxt-1.0.0/videoxt/api.py
--rw-rw-rw-   0        0        0     7947 2023-04-02 02:26:05.000000 videoxt-1.0.0/videoxt/cli.py
--rw-rw-rw-   0        0        0      774 2023-03-31 01:36:46.000000 videoxt-1.0.0/videoxt/constants.py
--rw-rw-rw-   0        0        0     4435 2023-04-02 02:25:44.000000 videoxt-1.0.0/videoxt/displays.py
--rw-rw-rw-   0        0        0     1971 2023-04-01 01:26:22.000000 videoxt-1.0.0/videoxt/editors.py
--rw-rw-rw-   0        0        0      109 2023-03-28 19:24:36.000000 videoxt-1.0.0/videoxt/exceptions.py
--rw-rw-rw-   0        0        0     9146 2023-04-01 19:20:56.000000 videoxt-1.0.0/videoxt/extractors.py
--rw-rw-rw-   0        0        0     5952 2023-04-01 18:33:23.000000 videoxt-1.0.0/videoxt/preppers.py
--rw-rw-rw-   0        0        0     8729 2023-04-01 18:57:03.000000 videoxt-1.0.0/videoxt/requestors.py
--rw-rw-rw-   0        0        0     1900 2023-04-01 19:04:32.000000 videoxt-1.0.0/videoxt/utils.py
--rw-rw-rw-   0        0        0    12816 2023-04-01 18:36:41.000000 videoxt-1.0.0/videoxt/validators.py
--rw-rw-rw-   0        0        0     2596 2023-04-01 18:59:11.000000 videoxt-1.0.0/videoxt/video.py
-drwxrwxrwx   0        0        0        0 2023-04-02 02:35:48.812767 videoxt-1.0.0/videoxt.egg-info/
--rw-rw-rw-   0        0        0    12937 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-02 02:35:48.000000 videoxt-1.0.0/videoxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:23:57.140540 videoxt-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-03-04 04:21:35.000000 videoxt-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    12937 2023-04-08 18:23:57.140540 videoxt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12178 2023-04-02 02:31:47.000000 videoxt-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1067 2023-04-08 18:23:57.144541 videoxt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-24 20:43:32.000000 videoxt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:23:57.069194 videoxt-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-05 19:38:31.000000 videoxt-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3586 2023-04-02 19:05:14.000000 videoxt-1.0.1/tests/utils_test.py
+-rw-rw-rw-   0        0        0    23911 2023-03-31 01:36:07.000000 videoxt-1.0.1/tests/validators_test.py
+-rw-rw-rw-   0        0        0     1216 2023-04-08 18:11:55.000000 videoxt-1.0.1/tests/video_test.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:23:57.098544 videoxt-1.0.1/videoxt/
+-rw-rw-rw-   0        0        0      154 2023-03-31 01:40:22.000000 videoxt-1.0.1/videoxt/__init__.py
+-rw-rw-rw-   0        0        0     8942 2023-04-02 02:26:05.000000 videoxt-1.0.1/videoxt/api.py
+-rw-rw-rw-   0        0        0     7947 2023-04-02 02:26:05.000000 videoxt-1.0.1/videoxt/cli.py
+-rw-rw-rw-   0        0        0      774 2023-03-31 01:36:46.000000 videoxt-1.0.1/videoxt/constants.py
+-rw-rw-rw-   0        0        0     4435 2023-04-02 02:25:44.000000 videoxt-1.0.1/videoxt/displays.py
+-rw-rw-rw-   0        0        0     1971 2023-04-01 01:26:22.000000 videoxt-1.0.1/videoxt/editors.py
+-rw-rw-rw-   0        0        0      109 2023-03-28 19:24:36.000000 videoxt-1.0.1/videoxt/exceptions.py
+-rw-rw-rw-   0        0        0     9168 2023-04-08 01:38:30.000000 videoxt-1.0.1/videoxt/extractors.py
+-rw-rw-rw-   0        0        0     5952 2023-04-01 18:33:23.000000 videoxt-1.0.1/videoxt/preppers.py
+-rw-rw-rw-   0        0        0     8729 2023-04-01 18:57:03.000000 videoxt-1.0.1/videoxt/requestors.py
+-rw-rw-rw-   0        0        0     1900 2023-04-02 18:43:06.000000 videoxt-1.0.1/videoxt/utils.py
+-rw-rw-rw-   0        0        0    12816 2023-04-01 18:36:41.000000 videoxt-1.0.1/videoxt/validators.py
+-rw-rw-rw-   0        0        0     3610 2023-04-08 18:11:55.000000 videoxt-1.0.1/videoxt/video.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:23:57.138542 videoxt-1.0.1/videoxt.egg-info/
+-rw-rw-rw-   0        0        0    12937 2023-04-08 18:23:56.000000 videoxt-1.0.1/videoxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-04-08 18:23:57.000000 videoxt-1.0.1/videoxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:23:56.000000 videoxt-1.0.1/videoxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-08 18:23:56.000000 videoxt-1.0.1/videoxt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-04-08 18:23:56.000000 videoxt-1.0.1/videoxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-08 18:23:56.000000 videoxt-1.0.1/videoxt.egg-info/top_level.txt
```

### Comparing `videoxt-1.0.0/LICENSE` & `videoxt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/PKG-INFO` & `videoxt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoxt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extract audio, clips, frames and create gifs from a video.
 Home-page: https://github.com/gurrutia/videoxt
 Author: Gerardo Urrutia
 Author-email: durru7@gmail.com
 License: MIT
 Keywords: video,frame,image,gif,audio,extract,convert,ffmpeg,moviepy,opencv
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: videoxt Version: 1.0.0 Summary: Extract audio,
+Metadata-Version: 2.1 Name: videoxt Version: 1.0.1 Summary: Extract audio,
 clips, frames and create gifs from a video. Home-page: https://github.com/
 gurrutia/videoxt Author: Gerardo Urrutia Author-email: durru7@gmail.com
 License: MIT Keywords:
 video,frame,image,gif,audio,extract,convert,ffmpeg,moviepy,opencv Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Topic :: Multimedia :: Graphics Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `videoxt-1.0.0/README.md` & `videoxt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/setup.cfg` & `videoxt-1.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6964 656f 7874 0d0a 7665 7273   = videoxt..vers
-00000020: 696f 6e20 3d20 312e 302e 300d 0a64 6573  ion = 1.0.0..des
+00000020: 696f 6e20 3d20 312e 302e 310d 0a64 6573  ion = 1.0.1..des
 00000030: 6372 6970 7469 6f6e 203d 2045 7874 7261  cription = Extra
 00000040: 6374 2061 7564 696f 2c20 636c 6970 732c  ct audio, clips,
 00000050: 2066 7261 6d65 7320 616e 6420 6372 6561   frames and crea
 00000060: 7465 2067 6966 7320 6672 6f6d 2061 2076  te gifs from a v
 00000070: 6964 656f 2e0d 0a6c 6f6e 675f 6465 7363  ideo...long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
```

### Comparing `videoxt-1.0.0/tests/validators_test.py` & `videoxt-1.0.1/tests/validators_test.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/api.py` & `videoxt-1.0.1/videoxt/api.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/cli.py` & `videoxt-1.0.1/videoxt/cli.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/constants.py` & `videoxt-1.0.1/videoxt/constants.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/displays.py` & `videoxt-1.0.1/videoxt/displays.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/editors.py` & `videoxt-1.0.1/videoxt/editors.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/extractors.py` & `videoxt-1.0.1/videoxt/extractors.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,68 +131,64 @@
         """Apply edits to an image `numpy.ndarray`."""
         return E.edit_image(
             image, self.request.dimensions, self.request.rotate, self.request.monochrome
         )
 
     def extract(self) -> None:
         """Extract frames from a video and save them to a directory as images."""
-        video_capture = cv2.VideoCapture(str(self.request.video.filepath))
-
         if not self.request.destdir.exists():
             self.request.destdir.mkdir()
 
         if self.request.verbose:
             print(self.request.video.__str__() + str(self.request))
 
         with Progress(transient=True) as progress:
             task = progress.add_task(
-                "EXTRACTING FRAMES", total=self.request.images_expected
+                "EXTRACTING FRAMES",
+                total=self.request.images_expected,
             )
 
-            frame_numbers = itertools.count(
+            images_written = 0
+            frame_queue = itertools.count(
                 start=self.request.time_range.start_frame,
                 step=self.request.capture_rate,
             )
+            for frame_num in frame_queue:
+                with self.request.video.open_capture() as opencap:
+                    opencap.set(cv2.CAP_PROP_POS_FRAMES, frame_num)
+                    read_successful, image = opencap.read()
+
+                    if not read_successful:
+                        break
+
+                    # Generate the filepath for the next image to be written
+                    image_filepath = P.prepare_filepath_image(
+                        self.request.destdir,
+                        self.request.filename,
+                        frame_num,
+                        self.request.image_format,
+                    )
+                    image = self.apply_edits(image)
+                    cv2.imwrite(image_filepath, image)
+                    images_written += 1
+
+                    # Update progress bar
+                    progress.update(
+                        task,
+                        advance=1,
+                        description=(
+                            f"[yellow]EXTRACTING FRAMES FROM "
+                            f"{self.request.video.filepath.name!r} "
+                            f"[{images_written}/{self.request.images_expected}]"
+                            f"[/yellow]"
+                        ),
+                    )
 
-            images_written = 0
-
-            for frame_num in frame_numbers:
-                video_capture.set(cv2.CAP_PROP_POS_FRAMES, frame_num)
-                read_successful, image = video_capture.read()
-
-                if not read_successful:
-                    break
-
-                # Generate the filepath for the next image to be written
-                image_filepath = P.prepare_filepath_image(
-                    self.request.destdir,
-                    self.request.filename,
-                    frame_num,
-                    self.request.image_format,
-                )
-                image = self.apply_edits(image)
-                cv2.imwrite(image_filepath, image)
-
-                images_written += 1
-
-                # Update progress bar
-                progress.update(
-                    task,
-                    advance=1,
-                    description=(
-                        f"[yellow]EXTRACTING FRAMES FROM {self.request.video.filepath.name!r} "
-                        f"[{images_written}/{self.request.images_expected}][/yellow]"
-                    ),
-                )
-
-                # Stop extracting frames when the expected number of frames have been written
-                if images_written == self.request.images_expected:
-                    break
-
-        video_capture.release()
+                    if images_written == self.request.images_expected:
+                        break
 
         print(f"[green]FRAMES EXTRACTED: {self.request.destdir.resolve()}[/green]")
 
 
 @dataclass
 class GifExtractor(Extractor):
     """Applies edits to a VideoFileClip and extracts the gif from the clip."""
```

### Comparing `videoxt-1.0.0/videoxt/preppers.py` & `videoxt-1.0.1/videoxt/preppers.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/requestors.py` & `videoxt-1.0.1/videoxt/requestors.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/utils.py` & `videoxt-1.0.1/videoxt/utils.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt/validators.py` & `videoxt-1.0.1/videoxt/validators.py`

 * *Files identical despite different names*

### Comparing `videoxt-1.0.0/videoxt.egg-info/PKG-INFO` & `videoxt-1.0.1/videoxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoxt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extract audio, clips, frames and create gifs from a video.
 Home-page: https://github.com/gurrutia/videoxt
 Author: Gerardo Urrutia
 Author-email: durru7@gmail.com
 License: MIT
 Keywords: video,frame,image,gif,audio,extract,convert,ffmpeg,moviepy,opencv
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: videoxt Version: 1.0.0 Summary: Extract audio,
+Metadata-Version: 2.1 Name: videoxt Version: 1.0.1 Summary: Extract audio,
 clips, frames and create gifs from a video. Home-page: https://github.com/
 gurrutia/videoxt Author: Gerardo Urrutia Author-email: durru7@gmail.com
 License: MIT Keywords:
 video,frame,image,gif,audio,extract,convert,ffmpeg,moviepy,opencv Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Topic :: Multimedia :: Graphics Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `videoxt-1.0.0/videoxt.egg-info/SOURCES.txt` & `videoxt-1.0.1/videoxt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 tests/__init__.py
 tests/utils_test.py
 tests/validators_test.py
+tests/video_test.py
 videoxt/__init__.py
 videoxt/api.py
 videoxt/cli.py
 videoxt/constants.py
 videoxt/displays.py
 videoxt/editors.py
 videoxt/exceptions.py
```

