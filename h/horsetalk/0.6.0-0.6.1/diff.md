# Comparing `tmp/horsetalk-0.6.0.tar.gz` & `tmp/horsetalk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.6.0.tar", max compression
+gzip compressed data, was "horsetalk-0.6.1.tar", max compression
```

## Comparing `horsetalk-0.6.0.tar` & `horsetalk-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1502 2023-04-08 19:59:38.806863 horsetalk-0.6.0/horsetalk/__init__.py
--rw-r--r--   0        0        0      157 2023-04-08 16:43:51.100371 horsetalk-0.6.0/horsetalk/age_category.py
--rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.6.0/horsetalk/aw_going_description.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.6.0/horsetalk/breed.py
--rw-r--r--   0        0        0      514 2023-04-08 16:50:46.370436 horsetalk-0.6.0/horsetalk/coat_colour.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.6.0/horsetalk/dirt_going_description.py
--rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.6.0/horsetalk/disaster.py
--rw-r--r--   0        0        0      275 2023-04-08 18:27:27.925629 horsetalk-0.6.0/horsetalk/finishing_position.py
--rw-r--r--   0        0        0      138 2023-04-08 18:27:27.925629 horsetalk-0.6.0/horsetalk/form_break.py
--rw-r--r--   0        0        0      422 2023-04-08 16:50:46.371438 horsetalk-0.6.0/horsetalk/form_figures.py
--rw-r--r--   0        0        0      566 2023-04-08 16:43:51.100371 horsetalk-0.6.0/horsetalk/gender.py
--rw-r--r--   0        0        0      542 2023-04-08 16:50:46.371438 horsetalk-0.6.0/horsetalk/headgear.py
--rw-r--r--   0        0        0     2043 2023-04-08 20:08:40.056905 horsetalk-0.6.0/horsetalk/horse_age.py
--rw-r--r--   0        0        0      205 2023-04-08 16:50:46.372436 horsetalk-0.6.0/horsetalk/horse_experience_level.py
--rw-r--r--   0        0        0     1146 2023-04-08 20:08:40.009182 horsetalk-0.6.0/horsetalk/horse_height.py
--rw-r--r--   0        0        0     3780 2023-04-08 19:59:38.807844 horsetalk-0.6.0/horsetalk/horselength.py
--rw-r--r--   0        0        0      303 2023-04-08 16:50:46.372436 horsetalk-0.6.0/horsetalk/jockey_experience_level.py
--rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.6.0/horsetalk/obstacle.py
--rw-r--r--   0        0        0      415 2023-04-08 16:43:51.100371 horsetalk-0.6.0/horsetalk/parsing_enum.py
--rw-r--r--   0        0        0      332 2023-04-08 16:50:46.372436 horsetalk-0.6.0/horsetalk/race_designation.py
--rw-r--r--   0        0        0     1345 2023-04-08 20:08:40.010192 horsetalk-0.6.0/horsetalk/race_distance.py
--rw-r--r--   0        0        0     2046 2023-04-08 16:50:46.373436 horsetalk-0.6.0/horsetalk/race_title.py
--rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.6.0/horsetalk/racing_code.py
--rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.6.0/horsetalk/sex.py
--rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.6.0/horsetalk/surface.py
--rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.6.0/horsetalk/turf_going_description.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.6.0/LICENSE
--rw-r--r--   0        0        0      723 2023-04-08 20:08:40.108405 horsetalk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.6.0/README.md
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1502 2023-04-08 20:26:53.418399 horsetalk-0.6.1/horsetalk/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-08 16:43:51.100371 horsetalk-0.6.1/horsetalk/age_category.py
+-rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.6.1/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.6.1/horsetalk/breed.py
+-rw-r--r--   0        0        0      514 2023-04-08 16:50:46.370436 horsetalk-0.6.1/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.6.1/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.6.1/horsetalk/disaster.py
+-rw-r--r--   0        0        0      275 2023-04-08 18:27:27.925629 horsetalk-0.6.1/horsetalk/finishing_position.py
+-rw-r--r--   0        0        0      138 2023-04-08 18:27:27.925629 horsetalk-0.6.1/horsetalk/form_break.py
+-rw-r--r--   0        0        0      422 2023-04-08 16:50:46.371438 horsetalk-0.6.1/horsetalk/form_figures.py
+-rw-r--r--   0        0        0      566 2023-04-08 16:43:51.100371 horsetalk-0.6.1/horsetalk/gender.py
+-rw-r--r--   0        0        0      542 2023-04-08 16:50:46.371438 horsetalk-0.6.1/horsetalk/headgear.py
+-rw-r--r--   0        0        0     2043 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horse_age.py
+-rw-r--r--   0        0        0      205 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/horse_experience_level.py
+-rw-r--r--   0        0        0     1146 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horse_height.py
+-rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.6.1/horsetalk/horselength.py
+-rw-r--r--   0        0        0      303 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/jockey_experience_level.py
+-rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.6.1/horsetalk/obstacle.py
+-rw-r--r--   0        0        0      529 2023-04-08 20:26:58.137781 horsetalk-0.6.1/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      332 2023-04-08 16:50:46.372436 horsetalk-0.6.1/horsetalk/race_designation.py
+-rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.6.1/horsetalk/race_distance.py
+-rw-r--r--   0        0        0     2046 2023-04-08 16:50:46.373436 horsetalk-0.6.1/horsetalk/race_title.py
+-rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.6.1/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/sex.py
+-rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/surface.py
+-rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.6.1/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.6.1/LICENSE
+-rw-r--r--   0        0        0      723 2023-04-08 20:27:24.446544 horsetalk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.6.1/README.md
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.6.1/PKG-INFO
```

### Comparing `horsetalk-0.6.0/horsetalk/__init__.py` & `horsetalk-0.6.1/horsetalk/__init__.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/coat_colour.py` & `horsetalk-0.6.1/horsetalk/coat_colour.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/disaster.py` & `horsetalk-0.6.1/horsetalk/disaster.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/gender.py` & `horsetalk-0.6.1/horsetalk/gender.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/headgear.py` & `horsetalk-0.6.1/horsetalk/headgear.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/horse_age.py` & `horsetalk-0.6.1/horsetalk/horse_age.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/horse_height.py` & `horsetalk-0.6.1/horsetalk/horse_height.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/horselength.py` & `horsetalk-0.6.1/horsetalk/horselength.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/race_distance.py` & `horsetalk-0.6.1/horsetalk/race_distance.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/race_title.py` & `horsetalk-0.6.1/horsetalk/race_title.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/horsetalk/turf_going_description.py` & `horsetalk-0.6.1/horsetalk/turf_going_description.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/LICENSE` & `horsetalk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.6.0/pyproject.toml` & `horsetalk-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.6.0"
+version = "0.6.1"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `horsetalk-0.6.0/PKG-INFO` & `horsetalk-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

