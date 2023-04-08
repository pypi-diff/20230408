# Comparing `tmp/light-curve-python-0.7.1.tar.gz` & `tmp/light-curve-python-0.7.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light-curve-python-0.7.1.tar", last modified: Fri Mar 17 02:13:48 2023, max compression
+gzip compressed data, was "light-curve-python-0.7.2b0.tar", last modified: Fri Apr  7 22:27:38 2023, max compression
```

## Comparing `light-curve-python-0.7.1.tar` & `light-curve-python-0.7.2b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 02:13:48.612428 light-curve-python-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-03-17 02:13:36.000000 light-curve-python-0.7.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-17 02:13:36.000000 light-curve-python-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-03-17 02:13:48.612428 light-curve-python-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-03-17 02:13:36.000000 light-curve-python-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 02:13:48.612428 light-curve-python-0.7.1/light_curve_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-03-17 02:13:48.000000 light-curve-python-0.7.1/light_curve_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-03-17 02:13:48.000000 light-curve-python-0.7.1/light_curve_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 02:13:48.000000 light-curve-python-0.7.1/light_curve_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-17 02:13:48.000000 light-curve-python-0.7.1/light_curve_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 02:13:48.000000 light-curve-python-0.7.1/light_curve_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-03-17 02:13:36.000000 light-curve-python-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-03-17 02:13:48.612428 light-curve-python-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-03-17 02:13:36.000000 light-curve-python-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/light_curve_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 22:27:38.000000 light-curve-python-0.7.2b0/light_curve_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-04-07 22:27:38.683176 light-curve-python-0.7.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-07 22:27:26.000000 light-curve-python-0.7.2b0/setup.py
```

### Comparing `light-curve-python-0.7.1/Cargo.toml` & `light-curve-python-0.7.2b0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [package]
 name = "light-curve-python"
-version = "0.7.1"
+version = "0.7.2-beta.0"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
-rust-version = "1.60"
+rust-version = "1.62"
 
 [lib]
 name = "light_curve"
 crate-type = ["cdylib"]
 
 [profile.release]
 lto = true
@@ -28,30 +28,31 @@
 
 [dependencies]
 # it is a dependency of intel-mkl-tool, we pin it to temporary solve
 # https://github.com/rust-math/intel-mkl-src/issues/68
 anyhow = "<1.0.49"
 const_format = "0.2.30"
 conv = "0.3.3"
+enum-iterator = "1.1.0,<1.2.0" # 1.2.0 requires MSRV 1.63
 enumflags2 = { version = "0.7.5", features = ["serde"] }
 itertools = "0.10.5"
 macro_const = "0.1.0"
 ndarray = { version = "0.15.3", features = ["rayon"] }
 numpy = "0.18.0"
 num_cpus = "1.13.0"
 num-traits = "0.2"
-pyo3 = {version = "0.18.1", features = ["extension-module"]}
+pyo3 = {version = "0.18.2", features = ["extension-module", "multiple-pymethods"]}
 rand = "0.8.5"
 rand_xoshiro = "0.6.0"
 thiserror = "1.0.37"
 serde = { version = "1", features = ["derive"] }
 serde-pickle = "1"
 rayon = "1.6.1"
 unzip3 = "1.0.0"
 
 [dependencies.light-curve-dmdt]
 version = "0.7.1"
 features = ["serde"]
 
 [dependencies.light-curve-feature]
-version = "0.5.4"
+version = "0.5.5"
 default_features = false
```

### Comparing `light-curve-python-0.7.1/PKG-INFO` & `light-curve-python-0.7.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.7.1
+Version: 0.7.2b0
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `light-curve-python-0.7.1/light_curve_python.egg-info/PKG-INFO` & `light-curve-python-0.7.2b0/light_curve_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-curve-python
-Version: 0.7.1
+Version: 0.7.2b0
 Summary: An alias to light-curve package
 Home-page: http://github.com/hombit/light-curve
 Author: Konstantin Malanchev
 Author-email: hombit@gmail.com
 License: MIT
 Keywords: science,astrophysics
 Classifier: Intended Audience :: Science/Research
```

### Comparing `light-curve-python-0.7.1/setup.cfg` & `light-curve-python-0.7.2b0/setup.cfg`

 * *Files identical despite different names*

