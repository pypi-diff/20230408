# Comparing `tmp/env_canada-0.5.8.tar.gz` & `tmp/env_canada-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_canada-0.5.8.tar", last modified: Mon Sep 13 23:29:14 2021, max compression
+gzip compressed data, was "env_canada-0.5.9.tar", last modified: Tue Sep 14 11:49:14 2021, max compression
```

## Comparing `env_canada-0.5.8.tar` & `env_canada-0.5.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 23:29:14.622679 env_canada-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-13 23:29:07.000000 env_canada-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-13 23:29:07.000000 env_canada-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2021-09-13 23:29:14.622679 env_canada-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-09-13 23:29:07.000000 env_canada-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 23:29:14.618679 env_canada-0.5.8/env_canada/
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/10x20.pbm
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/10x20.pil
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/ec_aqhi.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/ec_historical.py
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/ec_hydro.py
--rw-r--r--   0 runner    (1001) docker     (121)    10010 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/ec_radar.py
--rw-r--r--   0 runner    (1001) docker     (121)    13463 2021-09-13 23:29:07.000000 env_canada-0.5.8/env_canada/ec_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 23:29:14.618679 env_canada-0.5.8/env_canada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2021-09-13 23:29:14.000000 env_canada-0.5.8/env_canada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-09-13 23:29:14.000000 env_canada-0.5.8/env_canada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-13 23:29:14.000000 env_canada-0.5.8/env_canada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-13 23:29:14.000000 env_canada-0.5.8/env_canada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-13 23:29:14.000000 env_canada-0.5.8/env_canada.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-13 23:29:14.622679 env_canada-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-09-13 23:29:07.000000 env_canada-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 23:29:14.622679 env_canada-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/test_ec_aqhi.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/test_ec_historical.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/test_ec_hydro.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/test_ec_radar.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-09-13 23:29:07.000000 env_canada-0.5.8/tests/test_ec_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 11:49:14.860212 env_canada-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-14 11:49:05.000000 env_canada-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-14 11:49:05.000000 env_canada-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5095 2021-09-14 11:49:14.860212 env_canada-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-09-14 11:49:05.000000 env_canada-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 11:49:14.856212 env_canada-0.5.9/env_canada/
+-rw-r--r--   0 runner    (1001) docker     (121)     2463 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/10x20.pbm
+-rw-r--r--   0 runner    (1001) docker     (121)     5143 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/10x20.pil
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6921 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/ec_aqhi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10483 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/ec_historical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4842 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/ec_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10010 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/ec_radar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13463 2021-09-14 11:49:05.000000 env_canada-0.5.9/env_canada/ec_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 11:49:14.860212 env_canada-0.5.9/env_canada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5095 2021-09-14 11:49:14.000000 env_canada-0.5.9/env_canada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-09-14 11:49:14.000000 env_canada-0.5.9/env_canada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 11:49:14.000000 env_canada-0.5.9/env_canada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-14 11:49:14.000000 env_canada-0.5.9/env_canada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-14 11:49:14.000000 env_canada-0.5.9/env_canada.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-14 11:49:14.860212 env_canada-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2021-09-14 11:49:05.000000 env_canada-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 11:49:14.860212 env_canada-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/test_ec_aqhi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/test_ec_historical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/test_ec_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/test_ec_radar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-09-14 11:49:05.000000 env_canada-0.5.9/tests/test_ec_weather.py
```

### Comparing `env_canada-0.5.8/LICENSE` & `env_canada-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/PKG-INFO` & `env_canada-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env_canada
-Version: 0.5.8
+Version: 0.5.9
 Summary: A package to access meteorological data from Environment Canada
 Home-page: https://github.com/michaeldavie/env_canada
 Author: Michael Davie
 Author-email: michael.davie@gmail.com
 License: MIT
 Description: # Environment Canada (env_canada)
```

### Comparing `env_canada-0.5.8/README.md` & `env_canada-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/10x20.pbm` & `env_canada-0.5.9/env_canada/10x20.pbm`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/10x20.pil` & `env_canada-0.5.9/env_canada/10x20.pil`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/ec_aqhi.py` & `env_canada-0.5.9/env_canada/ec_aqhi.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,27 +150,29 @@
 
         if aqhi_current:
             # Update region name
             element = aqhi_current.find("region")
             self.region_name = element.attrib[
                 "name{lang}".format(lang=self.language.title())
             ]
+            self.metadata["location"] = self.region_name
 
             # Update AQHI current condition
             element = aqhi_current.find("airQualityHealthIndex")
             if element is not None:
                 self.current = float(element.text)
             else:
                 self.current = None
 
             element = aqhi_current.find("./dateStamp/UTCStamp")
             if element is not None:
                 self.current_timestamp = timestamp_to_datetime(element.text)
             else:
                 self.current_timestamp = None
+            self.metadata["timestamp"] = self.current_timestamp
 
         # Update AQHI forecasts
         aqhi_forecast = await self.get_aqhi_data(url=AQHI_FORECAST_URL)
 
         if aqhi_forecast:
             # Update AQHI daily forecasts
             for f in aqhi_forecast.findall("./forecastGroup/forecast"):
```

### Comparing `env_canada-0.5.8/env_canada/ec_historical.py` & `env_canada-0.5.9/env_canada/ec_historical.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/ec_hydro.py` & `env_canada-0.5.9/env_canada/ec_hydro.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/ec_radar.py` & `env_canada-0.5.9/env_canada/ec_radar.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada/ec_weather.py` & `env_canada-0.5.9/env_canada/ec_weather.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/env_canada.egg-info/PKG-INFO` & `env_canada-0.5.9/env_canada.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-canada
-Version: 0.5.8
+Version: 0.5.9
 Summary: A package to access meteorological data from Environment Canada
 Home-page: https://github.com/michaeldavie/env_canada
 Author: Michael Davie
 Author-email: michael.davie@gmail.com
 License: MIT
 Description: # Environment Canada (env_canada)
```

### Comparing `env_canada-0.5.8/env_canada.egg-info/SOURCES.txt` & `env_canada-0.5.9/env_canada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/setup.py` & `env_canada-0.5.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="env_canada",
-    version="0.5.8",
+    version="0.5.9",
     author="Michael Davie",
     author_email="michael.davie@gmail.com",
     description="A package to access meteorological data from Environment Canada",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaeldavie/env_canada",
```

### Comparing `env_canada-0.5.8/tests/test_ec_aqhi.py` & `env_canada-0.5.9/tests/test_ec_aqhi.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/tests/test_ec_historical.py` & `env_canada-0.5.9/tests/test_ec_historical.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/tests/test_ec_hydro.py` & `env_canada-0.5.9/tests/test_ec_hydro.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/tests/test_ec_radar.py` & `env_canada-0.5.9/tests/test_ec_radar.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.5.8/tests/test_ec_weather.py` & `env_canada-0.5.9/tests/test_ec_weather.py`

 * *Files identical despite different names*

