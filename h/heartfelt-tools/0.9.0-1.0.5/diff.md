# Comparing `tmp/heartfelt_tools-0.9.0.tar.gz` & `tmp/heartfelt_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartfelt_tools-0.9.0.tar", max compression
+gzip compressed data, was "heartfelt_tools-1.0.5.tar", max compression
```

## Comparing `heartfelt_tools-0.9.0.tar` & `heartfelt_tools-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,19 @@
--rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-0.9.0/LICENSE
--rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-0.9.0/database_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/datastores/__init__.py
--rw-r--r--   0        0        0      938 2023-04-07 19:00:09.619442 heartfelt_tools-0.9.0/database_tools/datastores/records.py
--rw-r--r--   0        0        0     2520 2023-04-07 18:53:23.861591 heartfelt_tools-0.9.0/database_tools/datastores/signals.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/errors.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/io/__init__.py
--rw-r--r--   0        0        0      470 2023-04-07 17:47:29.796060 heartfelt_tools-0.9.0/database_tools/io/data.py
--rw-r--r--   0        0        0      224 2023-04-07 17:58:25.968297 heartfelt_tools-0.9.0/database_tools/io/utils.py
--rw-r--r--   0        0        0     7001 2023-04-07 20:08:43.428482 heartfelt_tools-0.9.0/database_tools/io/wfdb.py
--rw-r--r--   0        0        0        0 2023-02-09 01:25:56.000000 heartfelt_tools-0.9.0/database_tools/processing/__init__.py
--rw-r--r--   0        0        0     1228 2023-04-05 20:48:44.315318 heartfelt_tools-0.9.0/database_tools/processing/cardiac.py
--rw-r--r--   0        0        0     2721 2023-04-07 19:06:50.432508 heartfelt_tools-0.9.0/database_tools/processing/detect.py
--rw-r--r--   0        0        0     4765 2023-04-07 19:04:56.823116 heartfelt_tools-0.9.0/database_tools/processing/metrics.py
--rw-r--r--   0        0        0     1859 2023-04-07 20:26:24.799112 heartfelt_tools-0.9.0/database_tools/processing/modify.py
--rw-r--r--   0        0        0     5038 2023-04-07 20:26:09.535953 heartfelt_tools-0.9.0/database_tools/processing/utils.py
--rw-r--r--   0        0        0    10403 2023-04-05 21:19:59.194064 heartfelt_tools-0.9.0/database_tools/tools/DataEvaluator.py
--rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-0.9.0/database_tools/tools/DataLocator.py
--rw-r--r--   0        0        0       82 2023-04-07 20:11:00.337873 heartfelt_tools-0.9.0/database_tools/tools/__init__.py
--rw-r--r--   0        0        0    12276 2023-04-07 21:42:30.599494 heartfelt_tools-0.9.0/database_tools/tools/dataset.py
--rw-r--r--   0        0        0     6884 2023-04-07 20:11:10.345976 heartfelt_tools-0.9.0/database_tools/tools/records.py
--rw-r--r--   0        0        0      953 2023-04-07 21:42:52.932048 heartfelt_tools-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 heartfelt_tools-0.9.0/setup.py
--rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 heartfelt_tools-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-1.0.5/database_tools/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-01 16:18:45.571317 heartfelt_tools-1.0.5/database_tools/plotting/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-01 16:18:45.571317 heartfelt_tools-1.0.5/database_tools/plotting/bland_altman_plot.py
+-rw-r--r--   0        0        0     4285 2023-04-01 16:18:45.571317 heartfelt_tools-1.0.5/database_tools/plotting/histogram3d.py
+-rw-r--r--   0        0        0        0 2023-02-09 01:25:56.000000 heartfelt_tools-1.0.5/database_tools/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1228 2023-04-03 23:24:21.431033 heartfelt_tools-1.0.5/database_tools/preprocessing/cardiac.py
+-rw-r--r--   0        0        0     4046 2023-04-04 00:20:30.330619 heartfelt_tools-1.0.5/database_tools/preprocessing/datastores.py
+-rw-r--r--   0        0        0     7479 2023-04-04 00:19:23.657726 heartfelt_tools-1.0.5/database_tools/preprocessing/functions.py
+-rw-r--r--   0        0        0     3230 2023-04-03 23:37:43.625109 heartfelt_tools-1.0.5/database_tools/preprocessing/utils.py
+-rw-r--r--   0        0        0     4782 2023-02-23 00:29:14.233005 heartfelt_tools-1.0.5/database_tools/tools/BuildDatabase.py
+-rw-r--r--   0        0        0     6213 2022-11-08 19:03:04.000000 heartfelt_tools-1.0.5/database_tools/tools/DataEvaluator.py
+-rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-1.0.5/database_tools/tools/DataLocator.py
+-rw-r--r--   0        0        0      123 2023-02-20 19:13:25.248485 heartfelt_tools-1.0.5/database_tools/tools/__init__.py
+-rw-r--r--   0        0        0     7937 2023-02-20 19:24:11.259773 heartfelt_tools-1.0.5/database_tools/tools/records.py
+-rw-r--r--   0        0        0      821 2023-04-04 00:31:21.998658 heartfelt_tools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8544 1970-01-01 00:00:00.000000 heartfelt_tools-1.0.5/setup.py
+-rw-r--r--   0        0        0     8256 1970-01-01 00:00:00.000000 heartfelt_tools-1.0.5/PKG-INFO
```

### Comparing `heartfelt_tools-0.9.0/LICENSE` & `heartfelt_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/README.md` & `heartfelt_tools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/cardiac.py` & `heartfelt_tools-1.0.5/database_tools/preprocessing/cardiac.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/metrics.py` & `heartfelt_tools-1.0.5/database_tools/preprocessing/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,85 @@
 import itertools
 import numpy as np
 from scipy import signal, integrate
