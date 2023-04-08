# Comparing `tmp/audius-py-0.1.4.tar.gz` & `tmp/audius-py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audius-py-0.1.4.tar", last modified: Sun Apr  2 16:03:37 2023, max compression
+gzip compressed data, was "audius-py-0.1.5.tar", last modified: Sat Apr  8 18:26:59 2023, max compression
```

## Comparing `audius-py-0.1.4.tar` & `audius-py-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.332064 audius-py-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.332064 audius-py-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.332064 audius-py-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-02 16:03:20.000000 audius-py-0.1.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-02 16:03:20.000000 audius-py-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-02 16:03:20.000000 audius-py-0.1.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-02 16:03:20.000000 audius-py-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-02 16:03:37.336064 audius-py-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-02 16:03:20.000000 audius-py-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/audius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/audius/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/tracks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/audius/player/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/player/af.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/player/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/player/vlc.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/playlists.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/tracks.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-02 16:03:20.000000 audius-py-0.1.4/audius/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-02 16:03:36.000000 audius-py-0.1.4/audius/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/audius_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-02 16:03:37.000000 audius-py-0.1.4/audius_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-02 16:03:20.000000 audius-py-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-02 16:03:37.336064 audius-py-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-02 16:03:20.000000 audius-py-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:37.336064 audius-py-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:03:20.000000 audius-py-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-02 16:03:20.000000 audius-py-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-02 16:03:20.000000 audius-py-0.1.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-02 16:03:20.000000 audius-py-0.1.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-02 16:03:20.000000 audius-py-0.1.4/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:59.001590 audius-py-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:58.997590 audius-py-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:58.997590 audius-py-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:58.997590 audius-py-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-08 18:26:46.000000 audius-py-0.1.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-08 18:26:46.000000 audius-py-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 18:26:46.000000 audius-py-0.1.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 18:26:46.000000 audius-py-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-08 18:26:59.001590 audius-py-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-08 18:26:46.000000 audius-py-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:58.997590 audius-py-0.1.5/audius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:58.997590 audius-py-0.1.5/audius/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:59.001590 audius-py-0.1.5/audius/player/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/player/af.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/player/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/player/vlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-08 18:26:46.000000 audius-py-0.1.5/audius/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:59.001590 audius-py-0.1.5/audius_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 18:26:58.000000 audius-py-0.1.5/audius_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 18:26:46.000000 audius-py-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 18:26:59.001590 audius-py-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-08 18:26:46.000000 audius-py-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:59.001590 audius-py-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:26:46.000000 audius-py-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-08 18:26:46.000000 audius-py-0.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-08 18:26:46.000000 audius-py-0.1.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-08 18:26:46.000000 audius-py-0.1.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-08 18:26:46.000000 audius-py-0.1.5/tests/test_sdk.py
```

### Comparing `audius-py-0.1.4/.github/ISSUE_TEMPLATE/bug.md` & `audius-py-0.1.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/ISSUE_TEMPLATE/feature.md` & `audius-py-0.1.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/PULL_REQUEST_TEMPLATE.md` & `audius-py-0.1.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/release-drafter.yml` & `audius-py-0.1.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/workflows/lint.yaml` & `audius-py-0.1.5/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/workflows/publish.yaml` & `audius-py-0.1.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.github/workflows/test.yaml` & `audius-py-0.1.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/.gitignore` & `audius-py-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/LICENSE` & `audius-py-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/PKG-INFO` & `audius-py-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audius-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interact with the Audius platform in Python and the terminal
 Home-page: https://github.com/unparalleled-js/audius-py
 Author: Juliya Smith <juliya@juliyasmith.com>
 Author-email: juliya@juliyasmith.com
 License: Apache-2.0
 Keywords: audius
 Platform: UNKNOWN
