# Comparing `tmp/rul_datasets-0.9.0.tar.gz` & `tmp/rul_datasets-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rul_datasets-0.9.0.tar", max compression
+gzip compressed data, was "rul_datasets-0.9.1.tar", max compression
```

## Comparing `rul_datasets-0.9.0.tar` & `rul_datasets-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1910 2023-03-15 14:37:52.542315 rul_datasets-0.9.0/README.md
--rw-r--r--   0        0        0     1532 2023-03-15 14:39:30.944964 rul_datasets-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      530 2023-03-15 14:39:30.960963 rul_datasets-0.9.0/rul_datasets/__init__.py
--rw-r--r--   0        0        0    21273 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/adaption.py
--rw-r--r--   0        0        0     9039 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/baseline.py
--rw-r--r--   0        0        0    20459 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/core.py
--rw-r--r--   0        0        0        0 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/py.typed
--rw-r--r--   0        0        0     6479 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/__init__.py
--rw-r--r--   0        0        0    15515 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/abstract.py
--rw-r--r--   0        0        0    14155 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/cmapss.py
--rw-r--r--   0        0        0     1420 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/data_root.py
--rw-r--r--   0        0        0     5909 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/dummy.py
--rw-r--r--   0        0        0    11953 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/femto.py
--rw-r--r--   0        0        0     4918 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/saving.py
--rw-r--r--   0        0        0    10825 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/scaling.py
--rw-r--r--   0        0        0     3450 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/truncating.py
--rw-r--r--   0        0        0    11232 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/reader/xjtu_sy.py
--rw-r--r--   0        0        0     6413 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/ssl.py
--rw-r--r--   0        0        0     3799 2023-03-15 14:37:52.546316 rul_datasets-0.9.0/rul_datasets/utils.py
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 rul_datasets-0.9.0/setup.py
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 rul_datasets-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1910 2023-03-16 08:59:03.566900 rul_datasets-0.9.1/README.md
+-rw-r--r--   0        0        0     1532 2023-03-16 09:00:28.992117 rul_datasets-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      530 2023-03-16 09:00:29.008117 rul_datasets-0.9.1/rul_datasets/__init__.py
+-rw-r--r--   0        0        0    21273 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/adaption.py
+-rw-r--r--   0        0        0     9039 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/baseline.py
+-rw-r--r--   0        0        0    20459 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/core.py
+-rw-r--r--   0        0        0        0 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/py.typed
+-rw-r--r--   0        0        0     6479 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/__init__.py
+-rw-r--r--   0        0        0    15515 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/abstract.py
+-rw-r--r--   0        0        0    14807 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/cmapss.py
+-rw-r--r--   0        0        0     1420 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/data_root.py
+-rw-r--r--   0        0        0     5909 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/dummy.py
+-rw-r--r--   0        0        0    11953 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/femto.py
+-rw-r--r--   0        0        0     4918 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/saving.py
+-rw-r--r--   0        0        0    10825 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/scaling.py
+-rw-r--r--   0        0        0     3450 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/truncating.py
+-rw-r--r--   0        0        0    11232 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/reader/xjtu_sy.py
+-rw-r--r--   0        0        0     6413 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/ssl.py
+-rw-r--r--   0        0        0     3799 2023-03-16 08:59:03.570900 rul_datasets-0.9.1/rul_datasets/utils.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 rul_datasets-0.9.1/setup.py
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 rul_datasets-0.9.1/PKG-INFO
```

### Comparing `rul_datasets-0.9.0/README.md` & `rul_datasets-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/pyproject.toml` & `rul_datasets-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rul_datasets"
-version = "0.9.0"
+version = "0.9.1"
 description = "A collection of datasets for RUL estimation as Lightning Data Modules."
 authors = ["Krokotsch, Tilman <tilman.krokotsch@tu-berlin.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://krokotsch.eu/rul-datasets"
 repository = "https://github.com/tilman151/rul-datasets"
 classifiers = [
```

### Comparing `rul_datasets-0.9.0/rul_datasets/__init__.py` & `rul_datasets-0.9.1/rul_datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 import warnings
 
 from .adaption import (
     DomainAdaptionDataModule,
     PretrainingAdaptionDataModule,
     LatentAlignDataModule,
```

### Comparing `rul_datasets-0.9.0/rul_datasets/adaption.py` & `rul_datasets-0.9.1/rul_datasets/adaption.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/baseline.py` & `rul_datasets-0.9.1/rul_datasets/baseline.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/core.py` & `rul_datasets-0.9.1/rul_datasets/core.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/__init__.py` & `rul_datasets-0.9.1/rul_datasets/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/abstract.py` & `rul_datasets-0.9.1/rul_datasets/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/cmapss.py` & `rul_datasets-0.9.1/rul_datasets/reader/cmapss.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,14 +216,16 @@
         if split in ["dev", "val"]:
             targets = self._generate_targets(time_steps)
         elif split == "test":
             targets = self._load_targets(features)
         else:
             raise ValueError(f"Unknown split {split}.")
 
+        features, targets = self._pad_data(features, targets)
+
         if alias in ["dev", "val"]:
             features, targets = self._window_data(features, targets)
         elif alias == "test":
             features, targets = self._crop_data(features, targets)
         else:
             raise ValueError(f"Unknown alias {alias}.")
 
@@ -296,41 +298,54 @@
         targets = [np.arange(len(f), 0, -1) + t - 1 for f, t in zip(features, targets)]
 
         max_rul = self.max_rul or np.inf
         targets = [np.minimum(max_rul, t) for t in targets]
 
         return targets
 
+    def _pad_data(self, features, targets):
+        padded_features = []
+        padded_targets = []
+        for i, (feat, target) in enumerate(zip(features, targets)):
+            if feat.shape[0] < self.window_size:
+                warnings.warn(
+                    f"Run {i} of CMAPSS FD{self.fd:03d} is shorter than window "
+                    f"size {self.window_size} and will be zero-padded."
+                )
+                missing = self.window_size - feat.shape[0]
+                feat_pad = (missing, feat.shape[1])
+                feat = np.concatenate([np.zeros(feat_pad), feat])
+                target = np.concatenate([np.zeros(missing), target])
+            padded_features.append(feat)
+            padded_targets.append(target)
+
+        return padded_features, padded_targets
+
     def _window_data(
         self, features: List[np.ndarray], targets: List[np.ndarray]
     ) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """Window features with specified window size."""
-        new_features = []
-        new_targets = []
+        windowed_features = []
+        windowed_targets = []
         for seq, target in zip(features, targets):
             windows = utils.extract_windows(seq, self.window_size)
             target = target[self.window_size - 1 :]
-            new_features.append(windows)
-            new_targets.append(target)
+            windowed_features.append(windows)
+            windowed_targets.append(target)
 
-        return new_features, new_targets
+        return windowed_features, windowed_targets
 
     def _crop_data(
         self, features: List[np.ndarray], targets: List[np.ndarray]
     ) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """Crop length of data to specified window size."""
         cropped_features = []
         cropped_targets = []
         for seq, target in zip(features, targets):
-            if seq.shape[0] < self.window_size:
-                pad = (self.window_size - seq.shape[0], seq.shape[1])
-                seq = np.concatenate([np.zeros(pad), seq])
-            else:
-                seq = seq[-self.window_size :]
-            cropped_features.append(np.expand_dims(seq, axis=0))
+            cropped_features.append(seq[None, -self.window_size :])
             cropped_targets.append(target[-1, None])
 
         return cropped_features, cropped_targets
 
 
 def _download_cmapss(data_root: str) -> None:
     with tempfile.TemporaryDirectory() as tmp_path:
```

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/data_root.py` & `rul_datasets-0.9.1/rul_datasets/reader/data_root.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/dummy.py` & `rul_datasets-0.9.1/rul_datasets/reader/dummy.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/femto.py` & `rul_datasets-0.9.1/rul_datasets/reader/femto.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/saving.py` & `rul_datasets-0.9.1/rul_datasets/reader/saving.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/scaling.py` & `rul_datasets-0.9.1/rul_datasets/reader/scaling.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/truncating.py` & `rul_datasets-0.9.1/rul_datasets/reader/truncating.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/reader/xjtu_sy.py` & `rul_datasets-0.9.1/rul_datasets/reader/xjtu_sy.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/ssl.py` & `rul_datasets-0.9.1/rul_datasets/ssl.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/rul_datasets/utils.py` & `rul_datasets-0.9.1/rul_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rul_datasets-0.9.0/setup.py` & `rul_datasets-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pytorch-lightning>=1.4.4,<2.0.0',
  'scikit-learn>=1.0.0,<2.0.0',
  'torch>=1.9.0,<2.0.0',
  'tqdm>=4.62.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'rul-datasets',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A collection of datasets for RUL estimation as Lightning Data Modules.',
     'long_description': '# RUL Datasets\n\n[![Master](https://github.com/tilman151/rul-datasets/actions/workflows/on_push.yaml/badge.svg)](https://github.com/tilman151/rul-datasets/actions/workflows/on_push.yaml)\n[![Release](https://github.com/tilman151/rul-datasets/actions/workflows/on_release.yaml/badge.svg)](https://github.com/tilman151/rul-datasets/actions/workflows/on_release.yaml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nThis library contains a collection of common benchmark datasets for **remaining useful lifetime (RUL)** estimation.\nThey are provided as [LightningDataModules](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.core.LightningDataModule.html#pytorch_lightning.core.LightningDataModule) to be readily used in [PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/latest/).\n\nCurrently, four datasets are supported:\n\n* **C-MAPSS** Turbofan Degradation Dataset\n* **FEMTO** (PRONOSTIA) Bearing Dataset\n* **XJTU-SY** Bearing Dataset\n* **Dummy** A tiny, simple dataset for debugging\n\nAll datasets share the same API, so they can be used as drop-in replacements for each other.\nThat means, if an experiment can be run with one of the datasets, it can be run with all of them.\nNo code changes needed.\n\nAside from the basic ones, this library contains data modules for advanced experiments concerning **transfer learning**, **unsupervised domain adaption** and **semi-supervised learning**.\nThese data modules are designed as **higher-order data modules**.\nThis means they take one or more of the basic data modules as inputs and adjust them to the desired use case.\n\n## Installation\n\nThe library is pip-installable. Simply type:\n\n```shell\npip install rul-datasets\n```\n\n## Contribution\n\nContributions are always welcome. Whether you want to fix a bug, add a feature or a new dataset, just open an issue and a PR.',
     'author': 'Krokotsch, Tilman',
     'author_email': 'tilman.krokotsch@tu-berlin.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://krokotsch.eu/rul-datasets',
```

### Comparing `rul_datasets-0.9.0/PKG-INFO` & `rul_datasets-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rul-datasets
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of datasets for RUL estimation as Lightning Data Modules.
 Home-page: https://krokotsch.eu/rul-datasets
 License: MIT
 Author: Krokotsch, Tilman
 Author-email: tilman.krokotsch@tu-berlin.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