-from database_tools.processing.utils import make_equal_len
+from heartpy.peakdetection import detect_peaks
+from heartpy.datautils import rolling_mean
+from database_tools.preprocessing.utils import make_equal_len
+from neurokit2.ppg.ppg_findpeaks import _ppg_findpeaks_bishop
+
+def bandpass(x, low, high, fs, method='cheby2'):
+    """
+    Apply one of the following bandpass filters.
+      - 4th order Cheby II filter.
+      - 4th order butterworth filter.
+
+    Args:
+        x (np.ndarray): Signal data.
+        low (float, optional): Lower frequency in Hz.
+        high (float, optional): Upper frequency in Hz.
+        fs (int, optional): Sampling rate.
+        method (str, optional): One of ['cheby2', 'butter']. Defaults to 'cheby2'.
+
+    Returns:
+        x (np.ndarray): Filtered signal.
+    """
+    if method == 'cheby2':
+        filt = signal.cheby2(
+            N=4,
+            rs=20,
+            Wn=[low, high],
+            btype='bandpass',
+            output='sos',
+            fs=fs,
+        )
+    elif method == 'butter':
+        filt = signal.butter(
+            4,
+            [low, high],
+            btype='bandpass',
+            output='sos',
+            fs=fs
+        )
+    else:
+        raise ValueError('Method must be one of [\'cheby2\', \'butter\']')
+    x = signal.sosfiltfilt(filt, x, padtype=None)
+    return x
+
+def find_peaks(sig, show=False, **kwargs):
+    """Modified version of neuroki2 ppg_findpeaks method. Returns peaks and troughs
+       instead of just peaks. See neurokit2 documentation for original function.
+    """
+    peaks, troughs = _ppg_findpeaks_bishop(sig, show=show, **kwargs)
+    return dict(peaks=peaks[0], troughs=troughs[0])
+
+def align_signals(ppg, abp, win_len, fs):
+    """
+    Find the index at which the two signals
+    have the largest time correlation.
+
+    Args:
+        ppg (np.ndarray): PPG data.
+        abp (np.ndarray): ABP data.
+        win_len (int): Length of windows.
+        fs (int, optional): Sampling rate of signal.
+
+    Returns:
+        signals (tuple(np.ndarray)): Aligned PPG and ABP window.
+    """
+    max_offset = int(fs / 2)
+
+    abp = abp[0:win_len]
+
+    corr = []
+    for offset in range(0, max_offset):
+        x = ppg[offset : win_len + offset]
+        corr.append(np.sum( x * abp ))
+    idx = np.argmax(corr)
+    ppg_shift = ppg[idx : win_len + idx]
+    return (ppg_shift, abp)
 
 def get_similarity(x, y):
     """
     Calculates time or spectral similarity.
 
     Args:
         x (np.ndarray): PPG data.
@@ -95,37 +169,55 @@
         try:
             # Find SNR and convert to dB
             snr = 10 * np.log10(p_sig / p_noise)
         except (ZeroDivisionError, RuntimeWarning):
             snr = -10
     return snr, f0
 
-def get_beat_similarity(x, troughs, fs, return_beats=False):
+def flat_lines(x: np.ndarray, n: int) -> bool:
+    """
+    Flat line detection.
+
+    Args:
+        x (np.ndarray): Signal to process.
+        n (int): Maximum length of flat line.
+
+    Returns:
+        bool: True if n identical values exist consecutively in x.
+    """
+    return any(sum(1 for _ in g) > (n - 1) for _, g in itertools.groupby(x))
+
+def beat_similarity(x, fs, return_beats=False):
     """Calculates beat similarity by segmenting beats at valleys and
        calculating the Pearson correlation coefficient. The final value
        output is the mean of the correlation coefficients calculated from
        every combination (n=2) of beats in the signal.
 
        Returns -1 if there are less than 2 beats.
        ZeroDivisionError returns -2.
 
     Args:
         x (np.ndarray): Cardiac signal.
