# Comparing `tmp/oranchada-0.0.5.tar.gz` & `tmp/oranchada-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oranchada-0.0.5.tar", last modified: Wed Mar 15 18:03:27 2023, max compression
+gzip compressed data, was "oranchada-0.0.6.tar", last modified: Fri Apr  7 22:13:46 2023, max compression
```

## Comparing `oranchada-0.0.5.tar` & `oranchada-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.478734 oranchada-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-15 18:03:17.000000 oranchada-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-15 18:03:17.000000 oranchada-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-15 18:03:27.478734 oranchada-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-03-15 18:03:17.000000 oranchada-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-15 18:03:17.000000 oranchada-0.0.5/README.pypi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/oranchada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 18:03:27.000000 oranchada-0.0.5/oranchada.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/base_widget/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/arithmetic_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/creator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/filter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/base_widget/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/processings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/processings/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/processings/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/processings/gen_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/tests/process_spectra_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.474734 oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.478734 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/gen_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:03:27.478734 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/load_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/moving_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/remove_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/set_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-03-15 18:03:17.000000 oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 18:03:27.478734 oranchada-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-15 18:03:17.000000 oranchada-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 22:13:35.000000 oranchada-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-07 22:13:35.000000 oranchada-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-07 22:13:46.340067 oranchada-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-07 22:13:35.000000 oranchada-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-07 22:13:35.000000 oranchada-0.0.6/README.pypi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/oranchada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/base_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/arithmetic_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/creator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/filter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/processings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/gen_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/tests/process_spectra_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/gen_spe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/moving_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/remove_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/set_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:13:46.340067 oranchada-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-07 22:13:35.000000 oranchada-0.0.6/setup.py
```

### Comparing `oranchada-0.0.5/LICENSE` & `oranchada-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/PKG-INFO` & `oranchada-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.5
+Version: 0.0.6
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.5/README.md` & `oranchada-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/oranchada.egg-info/PKG-INFO` & `oranchada-0.0.6/oranchada.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.5
+Version: 0.0.6
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.5/oranchada.egg-info/SOURCES.txt` & `oranchada-0.0.6/oranchada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/base_widget/base_widget.py` & `oranchada-0.0.6/orangecontrib/oranchada/base_widget/base_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-from Orange.data import Table
-from Orange.widgets import gui
-from Orange.widgets.widget import OWBaseWidget, Output
-from Orange.data.pandas_compat import table_from_frame
-
-from AnyQt.QtWidgets import QSizePolicy
 import matplotlib.pyplot as plt
 import pandas as pd
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+from AnyQt.QtWidgets import QSizePolicy
+from matplotlib.backends.backend_qt5agg import \
+    FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qt5agg import \
+    NavigationToolbar2QT as NavigationToolbar
+from Orange.data import Table
+from Orange.data.pandas_compat import table_from_frame
+from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+from Orange.widgets.widget import Output, OWBaseWidget
 
 from .types import RC2Spectra
 
 
 class BaseWidget(OWBaseWidget, openclass=True):
     resizing_enabled = True
     priority = 10
 
+    should_auto_plot = Setting(False)
+    should_auto_proc = Setting(True)
+    should_pass_datatable = Setting(False)
+    should_plot_legend = Setting(True)
+
     def __init__(self):
         super().__init__()
         self.in_spe = RC2Spectra()
-        self.should_auto_plot = False
-        self.should_auto_proc = True
-        self.should_pass_datatable = False
         self.figure = None
         self.is_processed = False
         self.controlArea.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
         self.optionsBox = gui.widgetBox(self.controlArea, "Main Options")
         self.optionsBox.setDisabled(False)
         self.should_auto_plot_checkbox = gui.checkBox(self.optionsBox, self, "should_auto_plot", "Auto update plot",
                                                       stateWhenDisabled=False, callback=self.force_plot)
         pass_datatable = gui.checkBox(self.optionsBox, self, "should_pass_datatable", "Pass datatable",
                                       stateWhenDisabled=False, callback=self.process)
         gui.checkBox(self.optionsBox, self, "should_auto_proc", "Auto process",
                      disables=[self.should_auto_plot_checkbox, pass_datatable])
         gui.button(self.optionsBox, self, "Process", callback=self.process)
         gui.button(self.optionsBox, self, "Plot", callback=self.force_plot)
+        gui.checkBox(self.optionsBox, self, "should_plot_legend", "Plot legend", callback=self.auto_process)
 
     class Outputs:
         out_spe = Output("RC2Spectra", RC2Spectra, default=True)
         data = Output("Data", Table, default=False)
 
     def force_plot(self):
         if not self.is_processed:
