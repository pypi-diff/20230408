# Comparing `tmp/cllm-data-curation-0.1.0.tar.gz` & `tmp/cllm-data-curation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cllm-data-curation-0.1.0.tar", last modified: Sat Apr  8 15:11:37 2023, max compression
+gzip compressed data, was "cllm-data-curation-0.1.1.tar", last modified: Sat Apr  8 20:55:59 2023, max compression
```

## Comparing `cllm-data-curation-0.1.0.tar` & `cllm-data-curation-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 15:11:37.172840 cllm-data-curation-0.1.0/
--rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 15:11:37.172714 cllm-data-curation-0.1.0/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      176 2023-03-27 19:27:04.000000 cllm-data-curation-0.1.0/README.md
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 15:11:37.168348 cllm-data-curation-0.1.0/cllm_data_curation/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:56:48.000000 cllm-data-curation-0.1.0/cllm_data_curation/__init__.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 15:11:37.170453 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-22 21:31:03.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2023 2023-03-23 16:08:20.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/multiprocessing_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)      744 2023-03-29 23:32:35.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/other_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     1768 2023-03-28 17:42:00.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/parallel_dl.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     3284 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/preprocessing_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     7872 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/processing_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 15:11:37.172280 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:57:34.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2736 2023-03-28 16:55:45.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/curation_configs.py
--rw-r--r--   0 darienschettler   (501) staff       (20)    13262 2023-03-28 17:18:26.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/curation_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     4123 2023-03-27 22:03:56.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/download.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     6188 2023-03-27 22:00:32.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/download_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2492 2023-03-27 21:22:03.000000 cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/general_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 15:11:37.168982 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 15:11:37.000000 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      873 2023-04-08 15:11:37.000000 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-08 15:11:37.000000 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       86 2023-04-08 15:11:37.000000 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-08 15:11:37.000000 cllm-data-curation-0.1.0/cllm_data_curation.egg-info/top_level.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-08 15:11:37.172891 cllm-data-curation-0.1.0/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)     1110 2023-04-08 15:11:24.000000 cllm-data-curation-0.1.0/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.891193 cllm-data-curation-0.1.1/
+-rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 20:55:59.891095 cllm-data-curation-0.1.1/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      176 2023-03-27 19:27:04.000000 cllm-data-curation-0.1.1/README.md
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.889036 cllm-data-curation-0.1.1/cllm_data_curation/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:56:48.000000 cllm-data-curation-0.1.1/cllm_data_curation/__init__.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.890230 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-22 21:31:03.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2023 2023-03-23 16:08:20.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/multiprocessing_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)      744 2023-03-29 23:32:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/other_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1768 2023-03-28 17:42:00.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/parallel_dl.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     3284 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/preprocessing_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     7872 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/processing_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.890922 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:57:34.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2736 2023-03-28 16:55:45.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_configs.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)    16183 2023-04-08 20:54:00.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     4123 2023-03-27 22:03:56.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     6188 2023-03-27 22:00:32.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2492 2023-03-27 21:22:03.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/general_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.889552 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      873 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       86 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/top_level.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-08 20:55:59.891229 cllm-data-curation-0.1.1/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1110 2023-04-08 20:55:09.000000 cllm-data-curation-0.1.1/setup.py
```

### Comparing `cllm-data-curation-0.1.0/PKG-INFO` & `cllm-data-curation-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cllm-data-curation
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/cllm-data-curation
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.1 Summary: A
 package to visualize tokenization of text using HTML Home-page: https://
 github.com/ds08tf/cllm-data-curation Author: Darien Schettler Author-email:
 ds08tf@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.7