-        troughs (list): Trough indices.
         fs (int): Sampling rate of cardiac signal.
 
     Returns:
         s (float): Mean of beat correlation coeffients.
     """
+    pad_width = 40
+    x_pad = np.pad(x, pad_width=pad_width, constant_values=np.mean(x))
+    
+    _, peaks = find_peaks(x_pad).values()
+    peaks = np.array(peaks) - pad_width - 1
+
     # check there are at least 2 peaks
-    if (len(troughs) < 2):
+    if (len(peaks) < 2):
         return -1
 
     neg_len = lambda x : len(x) * -1
-    beats = sorted(np.split(x, troughs), key=neg_len)
+    beats = sorted(np.split(x, peaks), key=neg_len)
 
     aligned_beats = [beats[0]]
 
     for i, b in enumerate(beats[1::]):
         b_new = np.pad(b, pad_width=[0, len(beats[0]) - len(b)])
         aligned_beats.append(b_new)
```

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/DataLocator.py` & `heartfelt_tools-1.0.5/database_tools/tools/DataLocator.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/records.py` & `heartfelt_tools-1.0.5/database_tools/tools/records.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,56 @@
 import glob
 import numpy as np
+import pandas as pd
 import pickle as pkl
 from tqdm import tqdm
-import tensorflow as tf
 from time import time_ns
-from typing import Tuple, List
+import tensorflow as tf
 from sklearn.model_selection import train_test_split
-from database_tools.tools.dataset import Dataset
+
+import logging
+from typing import Tuple, List
+from dataclasses import dataclass, InitVar, field
+
+logging.basicConfig(level=logging.INFO)
+
+
+@dataclass
+class Dataset:
+
+    data_dir: InitVar[str]
+    ppg: np.ndarray = field(init=False)
+    vpg: np.ndarray = field(init=False)
+    apg: np.ndarray = field(init=False)
+    abp: np.ndarray = field(init=False)
+
+    _nframes: int = field(init=False)
+
+    def __post_init__(self, data_dir: str) -> None:
+        frames = [pd.read_json(file, lines=True) for file in glob.glob(f'{data_dir}lines/*.jsonlines')]
+        object.__setattr__(self, '_nframes', len(frames))
+        data = pd.concat(frames, ignore_index=True)
+        object.__setattr__(self, 'ppg', np.array(data['ppg'].to_list()))
+        vpg = np.gradient(self.ppg, axis=1)  # 1st derivative of ppg
+        apg = np.gradient(vpg, axis=1) # 2nd derivative of vpg
+        object.__setattr__(self, 'vpg', vpg)
+        object.__setattr__(self, 'apg', apg)
+        object.__setattr__(self, 'abp', np.array(data['abp'].to_list()))
+        self.info
+
+    @property
+    def info(self):
+        logging.info(f'Data was extracted from {self._nframes} JSONLINES files.')
+        logging.info(f'The total number of windows is {self.ppg.shape[0]}.')
+
 
 def generate_records(
     ds: Dataset,
     data_dir: str,
-    split_strategy: Tuple[float, float, float] = (0.7, 0.15, 0.15),
+    split_strategy: Tuple[float, float, float] = None,
     samples_per_file: int = 10000,
     scaler_path: str = None,
 ) -> Tuple[dict, dict]:
     """Generates TFRecords files from dataset.
 
     Args:
         ds (Dataset): Dataset object consisting of ppg and abp data from JSONLINES files.
