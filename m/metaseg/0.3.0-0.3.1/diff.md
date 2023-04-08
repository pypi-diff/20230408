# Comparing `tmp/metaseg-0.3.0.tar.gz` & `tmp/metaseg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.3.0.tar", last modified: Sat Apr  8 09:47:23 2023, max compression
+gzip compressed data, was "metaseg-0.3.1.tar", last modified: Sat Apr  8 23:50:19 2023, max compression
```

## Comparing `metaseg-0.3.0.tar` & `metaseg-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 09:47:23.414956 metaseg-0.3.0/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.0/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.0/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1736 2023-04-08 09:47:23.414956 metaseg-0.3.0/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1462 2023-04-08 08:19:39.000000 metaseg-0.3.0/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 09:47:23.398289 metaseg-0.3.0/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-08 09:47:06.000000 metaseg-0.3.0/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4531 2023-04-08 09:47:17.000000 metaseg-0.3.0/metaseg/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.3.0/metaseg/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4281 2023-04-08 09:47:17.000000 metaseg-0.3.0/metaseg/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 09:47:23.408289 metaseg-0.3.0/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.0/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.0/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.0/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.0/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.0/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.0/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.0/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 09:47:23.414956 metaseg-0.3.0/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      197 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1257 2023-04-07 20:16:03.000000 metaseg-0.3.0/metaseg/utils/file.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.0/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 09:47:23.401623 metaseg-0.3.0/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1736 2023-04-08 09:47:23.000000 metaseg-0.3.0/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      696 2023-04-08 09:47:23.000000 metaseg-0.3.0/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-08 09:47:23.000000 metaseg-0.3.0/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-08 09:47:23.000000 metaseg-0.3.0/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-08 09:47:23.000000 metaseg-0.3.0/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.0/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.0/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-08 09:47:23.414956 metaseg-0.3.0/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.0/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.536091 metaseg-0.3.1/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.1/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.1/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1777 2023-04-08 23:50:19.536091 metaseg-0.3.1/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1503 2023-04-08 23:49:11.000000 metaseg-0.3.1/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.519424 metaseg-0.3.1/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-08 23:50:05.000000 metaseg-0.3.1/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.3.1/metaseg/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3686 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.526091 metaseg-0.3.1/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.1/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.1/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.1/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.1/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.1/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.1/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.1/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.532757 metaseg-0.3.1/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-08 23:50:14.000000 metaseg-0.3.1/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.1/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.522757 metaseg-0.3.1/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1777 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      730 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.1/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.1/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-08 23:50:19.539424 metaseg-0.3.1/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.1/setup.py
```

### Comparing `metaseg-0.3.0/LICENSE` & `metaseg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/PKG-INFO` & `metaseg-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -15,15 +15,15 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20MetaSeg%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 
 ### Installation
@@ -39,24 +39,26 @@
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=1000,
 )
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
 ( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) # For video autoseg_video = SegAutoMaskGenerator
-().save_video( source="video.mp4", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for automatic download model weights
+points_per_batch=64, min_area=0, ) # For video autoseg_video =
+SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
+points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
+- [x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for automatic download model weights
```

### Comparing `metaseg-0.3.0/README.md` & `metaseg-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20MetaSeg%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 
 ### Installation
@@ -27,24 +27,26 @@
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=1000,
 )
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
```

#### html2text {}

```diff
@@ -3,12 +3,12 @@
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
 ( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) # For video autoseg_video = SegAutoMaskGenerator
-().save_video( source="video.mp4", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for automatic download model weights
+points_per_batch=64, min_area=0, ) # For video autoseg_video =
+SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
+points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
+- [x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for automatic download model weights
```

### Comparing `metaseg-0.3.0/metaseg/app.py` & `metaseg-0.3.1/metaseg/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,32 @@
                             minimum=0,
                             maximum=64,
                             step=2,
                             value=64,
                             label="Points per Batch",
                         )
 
+                        seg_automask_image_min_area = gr.Number(
+                            value=0,
+                            label="Min Area",
+                        )
+
                 seg_automask_image_predict = gr.Button(value="Generator")
 
             with gr.Column():
                 output_image = gr.Image()
 
         seg_automask_image_predict.click(
             fn=SegAutoMaskGenerator().save_image,
             inputs=[
                 seg_automask_image_file,
                 seg_automask_image_model_type,
                 seg_automask_image_points_per_side,
                 seg_automask_image_points_per_batch,
+                seg_automask_image_min_area,
             ],
             outputs=[output_image],
         )
 
 
 def video_app():
     with gr.Blocks():
