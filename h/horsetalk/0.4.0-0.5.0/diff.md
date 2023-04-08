# Comparing `tmp/horsetalk-0.4.0.tar.gz` & `tmp/horsetalk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.4.0.tar", max compression
+gzip compressed data, was "horsetalk-0.5.0.tar", max compression
```

## Comparing `horsetalk-0.4.0.tar` & `horsetalk-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
--rw-r--r--   0        0        0      935 2023-04-08 14:32:29.680135 horsetalk-0.4.0/horsetalk/__init__.py
--rw-r--r--   0        0        0      157 2023-04-08 14:32:29.681370 horsetalk-0.4.0/horsetalk/age_category.py
--rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.4.0/horsetalk/aw_going_description.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.4.0/horsetalk/breed.py
--rw-r--r--   0        0        0      471 2023-04-07 18:00:16.677798 horsetalk-0.4.0/horsetalk/coat_colour.py
--rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.4.0/horsetalk/dirt_going_description.py
--rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.4.0/horsetalk/disaster.py
--rw-r--r--   0        0        0      200 2023-04-08 14:32:29.681370 horsetalk-0.4.0/horsetalk/experience_level.py
--rw-r--r--   0        0        0      566 2023-04-08 14:32:29.682376 horsetalk-0.4.0/horsetalk/gender.py
--rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.4.0/horsetalk/obstacle.py
--rw-r--r--   0        0        0      415 2023-04-08 14:32:29.682376 horsetalk-0.4.0/horsetalk/parsing_enum.py
--rw-r--r--   0        0        0     2029 2023-04-08 14:32:29.682376 horsetalk-0.4.0/horsetalk/race_title.py
--rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.4.0/horsetalk/racing_code.py
--rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.4.0/horsetalk/sex.py
--rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.4.0/horsetalk/surface.py
--rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.4.0/horsetalk/turf_going_description.py
--rw-r--r--   0        0        0      164 2023-04-08 14:32:29.683376 horsetalk-0.4.0/horsetalk/weight_determinant.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.4.0/LICENSE
--rw-r--r--   0        0        0      653 2023-04-08 14:32:29.683376 horsetalk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.4.0/README.md
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 horsetalk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-04-08 16:50:46.370436 horsetalk-0.5.0/horsetalk/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-08 16:43:51.100371 horsetalk-0.5.0/horsetalk/age_category.py
+-rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.5.0/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.5.0/horsetalk/breed.py
+-rw-r--r--   0        0        0      514 2023-04-08 16:50:46.370436 horsetalk-0.5.0/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.5.0/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.5.0/horsetalk/disaster.py
+-rw-r--r--   0        0        0      275 2023-04-08 16:50:46.370436 horsetalk-0.5.0/horsetalk/finishing_position.py
+-rw-r--r--   0        0        0      138 2023-04-08 16:50:46.371438 horsetalk-0.5.0/horsetalk/form_break.py
+-rw-r--r--   0        0        0      422 2023-04-08 16:50:46.371438 horsetalk-0.5.0/horsetalk/form_figures.py
+-rw-r--r--   0        0        0      566 2023-04-08 16:43:51.100371 horsetalk-0.5.0/horsetalk/gender.py
+-rw-r--r--   0        0        0      542 2023-04-08 16:50:46.371438 horsetalk-0.5.0/horsetalk/headgear.py
+-rw-r--r--   0        0        0      205 2023-04-08 16:50:46.372436 horsetalk-0.5.0/horsetalk/horse_experience_level.py
+-rw-r--r--   0        0        0      303 2023-04-08 16:50:46.372436 horsetalk-0.5.0/horsetalk/jockey_experience_level.py
+-rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.5.0/horsetalk/obstacle.py
+-rw-r--r--   0        0        0      415 2023-04-08 16:43:51.100371 horsetalk-0.5.0/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      332 2023-04-08 16:50:46.372436 horsetalk-0.5.0/horsetalk/race_designation.py
+-rw-r--r--   0        0        0     2046 2023-04-08 16:50:46.373436 horsetalk-0.5.0/horsetalk/race_title.py
+-rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.5.0/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.5.0/horsetalk/sex.py
+-rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.5.0/horsetalk/surface.py
+-rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.5.0/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.5.0/LICENSE
+-rw-r--r--   0        0        0      653 2023-04-08 16:50:46.373436 horsetalk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.5.0/README.md
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 horsetalk-0.5.0/PKG-INFO
```

### Comparing `horsetalk-0.4.0/horsetalk/disaster.py` & `horsetalk-0.5.0/horsetalk/disaster.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.4.0/horsetalk/gender.py` & `horsetalk-0.5.0/horsetalk/gender.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.4.0/horsetalk/race_title.py` & `horsetalk-0.5.0/horsetalk/race_title.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import List, Type
 from .age_category import AgeCategory
-from .experience_level import ExperienceLevel
+from .horse_experience_level import HorseExperienceLevel
 from .gender import Gender
 from .obstacle import Obstacle
-from .weight_determinant import WeightDeterminant
+from .race_designation import RaceDesignation
 
 
 class RaceTitle:
     _words: List[str] = []
 
     @classmethod
     def parse(cls, title: str) -> dict:
@@ -18,28 +18,28 @@
         :type title: str
         :return: A dictionary of component parts
         :rtype: dict
         """
         self = cls()
         self._words = title.split()
 
-        enums = [AgeCategory, ExperienceLevel, Gender, Obstacle, WeightDeterminant]
+        enums = [AgeCategory, HorseExperienceLevel, Gender, Obstacle, RaceDesignation]
         end_index = -1
         for i, word in enumerate(self._words):
             if any(getattr(enum, word, None) is not None for enum in enums):
                 end_index = i
                 break
         name = " ".join(self._words[:end_index])
 
         return {
             "age_category": self._lookup(AgeCategory),
-            "experience_level": self._lookup(ExperienceLevel),
+            "horse_experience_level": self._lookup(HorseExperienceLevel),
             "gender": self._lookup(Gender, allow_multiple=True),
             "obstacle": self._lookup(Obstacle),
-            "weight_determinant": self._lookup(WeightDeterminant),
+            "race_designation": self._lookup(RaceDesignation),
             "name": name,
         }
 
     def _lookup(
         self, enum: Type[Enum], allow_multiple: bool = False
     ) -> List[Enum] | Enum | None:
         """Private method to lookup an enum value from a list of words
```

### Comparing `horsetalk-0.4.0/horsetalk/turf_going_description.py` & `horsetalk-0.5.0/horsetalk/turf_going_description.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.4.0/LICENSE` & `horsetalk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.4.0/pyproject.toml` & `horsetalk-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.4.0"
+version = "0.5.0"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `horsetalk-0.4.0/PKG-INFO` & `horsetalk-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