```

### Comparing `audius-py-0.1.4/README.md` & `audius-py-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/cli/__init__.py` & `audius-py-0.1.5/audius/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/cli/playlists.py` & `audius-py-0.1.5/audius/cli/playlists.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/cli/tips.py` & `audius-py-0.1.5/audius/cli/tips.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/cli/tracks.py` & `audius-py-0.1.5/audius/cli/tracks.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/cli/users.py` & `audius-py-0.1.5/audius/cli/users.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/client.py` & `audius-py-0.1.5/audius/client.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/client_factory.py` & `audius-py-0.1.5/audius/client_factory.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/config.py` & `audius-py-0.1.5/audius/config.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/exceptions.py` & `audius-py-0.1.5/audius/exceptions.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/player/__init__.py` & `audius-py-0.1.5/audius/player/__init__.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/player/af.py` & `audius-py-0.1.5/audius/player/af.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import os
-import subprocess
 import tempfile
 import threading
 import time
 from typing import TYPE_CHECKING
 
+from afplay import afplay, is_installed
+
 from audius.player.base import BasePlayer
 from audius.types import PlayerType
 
 if TYPE_CHECKING:
     from audius.sdk import Audius
 
 
 class AFPlayer(BasePlayer):
     def __init__(self, sdk: "Audius"):
         super().__init__(PlayerType.AFPLAY, sdk)
 
-    def is_available(self):
-        try:
-            subprocess.run("afplay", stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-            return True
-        except FileNotFoundError:
-            return False
+    def is_available(self) -> bool:
+        return is_installed()
 
     def play(self, url: str):
         download_url = self.client.get_redirect_url(url)
         with tempfile.NamedTemporaryFile(mode="w+b", delete=False) as _file:
             fd3 = os.dup(_file.fileno())
 
             def download():
                 self.sdk.tracks.download(download_url, fd3, hide_output=True)
 
             # Stream the song while playing it to prevent waiting
             # for entire track to finish download.
             thread = threading.Thread(target=download)
             thread.start()
-            time.sleep(5)  # Buffer
-            subprocess.Popen(["afplay", _file.name])
+            time.sleep(3)  # Buffer
+            afplay(_file.name)
             thread.join()
             time.sleep(1)
```

### Comparing `audius-py-0.1.4/audius/player/base.py` & `audius-py-0.1.5/audius/player/base.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/player/vlc.py` & `audius-py-0.1.5/audius/player/vlc.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/playlists.py` & `audius-py-0.1.5/audius/playlists.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/sdk.py` & `audius-py-0.1.5/audius/sdk.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/tips.py` & `audius-py-0.1.5/audius/tips.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/tracks.py` & `audius-py-0.1.5/audius/tracks.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius/users.py` & `audius-py-0.1.5/audius/users.py`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius_py.egg-info/PKG-INFO` & `audius-py-0.1.5/audius_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audius-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interact with the Audius platform in Python and the terminal
 Home-page: https://github.com/unparalleled-js/audius-py
 Author: Juliya Smith <juliya@juliyasmith.com>
 Author-email: juliya@juliyasmith.com
 License: Apache-2.0
 Keywords: audius
 Platform: UNKNOWN
```

### Comparing `audius-py-0.1.4/audius_py.egg-info/SOURCES.txt` & `audius-py-0.1.5/audius_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audius-py-0.1.4/audius_py.egg-info/requires.txt` & `audius-py-0.1.5/audius_py.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 requests<3,>=2.28.2
 click<9,>=8.1.3
 tqdm<5,>=4.65.0
+afplay-py<0.3,>=0.2.0
 
 [dev]
 pytest>=7.0
 black>=23.1.0
 mypy<2,>=1.0
 types-requests
 types-setuptools
```

### Comparing `audius-py-0.1.4/setup.py` & `audius-py-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     author_email="juliya@juliyasmith.com",
     url="https://github.com/unparalleled-js/audius-py",
     include_package_data=True,
     install_requires=[
         "requests>=2.28.2,<3",
         "click>=8.1.3,<9",
         "tqdm>=4.65.0,<5",
+        "afplay-py>=0.2.0,<0.3",
     ],
     python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["audius"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="audius",
```

### Comparing `audius-py-0.1.4/tests/conftest.py` & `audius-py-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

