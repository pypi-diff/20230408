# Comparing `tmp/home_assistant_streamdeck_yaml-2023.4.8.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.4.8.tar", last modified: Sat Apr  8 19:15:32 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.4.9.tar", last modified: Sat Apr  8 19:22:57 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.4.8.tar` & `home_assistant_streamdeck_yaml-2023.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.730496 home_assistant_streamdeck_yaml-2023.4.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.730496 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 19:15:32.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    45796 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:15:32.734496 home_assistant_streamdeck_yaml-2023.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    32493 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    35837 2023-04-08 19:15:15.000000 home_assistant_streamdeck_yaml-2023.4.8/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45796 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32493 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35837 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.github/release.py` & `home_assistant_streamdeck_yaml-2023.4.9/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.gitignore` & `home_assistant_streamdeck_yaml-2023.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/Dockerfile` & `home_assistant_streamdeck_yaml-2023.4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/LICENSE` & `home_assistant_streamdeck_yaml-2023.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2023.4.8
+Version: 2023.4.9
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/README.md` & `home_assistant_streamdeck_yaml-2023.4.9/README.md`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.4.9/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.4.9/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/configuration.yaml` & `home_assistant_streamdeck_yaml-2023.4.9/configuration.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.4.8
+Version: 2023.4.9
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.4.9/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/tests/state.json` & `home_assistant_streamdeck_yaml-2023.4.9/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.4.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.8/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.4.9/tests/test_examples.py`

 * *Files identical despite different names*