@@ -35,28 +70,31 @@
     else:
         idx = get_split_idx(n=ds.ppg.shape[0], split_strategy=split_strategy)
     data_unscaled = split_data(ds, idx)
 
     print('Scaling data...')
     if scaler_path is not None:
         with open(scaler_path, 'rb') as f:
-            scaler, scaler_split_idx = pkl.load(f)
+            scaler = pkl.load(f)
     else:
         scaler = None
     data_scaled, scaler_dict = scale_data(data_unscaled, scaler)
 
+    if scaler_path is None:
+        with open(f'{data_dir}min_max_scaler_{time_ns()}.pkl', 'wb') as f:
+            pkl.dump(scaler_dict, f)
+    with open(f'{data_dir}split_idx_{time_ns()}.pkl', 'wb') as f:
+        pkl.dump(idx, f)
+
     print('Generating TFRecords...')
     write_records(
         data=data_scaled,
         data_dir=data_dir,
         samples_per_file=samples_per_file,
     )
-    if scaler_path is None:
-        with open(f'{data_dir}records_info_{time_ns()}.pkl', 'wb') as f:
-            pkl.dump([scaler_dict, idx], f)
     return (data_unscaled, data_scaled, scaler_dict)
 
 def get_split_idx(n: int, split_strategy: Tuple[float, float, float]) -> dict:
     idx = [i for i in range(0, n)]
     tmp = split_strategy[1] + split_strategy[2]  # val + test size
     idx_train, idx_val = train_test_split(
         idx,
@@ -80,34 +118,31 @@
             test=tmp[idx['test']],
         )
     return data
 
 def scale_data(data_unscaled: dict, scaler: dict) -> Tuple[dict, dict]:
     data_scaled = {'ppg': {}, 'vpg': {}, 'apg': {}, 'abp': {}}
     scaler_dict = {}
-    for key in ['ppg', 'vpg', 'apg']:
+    for key in ['ppg', 'vpg', 'apg', 'abp']:
         if scaler is None:
             min_ = np.min(data_unscaled[key]['train'])
             max_ = np.max(data_unscaled[key]['train'])
         else:
             min_ = scaler[key][0]
             max_ = scaler[key][1]
         scaler_dict[key] = [min_, max_]
 
         for split in ['train', 'val', 'test']:
             tmp = data_unscaled[key][split]
             tmp_scaled = np.divide(tmp - min_, max_ - min_)
             data_scaled[key][split] = tmp_scaled
-    data_scaled['abp']['train'] = data_unscaled['abp']['train']
-    data_scaled['abp']['val'] = data_unscaled['abp']['val']
-    data_scaled['abp']['test'] = data_unscaled['abp']['test']
     return (data_scaled, scaler_dict)
 
 def write_records(data: dict, data_dir: str, samples_per_file: int) -> None:
-    records_dir = data_dir + 'data/records/'
+    records_dir = data_dir + 'records/'
     for split in ['train', 'val', 'test']:
         print(f'Starting {split} split...')
         split_data = {f'{sig}': data[sig][split] for sig in data.keys()}
 
         file_number = 0
         num_samples = 0
         examples = []
```

### Comparing `heartfelt_tools-0.9.0/pyproject.toml` & `heartfelt_tools-1.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heartfelt-tools"
-version = "0.9.0"
+version = "1.0.5"
 description = "Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb."
 authors = ["Cameron Johnson"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "database_tools"}]
 
 [tool.poetry.dependencies]
@@ -18,24 +18,17 @@
 openpyxl = "^3.0.10"
 scipy = "^1.9.3"
 neurokit2 = "^0.2.1"
 heartpy = "^1.2.7"
 wfdb = "^4.0.0"
 tensorflow = "==2.9.2"
 vitaldb = "^1.2.10"