@@ -58,27 +63,34 @@
             self.mainArea.layout().addWidget(self.canvas)
         for ax in self.figure.axes:
             self.figure.delaxes(ax)
         ax = self.plot_create_axes()
         for spe in self.out_spe:
             spe.plot(ax=ax, label=f'id(spe)={id(spe)}')
         self.custom_plot(ax)
+        if self.should_plot_legend:
+            ax.legend(fontsize='x-small', ncols=2)
+        else:
+            ax.legend([])
         self.canvas.draw()
 
     def custom_plot(self, ax):
         pass
 
-    def send_outputs(self):
-        self.Outputs.out_spe.send(self.out_spe)
+    def send_output_table(self):
         if self.should_pass_datatable:
             df = pd.DataFrame([pd.Series(index=spe.x, data=spe.y) for spe in self.out_spe])
             df = df.sort_index(axis='columns')
             df.columns = [f'{i}' for i in df.columns]
             self.Outputs.data.send(table_from_frame(df))
 
+    def send_outputs(self):
+        self.Outputs.out_spe.send(self.out_spe)
+        self.send_output_table()
+
     def process(self):
         self.is_processed = True
 
     def auto_process(self):
         self.is_processed = False
         if self.should_auto_proc:
             self.process()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/processings/add_baseline.py` & `oranchada-0.0.6/orangecontrib/oranchada/processings/add_baseline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import ramanchada2 as rc2
-import pydantic
 from typing import Union
