# Comparing `tmp/hordelib-0.1.0.tar.gz` & `tmp/hordelib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.1.0.tar", last modified: Thu Apr  6 15:07:48 2023, max compression
+gzip compressed data, was "hordelib-0.2.0.tar", last modified: Sat Apr  8 17:41:21 2023, max compression
```

## Comparing `hordelib-0.1.0.tar` & `hordelib-0.2.0.tar`

### file list

```diff
@@ -1,85 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.519635 hordelib-0.1.0/
--rw-rw-rw-   0        0        0      167 2023-04-03 21:13:26.000000 hordelib-0.1.0/.coveragerc
--rw-rw-rw-   0        0        0       88 2023-04-03 21:13:26.000000 hordelib-0.1.0/.flake8
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.461122 hordelib-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.476123 hordelib-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     2265 2023-04-06 13:01:44.000000 hordelib-0.1.0/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0      571 2023-04-03 21:13:26.000000 hordelib-0.1.0/.github/workflows/tests.yaml
--rw-rw-rw-   0        0        0     2128 2023-04-06 12:58:27.000000 hordelib-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     2962 2023-04-06 14:58:19.000000 hordelib-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35182 2023-04-05 20:05:31.000000 hordelib-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    46759 2023-04-06 15:07:48.518636 hordelib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5654 2023-04-06 14:52:46.000000 hordelib-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.481122 hordelib-0.1.0/hordelib/
--rw-rw-rw-   0        0        0       94 2023-04-06 13:01:50.000000 hordelib-0.1.0/hordelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.497125 hordelib-0.1.0/hordelib/cache/
--rw-rw-rw-   0        0        0       60 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/cache/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/cache/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.500635 hordelib-0.1.0/hordelib/clip/
--rw-rw-rw-   0        0        0      131 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/clip/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-04-04 18:26:09.000000 hordelib-0.1.0/hordelib/clip/bulk.py
--rw-rw-rw-   0        0        0     1088 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/clip/coca.py
--rw-rw-rw-   0        0        0     4627 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/clip/image.py
--rw-rw-rw-   0        0        0    11906 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/clip/interrogate.py
--rw-rw-rw-   0        0        0     2979 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/clip/text.py
--rw-rw-rw-   0        0        0     9164 2023-04-06 14:49:12.000000 hordelib-0.1.0/hordelib/comfy_horde.py
--rw-rw-rw-   0        0        0      525 2023-04-06 13:45:20.000000 hordelib-0.1.0/hordelib/config_path.py
--rw-rw-rw-   0        0        0      334 2023-04-06 14:51:30.000000 hordelib-0.1.0/hordelib/consts.py
--rw-rw-rw-   0        0        0     4029 2023-04-06 14:39:53.000000 hordelib-0.1.0/hordelib/horde.py
--rw-rw-rw-   0        0        0      574 2023-04-06 14:39:42.000000 hordelib-0.1.0/hordelib/initialisation.py
--rw-rw-rw-   0        0        0     2578 2023-04-06 12:55:51.000000 hordelib-0.1.0/hordelib/install_comfy.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.508635 hordelib-0.1.0/hordelib/model_manager/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/model_manager/__init__.py
--rw-rw-rw-   0        0        0     7757 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/aitemplate.py
--rw-rw-rw-   0        0        0    20755 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/base.py
--rw-rw-rw-   0        0        0     4132 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/blip.py
--rw-rw-rw-   0        0        0     6498 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/model_manager/clip.py
--rw-rw-rw-   0        0        0     3629 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/codeformer.py
--rw-rw-rw-   0        0        0     2199 2023-04-06 13:28:56.000000 hordelib-0.1.0/hordelib/model_manager/compvis.py
--rw-rw-rw-   0        0        0     5476 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/controlnet.py
--rw-rw-rw-   0        0        0     4656 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/model_manager/diffusers.py
--rw-rw-rw-   0        0        0     5163 2023-04-06 12:32:24.000000 hordelib-0.1.0/hordelib/model_manager/esrgan.py
--rw-rw-rw-   0        0        0     3213 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/gfpgan.py
--rw-rw-rw-   0        0        0    16218 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/hyper.py
--rw-rw-rw-   0        0        0     3317 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/new.py
--rw-rw-rw-   0        0        0     3490 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/model_manager/safety_checker.py
--rw-rw-rw-   0        0        0     8575 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/sdu.py
--rw-rw-rw-   0        0        0     6913 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/model_manager/torch_hijack.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.510636 hordelib-0.1.0/hordelib/nodes/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/nodes/__init__.py
--rw-rw-rw-   0        0        0     1413 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/nodes/node_clip_similarities.py
--rw-rw-rw-   0        0        0     1634 2023-04-06 14:10:46.000000 hordelib-0.1.0/hordelib/nodes/node_image_output.py
--rw-rw-rw-   0        0        0     1225 2023-04-06 14:00:19.000000 hordelib-0.1.0/hordelib/nodes/node_model_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.511634 hordelib-0.1.0/hordelib/pipeline_designs/
--rw-rw-rw-   0        0        0     6710 2023-04-03 21:25:36.000000 hordelib-0.1.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-rw-rw-   0        0        0     9464 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.512635 hordelib-0.1.0/hordelib/pipelines/
--rw-rw-rw-   0        0        0     2051 2023-04-03 21:28:04.000000 hordelib-0.1.0/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-rw-rw-   0        0        0     2869 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-rw-rw-   0        0        0     2573 2023-04-06 15:05:18.000000 hordelib-0.1.0/hordelib/run_comfyui.py
--rw-rw-rw-   0        0        0      505 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/settings.py
--rw-rw-rw-   0        0        0      930 2023-04-06 14:38:17.000000 hordelib-0.1.0/hordelib/shared_model_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.514637 hordelib-0.1.0/hordelib/utils/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/utils/__init__.py
--rw-rw-rw-   0        0        0      627 2023-04-03 21:13:26.000000 hordelib-0.1.0/hordelib/utils/cast.py
--rw-rw-rw-   0        0        0      218 2023-04-06 09:46:54.000000 hordelib-0.1.0/hordelib/utils/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.496126 hordelib-0.1.0/hordelib.egg-info/
--rw-rw-rw-   0        0        0    46759 2023-04-06 15:07:48.000000 hordelib-0.1.0/hordelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2023-04-06 15:07:48.000000 hordelib-0.1.0/hordelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 15:07:48.000000 hordelib-0.1.0/hordelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      225 2023-04-06 15:07:48.000000 hordelib-0.1.0/hordelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-06 15:07:48.000000 hordelib-0.1.0/hordelib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1659 2023-04-03 21:13:26.000000 hordelib-0.1.0/publish.py
--rw-rw-rw-   0        0        0     1318 2023-04-06 15:07:42.000000 hordelib-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       71 2023-04-03 21:13:26.000000 hordelib-0.1.0/pytest.ini
--rw-rw-rw-   0        0        0       28 2023-04-06 09:46:54.000000 hordelib-0.1.0/requirements.dev.txt
--rw-rw-rw-   0        0        0      348 2023-04-06 15:07:42.000000 hordelib-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 15:07:48.519635 hordelib-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 15:07:48.517637 hordelib-0.1.0/tests/
--rw-rw-rw-   0        0        0       40 2023-04-06 13:10:51.000000 hordelib-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     4157 2023-04-06 12:46:50.000000 hordelib-0.1.0/tests/test_comfy.py
--rw-rw-rw-   0        0        0     1550 2023-04-06 13:25:34.000000 hordelib-0.1.0/tests/test_comfy_install.py
--rw-rw-rw-   0        0        0     8676 2023-04-06 14:42:08.000000 hordelib-0.1.0/tests/test_horde.py
--rw-rw-rw-   0        0        0     4045 2023-04-06 14:40:46.000000 hordelib-0.1.0/tests/test_inference.py
--rw-rw-rw-   0        0        0      382 2023-04-06 12:47:28.000000 hordelib-0.1.0/tests/test_initialisation.py
--rw-rw-rw-   0        0        0      805 2023-04-06 15:01:58.000000 hordelib-0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.546485 hordelib-0.2.0/
+-rw-rw-rw-   0        0        0      158 2023-04-06 17:36:05.000000 hordelib-0.2.0/.coveragerc
+-rw-rw-rw-   0        0        0       88 2023-04-03 21:13:26.000000 hordelib-0.2.0/.flake8
+-rw-rw-rw-   0        0        0      162 2023-04-07 14:09:36.000000 hordelib-0.2.0/.git-blame-ignore-revs
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.464260 hordelib-0.2.0/.github/
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.475261 hordelib-0.2.0/.github/workflows/
+-rw-rw-rw-   0        0        0     2270 2023-04-06 23:34:51.000000 hordelib-0.2.0/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0      615 2023-04-08 16:55:32.000000 hordelib-0.2.0/.github/workflows/tests.yaml
+-rw-rw-rw-   0        0        0     2191 2023-04-08 16:59:24.000000 hordelib-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     3260 2023-04-08 17:26:58.000000 hordelib-0.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35182 2023-04-05 20:05:31.000000 hordelib-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    47456 2023-04-08 17:41:21.546485 hordelib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6314 2023-04-08 16:59:24.000000 hordelib-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1666 2023-04-06 23:36:10.000000 hordelib-0.2.0/build_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.482260 hordelib-0.2.0/hordelib/
+-rw-rw-rw-   0        0        0       94 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.507485 hordelib-0.2.0/hordelib/cache/
+-rw-rw-rw-   0        0        0       60 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/cache/__init__.py
+-rw-rw-rw-   0        0        0     8739 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/cache/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.511485 hordelib-0.2.0/hordelib/clip/
+-rw-rw-rw-   0        0        0      131 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/clip/__init__.py
+-rw-rw-rw-   0        0        0     2481 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/bulk.py
+-rw-rw-rw-   0        0        0     1088 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/clip/coca.py
+-rw-rw-rw-   0        0        0     4681 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/image.py
+-rw-rw-rw-   0        0        0    12260 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/interrogate.py
+-rw-rw-rw-   0        0        0     3034 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/text.py
+-rw-rw-rw-   0        0        0    12822 2023-04-08 10:08:14.000000 hordelib-0.2.0/hordelib/comfy_horde.py
+-rw-rw-rw-   0        0        0      527 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/config_path.py
+-rw-rw-rw-   0        0        0      569 2023-04-08 17:40:47.000000 hordelib-0.2.0/hordelib/consts.py
+-rw-rw-rw-   0        0        0     8631 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/horde.py
+-rw-rw-rw-   0        0        0      789 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/initialisation.py
+-rw-rw-rw-   0        0        0     3773 2023-04-07 17:27:13.000000 hordelib-0.2.0/hordelib/install_comfy.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.520484 hordelib-0.2.0/hordelib/model_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/model_manager/__init__.py
+-rw-rw-rw-   0        0        0     7823 2023-04-07 15:47:10.000000 hordelib-0.2.0/hordelib/model_manager/aitemplate.py
+-rw-rw-rw-   0        0        0    20616 2023-04-07 15:47:24.000000 hordelib-0.2.0/hordelib/model_manager/base.py
+-rw-rw-rw-   0        0        0     4195 2023-04-07 15:47:35.000000 hordelib-0.2.0/hordelib/model_manager/blip.py
+-rw-rw-rw-   0        0        0     6767 2023-04-07 15:47:41.000000 hordelib-0.2.0/hordelib/model_manager/clip.py
+-rw-rw-rw-   0        0        0     2858 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/model_manager/codeformer.py
+-rw-rw-rw-   0        0        0     2226 2023-04-07 15:47:53.000000 hordelib-0.2.0/hordelib/model_manager/compvis.py
+-rw-rw-rw-   0        0        0     5500 2023-04-07 15:47:57.000000 hordelib-0.2.0/hordelib/model_manager/controlnet.py
+-rw-rw-rw-   0        0        0     4719 2023-04-07 15:48:03.000000 hordelib-0.2.0/hordelib/model_manager/diffusers.py
+-rw-rw-rw-   0        0        0     2431 2023-04-07 15:48:06.000000 hordelib-0.2.0/hordelib/model_manager/esrgan.py
+-rw-rw-rw-   0        0        0     2409 2023-04-07 15:48:10.000000 hordelib-0.2.0/hordelib/model_manager/gfpgan.py
+-rw-rw-rw-   0        0        0    15731 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/model_manager/hyper.py
+-rw-rw-rw-   0        0        0     3380 2023-04-07 15:48:13.000000 hordelib-0.2.0/hordelib/model_manager/new.py
+-rw-rw-rw-   0        0        0     3553 2023-04-07 15:48:16.000000 hordelib-0.2.0/hordelib/model_manager/safety_checker.py
+-rw-rw-rw-   0        0        0     8699 2023-04-07 20:20:31.000000 hordelib-0.2.0/hordelib/model_manager/sdu.py
+-rw-rw-rw-   0        0        0     7282 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/model_manager/torch_hijack.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.524484 hordelib-0.2.0/hordelib/nodes/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/nodes/__init__.py
+-rw-rw-rw-   0        0        0     1449 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/nodes/node_clip_similarities.py
+-rw-rw-rw-   0        0        0      947 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/nodes/node_image_loader.py
+-rw-rw-rw-   0        0        0     1634 2023-04-06 14:10:46.000000 hordelib-0.2.0/hordelib/nodes/node_image_output.py
+-rw-rw-rw-   0        0        0     1244 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/nodes/node_model_loader.py
+-rw-rw-rw-   0        0        0     1065 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/nodes/node_upscale_model_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.527484 hordelib-0.2.0/hordelib/pipeline_designs/
+-rw-rw-rw-   0        0        0     2807 2023-04-07 08:03:23.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-rw-rw-   0        0        0     8264 2023-04-07 17:52:13.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-rw-rw-   0        0        0    11353 2023-04-07 19:35:03.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-rw-rw-   0        0        0     8478 2023-04-08 08:48:44.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.529483 hordelib-0.2.0/hordelib/pipelines/
+-rw-rw-rw-   0        0        0      802 2023-04-07 08:03:55.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_image_upscale.json
+-rw-rw-rw-   0        0        0     2470 2023-04-07 17:51:47.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-rw-rw-   0        0        0     3507 2023-04-07 19:08:34.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-rw-rw-   0        0        0     2561 2023-04-08 09:41:56.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-rw-rw-   0        0        0      473 2023-04-07 16:38:47.000000 hordelib-0.2.0/hordelib/run_comfyui.patch
+-rw-rw-rw-   0        0        0     1245 2023-04-07 17:27:31.000000 hordelib-0.2.0/hordelib/run_comfyui.py
+-rw-rw-rw-   0        0        0      717 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/safety_checker.py
+-rw-rw-rw-   0        0        0      505 2023-04-06 09:46:54.000000 hordelib-0.2.0/hordelib/settings.py
+-rw-rw-rw-   0        0        0      926 2023-04-07 10:32:48.000000 hordelib-0.2.0/hordelib/shared_model_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.530483 hordelib-0.2.0/hordelib/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/utils/__init__.py
+-rw-rw-rw-   0        0        0      655 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/utils/cast.py
+-rw-rw-rw-   0        0        0      218 2023-04-06 09:46:54.000000 hordelib-0.2.0/hordelib/utils/switch.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.506484 hordelib-0.2.0/hordelib.egg-info/
+-rw-rw-rw-   0        0        0    47456 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2662 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      225 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.533487 hordelib-0.2.0/images/
+-rw-rw-rw-   0        0        0    36815 2023-04-06 23:19:06.000000 hordelib-0.2.0/images/test_db0.jpg
+-rw-rw-rw-   0        0        0  1474994 2023-04-08 09:16:11.000000 hordelib-0.2.0/images/test_inpaint.png
+-rw-rw-rw-   0        0        0  1467500 2023-04-08 09:41:06.000000 hordelib-0.2.0/images/test_outpaint.png
+-rw-rw-rw-   0        0        0     2369 2023-04-08 17:41:15.000000 hordelib-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       71 2023-04-03 21:13:26.000000 hordelib-0.2.0/pytest.ini
+-rw-rw-rw-   0        0        0       73 2023-04-07 14:09:36.000000 hordelib-0.2.0/requirements.dev.txt
+-rw-rw-rw-   0        0        0      348 2023-04-08 17:41:15.000000 hordelib-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:41:21.546485 hordelib-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.545487 hordelib-0.2.0/tests/
+-rw-rw-rw-   0        0        0      180 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img.py
+-rw-rw-rw-   0        0        0     1107 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_hires.py
+-rw-rw-rw-   0        0        0     1136 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_inpaint.py
+-rw-rw-rw-   0        0        0     1181 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_outpaint.py
+-rw-rw-rw-   0        0        0     1016 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_txt2img.py
+-rw-rw-rw-   0        0        0     1021 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_txt2img_hires.py
+-rw-rw-rw-   0        0        0      930 2023-04-08 10:50:44.000000 hordelib-0.2.0/tests/run_upscale.py
+-rw-rw-rw-   0        0        0     1786 2023-04-08 09:21:29.000000 hordelib-0.2.0/tests/test_clip.py
+-rw-rw-rw-   0        0        0     5948 2023-04-08 10:19:21.000000 hordelib-0.2.0/tests/test_comfy.py
+-rw-rw-rw-   0        0        0     1550 2023-04-06 13:25:34.000000 hordelib-0.2.0/tests/test_comfy_install.py
+-rw-rw-rw-   0        0        0    12444 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/test_horde_inference.py
+-rw-rw-rw-   0        0        0     4410 2023-04-08 17:01:41.000000 hordelib-0.2.0/tests/test_horde_pp.py
+-rw-rw-rw-   0        0        0     6230 2023-04-07 15:57:33.000000 hordelib-0.2.0/tests/test_inference.py
+-rw-rw-rw-   0        0        0      382 2023-04-06 12:47:28.000000 hordelib-0.2.0/tests/test_initialisation.py
+-rw-rw-rw-   0        0        0     3328 2023-04-07 11:33:18.000000 hordelib-0.2.0/tests/test_model_manager.py
+-rw-rw-rw-   0        0        0     1587 2023-04-08 09:21:33.000000 hordelib-0.2.0/tests/test_safety_checker.py
+-rw-rw-rw-   0        0        0     1058 2023-04-07 14:09:36.000000 hordelib-0.2.0/tox.ini
```

### Comparing `hordelib-0.1.0/.github/workflows/pypi.yml` & `hordelib-0.2.0/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         python -m
         pip install
         build
         --user
     - name: "🔧 Build a binary wheel and a source tarball"
       if: ${{ steps.release.outputs.version != '' }}
       run: >-