-pytest = "^7.2.1"
-alive-progress = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 ipywidgets = "==7.7.1"
 jupyterlab-widgets = "==1.1.1"
 widgetsnbextension = "==3.6.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-filterwarnings = [
-    "ignore::DeprecationWarning:wfdb.*",
-]
```

### Comparing `heartfelt_tools-0.9.0/setup.py` & `heartfelt_tools-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['database_tools',
- 'database_tools.datastores',
- 'database_tools.io',
- 'database_tools.processing',
+ 'database_tools.plotting',
+ 'database_tools.preprocessing',
  'database_tools.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['alive-progress>=3.0.1,<4.0.0',
- 'heartpy>=1.2.7,<2.0.0',
+['heartpy>=1.2.7,<2.0.0',
  'neurokit2>=0.2.1,<0.3.0',
  'numpy>=1.23.4,<2.0.0',
  'openpyxl>=3.0.10,<4.0.0',
  'pandas>=1.5.1,<2.0.0',
  'plotly>=5.10.0,<6.0.0',
- 'pytest>=7.2.1,<8.0.0',
  'scikit-learn>=1.1.2,<2.0.0',
  'scipy>=1.9.3,<2.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'tensorflow==2.9.2',
  'tqdm>=4.64.1,<5.0.0',
  'vitaldb>=1.2.10,<2.0.0',
  'wfdb>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'heartfelt-tools',
-    'version': '0.9.0',
+    'version': '1.0.5',
     'description': 'Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.',
     'long_description': '<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->\n<a name="readme-top"></a>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n      \n            \n <img src="images/heartfelt-logo.png"  width="300em" height="300em"> \n\n  \n  <h1 align="center">MIMIC-III Database Tools</h1>\n\n  <p align="center">\n    For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms Database.\n    <br />\n  </p>\n</div>\n\n\n\n<!-- TABLE OF CONTENTS -->\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#introduction">Introduction</a>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n      <ul>\n        <li><a href="#poetry">Poetry</a></li>\n        <li><a href="#get-valid-records">Get Valid Records</a></li>\n        <li><a href="#build-database">Build Database</a></li>\n        <li><a href="#evaluate-dataset">Evaluate Dataset</a></li>\n        <li><a href="#generate-records">Generate Records</a></li>\n        <li><a href="#read-records">Read Records</a></li>\n      </ul>\n    <li><a href="#license">License</a></li>\n  </ol>\n</details>\n\n\n\n<!-- Introduction -->\n## Introduction\n\nThis repo contains a set of tools for extracting and cleaning photoplethysmography (ppg) and artial blood pressure (abp) waveforms from the [MIMIC-III Waveforms Database](https://physionet.org/content/mimic3wdb/1.0/) for the purpose of blood pressure estimation via deep learning. \n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nThis sections details the requirements to start using this library. Links are for Ubuntu installation.\n\n### Prerequisites\n\n1. Python\n```shell\nsudo apt install python3.8 -y\nsudo apt install python3.8-dev python3.8-venv -y\n\necho \'export PATH="$PATH:/home/ubuntu/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\ncurl -sS https://bootstrap.pypa.io/get-pip.py | python3.8\npython3.8 -m pip install virtualenv\npython3.8 -m venv .venv/base-env\necho \'alias base-env="source ~/.venv/base-env/bin/activate"\' >> ~/.bashrc\nbase-env\n\npython3.8 -m pip install --upgrade pip\n```\n2. Poetry\n```shell\ncurl -sSL https://install.python-poetry.org | python3 -\necho \'export PATH="$PATH:$HOME/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\n# Verify installation\npoetry --version\n```\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\n### Poetry\nThe commands below can be used to install the poetry environment, build the project, and activate the environment.\n```shell\ncd database-tools\npoetry lock\npoetry install\npoetry build\npoetry shell\n```\n\n### Create Data Directory\nThe functions in this library rely on a data folder named with the convention `data-YYYY-MM-DD`. This directory contains two additional folders, `mimic3/` and `figures/`. The `mimic3/lines/` folder is intended to hold the jsonlines files the data will initially saved to. The `mimic3/records/` folder will hold the TFRecords files generated from these jsonlines files. This will be discussed in greater depth in the <a href="#generate-records">Generate Records</a> section.\n\n### Get Valid Records\nThe class DataLocator (located in `database_tools/tools/`) is specifically written to find valid data files in the MIMIC-III Waveforms subset and create a csv of the html links for these data files. Performing this task prior to downloading is done to improve runtime and the usability of this workflow. Valid records refers to data files that contain both PPG and ABP recordings and are at least 10 minutes in length. Currently this code is only intended for the MIMIC-III Waveforms subset but will likely be adapated to allow for valid segments to be identified in the MIMIC-III Matched Subset (records are linked to clinical data). To perform an extraction the file `scripts/get-valid-segs.py` can be run (data directory and repository path must be configured manually). This function will output a csv called `valid-segments.csv` to the data directory provided. The figure below shows how these signals are located.\n\nAdd mimic3 valid segs logic figure.\n\n### Build Database\nThe class `BuildDatabase` (located in `database_tools/tools/`) downloads data from `valid-segments.csv`, extracts PPG and ABP data, and then processed it by leveraging the `SignalProcessor` class (located in `database_tools/preprocessing/`). A database can be build by running `scripts/build_database.py` (be sure to configure the paths). BuildDatabase takes a few important parameters which modify how signals are excluded and how the signals are divided prior to processing. The `win_len` parameter controls the length of each window, `fs` is the sampling rate of the data (125 Hz in the case of MIMIC-III), while `samples_per_file`, `samples_per_patient`, and `max_samples` control the size of the dataset (how many files the data is spread across, how many samples a patient can contribute, and the total number of samples in the dataset. The final parameter `config` controls the various constants of the SignalProcessor that determine the quality threshold for accepting signals. The SignalProcessor filters signals according to the figure chart below. The functions used for this filtering can be found in `database_tools/preprocessing/`. Data exctracted with this script is saved directly to the `mimic3/lines/` folder in the data directory. A file named `mimic3_stats.csv` containing the stats of every processed waveform (not just the valid ones) will also be saved to the data directory.\n\nAdd data preprocessing figure.\n\n### Evaluate Dataset\nThe class `DataEvaluator` (located in `database_tools/tools/`) reads the `mimic3_stats.csv` file from the provided data directory and outputs figures to visualize the statistics. These figures are saved directly to the `figures/` folder in the data directory in addition to be output such that they can be viewed in a Jupyter notebook. The 3D histogram are generated using the fuction `histogram3d` located in `database_tools/plotting/`.\n\n### Generate Records\nOnce data has been extracted TFRecords can be generated for training a Tensorflow model. The class `RecordsHandler` contains the method `GenerateRecords` which is used to create the TFRecords. This can be done using `scripts/generate_records.py` (paths must be configured). When calling `GenerateRecords` the size of the train, validation, and test splits, as well as the max number of samples per file and a boolean to control whether or not the data is standardized must be specified (using `sklearn.preprocessing.StandardScaler()`.\n\n### Read Records\nThe class `RecordsHandler` also contains the function `ReadRecords` which can be used to read the TFRecords into a Tensorflow `TFRecordsDataset` object. This function can be used to inspect the integrity of the dataset or for loading the dataset for model training. The number of cores and a TensorFlow `AUTOTUNE` object must be provided.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the MIT License. See `LICENSE.txt` for more information.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n',
     'author': 'Cameron Johnson',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
-['database_tools', 'database_tools.datastores', 'database_tools.io',
-'database_tools.processing', 'database_tools.tools'] package_data = \ {'':
-['*']} install_requires = \ ['alive-progress>=3.0.1,<4.0.0',
-'heartpy>=1.2.7,<2.0.0', 'neurokit2>=0.2.1,<0.3.0', 'numpy>=1.23.4,<2.0.0',
+['database_tools', 'database_tools.plotting', 'database_tools.preprocessing',
+'database_tools.tools'] package_data = \ {'': ['*']} install_requires = \
+['heartpy>=1.2.7,<2.0.0', 'neurokit2>=0.2.1,<0.3.0', 'numpy>=1.23.4,<2.0.0',
 'openpyxl>=3.0.10,<4.0.0', 'pandas>=1.5.1,<2.0.0', 'plotly>=5.10.0,<6.0.0',
-'pytest>=7.2.1,<8.0.0', 'scikit-learn>=1.1.2,<2.0.0', 'scipy>=1.9.3,<2.0.0',
-'tabulate>=0.9.0,<0.10.0', 'tensorflow==2.9.2', 'tqdm>=4.64.1,<5.0.0',
-'vitaldb>=1.2.10,<2.0.0', 'wfdb>=4.0.0,<5.0.0'] setup_kwargs = { 'name':
-'heartfelt-tools', 'version': '0.9.0', 'description': 'Extract and process
-photoplethysmography and arterial blood pressure data from mimic3-waveforms and
-vitaldb.', 'long_description': '\n\n\n\n
+'scikit-learn>=1.1.2,<2.0.0', 'scipy>=1.9.3,<2.0.0', 'tabulate>=0.9.0,<0.10.0',
+'tensorflow==2.9.2', 'tqdm>=4.64.1,<5.0.0', 'vitaldb>=1.2.10,<2.0.0',
+'wfdb>=4.0.0,<5.0.0'] setup_kwargs = { 'name': 'heartfelt-tools', 'version':
+'1.0.5', 'description': 'Extract and process photoplethysmography and arterial
+blood pressure data from mimic3-waveforms and vitaldb.', 'long_description':
+'\n\n\n\n
 \n
                  \n \n \n [images/heartfelt-logo.png] \n\n \n
                     ****** MIMIC-III Database Tools ******
                                      \n\n
  \n For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms
                                  Database.\n
                                       \n
```

### Comparing `heartfelt_tools-0.9.0/PKG-INFO` & `heartfelt_tools-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: heartfelt-tools
-Version: 0.9.0
+Version: 1.0.5
 Summary: Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.
 License: MIT
 Author: Cameron Johnson
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: alive-progress (>=3.0.1,<4.0.0)
 Requires-Dist: heartpy (>=1.2.7,<2.0.0)
 Requires-Dist: neurokit2 (>=0.2.1,<0.3.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: plotly (>=5.10.0,<6.0.0)
-Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tensorflow (==2.9.2)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: vitaldb (>=1.2.10,<2.0.0)
 Requires-Dist: wfdb (>=4.0.0,<5.0.0)
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: heartfelt-tools Version: 0.9.0 Summary: Extract and
+Metadata-Version: 2.1 Name: heartfelt-tools Version: 1.0.5 Summary: Extract and
 process photoplethysmography and arterial blood pressure data from mimic3-
 waveforms and vitaldb. License: MIT Author: Cameron Johnson Requires-Python:
 >=3.9,<3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Requires-Dist: alive-progress (>=3.0.1,<4.0.0) Requires-Dist: heartpy
-(>=1.2.7,<2.0.0) Requires-Dist: neurokit2 (>=0.2.1,<0.3.0) Requires-Dist: numpy
-(>=1.23.4,<2.0.0) Requires-Dist: openpyxl (>=3.0.10,<4.0.0) Requires-Dist:
-pandas (>=1.5.1,<2.0.0) Requires-Dist: plotly (>=5.10.0,<6.0.0) Requires-Dist:
-pytest (>=7.2.1,<8.0.0) Requires-Dist: scikit-learn (>=1.1.2,<2.0.0) Requires-
-Dist: scipy (>=1.9.3,<2.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tensorflow (==2.9.2) Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: vitaldb (>=1.2.10,<2.0.0) Requires-Dist: wfdb (>=4.0.0,<5.0.0)
-Description-Content-Type: text/markdown
+:: 3.9 Requires-Dist: heartpy (>=1.2.7,<2.0.0) Requires-Dist: neurokit2
+(>=0.2.1,<0.3.0) Requires-Dist: numpy (>=1.23.4,<2.0.0) Requires-Dist: openpyxl
+(>=3.0.10,<4.0.0) Requires-Dist: pandas (>=1.5.1,<2.0.0) Requires-Dist: plotly
+(>=5.10.0,<6.0.0) Requires-Dist: scikit-learn (>=1.1.2,<2.0.0) Requires-Dist:
+scipy (>=1.9.3,<2.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
+tensorflow (==2.9.2) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist:
+vitaldb (>=1.2.10,<2.0.0) Requires-Dist: wfdb (>=4.0.0,<5.0.0) Description-
+Content-Type: text/markdown
                           [images/heartfelt-logo.png]
                     ****** MIMIC-III Database Tools ******
    For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms
                                   Database.
   Table of Contents
    1. Introduction
    2. Getting_Started
```