```

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/multiprocessing_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/other_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/other_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/parallel_dl.py` & `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/parallel_dl.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/preprocessing_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/parallel_dl/processing_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/processing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/curation_configs.py` & `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_configs.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/curation_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from glob import glob
 from tqdm import tqdm
 import pandas as pd
 import numpy as np
 import json
+import ast
 import os
 import re
 
 # So we can see progress bars
 tqdm.pandas()
 
 
@@ -57,76 +58,108 @@
         meta_df = meta_df[meta_df.lang_size_mb > mb_size_thresh]
     elif pq_file_cnt_thresh:
         meta_df = meta_df[meta_df.lang_file_cnt >= pq_file_cnt_thresh]
     return meta_df[~meta_df.lang.isin(bad_langs)].reset_index(drop=True)
 
 
 def filter_parquet_file(pq_path, output_dir,
-                        max_ll=600, min_len=50, min_max_ll=25, max_size_kbs=1_000,
-                        min_alphanum=0.001, max_alphanum=0.975, min_ave_ll=16, min_lines=3, is_slim=True):
-    """ Filter a Parquet file by line-length, file-size, number of lines, and alphanumerical fraction.
+                        max_ll=600, min_len=50, min_max_ll=25, max_size_kbs=1_000, keep_original_index=True,
+                        min_alphanum=0.001, max_alphanum=0.975, min_ave_ll=16, min_lines=3, is_slim=True, **kwargs):
+    """Filter a Parquet file by applying multiple criteria such as line length, file size,
+    number of lines, and alphanumerical fraction.
 
     Args:
-        pq_path (str): The path to the Parquet file to filter.
-        output_dir (str): The directory to save the filtered Parquet file.
-        max_ll (int, optional): The maximum allowed line length.
-        min_len (int, optional): The minimum allowed file size.
-        min_max_ll (int, optional): The minimum allowed maximum line length.
-        max_size_kbs (int, optional): The maximum allowed file size in kbs.
-        min_alphanum (float, optional): The minimum allowed alphanumerical fraction.
-        max_alphanum (float, optional): The maximum allowed alphanumerical fraction.
-        min_ave_ll (int, optional): The minimum allowed average line length.
-        min_lines (int, optional): The minimum allowed number of lines.
-        is_slim (bool, optional): Whether to apply slim filtering or not.
+        pq_path (str): Path to the input Parquet file.
+            - NOTE: This is expected to be in the form: .../<root_dir>/<lang>/<pq_file_name>.pq
+        output_dir (str): Directory to save the filtered Parquet file.
+        max_ll (int, optional): Maximum allowed line length. Defaults to 600.
+        min_len (int, optional): Minimum allowed file size. Defaults to 50.
+        min_max_ll (int, optional): Minimum allowed maximum line length. Defaults to 25.
+        max_size_kbs (int, optional): Maximum allowed file size in kilobytes. Defaults to 1000.
+        keep_original_index (bool, optional): Whether to keep the original index. Defaults to True.
+        min_alphanum (float, optional): Minimum allowed alphanumerical fraction. Defaults to 0.001.
+        max_alphanum (float, optional): Maximum allowed alphanumerical fraction. Defaults to 0.975.
+        min_ave_ll (int, optional): Minimum allowed average line length. Defaults to 16.
+        min_lines (int, optional): Minimum allowed number of lines. Defaults to 3.
+        is_slim (bool, optional): Whether to apply slim filtering or not. Defaults to True.
 
     Returns:
-        str: The path to the filtered Parquet file.
+        str: Path to the filtered Parquet file.
     """
-    # Step 0 - Identify originating directory and create destination directory (if necessary)
+    print(f"\nWORKING ON {pq_path} ...")
+
+    # Step 0: Identify input directory and create destination directory (if necessary)
     _root_path, _origin_root_dir, _lang, _fname = pq_path.rsplit("/", 3)
     _dest_dir = os.path.join(output_dir, _lang)
     _dest_path = pq_path.replace(_origin_root_dir, output_dir.rsplit("/", 1)[-1])
     if not os.path.isdir(_dest_dir):
         os.makedirs(_dest_dir, exist_ok=True)
 
-    # Step 1 - Load the dataframe from the Parquet file (slim if necessary)
+    # Step 1: Load the DataFrame from the Parquet file (slim if necessary)
     _df = open_pq_as_df(pq_path, is_slim=is_slim)
     print(f"\t--> ORIGINAL LENGTH: {len(_df)}")
 
-    # Step 2 - Filter out rows/files that have a maximum line length that falls outside
-    #          the required range (min_max_ll <= max_ll <= max_line_len)
-    _df = _df[((_df.max_ll <= max_ll) & (_df.max_ll >= min_max_ll))]
-    print(f"\t--> AFTER MAX LINE-LENGTH REDUX: {len(_df)}")
-
-    # Step 3 - Filter out rows/files that have a size (number of characters) less than `min_len`
-    _df = _df[_df.file_size >= min_len]
-    print(f"\t--> AFTER MIN FILE-SIZE REDUX: {len(_df)}")
-
-    # Step 4 - Filter out rows/files that have a size greater than `max_size_kbs`
-    _df = _df[_df.file_size // (1024 ** 2) <= max_size_kbs]
-    print(f"\t--> AFTER {max_size_kbs:,} KB MAX SIZE REDUX: {len(_df)}")
-
-    # Step 5 - Filter out rows/files that have an alphanumeric fraction that
-    #          falls outside the required range (min_alphanum, max_alphanum)
-    _df = _df[((_df.alphanum_frac > min_alphanum) & (_df.alphanum_frac < max_alphanum))]
-    print(f"\t--> AFTER ALPHANUMERIC REDUX: {len(_df)}")
-
-    # Step 6 - Filter out rows/files that have an average line length less than `min_ave_ll`
-    _df = _df[_df.ave_ll > min_ave_ll]
-    print(f"\t--> AFTER MIN AVE LL REDUX: {len(_df)}")
-
-    # Step 7 - Filter out rows/files that have fewer than `min_lines` lines
-    _df = _df[(_df.file_size / _df.ave_ll) >= min_lines]
-    print(f"\t--> AFTER MIN N-LINES REDUX: {len(_df)}")
+    # Step 2: Filter out rows/files with maximum line lengths outside the required range
+    filter_flag = ((_df.max_ll <= max_ll) & (_df.max_ll >= min_max_ll))
+    reject_df = _df[~filter_flag].copy()
+    reject_df.loc[:, "reason"] = "max_ll"
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER MAX LINE-LENGTH REDUCTION: {len(_df)}")
+
+    # Step 3: Filter out rows/files with sizes smaller than `min_len`
+    filter_flag = _df.file_size >= min_len
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("file_too_small")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER MIN FILE-SIZE REDUCTION: {len(_df)}")
+
+    # Step 4: Filter out rows/files with sizes larger than `max_size_kbs`
+    filter_flag = _df.file_size // 1024 <= max_size_kbs
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("file_too_large")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER {max_size_kbs:,} KB MAX SIZE REDUCTION: {len(_df)}")
+
+    # Step 5: Filter out rows/files with an alphanumeric fraction outside the required range
+    filter_flag = ((_df.alphanum_frac > min_alphanum) & (_df.alphanum_frac < max_alphanum))
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("alphanum_frac")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER ALPHANUMERIC REDUCTION: {len(_df)}")
+
+    # Step 6: Filter out rows/files with an average line length smaller than `min_ave_ll`
+    filter_flag = _df.ave_ll > min_ave_ll
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("ave_ll")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER MIN AVERAGE LINE LENGTH REDUCTION: {len(_df)}")
+
+    # Step 7: Filter out rows/files with fewer than `min_lines` lines
+    filter_flag = (_df.file_size / _df.ave_ll) >= min_lines
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("min_lines")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER MIN NUMBER OF LINES REDUCTION: {len(_df)}")
+
+    # Step 8: Filter out rows/files written in Python 2
+    filter_flag = _df.content.apply(test_source_code_compatible)
+    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("python2")
+    _df = _df[filter_flag]
+    print(f"\t--> AFTER PYTHON 2 DETECTION REDUCTION: {len(_df)}")
 
-    # Step 8 - Save the filtered dataframe to a Parquet file
+    # Step 9: Save the filtered DataFrame to a Parquet file
     print(f"\t--> SAVING ...\n\t--> `{_dest_path}` ...\n")
-    _df.to_parquet(_dest_path, index=False)
+    _df.to_parquet(_dest_path, index=keep_original_index)
+
+    # Step 9.5: Save the rejection DataFrame to a Parquet file
+    reject_df = reject_df.sort_index()  # sort to reorder according to the original ordering
+    reject_df.to_parquet(_dest_path.replace(".parquet", "_rejects.parquet"), index=keep_original_index)
 
-    # Step 9 - Return to sender
+    # Step 10: Return the path to the filtered Parquet file
     return _dest_path
 
 
 def open_pq_as_df(pq_path, is_slim=False):
     """Open a Parquet file as a Pandas DataFrame.
 
     Args:
@@ -220,15 +253,15 @@
 def glob_pq_paths(root_dir):
     """ Get all Parquet file paths in a directory. """
 
     def __check_capture(_path_list, _thresh=2):
         if len(_path_list) > _thresh:
             return True
 
-    pattern_checks = [("**", "*.parquet"), ("*.parquet"), ("**", "**", "*.parquet")]
+    pattern_checks = [("**", "*.parquet"), ("*.parquet",), ("**", "**", "*.parquet")]
     for pattern in pattern_checks:
         pq_paths = glob(os.path.join(root_dir, *pattern))
         if __check_capture(pq_paths):
             return pq_paths
     else:
         raise FileNotFoundError(f"\nNo Parquet files found in {root_dir} based on pattern checks (see below)\n"
                                 f"PATTERN CHECKS:  {pattern_checks}")
@@ -290,14 +323,40 @@
     # Escape the substring to prevent regex errors and build the pattern
     pattern = f"({re.escape(substring)}){{{n},}}"
 
     # Check if the pattern is found in the input string and return flag
     return bool(re.search(pattern, input_string))
 
 
+def test_source_code_compatible(input_string):
+    """
+    Test if the input source code is compatible with the current Python version.
+    This function has some limitations:
+    - It will only test compatibility with the Python version you are running.
+    - It won't differentiate between syntax errors and incompatibilities.
+
+    Args:
+        code_data (str): The source code to test compatibility.
+
+    Returns:
+        bool: If incompatible, returns False else True
+    """
+    try:
+        # Try to parse the source code as an Abstract Syntax Tree (AST)
+        # If it succeeds, the code is compatible with the current Python version
+        _ = ast.parse(input_string)
+        return True
+    except SyntaxError as exc:
+        # If a SyntaxError occurs, it means the code is not compatible with the current Python version
+        return False
+    except ValueError as exc:
+        # If a ValueError occurs, it means there is an issue with the input and the code is not compatible
+        return False
+
+
 ####################################################################################################
 # TODO - Create a function that allows us to visualize the filtered files and
 #        explains why the files were filtered out in the first place
 ####################################################################################################
 # def print_demo_omits(lang, n_demo_samples=10, max_print_ln=5000):
 #     print(f"\n{'='*100}\n\t\t\t{n_demo_samples} DEMO EXMAPLES FOR LANGUAGE --> {lang} \n{'='*100}\n")
 #     paths = lang_to_example_map[lang]
```

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/download.py` & `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/download_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation/thestack_curation/general_utils.py` & `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/general_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation.egg-info/PKG-INFO` & `cllm-data-curation-0.1.1/cllm_data_curation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cllm-data-curation
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/cllm-data-curation
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.1 Summary: A
 package to visualize tokenization of text using HTML Home-page: https://
 github.com/ds08tf/cllm-data-curation Author: Darien Schettler Author-email:
 ds08tf@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.7
```

### Comparing `cllm-data-curation-0.1.0/cllm_data_curation.egg-info/SOURCES.txt` & `cllm-data-curation-0.1.1/cllm_data_curation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.0/setup.py` & `cllm-data-curation-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cllm-data-curation",
-    version="0.1.0",
+    version="0.1.1",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization of text using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/cllm-data-curation",
     packages=find_packages(),
```

