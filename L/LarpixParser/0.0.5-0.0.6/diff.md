# Comparing `tmp/LarpixParser-0.0.5.tar.gz` & `tmp/LarpixParser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LarpixParser-0.0.5.tar", last modified: Fri Mar 24 06:46:37 2023, max compression
+gzip compressed data, was "LarpixParser-0.0.6.tar", last modified: Fri Apr  7 22:30:41 2023, max compression
```

## Comparing `LarpixParser-0.0.5.tar` & `LarpixParser-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.694709 LarpixParser-0.0.5/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/LICENSE
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-03-24 06:46:37.690880 LarpixParser-0.0.5/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/README.md
--rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-03-24 06:46:37.691880 LarpixParser-0.0.5/setup.cfg
--rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-03-24 06:43:28.000000 LarpixParser-0.0.5/setup.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.517830 LarpixParser-0.0.5/src/
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.533362 LarpixParser-0.0.5/src/LarpixParser/
--rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-03-22 21:50:55.000000 LarpixParser-0.0.5/src/LarpixParser/__init__.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/charge_calibration.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.547808 LarpixParser-0.0.5/src/LarpixParser/config_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1651 2023-03-24 04:19:53.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/2x2.yaml
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.564862 LarpixParser-0.0.5/src/LarpixParser/config_repo/dict_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-03-24 06:25:46.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-03-23 23:18:59.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/module0.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3851 2023-03-24 03:43:18.000000 LarpixParser-0.0.5/src/LarpixParser/config_repo/ndlar-module.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/coord_transform.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1312 2023-03-24 03:55:23.000000 LarpixParser-0.0.5/src/LarpixParser/event_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-03-24 06:31:03.000000 LarpixParser-0.0.5/src/LarpixParser/geom_to_dict.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/get_charge.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1986 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/get_raw_coord.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/get_vdrift.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/hit_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-03-21 22:03:05.000000 LarpixParser-0.0.5/src/LarpixParser/units.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3673 2023-03-24 02:47:50.000000 LarpixParser-0.0.5/src/LarpixParser/util.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-03-24 06:46:37.539766 LarpixParser-0.0.5/src/LarpixParser.egg-info/
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-03-24 06:46:37.000000 LarpixParser-0.0.5/src/LarpixParser.egg-info/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-03-24 06:46:37.000000 LarpixParser-0.0.5/src/LarpixParser.egg-info/SOURCES.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-03-24 06:46:37.000000 LarpixParser-0.0.5/src/LarpixParser.egg-info/dependency_links.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-03-24 06:46:37.000000 LarpixParser-0.0.5/src/LarpixParser.egg-info/requires.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-03-24 06:46:37.000000 LarpixParser-0.0.5/src/LarpixParser.egg-info/top_level.txt
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.974114 LarpixParser-0.0.6/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-04-07 06:11:46.000000 LarpixParser-0.0.6/LICENSE
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-07 22:30:41.970838 LarpixParser-0.0.6/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-04-07 06:11:46.000000 LarpixParser-0.0.6/README.md
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-04-07 22:30:41.972189 LarpixParser-0.0.6/setup.cfg
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-04-07 22:28:03.000000 LarpixParser-0.0.6/setup.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:40.522206 LarpixParser-0.0.6/src/
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.072965 LarpixParser-0.0.6/src/LarpixParser/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/__init__.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/charge_calibration.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.625224 LarpixParser-0.0.6/src/LarpixParser/config_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1696 2023-04-07 21:59:13.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/2x2.yaml
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.840979 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/module0.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3851 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/config_repo/ndlar-module.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/coord_transform.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1517 2023-04-07 22:23:31.000000 LarpixParser-0.0.6/src/LarpixParser/event_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/geom_to_dict.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_charge.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1986 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_raw_coord.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/get_vdrift.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/hit_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-04-07 06:11:47.000000 LarpixParser-0.0.6/src/LarpixParser/units.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3737 2023-04-07 21:58:17.000000 LarpixParser-0.0.6/src/LarpixParser/util.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-07 22:30:41.296863 LarpixParser-0.0.6/src/LarpixParser.egg-info/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/SOURCES.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/dependency_links.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/requires.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-04-07 22:30:40.000000 LarpixParser-0.0.6/src/LarpixParser.egg-info/top_level.txt
```

### Comparing `LarpixParser-0.0.5/LICENSE` & `LarpixParser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/PKG-INFO` & `LarpixParser-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.5/README.md` & `LarpixParser-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/setup.py` & `LarpixParser-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import setuptools
 
