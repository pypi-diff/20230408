# Comparing `tmp/screenpy_adapter_allure-4.0.2.tar.gz` & `tmp/screenpy_adapter_allure-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_adapter_allure-4.0.2.tar", last modified: Thu Feb 16 05:53:17 2023, max compression
+gzip compressed data, was "screenpy_adapter_allure-4.0.3.tar", max compression
```

## Comparing `screenpy_adapter_allure-4.0.2.tar` & `screenpy_adapter_allure-4.0.3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-16 05:53:17.211238 screenpy_adapter_allure-4.0.2/
--rw-r--r--   0 perry      (501) staff       (20)     1071 2023-02-16 04:16:09.000000 screenpy_adapter_allure-4.0.2/LICENSE
--rw-r--r--   0 perry      (501) staff       (20)     3001 2023-02-16 05:53:17.211115 screenpy_adapter_allure-4.0.2/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)     2229 2022-03-14 04:26:52.000000 screenpy_adapter_allure-4.0.2/README.md
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-16 05:53:17.210202 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure/
--rw-r--r--   0 perry      (501) staff       (20)      470 2023-02-16 04:16:09.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure/__init__.py
--rw-r--r--   0 perry      (501) staff       (20)      418 2023-02-16 05:52:32.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure/__version__.py
--rw-r--r--   0 perry      (501) staff       (20)     4049 2022-02-23 04:02:01.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure/adapters.py
-drwxr-xr-x   0 perry      (501) staff       (20)        0 2023-02-16 05:53:17.210924 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/
--rw-r--r--   0 perry      (501) staff       (20)     3001 2023-02-16 05:53:17.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/PKG-INFO
--rw-r--r--   0 perry      (501) staff       (20)      371 2023-02-16 05:53:17.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/SOURCES.txt
--rw-r--r--   0 perry      (501) staff       (20)        1 2023-02-16 05:53:17.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/dependency_links.txt
--rw-r--r--   0 perry      (501) staff       (20)       37 2023-02-16 05:53:17.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/requires.txt
--rw-r--r--   0 perry      (501) staff       (20)       24 2023-02-16 05:53:17.000000 screenpy_adapter_allure-4.0.2/screenpy_adapter_allure.egg-info/top_level.txt
--rw-r--r--   0 perry      (501) staff       (20)       38 2023-02-16 05:53:17.211275 screenpy_adapter_allure-4.0.2/setup.cfg
--rw-r--r--   0 perry      (501) staff       (20)     1260 2023-02-16 04:16:09.000000 screenpy_adapter_allure-4.0.2/setup.py
+-rw-r--r--   0        0        0     1071 2023-02-16 04:16:09.295593 screenpy_adapter_allure-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2229 2022-03-14 04:26:52.349243 screenpy_adapter_allure-4.0.3/README.md
+-rw-r--r--   0        0        0     2922 2023-04-07 22:37:26.083112 screenpy_adapter_allure-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0      470 2023-02-16 04:16:09.296251 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-06 18:55:21.867917 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/__version__.py
+-rw-r--r--   0        0        0     4040 2023-04-04 22:21:09.516157 screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/adapters.py
+-rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 screenpy_adapter_allure-4.0.3/PKG-INFO
```

### Comparing `screenpy_adapter_allure-4.0.2/LICENSE` & `screenpy_adapter_allure-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy_adapter_allure-4.0.2/PKG-INFO` & `screenpy_adapter_allure-4.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: screenpy_adapter_allure
-Version: 4.0.2
-Summary: ScreenPy Adapter to log test steps to Allure.
-Home-page: https://github.com/ScreenPyHQ/screenpy_adapter_allure
-Author: Perry Goy
-Author-email: perry.goy@gmail.com
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: BDD
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ScreenPy Adapter: Allure
 ========================
 
 ```
 TITLE CARD:
                          "ScreenPy Adapter: Allure"
 TITLE DISAPPEARS.
```

### Comparing `screenpy_adapter_allure-4.0.2/screenpy_adapter_allure/adapters.py` & `screenpy_adapter_allure-4.0.3/screenpy_adapter_allure/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 import allure
 from allure_commons._allure import StepContext
 from allure_commons._core import plugin_manager
 from allure_commons.utils import now
 from allure_pytest.listener import AllureListener
 from allure_pytest.utils import get_status, get_status_details
 from screenpy.exceptions import UnableToNarrate
-from screenpy.narration import narrator
+from screenpy.narration.gravitas import AIRY, EXTREME, HEAVY, LIGHT, NORMAL
 
 
 class AllureAdapter:
     """Adapt the Narrator's microphone to allow narration to Allure."""
 
     step_stack: List[StepContext]
 
     GRAVITAS = {
-        narrator.AIRY: allure.severity_level.TRIVIAL,
-        narrator.LIGHT: allure.severity_level.MINOR,
-        narrator.NORMAL: allure.severity_level.NORMAL,
-        narrator.HEAVY: allure.severity_level.CRITICAL,
-        narrator.EXTREME: allure.severity_level.BLOCKER,
+        AIRY: allure.severity_level.TRIVIAL,
+        LIGHT: allure.severity_level.MINOR,
+        NORMAL: allure.severity_level.NORMAL,
+        HEAVY: allure.severity_level.CRITICAL,
+        EXTREME: allure.severity_level.BLOCKER,
     }
 
     def __init__(self) -> None:
         self.step_stack = []
 
     def _get_allure_plugin(self) -> AllureListener:
         """Retrieve the AllureListener plugin, probably to log an error."""
```

