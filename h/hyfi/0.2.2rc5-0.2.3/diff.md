# Comparing `tmp/hyfi-0.2.2rc5.tar.gz` & `tmp/hyfi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.2.2rc5.tar", max compression
+gzip compressed data, was "hyfi-0.2.3.tar", max compression
```

## Comparing `hyfi-0.2.2rc5.tar` & `hyfi-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1071 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/LICENSE
--rw-r--r--   0        0        0     1829 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/README.md
--rw-r--r--   0        0        0     3478 2023-03-01 22:45:13.896373 hyfi-0.2.2rc5/pyproject.toml
--rw-r--r--   0        0        0      270 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/__init__.py
--rw-r--r--   0        0        0       46 2023-03-01 22:45:13.836372 hyfi-0.2.2rc5/src/hyfi/_version.py
--rw-r--r--   0        0        0     1700 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/cli.py
--rw-r--r--   0        0        0        0 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0       21 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19380 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/env.py
--rw-r--r--   0        0        0    12911 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     5625 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26361 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/main.py
--rw-r--r--   0        0        0     2134 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/pipe.py
--rw-r--r--   0        0        0        0 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     2281 2023-03-01 22:45:13.036358 hyfi-0.2.2rc5/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9852 2023-03-01 22:45:13.040358 hyfi-0.2.2rc5/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.2.2rc5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-08 19:42:17.036810 hyfi-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1949 2023-04-08 19:42:17.036810 hyfi-0.2.3/README.md
+-rw-r--r--   0        0        0     3904 2023-04-08 19:53:16.816112 hyfi-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      270 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-08 19:53:16.756112 hyfi-0.2.3/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1700 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/cli.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19380 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/env.py
+-rw-r--r--   0        0        0    12911 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     5625 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26361 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/main.py
+-rw-r--r--   0        0        0     2134 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/pipe.py
+-rw-r--r--   0        0        0        0 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     2281 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9852 2023-04-08 19:42:17.040810 hyfi-0.2.3/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     3202 1970-01-01 00:00:00.000000 hyfi-0.2.3/PKG-INFO
```

### Comparing `hyfi-0.2.2rc5/LICENSE` & `hyfi-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/README.md` & `hyfi-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # HyFI: Hydra Fast Interface
 
-[![license-image]][license-url]
+[![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![jupyter-book-image]][jupyter book]
+[![license-image]][license-url]
 
 <!-- Links: -->
+[pypi-image]: https://badge.fury.io/py/hyfi.svg
+[pypi-url]: https://badge.fury.io/py/hyfi
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://conventionalcommits.org
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-[jupyter book]: https://jupyterbook.org
+[jupyter book]: https://hyfi.entelecheia.cc
 
 [repo-url]: https://github.com/entelecheia/hyfi
 [pypi-url]: https://pypi.org/project/hyfi
 [docs-url]: https://hyfi.entelecheia.cc
 [changelog]: https://github.com/entelecheia/hyfi/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi/blob/main/CONTRIBUTING.md
 <!-- Links: -->
```

### Comparing `hyfi-0.2.2rc5/pyproject.toml` & `hyfi-0.2.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.2.2-rc.5"
+version = "0.2.3"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
@@ -21,17 +21,24 @@
 matplotlib = "<=3.5.3"
 numpy = "<1.24"
 python-dotenv = "^1.0.0"
 gdown = "<=4.4.0"
 requests = "<=2.25.1"
 tqdm = "^4.64.1"
 cached-path = "^1.3.3"
-pygments = "<=2.6.1"
-ipython-autotime = "^0.3.1"
-ipython = "<=7.9.0"
+
+# A list of all of the optional dependencies, some of which are included in the
+# below `extras`. They can be opted into by apps.
+ipython = { version = "<=7.9.0", optional = true }
+ipython-autotime = { version = "^0.3.1", optional = true }
+rich = { version = ">=11.1", optional = true }
+pygments = { version = "<=2.6.1", optional = true }
+
+[tool.poetry.extras]
+ipython = ["ipython", "ipython-autotime", "rich", "pygments"]
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
@@ -45,41 +52,41 @@
     '_version.py',
     'node_modules',
     '_build',
     'docs',
     'tests',
     'venv',
     '.copier-template',
-    '.refs'
+    '.refs',
 ]
 
 [tool.isort]
 profile = "black"
 skip = [
     '_version.py',
     'node_modules',
     '_build',
     'docs',
     'tests',
     'venv',
     '.copier-template',
     '.refs',
-    "cpath"
+    "cpath",
 ]
 
 [tool.flake8]
 exclude = [
     "node_modules",
     "_build",
     "docs",
     "tests",
     "venv",
     ".copier-template",
     ".refs",
-    "cpath"
+    "cpath",
 ]
 per-file-ignores = [
     '__init__.py:F401,F403',
     '_version.py:W292',
     '*:E501,E203',
     'notebook.py:F821,E501',
     'motion.py:W605,E501',
@@ -93,15 +100,15 @@
     "_build",
     "dist",
     "docs",
     "tests",
     "venv",
     ".copier-template",
     ".refs",
-    "cpath"
+    "cpath",
 ]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = false
 disallow_any_expr = false
 disallow_any_decorated = false
