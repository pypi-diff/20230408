# Comparing `tmp/magnify-0.1.9.tar.gz` & `tmp/magnify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.1.9.tar", max compression
+gzip compressed data, was "magnify-0.2.0.tar", max compression
```

## Comparing `magnify-0.1.9.tar` & `magnify-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.1.9/README.md
--rw-r--r--   0        0        0     1536 2023-03-28 00:19:31.749722 magnify-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      173 2023-03-28 00:19:26.481594 magnify-0.1.9/src/magnify/__init__.py
--rw-r--r--   0        0        0    23893 2023-03-27 23:58:18.530971 magnify-0.1.9/src/magnify/find.py
--rw-r--r--   0        0        0     1236 2023-03-27 23:57:26.857735 magnify-0.1.9/src/magnify/pipeline.py
--rw-r--r--   0        0        0      936 2023-03-27 23:48:43.833100 magnify-0.1.9/src/magnify/preprocess.py
--rw-r--r--   0        0        0     9092 2023-03-27 23:53:28.108034 magnify-0.1.9/src/magnify/reader.py
--rw-r--r--   0        0        0      988 2023-03-27 23:48:32.776831 magnify-0.1.9/src/magnify/registry.py
--rw-r--r--   0        0        0     1183 2023-03-27 23:48:09.076253 magnify-0.1.9/src/magnify/stitch.py
--rw-r--r--   0        0        0     1411 2023-03-27 21:04:09.485286 magnify-0.1.9/src/magnify/utils.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 magnify-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.0/README.md
+-rw-r--r--   0        0        0     1601 2023-04-07 23:32:37.299062 magnify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-04-07 23:32:44.975245 magnify-0.2.0/src/magnify/__init__.py
+-rw-r--r--   0        0        0    24452 2023-04-07 23:31:26.665378 magnify-0.2.0/src/magnify/find.py
+-rw-r--r--   0        0        0     1406 2023-04-07 22:21:05.340362 magnify-0.2.0/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      158 2023-04-07 22:03:32.255470 magnify-0.2.0/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1467 2023-04-07 21:54:53.107240 magnify-0.2.0/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    12742 2023-04-07 23:14:57.561770 magnify-0.2.0/src/magnify/reader.py
+-rw-r--r--   0        0        0     3084 2023-04-07 23:19:37.400458 magnify-0.2.0/src/magnify/registry.py
+-rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.0/src/magnify/stitch.py
+-rw-r--r--   0        0        0     1583 2023-03-28 01:44:15.928665 magnify-0.2.0/src/magnify/utils.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.0/PKG-INFO
```

### Comparing `magnify-0.1.9/pyproject.toml` & `magnify-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.1.9"
+version = "0.2.0"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
@@ -17,14 +17,17 @@
 pandas = "^1.3.0"
 tifffile = ">=2021.11.2"
 tqdm = "^4.64"
 types-tqdm = "^4.64"
 xarray = {extras = ["complete"], version = ">=2023.01.0"}
 dask = {extras = ["complete"], version = ">=2022.02.0"}
 catalogue = "^2.0.8"
+beautifulsoup4 = "^4.10.0"
+lxml = "^4.6.0"
+confection = "^0.0.4"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.6.0"
 mypy = "^1.0.1"
 pytest = ">=7.1.2"
 ruff = ">=0.0.249"
 sphinx = "^5.0.2"
```

### Comparing `magnify-0.1.9/src/magnify/find.py` & `magnify-0.2.0/src/magnify/find.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,46 +15,31 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ButtonFinder:
     def __init__(
         self,
-        row_dist: float = 126.3,
-        col_dist: float = 233.2,
+        row_dist: float = 375 / 3.22,
+        col_dist: float = 655 / 3.22,
         min_button_radius: int = 4,
         max_button_radius: int = 15,
         cluster_penalty: float = 10,
-        region_length: int = 61,
-    ):
-        self.row_dist = row_dist
-        self.col_dist = col_dist
-        self.min_button_radius = min_button_radius
-        self.max_button_radius = max_button_radius
-        self.cluster_penalty = cluster_penalty
-        self.region_length = region_length
-
-    def __call__(
-        self,
-        assay: xr.Dataset,
-        row_dist: float = 126.3,
-        col_dist: float = 233.2,
-        min_button_radius: int = 4,
-        max_button_radius: int = 15,
-        cluster_penalty: float = 10,
-        region_length: int = 61,
+        roi_length: int = 61,
         progress_bar: bool = False,
-    ) -> xr.Dataset:
+    ):
         self.row_dist = row_dist
         self.col_dist = col_dist
         self.min_button_radius = min_button_radius
         self.max_button_radius = max_button_radius
         self.cluster_penalty = cluster_penalty
