# Comparing `tmp/meteo_render-0.4.4.tar.gz` & `tmp/meteo_render-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteo_render-0.4.4.tar", max compression
+gzip compressed data, was "meteo_render-0.5.0.tar", max compression
```

## Comparing `meteo_render-0.4.4.tar` & `meteo_render-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       35 2023-01-13 21:36:28.795883 meteo_render-0.4.4/meteo_render/__init__.py
--rw-r--r--   0        0        0     3145 2023-02-12 20:25:53.804314 meteo_render-0.4.4/meteo_render/__main__.py
--rw-r--r--   0        0        0      893 2023-02-12 17:43:33.436626 meteo_render-0.4.4/meteo_render/config.py
--rw-r--r--   0        0        0     2684 2023-02-12 20:30:02.575667 meteo_render-0.4.4/meteo_render/render.py
--rw-r--r--   0        0        0    10886 2023-01-14 12:57:34.343863 meteo_render-0.4.4/meteo_render/templates/family/img/0.png
--rw-r--r--   0        0        0     5764 2023-01-14 14:19:10.437532 meteo_render-0.4.4/meteo_render/templates/family/img/1.png
--rw-r--r--   0        0        0    29923 2023-03-07 20:20:51.648846 meteo_render-0.4.4/meteo_render/templates/family/img/2.png
--rw-r--r--   0        0        0    43068 2023-01-14 12:29:11.979052 meteo_render-0.4.4/meteo_render/templates/family/img/3.png
--rw-r--r--   0        0        0      160 2023-01-14 14:17:47.167746 meteo_render-0.4.4/meteo_render/templates/family/img/45.png
--rw-r--r--   0        0        0    46641 2023-02-16 11:41:10.764459 meteo_render-0.4.4/meteo_render/templates/family/img/51.png
--rw-r--r--   0        0        0    42755 2023-02-10 18:55:10.011327 meteo_render-0.4.4/meteo_render/templates/family/img/53.png
--rw-r--r--   0        0        0    41342 2023-02-16 11:44:30.230500 meteo_render-0.4.4/meteo_render/templates/family/img/61.png
--rw-r--r--   0        0        0     6473 2023-01-19 21:02:15.867070 meteo_render-0.4.4/meteo_render/templates/family/img/65.png
--rw-r--r--   0        0        0    46815 2023-02-10 19:23:22.515686 meteo_render-0.4.4/meteo_render/templates/family/img/71.png
--rw-r--r--   0        0        0    24549 2023-01-14 12:56:42.793882 meteo_render-0.4.4/meteo_render/templates/family/img/73.png
--rw-r--r--   0        0        0     3726 2023-01-20 14:04:09.829762 meteo_render-0.4.4/meteo_render/templates/family/img/75.png
--rw-r--r--   0        0        0    52366 2023-04-07 17:53:58.450037 meteo_render-0.4.4/meteo_render/templates/family/img/80.png
--rw-r--r--   0        0        0     1618 2023-02-23 19:45:32.632085 meteo_render-0.4.4/meteo_render/templates/family/img/85.png
--rw-r--r--   0        0        0    63831 2023-02-10 18:57:27.259644 meteo_render-0.4.4/meteo_render/templates/family/img/86.png
--rw-r--r--   0        0        0    52440 2023-02-10 18:53:27.772581 meteo_render-0.4.4/meteo_render/templates/family/img/95.png
--rw-r--r--   0        0        0     3590 2023-01-20 14:02:26.709446 meteo_render-0.4.4/meteo_render/templates/family/img/99.png
--rw-r--r--   0        0        0     1698 2023-01-19 21:02:15.867070 meteo_render-0.4.4/meteo_render/templates/family/img/XXX.png
--rw-r--r--   0        0        0     1650 2023-01-19 21:02:15.867070 meteo_render-0.4.4/meteo_render/templates/family/page.html.j2
--rw-r--r--   0        0        0      712 2023-01-14 14:11:21.548763 meteo_render-0.4.4/meteo_render/templates/family/style.css
--rw-r--r--   0        0        0      464 2023-04-07 17:54:18.949874 meteo_render-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 meteo_render-0.4.4/setup.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 meteo_render-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-01-13 21:36:28.795883 meteo_render-0.5.0/meteo_render/__init__.py
+-rw-r--r--   0        0        0     3145 2023-02-12 20:25:53.804314 meteo_render-0.5.0/meteo_render/__main__.py
+-rw-r--r--   0        0        0      950 2023-04-08 17:48:12.262846 meteo_render-0.5.0/meteo_render/config.py
+-rw-r--r--   0        0        0     2705 2023-04-08 17:49:02.932720 meteo_render-0.5.0/meteo_render/render.py
+-rw-r--r--   0        0        0    10886 2023-01-14 12:57:34.343863 meteo_render-0.5.0/meteo_render/templates/family/img/0.png
+-rw-r--r--   0        0        0     5764 2023-01-14 14:19:10.437532 meteo_render-0.5.0/meteo_render/templates/family/img/1.png
+-rw-r--r--   0        0        0    29923 2023-03-07 20:20:51.648846 meteo_render-0.5.0/meteo_render/templates/family/img/2.png
+-rw-r--r--   0        0        0    43068 2023-01-14 12:29:11.979052 meteo_render-0.5.0/meteo_render/templates/family/img/3.png
+-rw-r--r--   0        0        0      160 2023-01-14 14:17:47.167746 meteo_render-0.5.0/meteo_render/templates/family/img/45.png
+-rw-r--r--   0        0        0    46641 2023-02-16 11:41:10.764459 meteo_render-0.5.0/meteo_render/templates/family/img/51.png
+-rw-r--r--   0        0        0    42755 2023-02-10 18:55:10.011327 meteo_render-0.5.0/meteo_render/templates/family/img/53.png
+-rw-r--r--   0        0        0    41342 2023-02-16 11:44:30.230500 meteo_render-0.5.0/meteo_render/templates/family/img/61.png
+-rw-r--r--   0        0        0     6473 2023-01-19 21:02:15.867070 meteo_render-0.5.0/meteo_render/templates/family/img/65.png
+-rw-r--r--   0        0        0    46815 2023-02-10 19:23:22.515686 meteo_render-0.5.0/meteo_render/templates/family/img/71.png
+-rw-r--r--   0        0        0    24549 2023-01-14 12:56:42.793882 meteo_render-0.5.0/meteo_render/templates/family/img/73.png
+-rw-r--r--   0        0        0     3726 2023-01-20 14:04:09.829762 meteo_render-0.5.0/meteo_render/templates/family/img/75.png
+-rw-r--r--   0        0        0    52366 2023-04-07 17:53:58.450037 meteo_render-0.5.0/meteo_render/templates/family/img/80.png
+-rw-r--r--   0        0        0     1618 2023-02-23 19:45:32.632085 meteo_render-0.5.0/meteo_render/templates/family/img/85.png
+-rw-r--r--   0        0        0    63831 2023-02-10 18:57:27.259644 meteo_render-0.5.0/meteo_render/templates/family/img/86.png
+-rw-r--r--   0        0        0    52440 2023-02-10 18:53:27.772581 meteo_render-0.5.0/meteo_render/templates/family/img/95.png
+-rw-r--r--   0        0        0     3590 2023-01-20 14:02:26.709446 meteo_render-0.5.0/meteo_render/templates/family/img/99.png
+-rw-r--r--   0        0        0     1698 2023-01-19 21:02:15.867070 meteo_render-0.5.0/meteo_render/templates/family/img/XXX.png
+-rw-r--r--   0        0        0     1650 2023-01-19 21:02:15.867070 meteo_render-0.5.0/meteo_render/templates/family/page.html.j2
+-rw-r--r--   0        0        0      712 2023-01-14 14:11:21.548763 meteo_render-0.5.0/meteo_render/templates/family/style.css
+-rw-r--r--   0        0        0      481 2023-04-08 17:51:05.722417 meteo_render-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 meteo_render-0.5.0/setup.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 meteo_render-0.5.0/PKG-INFO
```

### Comparing `meteo_render-0.4.4/meteo_render/__main__.py` & `meteo_render-0.5.0/meteo_render/__main__.py`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/config.py` & `meteo_render-0.5.0/meteo_render/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from collections import defaultdict
 
+import pytz
+
 
 WEATHER_CODE_NAMES = defaultdict(lambda: "???")
 
 WEATHER_CODE_NAMES.update(
     {
         0: "CLEAR SKY",
         1: "MAINLY CLEAR",
@@ -31,7 +33,10 @@
         85: "LIGHT SNOW SHOWERS",
         86: "SNOW SHOWERS",
         95: "THUNDER",
         96: "THUNDER WITH LIGHT HAIL",
         99: "THUNDER WITH HAIL",
     }
 )
+
+TIMEZONE = pytz.timezone("Europe/London")
+
```

