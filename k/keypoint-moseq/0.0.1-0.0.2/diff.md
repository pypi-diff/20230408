# Comparing `tmp/keypoint-moseq-0.0.1.tar.gz` & `tmp/keypoint-moseq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.0.1.tar", last modified: Tue Mar 28 23:12:29 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.0.2.tar", last modified: Fri Apr  7 22:26:29 2023, max compression
```

## Comparing `keypoint-moseq-0.0.1.tar` & `keypoint-moseq-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-28 23:12:29.740463 keypoint-moseq-0.0.1/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-03-27 14:28:54.000000 keypoint-moseq-0.0.1/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-03-27 14:28:54.000000 keypoint-moseq-0.0.1/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-03-28 23:12:29.740652 keypoint-moseq-0.0.1/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4514 2023-03-27 14:28:54.000000 keypoint-moseq-0.0.1/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-28 23:12:29.738160 keypoint-moseq-0.0.1/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      633 2023-02-25 00:06:15.000000 keypoint-moseq-0.0.1/keypoint_moseq/__init__.py
--rw-rw-r--   0 calebweinreb   (501) staff       (20)    21235 2022-12-01 15:26:20.000000 keypoint-moseq-0.0.1/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17620 2023-02-10 16:07:10.000000 keypoint-moseq-0.0.1/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16129 2023-03-11 00:23:09.000000 keypoint-moseq-0.0.1/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32706 2023-03-28 23:11:41.000000 keypoint-moseq-0.0.1/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28227 2023-03-28 23:11:41.000000 keypoint-moseq-0.0.1/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    59378 2023-03-28 23:11:41.000000 keypoint-moseq-0.0.1/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-03-28 23:12:29.740067 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-03-28 23:12:29.000000 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-03-28 23:12:29.000000 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-03-28 23:12:29.000000 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      131 2023-03-28 23:12:29.000000 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-03-28 23:12:29.000000 keypoint-moseq-0.0.1/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-03-28 23:12:29.741483 keypoint-moseq-0.0.1/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      814 2023-03-28 23:11:41.000000 keypoint-moseq-0.0.1/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.017337 keypoint-moseq-0.0.2/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-07 22:26:29.017483 keypoint-moseq-0.0.2/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4694 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.015037 keypoint-moseq-0.0.2/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      633 2023-02-25 00:06:15.000000 keypoint-moseq-0.0.2/keypoint_moseq/__init__.py
+-rw-rw-r--   0 calebweinreb   (501) staff       (20)    21235 2022-12-01 15:26:20.000000 keypoint-moseq-0.0.2/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17620 2023-02-10 16:07:10.000000 keypoint-moseq-0.0.2/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    16129 2023-03-11 00:23:09.000000 keypoint-moseq-0.0.2/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    32763 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28233 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    60436 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.017011 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-07 22:26:29.018123 keypoint-moseq-0.0.2/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      807 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/setup.py
```

### Comparing `keypoint-moseq-0.0.1/LICENSE.md` & `keypoint-moseq-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/NOTICE.md` & `keypoint-moseq-0.0.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/README.md` & `keypoint-moseq-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 - [Slack workspace](https://join.slack.com/t/moseqworkspace/shared_invite/zt-151x0shoi-z4J0_g_5rwJDlO1IfCU34A)
 
 - [MoSeq homepage](https://dattalab.github.io/moseq2-website/index.html)
 
 ## Installation
 
+- The first import of `keypoint_moseq` after installation can take a few minutes. 
+- To install on a Mac with an M1 chip, we recommend option 2 (conda environment installation).
+
 ### Option 1: Install using pip
 
 1. If you plan to use a GPU (recommended), install the appropriate driver and CUDA version. CUDA ≥11.1 and cuDNN ≥8.2 are required. [This section of the DeepLabCut docs](https://deeplabcut.github.io/DeepLabCut/docs/installation.html#gpu-support) may be helpful.
 
 
 2. Install [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html). Create and activate an environment called `keypoint_moseq` with python 3.9:
 ```
@@ -87,14 +90,15 @@
 See [this issue](https://github.com/dattalab/keypoint-moseq/issues/5) for updates regarding Apple Silicon (M1/M2) support. For now, you can use the Mac (CPU) version on newer Macs.
 
 3. Activate the new environment:
 ```
 conda activate keypoint_moseq
 ```
 
+
 ### Troubleshooting
 #### `UNKNOWN: no kernel image is available for execution on the device`
 If you're running into issues when trying to use the GPU-accelerated version, you might see this error message:
 ```
 jaxlib.xla_extension.XlaRuntimeError: UNKNOWN: no kernel image is available for execution on the device
 ```
 First, check if Jax can detect your GPU:
```

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/__init__.py` & `keypoint-moseq-0.0.2/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/analysis.py` & `keypoint-moseq-0.0.2/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/calibration.py` & `keypoint-moseq-0.0.2/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/fitting.py` & `keypoint-moseq-0.0.2/keypoint_moseq/fitting.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/io.py` & `keypoint-moseq-0.0.2/keypoint_moseq/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -743,15 +743,16 @@
     
     if return_bodyparts: 
         return coordinates,confidences,bodyparts
     else: return coordinates,confidences
 
 
 
-def load_sleap_results(filepath_pattern, recursive=True, return_bodyparts=False):
+def load_sleap_results(filepath_pattern, recursive=True, path_sep='-',
+                       path_in_name=False, return_bodyparts=False):
     """
     Load keypoints from sleap hdf5 files.
 
     Parameters
     ----------
     filepath_pattern: str, default=None
         Filepath pattern for a set of sleap hdf5 files, or a list of
```

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/util.py` & `keypoint-moseq-0.0.2/keypoint_moseq/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,26 +292,26 @@
         extensions = [video_extension]
 
     videos = list_files_with_exts(video_dir, extensions, recursive=recursive)
     videos_to_paths = {os.path.splitext(os.path.basename(f))[0]:f for f in videos}
 
     video_paths = []
     for key in keys:
-
-        matches,lengths = tuple(zip(
-            *[(path,len(video)) for video,path in videos_to_paths.items() 
-            if os.path.basename(key).startswith(video+session_name_suffix)]))
-        
+        matches = [v for v in videos_to_paths if \
+                   os.path.basename(key).startswith(v+session_name_suffix)]
         assert len(matches)>0, fill(f'No matching videos found for {key}')
-        video_paths.append(matches[np.argmax(lengths)])
+        
+        longest_match = sorted(matches, key=lambda v: len(v))[-1]
+        video_paths.append(videos_to_paths[longest_match])
 
     if as_dict: return dict(zip(sorted(keys),video_paths))
     else: return video_paths
 
 
+
 def pad_along_axis(arr, pad_widths, axis=0, value=0):
     """
     Pad an array along a single axis
 
     Parameters
     -------
     arr: ndarray, Array to be padded
```

### Comparing `keypoint-moseq-0.0.1/keypoint_moseq/viz.py` & `keypoint-moseq-0.0.2/keypoint_moseq/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import os
 import cv2
 import tqdm
 import imageio
 import warnings
+import logging
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.ndimage import gaussian_filter1d
-plt.rcParams['figure.dpi'] = 100
-warnings.formatwarning = lambda msg, *a: str(msg)
-
 from vidio.read import OpenCVReader
 from textwrap import fill
 
 from keypoint_moseq.util import (
     get_edges, get_durations, get_frequencies, reindex_by_bodyparts,
     find_matching_videos, get_syllable_instances, sample_instances,
     filter_centroids_headings, get_trajectories, interpolate_keypoints,
     interpolate_along_axis
 )
 from keypoint_moseq.io import load_results
 from jax_moseq.models.keypoint_slds import center_embedding
 
+# simple warning formatting
+plt.rcParams['figure.dpi'] = 100
+warnings.formatwarning = lambda msg, *a: str(msg)
+
+# suppress warnings from imageio
+logging.getLogger().setLevel(logging.ERROR)
+
+
 
 def crop_image(image, centroid, crop_size):
     """
     Crop an image around a centroid.
 
     Parameters
     ----------
@@ -320,15 +326,31 @@
                 'or a ``name`` and ``project_dir``')
             path = os.path.join(project_dir,name,'fitting_progress.pdf')
         plt.savefig(path)  
     plt.show()
 
     
 def write_video_clip(frames, path, fps=30, quality=7):
-    """Write a video clip to a file.
+    """
+    Write a video clip to a file.
+
+    Parameters
+    ----------
+    frames : np.ndarray
+        Video frames as a 4D array of shape `(num_frames, height, width, 3)`
+        or a 3D array of shape `(num_frames, height, width)`.
+
+    path : str
+        Path to save the video clip.
+
+    fps : int, default=30
+        Framerate of video encoding.
+
+    quality : int, default=7
+        Quality of video encoding.
     """
     with imageio.get_writer(
         path, pixelformat='yuv420p', 
         fps=fps, quality=quality) as writer:
         for frame in frames: 
             writer.append_data(frame)
 
@@ -787,15 +809,15 @@
     overlap: tuple of float, default=(0.2,0)
         Amount of overlap between each trajectory plot as a tuple 
         with the format ``(x_overlap, y_overlap)``. The values should
         be between 0 and 1.
         
     return_rasters: bool, default=False
         Rasterize the matplotlib canvas after plotting each step of
-        the trajecory. This is used to generate an animated gif
+        the trajecory. This is used to generate an animated video/gif
         of the trajectory. 
 
     Returns
     -------
     fig : :py:class:`matplotlib.figure.Figure`
         Figure handle
 
@@ -876,15 +898,15 @@
     coordinates=None, results=None, output_dir=None, name=None, 
     project_dir=None, results_path=None, pre=5, post=15, 
     min_frequency=0.005, min_duration=3, use_reindexed=True, 
     use_estimated_coords=False, skeleton=[], bodyparts=None, 
     use_bodyparts=None, num_samples=40, keypoint_colormap='autumn',
     plot_options={}, sampling_options={'mode':'density'},
     padding={'left':0.1, 'right':0.1, 'top':0.2, 'bottom':0.2},
-    save_individually=True, save_gifs=True, fps=30, 
+    save_individually=True, save_gifs=True, save_mp4s=False, fps=30, 
     projection_planes=['xy','xz'], **kwargs):
     """
     Generate trajectory plots for a modeled dataset.
 
     Each trajectory plot shows a sequence of poses along the average
     trajectory through latent space associated with a given syllable.
     A separate figure (and gif, optionally) is saved for each syllable, 
@@ -993,15 +1015,18 @@
         as well as the title offset. 
 
     save_individually: bool, default=True
         If True, a separate figure is saved for each syllable (in
         addition to the grid figure).
         
     save_gifs: bool, default=True
-        Whether to save an animated gif of the trajectory plots. 
+        Whether to save an animated gif of the trajectory plots.
+        
+    save_mp4s: bool, default=False
+        Whether to save videos of the trajectory plots as .mp4 files
         
     fps: int, default=30
         Framerate of the videos from which keypoints were derived.
         Used to set the framerate of gifs when ``save_gif=True``.
         
     projection_planes: list (subset of ['xy', 'yz', 'xz']), default=['xy','xz']
         For 3D data, defines the 2D plane(s) on which to project keypoint 
@@ -1075,37 +1100,47 @@
         # individual plots
         if save_individually:
             desc = 'Generating trajectory plots'
             for title,X in tqdm.tqdm(zip(titles,Xs), desc=desc, total=len(titles)):
 
                 fig,ax,rasters = plot_trajectories(
                     [title], X[None], lims, edges=edges, 
-                    return_rasters=save_gifs, **plot_options)
+                    return_rasters=(save_gifs or save_mp4s),
+                    **plot_options)
 
                 plt.savefig(os.path.join(output_dir, f'{title}{suffix}.pdf'))
                 plt.close(fig=fig)
 
                 if save_gifs:
-                    gif_fps = len(rasters)/(pre+post)*fps
+                    use_fps = len(rasters)/(pre+post)*fps
                     path = os.path.join(output_dir, f'{title}{suffix}.gif')
-                    imageio.mimsave(path, rasters, fps=gif_fps)
+                    imageio.mimsave(path, rasters, fps=use_fps)
+                if save_mp4s:
+                    use_fps = len(rasters)/(pre+post)*fps
+                    path = os.path.join(output_dir, f'{title}{suffix}.mp4')
+                    write_video_clip(rasters, path, fps=use_fps)
+                    
 
         # grid plot
         fig,ax,rasters = plot_trajectories(
             titles, Xs, lims, edges=edges, 
-            return_rasters=save_gifs, **plot_options)
+            return_rasters=(save_gifs or save_mp4s),
+            **plot_options)
 
         plt.savefig(os.path.join(output_dir, f'all_trajectories{suffix}.pdf'))
         plt.show()
 
         if save_gifs:
-            gif_fps = len(rasters)/(pre+post)*fps
+            use_fps = len(rasters)/(pre+post)*fps
             path = os.path.join(output_dir, f'all_trajectories{suffix}.gif')
-            imageio.mimsave(path, rasters, fps=gif_fps)
-
+            imageio.mimsave(path, rasters, fps=use_fps)
+        if save_mp4s:
+            use_fps = len(rasters)/(pre+post)*fps
+            path = os.path.join(output_dir, f'all_trajectories{suffix}.mp4')
+            write_video_clip(rasters, path, fps=use_fps)
 
 
 
 def overlay_keypoints_on_image(
     image, coordinates, edges=[], keypoint_colormap='autumn',
     node_size=3, line_width=2, copy=False, opacity=1.0):
     """
@@ -1527,12 +1562,9 @@
         sampled_instances.items(), desc='Generating crowd movies'):
         
         frames = crowd_movie(
             instances, coordinates, pre=pre, post=post,
             edges=edges, lims=limits, plot_options=plot_options)
 
         path = os.path.join(output_dir, f'syllable{syllable}.mp4')
-        
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore')
-            write_video_clip(frames, path, fps=fps, quality=quality)
+        write_video_clip(frames, path, fps=fps, quality=quality)
```

### Comparing `keypoint-moseq-0.0.1/setup.py` & `keypoint-moseq-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='keypoint-moseq',
-    version='0.0.1',
+    version='0.0.2',
     author='Caleb Weinreb',
     author_email='calebsw@gmail.com',
     include_package_data=True,
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
@@ -24,11 +24,11 @@
         'imageio[ffmpeg]',
         'pyyaml',
         'vidio',
         'holoviews[recommended]',
         'bokeh',
         'pandas',
         'tables',
-        'jax-moseq==0.0.1',
+        'jax-moseq',
     ], 
     url='https://github.com/dattalab/keypoint-moseq'
 )
```