-        self.region_length = region_length
+        self.roi_length = roi_length
+        self.progress_bar = progress_bar
 
+    def __call__(self, assay: xr.Dataset) -> xr.Dataset:
         num_rows, num_cols = assay.id.shape
         if isinstance(assay.search_channel, str):
             if assay.search_channel in assay.channel:
                 search_channels = [assay.search_channel]
             elif assay.search_channel == "all":
                 search_channels = assay.channel
             else:
@@ -64,67 +49,67 @@
             search_channels = assay.search_channel
         min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
         if min_button_dist % 2 == 0:
             # Certain opencv functions require an odd blocksize.
             min_button_dist -= 1
 
         # Create the array of subimage regions.
-        regions = da.empty(
+        roi = da.empty(
             (
                 num_rows,
                 num_cols,
                 assay.dims["channel"],
                 assay.dims["time"],
-                self.region_length,
-                self.region_length,
+                self.roi_length,
+                self.roi_length,
             ),
             dtype=assay.image.dtype,
             chunks=(
                 1,
                 1,
                 assay.dims["channel"],
                 assay.dims["time"],
-                self.region_length,
-                self.region_length,
+                self.roi_length,
+                self.roi_length,
             ),
         )
         assay = assay.assign(
-            region=(
-                ("marker_row", "marker_col", "channel", "time", "row", "col"),
-                regions,
+            roi=(
+                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
+                roi,
             ),
             fg=(
-                ("marker_row", "marker_col", "channel", "time", "row", "col"),
+                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
                 da.empty_like(
-                    regions,
+                    roi,
                     dtype=bool,
                 ),
             ),
             bg=(
-                ("marker_row", "marker_col", "channel", "time", "row", "col"),
+                ("marker_row", "marker_col", "channel", "time", "roi_y", "roi_x"),
                 da.empty_like(
-                    regions,
+                    roi,
                     dtype=bool,
                 ),
             ),
         )
         # Create the x and y coordinates arrays for each button.
-        assay = assay.assign_coords(
+        assay = assay.assign(
             x=(
-                ["marker_row", "marker_col", "time"],
+                ("marker_row", "marker_col", "time"),
                 np.empty((num_rows, num_cols, assay.dims["time"])),
             ),
             y=(
-                ["marker_row", "marker_col", "time"],
+                ("marker_row", "marker_col", "time"),
                 np.empty((num_rows, num_cols, assay.dims["time"])),
             ),
         )
 
         # Run the button finding algorithm for each timestep.
-        for t, time in enumerate(tqdm.tqdm(assay.time, disable=not progress_bar)):
+        for t, time in enumerate(tqdm.tqdm(assay.time, disable=not self.progress_bar)):
             # Preload all images for this timnepoint so we only read from disk once.
             images = assay.image.sel(time=time).to_numpy()
             points = np.empty((0, 2))
             for channel in search_channels:
                 c = np.where(assay.channel == channel)[0][0]
                 image = utils.to_uint8(images[c])
                 # Step 1: Find an imperfect button mask by thresholding.
@@ -214,86 +199,90 @@
             assay.y[..., t] = (
                 row_slope * col_intercepts[np.newaxis] + row_intercepts[:, np.newaxis]
             ) / (1 - row_slope * col_slope)
             assay.x[..., t] = assay.y[..., t] * col_slope + col_intercepts[np.newaxis]
 
             # Step 6: Extract a region around each button.
             offsets = np.empty((num_rows, num_cols, 2), dtype=int)
-            regions = np.empty(
-                (num_rows, num_cols, assay.dims["channel"], self.region_length, self.region_length),
-                dtype=assay.region.dtype,
+            roi = np.empty(
+                (num_rows, num_cols, assay.dims["channel"], self.roi_length, self.roi_length),
+                dtype=assay.roi.dtype,
             )
             for i in range(num_rows):
                 for j in range(num_cols):
                     top, bottom, left, right = utils.bounding_box(
                         round(float(assay.x[i, j, t])),
                         round(float(assay.y[i, j, t])),
-                        self.region_length,
-                        assay.dims["im_row"],
-                        assay.dims["im_col"],
+                        self.roi_length,
+                        assay.sizes["im_y"],
+                        assay.sizes["im_x"],
                     )
-                    regions[i, j] = images[:, top:bottom, left:right]
+                    roi[i, j] = images[:, top:bottom, left:right]
                     offsets[i, j] = [left, top]
-            assay.region[:, :, :, t] = regions
+            assay.roi[:, :, :, t] = roi
 
             # Step 7: Compute the foreground and background masks for all buttons.
             fg = np.empty(
-                (num_rows, num_cols, assay.dims["channel"], self.region_length, self.region_length),
+                (num_rows, num_cols, assay.dims["channel"], self.roi_length, self.roi_length),
                 dtype=bool,
             )
             bg = np.empty_like(fg)
             for i in range(num_rows):
                 for j in range(num_cols):
                     # TODO: This step should occur over multiple channels.
                     c = np.where(assay.channel == search_channels[0])[0][0]
-                    subimage = utils.to_uint8(regions[i, j, c])
-                    # Filter the subimage to smooth edges and remove noise.
-                    filtered = cv.bilateralFilter(
-                        subimage,
-                        d=9,
-                        sigmaColor=75,
-                        sigmaSpace=75,
-                        borderType=cv.BORDER_DEFAULT,
-                    )
+                    subimage = utils.to_uint8(roi[i, j, c])
 
-                    # Find any circles in the subimage.
-                    circles = cv.HoughCircles(
-                        filtered,
-                        method=cv.HOUGH_GRADIENT,
-                        dp=1,
-                        minDist=50,
-                        param1=20,
-                        param2=5,
-                        minRadius=self.min_button_radius,
-                        maxRadius=self.max_button_radius,
-                    )
+                    # Find circles to refine our button estimate unless we have a blank chamber.
+                    circles = None
+                    if assay.id[i, j] != "":
+                        # Filter the subimage to smooth edges and remove noise.
+                        filtered = cv.bilateralFilter(
+                            subimage,
+                            d=9,
+                            sigmaColor=75,
+                            sigmaSpace=75,
+                            borderType=cv.BORDER_DEFAULT,
+                        )
+
+                        # Find any circles in the subimage.
+                        circles = cv.HoughCircles(
+                            filtered,
+                            method=cv.HOUGH_GRADIENT,
+                            dp=1,
+                            minDist=50,
+                            param1=20,
+                            param2=5,
+                            minRadius=self.min_button_radius,
+                            maxRadius=self.max_button_radius,
+                        )
 
                     # Update our estimate of the button position if we found some circles.
                     if circles is not None:
                         circles = circles[0, :, :2]
                         point = np.array([assay.x[i, j, t], assay.y[i, j, t]]) - offsets[i, j]
                         # Use the circle center closest to our previous estimate of the button.
                         closest_idx = np.argmin(np.linalg.norm(circles - point, axis=1))
                         assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx] + offsets[i, j]
 
                     x_rel = round(float(assay.x[i, j, t])) - offsets[i, j, 0]
                     y_rel = round(float(assay.y[i, j, t])) - offsets[i, j, 1]
 
                     # Set the foreground (the button) to be a circle of fixed radius.
                     fg_mask = utils.circle(
-                        self.region_length,
+                        self.roi_length,
                         row=y_rel,
                         col=x_rel,
                         radius=self.max_button_radius,
                         value=True,
                     )
 
                     # Set the background to be the annulus around our foreground.
                     bg_mask = utils.circle(
-                        self.region_length,
+                        self.roi_length,
                         row=y_rel,
                         col=x_rel,
                         radius=2 * self.max_button_radius,
                         value=True,
                     )
                     bg_mask &= ~fg_mask
 
@@ -317,50 +306,57 @@
 
                     fg[i, j] = fg_mask
                     bg[i, j] = bg_mask
 
             assay.fg[:, :, :, t] = fg
             assay.bg[:, :, :, t] = bg
 
+        assay = assay.stack(marker=("marker_row", "marker_col"), create_index=True).transpose(
+            "marker", ...
+        )
+        assay = assay.set_xindex("id")
+
         return assay
 
     @registry.components.register("find_buttons")
-    def make():
-        return ButtonFinder()
+    def make(
+        row_dist: float = 375 / 3.22,
+        col_dist: float = 655 / 3.22,
+        min_button_radius: int = 4,
+        max_button_radius: int = 15,
+        cluster_penalty: float = 10,
+        roi_length: int = 61,
+        progress_bar: bool = False,
+    ):
+        return ButtonFinder(
+            row_dist=row_dist,
+            col_dist=col_dist,
+            min_button_radius=min_button_radius,
+            cluster_penalty=cluster_penalty,
+            roi_length=roi_length,
+            progress_bar=progress_bar,
+        )
 
 
 class BeadFinder:
     def __init__(
         self,
         min_bead_radius: int = 10,
         max_bead_radius: int = 30,
-        region_length: int = 61,
+        roi_length: int = 61,
         param1: int = 50,
         param2: int = 30,
     ):
         self.min_bead_radius = min_bead_radius
         self.max_bead_radius = max_bead_radius
-        self.region_length = region_length
+        self.roi_length = roi_length
         self.param1 = param1
         self.param2 = param2
 
-    def __call__(
-        self,
-        assay: xr.Dataset,
-        min_bead_radius: int = 10,
-        max_bead_radius: int = 30,
-        region_length: int = 61,
-        param1: int = 50,
-        param2: int = 30,
-    ) -> xr.Dataset:
-        self.min_bead_radius = min_bead_radius
-        self.max_bead_radius = max_bead_radius
-        self.region_length = region_length
-        self.param1 = param1
-        self.param2 = param2
+    def __call__(self, assay: xr.Dataset) -> xr.Dataset:
         if isinstance(assay.search_channel, str):
             if assay.search_channel in assay.channel:
                 search_channels = [assay.search_channel]
             elif assay.search_channel == "all":
                 search_channels = assay.channel
             else:
                 raise ValueError(f"{assay.search_channel} is not a channel name.")
@@ -409,101 +405,118 @@
                     radii = np.concatenate([radii, circles[valid, 2]])
 
         # Update the assay object with the beads we found.
         if len(centers) > 0:
             num_beads = len(centers)
             # Create the array of subimage regions.
             assay = assay.assign(
-                region=(
-                    ("marker", "channel", "time", "row", "col"),
+                roi=(
+                    ("marker", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
-                            self.region_length,
-                            self.region_length,
+                            self.roi_length,
+                            self.roi_length,
                         ),
                         dtype=assay.image.dtype,
                     ),
                 ),
                 fg=(
-                    ("marker", "channel", "time", "row", "col"),
+                    ("marker", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
-                            self.region_length,
-                            self.region_length,
+                            self.roi_length,
+                            self.roi_length,
                         ),
                         dtype=bool,
                     ),
                 ),
                 bg=(
-                    ("marker", "channel", "time", "row", "col"),
+                    ("marker", "channel", "time", "roi_y", "roi_x"),
                     np.empty(
                         (
                             num_beads,
                             assay.dims["channel"],
                             assay.dims["time"],
-                            self.region_length,
-                            self.region_length,
+                            self.roi_length,
+                            self.roi_length,
                         ),
                         dtype=bool,
                     ),
                 ),
             )
-            assay = assay.assign_coords(
+            assay = assay.assign(
                 x=(
                     ["marker", "time"],
                     np.repeat(centers[:, np.newaxis, 0], assay.dims["time"], axis=1),
                 ),
                 y=(
                     ["marker", "time"],
                     np.repeat(centers[:, np.newaxis, 1], assay.dims["time"], axis=1),
                 ),
             )
 
+            rois = np.empty(assay.roi.shape, dtype=assay.roi.dtype)
+            fgs = np.empty(assay.roi.shape, dtype=bool)
+            bgs = np.empty(assay.roi.shape, dtype=bool)
+            image = assay.image.to_numpy()
             # Compute the foreground and background masks for all buttons.
             for i in range(num_beads):
                 # Set the subimage region for this bead.
                 top, bottom, left, right = utils.bounding_box(
                     round(float(assay.x[i, 0])),
                     round(float(assay.y[i, 0])),
-                    self.region_length,
+                    self.roi_length,
                     image.shape[-2],
                     image.shape[-1],
                 )
-                assay.region[i] = assay.image.sel(
-                    im_row=slice(top, bottom), im_col=slice(left, right)
-                )
+                rois[i] = image[..., top:bottom, left:right]
 
                 # Set the foreground of the bead to be the circle we found.
                 fg_mask = utils.circle(
-                    self.region_length,
+                    self.roi_length,
                     row=round(float(assay.y[i, 0] - top)),
                     col=round(float(assay.x[i, 0] - left)),
                     radius=round(radii[i]),
                     value=True,
                 )
 
                 # Set the background to be everything else in the region,
                 # which could include other beads.
                 bg_mask = ~fg_mask
 
                 # Set the masked arrays with our computed masks.
-                assay.fg[i] = fg_mask
-                assay.bg[i] = bg_mask
+                fgs[i] = fg_mask
+                bgs[i] = bg_mask
 
+        assay.fg[:] = fgs
+        assay.bg[:] = bgs
+        assay.roi[:] = rois
         return assay
 
     @registry.components.register("find_beads")
-    def make():
-        return BeadFinder()
+    def make(
+        min_bead_radius: int = 10,
+        max_bead_radius: int = 30,
+        roi_length: int = 61,
+        param1: int = 50,
+        param2: int = 30,
+    ):
+        return BeadFinder(
+            min_bead_radius=min_bead_radius,
+            max_bead_radius=max_bead_radius,
+            roi_length=roi_length,
+            param1=param1,
+            param2=param2,
+        )
 
 
 def cluster_1d(
     points: np.ndarray,
     total_length: int,
     num_clusters: int,
     cluster_length: float,
```

### Comparing `magnify-0.1.9/src/magnify/pipeline.py` & `magnify-0.2.0/src/magnify/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from __future__ import annotations
 from typing import Callable
 
+import confection
 from numpy.typing import ArrayLike
 import xarray as xr
 
 import magnify.registry as registry
 import magnify.utils as utils
 
 
 class Pipeline:
-    def __init__(self, reader: str):
+    def __init__(self, reader: str, config: dict[str, dict[str, str]]):
         self.reader: Callable[[ArrayLike | str], xr.Dataset] = registry.readers.get(reader)()
+        self.config = confection.Config(config)
         self.components: list[Callable[[xr.Dataset], xr.Dataset]] = []
 
     def __call__(
         self,
         data: ArrayLike | str,
         names: ArrayLike | str = None,
         search_on: str = "egfp",
         times: Sequence[int] | None = None,
         channels: Sequence[str] | None = None,
-        **kwargs,
     ) -> xr.Dataset | list[xr.Dataset]:
         inputs = self.reader(
             data=data, names=names, search_on=search_on, times=times, channels=channels
         )
         assays = []
         for assay in inputs:
             for name, component in self.components:
-                assay = component(assay, **utils.valid_kwargs(kwargs, component))
+                assay = component(assay)
 
             assays.append(assay)
 
         if len(assays) == 1:
             assays = assays[0]
 
         return assays
 
     def add_pipe(self, name: str) -> None:
-        self.components.append((name, registry.components.get(name)()))
+        component_factory = registry.components.get(name)
+        component = component_factory(**utils.valid_kwargs(self.config, component_factory))
+        self.components.append((name, component))
```

### Comparing `magnify-0.1.9/src/magnify/preprocess.py` & `magnify-0.2.0/src/magnify/preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 from typing import cast
+import os
 
 import basicpy
+import tifffile
 import numpy as np
 import xarray as xr
 
 import magnify.registry as registry
 
 
 class Preprocessor:
@@ -18,14 +20,27 @@
         return assay
 
     @registry.components.register("preprocess")
     def make():
         return Preprocessor()
 
 
-@registry.components.register("flip_horizontal")
-def make_horizontal_flip():
-    def horizontal_flip(assay: xr.Dataset):
-        assay["image"] = assay.image.isel(im_col=slice(None, None, -1))
-        return assay
-
-    return horizontal_flip
+@registry.component("flatfield_correct")
+def flatfield_correct(assay: xr.Dataset, flatfield=1.0, darkfield=0.0):
+    if isinstance(flatfield, str):
+        with tifffile.TiffFile(os.path.expanduser(flatfield)) as tif:
+            flatfield = tif.asarray()
+    if isinstance(darkfield, str):
+        with tifffile.TiffFile(os.path.expanduser(darkfield)) as tif:
+            darkfield = tif.asarray()
+
+    assay["tile"] = (assay.tile - darkfield) / flatfield
+    return assay
+
+
+@registry.component("horizontal_flip")
+def horizontal_flip(assay: xr.Dataset):
+    if "image" in assay:
+        assay["image"] = assay.image.isel(im_x=slice(None, None, -1))
+    else:
+        assay["tile"] = assay.tile.isel(tile_x=slice(None, None, -1))
+    return assay
```

### Comparing `magnify-0.1.9/src/magnify/reader.py` & `magnify-0.2.0/src/magnify/reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 from collections.abc import Iterator
 import collections
 import datetime
 import fnmatch
+import functools
 import glob
 import os
 import re
 
 from numpy.typing import ArrayLike
 from typing import Iterator
+import bs4
 import dask.array as da
 import numpy as np
 import pandas as pd
 import tifffile
 import xarray as xr
 
 from magnify.pipeline import Pipeline
 import magnify.registry as registry
+import magnify.utils as utils
 
 
 class Reader:
     def __init__(self) -> None:
         pass
 
     def __call__(
@@ -35,15 +38,17 @@
             data = [data]
 
         for d in data:
             path_dict = extract_paths(d)
             if len(path_dict) == 0:
                 raise FileNotFoundError(f"The pattern {d} did not lead to any files.")
 
-            for assay_name, assay_dict in path_dict.items():
+            for assay_name, assay_dict in sorted(
+                path_dict.items(), key=lambda x: utils.natural_sort_key(x[0])
+            ):
                 # Use these variables within the loop so we don't affect other assays.
                 channel_coords = channels
                 time_coords = times
 
                 # Get the indices specified in the path each in sorted order.
                 channel_idxs, time_idxs, row_idxs, col_idxs = (
                     sorted(set(idx)) for idx in zip(*assay_dict.keys())
@@ -69,115 +74,174 @@
                 if time_coords is None and "time" in dims_in_path:
                     time_coords = time_idxs
                 if channel_coords is None and "channel" in dims_in_path:
                     channel_coords = channel_idxs
 
                 # Read in a single image to get the metadata stored within the file.
                 with tifffile.TiffFile(next(iter(assay_dict.values()))) as tif:
+                    dtype = tif.series[0].dtype
+                    inner_shape = tif.series[0].shape
+                    page_shape = tif.pages[0].shape
+
                     letter_to_dim = {
                         "C": "channel",
                         "T": "time",
                         "Z": "depth",
-                        "Y": "im_row",
-                        "X": "im_col",
+                        "Y": "tile_y",
+                        "X": "tile_x",
+                        "R": "tile_pos",
                     }
                     dims_in_file = [letter_to_dim[c] for c in tif.series[0].axes]
 
-                    if channel_coords is None and "channel" in dims_in_file:
+                    if (
+                        time_coords is None
+                        and tif.is_micromanager
+                        and "StartTime" in tif.micromanager_metadata["Summary"]
+                    ):
+                        # Get the time string without timezone info.
+                        time_str = tif.micromanager_metadata["Summary"]["StartTime"][:-6]
+                        start_time = datetime.datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S.%f")
+                        if "time" in dims_in_file:
+                            # Only look at the first file's description since time isn't across multiple files.
+                            planes = [
+                                pl
+                                for pl in bs4.BeautifulSoup(tif.pages[0].description, "xml")
+                                .find("Image")
+                                .find_all("Plane")
+                            ]
+                            assert all(pl.get("DeltaTUnit") == "ms" for pl in planes)
+                            time_coords = [
+                                start_time
+                                + datetime.timedelta(milliseconds=float(pl.get("DeltaT")))
+                                for pl in planes
+                            ]
+                            if "channel" in dims_in_file:
+                                stride = inner_shape[dims_in_file.index("channel")]
+                            else:
+                                stride = 1
+                            assert len(time_coords) % stride == 0
+                            time_coords = time_coords[::stride]
+                        else:
+                            time_coords = [start_time]
+                    if channel_coords is None and tif.is_micromanager:
                         channel_coords = tif.micromanager_metadata["Summary"]["ChNames"]
 
-                    if "time" in dims_in_file:
-                        raise ValueError("tiff files with a time dimension are not yet supported.")
+                    if "tile_pos" in dims_in_file:
+                        # Tiles are always saved in multiple files so ignore this dimension
+                        # since the user should specify tiles in their search path.
+                        tile_idx = dims_in_file.index("tile_pos")
+                        inner_shape = inner_shape[:tile_idx] + inner_shape[tile_idx + 1 :]
+                        dims_in_file = dims_in_file[:tile_idx] + dims_in_file[tile_idx + 1 :]
+
                     if "depth" in dims_in_file:
                         raise ValueError("tiff files with a Z dimension are not yet supported.")
-                    if "im_row" not in dims_in_file or "im_col" not in dims_in_file:
+                    if "tile_y" not in dims_in_file or "tile_x" not in dims_in_file:
                         raise ValueError("tiff files must contain an X and Y dimension.")
 
-                    dtype = tif.series[0].dtype
-                    inner_shape = tif.series[0].shape
-
                 # Check the dimensions specified in the path and inside the tiff file do not overlap.
                 if set(dims_in_file).intersection(dims_in_path):
                     raise ValueError(
                         "Dimensions specified in the path names and inside the tiff file overlap."
                     )
 
-                # Setup a dask array to lazyload images.
+                # Setup a dask array to lazyload image tiles.
                 filenames = [path for _, path in sorted(assay_dict.items())]
 
-                def read_image(block_id):
-                    block_id = block_id[: len(outer_shape)]
-                    idx = np.ravel_multi_index(block_id, outer_shape)
-                    with tifffile.TiffFile(filenames[idx]) as tif:
-                        return np.expand_dims(tif.asarray(), axis=tuple(range(len(block_id))))
-
-                # Chunk the images so that each chunk represents a single file.
-                images = da.map_blocks(
-                    read_image,
+                def read_tile(block_id, filenames):
+                    outer_id = block_id[: len(outer_shape)]
+                    inner_id = block_id[len(outer_shape) :]
+                    if len(outer_id) > 0:
+                        file_idx = np.ravel_multi_index(outer_id, outer_shape)
+                    else:
+                        # This is the case where we don't have indices outside the file.
+                        file_idx = 0
+
+                    with tifffile.TiffFile(filenames[file_idx]) as tif:
+                        page_ndim = len(page_shape)
+                        if len(inner_shape) > page_ndim:
+                            page_idx = np.ravel_multi_index(
+                                inner_id[:-page_ndim], inner_shape[:-page_ndim]
+                            )
+                        else:
+                            # This is the case where no dimensions correspond to page dims.
+                            page_idx = 0
+                        # Read the page from disk.
+                        page = tif.pages[page_idx].asarray()
+                        # Expand the dimensions of the block to incorporate outer dims and page index dims.
+                        return np.expand_dims(page, axis=tuple(range(len(block_id) - page_ndim)))
+
+                # Chunk the images so that each chunk represents a single page in the tiff file.
+                tiles = da.map_blocks(
+                    functools.partial(read_tile, filenames=filenames),
                     dtype=dtype,
-                    chunks=((tuple((1,) * size for size in outer_shape) + inner_shape)),
+                    chunks=(
+                        (
+                            tuple((1,) * size for size in outer_shape)
+                            + tuple((1,) * size for size in inner_shape[: -len(page_shape)])
+                            + inner_shape[-len(page_shape) :]
+                        )
+                    ),
                 )
 
-                # Set named coordinates for channels and times if they're available.
                 coords = {}
+                # Set named coordinates for channels and times if they're available.
                 if channel_coords is not None:
                     coords["channel"] = channel_coords
                 if time_coords is not None:
                     coords["time"] = time_coords
 
                 # Put all our data into an xarray dataset.
                 assay = xr.Dataset(
-                    {"image": (dims_in_path + dims_in_file, images)},
+                    {"tile": (dims_in_path + dims_in_file, tiles)},
                     coords=coords,
                     attrs={
                         "name": assay_name,
                         "search_channel": search_on,
                     },
                 )
 
                 # Make sure the assay always has a time and channel dimension.
                 if "channel" not in assay.dims:
                     assay = assay.expand_dims("channel", 0)
                 if "time" not in assay.dims:
                     assay = assay.expand_dims("time", 1)
 
-                # Reorder the dimensions so they're always consistent.
-                desired_order = []
-                for dim in ["channel", "time", "tile_row", "tile_col", "im_row", "im_col"]:
-                    if dim in assay.dims:
-                        desired_order.append(dim)
-                assay.transpose(*desired_order)
+                # Reorder the dimensions so they're always consistent and add missing dimensions.
+                desired_order = ["channel", "time", "tile_row", "tile_col", "tile_y", "tile_x"]
+                for dim in desired_order:
+                    if dim not in assay.tile.dims:
+                        assay["tile"] = assay.tile.expand_dims(dim)
+
+                assay = assay.transpose(*desired_order)
 
                 yield assay
 
     @registry.readers.register("read")
     def make():
         return Reader()
 
 
-@registry.components.register("read_pinlist")
-def make_read_pinlist():
-    def read_pinlist(assay, pinlist):
-        assay = assay.assign_coords(id=(("marker_row", "marker_col"), read_names(pinlist)))
-        return assay
-
-    return read_pinlist
-
+@registry.component("read_pinlist")
+def read_pinlist(assay, pinlist, blank=None):
+    if blank is None:
+        blank = ["", "blank", "BLANK"]
 
-def read_names(path):
-    df = pd.read_csv(path)
+    df = pd.read_csv(pinlist)
     df["Indices"] = df["Indices"].apply(
         lambda s: [int(x) for x in re.sub(r"[\(\)]", "", s).split(",")]
     )
+    # Replace blanks with the empty string.
+    df["MutantID"] = df["MutantID"].replace(blank, "")
     # Zero-index the indices.
     cols, rows = np.array(df["Indices"].to_list()).T - 1
     names = df["MutantID"].to_numpy(dtype=str, na_value="")
     names_array = np.empty((max(rows) + 1, max(cols) + 1), dtype=names.dtype)
     names_array[rows, cols] = names
-    return names_array
+    assay = assay.assign_coords(id=(("marker_row", "marker_col"), names_array))
+    return assay
 
 
 def extract_paths(pattern) -> dict[tuple[int, str, int, int], str]:
     pattern = os.path.expanduser(pattern)
 
     # Filter out special signifiers used for pattern matching.
     glob_path = pattern.replace("(assay)", "*")
@@ -186,19 +250,19 @@
     glob_path = glob_path.replace("(row)", "*")
     glob_path = glob_path.replace("(col)", "*")
 
     # Search for files matching the pattern.
     paths = glob.glob(glob_path, recursive=True)
 
     regex_path = fnmatch.translate(pattern)
-    regex_path = regex_path.replace("\\(assay\\)", "(?P<assay>.*?)")
-    regex_path = regex_path.replace("\\(channel\\)", "(?P<channel>.*?)")
-    regex_path = re.sub(r"\\\(time\s*\|?.*?\\\)", r"(?P<time>.*?)", regex_path)
-    regex_path = regex_path.replace("\\(row\\)", "(?P<row>.*?)")
-    regex_path = regex_path.replace("\\(col\\)", "(?P<col>.*?)")
+    regex_path = regex_path.replace("\\(assay\\)", "(?P<assay>.*)")
+    regex_path = regex_path.replace("\\(channel\\)", "(?P<channel>.*)")
+    regex_path = re.sub(r"\\\(time\s*\|?.*?\\\)", r"(?P<time>.*)", regex_path)
+    regex_path = regex_path.replace("\\(row\\)", "(?P<row>.*)")
+    regex_path = regex_path.replace("\\(col\\)", "(?P<col>.*)")
     regex_path = re.compile(regex_path, re.IGNORECASE)
 
     path_dict = collections.defaultdict(dict)
     for path in paths:
         match = regex_path.fullmatch(path)
         if "(assay)" in pattern:
             assay = match.group("assay")
@@ -228,12 +292,12 @@
         if "(col)" in pattern:
             col = int(match.group("col"))
         else:
             col = -1
 
         idx = (channel, time, row, col)
         if idx not in path_dict[assay]:
-            path_dict[assay][idx] = path
+            path_dict[assay][idx] = os.path.abspath(path)
         else:
             raise ValueError(f"{path} and {path_dict[assay][idx]} map to the same index.")
 
     return path_dict
```

### Comparing `magnify-0.1.9/src/magnify/utils.py` & `magnify-0.2.0/src/magnify/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from collections.abc import Callable
 from typing import Any
 import inspect
+import re
 
 import cv2 as cv
 import numpy as np
 
 
 def to_uint8(arr: np.ndarray) -> np.ndarray:
     arr = arr.astype(float)
@@ -45,7 +46,12 @@
         right = image_width
     return top, bottom, left, right
 
 
 def valid_kwargs(kwargs: dict[str, Any], func: Callable) -> dict[str, Any]:
     args = list(inspect.signature(func).parameters)
     return {k: kwargs[k] for k in kwargs if k in args}
+
+
+def natural_sort_key(s: str) -> list[str]:
+    reg = re.compile("([0-9]+)")
+    return [int(text) if text.isdigit() else text.lower() for text in reg.split(s)]
```

### Comparing `magnify-0.1.9/PKG-INFO` & `magnify-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.1.9
+Version: 0.2.0
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: basicpy (>=1.0.1,<2.0.0)
+Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: catalogue (>=2.0.8,<3.0.0)
+Requires-Dist: confection (>=0.0.4,<0.0.5)
 Requires-Dist: dask[complete] (>=2022.02.0)
+Requires-Dist: lxml (>=4.6.0,<5.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.0) ; sys_platform != "darwin"
 Requires-Dist: opencv-python (>=4.0,!=4.7.0.68) ; sys_platform == "darwin"
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: tifffile (>=2021.11.2)
 Requires-Dist: tqdm (>=4.64,<5.0)
```