@@ -89,32 +95,26 @@
                         with gr.Row():
                             with gr.Column():
                                 seg_automask_video_min_area = gr.Number(
                                     value=1000,
                                     label="Min Area",
                                 )
 
-                                seg_automask_video_max_area = gr.Number(
-                                    value=10000,
-                                    label="Max Area",
-                                )
-
                 seg_automask_video_predict = gr.Button(value="Generator")
             with gr.Column():
                 output_video = gr.Video()
 
         seg_automask_video_predict.click(
             fn=SegAutoMaskGenerator().save_video,
             inputs=[
                 seg_automask_video_file,
                 seg_automask_video_model_type,
                 seg_automask_video_points_per_side,
                 seg_automask_video_points_per_batch,
                 seg_automask_video_min_area,
-                seg_automask_video_max_area,
             ],
             outputs=[output_video],
         )
 
 
 def metaseg_app():
     app = gr.Blocks()
```

### Comparing `metaseg-0.3.0/metaseg/automatic_mask_generator.py` & `metaseg-0.3.1/metaseg/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/build_sam.py` & `metaseg-0.3.1/metaseg/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/demo.py` & `metaseg-0.3.1/metaseg/demo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 import cv2
 import numpy as np
 import torch
 
 from metaseg import SamAutomaticMaskGenerator, sam_model_registry
-from metaseg.utils.file import download_model
+from metaseg.utils import download_model, load_image, load_video
 
 
 class SegAutoMaskGenerator:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
 
     def load_model(self, model_type):
         if self.model is None:
-            model_path = download_model(model_type)
-            model = sam_model_registry[model_type](checkpoint=model_path)
-            model.to(device=self.device)
-            self.model = model
+            self.model_path = download_model(model_type)
+            self.model = sam_model_registry[model_type](checkpoint=self.model_path)
+            self.model.to(device=self.device)
 
         return self.model
 
-    def load_image(self, image_path):
-        image = cv2.imread(image_path)
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        return image
-
-    def load_video(self, video_path):
-        cap = cv2.VideoCapture(video_path)
-        frame_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-        frame_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        fourcc = cv2.VideoWriter_fourcc(*"XVID")
-        fps = int(cap.get(cv2.CAP_PROP_FPS))
-        out = cv2.VideoWriter("output.mp4", fourcc, fps, (frame_width, frame_height))
-
-        return cap, out
-
-    def predict(self, frame, model_type, points_per_side, points_per_batch):
+    def predict(self, frame, model_type, points_per_side, points_per_batch, min_area):
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
-            model, points_per_side=points_per_side, points_per_batch=points_per_batch
+            model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
         )
+
         masks = mask_generator.generate(frame)
 
         return frame, masks
 
-    def save_image(self, source, model_type, points_per_side, points_per_batch):
-        read_image = self.load_image(source)
-        image, anns = self.predict(read_image, model_type, points_per_side, points_per_batch)
+    def save_image(self, source, model_type, points_per_side, points_per_batch, min_area):
+        read_image = load_image(source)
+        image, anns = self.predict(read_image, model_type, points_per_side, points_per_batch, min_area)
         if len(anns) == 0:
             return
 
         sorted_anns = sorted(anns, key=(lambda x: x["area"]), reverse=True)
         mask_image = np.zeros((anns[0]["segmentation"].shape[0], anns[0]["segmentation"].shape[1], 3), dtype=np.uint8)
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
         for i, ann in enumerate(sorted_anns):
@@ -66,43 +51,42 @@
             mask_image = cv2.add(mask_image, img)
 
         combined_mask = cv2.add(image, mask_image)
         cv2.imwrite("output.jpg", combined_mask)
 
         return "output.jpg"
 
-    def save_video(self, source, model_type, points_per_side, points_per_batch, min_area, max_area):
-        cap, out = self.load_video(source)
+    def save_video(self, source, model_type, points_per_side, points_per_batch, min_area):
+        cap, out = load_video(source)
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
         while True:
             ret, frame = cap.read()
             if not ret:
                 break
 