-        python publish.py
+        python build_helper.py
     - name: "📦 Publish distribution to PyPI"
       if: ${{ steps.release.outputs.version != '' }}
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
     # TODO: Once we make it official
     # - name: "Inform with Discord Webhook"
```

### Comparing `hordelib-0.1.0/.gitignore` & `hordelib-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -136,11 +136,14 @@
 
 # Local
 test-image.png
 hordelib/ComfyUI
 ComfyUI
 model.ckpt
 coverage.lcov
-*.png
-comfy-prompt.json
+images/pip*.png
+images/test.png
+images/hor*.png
+images/hor*.webp
+comfy-prompt*.json
 
 .vscode
```

### Comparing `hordelib-0.1.0/CHANGELOG.md` & `hordelib-0.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 ﻿# Changelog
 
 Release history for `hordelib`.
 
+## v0.2.0 - 2023-04-08
+
+### Added
+- Horde hires_fix support.
+- Add upscaler support.
+- Add inpainting.
+- Add outpainting.
+
 ## v0.1.0 - 2023-04-06
 
 ### Added
 - Clip skip support.
 - Adds "tox -e comfyui" command to run comfyui web app.
 - Significant refactors and build changes.
+- Safety Checker
 
 ### Fixed
 - ComfyUI upgrades work correctly now.
 - Various fixes for Horde Worker integration.
 
 ## v0.0.10 - 2023-04-03
```

### Comparing `hordelib-0.1.0/LICENSE` & `hordelib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.1.0/PKG-INFO` & `hordelib-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
-Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>
+Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -728,15 +728,15 @@
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
-pil_image = generate.text_to_image(data)
+pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
 ## Development
 
 Requirements:
 - `git` (install git)
@@ -806,26 +806,35 @@
 The main config files for the project are: `pyproject.toml`, `tox.ini` and `requirements.txt`
 
 ### PyPi Publishing
 
 Three steps:
 1. Bump the version in `hordelib/cosnts.py`
 1. `tox` _make sure everything works_
-1. `python publish.py` _builds the dist files_
+1. `python build_helper.py` _builds the dist files_
 1. `twine upload -r pypi dist/*`
 
 ### Updating the embedded version of ComfyUI
 
 We use a ComfyUI version pinned to a specific commit, see `hordelib/consts.py:COMFYUI_VERSION`
 
 To test if the latest version works and upgrade to it, from the project root simply:
 
-1. `cd hordelib/Comfy` _Change CWD to the embedded comfy_
+1. `cd ComfyUI` _Change CWD to the embedded comfy_
 1. `git checkout master` _Switch to master branch_
 1. `git pull` _Get the latest comfyui code_
-1. `git rev-parse HEAD` _Print the commit hash we'll need this_
-1. `cd ../../` _Get back to the hordelib project root_
+1. `git rev-parse HEAD` _Update the hash in `hordelib.consts:COMFYUI_VERSION`_
+1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
-If everything still works. Take the commit hash printed above and put it in `hordelib/consts.py:COMFYUI_VERSION`
-
 Now ComfyUI is pinned to a new version.
+
+### ComfyUI Patching
+
+It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+
+To create a patch file:
+- Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
+
+Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
+
+Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.1.0/README.md` & `hordelib-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
-pil_image = generate.text_to_image(data)
+pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
 ## Development
 
 Requirements:
 - `git` (install git)
@@ -130,26 +130,35 @@
 The main config files for the project are: `pyproject.toml`, `tox.ini` and `requirements.txt`
 
 ### PyPi Publishing
 
 Three steps:
 1. Bump the version in `hordelib/cosnts.py`
 1. `tox` _make sure everything works_
-1. `python publish.py` _builds the dist files_
+1. `python build_helper.py` _builds the dist files_
 1. `twine upload -r pypi dist/*`
 
 ### Updating the embedded version of ComfyUI
 
 We use a ComfyUI version pinned to a specific commit, see `hordelib/consts.py:COMFYUI_VERSION`
 
 To test if the latest version works and upgrade to it, from the project root simply:
 
-1. `cd hordelib/Comfy` _Change CWD to the embedded comfy_
+1. `cd ComfyUI` _Change CWD to the embedded comfy_
 1. `git checkout master` _Switch to master branch_
 1. `git pull` _Get the latest comfyui code_
-1. `git rev-parse HEAD` _Print the commit hash we'll need this_
-1. `cd ../../` _Get back to the hordelib project root_
+1. `git rev-parse HEAD` _Update the hash in `hordelib.consts:COMFYUI_VERSION`_
+1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
-If everything still works. Take the commit hash printed above and put it in `hordelib/consts.py:COMFYUI_VERSION`
-
 Now ComfyUI is pinned to a new version.
+
+### ComfyUI Patching
+
+It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+
+To create a patch file:
+- Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
+
+Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
+
+Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.1.0/hordelib/cache/cache.py` & `hordelib-0.2.0/hordelib/cache/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     """The AI Horde Worker specific directory for caching."""
     AIWORKER_CACHE_HOME = os.environ.get("AIWORKER_CACHE_HOME")
     base_dir = ""
     if AIWORKER_CACHE_HOME:
         base_dir = AIWORKER_CACHE_HOME
     else:
         base_dir = os.environ.get(
-            "XDG_CACHE_HOME", os.path.join(Path.home(), ".cache/")
+            "XDG_CACHE_HOME",
+            os.path.join(Path.home(), ".cache/"),
         )
     return os.path.join(base_dir, "nataili")
 
 
 class Cache:
     def __init__(self, cache_name, cache_subname=None, cache_parentname=None):
         """
@@ -76,15 +77,16 @@
         List all files in a directory
         :param input_directory: Directory to list
         :param extensions: List of extensions to filter for
         :return: List of files
         """
         files = []
         for file in tqdm(
-            os.listdir(input_directory), disable=WorkerSettings.disable_progress.active
+            os.listdir(input_directory),
+            disable=WorkerSettings.disable_progress.active,
         ):
             if os.path.splitext(file)[1] in extensions:
                 files.append(os.path.splitext(file)[0])
         return files
 
     def get_all(self):
         """
@@ -159,41 +161,45 @@
         return pil_hashes, file_hashes
 
     def create_sqlite_db(self):
         """
         Create a sqlite database from the cache
         """
         self.cursor.execute(
-            "CREATE TABLE IF NOT EXISTS cache (file text, hash text, pil_hash text)"
+            "CREATE TABLE IF NOT EXISTS cache (file text, hash text, pil_hash text)",
         )
         self.cursor.execute("CREATE INDEX IF NOT EXISTS file_index ON cache (file)")
         self.cursor.execute("CREATE INDEX IF NOT EXISTS hash_index ON cache (hash)")
         self.cursor.execute(
-            "CREATE INDEX IF NOT EXISTS pil_hash_index ON cache (pil_hash)"
+            "CREATE INDEX IF NOT EXISTS pil_hash_index ON cache (pil_hash)",
         )
         self.conn.commit()
 
     def add_sqlite_row(self, file: str, hash: str, pil_hash: str, commit=True):
         """
         Add a row to the sqlite database
         """
         self.cursor.execute(
-            "INSERT INTO cache VALUES (?, ?, ?)", (file, hash, pil_hash)
+            "INSERT INTO cache VALUES (?, ?, ?)",
+            (file, hash, pil_hash),
         )
         if commit:
             self.conn.commit()
 
     def populate_sqlite_db(self, list_of_files: list):
         """
         Populate the sqlite database from the cache
         """
         # Populate sqlite database
         for file in list_of_files:
             self.add_sqlite_row(
-                file["file"], file["hash"], file["pil_hash"], commit=False
+                file["file"],
+                file["hash"],
+                file["pil_hash"],
+                commit=False,
             )
         self.conn.commit()
 
     def key_exists(self, key):
         """
         Check if a key exists in the cache
         """
@@ -211,15 +217,15 @@
         no_return=False,
     ):
         """
         Get a file from the cache
         """
         if not any([file, file_hash, pil_hash]):
             raise ValueError(
-                "At least one value must be provided to search the database"
+                "At least one value must be provided to search the database",
             )
         file = os.path.splitext(file)[0] if file else None
         query = "SELECT hash, pil_hash FROM cache WHERE "
         conditions = []
         values = []
         if file:
             conditions.append("file=?")
```

### Comparing `hordelib-0.1.0/hordelib/clip/bulk.py` & `hordelib-0.2.0/hordelib/clip/bulk.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,22 @@
         """
         :param model_name: Name of model to use
         :param input_directory: Directory to read input from
         """
         self.model_name = model_name
         self.model_manager = ClipModelManager()
         self.cache_image = Cache(
-            self.model_name, cache_parentname="embeds", cache_subname="image"
+            self.model_name,
+            cache_parentname="embeds",
+            cache_subname="image",
         )
         self.model_manager.load(self.model_name)
         self.image_embed = ImageEmbed(
-            self.model_manager.loaded_models[self.model_name], self.cache_image
+            self.model_manager.loaded_models[self.model_name],
+            self.cache_image,
         )
         self._prepare_from_directory(input_directory=input_directory)
 
     def insert(self, image, input_directory):
         pil_image = Image.open(f"{input_directory}/{image}.webp").convert("RGB")
         pil_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         # hash = hashlib.sha256(open(f"{input_directory}/{image}.webp", "rb").read()).hexdigest()
@@ -54,10 +57,11 @@
         """
         logger.info(f"Reading from {input_directory}")
         directory_list = self.cache_image.list_dir(input_directory)
         logger.info(f"Found {len(directory_list)} files. Filtering...")
         filtered_list = self.cache_image.filter_list(directory_list)
         logger.info(f"Found {len(filtered_list)} files to embed.")
         for image in tqdm(
-            filtered_list, disable=WorkerSettings.disable_progress.active
+            filtered_list,
+            disable=WorkerSettings.disable_progress.active,
         ):
             self.insert(image, input_directory)
```

### Comparing `hordelib-0.1.0/hordelib/clip/coca.py` & `hordelib-0.2.0/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.1.0/hordelib/clip/image.py` & `hordelib-0.2.0/hordelib/clip/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,66 +5,69 @@
 import threading
 import time
 from concurrent.futures import ThreadPoolExecutor
 from uuid import uuid4
 
 import numpy as np
 import torch
+from loguru import logger
 from PIL import Image
 
 from hordelib.cache import Cache
 from hordelib.utils.cast import autocast_cuda
-from loguru import logger
 
 
 class ImageEmbed:
     def __init__(self, model, cache: Cache):
         """
         :param model: Loaded model from ModelManager
         :param cache: Cache object
         """
         self.model = model
         self.cache = cache
         self.executor = ThreadPoolExecutor(
-            max_workers=1024, thread_name_prefix="SaveThread"
+            max_workers=1024,
+            thread_name_prefix="SaveThread",
         )
 
     @autocast_cuda
     def _batch(self, pil_images: list):
         # logger.info(pil_images)
         for pil_image in pil_images:
             # logger.info(pil_image)
             pil_image["hash"] = hashlib.sha256(
-                pil_image["pil_image"].tobytes()
+                pil_image["pil_image"].tobytes(),
             ).hexdigest()
         preprocess_images = []
         to_remove = []
         with torch.no_grad():
             for pil_image in pil_images:
                 try:
                     preprocess_images.append(
                         self.model["preprocess"](pil_image["pil_image"])
                         .unsqueeze(0)
-                        .to(self.model["device"])
+                        .to(self.model["device"]),
                     )
                 except RuntimeError as e:
                     logger.error(e)
                     logger.error(pil_image)
                     to_remove.append(pil_image)
                     continue
             for pil_image in to_remove:
                 pil_images.remove(pil_image)
             assert len(preprocess_images) == len(pil_images)
             if len(preprocess_images) == 0:
                 return
             preprocess_images = torch.cat(preprocess_images, dim=0)
             image_features = self.model["model"].encode_image(preprocess_images)
             for image_embed_array, pil_image in zip(image_features, pil_images):