@@ -141,21 +148,21 @@
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_variable = "src/hyfi/_version.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_source = "tag"
-commit_version_number = true # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "pip install poetry && poetry build"
-hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = 'setuptools.build_meta'
```

### Comparing `hyfi-0.2.2rc5/src/hyfi/cli.py` & `hyfi-0.2.3/src/hyfi/cli.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.2.3/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.2.3/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.2.3/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.2.3/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.2.3/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/config/batch.py` & `hyfi-0.2.3/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/env.py` & `hyfi-0.2.3/src/hyfi/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/hydra.py` & `hyfi-0.2.3/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/image/collage.py` & `hyfi-0.2.3/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/image/motion.py` & `hyfi-0.2.3/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/image/plot.py` & `hyfi-0.2.3/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/image/utils.py` & `hyfi-0.2.3/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/io/cached_path.py` & `hyfi-0.2.3/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/io/file.py` & `hyfi-0.2.3/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/main.py` & `hyfi-0.2.3/src/hyfi/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/pipe.py` & `hyfi-0.2.3/src/hyfi/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/batch/apply.py` & `hyfi-0.2.3/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.2.3/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/batch/batcher.py` & `hyfi-0.2.3/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/env.py` & `hyfi-0.2.3/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/func.py` & `hyfi-0.2.3/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/google.py` & `hyfi-0.2.3/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/gpu.py` & `hyfi-0.2.3/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/lib.py` & `hyfi-0.2.3/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/logging.py` & `hyfi-0.2.3/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/src/hyfi/utils/notebook.py` & `hyfi-0.2.3/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.2rc5/PKG-INFO` & `hyfi-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.2.2rc5
+Version: 0.2.3
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: ipython
 Requires-Dist: cached-path (>=1.3.3,<2.0.0)
 Requires-Dist: chardet (<=4.0.0)
 Requires-Dist: gdown (<=4.4.0)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
-Requires-Dist: ipython (<=7.9.0)
-Requires-Dist: ipython-autotime (>=0.3.1,<0.4.0)
+Requires-Dist: ipython (<=7.9.0) ; extra == "ipython"
+Requires-Dist: ipython-autotime (>=0.3.1,<0.4.0) ; extra == "ipython"
 Requires-Dist: matplotlib (<=3.5.3)
 Requires-Dist: numpy (<1.24)
 Requires-Dist: pandas (<1.4.0)
 Requires-Dist: pydantic (<=1.10.5)
-Requires-Dist: pygments (<=2.6.1)
+Requires-Dist: pygments (<=2.6.1) ; extra == "ipython"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (<=2.25.1)
+Requires-Dist: rich (>=11.1) ; extra == "ipython"
 Requires-Dist: scipy (<=1.8)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # HyFI: Hydra Fast Interface
 
-[![license-image]][license-url]
+[![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![jupyter-book-image]][jupyter book]
+[![license-image]][license-url]
 
 <!-- Links: -->
+[pypi-image]: https://badge.fury.io/py/hyfi.svg
+[pypi-url]: https://badge.fury.io/py/hyfi
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://conventionalcommits.org
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-[jupyter book]: https://jupyterbook.org
+[jupyter book]: https://hyfi.entelecheia.cc
 
 [repo-url]: https://github.com/entelecheia/hyfi
 [pypi-url]: https://pypi.org/project/hyfi
 [docs-url]: https://hyfi.entelecheia.cc
 [changelog]: https://github.com/entelecheia/hyfi/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi/blob/main/CONTRIBUTING.md
 <!-- Links: -->
```

