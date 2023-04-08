# Comparing `tmp/coverage-plot-0.2.0.tar.gz` & `tmp/coverage_plot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-plot-0.2.0.tar", max compression
+gzip compressed data, was "coverage_plot-0.3.0.tar", max compression
```

## Comparing `coverage-plot-0.2.0.tar` & `coverage_plot-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      394 2022-04-12 08:50:21.722669 coverage-plot-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1169 2022-04-12 07:55:50.079213 coverage-plot-0.2.0/README.md
--rw-r--r--   0        0        0      195 2022-04-12 08:50:21.722130 coverage-plot-0.2.0/coverage_plot/__init__.py
--rw-r--r--   0        0        0     1561 2021-01-13 12:47:10.022975 coverage-plot-0.2.0/coverage_plot/cli.py
--rw-r--r--   0        0        0     5358 2021-01-13 12:47:10.023431 coverage-plot-0.2.0/coverage_plot/git_changes.py
--rw-r--r--   0        0        0      496 2021-01-13 12:47:10.023902 coverage-plot-0.2.0/coverage_plot/importance_filesize.py
--rw-r--r--   0        0        0      356 2021-01-13 12:47:10.024783 coverage-plot-0.2.0/coverage_plot/importance_interface.py
--rw-r--r--   0        0        0     2915 2021-01-13 12:47:10.025254 coverage-plot-0.2.0/coverage_plot/importance_recency.py
--rw-r--r--   0        0        0     4537 2021-01-13 12:47:10.025733 coverage-plot-0.2.0/coverage_plot/plot.py
--rw-r--r--   0        0        0     1074 2022-04-12 08:50:21.721557 coverage-plot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2198 2022-04-12 09:03:06.504562 coverage-plot-0.2.0/setup.py
--rw-r--r--   0        0        0     2111 2022-04-12 09:03:06.504881 coverage-plot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-04-08 21:17:12.549876 coverage_plot-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1173 2023-04-08 21:14:22.312818 coverage_plot-0.3.0/README.md
+-rw-r--r--   0        0        0      195 2023-04-08 21:17:12.549693 coverage_plot-0.3.0/coverage_plot/__init__.py
+-rw-r--r--   0        0        0     1561 2023-04-08 10:42:16.322124 coverage_plot-0.3.0/coverage_plot/cli.py
+-rw-r--r--   0        0        0     1321 2023-04-08 21:14:22.313034 coverage_plot-0.3.0/coverage_plot/fake_implementations.py
+-rw-r--r--   0        0        0     5481 2023-04-08 21:14:22.313314 coverage_plot-0.3.0/coverage_plot/git_changes.py
+-rw-r--r--   0        0        0      490 2023-04-08 21:14:22.313609 coverage_plot-0.3.0/coverage_plot/importance_filesize.py
+-rw-r--r--   0        0        0      367 2023-04-08 21:14:22.313842 coverage_plot-0.3.0/coverage_plot/importance_interface.py
+-rw-r--r--   0        0        0     2920 2023-04-08 21:14:22.314033 coverage_plot-0.3.0/coverage_plot/importance_recency.py
+-rw-r--r--   0        0        0     4577 2023-04-08 21:14:22.314255 coverage_plot-0.3.0/coverage_plot/plot.py
+-rw-r--r--   0        0        0     1333 2023-04-08 21:17:12.549518 coverage_plot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 coverage_plot-0.3.0/PKG-INFO
```

### Comparing `coverage-plot-0.2.0/README.md` & `coverage_plot-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 [![Maintainability](https://api.codeclimate.com/v1/badges/0f758ae06864812dce12/maintainability)](https://codeclimate.com/github/imankulov/coverage-plot/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/coverage-plot/badge/?version=latest)](https://coverage-plot.readthedocs.io/en/latest/?badge=latest)
 
 A library and a script to plot Python code coverage results.
 
 ## Getting Started
 
-Run the tests for your project with the test coverage, and convert the coverage results to a JSON or XML format. As a result, you shoud find a coverage.json or coverage.xml file in your current working directory.
+Run the tests for your project with the test coverage, and convert the coverage results to a JSON or XML format. As a result, you should find a coverage.json or coverage.xml file in your current working directory.
 
 ```
-coverage run pytest
+coverage run -m pytest
 coverage xml  # or coverage json
 ```
 
 Install the package.
 
 ```
 pip install coverage-plot
 ```
 
-Run the coverage visualization. The script opens the browser with the visualization-results.
+Run the coverage visualization. The script opens the browser with the visualization results.
 
 ```
 coverage-plot coverage.xml
 ```
```

### Comparing `coverage-plot-0.2.0/coverage_plot/cli.py` & `coverage_plot-0.3.0/coverage_plot/cli.py`

 * *Files identical despite different names*

### Comparing `coverage-plot-0.2.0/coverage_plot/git_changes.py` & `coverage_plot-0.3.0/coverage_plot/git_changes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,138 @@
 import abc
 import enum
 import fnmatch
 from datetime import datetime, timezone
-from typing import Generator, Iterator, List, Optional
+from typing import Generator, Iterator, List, Optional, Union
 
-import attr
 import pydriller
+from attrs import frozen
 from pydriller import Commit, Modification
+from pydriller.domain.developer import Developer
+
+from coverage_plot.fake_implementations import (
+    FakeCommit,
+    FakeDeveloper,
+    FakeModification,
+)
+
+DeveloperT = Union[Developer, FakeDeveloper]
+CommitT = Union[Commit, FakeCommit]
+ModificationT = Union[Modification, FakeModification]
 
 
 class FilterResult(enum.Enum):
     INCLUDE = "INCLUDE"
     EXCLUDE = "EXCLUDE"
     DONT_KNOW = "DONT_KNOW"
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class NormalizedModification:
     hash: str
     msg: str
     author_name: str
     author_email: str
-    author_date: str
+    author_date: datetime
     path: str
 
     @classmethod
-    def from_commit_modification(cls, commit: Commit, modification: Modification):
+    def from_commit_modification(cls, commit: CommitT, modification: ModificationT):
         return NormalizedModification(
             hash=commit.hash,
             msg=commit.msg,
             author_name=commit.author.name,
             author_email=commit.author.email,
             author_date=commit.author_date.astimezone(timezone.utc).replace(
                 tzinfo=None
             ),
             path=modification.old_path or modification.new_path,
         )
 
 
 class CommitFilter(abc.ABC):
-    def filter_commit(self, commit: Commit) -> FilterResult:
+    @abc.abstractmethod
+    def filter_commit(self, commit: CommitT) -> FilterResult:
         ...
 
 
 class ModificationFilter(abc.ABC):
-    def filter_modification(self, modification: Modification) -> FilterResult:
+    @abc.abstractmethod
+    def filter_modification(self, modification: ModificationT) -> FilterResult:
         ...
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class ExcludeAuthor(CommitFilter):
     author_name: str
 
-    def filter_commit(self, commit: Commit) -> FilterResult:
+    def filter_commit(self, commit: CommitT) -> FilterResult:
         if self.author_name in commit.author.name:
             return FilterResult.EXCLUDE
         if self.author_name in commit.author.email:
             return FilterResult.EXCLUDE
         return FilterResult.DONT_KNOW
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class ExcludeMessage(CommitFilter):
     message: str
 
-    def filter_commit(self, commit: Commit) -> FilterResult:
+    def filter_commit(self, commit: CommitT) -> FilterResult:
         if self.message in commit.msg:
             return FilterResult.EXCLUDE
         return FilterResult.DONT_KNOW
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class ExcludeAllCommits(CommitFilter):
-    def filter_commit(self, commit: Commit) -> FilterResult:
+    def filter_commit(self, commit: CommitT) -> FilterResult:
         return FilterResult.EXCLUDE
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class IncludeAllCommits(CommitFilter):
-    def filter_commit(self, commit: Commit) -> FilterResult:
+    def filter_commit(self, commit: CommitT) -> FilterResult:
         return FilterResult.INCLUDE
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class IncludeFile(ModificationFilter):
-
     file_pattern: str
 
-    def filter_modification(self, modification: Modification) -> FilterResult:
+    def filter_modification(self, modification: ModificationT) -> FilterResult:
         path = modification.old_path or modification.new_path
         if fnmatch.fnmatch(path, self.file_pattern):
             return FilterResult.INCLUDE
         return FilterResult.DONT_KNOW
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class ExcludeAllModifications(ModificationFilter):
     """
     Catch-all filter to exclude all modifications.
 
     Add to the end of the list to filters to define the default behavior as
     "exclude the modification."
     """
 
-    def filter_modification(self, modification: Modification) -> FilterResult:
+    def filter_modification(self, modification: ModificationT) -> FilterResult:
         return FilterResult.EXCLUDE
 
 
-@attr.s(auto_attribs=True, frozen=True)
+@frozen
 class IncludeAllModifications(ModificationFilter):
     """
     Catch-all filter to incldue all modifications.
 
     Add to the end of the list to filters to define the default behavior as
     "include the modification."
     """
 
-    def filter_modification(self, modification: Modification) -> FilterResult:
+    def filter_modification(self, modification: ModificationT) -> FilterResult:
         return FilterResult.INCLUDE
 
 
 def get_git_changes(
     git_root: str,
     commit_filters: List[CommitFilter],
     modification_filters: List[ModificationFilter],
@@ -148,23 +160,23 @@
         for mod in commit.modifications:
             filter_result = apply_modification_filters(mod, modification_filters)
             if filter_result == FilterResult.EXCLUDE:
                 continue
             yield NormalizedModification.from_commit_modification(commit, mod)
 
 
-def apply_commit_filters(commit: Commit, commit_filters: List[CommitFilter]):
+def apply_commit_filters(commit: CommitT, commit_filters: List[CommitFilter]):
     for filt in commit_filters:
         result = filt.filter_commit(commit)
         if result in (FilterResult.INCLUDE, FilterResult.EXCLUDE):
             return result
     raise RuntimeError(f"Don't know what to do with commit {commit}")
 
 
 def apply_modification_filters(
-    modification: Modification, modification_filters: List[ModificationFilter]
+    modification: ModificationT, modification_filters: List[ModificationFilter]
 ):
     for filt in modification_filters:
         result = filt.filter_modification(modification)
         if result in (FilterResult.INCLUDE, FilterResult.EXCLUDE):
             return result
     raise RuntimeError(f"Don't know what to do with modification {modification}")
```

### Comparing `coverage-plot-0.2.0/coverage_plot/importance_recency.py` & `coverage_plot-0.3.0/coverage_plot/importance_recency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from datetime import MINYEAR, datetime, timedelta
 from typing import Dict, Iterator, List, cast
 
-import attr
+from attrs import define, field
 
 from coverage_plot.git_changes import (
     CommitFilter,
     ExcludeAllModifications,
     ExcludeAuthor,
     ExcludeMessage,
     IncludeAllCommits,
@@ -18,30 +18,30 @@
 from coverage_plot.importance_interface import Importance
 
 
 def year_ago():
     return datetime.utcnow() - timedelta(days=365)
 
 
-@attr.s(auto_attribs=True)
+@define
 class GitImportance(Importance):
     git_root: str
-    commit_filters: List[CommitFilter] = attr.ib(
+    commit_filters: List[CommitFilter] = field(
         factory=lambda: [
             ExcludeAuthor("bot"),
             ExcludeMessage("yapf"),
             ExcludeMessage("literals"),
             IncludeAllCommits(),
         ]
     )
-    modification_filters: List[ModificationFilter] = attr.ib(
+    modification_filters: List[ModificationFilter] = field(
         factory=lambda: [IncludeFile("*.py"), ExcludeAllModifications()]
     )
-    since: datetime = attr.ib(factory=year_ago)
-    last_modified_dict: Dict[str, datetime] = attr.ib(
+    since: datetime = field(factory=year_ago)
+    last_modified_dict: Dict[str, datetime] = field(
         factory=dict, init=False, repr=False
     )
 
     def __attrs_post_init__(self):
         git_changes = get_git_changes(
             self.git_root,
             self.commit_filters,
@@ -87,10 +87,11 @@
     """
     Take modifications and return the dict from filename to last modification timestamp.
     """
     sentinel = datetime(MINYEAR, 1, 1)
     last_modified_dict: Dict[str, datetime] = {}
     for mod in modifications:
         last_modified_dict[mod.path] = cast(
-            datetime, max(mod.author_date, last_modified_dict.get(mod.path, sentinel)),
+            datetime,
+            max(mod.author_date, last_modified_dict.get(mod.path, sentinel)),
         )
     return last_modified_dict
```

### Comparing `coverage-plot-0.2.0/coverage_plot/plot.py` & `coverage_plot-0.3.0/coverage_plot/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import os
 from typing import Dict
 from xml.etree import ElementTree as ET
 
-import attr
 import pandas as pd
 import plotly.express as px
+from attrs import frozen
 from plotly.graph_objs import Figure
 
 from coverage_plot.importance_interface import Importance
 
-# Coverare Report, where str is a filename, and "FileCoverage"
+# Coverage Report, where str is a filename, and "FileCoverage"
 # is the coverage result
 Report = Dict[str, "FileCoverage"]
 
 
 def import_json(content: str) -> Report:
     """Create a Report object from JSON-encoded content."""
     content_dict = json.loads(content)
@@ -75,15 +75,18 @@
             "path": filename,
             "name": os.path.basename(filename),
             "percent_covered": coverage.percent_covered(),
             "importance": imp,
         }
         records.append(record)
 
-    records = sorted(records, key=lambda k: k["path"])
+    def _sorter(record_: Dict) -> str:
+        return record_["path"]
+
+    records = sorted(records, key=_sorter)
     return pd.DataFrame(records)
 
 
 def make_path_components(report_df: pd.DataFrame) -> pd.DataFrame:
     """
     Generate a dataframe with path components.
     """
@@ -91,15 +94,15 @@
     def splitter(path):
         chunks = {f"p{i}": component for i, component in enumerate(path.split("/"))}
         return pd.Series(chunks)
 
     return report_df["path"].apply(splitter)
 
 
-@attr.s(frozen=True, auto_attribs=True)
+@frozen
 class FileCoverage:
     covered_lines: int = 0
     missing_lines: int = 0
 
     def total_lines(self) -> int:
         return self.covered_lines + self.missing_lines
```

### Comparing `coverage-plot-0.2.0/pyproject.toml` & `coverage_plot-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 [tool.poetry]
 name = "coverage-plot"
-version = "0.2.0"
+version = "0.3.0"
 description = "Library to plot Python code coverage results"
 readme = "README.md"
 homepage = "https://github.com/imankulov/coverage-plot"
 repository = "https://github.com/imankulov/coverage-plot"
 authors = ["Roman Imankulov <roman.imankulov@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 include = [
     "CHANGELOG.md"
 ]
 
 
 [tool.poetry.scripts]
 coverage-plot = "coverage_plot.cli:coverage_plot"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-plotly = "^4.8.2"
+python = "^3.8.1"
+plotly = "^5"
 pandas = "^1.0.5"
-attrs = "^19.3.0"
+attrs = ">=21.1.0"
 click = "^8.1.2"
 pydriller = "^1.15.2"
-sphinx = {version = "^3", optional = true}
+sphinx = { version = "^3", optional = true }
 
 [tool.poetry.extras]
 docs = ["sphinx"]
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.3.2"
-black = "^19.10b0"
-flake8 = "^3.7.9"
-mypy = "^0.782"
-coverage = {extras = ["toml"], version = "^5.2"}
-ipython = "^7.16.1"
-faker = "^4.1.1"
-pdbpp = "^0.10.2"
-sphinx = "^3.1.2"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.2"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+mypy = "^1.2.0"
+coverage = {extras = ["toml"], version = "^7.2.3"}
+faker = "^18.4.0"
 
 [tool.coverage.run]
 source = ["coverage_plot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coverage-plot-0.2.0/PKG-INFO` & `coverage_plot-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 Metadata-Version: 2.1
 Name: coverage-plot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library to plot Python code coverage results
 Home-page: https://github.com/imankulov/coverage-plot
 License: MIT
 Author: Roman Imankulov
 Author-email: roman.imankulov@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
-Requires-Dist: attrs (>=19.3.0,<20.0.0)
+Requires-Dist: attrs (>=21.1.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: pandas (>=1.0.5,<2.0.0)
-Requires-Dist: plotly (>=4.8.2,<5.0.0)
+Requires-Dist: plotly (>=5,<6)
 Requires-Dist: pydriller (>=1.15.2,<2.0.0)
-Requires-Dist: sphinx (>=3,<4); extra == "docs"
+Requires-Dist: sphinx (>=3,<4) ; extra == "docs"
 Project-URL: Repository, https://github.com/imankulov/coverage-plot
 Description-Content-Type: text/markdown
 
 # Coverage Plot
 
 [![codecov](https://codecov.io/gh/imankulov/coverage-plot/branch/master/graph/badge.svg)](https://codecov.io/gh/imankulov/coverage-plot)
 [![Coverage Status](https://coveralls.io/repos/github/imankulov/coverage-plot/badge.svg)](https://coveralls.io/github/imankulov/coverage-plot)
 [![Maintainability](https://api.codeclimate.com/v1/badges/0f758ae06864812dce12/maintainability)](https://codeclimate.com/github/imankulov/coverage-plot/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/coverage-plot/badge/?version=latest)](https://coverage-plot.readthedocs.io/en/latest/?badge=latest)
 
 A library and a script to plot Python code coverage results.
 
 ## Getting Started
 
-Run the tests for your project with the test coverage, and convert the coverage results to a JSON or XML format. As a result, you shoud find a coverage.json or coverage.xml file in your current working directory.
+Run the tests for your project with the test coverage, and convert the coverage results to a JSON or XML format. As a result, you should find a coverage.json or coverage.xml file in your current working directory.
 
 ```
-coverage run pytest
+coverage run -m pytest
 coverage xml  # or coverage json
 ```
 
 Install the package.
 
 ```
 pip install coverage-plot
 ```
 
-Run the coverage visualization. The script opens the browser with the visualization-results.
+Run the coverage visualization. The script opens the browser with the visualization results.
 
 ```
 coverage-plot coverage.xml
 ```
```

