# Comparing `tmp/wom_py-0.2.0.tar.gz` & `tmp/wom_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.2.0.tar", max compression
+gzip compressed data, was "wom_py-0.3.0.tar", max compression
```

## Comparing `wom_py-0.2.0.tar` & `wom_py-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-02-27 23:30:01.934817 wom_py-0.2.0/LICENSE
--rw-r--r--   0        0        0     1889 2023-02-27 23:30:01.934817 wom_py-0.2.0/README.md
--rw-r--r--   0        0        0     2157 2023-02-27 23:30:01.938817 wom_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4275 2023-02-27 23:30:02.062818 wom_py-0.2.0/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/_cli.py
--rw-r--r--   0        0        0     7795 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/client.py
--rw-r--r--   0        0        0     1447 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/constants.py
--rw-r--r--   0        0        0     7084 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/errors.py
--rw-r--r--   0        0        0     3118 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/__init__.py
--rw-r--r--   0        0        0     1555 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7364 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/groups/enums.py
--rw-r--r--   0        0        0     8889 2023-02-27 23:30:01.938817 wom_py-0.2.0/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/http.py
--rw-r--r--   0        0        0     1381 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1413 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/names/enums.py
--rw-r--r--   0        0        0     3780 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/names/models.py
--rw-r--r--   0        0        0     1734 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5471 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/players/enums.py
--rw-r--r--   0        0        0    11316 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2226 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/py.typed
--rw-r--r--   0        0        0     5607 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/result.py
--rw-r--r--   0        0        0     6420 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/routes.py
--rw-r--r--   0        0        0    33956 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/__init__.py
--rw-r--r--   0        0        0     2042 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/base.py
--rw-r--r--   0        0        0    20760 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/competitions.py
--rw-r--r--   0        0        0     3477 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/deltas.py
--rw-r--r--   0        0        0     3637 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/efficiency.py
--rw-r--r--   0        0        0    23384 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/groups.py
--rw-r--r--   0        0        0     5355 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/http.py
--rw-r--r--   0        0        0     4722 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/names.py
--rw-r--r--   0        0        0    17519 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/players.py
--rw-r--r--   0        0        0     3455 2023-02-27 23:30:01.942817 wom_py-0.2.0/wom/services/records.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 wom_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-08 19:46:24.132712 wom_py-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-08 19:46:24.132712 wom_py-0.3.0/README.md
+-rw-r--r--   0        0        0     2138 2023-04-08 19:46:24.132712 wom_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4295 2023-04-08 19:46:24.212712 wom_py-0.3.0/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/_cli.py
+-rw-r--r--   0        0        0     7795 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/constants.py
+-rw-r--r--   0        0        0     7140 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/errors.py
+-rw-r--r--   0        0        0     3138 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7364 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9075 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/http.py
+-rw-r--r--   0        0        0     1381 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/enums.py
+-rw-r--r--   0        0        0     3778 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11832 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/py.typed
+-rw-r--r--   0        0        0     5509 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/result.py
+-rw-r--r--   0        0        0     6420 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/routes.py
+-rw-r--r--   0        0        0    33973 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/__init__.py
+-rw-r--r--   0        0        0     2042 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/base.py
+-rw-r--r--   0        0        0    20760 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/competitions.py
+-rw-r--r--   0        0        0     3477 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/deltas.py
+-rw-r--r--   0        0        0     3637 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/efficiency.py
+-rw-r--r--   0        0        0    23384 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/groups.py
+-rw-r--r--   0        0        0     5355 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/http.py
+-rw-r--r--   0        0        0     4722 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/names.py
+-rw-r--r--   0        0        0    17519 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/players.py
+-rw-r--r--   0        0        0     3455 2023-04-08 19:46:24.136712 wom_py-0.3.0/wom/services/records.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.0/PKG-INFO
```

### Comparing `wom_py-0.2.0/LICENSE` & `wom_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/README.md` & `wom_py-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 An asynchronous wrapper for the [Wise Old Man API](https://docs.wiseoldman.net/).
 
 The library aims to make it easy to interact with the Wise Old Man API by
 providing service methods for all available endpoints and model classes
 for data consistency.
 
+Python version 3.8 or greater is required to use wom.py.
+
 ## Disclaimer
 
-The library is in early development, and as such features or public interfaces
-may change at any time. Thanks for following our progress!
+The library is still in Beta, and as such features or public interfaces
+may change at any time. Thanks for checking out the project!
 
 ## Documentation
 
 - [Stable](https://jonxslays.github.io/wom.py/)
 - [Development](https://jonxslays.github.io/wom.py/dev/)
 
 ## Installation
@@ -28,14 +30,20 @@
 
 ```sh
 pip install -U git+https://github.com/Jonxslays/wom.py
 ```
 
 For more information on using `pip`, check out the [pip documentation](https://pip.pypa.io/en/stable/).
 
+## Problems
+
+If you're experiencing a problem with the library, please open an issue
+[here](https://github.com/Jonxslays/wom.py/issues), after first confirming
+a similar issue was not already created.
+
 ## What is Wise Old Man
 
 Wise Old Man is an open source Oldschool Runescape player progress tracker.
 
 If you're interested in learning more about the Wise Old Man project, consider checking out any of these links:
 
 - [Website](https://wiseoldman.net/)
@@ -49,20 +57,14 @@
 - Experience tracking
 - Boss killcounts
 - Player achievements
 - Group competitions
 - Global leaderboards
 - A discord bot for interacting with the API
 
-## Problems
-
-If you're experiencing a problem with the library, please open an issue
-[here](https://github.com/Jonxslays/wom.py/issues), after first confirming
-a similar issue was not already created.
-
 ## Contributing
 
 wom.py is open to contributions.
 
 Come back soon™ once I've written the contributing guide.
 
 ## License
```

### Comparing `wom_py-0.2.0/pyproject.toml` & `wom_py-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.2.0"
+version = "0.3.0"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
 packages = [
     { include = "wom" },
     { include = "wom/py.typed" },
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -65,19 +65,19 @@
 [tool.len8]
 include = ["noxfile.py", "tests", "wom"]
 code-length = 99
 docs-length = 80
 strict = true
 
 [tool.mypy]
-packages = ["wom", "tests"]
+packages = ["wom"]
 strict = true
 
 [tool.pyright]
-include = ["wom", "tests"]
+include = ["wom"]
 typeCheckingMode = "strict"
 reportImportCycles = false
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [build-system]
```

### Comparing `wom_py-0.2.0/wom/__init__.py` & `wom_py-0.3.0/wom/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     "PlayerGains",
     "PlayerGainsData",
     "PlayerMembership",
     "Player",
     "PlayerDetail",
     "PlayerParticipation",
     "PlayerService",
+    "PlayerStatus",
     "PlayerType",
     "Record",
     "RecordService",
     "RecordLeaderboardEntry",
     "Result",
     "Route",
     "Serializer",
@@ -129,23 +130,23 @@
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.2.0"
+__version__: Final[str] = "0.3.0"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[4d74373]"
+__git_sha__: Final[str] = "[7403fdf]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.2.0/wom/__main__.py` & `wom_py-0.3.0/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/_cli.py` & `wom_py-0.3.0/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/client.py` & `wom_py-0.3.0/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/constants.py` & `wom_py-0.3.0/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/enums.py` & `wom_py-0.3.0/wom/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,18 @@
     !!! tip
 
         Will always be one of [`Activities`][wom.Activities],
         [`Bosses`][wom.Bosses], [`ComputedMetrics`][wom.ComputedMetrics],
         or [`Skills`][wom.Skills].
     """
 
-    @classmethod
-    def _filter_on_value(cls: t.Type[T], value: str) -> set[T]:
-        return set(filter(lambda x: x.value == value, cls))  # type: ignore
+    # TODO: Do we even need this method??????????
+    # @classmethod
+    # def _filter_on_value(cls: t.Type[T], value: str) -> set[T]:
+    #     return set(filter(lambda x: x.value == value, cls))  # type: ignore
 
     @classmethod
     def from_str(cls: t.Type[T], value: str) -> T:
         if cls is not Metric:
             return cls(value)
 
         children = {Skills, Activities, Bosses, ComputedMetrics}
```

### Comparing `wom_py-0.2.0/wom/errors.py` & `wom_py-0.3.0/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/__init__.py` & `wom_py-0.3.0/wom/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     "PlayerCompetitionStanding",
     "PlayerMembership",
     "Player",
     "PlayerDetail",
     "PlayerGains",
     "PlayerGainsData",
     "PlayerParticipation",
+    "PlayerStatus",
     "PlayerType",
     "Record",
     "RecordLeaderboardEntry",
     "Skill",
     "SkillGains",
     "SkillLeader",
     "SnapshotData",
```

### Comparing `wom_py-0.2.0/wom/models/base.py` & `wom_py-0.3.0/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/competitions/__init__.py` & `wom_py-0.3.0/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/competitions/enums.py` & `wom_py-0.3.0/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/competitions/models.py` & `wom_py-0.3.0/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/deltas/__init__.py` & `wom_py-0.3.0/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/deltas/models.py` & `wom_py-0.3.0/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/groups/__init__.py` & `wom_py-0.3.0/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/groups/enums.py` & `wom_py-0.3.0/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/groups/models.py` & `wom_py-0.3.0/wom/models/groups/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -313,28 +313,32 @@
     """The player leading in this metric."""
 
 
 @attrs.define(init=False)
 class MetricLeaders(BaseModel):
     """The leaders for each metric in a group."""
 
-    skills: list[SkillLeader]
-    """A list of [`SkillLeader`][wom.SkillLeader]'s for each skill."""
+    skills: dict[enums.Skills, SkillLeader]
+    """A mapping of [`Skills`][wom.Skills] keys to [`SkillLeader`]
+    [wom.SkillLeader] values.
+    """
 
-    bosses: list[BossLeader]
-    """A list of all [`BossLeader`][wom.BossLeader]'s for each boss."""
+    bosses: dict[enums.Bosses, BossLeader]
+    """A mapping of [`Bosses`][wom.Bosses] keys to [`BossLeader`]
+    [wom.BossLeader] values.
+    """
 
-    activities: list[ActivityLeader]
-    """A list of all [`ActivityLeader`][wom.ActivityLeader]'s for each
-    activity.
+    activities: dict[enums.Activities, ActivityLeader]
+    """A mapping of [`Activities`][wom.Activities] keys to [`ActivityLeader`]
+    [wom.ActivityLeader] values.
     """
 
-    computed: list[ComputedMetricLeader]
-    """A list of all [`ComputedMetricLeader`]
-    [wom.ComputedMetricLeader]'s for each computed metric.
+    computed: dict[enums.ComputedMetrics, ComputedMetricLeader]
+    """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
+    [`ComputedMetricLeader`][wom.ComputedMetricLeader] values.
     """
 
 
 @attrs.define(init=False)
 class GroupStatistics(BaseModel):
     """Represents accumulated group statistics."""
 
@@ -347,10 +351,10 @@
     maxed_200ms_count: int
     """The number of maxed 200M xp players in the group."""
 
     average_stats: Snapshot
     """The average group statistics in a [`Snapshot`][wom.Snapshot]."""
 
     metric_leaders: MetricLeaders
-    """The [`MetricLeader`][wom.MetricLeaders]'s in this group for each
+    """The [`MetricLeaders`][wom.MetricLeaders] in this group for each
     metric.
     """
```

### Comparing `wom_py-0.2.0/wom/models/http.py` & `wom_py-0.3.0/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/names/__init__.py` & `wom_py-0.3.0/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/names/enums.py` & `wom_py-0.3.0/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/names/models.py` & `wom_py-0.3.0/wom/models/names/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,33 @@
 
 @attrs.define(init=False)
 class NameChange(BaseModel):
     """Represents a player name change."""
 
     id: int
     """The unique ID of this name change."""
+
     player_id: int
     """The player ID associated with the name change."""
+
     old_name: str
     """The old username of the player."""
+
     new_name: str
     """The new username of the player."""
+
     status: NameChangeStatus
-    """The [`status`][wom.NameChangeStatus] of the name
-    change.
-    """
+    """The [`status`][wom.NameChangeStatus] of the name change."""
+
     resolved_at: datetime | None
     """The date the name change was approved or denied."""
+
     updated_at: datetime
     """The date the name change was updated."""
+
     created_at: datetime
     """The date the name change was created."""
 
 
 @attrs.define(init=False)
 class NameChangeData(BaseModel):
     """Metadata associated with a name change."""
```

### Comparing `wom_py-0.2.0/wom/models/players/__init__.py` & `wom_py-0.3.0/wom/models/players/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "Gains",
     "PlayerAchievementProgress",
     "PlayerBuild",
     "PlayerGains",
     "PlayerGainsData",
     "Player",
     "PlayerDetail",
+    "PlayerStatus",
     "PlayerType",
     "SkillGains",
     "Skill",
     "SnapshotData",
     "Snapshot",
 )
```

### Comparing `wom_py-0.2.0/wom/models/players/enums.py` & `wom_py-0.3.0/wom/models/players/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from wom.enums import BaseEnum
 
 __all__ = (
     "AchievementMeasure",
     "Country",
     "PlayerBuild",
+    "PlayerStatus",
     "PlayerType",
 )
 
 
 class PlayerType(BaseEnum):
     """Different types of players."""
 
@@ -49,14 +50,23 @@
     F2p = "f2p"
     Lvl3 = "lvl3"
     Zerker = "zerker"
     Def1 = "def1"
     Hp10 = "hp10"
 
 
+class PlayerStatus(BaseEnum):
+    """Status for the players account."""
+
+    Active = "active"
+    Unranked = "unranked"
+    Flagged = "flagged"
+    Archived = "archived"
+
+
 class AchievementMeasure(BaseEnum):
     """Measures used to categorize achievements."""
 
     Levels = "levels"
     Experience = "experience"
     Kills = "kills"
     Score = "score"
```

### Comparing `wom_py-0.2.0/wom/models/players/models.py` & `wom_py-0.3.0/wom/models/players/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from wom import enums
 
 from ..base import BaseModel
 from .enums import AchievementMeasure
 from .enums import Country
 from .enums import PlayerBuild
+from .enums import PlayerStatus
 from .enums import PlayerType
 
 __all__ = (
     "Achievement",
     "AchievementProgress",
     "ActivityGains",
     "Activity",
@@ -68,15 +69,15 @@
 
     level: int
     """The players level in the skill."""
 
     experience: int
     """The players experience in the skill."""
 
-    ehp: int
+    ehp: float
     """The players efficient hours played for the skill."""
 
 
 @attrs.define(init=False)
 class Boss(BaseModel):
     """Details regarding a particular boss."""
 
@@ -85,15 +86,15 @@
 
     rank: int
     """The players rank in killing the boss."""
 
     kills: int
     """The number of kills the player has."""
 
-    ehb: int
+    ehb: float
     """The players efficient hours bossed for the boss."""
 
 
 @attrs.define(init=False)
 class Activity(BaseModel):
     """Details regarding a particular activity."""
 
@@ -115,40 +116,40 @@
     """The [`ComputedMetrics`][wom.ComputedMetrics] being
     measured.
     """
 
     rank: int
     """The players rank in the computed metric."""
 
-    value: int
+    value: float
     """The value of the computed metric."""
 
 
 @attrs.define(init=False)
 class SnapshotData(BaseModel):
     """The data associated with this snapshot."""
 
-    skills: list[Skill]
-    """A list of all [`Skills`][wom.Skill] stored in this
-    snapshot.
+    skills: dict[enums.Skills, Skill]
+    """A mapping of [`Skills`][wom.Skills] keys to [`Skill`][wom.Skill] values
+    from this snapshot.
     """
 
-    bosses: list[Boss]
-    """A list of all [`Bosses`][wom.Boss] stored in this
-    snapshot.
+    bosses: dict[enums.Bosses, Boss]
+    """A mapping of [`Bosses`][wom.Bosses] keys to [`Boss`][wom.Boss] values
+    from this snapshot.
     """
 
-    activities: list[Activity]
-    """A list of all [`Activities`][wom.Activity] stored in this
-    snapshot.
+    activities: dict[enums.Activities, Activity]
+    """A mapping of [`Activities`][wom.Activities] keys to [`Activity`]
+    [wom.Activity] values from this snapshot.
     """
 
-    computed: list[ComputedMetric]
-    """A list of all [`ComputedMetrics`][wom.ComputedMetric] stored in
-    this snapshot.
+    computed: dict[enums.ComputedMetrics, ComputedMetric]
+    """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
+    [`ComputedMetric`][wom.ComputedMetric] values from this snapshot.
     """
 
 
 @attrs.define(init=False)
 class Snapshot(BaseModel):
     """Represents a player snapshot."""
 
@@ -188,18 +189,16 @@
     """The [`PlayerBuild`][wom.PlayerBuild] for this player."""
 
     country: Country | None
     """The players [`Country`][wom.Country] country of origin, if they
     have one set.
     """
 
-    flagged: bool
-    """Whether the player is flagged for having an invalid snapshot
-    history.
-    """
+    status: PlayerStatus
+    """The players status, i.e. flagged, archived, etc."""
 
     exp: int
     """The players overall experience."""
 
     ehp: float
     """The players efficient hours played."""
 
@@ -425,25 +424,33 @@
     """The value [`Gains`][wom.Gains]."""
 
 
 @attrs.define(init=False)
 class PlayerGainsData(BaseModel):
     """Contains all the player gains data."""
 
-    skills: list[SkillGains]
-    """A list of all [`SkillGains`][wom.SkillGains]."""
+    skills: dict[enums.Skills, SkillGains]
+    """A mapping of [`Skills`][wom.Skills] keys to [`SkillGains`]
+    [wom.SkillGains] values.
+    """
 
-    bosses: list[BossGains]
-    """A list of all [`BossGains`][wom.BossGains]."""
+    bosses: dict[enums.Bosses, BossGains]
+    """A mapping of [`Bosses`][wom.Bosses] keys to [`BossGains`]
+    [wom.BossGains] values.
+    """
 
-    activities: list[ActivityGains]
-    """A list of all [`ActivityGains`][wom.ActivityGains]."""
+    activities: dict[enums.Activities, ActivityGains]
+    """A mapping of [`Activities`][wom.Activities] keys to [`ActivityGains`]
+    [wom.ActivityGains] values.
+    """
 
-    computed: list[ComputedGains]
-    """A list of all [`ComputedGains`][wom.ComputedGains]."""
+    computed: dict[enums.ComputedMetrics, ComputedGains]
+    """A mapping of [`ComputedMetrics`][wom.ComputedMetrics] keys to
+    [`ComputedGains`] [wom.ComputedGains] values.
+    """
 
 
 @attrs.define(init=False)
 class PlayerGains(BaseModel):
     """Gains made by a player."""
 
     starts_at: datetime
```

### Comparing `wom_py-0.2.0/wom/models/records/__init__.py` & `wom_py-0.3.0/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/models/records/models.py` & `wom_py-0.3.0/wom/models/records/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
     id: int
     """The unique ID for this record."""
 
     player_id: int
     """The player ID associated with this record."""
 
     period: enums.Period
-    """The [`Period`][wom.Period] over which this record was
-    achieved.
-    """
+    """The [`Period`][wom.Period] over which this record was achieved."""
 
     metric: enums.Metric
     """The [`Metric`][wom.Metric] measured in this record."""
 
     value: int
     """The records gained value."""
```

### Comparing `wom_py-0.2.0/wom/result.py` & `wom_py-0.3.0/wom/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,21 +66,16 @@
     !!! note
 
         This class cannot be instantiated, only its variants can be.
     """
 
     __slots__ = ("_error", "_value")
 
-    def __init__(self, value: T, error: E) -> None:
-        # This is really only here because mypy cant infer from slots
-        self._value = value
-        self._error = error
-
     def __repr__(self) -> str:
-        inner = self._value if self.is_ok else self._error
+        inner = self._value if self.is_ok else self._error  # type: ignore [attr-defined]
         return f"{self.__class__.__name__}({inner})"
 
     @property
     @abc.abstractmethod
     def is_ok(self) -> bool:
         """`True` if this result is the [`Ok`][wom.Ok] variant."""
 
@@ -151,15 +146,16 @@
     def unwrap_err(self) -> E:
         """Always throws an exception for the [`Ok`][wom.Ok] variant.
 
         Raises:
             UnwrapError: Because the result was an [`Ok`][wom.Ok]
                 variant.
         """
-        raise errors.UnwrapError(f"Called unwrap error on an non error value - {self._value}")
+        actual = self._value.__class__.__name__
+        raise errors.UnwrapError(f"Called unwrap error on a non error value of type {actual!r}")
 
 
 @t.final
 class Err(Result[T, E]):
     """The [`Err`][wom.Err] variant of a [`Result`][wom.Result].
 
     !!! info
```

### Comparing `wom_py-0.2.0/wom/routes.py` & `wom_py-0.3.0/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/serializer.py` & `wom_py-0.3.0/wom/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,29 @@
 from wom import models
 
 __all__ = ("Serializer",)
 
 T = t.TypeVar("T")
 TransformT = t.Callable[[t.Any], t.Any] | None
 AchievementT = t.TypeVar("AchievementT", models.Achievement, models.AchievementProgress)
+HasMetricsT = t.TypeVar(
+    "HasMetricsT",
+    models.Skill,
+    models.Boss,
+    models.Activity,
+    models.ComputedMetric,
+    models.SkillLeader,
+    models.BossLeader,
+    models.ActivityLeader,
+    models.ComputedMetricLeader,
+    models.SkillGains,
+    models.BossGains,
+    models.ActivityGains,
+    models.ComputedGains,
+)
 
 
 class Serializer:
     """Deserializes JSON data into wom.py model classes."""
 
     __slots__ = ()
 
@@ -49,14 +64,19 @@
     def _dt_from_iso_maybe(self, timestamp: str | None) -> datetime | None:
         return self._dt_from_iso(timestamp) if timestamp else None
 
     def _to_camel_case(self, attr: str) -> str:
         first, *rest = attr.split("_")
         return "".join((first.lower(), *map(str.title, rest)))
 
+    def __map(
+        self, serializer: t.Callable[[dict[str, t.Any]], HasMetricsT], data: list[dict[str, t.Any]]
+    ) -> dict[t.Any, HasMetricsT]:
+        return {x.metric: x for x in (serializer(y) for y in data)}
+
     def _set_attrs(
         self,
         model: t.Any,
         data: dict[str, t.Any],
         *attrs: str,
         transform: TransformT = None,
         camel_case: bool = False,
@@ -120,24 +140,24 @@
         player = models.Player()
         self._set_attrs_cased(
             player,
             data,
             "id",
             "username",
             "display_name",
-            "flagged",
             "exp",
             "ehp",
             "ehb",
             "ttm",
             "tt200m",
         )
 
         player.type = models.PlayerType.from_str(data["type"])
         player.build = models.PlayerBuild.from_str(data["build"])
+        player.status = models.PlayerStatus.from_str(data["status"])
         player.country = models.Country.from_str_maybe(data["country"])
         player.registered_at = self._dt_from_iso(data["registeredAt"])
         player.updated_at = self._dt_from_iso(data["updatedAt"])
         player.last_changed_at = self._dt_from_iso_maybe(data["lastChangedAt"])
         player.last_imported_at = self._dt_from_iso_maybe(data["lastImportedAt"])
         return player
 
@@ -168,50 +188,29 @@
         snapshot = models.Snapshot()
         snapshot.created_at = self._dt_from_iso(data["createdAt"])
         snapshot.imported_at = self._dt_from_iso_maybe(data.get("importedAt"))
         snapshot.data = self.deserialize_snapshot_data(data["data"])
         self._set_attrs_cased(snapshot, data, "id", "player_id")
         return snapshot
 
-    def gather(
-        self, serializer: t.Callable[[dict[str, t.Any]], T], data: list[dict[str, t.Any]]
-    ) -> list[T]:
-        """Calls the serializer on each mapping passed in.
-
-        Args:
-            serializer: The deserialization function to use.
-
-            data: The collection of items to deserialize.
-
-        Returns:
-            A list of the deserialized items.
-        """
-        return [serializer(item) for item in data]
-
     def deserialize_snapshot_data(self, data: dict[str, t.Any]) -> models.SnapshotData:
         """Deserializes the data into a snapshot data model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
-        snapshot_data = models.SnapshotData()
-        snapshot_data.skills = self.gather(self.deserialize_skill, data["skills"].values())
-        snapshot_data.bosses = self.gather(self.deserialize_boss, data["bosses"].values())
-        snapshot_data.activities = self.gather(
-            self.deserialize_activity, data["activities"].values()
-        )
-
-        snapshot_data.computed = self.gather(
-            self.deserialize_computed_metric, data["computed"].values()
-        )
-
-        return snapshot_data
+        model = models.SnapshotData()
+        model.skills = self.__map(self.deserialize_skill, data["skills"].values())
+        model.bosses = self.__map(self.deserialize_boss, data["bosses"].values())
+        model.activities = self.__map(self.deserialize_activity, data["activities"].values())
+        model.computed = self.__map(self.deserialize_computed_metric, data["computed"].values())
+        return model
 
     def deserialize_skill(self, data: dict[str, t.Any]) -> models.Skill:
         """Deserializes the data into a skill model.
 
         Args:
             data: The JSON payload.
 
@@ -405,21 +404,18 @@
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         gains = models.PlayerGainsData()
-        gains.skills = self.gather(self.deserialize_skill_gains, data["skills"].values())
-        gains.bosses = self.gather(self.deserialize_boss_gains, data["bosses"].values())
-        gains.computed = self.gather(self.deserialize_computed_gains, data["computed"].values())
-        gains.activities = self.gather(
-            self.deserialize_activity_gains, data["activities"].values()
-        )
-
+        gains.skills = self.__map(self.deserialize_skill_gains, data["skills"].values())
+        gains.bosses = self.__map(self.deserialize_boss_gains, data["bosses"].values())
+        gains.computed = self.__map(self.deserialize_computed_gains, data["computed"].values())
+        gains.activities = self.__map(self.deserialize_activity_gains, data["activities"].values())
         return gains
 
     def deserialize_player_gains(self, data: dict[str, t.Any]) -> models.PlayerGains:
         """Deserializes the data into a player gains model.
 
         Args:
             data: The JSON payload.
@@ -622,15 +618,15 @@
 
         Returns:
             The requested model.
         """
         details = models.GroupDetail()
         details.verification_code = None
         details.group = self.deserialize_group(data)
-        details.memberships = self.gather(self.deserialize_group_membership, data["memberships"])
+        details.memberships = [self.deserialize_group_membership(m) for m in data["memberships"]]
         return details
 
     def deserialize_group_hiscores_activity_item(
         self, data: dict[str, t.Any]
     ) -> models.GroupHiscoresActivityItem:
         """Deserializes the data into a group hiscores activity item
         model.
@@ -854,17 +850,17 @@
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         details = models.CompetitionDetail()
         details.competition = self.deserialize_competition(data)
-        details.participations = self.gather(
-            self.deserialize_competition_participation_detail, data["participations"]
-        )
+        details.participations = [
+            self.deserialize_competition_participation_detail(d) for d in data["participations"]
+        ]
 
         return details
 
     def deserialize_competition_participation_detail(
         self, data: dict[str, t.Any]
     ) -> models.CompetitionParticipationDetail:
         """Deserializes the data into a competition participation
@@ -907,17 +903,17 @@
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         progress = models.Top5ProgressResult()
         progress.player = self.deserialize_player(data["player"])
-        progress.history = self.gather(
-            self.deserialize_competition_history_data_point, data["history"]
-        )
+        progress.history = [
+            self.deserialize_competition_history_data_point(h) for h in data["history"]
+        ]
 
         return progress
 
     def deserialize_competition_with_participation(
         self, data: dict[str, t.Any]
     ) -> models.CompetitionWithParticipations:
         """Deserializes the data into a competition with participations
@@ -928,17 +924,17 @@
 
         Returns:
             The requested model.
         """
         model = models.CompetitionWithParticipations()
         model.verification_code = data.get("verificationCode")
         model.competition = self.deserialize_competition(data)
-        model.participations = self.gather(
-            self.deserialize_competition_participation, data["participations"]
-        )
+        model.participations = [
+            self.deserialize_competition_participation(p) for p in data["participations"]
+        ]
 
         return model
 
     def deserialize_skill_leader(self, data: dict[str, t.Any]) -> models.SkillLeader:
         """Deserializes the data into a skill leader model.
 
         Args:
@@ -995,24 +991,24 @@
         leader = models.ComputedMetricLeader()
         leader.metric = enums.ComputedMetrics.from_str(data["metric"])
         leader.player = self.deserialize_player(data["player"])
         self._set_attrs(leader, data, "value", "rank")
         return leader
 
     def deserialize_metric_leaders(self, data: dict[str, t.Any]) -> models.MetricLeaders:
-        """Deserializes the data into a metric leaders model model.
+        """Deserializes the data into a metric leaders model.
 
         Args:
             data: The JSON payload.
 
         Returns:
             The requested model.
         """
         leaders = models.MetricLeaders()
-        leaders.skills = self.gather(self.deserialize_skill_leader, data["skills"].values())
-        leaders.bosses = self.gather(self.deserialize_boss_leader, data["bosses"].values())
-        leaders.computed = self.gather(self.deserialize_computed_leader, data["computed"].values())
-        leaders.activities = self.gather(
+        leaders.skills = self.__map(self.deserialize_skill_leader, data["skills"].values())
+        leaders.bosses = self.__map(self.deserialize_boss_leader, data["bosses"].values())
+        leaders.computed = self.__map(self.deserialize_computed_leader, data["computed"].values())
+        leaders.activities = self.__map(
             self.deserialize_activity_leader, data["activities"].values()
         )
 
         return leaders
```

### Comparing `wom_py-0.2.0/wom/services/__init__.py` & `wom_py-0.3.0/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/base.py` & `wom_py-0.3.0/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/competitions.py` & `wom_py-0.3.0/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/deltas.py` & `wom_py-0.3.0/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/efficiency.py` & `wom_py-0.3.0/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/groups.py` & `wom_py-0.3.0/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/http.py` & `wom_py-0.3.0/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/names.py` & `wom_py-0.3.0/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/players.py` & `wom_py-0.3.0/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/wom/services/records.py` & `wom_py-0.3.0/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.2.0/PKG-INFO` & `wom_py-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -34,18 +34,20 @@
 
 An asynchronous wrapper for the [Wise Old Man API](https://docs.wiseoldman.net/).
 
 The library aims to make it easy to interact with the Wise Old Man API by
 providing service methods for all available endpoints and model classes
 for data consistency.
 
+Python version 3.8 or greater is required to use wom.py.
+
 ## Disclaimer
 
-The library is in early development, and as such features or public interfaces
-may change at any time. Thanks for following our progress!
+The library is still in Beta, and as such features or public interfaces
+may change at any time. Thanks for checking out the project!
 
 ## Documentation
 
 - [Stable](https://jonxslays.github.io/wom.py/)
 - [Development](https://jonxslays.github.io/wom.py/dev/)
 
 ## Installation
@@ -60,14 +62,20 @@
 
 ```sh
 pip install -U git+https://github.com/Jonxslays/wom.py
 ```
 
 For more information on using `pip`, check out the [pip documentation](https://pip.pypa.io/en/stable/).
 
+## Problems
+
+If you're experiencing a problem with the library, please open an issue
+[here](https://github.com/Jonxslays/wom.py/issues), after first confirming
+a similar issue was not already created.
+
 ## What is Wise Old Man
 
 Wise Old Man is an open source Oldschool Runescape player progress tracker.
 
 If you're interested in learning more about the Wise Old Man project, consider checking out any of these links:
 
 - [Website](https://wiseoldman.net/)
@@ -81,20 +89,14 @@
 - Experience tracking
 - Boss killcounts
 - Player achievements
 - Group competitions
 - Global leaderboards
 - A discord bot for interacting with the API
 
-## Problems
-
-If you're experiencing a problem with the library, please open an issue
-[here](https://github.com/Jonxslays/wom.py/issues), after first confirming
-a similar issue was not already created.
-
 ## Contributing
 
 wom.py is open to contributions.
 
 Come back soon™ once I've written the contributing guide.
 
 ## License
```