-VER = "0.0.5"
+VER = "0.0.6"
 
 setuptools.setup(
     name="LarpixParser",
     version=VER,
     author="Yifan C. and others",
     author_email="cyifan@slac.stanford.edu",
     description="A package parsing the larpix output to hit-level",
```

### Comparing `LarpixParser-0.0.5/src/LarpixParser/charge_calibration.py` & `LarpixParser-0.0.6/src/LarpixParser/charge_calibration.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/2x2.yaml` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/2x2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,9 @@
   1: [1, 2]
   2: [3, 4]
   3: [5, 6]
   4: [7, 8]
 
 ifspill: True
 spill_spacing: 1.2e6          # microseconds
+beam_duration: 10             # microseconds
```

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/module0.yaml` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/module0.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/config_repo/ndlar-module.yaml` & `LarpixParser-0.0.6/src/LarpixParser/config_repo/ndlar-module.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/event_parser.py` & `LarpixParser-0.0.6/src/LarpixParser/event_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from sklearn.cluster import DBSCAN
 
+# still need to check what to do with non-beam simulation
+
 def get_t0(packets):
 
     t0 = []
     pckts_t0 = packets[packets['packet_type'] == 7]['timestamp'] # external trigger # by default larnd-sim fills external trigger for each event
 
     pckts_t0_db = pckts_t0.reshape(-1,1)
 
@@ -13,14 +15,17 @@
     n_clusters_ = len(set(labels)) - (1 if -1 in labels else 0)
     for i_ct in range(n_clusters_):
         ct_mask = labels == i_ct
         t0.append(np.min(pckts_t0[ct_mask]))
 
     return np.array(t0)
 
+def get_t0_spill(vertices, run_config):
+    dt_beam = run_config['beam_duration']
+    return (np.unique(vertices['t_spill']) + dt_beam *0.5) * 10
 
 def packet_to_eventid(assn, tracks, ifspill):
     '''
     Assoiciate packet to eventID.
     
     Arguments
     ---------
```

### Comparing `LarpixParser-0.0.5/src/LarpixParser/geom_to_dict.py` & `LarpixParser-0.0.6/src/LarpixParser/geom_to_dict.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/get_charge.py` & `LarpixParser-0.0.6/src/LarpixParser/get_charge.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/get_raw_coord.py` & `LarpixParser-0.0.6/src/LarpixParser/get_raw_coord.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/get_vdrift.py` & `LarpixParser-0.0.6/src/LarpixParser/get_vdrift.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/hit_parser.py` & `LarpixParser-0.0.6/src/LarpixParser/hit_parser.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/units.py` & `LarpixParser-0.0.6/src/LarpixParser/units.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.5/src/LarpixParser/util.py` & `LarpixParser-0.0.6/src/LarpixParser/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     run_config['birks_kb'] = run_yaml['birks_kb'] 
 
     run_config['W_ion'] = run_yaml['W_ion'] #MeV
 
     run_config['lifetime'] = run_yaml['lifetime'] #us
 
     run_config['ifspill'] = run_yaml['ifspill']
+    run_config['beam_duration'] = run_yaml['beam_duration'] #us
 
     return run_config
 
 def configuration_keywords():
     return ['module0','2x2','ndlar']
 
 def detector_configuration(detector):
```

### Comparing `LarpixParser-0.0.5/src/LarpixParser.egg-info/PKG-INFO` & `LarpixParser-0.0.6/src/LarpixParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.5/src/LarpixParser.egg-info/SOURCES.txt` & `LarpixParser-0.0.6/src/LarpixParser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