-                future = self.executor.submit(
-                    self._save, image_embed_array, pil_image["hash"]
+                self.executor.submit(
+                    self._save,
+                    image_embed_array,
+                    pil_image["hash"],
                 )
                 self.cache.add_sqlite_row(
                     file=pil_image["filename"].replace(".webp", ""),
                     pil_hash=pil_image["hash"],
                     hash=None,
                 )
 
@@ -89,21 +92,22 @@
         If image is not in cache, embed it and save it to cache
         Returns SHA256 hash of image
         """
         if image is None and filename is None:
             raise ValueError("Either image or filename must be set")
         if image is not None and filename is not None:
             raise ValueError("Only one of image or filename must be set")
-        if image is None:
-            pil_image = Image.open(f"{directory}/{filename}").convert("RGB")
-        else:
-            pil_image = image
+        pil_image = (
+            Image.open(f"{directory}/{filename}").convert("RGB")
+            if image is None
+            else image
+        )
         if image is None:
             file_hash = hashlib.sha256(
-                open(f"{directory}/{filename}", "rb").read()
+                open(f"{directory}/{filename}", "rb").read(),
             ).hexdigest()
             image_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         else:
             file_hash = None
             image_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         if not skip_cache:
             cached = self.cache.get(pil_hash=image_hash)
```

### Comparing `hordelib-0.1.0/hordelib/clip/interrogate.py` & `hordelib-0.2.0/hordelib/clip/interrogate.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,22 @@
         :param model: Loaded model from ModelManager
         For each data list in model["data_lists"], check if all items are cached.
         If not, embed all items and save to cache.
         If yes, load all text embeds from cache.
         """
         self.model = model
         self.cache = Cache(
-            self.model["cache_name"], cache_parentname="embeds", cache_subname="text"
+            self.model["cache_name"],
+            cache_parentname="embeds",
+            cache_subname="text",
         )
         self.cache_image = Cache(
-            self.model["cache_name"], cache_parentname="embeds", cache_subname="image"
+            self.model["cache_name"],
+            cache_parentname="embeds",
+            cache_subname="image",
         )
         self.embed_lists = {}
 
     def load(
         self,
         key: str,
         text_array: List[str],
@@ -62,28 +66,28 @@
         logger.debug(f"Loading {key} embeds")
         if individual:
             self.embed_lists[key] = {}
             for text in text_array:
                 text_hash = hashlib.sha256(text.encode("utf-8")).hexdigest()
                 filename = f"{self.cache.cache_dir}/{text_hash}.npy"
                 logger.debug(
-                    f"text: {text}, text_hash: {text_hash}, filename: {filename}"
+                    f"text: {text}, text_hash: {text_hash}, filename: {filename}",
                 )
                 embed = torch.from_numpy(np.load(filename)).float().to(device)
                 if len(embed.shape) == 1:
                     embed = embed.view(1, -1)
                 self.embed_lists[key][text] = embed
         else:
             with torch.no_grad():
                 text_features = []
                 for text in text_array:
                     text_hash = hashlib.sha256(text.encode("utf-8")).hexdigest()
                     filename = f"{self.cache.cache_dir}/{text_hash}.npy"
                     logger.debug(
-                        f"text: {text}, text_hash: {text_hash}, filename: {filename}"
+                        f"text: {text}, text_hash: {text_hash}, filename: {filename}",
                     )
                     embed = torch.from_numpy(np.load(filename)).float().to(device)
                     if len(embed.shape) == 1:
                         embed = embed.view(1, -1)
                     text_features.append(embed)
                 text_features = torch.cat(text_features, dim=0)
             text_features /= text_features.norm(dim=-1, keepdim=True)
@@ -146,22 +150,24 @@
             logger.debug(f"Loading {key} embeds")
             self.load(key, text_array, individual=True, device=device)
         logger.debug(f"{len(text_array)} text_array: {text_array}")
         similarity = {}
         for text in text_array:
             text_features = self.embed_lists[key][text].to(device)
             similarity[text] = round(
-                self._similarity(image_features, text_features)[0][0].item(), 4
+                self._similarity(image_features, text_features)[0][0].item(),
+                4,
             )
-        return {
-            k: v
-            for k, v in sorted(
-                similarity.items(), key=lambda item: item[1], reverse=True
-            )
-        }
+        return dict(
+            sorted(
+                similarity.items(),
+                key=lambda item: item[1],
+                reverse=True,
+            ),
+        )
 
     def rank(self, image_features, text_array, key, device, top_count=2):
         """
         Ranks the text_array by similarity to the image.
         The top results are the most similar to the image out of the text_array.
         The bottom results are the least similar to the image out of the text_array.
         The results are relative to each other, not absolute.
@@ -238,38 +244,52 @@
         image_hash = image_embed(image, filename, directory)
         image_embed_array = np.load(f"{self.cache_image.cache_dir}/{image_hash}.npy")
         image_features = (
             torch.from_numpy(image_embed_array).float().to(self.model["device"])
         )
         if similarity and not rank:
             results = {}
-            for k in text_array.keys():
+            for k in text_array:
                 results[k] = self.similarity(
-                    image_features, text_array[k], k, self.model["device"]
+                    image_features,
+                    text_array[k],
+                    k,
+                    self.model["device"],
                 )
                 logger.debug(f"{k}: {results[k]}")
             return results
         elif rank and not similarity:
             results = {}
-            for k in text_array.keys():
+            for k in text_array:
                 results[k] = self.rank(
-                    image_features, text_array[k], k, self.model["device"], top_count
+                    image_features,
+                    text_array[k],
+                    k,
+                    self.model["device"],
+                    top_count,
                 )
                 logger.debug(f"{k}: {results[k]}")
             return results
         else:
             similarity = {}
-            for k in text_array.keys():
+            for k in text_array:
                 similarity[k] = self.similarity(
-                    image_features, text_array[k], k, self.model["device"]
+                    image_features,
+                    text_array[k],
+                    k,
+                    self.model["device"],
                 )
                 logger.debug(f"{k}: {similarity[k]}")
             rank = {}
-            for k in text_array.keys():
+            for k in text_array:
                 rank[k] = self.rank(
-                    image_features, text_array[k], k, self.model["device"], top_count
+                    image_features,
+                    text_array[k],
+                    k,
+                    self.model["device"],
+                    top_count,
                 )
                 logger.debug(f"{k}: {rank[k]}")
             return {
                 "similarity": similarity,
                 "rank": rank,
             }
```

### Comparing `hordelib-0.1.0/hordelib/clip/text.py` & `hordelib-0.2.0/hordelib/clip/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import hashlib
 from concurrent.futures import ThreadPoolExecutor
 
 import clip
 import numpy as np
 import torch
+from loguru import logger
 
 from hordelib.cache import Cache
 from hordelib.utils.cast import autocast_cuda
-from loguru import logger
 
 
 class TextEmbed:
     def __init__(self, model, cache: Cache):
         """
         :param model: Loaded model from ModelManager
         :param cache: Cache object
         """
         self.model = model
         self.cache = cache
         self.executor = ThreadPoolExecutor(
-            max_workers=1024, thread_name_prefix="SaveThread"
+            max_workers=1024,
+            thread_name_prefix="SaveThread",
         )
 
     @autocast_cuda
     def _batch(self, text_list: list):
         for text in text_list:
             if isinstance(text["prompt"], bytes):
                 text["prompt"] = text["prompt"].decode("utf-8")
@@ -32,15 +33,15 @@
             clip.tokenize(text["prompt"], truncate=True).to(self.model["device"])
             for text in text_list
         ]
         text_tokens = torch.cat(text_tokens, dim=0)
         with torch.no_grad():
             text_features = self.model["model"].encode_text(text_tokens).float()
         for text_embed_array, text in zip(text_features, text_list):
-            future = self.executor.submit(self._save, text_embed_array, text["hash"])
+            self.executor.submit(self._save, text_embed_array, text["hash"])
             self.cache.add_sqlite_row(text["filename"], text["hash"], text["hash"])
 
     def _save(self, text_embed_array, text_hash):
         text_embed_array /= text_embed_array.norm(dim=-1, keepdim=True)
         np.save(
             f"{self.cache.cache_dir}/{text_hash}",
             text_embed_array.float().cpu().detach().numpy(),
@@ -65,10 +66,12 @@
         with torch.no_grad():
             text_features = self.model["model"].encode_text(text_tokens).float()
         text_features /= text_features.norm(dim=-1, keepdim=True)
         text_embed_array = text_features.cpu().detach().numpy()
         if filename:
             np.save(f"{self.cache.cache_dir}/{text_hash}", text_embed_array)
             self.cache.add_sqlite_row(filename, text_hash, text_hash)
+            return None
         else:
             np.save(f"{self.cache.cache_dir}/{text_hash}", text_embed_array)
             self.cache.add_sqlite_row(text, text_hash, text_hash)
+            return None
```

### Comparing `hordelib-0.1.0/hordelib/comfy_horde.py` & `hordelib-0.2.0/hordelib/comfy_horde.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,42 +6,54 @@
 import os
 import re
 from io import BytesIO
 
 from loguru import logger
 from PIL import Image
 
+from hordelib.config_path import get_comfyui_path
+
 # Do not change the order of these imports
 # fmt: off
 import execution
 from comfy.sd import load_checkpoint_guess_config
+from comfy.utils import load_torch_file
+from comfy_extras.chainner_models import model_loading
 # fmt: on
 
+
 class Comfy_Horde:
     """Handles horde-specific behavior against ComfyUI."""
 
-    # Lookup of ComfyUI standard nodes to hordelib custom nodes
+    # We save pipelines from the ComfyUI GUI. This is very convenient as it
+    # makes it super easy to load and edit them in the future. However standard
+    # ComfyUI's GUI doesn't know about our custom nodes, so we allow the pipeline
+    # design with standard nodes, then at runtime we dynamically replace these
+    # node types with our own where we need to.
     NODE_REPLACEMENTS = {
         "CheckpointLoaderSimple": "HordeCheckpointLoader",
+        "UpscaleModelLoader": "HordeUpscaleModelLoader",
         "SaveImage": "HordeImageOutput",
+        "LoadImage": "HordeImageLoader",
+    }
+
+    # We may wish some ComfyUI standard nodes had different names for consistency. Here
+    # we can dynamically rename some node input parameter names.
+    NODE_PARAMETER_REPLACEMENTS = {
+        "HordeCheckpointLoader": {
+            # We name this "model_name" as then we can use the same generic code in our model loaders
+            "ckpt_name": "model_name"
+        }
     }
 
     def __init__(self) -> None:
+        self.client_id = None  # used for receiving comfyUI async events
         self.pipelines = {}
         self.unit_testing = os.getenv("HORDELIB_TESTING", "")
 
-        # XXX Temporary hack for model dir
-        model_dir = os.getenv("AIWORKER_CACHE_HOME", "")
-        if not model_dir:
-            os.environ["HORDE_MODEL_DIR_CHECKPOINTS"] = self._this_dir("../")
-        else:
-            os.environ["HORDE_MODEL_DIR_CHECKPOINTS"] = os.path.join(
-                model_dir, "nataili", "compvis"
-            )
-
         # Load our pipelines
         self._load_pipelines()
 
     def _this_dir(self, filename: str, subdir="") -> str:
         target_dir = os.path.dirname(os.path.realpath(__file__))
         if subdir:
             target_dir = os.path.join(target_dir, subdir)
@@ -52,27 +64,59 @@
             execution.nodes.load_custom_node(self._this_dir(filename, subdir="nodes"))
         except Exception:
             logger.error(f"Failed to load custom pipeline node: {filename}")
             return
         logger.debug(f"Loaded custom pipeline node: {filename}")
 
     def _load_custom_nodes(self) -> None:
+        # Load standard nodes stored in odd locations first
+        self._load_extra_nodes()
+        # Now load our own nodes
         files = glob.glob(self._this_dir("node_*.py", subdir="nodes"))
         for file in files:
             self._load_node(os.path.basename(file))
 
+    def _load_comfy_node(self, filename: str) -> None:
+        try:
+            pathname = os.path.join(get_comfyui_path(), "comfy_extras", filename)
+            execution.nodes.load_custom_node(pathname)
+        except Exception:
+            logger.error(f"Failed to load comfy extra node: {filename}")
+            return
+        logger.debug(f"Loaded comfy extra node: {filename}")
+
+    # Load the comfy nodes that comfy stores in a different location from it's other nodes...
+    def _load_extra_nodes(self) -> None:
+        self._load_comfy_node("nodes_upscale_model.py")
+
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
         for nodename, node in data.items():
             if ("class_type" in node) and (
                 node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS
             ):
+                logger.debug(
+                    f"Changed type {data[nodename]['class_type']} to {Comfy_Horde.NODE_REPLACEMENTS[node['class_type']]}",
+                )
                 data[nodename]["class_type"] = Comfy_Horde.NODE_REPLACEMENTS[
                     node["class_type"]
                 ]
+        # Now we've fixed up node types, check for any node input parameter rename needed
+        for nodename, node in data.items():
+            if ("class_type" in node) and (
+                node["class_type"] in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS
+            ):
+                for oldname, newname in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS[
+                    node["class_type"]
+                ].items():
+                    if "inputs" in node and oldname in node["inputs"]:
+                        node["inputs"][newname] = node["inputs"][oldname]
+                        del node["inputs"][oldname]
+                logger.debug(f"Renamed node input {nodename}.{oldname} to {newname}")
+
         return data
 
     def _fix_node_names(self, data: dict, design: dict) -> dict:
         # We have a list of nodes, attempt to rename them to the "title" set
         # in the design file. These must be unique names.
         newnodes = {}
         renames = {}
@@ -85,17 +129,16 @@
                     break
             renames[nodename] = newname
             newnodes[newname] = oldnode
         # Now we've renamed the node names, change any references to them also
         for node in newnodes.values():
             if "inputs" in node:
                 for _, input in node["inputs"].items():
-                    if type(input) is list:
-                        if input and input[0] in renames:
-                            input[0] = renames[input[0]]
+                    if type(input) is list and input and input[0] in renames:
+                        input[0] = renames[input[0]]
         return newnodes
 
     # We are passed a valid comfy pipeline and a design file from the comfyui web app.
     # Why?
     #
     # 1. We replace some nodes with our own hordelib nodes, for example "CheckpointLoaderSimple"
     #    with "HordeCheckpointLoader".
@@ -169,49 +212,83 @@
                     logger.error(f"Attempt to set unknown pipeline parameter {key}")
                     break
 
                 current = current[k]
 
             current[keys[-1]] = value
 
+    # Connect the named input to the named node (output).
+    # Used for dynamic switching of pipeline graphs
+    @classmethod
+    def reconnect_input(cls, dct, input, output):
+        logger.debug(f"Request to reconnect input {input} to output {output}")
+        keys = input.split(".")
+        if "inputs" not in keys:
+            keys.insert(1, "inputs")
+        current = dct
+        for k in keys:
+            if k not in current:
+                logger.error(f"Attempt to reconnect unknown input {input}")
+                return None
+
+            current = current[k]
+
+        current[0] = output
+        return True
+
+    # This is the callback handler for comfy async events. We only use it for debugging.
+    def send_sync(self, p1, p2, p3):
+        logger.debug(f"{p1}, {p2}, {p3}")
+
     # Execute the named pipeline and pass the pipeline the parameter provided.
     # For the horde we assume the pipeline returns an array of images.
     def run_pipeline(self, pipeline_name: str, params: dict) -> dict | None:
         # Sanity
         if pipeline_name not in self.pipelines:
             logger.error(f"Unknown inference pipeline: {pipeline_name}")
             return None
 
+        logger.info(f"Running pipeline {pipeline_name}")
+
         # Grab a copy of the pipeline
         pipeline = copy.copy(self.pipelines[pipeline_name])
 
         # Inject our model manager if required
         from hordelib.shared_model_manager import SharedModelManager
+
         if "model_loader.model_manager" not in params:
+            logger.debug("Injecting model manager")
             params["model_loader.model_manager"] = SharedModelManager
 
+        # If we have a source image, use that rather than noise (i.e. img2img)
+        # XXX This probably shouldn't be here. But for the moment, it works.
+        if "image_loader.image" in params:
+            self.reconnect_input(pipeline, "sampler.latent_image", "vae_encode")
+
         # Set the pipeline parameters
         self._set(pipeline, **params)
 
         # Fake it!
         if self.unit_testing:
             img = Image.new("RGB", (64, 64), (0, 0, 0))
             byte_stream = BytesIO()
             img.save(byte_stream, format="PNG", compress_level=4)
             byte_stream.seek(0)
 
             return {
-                "output_image": {"images": [{"imagedata": byte_stream, "type": "PNG"}]}
+                "output_image": {"images": [{"imagedata": byte_stream, "type": "PNG"}]},
             }
 
         # Run it!
         inference = execution.PromptExecutor(self)
         # Load our custom nodes
         self._load_custom_nodes()
-        inference.execute(pipeline)
+        # The client_id parameter here is just so we receive comfy callbacks for debugging.
+        # We essential pretend we are a web client and want async callbacks.
+        inference.execute(pipeline, extra_data={"client_id": 1})
 
         return inference.outputs
 
     # Run a pipeline that returns an image in pixel space
     def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
         # is always in a HordeImageOutput node named "output_image". This is an array of
```

### Comparing `hordelib-0.1.0/hordelib/config_path.py` & `hordelib-0.2.0/hordelib/config_path.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 def get_comfyui_path():
     """Returns the path to ComfyUI that hordelib installs and manages."""
     return os.path.join(os.path.dirname(get_hordelib_path()), "ComfyUI")
 
 
 def set_system_path():
     """Adds ComfyUI to the python path, as it is not a proper library."""
-    sys.path.append(get_comfyui_path())
+    sys.path.append(get_comfyui_path())
```

### Comparing `hordelib-0.1.0/hordelib/install_comfy.py` & `hordelib-0.2.0/hordelib/install_comfy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # install.py
 # Fetch a specific version of the upstream ComfyUI project
 import os
 import subprocess
 
 from loguru import logger
-from hordelib.config_path import get_hordelib_path, get_comfyui_path
+
+from hordelib.config_path import get_comfyui_path, get_hordelib_path
 
 
 class Installer:
     """Handles the installation of ComfyUI."""
 
     @classmethod
     def get_commit_hash(cls) -> str:
@@ -28,46 +29,80 @@
                 commit_hash = f.read().strip()
 
             return commit_hash
         except Exception:
             return ""
 
     @classmethod
+    def _run_get_result(cls, command, directory=get_hordelib_path()):
+        result = subprocess.run(
+            command,
+            shell=True,
+            text=True,
+            capture_output=True,
+            cwd=directory,
+        )
+        return result
+
+    @classmethod
     def _run(cls, command, directory=get_hordelib_path()) -> tuple[bool, str] | None:
         try:
-            result = subprocess.run(
-                command, shell=True, text=True, capture_output=True, cwd=directory
-            )
+            result = cls._run_get_result(command, directory)
         except Exception as Ex:
             logger.error(Ex)
             return None
         if result.returncode:
             logger.error(result.stderr)
             return None
         return (True, result.stdout)
 
     @classmethod
     def install(cls, comfy_version: str) -> None:
         # Install if ComfyUI is missing completely
         if not os.path.exists(get_comfyui_path()):
             installdir = os.path.dirname(get_comfyui_path())
-            cls._run("git clone https://github.com/comfyanonymous/ComfyUI.git", installdir)
+            cls._run(
+                "git clone https://github.com/comfyanonymous/ComfyUI.git",
+                installdir,
+            )
             cls._run(f"git checkout {comfy_version}", get_comfyui_path())
             return
 
         # If it's installed, is it up to date?
         version = cls.get_commit_hash()
         if version == comfy_version:
             # Yes, all done
             return
 
         # Update comfyui
         logger.info(
-            f"Current ComfyUI version {version[:8]} requires {comfy_version[:8]}"
+            f"Current ComfyUI version {version[:8]} requires {comfy_version[:8]}",
         )
         # Try hard to ensure we reset everything even if we have been
         # hacking on ComfyUI or are in a weird repo state
         cls._run("git reset --hard", get_comfyui_path())
         cls._run("git clean -fd", get_comfyui_path())
         cls._run("git checkout master", get_comfyui_path())
         cls._run("git pull", get_comfyui_path())
         cls._run(f"git checkout {comfy_version}", get_comfyui_path())
+
+    @classmethod
+    def apply_patch(cls, patchfile):
+        # Check if the patch has already been applied
+        result = cls._run_get_result(
+            f"git apply --check {patchfile}", get_comfyui_path()
+        )
+        could_apply = not result.returncode
+        result = cls._run_get_result(
+            f"git apply --reverse --check {patchfile}", get_comfyui_path()
+        )
+        could_reverse = not result.returncode
+        if could_apply:
+            # Apply the patch
+            logger.debug(f"Applying patch {patchfile}")
+            cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
+        elif could_reverse:
+            # Patch is already applied, all is well
+            logger.debug(f"Already applied patch {patchfile}")
+        else:
+            # Couldn't apply or reverse? That's not so good
+            logger.error(f"Could not apply patch {patchfile}")
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/aitemplate.py` & `hordelib-0.2.0/hordelib/model_manager/aitemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 import torch
 from diffusers import LMSDiscreteScheduler
 from loguru import logger
 from transformers import CLIPFeatureExtractor, CLIPTokenizer
 
 # from nataili.aitemplate import StableDiffusionAITPipeline
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 # from nataili.util.voodoo import init_ait_module
 
 
 class AITemplateModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{get_cache_directory()}/aitemplate"
         self.models_db_name = "aitemplate"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.ait_workdir = None
         self.init()
 
     def init(self):
         if self.cuda_available:
             logger.info(
-                f"Highest CUDA Compute Capability: {self.cuda_devices[0]['sm']}"
+                f"Highest CUDA Compute Capability: {self.cuda_devices[0]['sm']}",
             )
             logger.debug(f"Available CUDA Devices: {self.cuda_devices}")
             logger.info(f"Recommended GPU: {self.recommended_gpu}")
             sm = self.recommended_gpu[0]["sm"]
             logger.info(f"Using sm_{sm} for AITemplate")
             for aitemplate in self.models:
                 ait_files = self.get_aitemplate_files(sm)
@@ -120,33 +121,37 @@
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if len(self.available_models) == 0:
             logger.info("No available aitemplates")
             sm = self.recommended_gpu[0]["sm"]
             logger.info(
-                f"Downloading AITemplate for {sm}", status="Downloading"
+                f"Downloading AITemplate for {sm}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_ait()
             logger.info(
-                f"AITemplate for {sm} downloaded", status="Downloading"
+                f"AITemplate for {sm} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
             self.loaded_models["ait"] = self.load_aitemplate(
                 model_name,
                 gpu_id=gpu_id,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
 
     def load_aitemplate(
         self,
         model_name,
         gpu_id=0,
     ):
         model_path = self.get_model_files(model_name)[0]["path"]
@@ -162,19 +167,19 @@
         ait["pipe"] = StableDiffusionAITPipeline(
             # XXX # FIXME (StableDiffusionAITPipeline missing)
             vae=None,
             unet=None,
             text_encoder=None,
             tokenizer=CLIPTokenizer.from_pretrained("openai/clip-vit-large-patch14"),
             scheduler=LMSDiscreteScheduler.from_pretrained(
-                "runwayml/stable-diffusion-v1-5"
+                "runwayml/stable-diffusion-v1-5",
             ),
             safety_checker=None,
             feature_extractor=CLIPFeatureExtractor.from_pretrained(
-                "openai/clip-vit-large-patch14"
+                "openai/clip-vit-large-patch14",
             ),
             clip_ait_exe=self.loaded_models["ait"]["clip"],
             unet_ait_exe=self.loaded_models["ait"]["unet"],
             vae_ait_exe=self.loaded_models["ait"]["vae"],
             filter_nsfw=False,
         ).to("cuda")
         return ait
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/base.py` & `hordelib-0.2.0/hordelib/model_manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import requests
 import torch
 from loguru import logger
 from tqdm import tqdm
 from transformers import logging
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 
 # from nataili import disable_download_progress
 from hordelib.settings import WorkerSettings
 
 if sys.version_info < (3, 9):
     import importlib_resources
 else:
@@ -34,15 +35,15 @@
         self.loaded_models = {}
         self.tainted_models = []
         self.pkg = importlib_resources.files("hordelib")
         self.models_db_name = "models"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
         self.cuda_available = torch.cuda.is_available()
         self.cuda_devices, self.recommended_gpu = self.get_cuda_devices()
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.download_reference = download_reference
 
     def init(self, list_models=False):
         if self.download_reference:
             self.models = self.download_model_reference()
             logger.info(f"Downloaded model reference. Got {len(self.models)} models.")
         else:
@@ -66,15 +67,16 @@
             logger.info("Model Reference", status="Downloading")  # logger.init
             response = requests.get(self.remote_db)
             logger.info("Model Reference", status="OK")  # logger.init_ok
             models = response.json()
             return models
         except Exception as e:
             logger.info_err(
-                "Model Reference", status=f"Download failed: {e}"
+                "Model Reference",
+                status=f"Download failed: {e}",
             )  # logger.init_err
             logger.info_warn("Model Reference", status="Local")  # logger.init_warn
             return json.loads((self.models_path).read_text())
 
     def get_model(self, model_name):
         return self.models.get(model_name)
 
@@ -102,15 +104,15 @@
 
     def get_available_models_by_types(self, model_types=None):
         if not model_types:
             model_types = ["ckpt", "diffusers"]
         models_available = []
         for model in self.models:
             if self.models[model]["type"] in model_types and self.check_available(
-                self.get_model_files(model)
+                self.get_model_files(model),
             ):
                 models_available.append(model)
         return models_available
 
     def count_available_models_by_types(self, model_types=None):
         return len(self.get_available_models_by_types(model_types))
 
@@ -193,24 +195,21 @@
                 return False
         return True
 
     @staticmethod
     def get_file_md5sum_hash(file_name):
         # Bail out if the source file doesn't exist
         if not os.path.isfile(file_name):
-            return
+            return None
 
         # Check if we have a cached md5 hash for the source file
         # and use that unless our source file is newer than our hash
         md5_file = f"{os.path.splitext(file_name)[0]}.md5"
         source_timestamp = os.path.getmtime(file_name)
-        if os.path.isfile(md5_file):
-            hash_timestamp = os.path.getmtime(md5_file)
-        else:
-            hash_timestamp = 0
+        hash_timestamp = os.path.getmtime(md5_file) if os.path.isfile(md5_file) else 0
         if hash_timestamp > source_timestamp:
             # Use our cached hash
             with open(md5_file, "rt") as handle:
                 md5_hash = handle.read().split()[0]
             return md5_hash
 
         # Calculate the hash of the source file
@@ -238,18 +237,17 @@
         if not os.path.isfile(file_name):
             raise FileNotFoundError("No file {}".format(file_name))
 
         # Check if we have a cached sha256 hash for the source file
         # and use that unless our source file is newer than our hash
         sha256_file = f"{os.path.splitext(file_name)[0]}.sha256"
         source_timestamp = os.path.getmtime(file_name)
-        if os.path.isfile(sha256_file):
-            hash_timestamp = os.path.getmtime(sha256_file)
-        else:
-            hash_timestamp = 0
+        hash_timestamp = (
+            os.path.getmtime(sha256_file) if os.path.isfile(sha256_file) else 0
+        )
         if hash_timestamp > source_timestamp:
             # Use our cached hash
             with open(sha256_file, "rt") as handle:
                 sha256_hash = handle.read().split()[0]
             return sha256_hash
 
         # Calculate the hash of the source file
@@ -338,29 +336,28 @@
         :param file_path: Path of the model's file. File is from the model's files list.
         Downloads a file
         """
         full_path = f"{self.path}/{file_path}"
         os.makedirs(os.path.dirname(full_path), exist_ok=True)
         pbar_desc = full_path.split("/")[-1]
         r = requests.get(url, stream=True, allow_redirects=True)
-        with open(full_path, "wb") as f:
-            with tqdm(
-                # all optional kwargs
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1024,
-                miniters=1,
-                desc=pbar_desc,
-                total=int(r.headers.get("content-length", 0)),
-                disable=WorkerSettings.disable_download_progress.active,
-            ) as pbar:
-                for chunk in r.iter_content(chunk_size=16 * 1024):
-                    if chunk:
-                        f.write(chunk)
-                        pbar.update(len(chunk))
+        with open(full_path, "wb") as f, tqdm(
+            # all optional kwargs
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+            miniters=1,
+            desc=pbar_desc,
+            total=int(r.headers.get("content-length", 0)),
+            disable=WorkerSettings.disable_download_progress.active,
+        ) as pbar:
+            for chunk in r.iter_content(chunk_size=16 * 1024):
+                if chunk:
+                    f.write(chunk)
+                    pbar.update(len(chunk))
 
     def download_model(self, model_name):
         """
         :param model_name: Name of the model
         Checks if the model is available, downloads the model if it is not available.
         After download, validates the model.
         Returns True if the model is available, False otherwise.
@@ -396,15 +393,15 @@
                 download_name = download[i]["file_name"]
             if "file_path" in download[i]:
                 download_path = download[i]["file_path"]
 
             if "manual" in download[i]:
                 logger.warning(
                     f"The model {model_name} requires manual download from {download_url}. "
-                    f"Please place it in {download_path}/{download_name} then press ENTER to continue..."
+                    f"Please place it in {download_path}/{download_name} then press ENTER to continue...",
                 )
                 input("")
                 continue
             # TODO: simplify
             if "file_content" in download[i]:
                 file_content = download[i]["file_content"]
                 logger.info(f"writing {file_content} to {file_path}")
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/blip.py` & `hordelib-0.2.0/hordelib/model_manager/blip.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 import torch
 
 # from nataili.util.blip import blip_decoder # XXX # FIXME
 from loguru import logger
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 
 class BlipModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{get_cache_directory()}/blip"
         self.models_db_name = "blip"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
         model_name: str,
         half_precision=True,
         gpu_id=0,
@@ -43,36 +44,40 @@
         """
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
             self.loaded_models[model_name] = self.load_blip(
                 model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
                 blip_image_eval_size=blip_image_eval_size,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
 
     def load_blip(
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
         cpu_only=False,
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/clip.py` & `hordelib-0.2.0/hordelib/model_manager/clip.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import open_clip
 import torch
 
 # from nataili.util.load_list import load_list
 from loguru import logger
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 
 class ClipModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{get_cache_directory()}/clip"
         self.models_db_name = "clip"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init(list_models=True)
 
     def load_data_lists(self):
         data_lists = {}
         # data_lists["artist"] = load_list(self.pkg / "artists.txt")
         # data_lists["flavors"] = load_list(self.pkg / "flavors.txt")
         # data_lists["medium"] = load_list(self.pkg / "mediums.txt")
@@ -89,15 +90,17 @@
     def load_clip(self, model_name, half_precision=True, gpu_id=0, cpu_only=False):
         if cpu_only:
             device = torch.device("cpu")
             half_precision = False
         else:
             device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
         model, preprocess = clip.load(
-            model_name, device=device, download_root=self.path
+            model_name,
+            device=device,
+            download_root=self.path,
         )
         model = model.eval()
         if half_precision:
             model = model.half()
         data_lists = self.load_data_lists()
         return {
             "model": model,
@@ -119,35 +122,47 @@
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(f"Downloading {model_name}", status="Downloading")
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             if not self.cuda_available:
                 cpu_only = True
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
             if self.models[model_name]["type"] == "open_clip":
                 self.loaded_models[model_name] = self.load_open_clip(
-                    model_name, half_precision, gpu_id, cpu_only
+                    model_name,
+                    half_precision,
+                    gpu_id,
+                    cpu_only,
                 )
             elif self.models[model_name]["type"] == "clip":
                 self.loaded_models[model_name] = self.load_clip(
-                    model_name, half_precision, gpu_id, cpu_only
+                    model_name,
+                    half_precision,
+                    gpu_id,
+                    cpu_only,
                 )
             elif self.models[model_name]["type"] == "coca":
                 self.loaded_models[model_name] = self.load_coca(
-                    model_name, half_precision, gpu_id, cpu_only
+                    model_name,
+                    half_precision,
+                    gpu_id,
+                    cpu_only,
                 )
             else:
                 logger.error(f"Unknown model type: {self.models[model_name]['type']}")
-                return
+                return None
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/codeformer.py` & `hordelib-0.2.0/hordelib/model_manager/safety_checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 import time
 
 import torch
-
-# from worker.model_manager.esrgan import EsrganModelManager# XXX # FIXME
-# from worker.model_manager.gfpgan import GfpganModelManager # XXX # FIXME
-# from nataili.util.codeformer import CodeFormer # XXX # FIXME
+from diffusers.pipelines.stable_diffusion.safety_checker import (
+    StableDiffusionSafetyChecker,
+)
 from loguru import logger
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 
-class CodeFormerModelManager(BaseModelManager):
+class SafetyCheckerModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
-        self.path = f"{get_cache_directory()}/codeformer"
-        self.models_db_name = "codeformer"
-        # self.gfpgan = GfpganModelManager()
-        # self.esrgan = EsrganModelManager()
+        self.path = f"{get_cache_directory()}/safety_checker"
+        self.models_db_name = "safety_checker"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
-        model_name: str,
+        model_name,
         half_precision=True,
         gpu_id=0,
         cpu_only=False,
     ):
         """
         model_name: str. Name of the model to load. See available_models for a list of available models.
         half_precision: bool. If True, the model will be loaded in half precision.
         gpu_id: int. The id of the gpu to use. If the gpu is not available, the model will be loaded on the cpu.
         cpu_only: bool. If True, the model will be loaded on the cpu. If True, half_precision will be set to False.
         """
+        if not self.cuda_available:
+            cpu_only = True
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
-            self.loaded_models[model_name] = self.load_codeformer(
+            self.loaded_models[model_name] = self.load_safety_checker(
                 model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
 
-    def load_codeformer(
+    def load_safety_checker(
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
-        cpu_only=False,
+        cpu_only=True,  # True by default for easy Horde compatibility
     ):
-        model_path = self.get_model_files(model_name)[0]["path"]
-        model_path = f"{self.path}/{model_path}"
         if not self.cuda_available:
             cpu_only = True
         if cpu_only:
             device = torch.device("cpu")
             half_precision = False
         else:
             device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
         logger.info(f"Loading model {model_name} on {device}")
-        logger.info(f"Model path: {model_path}")
-        model = CodeFormer(self.esrgan, self.gfpgan, self, device=device, upscale=1).to(
-            device
-        )  # XXX # FIXME
+        logger.info(f"Model path: {self.path}")
+        model = StableDiffusionSafetyChecker.from_pretrained(self.path)
+        model = model.eval()
+        model.to(device)
+        if half_precision:
+            model = model.half()
         return {"model": model, "device": device, "half_precision": half_precision}
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/compvis.py` & `hordelib-0.2.0/hordelib/model_manager/codeformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 import os
 import time
 
 from loguru import logger
 
+from hordelib import comfy_horde
 from hordelib.cache import get_cache_directory
-from hordelib.comfy_horde import load_checkpoint_guess_config
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 
-class CompVisModelManager(BaseModelManager):
-    def __init__(self, download_reference=True, custom_path="models/custom"):
+class CodeFormerModelManager(BaseModelManager):
+    def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
-        self.path = f"{get_cache_directory()}/compvis"
-        self.custom_path = custom_path
-        self.models_db_name = "stable_diffusion"
+        self.path = f"{get_cache_directory()}/codeformer"
+        self.models_db_name = "codeformer"
+        # self.gfpgan = GfpganModelManager()
+        # self.esrgan = EsrganModelManager()
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
         model_name: str,
-        output_vae=True,
-        output_clip=True,
+        half_precision=True,
+        gpu_id=0,
+        cpu_only=False,
     ):
         """
         model_name: str. Name of the model to load. See available_models for a list of available models.
+        half_precision: bool. If True, the model will be loaded in half precision.
+        gpu_id: int. The id of the gpu to use. If the gpu is not available, the model will be loaded on the cpu.
+        cpu_only: bool. If True, the model will be loaded on the cpu. If True, half_precision will be set to False.
         """
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
+            logger.info(
+                f"Downloading {model_name}",
+                status="Downloading",
+            )  # logger.init_ok
             self.download_model(model_name)
-            logger.info(f"{model_name}", status="Downloaded")  # logger.init_ok
+            logger.info(
+                f"{model_name} downloaded",
+                status="Downloading",
+            )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
-            embeddings_path = os.getenv("HORDE_MODEL_DIR_EMBEDDINGS", "./")
-            ckpt_path = self.get_model_files(model_name)[0]["path"]
-            ckpt_path = f"{self.path}/{ckpt_path}"
-            self.loaded_models[model_name] = load_checkpoint_guess_config(
-                ckpt_path,
-                output_vae=True,
-                output_clip=True,
-                embedding_directory=embeddings_path,
+            self.loaded_models[model_name] = self.load_codeformer(
+                model_name,
             )
+            logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"{model_name}: {round(toc-tic,2)} seconds", status="Loaded"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
+
+    def load_codeformer(
+        self,
+        model_name,
+    ):
+        model_path = self.get_model_files(model_name)[0]["path"]
+        model_path = f"{self.path}/{model_path}"
+        sd = comfy_horde.load_torch_file(model_path)
+        out = comfy_horde.model_loading.load_state_dict(sd).eval()
+        return (out,)
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/controlnet.py` & `hordelib-0.2.0/hordelib/model_manager/controlnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import safetensors.torch
 import torch
 from loguru import logger
 from omegaconf import OmegaConf
 
 # from ldm.util import instantiate_from_config
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 from hordelib.model_manager.torch_hijack import (
     DisableInitialization,
     instantiate_from_config,
 )
 
 
 class ControlNetModelManager(BaseModelManager):
     def __init__(self, download_reference=True, compvis=None):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{get_cache_directory()}/controlnet"
         self.models_db_name = "controlnet"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.control_nets = {}
         self.init()
 
     def load_control_ldm(
         self,
         model_name,
         target_name,
@@ -60,63 +61,66 @@
         logger.info("Merge control net state dict into target state dict")
         if "_sd2" not in model_name:
             for key in keys:
                 if not key.startswith("control_"):
                     continue
                 p = sd15_with_control_state_dict[key]
                 key_name = f'model.diffusion_model.{key.replace("control_model.", "")}'
-                if key_name in input_state_dict.keys():
+                if key_name in input_state_dict:
                     # logger.info(f"merging {key_name} from input {key} from control")
                     p_new = p + input_state_dict[key_name].clone().cpu()
                 else:
                     # logger.info(f"directly copying {key_name} from control")
                     p_new = p
                 final_state_dict[key] = p_new
         else:
             for key in keys:
                 p = sd15_with_control_state_dict[key]
                 key_name = f'model.diffusion_model.{key.replace("control_model.", "")}'
-                if key in input_state_dict.keys():
+                if key in input_state_dict:
                     # logger.info(f"merging {key_name} from input {key} from control")
                     p_new = p + input_state_dict[key_name].clone().cpu()
                 else:
                     # logger.info(f"directly copying {key_name} from control")
                     p_new = p
                 final_state_dict[f"control_model.{key}"] = p_new
         # remove key "lvlb_weights"
-        if "lvlb_weights" in final_state_dict.keys():
+        if "lvlb_weights" in final_state_dict:
             final_state_dict.pop("lvlb_weights")
         logger.info("Finished merging control net state dict into target state dict")
         logger.info(f"Loading {full_name} state dict")
         model.load_state_dict(final_state_dict, strict=True)
         logger.info(f"Loaded {full_name} state dict")
         if half_precision:
             model.half()
         del final_state_dict, sd15_with_control_state_dict, input_state_dict
         self.loaded_models[full_name] = {
             "model": model,
             "device": device,
             "half_precision": half_precision,
         }
+        return None
 
     def load_controlnet(
         self,
         model_name,
     ):
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name in self.control_nets:
             logger.info(f"{model_name} already loaded")
             return True
         model_path = self.get_model_files(model_name)[0]["path"]
         model_path = f"{self.path}/{model_path}"
         logger.info(f"Loading controlnet {model_name}")
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/diffusers.py` & `hordelib-0.2.0/hordelib/model_manager/diffusers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from diffusers.pipelines import (
     StableDiffusionDepth2ImgPipeline,
     StableDiffusionInpaintPipeline,
 )
 from loguru import logger
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 # from nataili.util.voodoo import push_diffusers_pipeline_to_plasma
 
 
 class DiffusersModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{get_cache_directory()}/diffusers"
         self.models_db_name = "diffusers"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
@@ -40,36 +41,40 @@
         """
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
             self.loaded_models[model_name] = self.load_diffusers(
                 model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
                 voodoo=voodoo,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
 
     def load_diffusers(
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
         cpu_only=False,
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/gfpgan.py` & `hordelib-0.2.0/hordelib/model_manager/new.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 import time
 
 import torch
-
-# from nataili.util.gfpgan import GFPGANer # XXX # FIXME
 from loguru import logger
 
 from hordelib.cache import get_cache_directory
+from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.model_manager.base import BaseModelManager
 
 
-class GfpganModelManager(BaseModelManager):
+class NewModelManager(BaseModelManager):
     def __init__(self, download_reference=True):
         super().__init__()
         self.download_reference = download_reference
-        self.path = f"{get_cache_directory()}/gfpgan"
-        self.models_db_name = "gfpgan"
+        self.path = f"{get_cache_directory()}/new"
+        self.models_db_name = "new"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
-        model_name: str,
+        model_name,
+        half_precision=True,
         gpu_id=0,
         cpu_only=False,
     ):
         """
         model_name: str. Name of the model to load. See available_models for a list of available models.
+        half_precision: bool. If True, the model will be loaded in half precision.
         gpu_id: int. The id of the gpu to use. If the gpu is not available, the model will be loaded on the cpu.
         cpu_only: bool. If True, the model will be loaded on the cpu. If True, half_precision will be set to False.
         """
         if not self.cuda_available:
             cpu_only = True
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
-            self.loaded_models[model_name] = self.load_gfpgan(
+            self.loaded_models[model_name] = self.load_new(
                 model_name,
+                half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
             )
-            logger.info(f"Loading {model_name}", status="Success")
+            logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
             return True
+        return None
 
-    def load_gfpgan(
+    def load_new(
         self,
         model_name,
+        half_precision=True,
         gpu_id=0,
         cpu_only=False,
     ):
         model_path = self.get_model_files(model_name)[0]["path"]
         model_path = f"{self.path}/{model_path}"
         if cpu_only:
             device = torch.device("cpu")
+            half_precision = False
         else:
             device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
         logger.info(f"Loading model {model_name} on {device}")
         logger.info(f"Model path: {model_path}")
-        model = GFPGANer(  # XXX # FIXME
-            model_path=model_path,
-            upscale=1,
-            arch="clean",
-            channel_multiplier=2,
-            bg_upsampler=None,
-            device=device,
-            cache_dir=self.path,
-        )
-        return {"model": model, "device": device}
+
+        model = model.eval()  # XXX # FIXME model can be unbound at this point...
+        model.to(device)
+        if half_precision:
+            model = model.half()
+        return {"model": model, "device": device, "half_precision": half_precision}
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/hyper.py` & `hordelib-0.2.0/hordelib/model_manager/hyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,40 +6,31 @@
 from hordelib.model_manager.base import BaseModelManager
 from hordelib.model_manager.blip import BlipModelManager
 from hordelib.model_manager.clip import ClipModelManager
 from hordelib.model_manager.codeformer import CodeFormerModelManager
 from hordelib.model_manager.compvis import CompVisModelManager
 from hordelib.model_manager.controlnet import ControlNetModelManager
 from hordelib.model_manager.diffusers import DiffusersModelManager
-
-# from hordelib.model_manager.esrgan import EsrganModelManager
-# from hordelib.model_manager.gfpgan import GfpganModelManager
+from hordelib.model_manager.esrgan import EsrganModelManager
+from hordelib.model_manager.gfpgan import GfpganModelManager
 from hordelib.model_manager.safety_checker import SafetyCheckerModelManager
 
 # from worker.util.voodoo import initialise_voodoo
 
 
-class EsrganModelManager:  # XXX # FIXME
-    pass
-
-
-class GfpganModelManager:  # XXX # FIXME
-    pass
-
-
 MODEL_MANAGERS_TYPE_LOOKUP = {
     "aitemplate": AITemplateModelManager,
     "blip": BlipModelManager,
     "clip": ClipModelManager,
     "codeformer": CodeFormerModelManager,
     "compvis": CompVisModelManager,
     "controlnet": ControlNetModelManager,
     "diffusers": DiffusersModelManager,
-    # "esrgan": EsrganModelManager,
-    # "gfpgan": GfpganModelManager,
+    "esrgan": EsrganModelManager,
+    "gfpgan": GfpganModelManager,
     "safety_checker": SafetyCheckerModelManager,
 }
 """Keys are `str` which represent attrs in `ModelManger`. Values are the corresponding `type`."""
 
 
 class ModelManager:
     """Controller class for all managers which extend `BaseModelManager`."""
@@ -76,28 +67,28 @@
         aitemplate: bool = False,
         blip: bool = False,
         clip: bool = False,
         codeformer: bool = False,
         compvis: bool = False,
         controlnet: bool = False,
         diffusers: bool = False,
-        # esrgan: bool = False,
-        # gfpgan: bool = False,
+        esrgan: bool = False,
+        gfpgan: bool = False,
         safety_checker: bool = False,
     ):  # XXX are we married to the name and/or the idea behind this function
         """For each arg which is true, attempt to load that `BaseModelManager` type."""
         args_passed: dict = locals().copy()
         args_passed.pop("self")
 
         allModelMangerTypeKeys = MODEL_MANAGERS_TYPE_LOOKUP.keys()
         # e.g. `MODEL_MANAGERS_TYPE_LOOKUP["compvis"]`` returns type `CompVisModelManager`
 
         for argName, argValue in args_passed.items():
             if not (argName in allModelMangerTypeKeys and hasattr(self, argName)):
-                raise Exception()  # XXX better guarantees need to be made
+                raise Exception  # XXX better guarantees need to be made
             if not argValue:
                 continue
 
             modelmanager = MODEL_MANAGERS_TYPE_LOOKUP[argName]
 
             # at runtime modelmanager() will be CompVisModelManager(), ClipModelManager(), etc
             setattr(self, argName, modelmanager())
@@ -124,15 +115,15 @@
             if model_type is not None:
                 self.models.update(model_type.models)
                 self.available_models.extend(model_type.available_models)
 
     def reload_database(self) -> None:
         """Completely resets the `BaseModelManager` classes, and forces each to re-init."""
         model_managers: list[BaseModelManager] = []
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_managers.append(getattr(self, model_manager_type))
 
         self.available_models = []  # reset available models
         for model_manager in model_managers:
             if model_manager is not None:
                 model_manager.init()
                 self.models.update(model_manager.models)
@@ -143,51 +134,53 @@
 
         Args:
             model_name (str): The name of the model to find and attempt to download.
 
         Returns:
             bool | None: The success of the download. If `None`, the model_name was not found.
         """
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             if model_name not in model_manager.models:
                 continue
 
             return model_manager.download_model(model_name)
         logger.warning(f"Model '{model_name}' not found!")
         return None  # XXX if the download fails, the file causes issues # FIXME
 
     def download_all(self) -> None:
         """Attempts to download all available models for all `BaseModelManager` types."""
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             if isinstance(model_manager, AITemplateModelManager):
                 model_manager.download_ait("cuda")
                 # XXX this special handling predates me (@tazlin)
                 continue
 
             model_manager.download_all_models()
 
     def validate_model(
-        self, model_name: str, skip_checksum: bool = False
+        self,
+        model_name: str,
+        skip_checksum: bool = False,
     ) -> bool | None:
         """Runs a integrity check against the model specified.
 
         Args:
             model_name (str): The model to check.
             skip_checksum (bool, optional): Whether to skip the SHA/MD5 check. Defaults to False.
 
         Returns:
             bool | None: The result of the validation. If `None`, the model was not found.
         """
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             if model_manager_type == "aitemplate":
                 continue
                 # XXX the special handling here predates me (@tazlin), unknown if needed
             if model_name in model_manager.models:
@@ -196,15 +189,15 @@
 
     def taint_models(self, models: list[str]) -> None:
         """Marks a list of models to be unavailable.
 
         Args:
             models (list[str]): The list of models to mark.
         """
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             if any(model in model_manager.models for model in models):
                 model_manager.taint_models(models)
         self.refreshManagers()
 
@@ -213,15 +206,15 @@
 
         Args:
             model_name (str): The model name to remove.
 
         Returns:
             bool | None: The result of the unloading. If `None`, the model was not found.
         """
-        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP.keys():
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
             if model_name not in model_manager.models:
                 continue
             model_unloaded = model_manager.unload_model(model_name)
             del self.loaded_models[model_name]
@@ -237,36 +230,35 @@
         return list(self.loaded_models.keys())
 
     def get_available_models_by_types(self, model_types: list[str] | None = None):
         if not model_types:
             model_types = ["ckpt", "diffusers"]
         models_available = []
         for model_type in model_types:
-            if model_type == "ckpt":
-                if self.compvis is not None:
-                    for model in self.compvis.models:
-                        # We don't want to check the .yaml file as those exist in this repo instead
-                        model_files = [
-                            filename
-                            for filename in self.compvis.get_model_files(model)
-                            if not filename["path"].endswith(".yaml")
-                        ]
-                        if self.compvis.check_available(model_files):
-                            models_available.append(model)
-            if model_type == "diffusers":
-                if self.diffusers is not None:
-                    for model in self.diffusers.models:
-                        if self.diffusers.check_available(
-                            self.diffusers.get_model_files(model)
-                        ):
-                            models_available.append(model)
+            if model_type == "ckpt" and self.compvis is not None:
+                for model in self.compvis.models:
+                    # We don't want to check the .yaml file as those exist in this repo instead
+                    model_files = [
+                        filename
+                        for filename in self.compvis.get_model_files(model)
+                        if not filename["path"].endswith(".yaml")
+                    ]
+                    if self.compvis.check_available(model_files):
+                        models_available.append(model)
+            if model_type == "diffusers" and self.diffusers is not None:
+                for model in self.diffusers.models:
+                    if self.diffusers.check_available(
+                        self.diffusers.get_model_files(model),
+                    ):
+                        models_available.append(model)
         return models_available
 
     def count_available_models_by_types(
-        self, model_types: list[str] | None = None
+        self,
+        model_types: list[str] | None = None,
     ) -> int:
         return len(self.get_available_models_by_types(model_types))
 
     def get_available_models(self) -> list:
         """Returns a list of all available models.
 
         Returns:
@@ -307,93 +299,87 @@
                 model_name=model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.blip.loaded_models[model_name]}
+                    {model_name: self.blip.loaded_models[model_name]},
                 )
             return success
         if self.clip is not None and model_name in self.clip.models:
             success = self.clip.load(
                 model_name=model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.clip.loaded_models[model_name]}
+                    {model_name: self.clip.loaded_models[model_name]},
                 )
             return success
         if self.codeformer is not None and model_name in self.codeformer.models:
             success = self.codeformer.load(
                 model_name=model_name,
-                half_precision=half_precision,
-                gpu_id=gpu_id,
-                cpu_only=cpu_only,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.codeformer.loaded_models[model_name]}
+                    {model_name: self.codeformer.loaded_models[model_name]},
                 )
             return success
         if self.compvis is not None and model_name in self.compvis.models:
             success = self.compvis.load(
                 model_name=model_name,
                 output_vae=True,
                 output_clip=True,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.compvis.loaded_models[model_name]}
+                    {model_name: self.compvis.loaded_models[model_name]},
                 )
             return success
         if self.diffusers is not None and model_name in self.diffusers.models:
             success = self.diffusers.load(
                 model_name=model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
                 voodoo=voodoo,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.diffusers.loaded_models[model_name]}
+                    {model_name: self.diffusers.loaded_models[model_name]},
                 )
             return success
         if self.esrgan is not None and model_name in self.esrgan.models:
             success = self.esrgan.load(
                 model_name=model_name,
-                half_precision=half_precision,
-                gpu_id=gpu_id,
-                cpu_only=cpu_only,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.esrgan.loaded_models[model_name]}
+                    {model_name: self.esrgan.loaded_models[model_name]},
                 )
             return success
         if self.gfpgan is not None and model_name in self.gfpgan.models:
             success = self.gfpgan.load(
-                model_name=model_name, gpu_id=gpu_id, cpu_only=cpu_only
+                model_name=model_name,
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.gfpgan.loaded_models[model_name]}
+                    {model_name: self.gfpgan.loaded_models[model_name]},
                 )
             return success
         if self.safety_checker is not None and model_name in self.safety_checker.models:
             success = self.safety_checker.load(
                 model_name=model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=True,  # for the horde
             )
             if success:
                 self.loaded_models.update(
-                    {model_name: self.safety_checker.loaded_models[model_name]}
+                    {model_name: self.safety_checker.loaded_models[model_name]},
                 )
             return success
         logger.error(f"{model_name} not found")
         return False
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/sdu.py` & `hordelib-0.2.0/hordelib/model_manager/sdu.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import k_diffusion as K
 import torch
 import torch.nn.functional as F
 from loguru import logger
 from omegaconf import OmegaConf
 from torch import nn
 