+
+import pydantic
+import ramanchada2 as rc2
 from AnyQt.QtWidgets import QGroupBox
 from Orange.widgets import gui
 
 
 class AddBaseline:
     @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(self, parent, *,
@@ -20,33 +21,29 @@
         if n_freq[1]:
             self.n_freq = 15
             gui.spin(n_freq[1], self._parent, 'n_freq', 3, 5000,
                      callback=self.auto_process, label='num freq')
 
         self._amplitude = amplitude[0]
         if amplitude[1]:
-            self.amplitude = 2
             gui.doubleSpin(amplitude[1], self._parent, self._amplitude, 0, 5000, decimals=5, step=.01,
                            label='amplitude', callback=self.auto_process)
 
         self._intercept = intercept[0]
         if intercept[1]:
-            self.intercept = 10
             gui.doubleSpin(intercept[1], self._parent, self._intercept, -20000, 20000, decimals=5, step=1,
                            label='intercept', callback=self.auto_process)
 
         self._slope = slope[0]
         if slope[1]:
-            self.slope = .01
             gui.doubleSpin(slope[1], self._parent, self._slope, -1000, 1000, decimals=5, step=.001,
                            label='slope', callback=self.auto_process)
 
         self._quadratic = quadratic[0]
         if quadratic[1]:
-            self.quadratic = -.000005
             gui.doubleSpin(quadratic[1], self._parent, self._quadratic, -100, 100, decimals=7, step=.000001,
                            label='quadratic', callback=self.auto_process)
 
     @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __call__(self, spe: rc2.spectrum.Spectrum) -> rc2.spectrum.Spectrum:
         return spe.add_baseline(n_freq=self.n_freq,
                                 amplitude=self.amplitude,
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/processings/add_noise.py` & `oranchada-0.0.6/orangecontrib/oranchada/processings/add_noise.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from Orange.widgets import gui
-from AnyQt.QtWidgets import QGroupBox
-import ramanchada2 as rc2
+from typing import Union
 
 import pydantic
-from typing import Union
+import ramanchada2 as rc2
+from AnyQt.QtWidgets import QGroupBox
+from Orange.widgets import gui
 
 
 class AddNoise:
     @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def __init__(self, parent, *,
                  noise_scale: tuple[str, Union[None, QGroupBox]],
                  ):
         self._parent = parent
 
         self._noise_scale = noise_scale[0]
         if noise_scale[1]:
-            self.noise_scale = .01
             gui.doubleSpin(noise_scale[1], self._parent, self._noise_scale, 0, 100, decimals=5, step=.001,
                            callback=self.auto_process)
 
     def auto_process(self):
         self._parent.auto_process()
 
     @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/processings/gen_spe.py` & `oranchada-0.0.6/orangecontrib/oranchada/processings/gen_spe.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,35 +13,30 @@
                  spe_xmax: tuple[str, Union[None, QGroupBox]],
                  spe_nbins: tuple[str, Union[None, QGroupBox]],
                  deltas: tuple[str, Union[None, QGroupBox]],
                  ):
         self._parent = parent
 
         self._spe_xmin = spe_xmin[0]
-        self.spe_xmin = 0
         if spe_xmin[1]:
             gui.spin(spe_xmin[1], self._parent, self._spe_xmin, -1000, 10000, label='xmin', callback=self.auto_process)
 
         self._spe_xmax = spe_xmax[0]
-        self.spe_xmax = 2000
         if spe_xmax[1]:
             gui.spin(spe_xmax[1], self._parent, self._spe_xmax, -1000, 10000, label='xmax', callback=self.auto_process)
 
         self._spe_nbins = spe_nbins[0]
-        self.spe_nbins = 1500
         if spe_nbins[1]:
             gui.spin(spe_nbins[1], self._parent, self._spe_nbins, 1, 200000, label='n_bins', callback=self.auto_process)
 
         self._deltas = deltas[0]
         self._deltas_combo = deltas[0] + '_combo'
-        self.deltas = '1: 1'
         if deltas[1]:
             self.deltas_edit = gui.lineEdit(deltas[1], self._parent, self._deltas, label='Deltas',
                                             callback=self.auto_process)
-            self.deltas_combo = 'PST'
             gui.comboBox(deltas[1], self._parent, self._deltas_combo, sendSelectedValue=True,
                          items=['PST', 'User defined'], callback=self.set_deltas)
             self.set_deltas()
 
     def set_deltas(self):
         if self.deltas_combo == 'User defined':
             self.deltas_edit.setReadOnly(False)
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/tests/process_spectra_test.py` & `oranchada-0.0.6/orangecontrib/oranchada/tests/process_spectra_test.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 from Orange.widgets import gui
-from ..base_widget import CreatorWidget
+from Orange.widgets.settings import Setting
 
-from ..processings.gen_spe import GenSpe
+from ..base_widget import CreatorWidget
 from ..processings.add_baseline import AddBaseline
 from ..processings.add_noise import AddNoise
+from ..processings.gen_spe import GenSpe
 
 
 class GenNoisySpe(CreatorWidget):
     name = "Gen Noisy Spectra"
     description = "Generate spectra with baseline and noise"
     icon = "icons/spectra.svg"
 
+    # Generate Spectrum
+    spe_xmin = Setting(0)
+    spe_xmax = Setting(2000)
+    spe_nbins = Setting(1500)
+    deltas_combo = Setting('PST')
+    deltas = Setting('1: 1')
+
+    # Add baseline
+    n_freq = Setting(15)
+    amplitude = Setting(2)
+    intercept = Setting(10)
+    slope = Setting(.01)
+    quadratic = Setting(-.000005)
+
+    # Add noise
+    noise_scale = Setting(.01)
+
     def __init__(self):
         super().__init__()
         self.n_spectra = 1
         box = gui.widgetBox(self.controlArea, self.name)
         box_params = gui.widgetBox(box, 'Spe Params')
         self.gen_spe = GenSpe(self,
                               spe_xmin=('spe_xmin', box_params),
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_easy/icons/spectra.svg` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/add_baseline.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_baseline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 from ..processings.add_baseline import AddBaseline
 
 
 class AddBaselineOW(FilterWidget):
     name = "Add Baseline"
     description = "add baseline"
     icon = "icons/spectra.svg"
 
+    n_freq = Setting(15)
+    amplitude = Setting(2)
+    intercept = Setting(10)
+    slope = Setting(.01)
+    quadratic = Setting(-.000005)
+
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
         self.add_baseline = AddBaseline(self,
                                         n_freq=('n_freq', box),
                                         amplitude=('amplitude', box),
                                         intercept=('intercept', box),
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/add_noise.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_noise.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 from ..processings.add_noise import AddNoise
 
 
 class AddNoiseOW(FilterWidget):
     name = "Add Noise"
     description = "add noise"
     icon = "icons/spectra.svg"
 
+    noise_scale = Setting(.01)
+
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
         self.add_noise = AddNoise(self,
                                   noise_scale=('noise_scale', box))
 
     def process(self):
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/arithmetics_add.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_add.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/find_peaks.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/find_peaks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 from Orange.widgets import gui
-from ..base_widget import FilterWidget
+from Orange.widgets.settings import Setting
 from ramanchada2.misc.types.peak_candidates import ListPeakCandidateMultiModel
 
+from ..base_widget import FilterWidget
+
 
 class FindPeaks(FilterWidget):
     name = "Find Peaks"
     description = "Find Peaks"
     icon = "icons/spectra.svg"
 
+    prominence_val = Setting(5)
+    hht_chain_str = Setting('80 20')
+    is_sharpening_enabled = Setting(True)
+    wlen = Setting(200)
+    min_peak_width = Setting(2)
+
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
-        self.prominence_val = .02
-        self.hht_chain_str = '80 20'
-        self.manual_prominence = True
-        self.is_sharpening_enabled = True
-        self.prominence_val_spin = gui.doubleSpin(box, self, 'prominence_val', 0, 100, decimals=5,
-                                                  label='Prominence', step=.001, callback=self.auto_process)
-
-        gui.checkBox(box, self, "manual_prominence", "Manual Prominence", callback=self.auto_process,
-                     stateWhenDisabled=False, disables=self.prominence_val_spin)
-
         self.hht_chain_edit = gui.lineEdit(box, self, 'hht_chain_str', label='HHT Chain', callback=self.auto_process)
         gui.checkBox(box, self, "is_sharpening_enabled", "Enable shaprening", callback=self.auto_process,
                      stateWhenDisabled=False, disables=self.hht_chain_edit)
         self.is_sharpening_enabled = False
-        self.manual_prominence = False
 
-        self.wlen = 50
-        self.min_peak_width = 1
-        gui.spin(box, self, 'wlen', 1, 5000, callback=self.auto_process, label='Window length')
+        self.prominence_val_spin = gui.doubleSpin(box, self, 'prominence_val', 0, 1000, decimals=2,
+                                                  label='Prominence [×σ]', step=.5, callback=self.auto_process)
+        gui.spin(box, self, 'wlen', 1, 5000, step=20, callback=self.auto_process, label='Window length')
         gui.spin(box, self, 'min_peak_width', 1, 5000, callback=self.auto_process, label='Min peak width')
 
     def process(self):
         hht_chain = [int(i) for i in self.hht_chain_str.split()]
         self.hht_chain_str = ' '.join([str(i) for i in hht_chain])
         self.out_spe = list()
         for spe in self.in_spe:
+            prominence = spe.y_noise * self.prominence_val
             self.out_spe.append(
                 spe.find_peak_multipeak_filter(
                     wlen=self.wlen,
                     width=self.min_peak_width,
                     hht_chain=hht_chain,
                     sharpening=('hht' if self.is_sharpening_enabled else None),
-                    prominence=(self.prominence_val if self.manual_prominence else None))
+                    prominence=prominence)
                 )
         self.send_outputs()
 
     def custom_plot(self, ax):
         for spe in self.out_spe:
             ListPeakCandidateMultiModel.validate(spe.result).plot(ax)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/fit_peaks.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/fit_peaks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,54 @@
+import pandas as pd
 from Orange.data import Table
-from Orange.widgets.widget import Output
+from Orange.data.pandas_compat import table_from_frame
 from Orange.widgets import gui
-from ..base_widget import FilterWidget
-from ramanchada2.misc.types.peak_candidates import ListPeakCandidateMultiModel
+from Orange.widgets.settings import Setting
+from Orange.widgets.widget import Output
+from ramanchada2.misc.types.fit_peaks_result import FitPeaksResult
 from ramanchada2.spectrum.peaks.fit_peaks import available_models
-# from Orange.data.pandas_compat import table_from_frame
+
+from ..base_widget import FilterWidget
 
 
 class Fit(FilterWidget):
     name = "Fit Peaks"
     description = "Fit Peaks"
     icon = "icons/spectra.svg"
 
+    should_fit = Setting(True)
+    vary_baseline = Setting(False)
+    peak_profile = Setting(available_models[0])
+    plot_individual_peaks = Setting(False)
+    should_auto_proc = Setting(False)
+
     class Outputs(FilterWidget.Outputs):
         peaks_out = Output("Peaks", Table, default=False)
 
     def __init__(self):
         super().__init__()
-        self.should_auto_proc = False
         box = gui.widgetBox(self.controlArea, self.name)
-        self.should_fit = True
-        self.vary_baseline = False
-        self.peak_profile = available_models[0]
 
         gui.checkBox(box, self, "should_fit", "Perform fit", callback=self.auto_process)
+        gui.checkBox(box, self, "plot_individual_peaks", "Plot individual peaks", callback=self.auto_process)
         gui.checkBox(box, self, "vary_baseline", "Vary baseline", callback=self.auto_process)
         gui.comboBox(box, self, 'peak_profile', sendSelectedValue=True, items=available_models,
                      callback=self.auto_process)
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
-            cand = ListPeakCandidateMultiModel.validate(spe.result)
             self.out_spe.append(
-                spe.fit_peak_multimodel(profile=self.peak_profile, candidates=cand, no_fit=not self.should_fit,
-                                        vary_baseline=self.vary_baseline)
+                spe.fit_peaks_filter(profile=self.peak_profile, no_fit=not self.should_fit,
+                                     vary_baseline=self.vary_baseline)
             )
         self.send_outputs()
-        # TODO: fix the dataframe with peak information
-        # self.Outputs.peaks_out.send(table_from_frame(df))
+        dfs = [FitPeaksResult.loads(spe.result).to_dataframe_peaks() for spe in self.out_spe]
+        self.Outputs.peaks_out.send(table_from_frame(pd.concat(dfs)))
 
     def custom_plot(self, ax):
+        if self.plot_individual_peaks:
+            peaks_ax = ax.twinx()
+        else:
+            peaks_ax = ax
         for spe in self.out_spe:
-            ListPeakCandidateMultiModel.validate(spe.result).plot(ax)
+            FitPeaksResult.loads(spe.result).plot(peaks_ax, individual_peaks=self.plot_individual_peaks)
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/gen_spe.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/gen_spe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import CreatorWidget
+from ..processings.gen_spe import GenSpe
 
 
-class GenSpe(CreatorWidget):
+class GenSpeOW(CreatorWidget):
     name = "Gen Spectra"
     description = "gen spectra"
     icon = "icons/spectra.svg"
 
+    spe_xmin = Setting(0)
+    spe_xmax = Setting(2000)
+    spe_nbins = Setting(1500)
+    deltas_combo = Setting('PST')
+    deltas = Setting('1: 1')
+
+    n_spectra = Setting(1)
+
     def __init__(self):
         super().__init__()
-        self.n_spectra = 1
         box = gui.widgetBox(self.controlArea, self.name)
         box_params = gui.widgetBox(box, 'Spe Params')
         self.gen_spe = GenSpe(self,
                               spe_xmin=('spe_xmin', box_params),
                               spe_xmax=('spe_xmax', box_params),
                               spe_nbins=('spe_nbins', box_params),
                               deltas=('deltas', box_params),
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/hht_sharpening.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/hht_sharpening.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 
 
 class HHT_Sharpening(FilterWidget):
     name = "HHT Sharpening"
     description = "hht sharpening"
     icon = "icons/spectra.svg"
 
+    window_size = Setting(100)
+
     def __init__(self):
         super().__init__()
-        self.window_size = 100
         box = gui.widgetBox(self.controlArea, self.name)
         gui.spin(box, self, 'window_size', 0, 5000, callback=self.auto_process)
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/icons/spectra.svg` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/load_file.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from Orange.widgets import gui
 import ramanchada2 as rc2
-from ..base_widget import CreatorWidget
 from AnyQt.QtWidgets import QFileDialog
+from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
+from ..base_widget import CreatorWidget
 
 
 class LoadFile(CreatorWidget):
     name = "Load File"
     description = "Load spectrum from file"
     icon = "icons/spectra.svg"
 
+    filenames = Setting([])
+
     def __init__(self):
         super().__init__()
-        self.filenames = list()
         box = gui.widgetBox(self.controlArea, self.name)
         gui.button(box, self, "Load File", callback=self.load_file)
         self.fileformat = 'Auto'
         gui.comboBox(box, self, 'fileformat', sendSelectedValue=True,
                      items=['Auto', 'spc', 'sp', 'spa', '0', '1', '2',
                             'wdf', 'ngs', 'jdx', 'dx',
                             'txt', 'txtr', 'csv', 'prn', 'rruf'],
@@ -25,15 +28,15 @@
         filters = ['TXT (*.txt)',
                    'CSV (*.csv)',
                    'All spectra formats (*.txt *.csv)',
                    'All files (*)',
                    ]
         filenames, filt = QFileDialog.getOpenFileNames(
             caption='Open spectra',
-            directory='/data/RamanSpe/FNMT-Madrid/Horiba_785nm/PST/PST10_iR785_OP02_8000msx8_01.txt',
+            directory='',
             filter=';;'.join(filters),
             initialFilter=filters[-2],
             )
         if filenames:
             self.filenames = filenames
             self.auto_process()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/load_test_spectra.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_test_spectra.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-from Orange.widgets import gui
 import ramanchada2 as rc2
-from ..base_widget import CreatorWidget
-from ramanchada2.auxiliary.spectra import datasets2 as data
 from AnyQt.QtWidgets import QAbstractItemView
+from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+from ramanchada2.auxiliary.spectra import datasets2 as data
+
+from ..base_widget import CreatorWidget
 
 
 class TestSpectra(CreatorWidget):
     name = "Load Test Spectra"
     description = "load test spectra from ramanchada2"
     icon = "icons/spectra.svg"
 
+    filters = Setting({})
+    selected_filenames = Setting([])
+
     def __init__(self):
         super().__init__()
-        self.list_boxes = dict()
-
+        self.list_boxes = {}
         box = gui.widgetBox(self.controlArea, self.name)
         for k, v in data.get_filters().items():
-            var = k + '_select_list_box_idx'
+            var = 'listbox_' + k + '_select_idx'
             setattr(self, var, list())
             gui.label(box, self, k)
             self.list_boxes[k] = gui.listBox(
                 box, self, var, selectionMode=QAbstractItemView.MultiSelection,
                 callback=self.update_filters)
             for item in sorted(v):
                 self.list_boxes[k].addItem(item)
 
         gui.label(box, self, 'filenames')
 
-        self.filename_select_list_box_idx = list()
+        self.listbox_filename_select_idx = []
         self.list_box_filename = gui.listBox(
-            box, self, 'filename_select_list_box_idx', selectionMode=QAbstractItemView.MultiSelection,
-            callback=self.auto_process)
-        self.update_filters()
+            box, self, 'listbox_filename_select_idx', selectionMode=QAbstractItemView.MultiSelection,
+            callback=self.select_filename)
+
+        filenames = sorted(data.get_filenames(**self.filters))
+        for item in filenames:
+            self.list_box_filename.addItem(item)
+        self.auto_process()
 
     def update_filters(self):
-        filters = dict()
+        self.filters = {}
         for k, lb in self.list_boxes.items():
-            filters[k] = [item.text() for item in self.list_boxes[k].selectedItems()]
-        filenames = data.get_filenames(**filters)
+            self.filters[k] = [item.text() for item in self.list_boxes[k].selectedItems()]
+        filenames = sorted(data.get_filenames(**self.filters))
         self.list_box_filename.clear()
-        for item in sorted(filenames):
+        for item in filenames:
             self.list_box_filename.addItem(item)
 
+    def select_filename(self):
+        self.selected_filenames = [fn_item.text() for fn_item in self.list_box_filename.selectedItems()]
+        self.auto_process()
+
     def process(self):
         self.out_spe = list()
-        for fn_item in self.list_box_filename.selectedItems():
-            fn = fn_item.text()
+        for fn in self.selected_filenames:
             spe = rc2.spectrum.from_local_file(fn)
             self.out_spe.append(spe)
         self.send_outputs()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/merger.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/merger.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/moving_minimum.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/moving_minimum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 
 
 class MovingMinimum(FilterWidget):
     name = "Moving minimum"
     description = "moving minimum"
     icon = "icons/spectra.svg"
 
+    window_size = Setting(10)
+
     def __init__(self):
         # Initialize the widget
         super().__init__()
-        self.window_size = 10
         box = gui.widgetBox(self.controlArea, self.name)
         gui.spin(box, self, 'window_size', 0, 5000, callback=self.auto_process)
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/normalize.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 
 
 class Normalize(FilterWidget):
     name = "Normalize"
     description = "Normalize"
     icon = "icons/spectra.svg"
 
+    method = Setting('minmax')
+
     def __init__(self):
         super().__init__()
-        self.method = 'minmax'
         box = gui.widgetBox(self.controlArea, self.name)
         gui.comboBox(box, self, 'method', sendSelectedValue=True,
                      items=['unity', 'min_unity', 'unity_density', 'minmax'],
                      label='Normalization method', callback=self.auto_process)
 
     def process(self):
         self.out_spe = list()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/process_spectra.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/process_spectra.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 
 
-class RS2WL(FilterWidget):
-    name = "RS to WL"
-    description = "Raman shift to Wavelength"
+class WL2RS(FilterWidget):
+    name = "WL to RS"
+    description = "Wavelength to Raman shift"
     icon = "icons/spectra.svg"
 
+    laser_wl = Setting(785)
+
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
-        self.laser_wl = 785
         gui.doubleSpin(box, self, 'laser_wl', 0, 5000, decimals=5, step=1, callback=self.auto_process,
                        label='Laser Wavelength [nm]')
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
-                spe.shift_cm_1_to_abs_nm_filter(laser_wave_length_nm=self.laser_wl)
+                spe.abs_nm_to_shift_cm_1_filter(laser_wave_length_nm=self.laser_wl)
             )
         self.send_outputs()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/remove_spikes.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/remove_spikes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
 from ..base_widget import FilterWidget
 
 
 class RecoverSpikes(FilterWidget):
     name = "Recover Spikes"
     description = "Recover single-bin spikes using linear interpolation"
     icon = "icons/spectra.svg"
 
+    sigma = Setting(10)
+
     def __init__(self):
         super().__init__()
-        self.sigma = 10
         box = gui.widgetBox(self.controlArea, self.name)
         gui.spin(box, self, 'sigma', 1, 100, callback=self.auto_process)
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from Orange.widgets import gui
-from ..base_widget import FilterWidget
+from Orange.widgets.settings import Setting
 from scipy import signal
 
+from ..base_widget import FilterWidget
+
 
 class Resample_NUDFT(FilterWidget):
     name = "Resample NUDFT"
     description = "Resample Non-Uniform Discrete Fourier Transform"
     icon = "icons/spectra.svg"
 
+    xmin = Setting(0)
+    xmax = Setting(4000)
+    nbins = Setting(100)
+    window_function = Setting('blackmanharris')
+
     def __init__(self):
         super().__init__()
-        self.xmin = 0
-        self.xmax = 4000
-        self.nbins = 100
-        self.window_function = 'blackmanharris'
         box = gui.widgetBox(self.controlArea, self.name)
         gui.spin(box, self, 'xmin', -1000, 10000, callback=self.auto_process, label='x-min')
         gui.spin(box, self, 'xmax', -1000, 10000, callback=self.auto_process, label='x-max')
         gui.spin(box, self, 'nbins', 1, 10000, callback=self.auto_process, label='n-bins')
         gui.comboBox(box, self, 'window_function', label='window', sendSelectedValue=True,
                      items=['barthann',
                             'bartlett',
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/select.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/select.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from AnyQt.QtWidgets import QAbstractItemView
 from Orange.widgets import gui
-from ..base_widget import FilterWidget
+from Orange.widgets.settings import Setting
 
-from AnyQt.QtWidgets import QAbstractItemView
+from ..base_widget import FilterWidget
 
 
 class Select(FilterWidget):
     name = "Select"
     description = "select spectra"
     icon = "icons/spectra.svg"
 
+    select_inputs_idx = Setting([])
+
     def __init__(self):
         super().__init__()
-        self.select_inputs_idx = []
         box = gui.widgetBox(self.controlArea, self.name)
         self.select_box = gui.listBox(box, self, 'select_inputs_idx',
                                       selectionMode=QAbstractItemView.MultiSelection, callback=self.auto_process)
 
     def input_hook(self):
         while self.select_box.takeItem(0):
             pass
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/set_xaxis.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/set_xaxis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from Orange.widgets.widget import Input
+
 from ..base_widget import FilterWidget, RC2Spectra
 
 
 class SetXaxis(FilterWidget):
     name = "Set X-axis"
     description = "Set x-axis of the spectra equal to the calibrated spectrum"
     icon = "icons/spectra.svg"
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from Orange.widgets import gui
 from ..base_widget import FilterWidget
+from Orange.widgets.settings import Setting
 
 
-class WL2RS(FilterWidget):
-    name = "WL to RS"
-    description = "Wavelength to Raman shift"
+class RS2WL(FilterWidget):
+    name = "RS to WL"
+    description = "Raman shift to Wavelength"
     icon = "icons/spectra.svg"
 
+    laser_wl = Setting(785)
+
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
-        self.laser_wl = 785
         gui.doubleSpin(box, self, 'laser_wl', 0, 5000, decimals=5, step=1, callback=self.auto_process,
                        label='Laser Wavelength [nm]')
 
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
-                spe.abs_nm_to_shift_cm_1_filter(laser_wave_length_nm=self.laser_wl)
+                spe.shift_cm_1_to_abs_nm_filter(laser_wave_length_nm=self.laser_wl)
             )
         self.send_outputs()
```

### Comparing `oranchada-0.0.5/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py` & `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-#!/usr/bin/env python
-
-from Orange.widgets import gui
-from ..base_widget import FilterWidget
+import numpy as np
 import ramanchada2.misc.constants as rc2const
 import ramanchada2.misc.utils as rc2utils
-import numpy as np
+from Orange.widgets import gui
+from Orange.widgets.settings import Setting
+
+from ..base_widget import FilterWidget
 
 
 class XAxisFineCalibration(FilterWidget):
     name = "Xaxis fine calibration"
     description = "X-axis fine calibration"
     icon = "icons/spectra.svg"
 
+    predefined_deltas = Setting('Ne WL D3.3')
+    deltas = Setting('')
+    poly_order = Setting('poly3')
+    should_fit = Setting(False)
+    prominence = Setting(3.)
+    wlen = Setting(200)
+    should_auto_proc = Setting(False)
+    n_iters = Setting(1)
+
     def __init__(self):
         super().__init__()
-        self.should_auto_proc = False
         box = gui.widgetBox(self.controlArea, self.name)
-        self.predefined_deltas = 'Ne WL D3.3'
-        self.deltas = ''
-        self.poly_order = 'poly3'
-        self.should_fit = False
-        self.prominence = 0
-        self.wlen = 100
 
-        gui.doubleSpin(box, self, 'prominence', 0, 50000, decimals=5, step=1, callback=self.auto_process,
-                       label='Prominence')
+        gui.doubleSpin(box, self, 'prominence', 0, 50000, decimals=2, step=1, callback=self.auto_process,
+                       label='Prominence [×σ]')
         gui.spin(box, self, 'wlen', 0, 50000, step=1, callback=self.auto_process, label='wlen')
 
-        gui.checkBox(self.optionsBox, self, "should_fit", "Should fit", callback=self.auto_process)
+        gui.checkBox(box, self, "should_fit", "Should fit", callback=self.auto_process)
 
         gui.comboBox(box, self, 'poly_order', sendSelectedValue=True,
                      items=['poly0', 'poly1', 'poly2', 'poly3', 'poly4'],
                      callback=self.auto_process
                      )
 
         self.combo = gui.comboBox(box, self, 'predefined_deltas', sendSelectedValue=True,
                                   items=[
                                       'Ne RS 532nm', 'Ne RS 633nm', 'Ne RS 785nm',
                                       'Ne WL 532nm', 'Ne WL 633nm', 'Ne WL 785nm',
                                       'Ne WL D3.3', 'PST', 'User defined'], label='Deltas',
                                   callback=self.deltas_combo_callback)
         self.deltas_edit = gui.lineEdit(box, self, 'deltas', callback=self.auto_process)
 
-        self.n_iters = 1
         gui.spin(box, self, 'n_iters', 0, 20, label='N iters', callback=self.auto_process)
 
         self.deltas_combo_callback()
 
     def deltas_combo_callback(self):
         self.deltas_edit.setReadOnly(True)
         if self.predefined_deltas == 'Ne RS 532nm':
@@ -84,15 +85,15 @@
 
         self.out_spe = list()
         if len(self.in_spe) > 1:
             raise ValueError(f'Expects a single spectrum input. {len(self.in_spe)} found')
         for spe in self.in_spe:
             for iter in range(self.n_iters):
                 spe = spe.xcal_fine(ref=self.deltas_dict, poly_order=poly_order_num, should_fit=self.should_fit,
-                                    find_peaks_kw=dict(prominence=self.prominence, wlen=self.wlen))
+                                    find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen))
             self.out_spe.append(spe)
         self.send_outputs()
 
     def custom_plot(self, ax):
         if not self.in_spe:
             return
         self.in_spe[0].plot(ax=self.axes[0])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.5/setup.py` & `oranchada-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 
 from os import path, walk
+
 from setuptools import find_packages, setup
 
 NAME = 'oranchada'
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 DESCRIPTION = 'Orange add-on for Raman spectroscopy'
 README_FILE = path.join(path.dirname(__file__), 'README.pypi')
 LONG_DESCRIPTION = open(README_FILE, 'r', encoding='utf-8').read()
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 URL = 'https://github.com/h2020charisma/oranchada'
 AUTHOR = 'IDEAconsult Ltd.'
@@ -37,15 +38,15 @@
 
 INSTALL_REQUIRES = [
     'Orange3>=3.31.0',
     'numpy>=1.18.0',
     'orange-canvas-core>=0.1.24',
     'orange-widget-base>=4.16.1',
     'pip>=9.0',  # same as for Orange 3.28
-    'ramanchada2~=0.0.3',
+    'ramanchada2~=0.0.4',
     'setuptools>=36.3',  # same as for Orange 3.28
     # 'AnyQt>=0.0.6',
     # 'bottleneck',
     # 'colorcet',
     # 'extranormal3 >=0.0.3',
     # 'h5py',
     # 'lmfit>=1.0.2',
```