### Comparing `meteo_render-0.4.4/meteo_render/render.py` & `meteo_render-0.5.0/meteo_render/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from collections import defaultdict
 
 import jinja2
 import requests
 
-from .config import WEATHER_CODE_NAMES
+from .config import WEATHER_CODE_NAMES, TIMEZONE
 
 ISO_LOCAL_FORMAT = "%Y-%m-%dT%H:%M"
 ISO_DATE_FORMAT = "%Y-%m-%d"
 URL_PATTERN = "https://api.open-meteo.com/v1/forecast?latitude=%f&longitude=%f&hourly=temperature_2m,apparent_temperature,precipitation,weathercode"
 
 
 def get_images(folder):
@@ -66,15 +66,15 @@
 def render_weather(location, template, image_folder):
     url = URL_PATTERN % location
     result = requests.get(url)
     result.raise_for_status()
     raw_data = result.json()
     data = format_data(raw_data)
 
-    now = datetime.datetime.now()
+    now = datetime.datetime.now(tz=TIMEZONE)
     this_hour = datetime.datetime(now.year, now.month, now.day, now.hour)
     extra = {
         "timestamp": now.strftime(ISO_LOCAL_FORMAT),
         "hour": this_hour.strftime(ISO_LOCAL_FORMAT),
         "names": WEATHER_CODE_NAMES,
         "images": get_images(image_folder),
         "day_names": make_day_names(datetime.date.today()),
```

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/0.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/0.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/1.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/1.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/2.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/2.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/3.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/3.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/51.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/51.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/53.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/53.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/61.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/61.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/65.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/65.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/71.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/71.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/73.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/73.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/75.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/75.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/80.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/80.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/85.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/85.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/86.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/86.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/95.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/95.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/99.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/99.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/img/XXX.png` & `meteo_render-0.5.0/meteo_render/templates/family/img/XXX.png`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/page.html.j2` & `meteo_render-0.5.0/meteo_render/templates/family/page.html.j2`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/meteo_render/templates/family/style.css` & `meteo_render-0.5.0/meteo_render/templates/family/style.css`

 * *Files identical despite different names*

### Comparing `meteo_render-0.4.4/setup.py` & `meteo_render-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['meteo_render']
 
 package_data = \
 {'': ['*'], 'meteo_render': ['templates/family/*', 'templates/family/img/*']}
 
 install_requires = \
-['Jinja2>=3.1.2,<4.0.0', 'requests>=2.28.2,<3.0.0']
+['Jinja2>=3.1.2,<4.0.0', 'pytz>=2023.3,<2024.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'meteo-render',
-    'version': '0.4.4',
+    'version': '0.5.0',
     'description': 'Retrieve open-meteo.com data and render it into HTML pages',
     'long_description': 'None',
     'author': 'Jack Grahl',
     'author_email': 'jack.grahl@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `meteo_render-0.4.4/PKG-INFO` & `meteo_render-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: meteo-render
-Version: 0.4.4
+Version: 0.5.0
 Summary: Retrieve open-meteo.com data and render it into HTML pages
 License: MIT
 Author: Jack Grahl
 Author-email: jack.grahl@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