+from hordelib.consts import REMOTE_MODEL_DB
+
 # from ldm.util import instantiate_from_config
 from hordelib.model_manager.base import BaseModelManager
 
 
 class NoiseLevelAndTextConditionedUpscaler(nn.Module):
     def __init__(self, inner_model, sigma_data=1.0, embed_dim=256):
         super().__init__()
@@ -75,15 +77,16 @@
     @property
     def device(self):
         return self.transformer.device
 
     def forward(self, tok_out):
         input_ids, cross_cond_padding = tok_out
         clip_out = self.transformer(
-            input_ids=input_ids.to(self.device), output_hidden_states=True
+            input_ids=input_ids.to(self.device),
+            output_hidden_states=True,
         )
         return (
             clip_out.hidden_states[-1],
             cross_cond_padding.to(self.device),
             clip_out.pooler_output,
         )
 
@@ -91,15 +94,15 @@
 class SDUModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__()
         self.download_reference = download_reference
         self.path = f"{Path.home()}/.cache/nataili/sdu"
         self.models_db_name = "sdu"
         self.models_path = self.pkg / f"{self.models_db_name}.json"
-        self.remote_db = f"https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/{self.models_db_name}.json"
+        self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.init()
 
     def load(
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
@@ -113,45 +116,52 @@
         """
         if model_name not in self.models:
             logger.error(f"{model_name} not found")
             return
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             logger.info(
-                f"Downloading {model_name}", status="Downloading"
+                f"Downloading {model_name}",
+                status="Downloading",
             )  # logger.init_ok
             self.download_model(model_name)
             logger.info(
-                f"{model_name} downloaded", status="Downloading"
+                f"{model_name} downloaded",
+                status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
             self.loaded_models[model_name] = self.load_sdu(
                 model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
             toc = time.time()
             logger.info(
-                f"Loading {model_name}: Took {toc-tic} seconds", status="Success"
+                f"Loading {model_name}: Took {toc-tic} seconds",
+                status="Success",
             )  # logger.init_ok
 
     def load_model_from_config(
-        self, model_path="", config_path="", map_location="cpu", device="cpu"
+        self,
+        model_path="",
+        config_path="",
+        map_location="cpu",
+        device="cpu",
     ):
         config = OmegaConf.load(config_path)
         pl_sd = torch.load(model_path, map_location=map_location)
         if "global_step" in pl_sd:
             logger.info(f"Global Step: {pl_sd['global_step']}")
         sd = pl_sd["state_dict"] if "state_dict" in pl_sd else pl_sd
         model = instantiate_from_config(
-            config.model
+            config.model,
         )  # XXX # FIXME (instantiate_from_config missing)
         m, u = model.load_state_dict(sd, strict=False)
         model = model.eval().requires_grad_(False)
         del pl_sd, sd, m, u
         return model
 
     def load_sdu(
@@ -191,18 +201,20 @@
         model.load_state_dict(ckpt["model_ema"])
         model = K.config.make_denoiser_wrapper(config)(model)
         if not train:
             model = model.eval().requires_grad_(False)
         model = model.eval()
         model.to(device)
         vae_model_840k = self.load_model_from_config(
-            model_path=vae_840k_path, config_path=vae_config_path
+            model_path=vae_840k_path,
+            config_path=vae_config_path,
         )
         vae_model_560k = self.load_model_from_config(
-            model_path=vae_560k_path, config_path=vae_config_path
+            model_path=vae_560k_path,
+            config_path=vae_config_path,
         )
         vae_model_840k = vae_model_840k.to(device)
         vae_model_560k = vae_model_560k.to(device)
         tokenizer = CLIPTokenizerTransform()
         text_encoder = CLIPEmbedder(device=device)
         return {
             "model": model,
```

### Comparing `hordelib-0.1.0/hordelib/model_manager/torch_hijack.py` & `hordelib-0.2.0/hordelib/model_manager/torch_hijack.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def instantiate_from_config(config):
     if "target" not in config:
         if config == "__is_first_stage__":
             return None
         elif config == "__is_unconditional__":
             return None
         raise KeyError("Expected key `target` to instantiate.")
-    return get_obj_from_str(config["target"])(**config.get("params", dict()))
+    return get_obj_from_str(config["target"])(**config.get("params", {}))
 
 
 def get_obj_from_str(string, reload=False):
     module, cls = string.rsplit(".", 1)
     if reload:
         module_imp = importlib.import_module(module)
         importlib.reload(module_imp)
@@ -53,46 +53,55 @@
         return original
 
     def __enter__(self):
         def do_nothing(*args, **kwargs):
             pass
 
         def create_model_and_transforms_without_pretrained(
-            self, *args, pretrained=None, **kwargs
+            self,
+            *args,
+            pretrained=None,
+            **kwargs,
         ):
             return self.create_model_and_transforms(*args, pretrained=None, **kwargs)
 
         def CLIPTextModel_from_pretrained(
-            self, pretrained_model_name_or_path, *model_args, **kwargs
+            self,
+            pretrained_model_name_or_path,
+            *model_args,
+            **kwargs,
         ):
             if sys.version_info != (3, 8, 10):
                 try:
                     res = self.CLIPTextModel_from_pretrained(
                         None,
                         *model_args,
                         config=pretrained_model_name_or_path,
                         state_dict={},
                         **kwargs,
                     )
                 except Exception:  # XXX should catch the actual exception intended
                     res = self.CLIPTextModel_from_pretrained(
-                        None, *model_args, **kwargs
+                        None,
+                        *model_args,
+                        **kwargs,
                     )
             else:
                 res = self.CLIPTextModel_from_pretrained(None, *model_args, **kwargs)
 
             res.name_or_path = pretrained_model_name_or_path
             return res
 
         def transformers_modeling_utils_load_pretrained_model(self, *args, **kwargs):
             args = args[0:3] + ("/",) + args[4:]
             # resolved_archive_file; must set it to something to prevent what seems to be a bug
             # XXX looks like some old hack
             return self.transformers_modeling_utils_load_pretrained_model(
-                *args, **kwargs
+                *args,
+                **kwargs,
             )
 
         def transformers_utils_hub_get_file_from_cache(original, url, *args, **kwargs):
             # this file is always 404, prevent making request
             # XXX looks like some old hack
             bad_url = "https://huggingface.co/openai/clip-vit-large-patch14/resolve/main/added_tokens.json"
             if (
@@ -107,35 +116,50 @@
                 if res is None:
                     res = original(url, *args, local_files_only=False, **kwargs)
                 return res
             except Exception:
                 return original(url, *args, local_files_only=False, **kwargs)
 
         def transformers_utils_hub_get_from_cache(
-            url, *args, local_files_only=False, **kwargs
+            url,
+            *args,
+            local_files_only=False,
+            **kwargs,
         ):
             return transformers_utils_hub_get_file_from_cache(
-                self.transformers_utils_hub_get_from_cache, url, *args, **kwargs
+                self.transformers_utils_hub_get_from_cache,
+                url,
+                *args,
+                **kwargs,
             )
 
         def transformers_tokenization_utils_base_cached_file(
-            url, *args, local_files_only=False, **kwargs
+            url,
+            *args,
+            local_files_only=False,
+            **kwargs,
         ):
             return transformers_utils_hub_get_file_from_cache(
                 self.transformers_tokenization_utils_base_cached_file,
                 url,
                 *args,
                 **kwargs,
             )
 
         def transformers_configuration_utils_cached_file(
-            url, *args, local_files_only=False, **kwargs
+            url,
+            *args,
+            local_files_only=False,
+            **kwargs,
         ):
             return transformers_utils_hub_get_file_from_cache(
-                self.transformers_configuration_utils_cached_file, url, *args, **kwargs
+                self.transformers_configuration_utils_cached_file,
+                url,
+                *args,
+                **kwargs,
             )
 
         self.replace(torch.nn.init, "kaiming_uniform_", do_nothing)
         self.replace(torch.nn.init, "_no_grad_normal_", do_nothing)
         self.replace(torch.nn.init, "_no_grad_uniform_", do_nothing)
 
         if self.disable_clip:
```

### Comparing `hordelib-0.1.0/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.2.0/hordelib/nodes/node_clip_similarities.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,22 @@
     def get_similarities(self, clip_name, images, string_list=None):
         results = []
         for image in images:
             model = SharedModelManager.manager.clip.loaded_models[clip_name]
             # XXX better guarantees need to be made
             interrogator = Interrogator(model)
             similarity_results = interrogator(
-                image=image, text_array=string_list, similarity=True
+                image=image,
+                text_array=string_list,
+                similarity=True,
             )
             if similarity_results is None:
                 return None  # XXX better guarantees need to be made
 
             results.append(
-                {"similarity_results": similarity_results["default"], "type": "ARRAY"}
+                {"similarity_results": similarity_results["default"], "type": "ARRAY"},
             )
 
         return {"similarities": results}
 
 
 NODE_CLASS_MAPPINGS = {"HordeClipSimilarities": HordeClipSimilarities}
```

### Comparing `hordelib-0.1.0/hordelib/nodes/node_image_output.py` & `hordelib-0.2.0/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.1.0/hordelib/nodes/node_model_loader.py` & `hordelib-0.2.0/hordelib/nodes/node_model_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # node_model_loader.py
 # Simple proof of concept custom node to load models.
-# We shall expand this to actually integrate with the horde model manager.
 
 from loguru import logger
 
 
 class HordeCheckpointLoader:
     @classmethod
     def INPUT_TYPES(s):
         return {
             "required": {
                 "model_manager": ("<model manager instance>",),
-                "ckpt_name": ("<checkpoint file>",),
-            }
+                "model_name": ("<model name>",),
+            },
         }
 
     RETURN_TYPES = ("MODEL", "CLIP", "VAE")
     FUNCTION = "load_checkpoint"
 
     CATEGORY = "loaders"
 
-    def load_checkpoint(self, model_manager, ckpt_name, output_vae=True, output_clip=True):
+    def load_checkpoint(
+        self,
+        model_manager,
+        model_name,
+        output_vae=True,
+        output_clip=True,
+    ):
+        logger.debug(f"Loading model {model_name} through our custom node")
+
+        if model_manager.manager is None:
+            logger.error("horde_model_manager appears to be missing!")
+            raise RuntimeError  # XXX better guarantees need to be made
+
+        if model_name not in model_manager.manager.loaded_models:
+            logger.error(f"Model {model_name} is not loaded")
+            raise RuntimeError  # XXX better guarantees need to be made
 
-        if model_manager.manager.compvis is None:
-            logger.error("horde_model_manager.compvis appears to be missing!")
-            raise RuntimeError()  # XXX better guarantees need to be made
-
-        if ckpt_name not in model_manager.manager.compvis.loaded_models:
-            logger.error(f"Model {ckpt_name} is not loaded")
-            raise RuntimeError()  # XXX better guarantees need to be made
-
-        return model_manager.manager.compvis.loaded_models[ckpt_name]
+        return model_manager.manager.loaded_models[model_name]
 
 
 NODE_CLASS_MAPPINGS = {"HordeCheckpointLoader": HordeCheckpointLoader}
```

### Comparing `hordelib-0.1.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8195494284361472%*

 * *Differences: {"'last_link_id'": '21',*

 * * "'last_node_id'": '14',*

 * * "'links'": "{insert: [(9, [18, 5, 0, 3, 3, 'LATENT']), (10, [19, 11, 1, 14, 2, 'MASK']), (11, "*

 * *            "[20, 4, 2, 14, 1, 'VAE']), (12, [21, 11, 0, 14, 0, 'IMAGE'])], delete: [1]}",*

 * * "'nodes'": "{3: {'id': 10, 'type': 'CLIPSetLastLayer', 'pos': [376, 145], 'size': {'0': 210, '1': "*

 * *            "58}, 'order': 3, 'outputs': {0: {'name': 'CLIP', 'type': 'CLIP', 'links': [11, 13]}}, "*

 * *            "'title': 'clip_skip', 'properties': {'Node name for S&R': ' […]*

```diff
@@ -1,31 +1,23 @@
 {
     "config": {},
     "extra": {},
     "groups": [],
-    "last_link_id": 13,
-    "last_node_id": 10,
+    "last_link_id": 21,
+    "last_node_id": 14,
     "links": [
         [
             1,
             4,
             0,
             3,
             0,
             "MODEL"
         ],
         [
-            2,
-            5,
-            0,
-            3,
-            3,
-            "LATENT"
-        ],
-        [
             4,
             6,
             0,
             3,
             1,
             "CONDITIONING"
         ],
@@ -80,118 +72,269 @@
         [
             13,
             10,
             0,
             7,
             0,
             "CLIP"
+        ],
+        [
+            18,
+            5,
+            0,
+            3,
+            3,
+            "LATENT"
+        ],
+        [
+            19,
+            11,
+            1,
+            14,
+            2,
+            "MASK"
+        ],
+        [
+            20,
+            4,
+            2,
+            14,
+            1,
+            "VAE"
+        ],
+        [
+            21,
+            11,
+            0,
+            14,
+            0,
+            "IMAGE"
         ]
     ],
     "nodes": [
         {
             "flags": {},
-            "id": 5,
+            "id": 8,
+            "inputs": [
+                {
+                    "link": 7,
+                    "name": "samples",
+                    "type": "LATENT"
+                },
+                {
+                    "link": 8,
+                    "name": "vae",
+                    "type": "VAE"
+                }
+            ],
             "mode": 0,
-            "order": 0,
+            "order": 8,
             "outputs": [
                 {
                     "links": [
-                        2
+                        9
                     ],
-                    "name": "LATENT",
+                    "name": "IMAGE",
                     "slot_index": 0,
-                    "type": "LATENT"
+                    "type": "IMAGE"
                 }
             ],
             "pos": [
-                510,
-                549
+                1384,
+                398
             ],
             "properties": {
-                "Node name for S&R": "EmptyLatentImage"
+                "Node name for S&R": "VAEDecode"
             },
             "size": {
-                "0": 315,
-                "1": 106
+                "0": 210,
+                "1": 46
             },
-            "title": "empty_latent_image",
-            "type": "EmptyLatentImage",
+            "title": "vae_decode",
+            "type": "VAEDecode"
+        },
+        {
+            "flags": {},
+            "id": 7,
+            "inputs": [
+                {
+                    "link": 13,
+                    "name": "clip",
+                    "slot_index": 0,
+                    "type": "CLIP"
+                }
+            ],
+            "mode": 0,
+            "order": 6,
+            "outputs": [
+                {
+                    "links": [
+                        6
+                    ],
+                    "name": "CONDITIONING",
+                    "slot_index": 0,
+                    "type": "CONDITIONING"
+                }
+            ],
+            "pos": [
+                588,
+                409
+            ],
+            "properties": {
+                "Node name for S&R": "CLIPTextEncode"
+            },
+            "size": {
+                "0": 243.0001220703125,
+                "1": 90.3333740234375
+            },
+            "title": "negative_prompt",
+            "type": "CLIPTextEncode",
             "widgets_values": [
-                512,
-                512,
-                1
+                "painting, drawing, artwork"
+            ]
+        },
+        {
+            "flags": {},
+            "id": 6,
+            "inputs": [
+                {
+                    "link": 11,
+                    "name": "clip",
+                    "type": "CLIP"
+                }
+            ],
+            "mode": 0,
+            "order": 5,
+            "outputs": [
+                {
+                    "links": [
+                        4
+                    ],
+                    "name": "CONDITIONING",
+                    "slot_index": 0,
+                    "type": "CONDITIONING"
+                }
+            ],
+            "pos": [
+                650,
+                54
+            ],
+            "properties": {
+                "Node name for S&R": "CLIPTextEncode"
+            },
+            "size": {
+                "0": 236.33343505859375,
+                "1": 83.00006103515625
+            },
+            "title": "prompt",
+            "type": "CLIPTextEncode",
+            "widgets_values": [
+                "dinosaur "
+            ]
+        },
+        {
+            "flags": {},
+            "id": 10,
+            "inputs": [
+                {
+                    "link": 12,
+                    "name": "clip",
+                    "type": "CLIP"
+                }
+            ],
+            "mode": 0,
+            "order": 3,
+            "outputs": [
+                {
+                    "links": [
+                        11,
+                        13
+                    ],
+                    "name": "CLIP",
+                    "slot_index": 0,
+                    "type": "CLIP"
+                }
+            ],
+            "pos": [
+                376,
+                145
+            ],
+            "properties": {
+                "Node name for S&R": "CLIPSetLastLayer"
+            },
+            "size": {
+                "0": 210,
+                "1": 58
+            },
+            "title": "clip_skip",
+            "type": "CLIPSetLastLayer",
+            "widgets_values": [
+                -1
             ]
         },
         {
             "flags": {},
             "id": 9,
             "inputs": [
                 {
                     "link": 9,
                     "name": "images",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 7,
+            "order": 9,
             "pos": [
                 1627,
                 432
             ],
             "properties": {},
             "size": {
-                "0": 210,
-                "1": 58
+                "0": 307,
+                "1": 400
             },
             "title": "output_image",
             "type": "SaveImage",
             "widgets_values": [
                 "ComfyUI"
             ]
         },
         {
             "flags": {},
-            "id": 8,
-            "inputs": [
-                {
-                    "link": 7,
-                    "name": "samples",
-                    "type": "LATENT"
-                },
-                {
-                    "link": 8,
-                    "name": "vae",
-                    "type": "VAE"
-                }
-            ],
+            "id": 5,
             "mode": 0,
-            "order": 6,
+            "order": 0,
             "outputs": [
                 {
                     "links": [
-                        9
+                        18
                     ],
-                    "name": "IMAGE",
+                    "name": "LATENT",
                     "slot_index": 0,
-                    "type": "IMAGE"
+                    "type": "LATENT"
                 }
             ],
             "pos": [
-                1384,
-                398
+                467,
+                563
             ],
             "properties": {
-                "Node name for S&R": "VAEDecode"
+                "Node name for S&R": "EmptyLatentImage"
             },
             "size": {
-                "0": 210,
-                "1": 46
+                "0": 315,
+                "1": 106
             },
-            "title": "vae",
-            "type": "VAEDecode"
+            "title": "empty_latent_image",
+            "type": "EmptyLatentImage",
+            "widgets_values": [
+                512,
+                512,
+                1
+            ]
         },
         {
             "flags": {},
             "id": 3,
             "inputs": [
                 {
                     "link": 1,
@@ -205,21 +348,21 @@
                 },
                 {
                     "link": 6,
                     "name": "negative",
                     "type": "CONDITIONING"
                 },
                 {
-                    "link": 2,
+                    "link": 18,
                     "name": "latent_image",
                     "type": "LATENT"
                 }
             ],
             "mode": 0,
-            "order": 5,
+            "order": 7,
             "outputs": [
                 {
                     "links": [
                         7
                     ],
                     "name": "LATENT",
                     "slot_index": 0,
@@ -236,15 +379,15 @@
             "size": {
                 "0": 315,
                 "1": 262
             },
             "title": "sampler",
             "type": "KSampler",
             "widgets_values": [
-                8566257,
+                843159458049729,
                 true,
                 20,
                 8,
                 "euler",
                 "normal",
                 1
             ]
@@ -269,15 +412,16 @@
                     ],
                     "name": "CLIP",
                     "slot_index": 1,
                     "type": "CLIP"
                 },
                 {
                     "links": [
-                        8
+                        8,
+                        20
                     ],
                     "name": "VAE",
                     "slot_index": 2,
                     "type": "VAE"
                 }
             ],
             "pos": [
@@ -290,132 +434,97 @@
             "size": {
                 "0": 315,
                 "1": 98
             },
             "title": "model_loader",
             "type": "CheckpointLoaderSimple",
             "widgets_values": [
-                "v1-5-pruned-emaonly.ckpt"
+                "Deliberate.ckpt"
             ]
         },
         {
             "flags": {},
-            "id": 7,
-            "inputs": [
-                {
-                    "link": 13,
-                    "name": "clip",
-                    "slot_index": 0,
-                    "type": "CLIP"
-                }
-            ],
+            "id": 11,
             "mode": 0,
-            "order": 4,
+            "order": 2,
             "outputs": [
                 {
                     "links": [
-                        6
+                        21
                     ],
-                    "name": "CONDITIONING",
+                    "name": "IMAGE",
                     "slot_index": 0,
-                    "type": "CONDITIONING"
-                }
-            ],
-            "pos": [
-                588,
-                409
-            ],
-            "properties": {
-                "Node name for S&R": "CLIPTextEncode"
-            },
-            "size": [
-                243.0001220703125,
-                90.3333740234375
-            ],
-            "title": "negative_prompt",
-            "type": "CLIPTextEncode",
-            "widgets_values": [
-                "bad hands"
-            ]
-        },
-        {
-            "flags": {},
-            "id": 6,
-            "inputs": [
-                {
-                    "link": 11,
-                    "name": "clip",
-                    "type": "CLIP"
-                }
-            ],
-            "mode": 0,
-            "order": 3,
-            "outputs": [
+                    "type": "IMAGE"
+                },
                 {
                     "links": [
-                        4
+                        19
                     ],
-                    "name": "CONDITIONING",
-                    "slot_index": 0,
-                    "type": "CONDITIONING"
+                    "name": "MASK",
+                    "slot_index": 1,
+                    "type": "MASK"
                 }
             ],
             "pos": [
-                650,
-                54
+                66,
+                755
             ],
             "properties": {
-                "Node name for S&R": "CLIPTextEncode"
+                "Node name for S&R": "LoadImage"
             },
-            "size": [
-                236.33343505859375,
-                83.00006103515625
-            ],
-            "title": "prompt",
-            "type": "CLIPTextEncode",
+            "size": {
+                "0": 315,
+                "1": 102
+            },
+            "title": "image_loader",
+            "type": "LoadImage",
             "widgets_values": [
-                "masterpiece best quality girl"
+                "example.png",
+                "image"
             ]
         },
         {
             "flags": {},
-            "id": 10,
+            "id": 14,
             "inputs": [
                 {
-                    "link": 12,
-                    "name": "clip",
-                    "type": "CLIP"
+                    "link": 21,
+                    "name": "pixels",
+                    "type": "IMAGE"
+                },
+                {
+                    "link": 20,
+                    "name": "vae",
+                    "type": "VAE"
+                },
+                {
+                    "link": 19,
+                    "name": "mask",
+                    "type": "MASK"
                 }
             ],
             "mode": 0,
-            "order": 2,
+            "order": 4,
             "outputs": [
                 {
-                    "links": [
-                        11,
-                        13
-                    ],
-                    "name": "CLIP",
-                    "slot_index": 0,
-                    "type": "CLIP"
+                    "links": null,
+                    "name": "LATENT",
+                    "type": "LATENT"
                 }
             ],
             "pos": [
-                376,
-                145
+                515,
+                758
             ],
             "properties": {
-                "Node name for S&R": "CLIPSetLastLayer"
+                "Node name for S&R": "VAEEncodeForInpaint"
             },
-            "size": [
-                210,
-                58
-            ],
-            "title": "clip_skip",
-            "type": "CLIPSetLastLayer",
-            "widgets_values": [
-                -1
-            ]
+            "size": {
+                "0": 210,
+                "1": 66
+            },
+            "title": "vae_encode",
+            "type": "VAEEncodeForInpaint"
         }
     ],
     "version": 0.4
 }
```

### Comparing `hordelib-0.1.0/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7931250000000001%*

 * *Differences: {"'11'": "OrderedDict([('inputs', OrderedDict([('image', 'example.png'), ('choose file to upload', "*

 * *         "'image')])), ('class_type', 'LoadImage')])",*

 * * "'14'": "OrderedDict([('inputs', OrderedDict([('pixels', ['11', 0]), ('vae', ['4', 2]), ('mask', "*

 * *         "['11', 1])])), ('class_type', 'VAEEncodeForInpaint')])",*

 * * "'3'": "{'inputs': {'seed': 843159458049729}}",*

 * * "'6'": "{'inputs': {'text': 'dinosaur '}}",*

 * * "'7'": "{'inputs': {'text': 'painting, drawing, artwork'}}"}*

```diff
@@ -5,14 +5,38 @@
             "clip": [
                 "4",
                 1
             ],
             "stop_at_clip_layer": -1
         }
     },
+    "11": {
+        "class_type": "LoadImage",
+        "inputs": {
+            "choose file to upload": "image",
+            "image": "example.png"
+        }
+    },
+    "14": {
+        "class_type": "VAEEncodeForInpaint",
+        "inputs": {
+            "mask": [
+                "11",
+                1
+            ],
+            "pixels": [
+                "11",
+                0
+            ],
+            "vae": [
+                "4",
+                2
+            ]
+        }
+    },
     "3": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 1.0,
             "latent_image": [
                 "5",
@@ -28,15 +52,15 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "euler",
             "scheduler": "normal",
-            "seed": 449976276651529,
+            "seed": 843159458049729,
             "steps": 20
         }
     },
     "4": {
         "class_type": "CheckpointLoaderSimple",
         "inputs": {
             "ckpt_name": "Deliberate.ckpt"
@@ -53,25 +77,25 @@
     "6": {
         "class_type": "CLIPTextEncode",
         "inputs": {
             "clip": [
                 "10",
                 0
             ],
-            "text": "masterpiece best quality girl"
+            "text": "dinosaur "
         }
     },
     "7": {
         "class_type": "CLIPTextEncode",
         "inputs": {
             "clip": [
                 "10",
                 0
             ],
-            "text": "bad hands"
+            "text": "painting, drawing, artwork"
         }
     },
     "8": {
         "class_type": "VAEDecode",
         "inputs": {
             "samples": [
                 "3",
```

### Comparing `hordelib-0.1.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7381944444444445%*

 * *Differences: {"'10'": "{'inputs': {'width': 512, 'height': 512}}",*

 * * "'11'": "{'inputs': {'seed': 1016912243210385}}",*

 * * "'17'": "OrderedDict([('inputs', OrderedDict([('stop_at_clip_layer', -1), ('clip', ['16', 1])])), "*

 * *         "('class_type', 'CLIPSetLastLayer')])",*

 * * "'18'": "OrderedDict([('inputs', OrderedDict([('image', 'example.png'), ('choose file to upload', "*

 * *         "'image')])), ('class_type', 'LoadImage')])",*

 * * "'19'": "OrderedDict([('inputs', OrderedDict([('pixels', ['18', 0]), ('vae', ['16', 2])])), "*

 * *       […]*

```diff
@@ -1,19 +1,19 @@
 {
     "10": {
         "class_type": "LatentUpscale",
         "inputs": {
             "crop": "disabled",
-            "height": 1152,
+            "height": 512,
             "samples": [
                 "3",
                 0
             ],
             "upscale_method": "nearest-exact",
-            "width": 1152
+            "width": 512
         }
     },
     "11": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 0.5,
@@ -31,15 +31,15 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "dpmpp_2m",
             "scheduler": "simple",
-            "seed": 529934750990886,
+            "seed": 1016912243210385,
             "steps": 14
         }
     },
     "12": {
         "class_type": "SaveImage",
         "inputs": {
             "filename_prefix": "ComfyUI",
@@ -64,14 +64,44 @@
     },
     "16": {
         "class_type": "CheckpointLoaderSimple",
         "inputs": {
             "ckpt_name": "Deliberate.ckpt"
         }
     },
+    "17": {
+        "class_type": "CLIPSetLastLayer",
+        "inputs": {
+            "clip": [
+                "16",
+                1
+            ],
+            "stop_at_clip_layer": -1
+        }
+    },
+    "18": {
+        "class_type": "LoadImage",
+        "inputs": {
+            "choose file to upload": "image",
+            "image": "example.png"
+        }
+    },
+    "19": {
+        "class_type": "VAEEncode",
+        "inputs": {
+            "pixels": [
+                "18",
+                0
+            ],
+            "vae": [
+                "16",
+                2
+            ]
+        }
+    },
     "3": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 1.0,
             "latent_image": [
                 "5",
@@ -87,40 +117,40 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "dpmpp_sde",
             "scheduler": "normal",
-            "seed": 222200787936635,
+            "seed": 1094518095629290,
             "steps": 12
         }
     },
     "5": {
         "class_type": "EmptyLatentImage",
         "inputs": {
             "batch_size": 1,
-            "height": 768,
-            "width": 768
+            "height": 256,
+            "width": 256
         }
     },
     "6": {
         "class_type": "CLIPTextEncode",
         "inputs": {
             "clip": [
-                "16",
-                1
+                "17",
+                0
             ],
             "text": "(masterpiece) HDR victorian portrait painting of (girl), blonde hair, mountain nature, blue sky\n"
         }
     },
     "7": {
         "class_type": "CLIPTextEncode",
         "inputs": {
             "clip": [
-                "16",
-                1
+                "17",
+                0
             ],
             "text": "bad hands, text, watermark\n"
         }
     }
 }
```

### Comparing `hordelib-0.1.0/hordelib/shared_model_manager.py` & `hordelib-0.2.0/hordelib/shared_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         # aitemplate: bool = False,
         blip: bool = False,
         clip: bool = False,
         codeformer: bool = False,
         compvis: bool = False,
         controlnet: bool = False,
         diffusers: bool = False,
-        # esrgan: bool = False,
-        # gfpgan: bool = False,
+        esrgan: bool = False,
+        gfpgan: bool = False,
         safety_checker: bool = False,
     ):
         if cls.manager is None:
             cls.manager = ModelManager()
 
         args_passed = locals().copy()
         args_passed.pop("cls")
```

### Comparing `hordelib-0.1.0/hordelib/utils/cast.py` & `hordelib-0.2.0/hordelib/utils/cast.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 T = TypeVar("T")
 
 
 def autocast_cuda(func: T, dtype: dtype = float16) -> T:
     @wraps(func)
     def wrap(*args, **kwargs):
         return amp.autocast(device_type="cuda", dtype=dtype)(no_grad()(func))(
-            *args, **kwargs
+            *args,
+            **kwargs,
         )
 
     return wrap
 
 
 def autocast_cpu(func: T, dtype: dtype = float16) -> T:
     @wraps(func)
     def wrap(*args, **kwargs):
         return amp.autocast(device_type="cpu", dtype=dtype)(no_grad()(func))(
-            *args, **kwargs
+            *args,
+            **kwargs,
         )
 
     return wrap
```

### Comparing `hordelib-0.1.0/hordelib.egg-info/PKG-INFO` & `hordelib-0.2.0/hordelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
-Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>
+Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -728,15 +728,15 @@
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
-pil_image = generate.text_to_image(data)
+pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
 ## Development
 
 Requirements:
 - `git` (install git)
@@ -806,26 +806,35 @@
 The main config files for the project are: `pyproject.toml`, `tox.ini` and `requirements.txt`
 
 ### PyPi Publishing
 
 Three steps:
 1. Bump the version in `hordelib/cosnts.py`
 1. `tox` _make sure everything works_
-1. `python publish.py` _builds the dist files_
+1. `python build_helper.py` _builds the dist files_
 1. `twine upload -r pypi dist/*`
 
 ### Updating the embedded version of ComfyUI
 
 We use a ComfyUI version pinned to a specific commit, see `hordelib/consts.py:COMFYUI_VERSION`
 
 To test if the latest version works and upgrade to it, from the project root simply:
 
-1. `cd hordelib/Comfy` _Change CWD to the embedded comfy_
+1. `cd ComfyUI` _Change CWD to the embedded comfy_
 1. `git checkout master` _Switch to master branch_
 1. `git pull` _Get the latest comfyui code_
-1. `git rev-parse HEAD` _Print the commit hash we'll need this_
-1. `cd ../../` _Get back to the hordelib project root_
+1. `git rev-parse HEAD` _Update the hash in `hordelib.consts:COMFYUI_VERSION`_
+1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
-If everything still works. Take the commit hash printed above and put it in `hordelib/consts.py:COMFYUI_VERSION`
-
 Now ComfyUI is pinned to a new version.
+
+### ComfyUI Patching
+
+It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+
+To create a patch file:
+- Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
+
+Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
+
+Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.1.0/publish.py` & `hordelib-0.2.0/build_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# build.py
+# build_helper.py
 # This is just a build helper script to build the pypi package.
 import subprocess
 
 
 def run(command):
     result = subprocess.run(command, shell=True, text=True)
     if result.returncode:
```

### Comparing `hordelib-0.1.0/tests/test_comfy_install.py` & `hordelib-0.2.0/tests/test_comfy_install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.1.0/tox.ini` & `hordelib-0.2.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 00000000: 5b74 6f78 5d0d 0a65 6e76 5f6c 6973 7420  [tox]..env_list 
-00000010: 3d0d 0a20 2020 2074 6573 7473 0d0a 0d0a  =..    tests....
-00000020: 5b74 6573 7465 6e76 5d0d 0a64 6573 6372  [testenv]..descr
-00000030: 6970 7469 6f6e 203d 2062 6173 6520 6576  iption = base ev
-00000040: 6972 6f6e 6d65 6e74 2077 6974 6820 616c  ironment with al
-00000050: 6c20 6465 7065 6e64 616e 6369 6573 0d0a  l dependancies..
-00000060: 7061 7373 656e 7620 3d0d 0a20 2020 2048  passenv =..    H
-00000070: 4f52 4445 4c49 425f 5445 5354 494e 470d  ORDELIB_TESTING.
-00000080: 0a20 2020 2041 4957 4f52 4b45 525f 4341  .    AIWORKER_CA
-00000090: 4348 455f 484f 4d45 0d0a 6465 7073 203d  CHE_HOME..deps =
-000000a0: 0d0a 2020 2020 7079 7465 7374 3e3d 370d  ..    pytest>=7.
-000000b0: 0a20 2020 2070 7974 6573 742d 7375 6761  .    pytest-suga
-000000c0: 720d 0a20 2020 2070 7974 6573 742d 636f  r..    pytest-co
-000000d0: 760d 0a20 2020 2072 6571 7565 7374 730d  v..    requests.
-000000e0: 0a20 2020 202d 7220 7265 7175 6972 656d  .    -r requirem
-000000f0: 656e 7473 2e74 7874 0d0a 0d0a 5b74 6573  ents.txt....[tes
-00000100: 7465 6e76 3a66 6f72 6d61 745d 0d0a 6465  tenv:format]..de
-00000110: 7363 7269 7074 696f 6e20 3d20 6c69 6e74  scription = lint
-00000120: 2063 6865 636b 2061 6e64 2072 6566 6f72   check and refor
-00000130: 6d61 740d 0a70 6173 7365 6e76 203d 0d0a  mat..passenv =..
-00000140: 2020 2020 484f 5244 454c 4942 5f54 4553      HORDELIB_TES
-00000150: 5449 4e47 0d0a 2020 2020 4149 574f 524b  TING..    AIWORK
-00000160: 4552 5f43 4143 4845 5f48 4f4d 450d 0a64  ER_CACHE_HOME..d
-00000170: 6570 7320 3d0d 0a20 2020 2062 6c61 636b  eps =..    black
-00000180: 3d3d 3232 2e33 2e30 0d0a 736b 6970 5f69  ==22.3.0..skip_i
-00000190: 6e73 7461 6c6c 203d 2074 7275 650d 0a63  nstall = true..c
-000001a0: 6f6d 6d61 6e64 7320 3d20 626c 6163 6b20  ommands = black 
-000001b0: 2e0d 0a0d 0a5b 7465 7374 656e 763a 636f  .....[testenv:co
-000001c0: 6d66 7975 695d 0d0a 6465 7363 7269 7074  mfyui]..descript
-000001d0: 696f 6e20 3d20 7275 6e20 636f 6d66 7975  ion = run comfyu
-000001e0: 690d 0a73 6b69 705f 696e 7374 616c 6c20  i..skip_install 
-000001f0: 3d20 7472 7565 0d0a 636f 6d6d 616e 6473  = true..commands
-00000200: 203d 0d0a 2020 2020 7b65 6e76 7079 7468   =..    {envpyth
-00000210: 6f6e 7d20 2d6d 2068 6f72 6465 6c69 622e  on} -m hordelib.
-00000220: 7275 6e5f 636f 6d66 7975 690d 0a0d 0a5b  run_comfyui....[
-00000230: 7465 7374 656e 763a 7465 7374 735d 0d0a  testenv:tests]..
-00000240: 6465 7363 7269 7074 696f 6e20 3d20 696e  description = in
-00000250: 7374 616c 6c20 7079 7465 7374 2069 6e20  stall pytest in 
-00000260: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
-00000270: 6e6d 656e 7420 616e 6420 696e 766f 6b65  nment and invoke
-00000280: 2069 7420 6f6e 2074 6865 2074 6573 7473   it on the tests
-00000290: 2066 6f6c 6465 720d 0a70 6173 7365 6e76   folder..passenv
-000002a0: 203d 0d0a 2020 2020 484f 5244 454c 4942   =..    HORDELIB
-000002b0: 5f54 4553 5449 4e47 0d0a 2020 2020 4149  _TESTING..    AI
-000002c0: 574f 524b 4552 5f43 4143 4845 5f48 4f4d  WORKER_CACHE_HOM
-000002d0: 450d 0a63 6f6d 6d61 6e64 7320 3d0d 0a20  E..commands =.. 
-000002e0: 2020 2070 7974 6573 7420 7465 7374 7320     pytest tests 
-000002f0: 7b70 6f73 6172 6773 7d20 2d2d 636f 7620  {posargs} --cov 
-00000300: 2d2d 636f 762d 7265 706f 7274 3d74 6572  --cov-report=ter
-00000310: 6d20 2d2d 636f 762d 7265 706f 7274 3d6c  m --cov-report=l
-00000320: 636f 760d 0a                             cov..
+00000010: 3d0d 0a20 2020 2066 6f72 6d61 740d 0a20  =..    format.. 
+00000020: 2020 2074 6573 7473 0d0a 0d0a 5b74 6573     tests....[tes
+00000030: 7465 6e76 5d0d 0a64 6573 6372 6970 7469  tenv]..descripti
+00000040: 6f6e 203d 2062 6173 6520 6576 6972 6f6e  on = base eviron
+00000050: 6d65 6e74 2077 6974 6820 616c 6c20 6465  ment with all de
+00000060: 7065 6e64 616e 6369 6573 0d0a 7061 7373  pendancies..pass
+00000070: 656e 7620 3d0d 0a20 2020 2048 4f52 4445  env =..    HORDE
+00000080: 4c49 425f 5445 5354 494e 470d 0a20 2020  LIB_TESTING..   
+00000090: 2041 4957 4f52 4b45 525f 4341 4348 455f   AIWORKER_CACHE_
+000000a0: 484f 4d45 0d0a 6465 7073 203d 0d0a 2020  HOME..deps =..  
+000000b0: 2020 7079 7465 7374 3e3d 370d 0a20 2020    pytest>=7..   
+000000c0: 2070 7974 6573 742d 7375 6761 720d 0a20   pytest-sugar.. 
+000000d0: 2020 2070 7974 6573 742d 636f 760d 0a20     pytest-cov.. 
+000000e0: 2020 2072 6571 7565 7374 730d 0a20 2020     requests..   
+000000f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
+00000100: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
+00000110: 3a66 6f72 6d61 745d 0d0a 6465 7363 7269  :format]..descri
+00000120: 7074 696f 6e20 3d20 6368 6563 6b20 666f  ption = check fo
+00000130: 726d 6174 7469 6e67 2072 756c 6573 0d0a  rmatting rules..
+00000140: 6465 7073 203d 0d0a 2020 2020 626c 6163  deps =..    blac
+00000150: 6b3d 3d32 322e 332e 300d 0a73 6b69 705f  k==22.3.0..skip_
+00000160: 696e 7374 616c 6c20 3d20 7472 7565 0d0a  install = true..
+00000170: 636f 6d6d 616e 6473 203d 2062 6c61 636b  commands = black
+00000180: 202d 2d63 6865 636b 202e 0d0a 0d0a 5b74   --check .....[t
+00000190: 6573 7465 6e76 3a6c 696e 745d 0d0a 6465  estenv:lint]..de
+000001a0: 7363 7269 7074 696f 6e20 3d20 6368 6563  scription = chec
+000001b0: 6b20 6c69 6e74 696e 6720 7275 6c65 730d  k linting rules.
+000001c0: 0a64 6570 7320 3d0d 0a20 2020 2072 7566  .deps =..    ruf
+000001d0: 663d 3d30 2e30 2e32 3631 0d0a 736b 6970  f==0.0.261..skip
+000001e0: 5f69 6e73 7461 6c6c 203d 2074 7275 650d  _install = true.
+000001f0: 0a63 6f6d 6d61 6e64 7320 3d20 7275 6666  .commands = ruff
+00000200: 202e 0d0a 0d0a 5b74 6573 7465 6e76 3a73   .....[testenv:s
+00000210: 6f72 7469 6d70 6f72 7473 5d0d 0a64 6573  ortimports]..des
+00000220: 6372 6970 7469 6f6e 203d 2063 6865 636b  cription = check
+00000230: 206c 696e 7469 6e67 2072 756c 6573 0d0a   linting rules..
+00000240: 6465 7073 203d 0d0a 2020 2020 7275 6666  deps =..    ruff
+00000250: 3d3d 302e 302e 3236 310d 0a73 6b69 705f  ==0.0.261..skip_
+00000260: 696e 7374 616c 6c20 3d20 7472 7565 0d0a  install = true..
+00000270: 636f 6d6d 616e 6473 203d 2072 7566 6620  commands = ruff 
+00000280: 2d2d 6669 7820 2d2d 6578 636c 7564 6520  --fix --exclude 
+00000290: 636f 6d66 795f 686f 7264 652e 7079 202d  comfy_horde.py -
+000002a0: 2d73 656c 6563 7420 4930 3031 202e 0d0a  -select I001 ...
+000002b0: 0d0a 5b74 6573 7465 6e76 3a63 6f6d 6679  ..[testenv:comfy
+000002c0: 7569 5d0d 0a64 6573 6372 6970 7469 6f6e  ui]..description
+000002d0: 203d 2072 756e 2063 6f6d 6679 7569 0d0a   = run comfyui..
+000002e0: 736b 6970 5f69 6e73 7461 6c6c 203d 2074  skip_install = t
+000002f0: 7275 650d 0a63 6f6d 6d61 6e64 7320 3d0d  rue..commands =.
+00000300: 0a20 2020 207b 656e 7670 7974 686f 6e7d  .    {envpython}
+00000310: 202d 6d20 686f 7264 656c 6962 2e72 756e   -m hordelib.run
+00000320: 5f63 6f6d 6679 7569 0d0a 0d0a 5b74 6573  _comfyui....[tes
+00000330: 7465 6e76 3a74 6573 7473 5d0d 0a64 6573  tenv:tests]..des
+00000340: 6372 6970 7469 6f6e 203d 2069 6e73 7461  cription = insta
+00000350: 6c6c 2070 7974 6573 7420 696e 2061 2076  ll pytest in a v
+00000360: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
+00000370: 6e74 2061 6e64 2069 6e76 6f6b 6520 6974  nt and invoke it
+00000380: 206f 6e20 7468 6520 7465 7374 7320 666f   on the tests fo
+00000390: 6c64 6572 0d0a 7061 7373 656e 7620 3d0d  lder..passenv =.
+000003a0: 0a20 2020 2048 4f52 4445 4c49 425f 5445  .    HORDELIB_TE
+000003b0: 5354 494e 470d 0a20 2020 2041 4957 4f52  STING..    AIWOR
+000003c0: 4b45 525f 4341 4348 455f 484f 4d45 0d0a  KER_CACHE_HOME..
+000003d0: 636f 6d6d 616e 6473 203d 0d0a 2020 2020  commands =..    
+000003e0: 7079 7465 7374 2074 6573 7473 207b 706f  pytest tests {po
+000003f0: 7361 7267 737d 202d 2d63 6f76 202d 2d63  sargs} --cov --c
+00000400: 6f76 2d72 6570 6f72 743d 7465 726d 202d  ov-report=term -
+00000410: 2d63 6f76 2d72 6570 6f72 743d 6c63 6f76  -cov-report=lcov
+00000420: 0d0a                                     ..
```