-            image, anns = self.predict(frame, model_type, points_per_side, points_per_batch)
+            image, anns = self.predict(frame, model_type, points_per_side, points_per_batch, min_area)
             if len(anns) == 0:
                 continue
 
             sorted_anns = sorted(anns, key=(lambda x: x["area"]), reverse=True)
             mask_image = np.zeros(
                 (anns[0]["segmentation"].shape[0], anns[0]["segmentation"].shape[1], 3), dtype=np.uint8
             )
 
             for i, ann in enumerate(sorted_anns):
-                if max_area > ann["area"] > min_area:
-                    m = ann["segmentation"]
-                    color = colors[i % 256]  # Her nesne için farklı bir renk kullan
-                    img = np.zeros((m.shape[0], m.shape[1], 3), dtype=np.uint8)
-                    img[:, :, 0] = color[0]
-                    img[:, :, 1] = color[1]
-                    img[:, :, 2] = color[2]
-                    img = cv2.bitwise_and(img, img, mask=m.astype(np.uint8))
-                    img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
-                    mask_image = cv2.add(mask_image, img)
+                m = ann["segmentation"]
+                color = colors[i % 256]  # Her nesne için farklı bir renk kullan
+                img = np.zeros((m.shape[0], m.shape[1], 3), dtype=np.uint8)
+                img[:, :, 0] = color[0]
+                img[:, :, 1] = color[1]
+                img[:, :, 2] = color[2]
+                img = cv2.bitwise_and(img, img, mask=m.astype(np.uint8))
+                img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
+                mask_image = cv2.add(mask_image, img)
 
             combined_mask = cv2.add(frame, mask_image)
             out.write(combined_mask)
 
         out.release()
         cap.release()
         cv2.destroyAllWindows()
```

### Comparing `metaseg-0.3.0/metaseg/modeling/common.py` & `metaseg-0.3.1/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/modeling/image_encoder.py` & `metaseg-0.3.1/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/modeling/mask_decoder.py` & `metaseg-0.3.1/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/modeling/prompt_encoder.py` & `metaseg-0.3.1/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/modeling/sam.py` & `metaseg-0.3.1/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/modeling/transformer.py` & `metaseg-0.3.1/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/predictor.py` & `metaseg-0.3.1/metaseg/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/utils/amg.py` & `metaseg-0.3.1/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/utils/file.py` & `metaseg-0.3.1/metaseg/utils/file_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,10 +23,7 @@
         print(f"{model_type} model has been successfully downloaded and saved as '{filename}'.")
     elif os.path.exists(filename):
         print(f"{model_type} model already exists as '{filename}'. Skipping download.")
     else:
         raise ValueError("Invalid model type. It should be 'vit_h', 'vit_l', or 'vit_b'.")
 
     return filename
-
-
-download_model("vit_b")
```

### Comparing `metaseg-0.3.0/metaseg/utils/onnx.py` & `metaseg-0.3.1/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg/utils/transforms.py` & `metaseg-0.3.1/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.0/metaseg.egg-info/PKG-INFO` & `metaseg-0.3.1/metaseg.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -15,15 +15,15 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20MetaSeg%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 
 ### Installation
@@ -39,24 +39,26 @@
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
     model_type="vit_l",
     points_per_side=16, 
-    points_per_batch=64
+    points_per_batch=64,
+    min_area=1000,
 )
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
 ( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) # For video autoseg_video = SegAutoMaskGenerator
-().save_video( source="video.mp4", model_type="vit_l", points_per_side=16,
-points_per_batch=64 ) ``` # Extra Features - [x] Support for video files - [x]
-Support for pip installation - [x] Support for web application - [x] Support
-for automatic download model weights
+points_per_batch=64, min_area=0, ) # For video autoseg_video =
+SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
+points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
+- [x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for automatic download model weights
```

### Comparing `metaseg-0.3.0/metaseg.egg-info/SOURCES.txt` & `metaseg-0.3.1/metaseg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 metaseg/modeling/image_encoder.py
 metaseg/modeling/mask_decoder.py
 metaseg/modeling/prompt_encoder.py
 metaseg/modeling/sam.py
 metaseg/modeling/transformer.py
 metaseg/utils/__init__.py
 metaseg/utils/amg.py
-metaseg/utils/file.py
+metaseg/utils/data_utils.py
+metaseg/utils/file_utils.py
 metaseg/utils/onnx.py
 metaseg/utils/transforms.py
```

### Comparing `metaseg-0.3.0/setup.py` & `metaseg-0.3.1/setup.py`

 * *Files identical despite different names*

