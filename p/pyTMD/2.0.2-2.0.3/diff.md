# Comparing `tmp/pyTMD-2.0.2.tar.gz` & `tmp/pyTMD-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTMD-2.0.2.tar", last modified: Thu Mar  9 22:34:11 2023, max compression
+gzip compressed data, was "pyTMD-2.0.3.tar", last modified: Sat Apr  8 20:10:31 2023, max compression
```

## Comparing `pyTMD-2.0.2.tar` & `pyTMD-2.0.3.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.392745 pyTMD-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-03-09 22:34:00.000000 pyTMD-2.0.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-03-09 22:34:00.000000 pyTMD-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-03-09 22:34:00.000000 pyTMD-2.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-03-09 22:34:00.000000 pyTMD-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-09 22:34:00.000000 pyTMD-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-03-09 22:34:11.392745 pyTMD-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6884 2023-03-09 22:34:00.000000 pyTMD-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-09 22:34:00.000000 pyTMD-2.0.2/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.380745 pyTMD-2.0.2/pyTMD/
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/calc_astrol_longitudes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8347 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/check_tide_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/compute_tide_corrections.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12474 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10081 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/convert_ll_xy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.392745 pyTMD-2.0.2/pyTMD/data/
--rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  3522744 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/finals.all
--rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)    10661 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (122)    78848 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/mean-pole.tab
--rwxr-xr-x   0 runner    (1001) docker     (122)   153000 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/opoleloadcoefcmcor.txt.gz
--rwxr-xr-x   0 runner    (1001) docker     (122)    34592 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (122)    14076 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/eop.py
--rw-r--r--   0 runner    (1001) docker     (122)    14536 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.392745 pyTMD-2.0.2/pyTMD/io/
--rw-r--r--   0 runner    (1001) docker     (122)    41905 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/ATLAS.py
--rw-r--r--   0 runner    (1001) docker     (122)    30319 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/FES.py
--rw-r--r--   0 runner    (1001) docker     (122)    28128 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/GOT.py
--rw-r--r--   0 runner    (1001) docker     (122)    68589 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/OTIS.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4278 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/constituents.py
--rw-r--r--   0 runner    (1001) docker     (122)    68702 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/io/ocean_pole_tide.py
--rw-r--r--   0 runner    (1001) docker     (122)     4727 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/load_constituent.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    20799 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/load_nodal_corrections.py
--rw-r--r--   0 runner    (1001) docker     (122)    20420 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)    52268 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/spatial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/tidal_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (122)    45305 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/time.py
--rw-r--r--   0 runner    (1001) docker     (122)    11766 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    36164 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-03-09 22:34:00.000000 pyTMD-2.0.2/pyTMD/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.380745 pyTMD-2.0.2/pyTMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-03-09 22:34:11.000000 pyTMD-2.0.2/pyTMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-03-09 22:34:11.000000 pyTMD-2.0.2/pyTMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 22:34:11.000000 pyTMD-2.0.2/pyTMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-03-09 22:34:11.000000 pyTMD-2.0.2/pyTMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-09 22:34:11.000000 pyTMD-2.0.2/pyTMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-03-09 22:34:00.000000 pyTMD-2.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-09 22:34:00.000000 pyTMD-2.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 22:34:11.392745 pyTMD-2.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/arcticdata_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13042 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/aviso_fes_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    16662 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/compute_LPET_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    20240 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/compute_LPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    22774 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/compute_OPT_displacements.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    25506 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/compute_tidal_currents.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    25560 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/compute_tidal_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11605 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/reduce_OTIS_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     5128 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/usap_cats_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-03-09 22:34:00.000000 pyTMD-2.0.2/scripts/verify_box_tpxo.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-09 22:34:11.392745 pyTMD-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-03-09 22:34:00.000000 pyTMD-2.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-09 22:34:00.000000 pyTMD-2.0.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.279295 pyTMD-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-08 20:10:16.000000 pyTMD-2.0.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-08 20:10:16.000000 pyTMD-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-08 20:10:16.000000 pyTMD-2.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-08 20:10:16.000000 pyTMD-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-08 20:10:16.000000 pyTMD-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7831 2023-04-08 20:10:31.279295 pyTMD-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6929 2023-04-08 20:10:16.000000 pyTMD-2.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-08 20:10:16.000000 pyTMD-2.0.3/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.263295 pyTMD-2.0.3/pyTMD/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14671 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/astro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/calc_astrol_longitudes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/check_tide_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53397 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/compute_tide_corrections.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16115 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/convert_crs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/convert_ll_xy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.275295 pyTMD-2.0.3/pyTMD/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3529324 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (122)    78848 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (122)   153560 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/opoleloadcoefcmcor.txt.gz
+-rwxr-xr-x   0 runner    (1001) docker     (122)    40928 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (122)    15314 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/eop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.275295 pyTMD-2.0.3/pyTMD/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    42922 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/ATLAS.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31482 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/FES.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28297 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/GOT.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70382 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/OTIS.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/constituents.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71442 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/io/ocean_pole_tide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/load_constituent.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21033 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/load_nodal_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53934 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/tidal_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47262 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11766 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37472 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-04-08 20:10:16.000000 pyTMD-2.0.3/pyTMD/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.263295 pyTMD-2.0.3/pyTMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7831 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-08 20:10:31.000000 pyTMD-2.0.3/pyTMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-08 20:10:16.000000 pyTMD-2.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-08 20:10:16.000000 pyTMD-2.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 20:10:31.279295 pyTMD-2.0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/arcticdata_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13042 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/aviso_fes_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16845 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_LPET_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_LPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23346 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_OPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20421 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_SET_displacements.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    25487 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_tidal_currents.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    25673 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/compute_tidal_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/reduce_OTIS_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5128 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/usap_cats_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-04-08 20:10:16.000000 pyTMD-2.0.3/scripts/verify_box_tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-08 20:10:31.279295 pyTMD-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-04-08 20:10:16.000000 pyTMD-2.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-08 20:10:16.000000 pyTMD-2.0.3/version.txt
```

### Comparing `pyTMD-2.0.2/.gitignore` & `pyTMD-2.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 *.gmtcommands4
 *.gmtdefaults4
 .RData
 .Rhistory
 octave-workspace
 __pycache__
 build/
+_build/
 dist/
 develop-eggs/
 run/
 wheels/
 .eggs/
 *.egg-info/
 .installed.cfg
```

### Comparing `pyTMD-2.0.2/CONTRIBUTORS.rst` & `pyTMD-2.0.3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/LICENSE` & `pyTMD-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/PKG-INFO` & `pyTMD-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.2
+Version: 2.0.3
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -57,26 +57,29 @@
 
 .. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
    :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
 
 .. |zenodo| image:: https://zenodo.org/badge/107997403.svg
    :target: https://zenodo.org/badge/latestdoi/107997403
 
-Python-based tidal prediction software that reads OTIS, GOT and FES formatted tidal solutions for calculating ocean and load tides
+
+Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
+
+Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
 - `OSU Global and Regional Tide Models <https://www.tpxo.net>`_
 - `ESR Polar Tide Models <https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/>`_
 - `A Global Ocean Tide Model From TOPEX/POSEIDON Altimetry: GOT99.2 <https://ntrs.nasa.gov/citations/19990089548>`_
 - `Finite Element Solution (FES) tide models <https://www.aviso.altimetry.fr/en/data/products/auxiliary-products/global-tide-fes.html>`_
 - `Delta times from US Naval Observatory (USNO) Earth Orientation Products <http://maia.usno.navy.mil/ser7/deltat.data>`_
 - `Delta times from NASA Crustal Dynamics Data Information System (CDDIS) <ftp://cddis.nasa.gov/products/iers/deltat.data>`_
 
-Pole tide prediction software for calculating radial pole tide displacements
+Radial solid Earth and pole tide displacements following IERS conventions
 
 - `IERS Conventions (2010) <http://iers-conventions.obspm.fr/>`_
 - `IERS Mean Pole Location <https://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.tab>`_
 - `IERS Pole Coordinates to Calculate Mean Pole <https://hpiers.obspm.fr/iers/eop/eopc01/eopc01.1900-now.dat>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
```

### Comparing `pyTMD-2.0.2/README.rst` & `pyTMD-2.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,29 @@
 
 .. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
    :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
 
 .. |zenodo| image:: https://zenodo.org/badge/107997403.svg
    :target: https://zenodo.org/badge/latestdoi/107997403
 
-Python-based tidal prediction software that reads OTIS, GOT and FES formatted tidal solutions for calculating ocean and load tides
+
+Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
+
+Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
 - `OSU Global and Regional Tide Models <https://www.tpxo.net>`_
 - `ESR Polar Tide Models <https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/>`_
 - `A Global Ocean Tide Model From TOPEX/POSEIDON Altimetry: GOT99.2 <https://ntrs.nasa.gov/citations/19990089548>`_
 - `Finite Element Solution (FES) tide models <https://www.aviso.altimetry.fr/en/data/products/auxiliary-products/global-tide-fes.html>`_
 - `Delta times from US Naval Observatory (USNO) Earth Orientation Products <http://maia.usno.navy.mil/ser7/deltat.data>`_
 - `Delta times from NASA Crustal Dynamics Data Information System (CDDIS) <ftp://cddis.nasa.gov/products/iers/deltat.data>`_
 
-Pole tide prediction software for calculating radial pole tide displacements
+Radial solid Earth and pole tide displacements following IERS conventions
 
 - `IERS Conventions (2010) <http://iers-conventions.obspm.fr/>`_
 - `IERS Mean Pole Location <https://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.tab>`_
 - `IERS Pole Coordinates to Calculate Mean Pole <https://hpiers.obspm.fr/iers/eop/eopc01/eopc01.1900-now.dat>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
```

### Comparing `pyTMD-2.0.2/pyTMD/__init__.py` & `pyTMD-2.0.3/pyTMD/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,27 +7,40 @@
 
 The package works using scientific Python packages (numpy, scipy and pyproj)
 combined with data storage in netCDF4 and HDF5 and mapping using
 matplotlib and cartopy
 
 Documentation is available at https://pytmd.readthedocs.io
 """
+import pyTMD.astro
 import pyTMD.eop
 import pyTMD.interpolate
 import pyTMD.predict
 import pyTMD.spatial
 import pyTMD.time
 import pyTMD.tools
 import pyTMD.utilities
 import pyTMD.version
 from pyTMD import io
-from pyTMD.calc_astrol_longitudes import calc_astrol_longitudes
 from pyTMD.check_tide_points import check_tide_points
-from pyTMD.compute_tide_corrections import compute_tide_corrections
-from pyTMD.constants import constants, _ellipsoids
-from pyTMD.convert_ll_xy import convert_ll_xy
+from pyTMD.compute_tide_corrections import (
+    compute_corrections,
+    compute_tide_corrections,
+    compute_LPET_corrections,
+    compute_LPT_corrections,
+    compute_OPT_corrections,
+    compute_SET_corrections,
+)
+from pyTMD.constants import (
+    constants,
+    _ellipsoids
+)
+from pyTMD.convert_crs import convert_crs
 from pyTMD.load_constituent import load_constituent
 from pyTMD.load_nodal_corrections import load_nodal_corrections
 from pyTMD.tidal_ellipse import tidal_ellipse
 
+# Deprecated functions
+from pyTMD.convert_ll_xy import convert_ll_xy
+
 # get semantic version from setuptools-scm
 __version__ = pyTMD.version.version
```

### Comparing `pyTMD-2.0.2/pyTMD/check_tide_points.py` & `pyTMD-2.0.3/pyTMD/check_tide_points.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 check_tide_points.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 Check if points are within a tide model domain
 
 OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -39,85 +39,92 @@
         https://docs.scipy.org/doc/
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
-    convert_ll_xy.py: convert lat/lon points to and from projected coordinates
+    convert_crs.py: convert points to and from Coordinates Reference Systems
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from ATLAS netcdf models
     io/GOT.py: extract tidal harmonic constants from GSFC GOT models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactored tide read programs under io
         refactored bilinear interpolation routine
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 05/2022: added ESR netCDF4 formats to list of model types
         updated keyword arguments to read tide model programs
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 09/2021: refactor to use model class for files and attributes
     Updated 07/2021: added check that tide model directory is accessible
     Updated 06/2021: add try/except for input projection strings
     Written 05/2021
 """
-from __future__ import print_function
+from __future__ import print_function, annotations
 
 import os
 import warnings
 import numpy as np
 import scipy.interpolate
 
 import pyTMD.io
 import pyTMD.io.model
-import pyTMD.convert_ll_xy
+import pyTMD.convert_crs
 import pyTMD.interpolate
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("pyproj not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: compute tides at points and times using tide model algorithms
-def check_tide_points(x, y, DIRECTORY=None, MODEL=None,
-    ATLAS_FORMAT='netcdf', GZIP=False, DEFINITION_FILE=None,
-    EPSG=3031, METHOD='spline'):
+def check_tide_points(x: np.ndarray, y: np.ndarray,
+        DIRECTORY: str | None = None,
+        MODEL: str | None = None,
+        ATLAS_FORMAT: str = 'netcdf',
+        GZIP: bool = False,
+        DEFINITION_FILE: str | None = None,
+        EPSG: str | int = 3031,
+        METHOD: str = 'spline'
+    ):
     """
     Check if points are within a tide model domain
 
     Parameters
     ----------
-    x: float
+    x: np.ndarray
         x-coordinates in projection EPSG
-    y: float
+    y: np.ndarray
         y-coordinates in projection EPSG
     DIRECTORY: str or NoneType, default None
         working data directory for tide models
-    MODEL:  str or NoneType, default None
+    MODEL: str or NoneType, default None
         Tide model to use
     ATLAS_FORMAT: str, default 'netcdf'
         ATLAS tide model format
 
             - ``'OTIS'``
             - ``'netcdf'``
     GZIP: bool, default False
         Tide model files are gzip compressed
     DEFINITION_FILE: str or NoneType, default None
         Tide model definition file for use
-    EPSG: int, default: 3031 (Polar Stereographic South, WGS84)
+    EPSG: str or int, default: 3031 (Polar Stereographic South, WGS84)
         Input coordinate system
-    METHOD: str
+    METHOD: str, default 'spline'
         interpolation method
 
             - ```bilinear```: quick bilinear interpolation
             - ```spline```: scipy bivariate spline interpolation
             - ```linear```, ```nearest```: scipy regular grid interpolations
 
     Returns
@@ -137,80 +144,84 @@
         model = pyTMD.io.model(DIRECTORY).from_file(DEFINITION_FILE)
     else:
         model = pyTMD.io.model(DIRECTORY, format=ATLAS_FORMAT,
             compressed=GZIP).elevation(MODEL)
 
     # input shape of data
     idim = np.shape(x)
-    # converting x,y from EPSG to latitude/longitude
+    # converting x,y from input coordinate reference system
     try:
         # EPSG projection code string or int
         crs1 = pyproj.CRS.from_epsg(int(EPSG))
     except (ValueError,pyproj.exceptions.CRSError):
         # Projection SRS string
         crs1 = pyproj.CRS.from_string(EPSG)
+    # convert to latitude and longitude
     crs2 = pyproj.CRS.from_epsg(4326)
     transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
-    lon,lat = transformer.transform(np.atleast_1d(x).flatten(),
-        np.atleast_1d(y).flatten())
+    lon, lat = transformer.transform(
+        np.atleast_1d(x).flatten(), np.atleast_1d(y).flatten()
+    )
 
     # read tidal constants and interpolate to grid points
     if model.format in ('OTIS','ATLAS','ESR'):
         # if reading a single OTIS solution
-        xi,yi,hz,mz,iob,dt = pyTMD.io.OTIS.read_otis_grid(model.grid_file)
+        xi, yi, hz, mz, iob, dt = pyTMD.io.OTIS.read_otis_grid(
+            model.grid_file)
         # invert model mask
         mz = np.logical_not(mz)
         # adjust dimensions of input coordinates to be iterable
         # run wrapper function to convert coordinate systems of input lat/lon
-        X,Y = pyTMD.convert_ll_xy(lon,lat,model.projection,'F')
+        X, Y = pyTMD.convert_crs(lon, lat, model.projection, 'F')
     elif (model.format == 'netcdf'):
         # if reading a netCDF OTIS atlas solution
-        xi,yi,hz = pyTMD.io.ATLAS.read_netcdf_grid(model.grid_file,
+        xi, yi, hz = pyTMD.io.ATLAS.read_netcdf_grid(model.grid_file,
             compressed=model.compressed, type=model.type)
         # copy bathymetry mask
         mz = np.copy(hz.mask)
         # copy latitude and longitude and adjust longitudes
         X,Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
     elif (model.format == 'GOT'):
         # if reading a NASA GOT solution
-        hc,xi,yi,c = pyTMD.io.GOT.read_ascii_file(model.model_file[0],
-            compressed=model.compressed)
+        hc, xi, yi, c = pyTMD.io.GOT.read_ascii_file(
+            model.model_file[0], compressed=model.compressed)
         # copy tidal constituent mask
         mz = np.copy(hc.mask)
         # copy latitude and longitude and adjust longitudes
-        X,Y = np.copy([lon,lat]).astype(np.float64)
+        X, Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
     elif (model.format == 'FES'):
         # if reading a FES netCDF solution
-        hc,xi,yi = pyTMD.io.FES.read_netcdf_file(model.model_file[0],
-            compressed=model.compressed, type=model.type,
-            version=model.version)
+        hc, xi, yi = pyTMD.io.FES.read_netcdf_file(
+            model.model_file[0], compressed=model.compressed,
+            type=model.type, version=model.version)
         # copy tidal constituent mask
         mz = np.copy(hc.mask)
         # copy latitude and longitude and adjust longitudes
-        X,Y = np.copy([lon,lat]).astype(np.float64)
+        X, Y = np.copy([lon,lat]).astype(np.float64)
         lt0, = np.nonzero(X < 0)
         X[lt0] += 360.0
 
     # interpolate masks
     if (METHOD == 'bilinear'):
         # replace invalid values with nan
-        mz1 = pyTMD.interpolate.bilinear(xi,yi,mz,X,Y)
+        mz1 = pyTMD.interpolate.bilinear(xi, yi, mz, X, Y)
         mask = np.floor(mz1).astype(mz.dtype)
     elif (METHOD == 'spline'):
-        f1=scipy.interpolate.RectBivariateSpline(xi,yi,mz.T,kx=1,ky=1)
-        mask = np.floor(f1.ev(X,Y)).astype(mz.dtype)
+        f1 = scipy.interpolate.RectBivariateSpline(xi, yi, mz.T,
+            kx=1, ky=1)
+        mask = np.floor(f1.ev(X, Y)).astype(mz.dtype)
     else:
         # use scipy regular grid to interpolate values
-        r1 = scipy.interpolate.RegularGridInterpolator((yi,xi),mz,
-            method=METHOD,bounds_error=False,fill_value=1)
-        mask = np.floor(r1.__call__(np.c_[y,x])).astype(mz.dtype)
+        r1 = scipy.interpolate.RegularGridInterpolator((yi, xi), mz,
+            method=METHOD, bounds_error=False, fill_value=1)
+        mask = np.floor(r1.__call__(np.c_[y, x])).astype(mz.dtype)
 
     # reshape to original dimensions
     valid = np.logical_not(mask).reshape(idim).astype(mz.dtype)
     # replace points outside model domain with invalid
     valid &= (X >= xi.min()) & (X <= xi.max())
     valid &= (Y >= yi.min()) & (Y <= yi.max())
     # return the valid mask
```

### Comparing `pyTMD-2.0.2/pyTMD/constants.py` & `pyTMD-2.0.3/pyTMD/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 constants.py
-Written by Tyler Sutterley (01/2023)
+Written by Tyler Sutterley (03/2023)
 
 Gravitational and ellipsoidal parameters
 
 CALLING SEQUENCE
     wgs84 = constants('WGS84', units='MKS')
 
 INPUT:
@@ -33,14 +33,16 @@
 
 REFERENCE:
     Hofmann-Wellenhof and Moritz, "Physical Geodesy" (2006)
     IERS Numerical Standards
         https://iers-conventions.obspm.fr/content/tn36.pdf
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing
+        set ellipsoid name and output units as constants attributes
     Updated 01/2023: include main ellipsoid attributes in docstring
     Written 12/2022
 """
 import numpy as np
 
 _ellipsoids = ['CLK66', 'GRS67', 'GRS80', 'WGS72', 'WGS84', 'ATS77',
     'NAD27', 'NAD83', 'INTER', 'KRASS', 'MAIRY', 'HGH80', 'TOPEX',
@@ -85,248 +87,253 @@
         Flattening of the ellipsoid
     omega: float
         Angular velocity of the Earth
     GM: float
         Geocentric gravitational constant
     """
     np.seterr(invalid='ignore')
-    def __init__(self, ellipsoid='WGS84', units='MKS'):
+    def __init__(self, ellipsoid: str = 'WGS84', units: str = 'MKS'):
+        # set ellipsoid name and units
+        self.name = ellipsoid.upper()
+        self.units = units.upper()
         # validate ellipsoid and units
-        assert ellipsoid in _ellipsoids
-        assert units in _units
+        assert self.name in _ellipsoids
+        assert self.units in _units
 
         # set parameters for ellipsoid
-        if ellipsoid.upper() in ('CLK66','NAD27'):
+        if self.name in ('CLK66','NAD27'):
             # Clarke 1866
             self.a_axis = 6378206.4# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/294.9786982# flattening of the ellipsoid
 
-        elif ellipsoid.upper() in ('GRS80','NAD83'):
+        elif self.name in ('GRS80','NAD83'):
             # Geodetic Reference System 1980
             # North American Datum 1983
             self.a_axis = 6378135.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.26# flattening of the ellipsoid
             self.GM = 3.986005e14# [m^3/s^2] Geocentric Gravitational Constant
 
-        elif (ellipsoid.upper() == 'GRS67'):
+        elif (self.name == 'GRS67'):
             # Geodetic Reference System 1967
             # International Astronomical Union (IAU ellipsoid)
             self.a_axis = 6378160.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.247167427# flattening of the ellipsoid
             self.GM = 3.98603e14# [m^3/s^2] Geocentric Gravitational Constant
             self.omega = 7292115.1467e-11# angular velocity of the Earth [rad/s]
 
-        elif (ellipsoid.upper() == 'WGS72'):
+        elif (self.name == 'WGS72'):
             # World Geodetic System 1972
             self.a_axis = 6378135.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.26# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'WGS84'):
+        elif (self.name == 'WGS84'):
             # World Geodetic System 1984
             self.a_axis = 6378137.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.257223563# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'ATS77'):
+        elif (self.name == 'ATS77'):
             # Quasi-earth centred ellipsoid for ATS77
             self.a_axis = 6378135.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.257# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'KRASS'):
+        elif (self.name == 'KRASS'):
             # Krassovsky (USSR)
             self.a_axis = 6378245.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.3# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'INTER'):
+        elif (self.name == 'INTER'):
             # International
             self.a_axis = 6378388.0# [m] semimajor axis of the ellipsoid
             self.flat = 1/297.0# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'MAIRY'):
+        elif (self.name == 'MAIRY'):
             # Modified Airy (Ireland 1965/1975)
             self.a_axis = 6377340.189# [m] semimajor axis of the ellipsoid
             self.flat = 1/299.3249646# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'HGH80'):
+        elif (self.name == 'HGH80'):
             # Hughes 1980 Ellipsoid used in some NSIDC data
             self.a_axis = 6378273.0# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.279411123064# flattening of the ellipsoid
 
-        elif (ellipsoid.upper() == 'TOPEX'):
+        elif (self.name == 'TOPEX'):
             # TOPEX/POSEIDON ellipsoid
             self.a_axis = 6378136.3# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.257# flattening of the ellipsoid
             self.GM = 3.986004415e14# [m^3/s^2]
 
-        elif (ellipsoid.upper() == 'EGM96'):
+        elif (self.name == 'EGM96'):
             # EGM 1996 gravity model
             self.a_axis = 6378136.3# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.256415099# flattening of the ellipsoid
             self.GM = 3.986004415e14# [m^3/s^2]
 
-        elif (ellipsoid.upper() == 'IERS'):
+        elif (self.name == 'IERS'):
             # IERS Numerical Standards
             self.a_axis = 6378136.6# [m] semimajor axis of the ellipsoid
             self.flat = 1.0/298.25642# flattening of the ellipsoid
 
         # set default parameters if not listed as part of ellipsoid
-        if ellipsoid.upper() not in ('GRS80','GRS67','NAD83','TOPEX','EGM96'):
+        if self.name not in ('GRS80','GRS67','NAD83','TOPEX','EGM96'):
             # for ellipsoids not listing the Geocentric Gravitational Constant
             self.GM = 3.986004418e14# [m^3/s^2]
 
-        if ellipsoid.upper() not in ('GRS67'):
+        if self.name not in ('GRS67'):
             # for ellipsoids not listing the angular velocity of the Earth
             self.omega = 7292115e-11# [rad/s]
 
         # universal gravitational constant [N*m^2/kg^2]
         self.G = 6.67430e-11
 
         # convert units to CGS
-        if (units == 'CGS'):
+        if (self.units == 'CGS'):
             self.a_axis *= 100.0
             self.GM *= 1e6
             self.G *= 1000.0 # [dyn*cm^2/g^2]
 
     # mean radius of the Earth having the same volume
     # (4pi/3)R^3 = (4pi/3)(a^2)b = (4pi/3)(a^3)(1 - f)
     @property
-    def rad_e(self):
+    def rad_e(self) -> float:
         """Average radius of the Earth with same volume as ellipsoid
         """
         return self.a_axis*(1.0 - self.flat)**(1.0/3.0)
 
     # semiminor axis of the ellipsoid
     @property
-    def b_axis(self):
+    def b_axis(self) -> float:
         """Semi-minor axis of the ellipsoid
         """
         return (1.0 - self.flat)*self.a_axis
 
     # Ratio between ellipsoidal axes
     @property
-    def ratio(self):
+    def ratio(self) -> float:
         """Ratio between ellipsoidal axes
         """
         return (1.0 - self.flat)
 
     # Polar radius of curvature
     @property
-    def rad_p(self):
+    def rad_p(self) -> float:
+        """Polar radius of curvature
+        """
         return self.a_axis/(1.0 - self.flat)
 
     # Linear eccentricity
     @property
-    def ecc(self):
+    def ecc(self) -> float:
         """Linear eccentricity
         """
         return np.sqrt((2.0*self.flat - self.flat**2)*self.a_axis**2)
 
     # first numerical eccentricity
     @property
-    def ecc1(self):
+    def ecc1(self) -> float:
         """First numerical eccentricity
         """
         return self.ecc/self.a_axis
 
     # second numerical eccentricity
     @property
-    def ecc2(self):
+    def ecc2(self) -> float:
         """Second numerical eccentricity
         """
         return self.ecc/self.b_axis
 
     # m parameter [omega^2*a^2*b/(GM)]
     # p. 70, Eqn.(2-137)
     @property
-    def m(self):
+    def m(self) -> float:
         """m Parameter
         """
         return self.omega**2*((1 - self.flat)*self.a_axis**3)/self.GM
 
     # flattening f2 component
     # p. 80, Eqn.(2-200)
     @property
-    def f2(self):
+    def f2(self) -> float:
         """f2 component
         """
         return -self.flat + (5.0/2.0)*self.m + (1.0/2.0)*self.flat**2.0 - \
             (26.0/7.0)*self.flat*self.m + (15.0/4.0)*self.m**2.0
 
     # flattening f4 component
     # p. 80, Eqn.(2-200)
     @property
-    def f4(self):
+    def f4(self) -> float:
         """f4 component
         """
         return -(1.0/2.0)*self.flat**2.0 + (5.0/2.0)*self.flat*self.m
 
     # q
     # p. 67, Eqn.(2-113)
     @property
-    def q(self):
+    def q(self) -> float:
         """q Parameter
         """
         return 0.5*((1.0 + 3.0/(self.ecc2**2))*np.arctan(self.ecc2)-3.0/self.ecc2)
 
     # q_0
     # p. 67, Eqn.(2-113)
     @property
-    def q0(self):
+    def q0(self) -> float:
         """q\ :sub:`0` Parameter
         """
         return 3*(1.0 + 1.0/(self.ecc2**2)) * \
             (1.0 -1.0/self.ecc2*np.arctan(self.ecc2)) - 1.0
 
     # J_2 p. 75 Eqn.(2-167), p. 76 Eqn.(2-172)
     @property
-    def J2(self):
+    def J2(self) -> float:
         """Oblateness coefficient
         """
         return (self.ecc1**2)*(1.0 - 2.0*self.m*self.ecc2/(15.0*self.q))/3.0
 
     # Normalized C20 harmonic
     # p. 60, Eqn.(2-80)
     @property
-    def C20(self):
+    def C20(self) -> float:
         """Normalized C\ :sub:`20` harmonic
         """
         return -self.J2/np.sqrt(5.0)
 
     # Normal gravity at the equator
     # p. 79, Eqn.(2-286)
     @property
-    def gamma_a(self):
+    def gamma_a(self) -> float:
         """Normal gravity at the equator
         """
         return (self.GM/(self.a_axis*self.b_axis)) * \
             (1.0 - (3.0/2.0)*self.m - (3.0/14.0)*self.ecc2**2.0*self.m)
 
     # Normal gravity at the pole
     # p. 79, Eqn.(2-286)
     @property
-    def gamma_b(self):
+    def gamma_b(self) -> float:
         """Normal gravity at the pole
         """
         return (self.GM/(self.a_axis**2)) * \
             (1.0 + self.m + (3.0/7.0)*self.ecc2**2.0*self.m)
 
     # Normal gravity at location
     # p. 80, Eqn.(2-199)
-    def gamma_0(self, theta):
+    def gamma_0(self, theta) -> float:
         """Normal gravity at colatitudes
 
         Parameters
         ----------
         theta: float
             Colatitudes in radians
         """
         return self.gamma_a*(1.0 + self.f2*np.cos(theta)**2.0 + self.f4*np.cos(theta)**4.0)
 
     # Normal gravity at location
     # p. 82, Eqn.(2-215)
-    def gamma_h(self, theta, height):
+    def gamma_h(self, theta, height) -> float:
         """Normal gravity at colatitudes and heights
 
         Parameters
         ----------
         theta: float
             Colatitudes in radians
         height: float
@@ -335,43 +342,43 @@
         return self.gamma_0(theta) * \
             (1.0 - (2.0/self.a_axis) * \
             (1.0 + self.flat + self.m - 2.0*self.flat*np.cos(theta)**2.0)*height +
             (3.0/self.a_axis**2.0)*height**2.0)
 
     # ratio between gravity at pole versus gravity at equator
     @property
-    def dk(self):
+    def dk(self) -> float:
         """Ratio between gravity at pole versus gravity at equator
         """
         return self.b_axis*self.gamma_b/(self.a_axis*self.gamma_b) - 1.0
 
     # Normal potential at the ellipsoid
     # p. 68, Eqn.(2-123)
     @property
-    def U0(self):
+    def U0(self) -> float:
         """Normal potential at the ellipsoid
         """
         return self.GM/self.ecc*np.arctan(self.ecc2) + \
             (1.0/3.0)*self.omega**2*self.a_axis**2
 
     # Surface area of the reference ellipsoid
     @property
-    def area(self):
+    def area(self) -> float:
         """Surface area of the ellipsoid
         """
         return np.pi*self.a_axis**2.0 * \
             (2.0 + ((1.0 - self.ecc1**2)/self.ecc1) *
                 np.log((1.0 + self.ecc1)/(1.0 - self.ecc1)))
 
     # Volume of the reference ellipsoid
     @property
-    def volume(self):
+    def volume(self) -> float:
         """Volume of the ellipsoid
         """
         return (4.0*np.pi/3.0)*(self.a_axis**3.0)*(1.0 - self.ecc1**2.0)**0.5
 
     # Average density
     @property
-    def rho_e(self):
+    def rho_e(self) -> float:
         """Average density
         """
         return self.GM/(self.G*self.volume)
```

### Comparing `pyTMD-2.0.2/pyTMD/data/deltat.data` & `pyTMD-2.0.3/pyTMD/data/deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/data/finals.all` & `pyTMD-2.0.3/pyTMD/data/finals.all`

 * *Files 0% similar despite different names*

```diff
@@ -17928,803 +17928,803 @@
 22 2 1 59611.00 I  0.026120 0.000021  0.323090 0.000015  I-0.1073939 0.0000037 -0.3676 0.0024  I  -110.025    0.395    -6.224    0.209  0.026102  0.323015 -0.1073994  -110.029    -6.256  
 22 2 2 59612.00 I  0.025848 0.000020  0.325440 0.000015  I-0.1071280 0.0000034 -0.1551 0.0026  I  -109.557    0.397    -6.236    0.225  0.025834  0.325489 -0.1071431  -109.538    -6.310  
 22 2 3 59613.00 I  0.025709 0.000021  0.327756 0.000014  I-0.1070840 0.0000037  0.0583 0.0026  I  -109.168    0.397    -6.270    0.225  0.025683  0.327751 -0.1070987  -109.116    -6.393  
 22 2 4 59614.00 I  0.025775 0.000020  0.329989 0.000014  I-0.1072185 0.0000040  0.1935 0.0037  I  -109.000    0.397    -6.201    0.225  0.025779  0.330022 -0.1072225  -108.919    -6.381  
 22 2 5 59615.00 I  0.025749 0.000015  0.332150 0.000008  I-0.1074256 0.0000065  0.1924 0.0030  I  -109.148    0.439    -5.977    0.284  0.025738  0.332211 -0.1074267  -109.063    -6.141  
 22 2 6 59616.00 I  0.025719 0.000021  0.333907 0.000008  I-0.1075777 0.0000046  0.1143 0.0040  I  -109.520    0.477    -5.750    0.130  0.025676  0.333942 -0.1076113  -109.447    -5.873  
 22 2 7 59617.00 I  0.025702 0.000021  0.335607 0.000008  I-0.1076483 0.0000047  0.0184 0.0036  I  -109.902    0.477    -5.709    0.130  0.025772  0.335603 -0.1076870  -109.853    -5.790  
-22 2 8 59618.00 I  0.025134 0.000020  0.337306 0.000007  I-0.1075833 0.0000055 -0.1713 0.0031  I  -110.137    0.481    -5.857    0.008  0.025193  0.337374 -0.1075919  -110.126    -5.888  
-22 2 9 59619.00 I  0.024112 0.000020  0.338499 0.000007  I-0.1072954 0.0000039 -0.3920 0.0033  I  -110.178    0.506    -6.027    0.019  0.024114  0.338478 -0.1072977  -110.203    -6.067  
-22 210 59620.00 I  0.022891 0.000019  0.339529 0.000007  I-0.1068102 0.0000037 -0.5800 0.0027  I  -110.000    0.506    -6.102    0.019  0.022952  0.339544 -0.1067962  -110.062    -6.157  
-22 211 59621.00 I  0.021292 0.000019  0.340652 0.000007  I-0.1061227 0.0000036 -0.8061 0.0025  I  -109.613    0.506    -6.138    0.019  0.021317  0.340636 -0.1061126  -109.706    -6.193  
-22 212 59622.00 I  0.019528 0.000014  0.341941 0.000008  I-0.1052490 0.0000035 -0.8793 0.0025  I  -109.149    0.564    -6.265    0.027  0.019510  0.341957 -0.1052912  -109.259    -6.321  
-22 213 59623.00 I  0.018053 0.000016  0.343130 0.000010  I-0.1044122 0.0000035 -0.8084 0.0024  I  -108.809    0.589    -6.506    0.098  0.017952  0.343165 -0.1044265  -108.917    -6.560  
-22 214 59624.00 I  0.017241 0.000016  0.344307 0.000010  I-0.1036357 0.0000034 -0.7272 0.0028  I  -108.674    0.589    -6.740    0.098  0.017178  0.344276 -0.1036375  -108.763    -6.785  
-22 215 59625.00 I  0.016798 0.000015  0.345873 0.000010  I-0.1029904 0.0000044 -0.5481 0.0026  I  -108.624    0.610    -6.831    0.135  0.016814  0.345848 -0.1029937  -108.690    -6.864  
-22 216 59626.00 I  0.016421 0.000022  0.347660 0.000013  I-0.1025441 0.0000039 -0.3550 0.0029  I  -108.503    0.578    -6.768    0.218  0.016373  0.347600 -0.1025279  -108.569    -6.803  
-22 217 59627.00 I  0.016159 0.000022  0.349967 0.000013  I-0.1022883 0.0000039 -0.1382 0.0028  I  -108.306    0.578    -6.657    0.218  0.016174  0.349955 -0.1022855  -108.379    -6.702  
-22 218 59628.00 I  0.015966 0.000020  0.352553 0.000012  I-0.1022741 0.0000039  0.0976 0.0031  I  -108.164    0.578    -6.608    0.218  0.015893  0.352552 -0.1022778  -108.238    -6.679  
-22 219 59629.00 I  0.016039 0.000018  0.354982 0.000013  I-0.1024662 0.0000047  0.2814 0.0029  I  -108.174    0.550    -6.645    0.272  0.016057  0.355009 -0.1024803  -108.239    -6.688  
-22 220 59630.00 I  0.016151 0.000029  0.357317 0.000016  I-0.1028123 0.0000042  0.3915 0.0031  I  -108.316    0.533    -6.707    0.218  0.016152  0.357350 -0.1028229  -108.367    -6.714  
-22 221 59631.00 I  0.016267 0.000030  0.359419 0.000016  I-0.1032028 0.0000041  0.3625 0.0033  I  -108.531    0.533    -6.723    0.218  0.016225  0.359459 -0.1032042  -108.568    -6.699  
-22 222 59632.00 I  0.016726 0.000027  0.361250 0.000014  I-0.1035161 0.0000050  0.2701 0.0027  I  -108.789    0.477    -6.674    0.059  0.016672  0.361277 -0.1035256  -108.817    -6.617  
-22 223 59633.00 I  0.017620 0.000030  0.362774 0.000014  I-0.1037175 0.0000034  0.1014 0.0031  I  -109.046    0.472    -6.605    0.143  0.017619  0.362779 -0.1037081  -109.078    -6.583  
-22 224 59634.00 I  0.018442 0.000030  0.364353 0.000015  I-0.1036983 0.0000035 -0.1292 0.0023  I  -109.216    0.472    -6.591    0.143  0.018496  0.364360 -0.1036928  -109.259    -6.613  
-22 225 59635.00 I  0.018979 0.000030  0.365795 0.000013  I-0.1034719 0.0000031 -0.3215 0.0025  I  -109.215    0.472    -6.678    0.143  0.018931  0.365807 -0.1034734  -109.270    -6.743  
-22 226 59636.00 I  0.019617 0.000020  0.367246 0.000008  I-0.1030795 0.0000035 -0.4411 0.0025  I  -109.042    0.467    -6.844    0.189  0.019607  0.367229 -0.1031018  -109.106    -6.902  
-22 227 59637.00 I  0.020237 0.000029  0.368838 0.000010  I-0.1026452 0.0000038 -0.3942 0.0026  I  -108.783    0.438    -7.004    0.149  0.020241  0.368836 -0.1026797  -108.854    -7.042  
-22 228 59638.00 I  0.020644 0.000029  0.370619 0.000011  I-0.1023227 0.0000039 -0.2524 0.0031  I  -108.547    0.438    -7.087    0.149  0.020656  0.370624 -0.1023250  -108.624    -7.107  
-22 3 1 59639.00 I  0.020988 0.000025  0.372332 0.000010  I-0.1021455 0.0000048 -0.0954 0.0030  I  -108.383    0.405    -7.104    0.093  0.020909  0.372342 -0.1021425  -108.462    -7.107  
-22 3 2 59640.00 I  0.021874 0.000028  0.374026 0.000012  I-0.1021640 0.0000046  0.1578 0.0033  I  -108.257    0.523    -7.117    0.099  0.021778  0.373951 -0.1021944  -108.199    -7.104  
-22 3 3 59641.00 I  0.023306 0.000028  0.376266 0.000011  I-0.1024446 0.0000046  0.3615 0.0033  I  -108.130    0.523    -7.148    0.099  0.023290  0.376273 -0.1024561  -107.898    -7.117  
-22 3 4 59642.00 I  0.025006 0.000028  0.378497 0.000012  I-0.1028384 0.0000047  0.4193 0.0039  I  -108.041    0.523    -7.157    0.099  0.024972  0.378479 -0.1028435  -107.637    -7.109  
-22 3 5 59643.00 I  0.026706 0.000017  0.380550 0.000010  I-0.1032446 0.0000063  0.3614 0.0030  I  -108.086    0.762    -7.123    0.115  0.026774  0.380581 -0.1032424  -107.706    -7.086  
-22 3 6 59644.00 I  0.028126 0.000021  0.382624 0.000012  I-0.1035438 0.0000037  0.2513 0.0037  I  -108.303    0.501    -7.108    0.074  0.028086  0.382600 -0.1035550  -108.027    -7.094  
-22 3 7 59645.00 I  0.029547 0.000020  0.384741 0.000012  I-0.1037274 0.0000038  0.0817 0.0025  I  -108.606    0.501    -7.183    0.074  0.029543  0.384798 -0.1037203  -108.450    -7.191  
-22 3 8 59646.00 I  0.030999 0.000016  0.386701 0.000011  I-0.1036824 0.0000033 -0.1622 0.0023  I  -108.837    0.446    -7.322    0.061  0.031018  0.386712 -0.1036844  -108.826    -7.354  
-22 3 9 59647.00 I  0.032216 0.000019  0.388513 0.000016  I-0.1034083 0.0000027 -0.3901 0.0021  I  -108.858    0.640    -7.427    0.047  0.032281  0.388541 -0.1034089  -108.866    -7.460  
-22 310 59648.00 I  0.033082 0.000019  0.390309 0.000016  I-0.1029234 0.0000026 -0.5542 0.0019  I  -108.611    0.640    -7.449    0.047  0.033104  0.390312 -0.1029383  -108.612    -7.475  
-22 311 59649.00 I  0.033672 0.000020  0.392120 0.000016  I-0.1023277 0.0000027 -0.6348 0.0022  I  -108.133    0.640    -7.456    0.047  0.033708  0.392105 -0.1023346  -108.109    -7.473  
-22 312 59650.00 I  0.034135 0.000018  0.393692 0.000015  I-0.1016715 0.0000035 -0.6623 0.0025  I  -107.560    0.785    -7.563    0.029  0.034130  0.393729 -0.1016864  -107.569    -7.581  
-22 313 59651.00 I  0.034427 0.000025  0.395169 0.000020  I-0.1010165 0.0000043 -0.6496 0.0028  I  -107.077    0.707    -7.794    0.042  0.034502  0.395152 -0.1010372  -107.117    -7.813  
-22 314 59652.00 I  0.034370 0.000025  0.396639 0.000019  I-0.1003901 0.0000043 -0.5833 0.0037  I  -106.827    0.707    -8.046    0.042  0.034354  0.396685 -0.1004104  -106.877    -8.063  
-22 315 59653.00 I  0.034234 0.000023  0.398077 0.000015  I-0.0998758 0.0000061 -0.4391 0.0032  I  -106.816    0.600    -8.186    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
-22 316 59654.00 I  0.033955 0.000033  0.399538 0.000017  I-0.0995335 0.0000048 -0.2299 0.0039  I  -106.912    0.616    -8.162    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
-22 317 59655.00 I  0.033459 0.000033  0.401249 0.000017  I-0.0994318 0.0000047  0.0269 0.0035  I  -106.970    0.616    -8.032    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
-22 318 59656.00 I  0.033076 0.000031  0.402917 0.000017  I-0.0995528 0.0000051  0.1803 0.0034  I  -106.956    0.616    -7.901    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
-22 319 59657.00 I  0.032925 0.000026  0.404430 0.000011  I-0.0997804 0.0000048  0.2978 0.0035  I  -106.966    0.655    -7.846    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
-22 320 59658.00 I  0.033031 0.000026  0.405970 0.000011  I-0.1001534 0.0000047  0.4302 0.0032  I  -107.127    0.655    -7.885    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
-22 321 59659.00 I  0.033373 0.000033  0.407434 0.000014  I-0.1005681 0.0000043  0.3445 0.0036  I  -107.460    0.570    -7.976    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
-22 322 59660.00 I  0.034272 0.000023  0.408887 0.000012  I-0.1007879 0.0000054  0.0955 0.0031  I  -107.841    0.533    -8.058    0.070  0.034163  0.408866 -0.1007374  -107.806    -8.084  
-22 323 59661.00 I  0.035751 0.000025  0.410764 0.000016  I-0.1007727 0.0000045 -0.1126 0.0035  I  -108.083    0.498    -8.100    0.073  0.035739  0.410677 -0.1007668  -108.069    -8.122  
-22 324 59662.00 I  0.037151 0.000025  0.412870 0.000016  I-0.1005689 0.0000044 -0.3020 0.0031  I  -108.063    0.498    -8.123    0.073  0.037184  0.412921 -0.1005632  -108.121    -8.146  
-22 325 59663.00 I  0.038266 0.000025  0.415013 0.000016  I-0.1001861 0.0000042 -0.4391 0.0031  I  -107.769    0.498    -8.166    0.073  0.038276  0.415002 -0.1001852  -107.917    -8.187  
-22 326 59664.00 I  0.039265 0.000024  0.416909 0.000016  I-0.0997290 0.0000045 -0.4614 0.0032  I  -107.300    0.498    -8.239    0.073  0.039275  0.416959 -0.0997325  -107.413    -8.263  
-22 327 59665.00 I  0.040351 0.000020  0.418580 0.000016  I-0.0993023 0.0000047 -0.3667 0.0033  I  -106.811    0.528    -8.320    0.082  0.040293  0.418593 -0.0993188  -106.847    -8.345  
-22 328 59666.00 I  0.041640 0.000019  0.420162 0.000016  I-0.0990360 0.0000047 -0.1509 0.0038  I  -106.452    0.528    -8.385    0.082  0.041691  0.420175 -0.0990554  -106.412    -8.410  
-22 329 59667.00 I  0.042745 0.000018  0.421728 0.000013  I-0.0989805 0.0000059  0.0047 0.0033  I  -106.300    0.617    -8.424    0.088  0.042792  0.421696 -0.0989777  -106.189    -8.449  
-22 330 59668.00 I  0.043408 0.000022  0.423080 0.000020  I-0.0990298 0.0000047  0.1133 0.0038  I  -106.336    0.617    -8.430    0.097  0.043491  0.423055 -0.0990426  -106.244    -8.453  
-22 331 59669.00 I  0.043545 0.000023  0.424811 0.000021  I-0.0992189 0.0000049  0.2572 0.0034  I  -106.449    0.617    -8.391    0.097  0.043570  0.424794 -0.0992346  -106.398    -8.414  
-22 4 1 59670.00 I  0.043354 0.000024  0.426955 0.000021  I-0.0995113 0.0000050  0.3023 0.0038  I  -106.519    0.617    -8.316    0.097  0.043301  0.426919 -0.0995031  -106.506    -8.343  
-22 4 2 59671.00 I  0.043559 0.000019  0.428890 0.000019  I-0.0997947 0.0000057  0.2611 0.0040  I  -106.522    0.617    -8.258    0.101  0.043471  0.428898 -0.0997958  -106.536    -8.278  
-22 4 3 59672.00 I  0.044379 0.000022  0.431003 0.000021  I-0.1000072 0.0000063  0.1410 0.0042  I  -106.546    0.606    -8.280    0.077  0.044401  0.430964 -0.1000185  -106.583    -8.291  
-22 4 4 59673.00 I  0.045127 0.000022  0.433545 0.000021  I-0.1000651 0.0000062 -0.0137 0.0051  I  -106.670    0.606    -8.393    0.077  0.045179  0.433548 -0.1000877  -106.727    -8.395  
-22 4 5 59674.00 I  0.045607 0.000017  0.436177 0.000015  I-0.0999591 0.0000081 -0.2303 0.0049  I  -106.846    0.592    -8.523    0.031  0.045558  0.436184 -0.0999601  -106.928    -8.515  
-22 4 6 59675.00 I  0.046389 0.000020  0.438254 0.000021  I-0.0996005 0.0000075 -0.4588 0.0055  I  -106.936    0.628    -8.593    0.040  0.046324  0.438296 -0.0996161  -107.011    -8.588  
-22 4 7 59676.00 I  0.047706 0.000019  0.440059 0.000021  I-0.0990853 0.0000073 -0.5559 0.0053  I  -106.835    0.628    -8.610    0.040  0.047660  0.440084 -0.0991087  -106.904    -8.610  
-22 4 8 59677.00 I  0.049434 0.000019  0.441857 0.000021  I-0.0985112 0.0000074 -0.5853 0.0053  I  -106.535    0.628    -8.668    0.040  0.049412  0.441800 -0.0985116  -106.602    -8.670  
-22 4 9 59678.00 I  0.051228 0.000016  0.443562 0.000018  I-0.0979307 0.0000077 -0.5666 0.0050  I  -106.076    0.659    -8.845    0.046  0.051279  0.443588 -0.0979207  -106.131    -8.844  
-22 410 59679.00 I  0.052563 0.000017  0.445329 0.000020  I-0.0973867 0.0000066 -0.5219 0.0051  I  -105.537    0.793    -9.110    0.054  0.052631  0.445310 -0.0973816  -105.574    -9.106  
-22 411 59680.00 I  0.053446 0.000016  0.447045 0.000019  I-0.0969104 0.0000066 -0.4066 0.0041  I  -105.077    0.793    -9.359    0.054  0.053447  0.447037 -0.0969159  -105.095    -9.347  
-22 412 59681.00 I  0.054291 0.000014  0.449051 0.000019  I-0.0965830 0.0000048 -0.2627 0.0041  I  -104.899    0.832    -9.512    0.125  0.054284  0.449011 -0.0965845  -104.884    -9.491  
-22 413 59682.00 I  0.055326 0.000013  0.451031 0.000018  I-0.0964181 0.0000047 -0.0195 0.0035  I  -105.058    0.832    -9.557    0.125  0.055292  0.451073 -0.0964523  -105.062    -9.565  
-22 414 59683.00 I  0.056532 0.000013  0.452922 0.000018  I-0.0965550 0.0000050  0.2567 0.0034  I  -105.350    0.832    -9.494    0.125  0.056547  0.452892 -0.0965557  -105.379    -9.547  
-22 415 59684.00 I  0.057880 0.000017  0.454452 0.000019  I-0.0968978 0.0000048  0.4317 0.0032  I  -105.519    0.832    -9.312    0.125  0.057823  0.454485 -0.0968994  -105.550    -9.362  
-22 416 59685.00 I  0.059421 0.000020  0.456175 0.000017  I-0.0974023 0.0000040  0.5583 0.0032  I  -105.579    0.796    -9.059    0.167  0.059424  0.456172 -0.0974129  -105.603    -9.095  
-22 417 59686.00 I  0.061288 0.000021  0.457791 0.000017  I-0.0979718 0.0000043  0.5570 0.0043  I  -105.787    0.796    -8.879    0.167  0.061164  0.457851 -0.0979865  -105.807    -8.908  
-22 418 59687.00 I  0.063720 0.000023  0.459297 0.000016  I-0.0984742 0.0000077  0.4292 0.0045  I  -106.253    0.724    -8.900    0.008  0.063734  0.459266 -0.0985020  -106.274    -8.922  
-22 419 59688.00 I  0.066168 0.000025  0.460808 0.000016  I-0.0988056 0.0000079  0.2274 0.0046  I  -106.740    0.724    -9.095    0.008  0.066192  0.460869 -0.0988272  -106.773    -9.104  
-22 420 59689.00 I  0.068334 0.000027  0.462047 0.000025  I-0.0988956 0.0000051 -0.0747 0.0047  I  -106.903    0.795    -9.307    0.093  0.068329  0.461999 -0.0988949  -106.960    -9.291  
-22 421 59690.00 I  0.070493 0.000026  0.463020 0.000025  I-0.0986762 0.0000052 -0.3169 0.0038  I  -106.654    0.795    -9.426    0.093  0.070468  0.463064 -0.0987060  -106.695    -9.434  
-22 422 59691.00 I  0.072756 0.000022  0.464164 0.000025  I-0.0983194 0.0000055 -0.3863 0.0037  I  -106.197    0.795    -9.466    0.093  0.072707  0.464098 -0.0983386  -106.211    -9.508  
-22 423 59692.00 I  0.075224 0.000021  0.465060 0.000025  I-0.0979197 0.0000054 -0.4074 0.0041  I  -105.773    0.795    -9.494    0.093  0.075204  0.465058 -0.0979051  -105.797    -9.527  
-22 424 59693.00 I  0.077857 0.000018  0.466295 0.000037  I-0.0975341 0.0000060 -0.3401 0.0040  I  -105.461    0.842    -9.540    0.119  0.077859  0.466247 -0.0975194  -105.498    -9.555  
-22 425 59694.00 I  0.080484 0.000016  0.467898 0.000037  I-0.0972695 0.0000059 -0.1828 0.0059  I  -105.224    0.842    -9.588    0.119  0.080557  0.467896 -0.0972632  -105.265    -9.590  
-22 426 59695.00 I  0.082817 0.000011  0.469933 0.000032  I-0.0971736 0.0000101 -0.0103 0.0041  I  -105.067    0.779    -9.602    0.091  0.082859  0.469891 -0.0971847  -105.109    -9.593  
-22 427 59696.00 I  0.084840 0.000018  0.471422 0.000034  I-0.0972297 0.0000057  0.1047 0.0058  I  -105.061    0.809    -9.544    0.149  0.084908  0.471486 -0.0972203  -105.096    -9.548  
-22 428 59697.00 I  0.086492 0.000019  0.472746 0.000034  I-0.0973573 0.0000055  0.1428 0.0042  I  -105.231    0.809    -9.382    0.149  0.086518  0.472819 -0.0973522  -105.258    -9.407  
-22 429 59698.00 I  0.087932 0.000019  0.473573 0.000035  I-0.0974929 0.0000062  0.1137 0.0038  I  -105.466    0.809    -9.149    0.149  0.087895  0.473595 -0.0974914  -105.480    -9.203  
-22 430 59699.00 I  0.089677 0.000019  0.474059 0.000016  I-0.0975659 0.0000052  0.0282 0.0040  I  -105.611    0.840    -8.964    0.195  0.089653  0.474104 -0.0975559  -105.614    -9.011  
-22 5 1 59700.00 I  0.091697 0.000020  0.474621 0.000017  I-0.0975399 0.0000052 -0.0855 0.0037  I  -105.636    0.840    -8.956    0.195  0.091728  0.474632 -0.0975257  -105.627    -8.987  
-22 5 2 59701.00 I  0.093634 0.000024  0.475322 0.000022  I-0.0973966 0.0000054 -0.1939 0.0042  I  -105.635    0.789    -9.133    0.114  0.093634  0.475311 -0.0974187  -105.619    -9.154  
-22 5 3 59702.00 I  0.095566 0.000019  0.476101 0.000018  I-0.0971749 0.0000066 -0.2337 0.0043  I  -105.680    0.775    -9.361    0.031  0.095563  0.476140 -0.0972185  -105.662    -9.372  
-22 5 4 59703.00 I  0.097692 0.000024  0.476979 0.000028  I-0.0969099 0.0000066 -0.3313 0.0046  I  -105.740    0.803    -9.494    0.034  0.097691  0.476906 -0.0969126  -105.734    -9.493  
-22 5 5 59704.00 I  0.099819 0.000025  0.477843 0.000028  I-0.0965003 0.0000065 -0.4650 0.0047  I  -105.760    0.803    -9.531    0.034  0.099882  0.477903 -0.0964992  -105.770    -9.526  
-22 5 6 59705.00 I  0.101673 0.000025  0.478886 0.000027  I-0.0960202 0.0000066 -0.4778 0.0046  I  -105.729    0.803    -9.600    0.034  0.101687  0.478833 -0.0960256  -105.754    -9.581  
-22 5 7 59706.00 I  0.103387 0.000026  0.479471 0.000026  I-0.0955612 0.0000066 -0.4412 0.0046  I  -105.611    0.803    -9.787    0.034  0.103404  0.479538 -0.0955546  -105.646    -9.779  
-22 5 8 59707.00 I  0.105104 0.000025  0.480073 0.000028  I-0.0951513 0.0000064 -0.3643 0.0046  I  -105.317    0.823   -10.025    0.110  0.105117  0.480078 -0.0951550  -105.347   -10.030  
-22 5 9 59708.00 I  0.106696 0.000026  0.480500 0.000028  I-0.0948663 0.0000064 -0.1865 0.0045  I  -104.887    0.823   -10.186    0.110  0.106699  0.480537 -0.0949242  -104.904   -10.197  
-22 510 59709.00 I  0.108520 0.000020  0.481018 0.000019  I-0.0947999 0.0000062  0.0561 0.0039  I  -104.601    0.786   -10.242    0.154  0.108427  0.480933 -0.0948334  -104.607   -10.261  
-22 511 59710.00 I  0.110913 0.000020  0.481753 0.000030  I-0.0949930 0.0000045  0.3422 0.0039  I  -104.725    0.784   -10.269    0.175  0.110941  0.481776 -0.0950144  -104.732   -10.281  
-22 512 59711.00 I  0.113494 0.000019  0.482660 0.000030  I-0.0954576 0.0000047  0.5482 0.0034  I  -105.149    0.784   -10.278    0.175  0.113474  0.482707 -0.0954543  -105.174   -10.290  
-22 513 59712.00 I  0.116067 0.000019  0.483438 0.000030  I-0.0960586 0.0000051  0.6620 0.0038  I  -105.514    0.784   -10.142    0.175  0.116107  0.483379 -0.0960629  -105.566   -10.162  
-22 514 59713.00 I  0.118511 0.000016  0.483916 0.000024  I-0.0967483 0.0000059  0.6760 0.0039  I  -105.714    0.783    -9.781    0.191  0.118527  0.483975 -0.0967431  -105.773    -9.799  
-22 515 59714.00 I  0.120714 0.000024  0.484483 0.000034  I-0.0973707 0.0000059  0.5703 0.0042  I  -106.022    0.853    -9.383    0.166  0.120799  0.484444 -0.0973670  -106.086    -9.399  
-22 516 59715.00 I  0.122294 0.000025  0.485269 0.000034  I-0.0978722 0.0000060  0.4145 0.0054  I  -106.587    0.853    -9.262    0.166  0.122385  0.485333 -0.0978659  -106.653    -9.281  
-22 517 59716.00 I  0.123270 0.000025  0.485893 0.000025  I-0.0981791 0.0000090  0.1968 0.0054  I  -107.085    0.963    -9.493    0.130  0.123240  0.485912 -0.0981728  -107.146    -9.513  
-22 518 59717.00 I  0.124657 0.000031  0.485630 0.000039  I-0.0982668 0.0000091 -0.0179 0.0064  I  -107.098    0.997    -9.832    0.133  0.124614  0.485666 -0.0982338  -107.148    -9.846  
-22 519 59718.00 I  0.126489 0.000029  0.485537 0.000039  I-0.0981549 0.0000091 -0.1978 0.0065  I  -106.633    0.997   -10.029    0.133  0.126492  0.485563 -0.0980742  -106.655   -10.034  
-22 520 59719.00 I  0.128443 0.000029  0.485661 0.000039  I-0.0979220 0.0000092 -0.2253 0.0069  I  -106.083    0.997   -10.073    0.133  0.128370  0.485536 -0.0979421  -106.062   -10.068  
-22 521 59720.00 I  0.130660 0.000023  0.485998 0.000032  I-0.0977440 0.0000103 -0.1339 0.0061  I  -105.784    1.070   -10.078    0.139  0.130677  0.486020 -0.0977739  -105.765   -10.071  
-22 522 59721.00 I  0.132973 0.000025  0.486761 0.000040  I-0.0976717 0.0000080  0.0098 0.0065  I  -105.760    0.848   -10.064    0.091  0.132949  0.486774 -0.0977075  -105.758   -10.059  
-22 523 59722.00 I  0.135354 0.000026  0.487348 0.000039  I-0.0977660 0.0000079  0.1605 0.0055  I  -105.829    0.848    -9.980    0.091  0.135359  0.487350 -0.0977582  -105.848    -9.982  
-22 524 59723.00 I  0.137671 0.000020  0.488199 0.000026  I-0.0979704 0.0000075  0.2443 0.0054  I  -105.844    0.782    -9.818    0.064  0.137703  0.488205 -0.0979698  -105.891    -9.829  
-22 525 59724.00 I  0.139654 0.000022  0.488515 0.000036  I-0.0982384 0.0000075  0.2793 0.0053  I  -105.828    0.831    -9.611    0.068  0.139642  0.488593 -0.0982642  -105.852    -9.614  
-22 526 59725.00 I  0.141661 0.000021  0.488486 0.000036  I-0.0984963 0.0000075  0.2160 0.0053  I  -105.918    0.831    -9.372    0.068  0.141637  0.488529 -0.0985094  -105.918    -9.361  
-22 527 59726.00 I  0.143575 0.000022  0.488507 0.000036  I-0.0986419 0.0000074  0.0672 0.0056  I  -106.168    0.831    -9.113    0.068  0.143638  0.488445 -0.0986407  -106.153    -9.084  
-22 528 59727.00 I  0.145157 0.000018  0.488342 0.000026  I-0.0986060 0.0000084 -0.1556 0.0056  I  -106.455    0.876    -8.932    0.072  0.145102  0.488400 -0.0986068  -106.467    -8.914  
-22 529 59728.00 I  0.146683 0.000016  0.488248 0.000026  I-0.0983124 0.0000083 -0.4333 0.0055  I  -106.618    0.876    -8.975    0.072  0.146706  0.488268 -0.0983314  -106.669    -8.976  
-22 530 59729.00 I  0.148142 0.000026  0.487976 0.000038  I-0.0977395 0.0000070 -0.7105 0.0053  I  -106.623    0.864    -9.281    0.057  0.148067  0.488086 -0.0977877  -106.716    -9.292  
-22 531 59730.00 I  0.149846 0.000025  0.487063 0.000029  I-0.0969106 0.0000065 -0.9299 0.0045  I  -106.562    0.840    -9.686    0.031  0.149795  0.487092 -0.0969563  -106.700    -9.703  
-22 6 1 59731.00 I  0.151999 0.000031  0.486256 0.000040  I-0.0959031 0.0000056 -1.0791 0.0045  I  -106.542    1.030    -9.952    0.050  0.151943  0.486170 -0.0959109  -106.731    -9.971  
-22 6 2 59732.00 I  0.154335 0.000031  0.485376 0.000039  I-0.0947794 0.0000062 -1.1475 0.0043  I  -106.621    1.030   -10.003    0.050  0.154357  0.485426 -0.0947757  -106.670   -10.005  
-22 6 3 59733.00 I  0.156607 0.000030  0.484838 0.000039  I-0.0936407 0.0000066 -1.1183 0.0048  I  -106.804    1.030    -9.972    0.050  0.156589  0.484781 -0.0936356  -106.660    -9.955  
-22 6 4 59734.00 I  0.158876 0.000031  0.484115 0.000039  I-0.0925698 0.0000074 -1.0082 0.0064  I  -106.995    1.030   -10.005    0.050  0.158889  0.484149 -0.0925602  -106.851    -9.984  
-22 6 5 59735.00 I  0.161157 0.000021  0.483629 0.000028  I-0.0916234 0.0000110 -0.9009 0.0056  I  -107.006    1.266   -10.076    0.066  0.161161  0.483622 -0.0916220  -106.921   -10.058  
-22 6 6 59736.00 I  0.163477 0.000027  0.483154 0.000033  I-0.0907768 0.0000085 -0.7674 0.0075  I  -106.756    0.996   -10.057    0.087  0.163382  0.483150 -0.0908246  -106.715   -10.044  
-22 6 7 59737.00 I  0.166258 0.000021  0.482825 0.000019  I-0.0901222 0.0000102 -0.5331 0.0062  I  -106.478    0.872    -9.931    0.096  0.166198  0.482812 -0.0901686  -106.474    -9.925  
-22 6 8 59738.00 I  0.169363 0.000027  0.482891 0.000038  I-0.0896770 0.0000090 -0.3995 0.0068  I  -106.547    0.889    -9.830    0.091  0.169346  0.482843 -0.0896819  -106.581    -9.834  
-22 6 9 59739.00 I  0.172338 0.000027  0.482824 0.000038  I-0.0893166 0.0000089 -0.2858 0.0061  I  -107.042    0.889    -9.826    0.091  0.172338  0.482895 -0.0893344  -107.056    -9.817  
-22 610 59740.00 I  0.175169 0.000026  0.482943 0.000038  I-0.0890927 0.0000083 -0.2102 0.0060  I  -107.668    0.889    -9.774    0.091  0.175150  0.482907 -0.0890843  -107.652    -9.745  
-22 611 59741.00 I  0.177825 0.000027  0.482603 0.000038  I-0.0888449 0.0000080 -0.2886 0.0055  I  -108.215    0.889    -9.494    0.091  0.177834  0.482720 -0.0888551  -108.201    -9.465  
-22 612 59742.00 I  0.180321 0.000023  0.482005 0.000041  I-0.0884903 0.0000073 -0.4425 0.0053  I  -108.808    0.779    -9.107    0.101  0.180290  0.482016 -0.0885165  -108.809    -9.083  
-22 613 59743.00 I  0.182802 0.000023  0.481196 0.000041  I-0.0879262 0.0000071 -0.6974 0.0051  I  -109.514    0.779    -8.964    0.101  0.182826  0.481258 -0.0879480  -109.531    -8.942  
-22 614 59744.00 I  0.185074 0.000016  0.480440 0.000025  I-0.0870864 0.0000072 -0.9794 0.0049  I  -109.993    0.724    -9.208    0.111  0.185100  0.480403 -0.0870940  -110.036    -9.188  
-22 615 59745.00 I  0.187071 0.000035  0.479251 0.000038  I-0.0859877 0.0000068 -1.2004 0.0050  I  -109.870    0.734    -9.587    0.125  0.187052  0.479331 -0.0859830  -109.873    -9.588  
-22 616 59746.00 I  0.189200 0.000035  0.478011 0.000038  I-0.0847345 0.0000068 -1.2746 0.0048  I  -109.272    0.734    -9.808    0.125  0.189149  0.478024 -0.0847332  -109.222    -9.837  
-22 617 59747.00 I  0.191611 0.000035  0.476754 0.000038  I-0.0834981 0.0000068 -1.1701 0.0058  I  -108.689    0.734    -9.874    0.125  0.191602  0.476728 -0.0834949  -108.594    -9.934  
-22 618 59748.00 I  0.194038 0.000032  0.475522 0.000030  I-0.0824289 0.0000093 -0.9619 0.0063  I  -108.459    0.898    -9.926    0.199  0.194019  0.475550 -0.0824189  -108.365    -9.983  
-22 619 59749.00 I  0.196594 0.000032  0.474527 0.000030  I-0.0815690 0.0000105 -0.7696 0.0059  I  -108.583    0.898    -9.933    0.199  0.196541  0.474534 -0.0815575  -108.509    -9.976  
-22 620 59750.00 I  0.199463 0.000034  0.473569 0.000035  I-0.0808708 0.0000072 -0.6340 0.0063  I  -108.896    0.835    -9.762    0.155  0.199454  0.473574 -0.0808812  -108.836    -9.796  
-22 621 59751.00 I  0.202394 0.000013  0.472804 0.000020  I-0.0802852 0.0000069 -0.5460 0.0047  I  -109.207    0.832    -9.441    0.148  0.202403  0.472799 -0.0803109  -109.153    -9.467  
-22 622 59752.00 I  0.205094 0.000019  0.472303 0.000025  I-0.0797451 0.0000060 -0.5592 0.0046  I  -109.399    0.719    -9.156    0.139  0.205128  0.472282 -0.0797589  -109.347    -9.174  
-22 623 59753.00 I  0.207617 0.000019  0.471581 0.000026  I-0.0791176 0.0000062 -0.7200 0.0043  I  -109.533    0.719    -9.018    0.139  0.207619  0.471645 -0.0791011  -109.587    -9.025  
-22 624 59754.00 I  0.210141 0.000019  0.470807 0.000026  I-0.0782996 0.0000063 -0.8975 0.0045  I  -109.766    0.719    -8.977    0.139  0.210148  0.470821 -0.0782976  -109.961    -8.971  
-22 625 59755.00 I  0.212733 0.000020  0.469677 0.000026  I-0.0773290 0.0000064 -1.0560 0.0046  I  -110.124    0.719    -8.981    0.139  0.212693  0.469719 -0.0773260  -110.305    -8.982  
-22 626 59756.00 I  0.215401 0.000025  0.468452 0.000028  I-0.0761678 0.0000067 -1.2740 0.0047  I  -110.449    0.715    -9.097    0.145  0.215376  0.468485 -0.0761726  -110.571    -9.112  
-22 627 59757.00 I  0.218223 0.000025  0.467013 0.000027  I-0.0748068 0.0000069 -1.4146 0.0054  I  -110.584    0.715    -9.400    0.145  0.218164  0.467038 -0.0748406  -110.659    -9.428  
-22 628 59758.00 I  0.221333 0.000021  0.465645 0.000024  I-0.0733560 0.0000085 -1.5028 0.0056  I  -110.545    0.907    -9.791    0.161  0.221330  0.465623 -0.0733645  -110.576    -9.834  
-22 629 59759.00 I  0.224403 0.000022  0.464126 0.000037  I-0.0718010 0.0000088 -1.5914 0.0063  I  -110.489    0.982   -10.034    0.135  0.224443  0.464165 -0.0718011  -110.473   -10.052  
-22 630 59760.00 I  0.227228 0.000022  0.462592 0.000036  I-0.0702027 0.0000092 -1.5915 0.0064  I  -110.548    0.982    -9.993    0.135  0.227220  0.462671 -0.0702118  -110.474    -9.975  
-22 7 1 59761.00 I  0.230016 0.000022  0.460896 0.000036  I-0.0686534 0.0000094 -1.4852 0.0080  I  -110.748    0.982    -9.779    0.135  0.230002  0.460818 -0.0686663  -110.599    -9.722  
-22 7 2 59762.00 I  0.232935 0.000012  0.459188 0.000030  I-0.0672368 0.0000131 -1.3652 0.0073  I  -111.002    1.080    -9.605    0.072  0.232881  0.459225 -0.0672447  -110.959    -9.582  
-22 7 3 59763.00 I  0.236098 0.000015  0.457832 0.000039  I-0.0659446 0.0000112 -1.1803 0.0086  I  -111.152    0.913    -9.542    0.143  0.236109  0.457809 -0.0659625  -111.150    -9.536  
-22 7 4 59764.00 I  0.239190 0.000015  0.456523 0.000040  I-0.0649100 0.0000110 -0.8941 0.0074  I  -111.085    0.913    -9.489    0.143  0.239234  0.456579 -0.0649159  -111.121    -9.498  
-22 7 5 59765.00 I  0.241892 0.000015  0.455190 0.000036  I-0.0641384 0.0000096 -0.6619 0.0071  I  -110.905    0.851    -9.367    0.185  0.241892  0.455171 -0.0641393  -110.976    -9.390  
-22 7 6 59766.00 I  0.244461 0.000014  0.453250 0.000036  I-0.0635510 0.0000090 -0.5352 0.0065  I  -110.908    0.851    -9.242    0.185  0.244450  0.453302 -0.0635337  -110.950    -9.262  
-22 7 7 59767.00 I  0.247122 0.000014  0.451664 0.000036  I-0.0630480 0.0000089 -0.4683 0.0063  I  -111.302    0.851    -9.212    0.185  0.247124  0.451582 -0.0630501  -111.305    -9.226  
-22 7 8 59768.00 I  0.249746 0.000014  0.450082 0.000036  I-0.0625849 0.0000089 -0.4898 0.0064  I  -111.986    0.851    -9.221    0.185  0.249756  0.450120 -0.0625785  -111.978    -9.228  
-22 7 9 59769.00 I  0.252293 0.000012  0.448663 0.000027  I-0.0620258 0.0000093 -0.6390 0.0054  I  -112.729    0.943    -9.129    0.218  0.252297  0.448682 -0.0620271  -112.723    -9.129  
-22 710 59770.00 I  0.254695 0.000018  0.447032 0.000030  I-0.0612787 0.0000060 -0.8726 0.0057  I  -113.425    0.796    -8.964    0.149  0.254733  0.447060 -0.0612967  -113.423    -8.960  
-22 711 59771.00 I  0.256801 0.000017  0.445386 0.000019  I-0.0602829 0.0000065 -1.0991 0.0044  I  -113.996    0.755    -8.945    0.115  0.256857  0.445395 -0.0603249  -114.007    -8.936  
-22 712 59772.00 I  0.258318 0.000017  0.443966 0.000019  I-0.0591144 0.0000065 -1.2238 0.0048  I  -114.213    0.755    -9.158    0.115  0.258411  0.443974 -0.0591324  -114.246    -9.142  
-22 713 59773.00 I  0.259225 0.000018  0.442014 0.000026  I-0.0578251 0.0000071 -1.3792 0.0048  I  -113.935    0.783    -9.395    0.154  0.259174  0.442066 -0.0577813  -113.960    -9.403  
-22 714 59774.00 I  0.260257 0.000018  0.439905 0.000025  I-0.0564307 0.0000072 -1.3105 0.0051  I  -113.405    0.783    -9.445    0.154  0.260201  0.439888 -0.0564587  -113.418    -9.484  
-22 715 59775.00 I  0.261703 0.000019  0.438170 0.000025  I-0.0552591 0.0000073 -1.0768 0.0065  I  -113.034    0.783    -9.394    0.154  0.261642  0.438122 -0.0552630  -113.037    -9.466  
-22 716 59776.00 I  0.263450 0.000015  0.436331 0.000022  I-0.0542681 0.0000109 -0.8702 0.0055  I  -112.980    0.857    -9.438    0.216  0.263441  0.436373 -0.0542876  -112.983    -9.496  
-22 717 59777.00 I  0.265297 0.000018  0.434383 0.000022  I-0.0535132 0.0000083 -0.6802 0.0068  I  -113.166    0.907    -9.519    0.145  0.265267  0.434398 -0.0535228  -113.161    -9.544  
-22 718 59778.00 I  0.267260 0.000019  0.432326 0.000022  I-0.0528764 0.0000082 -0.5841 0.0056  I  -113.524    0.907    -9.408    0.145  0.267234  0.432352 -0.0528927  -113.506    -9.398  
-22 719 59779.00 I  0.269238 0.000019  0.430313 0.000013  I-0.0523098 0.0000076 -0.5935 0.0055  I  -113.989    0.933    -9.085    0.075  0.269260  0.430298 -0.0523068  -113.947    -9.037  
-22 720 59780.00 I  0.270985 0.000027  0.428182 0.000028  I-0.0516582 0.0000074 -0.6963 0.0053  I  -114.395    0.857    -8.814    0.130  0.270974  0.428173 -0.0516628  -114.393    -8.784  
-22 721 59781.00 I  0.272566 0.000027  0.426241 0.000028  I-0.0509075 0.0000075 -0.8280 0.0052  I  -114.621    0.857    -8.806    0.130  0.272574  0.426255 -0.0508922  -114.674    -8.805  
-22 722 59782.00 I  0.274103 0.000027  0.424513 0.000029  I-0.0499788 0.0000074 -1.0297 0.0059  I  -114.774    0.857    -8.993    0.130  0.274053  0.424453 -0.0499591  -114.884    -9.018  
-22 723 59783.00 I  0.275659 0.000025  0.422648 0.000028  I-0.0488580 0.0000092 -1.2018 0.0055  I  -115.013    0.708    -9.183    0.183  0.275681  0.422673 -0.0488673  -115.096    -9.210  
-22 724 59784.00 I  0.277056 0.000026  0.420922 0.000035  I-0.0475835 0.0000081 -1.3492 0.0061  I  -115.302    0.799    -9.322    0.190  0.277006  0.420915 -0.0476028  -115.333    -9.343  
-22 725 59785.00 I  0.278485 0.000025  0.419309 0.000036  I-0.0461807 0.0000081 -1.4333 0.0061  I  -115.470    0.799    -9.504    0.190  0.278471  0.419285 -0.0462003  -115.452    -9.519  
-22 726 59786.00 I  0.279854 0.000016  0.417958 0.000025  I-0.0447424 0.0000092 -1.4409 0.0059  I  -115.459    0.892    -9.758    0.202  0.279867  0.417962 -0.0447491  -115.399    -9.768  
-22 727 59787.00 I  0.281074 0.000026  0.416100 0.000041  I-0.0432994 0.0000087 -1.4470 0.0068  I  -115.382    0.892    -9.944    0.202  0.281044  0.416126 -0.0432579  -115.379    -9.934  
-22 728 59788.00 I  0.282267 0.000025  0.414131 0.000040  I-0.0418483 0.0000099 -1.4533 0.0073  I  -115.353    0.892    -9.901    0.202  0.282267  0.414205 -0.0417953  -115.431    -9.867  
-22 729 59789.00 I  0.283371 0.000024  0.411916 0.000040  I-0.0404262 0.0000116 -1.3595 0.0097  I  -115.381    0.892    -9.653    0.202  0.283345  0.411841 -0.0404282  -115.538    -9.595  
-22 730 59790.00 I  0.284624 0.000024  0.409388 0.000034  I-0.0391777 0.0000166 -1.1206 0.0097  I  -115.415    0.322    -9.394    0.160  0.284587  0.409400 -0.0392089  -115.593    -9.353  
-22 731 59791.00 I  0.285988 0.000034  0.407302 0.000042  I-0.0381714 0.0000155 -0.9226 0.0114  I  -115.418    0.796    -9.280    0.318  0.286000  0.407286 -0.0381849  -115.593    -9.273  
-22 8 1 59792.00 I  0.287129 0.000035  0.405170 0.000042  I-0.0373377 0.0000155 -0.7091 0.0098  I  -115.369    0.796    -9.289    0.318  0.287161  0.405194 -0.0373892  -115.536    -9.320  
-22 8 2 59793.00 I  0.287882 0.000029  0.403321 0.000031  I-0.0367455 0.0000120 -0.5187 0.0097  I  -115.284    0.762    -9.304    0.284  0.287882  0.403262 -0.0367846  -115.439    -9.376  
-22 8 3 59794.00 I  0.288547 0.000030  0.400956 0.000032  I-0.0362588 0.0000117 -0.4530 0.0081  I  -115.272    0.762    -9.263    0.284  0.288468  0.401019 -0.0362792  -115.414    -9.314  
-22 8 4 59795.00 I  0.289527 0.000030  0.398753 0.000031  I-0.0358142 0.0000109 -0.4634 0.0079  I  -115.510    0.762    -9.205    0.284  0.289489  0.398709 -0.0358145  -115.635    -9.222  
-22 8 5 59796.00 I  0.290535 0.000029  0.396540 0.000031  I-0.0353137 0.0000106 -0.5287 0.0066  I  -116.063    0.762    -9.175    0.284  0.290582  0.396579 -0.0353263  -116.154    -9.192  
-22 8 6 59797.00 I  0.291094 0.000016  0.394201 0.000017  I-0.0347291 0.0000073 -0.6772 0.0060  I  -116.788    0.736    -9.176    0.244  0.291080  0.394221 -0.0347316  -116.838    -9.204  
-22 8 7 59798.00 I  0.291549 0.000023  0.391643 0.000021  I-0.0339357 0.0000055 -0.8967 0.0051  I  -117.423    0.716    -9.224    0.251  0.291487  0.391652 -0.0339451  -117.435    -9.261  
-22 8 8 59799.00 I  0.292338 0.000022  0.389015 0.000014  I-0.0329627 0.0000070 -1.0352 0.0045  I  -117.732    0.707    -9.356    0.256  0.292293  0.389056 -0.0329721  -117.715    -9.399  
-22 8 9 59800.00 I  0.293205 0.000022  0.386247 0.000014  I-0.0318899 0.0000071 -1.0998 0.0046  I  -117.614    0.707    -9.520    0.256  0.293211  0.386232 -0.0318918  -117.585    -9.565  
-22 810 59801.00 I  0.293835 0.000024  0.383242 0.000026  I-0.0308021 0.0000059 -1.0475 0.0048  I  -117.209    0.739    -9.544    0.271  0.293803  0.383250 -0.0308088  -117.149    -9.591  
-22 811 59802.00 I  0.294452 0.000023  0.380326 0.000027  I-0.0298461 0.0000064 -0.8416 0.0045  I  -116.855    0.739    -9.347    0.271  0.294459  0.380298 -0.0298577  -116.770    -9.397  
-22 812 59803.00 I  0.295057 0.000023  0.377858 0.000027  I-0.0291291 0.0000067 -0.6052 0.0052  I  -116.787    0.739    -9.114    0.271  0.295055  0.377755 -0.0291384  -116.681    -9.171  
-22 813 59804.00 I  0.295580 0.000016  0.375692 0.000025  I-0.0286212 0.0000082 -0.4123 0.0051  I  -116.918    0.775    -9.085    0.284  0.295537  0.375740 -0.0286307  -116.834    -9.134  
-22 814 59805.00 I  0.296375 0.000015  0.373574 0.000026  I-0.0282776 0.0000076 -0.3001 0.0053  I  -117.059    0.775    -9.225    0.284  0.296313  0.373591 -0.0282983  -117.006    -9.266  
-22 815 59806.00 I  0.297511 0.000016  0.371305 0.000030  I-0.0279766 0.0000068 -0.3210 0.0067  I  -117.234    0.763    -9.267    0.243  0.297500  0.371314 -0.0279699  -117.203    -9.307  
-22 816 59807.00 I  0.298549 0.000015  0.369034 0.000021  I-0.0276025 0.0000111 -0.4411 0.0068  I  -117.579    0.739    -9.095    0.156  0.298583  0.369059 -0.0276395  -117.555    -9.139  
-22 817 59808.00 I  0.299277 0.000022  0.366788 0.000030  I-0.0270778 0.0000117 -0.6109 0.0081  I  -118.034    0.739    -8.900    0.156  0.299254  0.366732 -0.0270866  -118.003    -8.949  
-22 818 59809.00 I  0.299911 0.000022  0.364371 0.000030  I-0.0263518 0.0000118 -0.8673 0.0083  I  -118.387    0.739    -8.906    0.156  0.299866  0.364425 -0.0263517  -118.274    -8.865  
-22 819 59810.00 I  0.300905 0.000023  0.362077 0.000030  I-0.0253535 0.0000119 -1.0928 0.0085  I  -118.557    0.739    -9.086    0.156  0.300823  0.362010 -0.0253455  -118.335    -8.928  
-22 820 59811.00 I  0.302123 0.000023  0.359734 0.000030  I-0.0241795 0.0000123 -1.2784 0.0087  I  -118.646    0.739    -9.236    0.156  0.302176  0.359779 -0.0241871  -118.439    -9.105  
-22 821 59812.00 I  0.303010 0.000024  0.357436 0.000038  I-0.0228179 0.0000126 -1.4006 0.0088  I  -118.712    0.583    -9.250    0.088  0.302992  0.357455 -0.0228266  -118.572    -9.196  
-22 822 59813.00 I  0.303769 0.000023  0.354906 0.000039  I-0.0214081 0.0000125 -1.4336 0.0083  I  -118.689    0.583    -9.228    0.088  0.303769  0.354926 -0.0213929  -118.632    -9.243  
-22 823 59814.00 I  0.304478 0.000017  0.352555 0.000032  I-0.0199843 0.0000108 -1.3658 0.0070  I  -118.541    0.583    -9.300    0.088  0.304513  0.352500 -0.0199836  -118.587    -9.375  
-22 824 59815.00 I  0.304889 0.000017  0.349871 0.000039  I-0.0186829 0.0000063 -1.2787 0.0063  I  -118.346    0.652    -9.436    0.123  0.304896  0.349874 -0.0186613  -118.307    -9.531  
-22 825 59816.00 I  0.305185 0.000015  0.347446 0.000039  I-0.0174154 0.0000065 -1.2262 0.0043  I  -118.187    0.652    -9.478    0.123  0.305201  0.347486 -0.0174037  -118.023    -9.577  
-22 826 59817.00 I  0.305352 0.000015  0.344978 0.000039  I-0.0162756 0.0000058 -1.0383 0.0043  I  -118.052    0.652    -9.337    0.123  0.305398  0.344912 -0.0162851  -117.767    -9.438  
-22 827 59818.00 I  0.305269 0.000010  0.342309 0.000026  I-0.0153427 0.0000056 -0.8388 0.0042  I  -117.902    0.898    -9.106    0.171  0.305290  0.342335 -0.0153482  -117.637    -9.193  
-22 828 59819.00 I  0.304966 0.000020  0.339926 0.000031  I-0.0146067 0.0000062 -0.6132 0.0043  I  -117.763    0.774    -8.965    0.186  0.304974  0.339946 -0.0146136  -117.565    -9.035  
-22 829 59820.00 I  0.304626 0.000019  0.337380 0.000031  I-0.0141124 0.0000066 -0.3993 0.0049  I  -117.692    0.774    -8.995    0.186  0.304586  0.337401 -0.0140968  -117.551    -9.055  
-22 830 59821.00 I  0.304494 0.000020  0.335030 0.000021  I-0.0137906 0.0000075 -0.2380 0.0043  I  -117.681    0.736    -9.122    0.195  0.304464  0.334971 -0.0137838  -117.601    -9.176  
-22 831 59822.00 I  0.304617 0.000022  0.332707 0.000025  I-0.0136135 0.0000054 -0.1456 0.0047  I  -117.698    0.747    -9.208    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
-22 9 1 59823.00 I  0.304748 0.000022  0.330389 0.000025  I-0.0134601 0.0000056 -0.1713 0.0042  I  -117.799    0.747    -9.187    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
-22 9 2 59824.00 I  0.304505 0.000022  0.327687 0.000025  I-0.0132442 0.0000064 -0.2773 0.0043  I  -118.087    0.747    -9.109    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
-22 9 3 59825.00 I  0.304211 0.000014  0.325030 0.000016  I-0.0128866 0.0000064 -0.4401 0.0043  I  -118.530    0.757    -9.072    0.134  0.304186  0.324993 -0.0128821  -118.590    -9.080  
-22 9 4 59826.00 I  0.304085 0.000016  0.322768 0.000024  I-0.0123626 0.0000058 -0.6070 0.0043  I  -118.886    0.735    -9.140    0.190  0.304085  0.322764 -0.0123741  -118.929    -9.170  
-22 9 5 59827.00 I  0.303786 0.000016  0.320441 0.000024  I-0.0117015 0.0000058 -0.6872 0.0059  I  -118.883    0.735    -9.277    0.190  0.303820  0.320481 -0.0117203  -118.916    -9.328  
-22 9 6 59828.00 I  0.303229 0.000013  0.318011 0.000020  I-0.0110168 0.0000103 -0.6816 0.0050  I  -118.485    0.709    -9.346    0.245  0.303248  0.318029 -0.0110190  -118.525    -9.426  
-22 9 7 59829.00 I  0.302620 0.000016  0.314903 0.000028  I-0.0103843 0.0000082 -0.5380 0.0064  I  -117.956    0.865    -9.204    0.195  0.302652  0.314951 -0.0103738  -117.930    -9.248  
-22 9 8 59830.00 I  0.301721 0.000017  0.311755 0.000029  I-0.0099750 0.0000075 -0.2919 0.0059  I  -117.660    0.865    -8.859    0.195  0.301793  0.311758 -0.0099952  -117.557    -8.853  
-22 9 9 59831.00 I  0.300343 0.000018  0.308729 0.000030  I-0.0098012 0.0000085 -0.0439 0.0061  I  -117.716    0.865    -8.517    0.195  0.300297  0.308670 -0.0098037  -117.537    -8.461  
-22 910 59832.00 I  0.299163 0.000016  0.305643 0.000024  I-0.0098891 0.0000096  0.2096 0.0057  I  -117.913    1.166    -8.403    0.074  0.299086  0.305665 -0.0098938  -117.785    -8.354  
-22 911 59833.00 I  0.298570 0.000025  0.302858 0.000035  I-0.0101811 0.0000077  0.3451 0.0062  I  -117.992    0.970    -8.521    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
-22 912 59834.00 I  0.298127 0.000025  0.300254 0.000036  I-0.0105439 0.0000079  0.3744 0.0060  I  -117.974    0.970    -8.669    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
-22 913 59835.00 I  0.297553 0.000024  0.297991 0.000032  I-0.0108731 0.0000093  0.2331 0.0056  I  -118.082    0.886    -8.702    0.168  0.297509  0.297897 -0.0108687  -118.179    -8.722  
-22 914 59836.00 I  0.296978 0.000025  0.295782 0.000050  I-0.0109851 0.0000078  0.0167 0.0061  I  -118.400    0.902    -8.680    0.136  0.296992  0.295809 -0.0110048  -118.515    -8.694  
-22 915 59837.00 I  0.296334 0.000024  0.293800 0.000049  I-0.0108942 0.0000078 -0.2364 0.0055  I  -118.755    0.902    -8.730    0.136  0.296326  0.293853 -0.0109071  -118.881    -8.735  
-22 916 59838.00 I  0.295607 0.000024  0.291752 0.000049  I-0.0105227 0.0000077 -0.4581 0.0058  I  -118.926    0.902    -8.848    0.136  0.295633  0.291666 -0.0105453  -119.064    -8.840  
-22 917 59839.00 I  0.294743 0.000016  0.289580 0.000042  I-0.0099860 0.0000087 -0.6558 0.0056  I  -118.849    0.928    -8.900    0.088  0.294765  0.289613 -0.0099966  -118.954    -8.905  
-22 918 59840.00 I  0.293576 0.000020  0.287798 0.000055  I-0.0092293 0.0000081 -0.7989 0.0059  I  -118.591    0.988    -8.822    0.130  0.293594  0.287789 -0.0092502  -118.640    -8.844  
-22 919 59841.00 I  0.292287 0.000020  0.285829 0.000054  I-0.0084301 0.0000079 -0.8164 0.0059  I  -118.236    0.988    -8.710    0.130  0.292235  0.285928 -0.0084134  -118.223    -8.750  
-22 920 59842.00 I  0.291352 0.000019  0.283571 0.000037  I-0.0075718 0.0000086 -0.9080 0.0051  I  -117.863    1.078    -8.710    0.170  0.291284  0.283515 -0.0075559  -117.778    -8.771  
-22 921 59843.00 I  0.290656 0.000020  0.281026 0.000039  I-0.0066711 0.0000064 -0.8287 0.0052  I  -117.562    0.957    -8.833    0.126  0.290675  0.281089 -0.0066950  -117.531    -8.864  
-22 922 59844.00 I  0.289762 0.000020  0.278372 0.000039  I-0.0059631 0.0000060 -0.6031 0.0046  I  -117.391    0.957    -8.934    0.126  0.289785  0.278400 -0.0059969  -117.441    -8.921  
-22 923 59845.00 I  0.288622 0.000019  0.275574 0.000039  I-0.0054438 0.0000065 -0.4406 0.0046  I  -117.332    0.957    -8.873    0.126  0.288673  0.275532 -0.0054471  -117.457    -8.810  
-22 924 59846.00 I  0.287260 0.000015  0.272925 0.000016  I-0.0050914 0.0000070 -0.2497 0.0048  I  -117.327    0.805    -8.661    0.027  0.287244  0.272949 -0.0051006  -117.468    -8.622  
-22 925 59847.00 I  0.285952 0.000026  0.270438 0.000036  I-0.0049406 0.0000070 -0.0703 0.0050  I  -117.350    0.769    -8.450    0.192  0.285878  0.270404 -0.0049635  -117.484    -8.457  
-22 926 59848.00 I  0.285169 0.000027  0.268145 0.000036  I-0.0049415 0.0000071  0.0811 0.0056  I  -117.407    0.769    -8.388    0.192  0.285103  0.268121 -0.0049793  -117.537    -8.441  
-22 927 59849.00 I  0.284703 0.000026  0.266489 0.000033  I-0.0050959 0.0000087  0.2118 0.0053  I  -117.484    0.744    -8.489    0.260  0.284746  0.266357 -0.0051012  -117.616    -8.597  
-22 928 59850.00 I  0.283878 0.000027  0.264895 0.000034  I-0.0053043 0.0000078  0.1603 0.0057  I  -117.553    0.670    -8.634    0.185  0.283878  0.264953 -0.0053014  -117.693    -8.702  
-22 929 59851.00 I  0.283010 0.000026  0.263310 0.000034  I-0.0053848 0.0000073  0.0139 0.0053  I  -117.615    0.670    -8.699    0.185  0.282943  0.263319 -0.0054180  -117.779    -8.707  
-22 930 59852.00 I  0.282320 0.000026  0.261522 0.000034  I-0.0053241 0.0000071 -0.1563 0.0050  I  -117.695    0.670    -8.656    0.185  0.282338  0.261528 -0.0053388  -117.905    -8.603  
-2210 1 59853.00 I  0.281361 0.000014  0.259739 0.000015  I-0.0050435 0.0000068 -0.4125 0.0049  I  -117.761    0.566    -8.581    0.031  0.281388  0.259744 -0.0049041  -117.934    -8.536  
-2210 2 59854.00 I  0.280044 0.000011  0.257886 0.000015  I-0.0045471 0.0000068 -0.5246 0.0043  I  -117.683    0.566    -8.557    0.031  0.280092  0.257931 -0.0043864  -117.763    -8.633  
-2210 3 59855.00 I  0.278450 0.000014  0.255735 0.000018  I-0.0040459 0.0000052 -0.4821 0.0045  I  -117.340    0.916    -8.591    0.134  0.278478  0.255746 -0.0040146  -117.380    -8.681  
-2210 4 59856.00 I  0.276546 0.000013  0.253512 0.000016  I-0.0035885 0.0000060 -0.4230 0.0034  I  -116.766    1.103    -8.598    0.179  0.276607  0.253527 -0.0035590  -116.777    -8.672  
-2210 5 59857.00 I  0.274389 0.000014  0.251451 0.000023  I-0.0032265 0.0000044 -0.2841 0.0039  I  -116.189    1.082    -8.485    0.156  0.274352  0.251450 -0.0032281  -116.158    -8.550  
-2210 6 59858.00 I  0.272447 0.000020  0.249211 0.000023  I-0.0030606 0.0000049 -0.0243 0.0035  I  -115.869    1.082    -8.248    0.156  0.272409  0.249284 -0.0030816  -115.892    -8.306  
-2210 7 59859.00 I  0.270891 0.000023  0.246757 0.000021  I-0.0031812 0.0000054  0.2453 0.0037  I  -115.880    1.082    -7.992    0.156  0.270869  0.246728 -0.0031810  -115.963    -8.047  
-2210 8 59860.00 I  0.269388 0.000023  0.244263 0.000021  I-0.0035327 0.0000055  0.4594 0.0043  I  -116.058    1.082    -7.833    0.156  0.269464  0.244272 -0.0035337  -116.181    -7.889  
-2210 9 59861.00 I  0.267405 0.000021  0.242155 0.000019  I-0.0040712 0.0000066  0.5870 0.0039  I  -116.178    1.063    -7.794    0.132  0.267436  0.242181 -0.0040628  -116.323    -7.852  
-221010 59862.00 I  0.265329 0.000023  0.239990 0.000020  I-0.0046600 0.0000054  0.5744 0.0047  I  -116.171    0.936    -7.812    0.107  0.265240  0.239987 -0.0046541  -116.330    -7.871  
-221011 59863.00 I  0.263669 0.000023  0.237864 0.000012  I-0.0051765 0.0000068  0.4314 0.0040  I  -116.170    0.775    -7.839    0.072  0.263701  0.237885 -0.0051692  -116.344    -7.899  
-221012 59864.00 I  0.262027 0.000024  0.235760 0.000013  I-0.0054966 0.0000060  0.2098 0.0046  I  -116.318    0.830    -7.892    0.053  0.262046  0.235701 -0.0055011  -116.517    -7.950  
-221013 59865.00 I  0.259878 0.000021  0.233760 0.000013  I-0.0055874 0.0000062 -0.0378 0.0044  I  -116.576    0.830    -7.987    0.053  0.260021  0.233734 -0.0055722  -116.707    -8.023  
-221014 59866.00 I  0.256985 0.000021  0.232115 0.000012  I-0.0054402 0.0000064 -0.2277 0.0045  I  -116.744    0.830    -8.074    0.053  0.256936  0.232102 -0.0054362  -116.793    -8.078  
-221015 59867.00 I  0.254060 0.000021  0.230353 0.000012  I-0.0051764 0.0000064 -0.2843 0.0044  I  -116.640    0.830    -8.073    0.053  0.254063  0.230356 -0.0051876  -116.700    -8.075  
-221016 59868.00 I  0.251189 0.000023  0.228848 0.000026  I-0.0048937 0.0000059 -0.2745 0.0043  I  -116.254    0.992    -7.982    0.107  0.251206  0.228893 -0.0049099  -116.365    -7.987  
-221017 59869.00 I  0.248067 0.000027  0.227220 0.000026  I-0.0046575 0.0000058 -0.1745 0.0043  I  -115.723    0.992    -7.905    0.107  0.248052  0.227286 -0.0046783  -115.804    -7.935  
-221018 59870.00 I  0.245191 0.000023  0.225178 0.000026  I-0.0045589 0.0000062 -0.0319 0.0043  I  -115.196    1.044    -7.948    0.141  0.245102  0.225158 -0.0045660  -115.200    -8.015  
-221019 59871.00 I  0.243014 0.000025  0.222922 0.000031  I-0.0045885 0.0000063  0.0950 0.0044  I  -114.756    1.067    -8.090    0.163  0.243041  0.222898 -0.0045814  -114.747    -8.164  
-221020 59872.00 I  0.240702 0.000026  0.221149 0.000031  I-0.0047677 0.0000062  0.2783 0.0043  I  -114.463    1.067    -8.188    0.163  0.240817  0.221191 -0.0047645  -114.446    -8.265  
-221021 59873.00 I  0.237717 0.000026  0.219354 0.000031  I-0.0051492 0.0000060  0.4738 0.0056  I  -114.387    1.067    -8.113    0.163  0.237688  0.219313 -0.0051434  -114.344    -8.197  
-221022 59874.00 I  0.234654 0.000024  0.217514 0.000021  I-0.0057166 0.0000094  0.6733 0.0049  I  -114.551    1.094    -7.857    0.192  0.234606  0.217522 -0.0057243  -114.532    -7.927  
-221023 59875.00 I  0.232021 0.000022  0.216039 0.000025  I-0.0065032 0.0000077  0.8952 0.0061  I  -114.851    0.932    -7.539    0.157  0.231878  0.216031 -0.0064986  -114.866    -7.589  
-221024 59876.00 I  0.230032 0.000023  0.214634 0.000024  I-0.0074609 0.0000078  0.9788 0.0057  I  -115.114    0.932    -7.308    0.157  0.230043  0.214645 -0.0074339  -115.163    -7.341  
-221025 59877.00 I  0.228132 0.000022  0.213262 0.000024  I-0.0084069 0.0000083  0.9008 0.0057  I  -115.232    0.802    -7.250    0.112  0.228137  0.213232 -0.0084121  -115.318    -7.265  
-221026 59878.00 I  0.226079 0.000022  0.211739 0.000024  I-0.0092399 0.0000083  0.7551 0.0059  I  -115.223    0.802    -7.357    0.112  0.226115  0.211747 -0.0092591  -115.297    -7.349  
-221027 59879.00 I  0.223692 0.000022  0.210429 0.000024  I-0.0098811 0.0000083  0.5013 0.0055  I  -115.166    0.802    -7.529    0.112  0.223756  0.210409 -0.0098856  -115.222    -7.492  
-221028 59880.00 I  0.220829 0.000020  0.208832 0.000024  I-0.0102285 0.0000073  0.2056 0.0064  I  -115.091    0.802    -7.644    0.112  0.220823  0.208832 -0.0102779  -115.143    -7.612  
-221029 59881.00 I  0.217712 0.000017  0.207411 0.000018  I-0.0103282 0.0000098  0.0175 0.0052  I  -114.966    0.844    -7.645    0.085  0.217709  0.207418 -0.0103958  -115.022    -7.628  
-221030 59882.00 I  0.214510 0.000027  0.206266 0.000022  I-0.0102931 0.0000073 -0.0818 0.0059  I  -114.747    0.857    -7.576    0.184  0.214473  0.206229 -0.0103095  -114.810    -7.575  
-221031 59883.00 I  0.211393 0.000025  0.205209 0.000014  I-0.0101980 0.0000064 -0.0809 0.0048  I  -114.423    0.864    -7.520    0.228  0.211345  0.205237 -0.0101927  -114.492    -7.538  
-2211 1 59884.00 I  0.208605 0.000025  0.204256 0.000017  I-0.0101866 0.0000063  0.0861 0.0040  I  -114.032    0.864    -7.499    0.228  0.208514  0.204211 -0.0101774  -114.100    -7.544  
-2211 2 59885.00 I  0.206229 0.000027  0.203467 0.000020  I-0.0104078 0.0000049  0.3660 0.0041  I  -113.653    0.879    -7.465    0.197  0.206235  0.203545 -0.0104065  -113.700    -7.501  
-2211 3 59886.00 I  0.203875 0.000028  0.202376 0.000020  I-0.0109405 0.0000051  0.7115 0.0035  I  -113.383    0.879    -7.373    0.197  0.203841  0.202359 -0.0109528  -113.392    -7.399  
-2211 4 59887.00 I  0.201539 0.000028  0.201382 0.000020  I-0.0118030 0.0000051  0.9735 0.0043  I  -113.296    0.879    -7.225    0.197  0.201477  0.201353 -0.0118134  -113.257    -7.249  
-2211 5 59888.00 I  0.199499 0.000017  0.200682 0.000016  I-0.0128131 0.0000069  1.0121 0.0033  I  -113.387    0.896    -7.046    0.154  0.199403  0.200700 -0.0128173  -113.353    -7.066  
-2211 6 59889.00 I  0.197923 0.000020  0.199804 0.000022  I-0.0138021 0.0000043  0.9754 0.0043  I  -113.552    0.734    -6.854    0.095  0.197880  0.199789 -0.0138349  -113.543    -6.869  
-2211 7 59890.00 I  0.196414 0.000020  0.198994 0.000020  I-0.0147303 0.0000051  0.8381 0.0035  I  -113.643    0.734    -6.680    0.095  0.196436  0.198985 -0.0147274  -113.659    -6.688  
-2211 8 59891.00 I  0.194598 0.000023  0.198426 0.000021  I-0.0154435 0.0000056  0.5965 0.0036  I  -113.611    0.653    -6.588    0.027  0.194574  0.198424 -0.0154466  -113.660    -6.582  
-2211 9 59892.00 I  0.192635 0.000022  0.197567 0.000021  I-0.0159442 0.0000052  0.4177 0.0038  I  -113.552    0.653    -6.634    0.027  0.192696  0.197558 -0.0159684  -113.571    -6.657  
-221110 59893.00 I  0.190355 0.000021  0.196692 0.000020  I-0.0162462 0.0000050  0.1409 0.0034  I  -113.579    0.653    -6.795    0.027  0.190367  0.196722 -0.0162302  -113.564    -6.849  
-221111 59894.00 I  0.187844 0.000021  0.195904 0.000020  I-0.0162285 0.0000043 -0.1283 0.0063  I  -113.650    0.653    -6.952    0.027  0.187822  0.195880 -0.0162520  -113.631    -7.013  
-221112 59895.00 I  0.185418 0.000019  0.195028 0.000014  I-0.0160436 0.0000116 -0.2353 0.0038  I  -113.600    0.322    -6.999    0.160  0.185361  0.195076 -0.0160839  -113.596    -7.056  
-221113 59896.00 I  0.183322 0.000020  0.193966 0.000018  I-0.0157760 0.0000062 -0.2879 0.0064  I  -113.336    0.729    -6.952    0.092  0.183217  0.193981 -0.0158151  -113.352    -6.999  
-221114 59897.00 I  0.181909 0.000014  0.192824 0.000014  I-0.0155066 0.0000054 -0.2241 0.0042  I  -112.926    0.729    -6.925    0.092  0.181786  0.192794 -0.0155444  -112.967    -6.958  
-221115 59898.00 I  0.181148 0.000015  0.192265 0.000014  I-0.0153471 0.0000058 -0.1025 0.0035  I  -112.487    0.729    -6.989    0.092  0.181089  0.192167 -0.0153549  -112.549    -7.008  
-221116 59899.00 I  0.180591 0.000016  0.192098 0.000022  I-0.0153092 0.0000046  0.0418 0.0038  I  -112.061    0.766    -7.081    0.132  0.180613  0.192084 -0.0153236  -112.120    -7.099  
-221117 59900.00 I  0.179828 0.000016  0.192243 0.000022  I-0.0154607 0.0000048  0.2760 0.0033  I  -111.695    0.766    -7.070    0.132  0.179894  0.192217 -0.0154871  -111.735    -7.093  
-221118 59901.00 I  0.178492 0.000016  0.192671 0.000023  I-0.0158540 0.0000048  0.4887 0.0038  I  -111.548    0.766    -6.903    0.132  0.178587  0.192658 -0.0158559  -111.559    -6.936  
-221119 59902.00 I  0.176651 0.000013  0.192916 0.000020  I-0.0164102 0.0000059  0.6179 0.0031  I  -111.769    0.806    -6.646    0.164  0.176631  0.192939 -0.0164100  -111.782    -6.671  
-221120 59903.00 I  0.174675 0.000015  0.192889 0.000023  I-0.0170987 0.0000039  0.7740 0.0035  I  -112.260    0.734    -6.384    0.155  0.174678  0.192941 -0.0171134  -112.283    -6.399  
-221121 59904.00 I  0.172506 0.000015  0.192678 0.000023  I-0.0179195 0.0000037  0.8141 0.0029  I  -112.717    0.734    -6.153    0.155  0.172482  0.192686 -0.0178985  -112.747    -6.164  
-221122 59905.00 I  0.170164 0.000015  0.192549 0.000017  I-0.0186682 0.0000043  0.6782 0.0026  I  -112.941    0.691    -5.989    0.148  0.170135  0.192562 -0.0186627  -112.985    -5.999  
-221123 59906.00 I  0.167915 0.000022  0.192100 0.000034  I-0.0192690 0.0000036  0.5216 0.0029  I  -112.977    0.713    -5.979    0.144  0.167864  0.192125 -0.0192839  -113.015    -5.992  
-221124 59907.00 I  0.165798 0.000022  0.191636 0.000033  I-0.0196789 0.0000038  0.2676 0.0028  I  -112.924    0.713    -6.160    0.144  0.165815  0.191634 -0.0196773  -112.960    -6.178  
-221125 59908.00 I  0.163382 0.000022  0.191462 0.000033  I-0.0198049 0.0000042  0.0159 0.0036  I  -112.761    0.713    -6.396    0.144  0.163449  0.191394 -0.0198119  -112.800    -6.422  
-221126 59909.00 I  0.160410 0.000021  0.191095 0.000032  I-0.0197336 0.0000061 -0.1669 0.0037  I  -112.468    0.747    -6.480    0.137  0.160439  0.191188 -0.0197408  -112.502    -6.504  
-221127 59910.00 I  0.156935 0.000021  0.190791 0.000032  I-0.0195085 0.0000062 -0.2376 0.0038  I  -112.154    0.747    -6.372    0.137  0.156985  0.190819 -0.0195486  -112.173    -6.392  
-221128 59911.00 I  0.153236 0.000022  0.190266 0.000036  I-0.0193092 0.0000046 -0.1561 0.0042  I  -111.937    0.807    -6.232    0.109  0.153168  0.190278 -0.0193141  -111.939    -6.246  
-221129 59912.00 I  0.149943 0.000016  0.189774 0.000019  I-0.0192199 0.0000057 -0.0038 0.0029  I  -111.810    0.875    -6.195    0.071  0.149881  0.189736 -0.0192085  -111.789    -6.198  
-221130 59913.00 I  0.147020 0.000022  0.189883 0.000024  I-0.0193118 0.0000034  0.1791 0.0032  I  -111.698    0.786    -6.216    0.110  0.146998  0.189837 -0.0193120  -111.648    -6.204  
-2212 1 59914.00 I  0.144055 0.000026  0.190055 0.000024  I-0.0195847 0.0000028  0.3817 0.0023  I  -111.587    0.786    -6.183    0.110  0.144039  0.190129 -0.0196037  -111.563    -6.191  
-2212 2 59915.00 I  0.141127 0.000026  0.189992 0.000023  I-0.0200268 0.0000031  0.4390 0.0020  I  -111.525    0.786    -6.068    0.110  0.141086  0.190030 -0.0200182  -111.557    -6.103  
-2212 3 59916.00 I  0.138499 0.000026  0.189606 0.000024  I-0.0204296 0.0000028  0.3969 0.0022  I  -111.557    0.786    -5.913    0.110  0.138520  0.189588 -0.0204483  -111.593    -5.954  
-2212 4 59917.00 I  0.135669 0.000027  0.189556 0.000018  I-0.0208098 0.0000031  0.3224 0.0022  I  -111.667    0.838    -5.748    0.138  0.135739  0.189603 -0.0208072  -111.696    -5.787  
-2212 5 59918.00 I  0.132722 0.000028  0.189090 0.000019  I-0.0210334 0.0000034  0.1249 0.0030  I  -111.745    0.838    -5.586    0.138  0.132595  0.189132 -0.0210271  -111.763    -5.625  
-2212 6 59919.00 I  0.130239 0.000026  0.188818 0.000012  I-0.0210510 0.0000051 -0.0983 0.0031  I  -111.681    0.992    -5.486    0.145  0.130234  0.188807 -0.0210546  -111.664    -5.528  
-2212 7 59920.00 I  0.127863 0.000025  0.188835 0.000018  I-0.0208444 0.0000053 -0.2985 0.0037  I  -111.508    0.845    -5.540    0.121  0.127804  0.188914 -0.0208636  -111.530    -5.568  
-2212 8 59921.00 I  0.125543 0.000024  0.188701 0.000019  I-0.0204736 0.0000054 -0.4397 0.0039  I  -111.370    0.845    -5.757    0.121  0.125550  0.188683 -0.0204842  -111.431    -5.765  
-2212 9 59922.00 I  0.123009 0.000023  0.188933 0.000018  I-0.0199682 0.0000057 -0.5711 0.0046  I  -111.348    0.845    -6.014    0.121  0.123051  0.188943 -0.0199575  -111.450    -5.997  
-221210 59923.00 I  0.120044 0.000021  0.189230 0.000016  I-0.0193447 0.0000074 -0.6624 0.0040  I  -111.358    0.678    -6.157    0.089  0.120023  0.189212 -0.0193465  -111.433    -6.148  
-221211 59924.00 I  0.117119 0.000025  0.189450 0.000025  I-0.0186819 0.0000056 -0.6381 0.0047  I  -111.267    0.747    -6.160    0.165  0.117059  0.189519 -0.0187186  -111.306    -6.171  
-221212 59925.00 I  0.114541 0.000023  0.189307 0.000025  I-0.0181000 0.0000057 -0.5193 0.0036  I  -111.038    0.747    -6.136    0.165  0.114474  0.189311 -0.0181257  -111.063    -6.164  
-221213 59926.00 I  0.112254 0.000020  0.189450 0.000024  I-0.0176363 0.0000045 -0.4216 0.0036  I  -110.705    0.858    -6.167    0.199  0.112235  0.189380 -0.0176371  -110.733    -6.213  
-221214 59927.00 I  0.110085 0.000020  0.189742 0.000023  I-0.0172739 0.0000043 -0.2728 0.0030  I  -110.291    0.858    -6.187    0.199  0.110057  0.189733 -0.0172887  -110.324    -6.215  
-221215 59928.00 I  0.107803 0.000020  0.190654 0.000023  I-0.0170975 0.0000039 -0.1036 0.0029  I  -109.856    0.858    -6.078    0.199  0.107848  0.190644 -0.0170929  -109.882    -6.084  
-221216 59929.00 I  0.105273 0.000020  0.191574 0.000023  I-0.0170761 0.0000038  0.0938 0.0032  I  -109.605    0.858    -5.851    0.199  0.105276  0.191662 -0.0170407  -109.642    -5.845  
-221217 59930.00 I  0.102628 0.000012  0.192141 0.000014  I-0.0172735 0.0000050  0.2563 0.0027  I  -109.763    0.905    -5.653    0.186  0.102588  0.192217 -0.0171383  -109.796    -5.644  
-221218 59931.00 I  0.100235 0.000024  0.192465 0.000018  I-0.0175362 0.0000037  0.2614 0.0035  I  -110.279    0.895    -5.567    0.171  0.100160  0.192490 -0.0173664  -110.291    -5.561  
-221219 59932.00 I  0.098288 0.000024  0.192763 0.000015  I-0.0177795 0.0000049  0.2161 0.0024  I  -110.844    0.780    -5.497    0.086  0.098210  0.192803 -0.0177187  -110.824    -5.496  
-221220 59933.00 I  0.096787 0.000029  0.193103 0.000020  I-0.0179622 0.0000032  0.1522 0.0030  I  -111.271    0.588    -5.339    0.101  0.096711  0.193084 -0.0179634  -111.212    -5.340  
-221221 59934.00 I  0.095783 0.000029  0.193352 0.000021  I-0.0180817 0.0000034  0.0819 0.0023  I  -111.654    0.588    -5.212    0.101  0.095777  0.193348 -0.0181234  -111.654    -5.239  
-221222 59935.00 I  0.094823 0.000030  0.194047 0.000021  I-0.0180950 0.0000034 -0.0812 0.0024  I  -112.014    0.588    -5.340    0.101  0.094877  0.193950 -0.0181060  -112.105    -5.394  
-221223 59936.00 I  0.093412 0.000032  0.194930 0.000021  I-0.0179100 0.0000035 -0.2721 0.0024  I  -112.083    0.588    -5.687    0.101  0.093472  0.194922 -0.0178955  -112.150    -5.759  
-221224 59937.00 I  0.091298 0.000025  0.196104 0.000019  I-0.0176012 0.0000035 -0.3118 0.0025  I  -111.698    0.565    -5.926    0.105  0.091397  0.196126 -0.0175841  -111.706    -6.007  
-221225 59938.00 I  0.088381 0.000025  0.197004 0.000018  I-0.0173337 0.0000036 -0.2097 0.0047  I  -111.131    0.565    -5.854    0.105  0.088402  0.197099 -0.0173115  -111.094    -5.943  
-221226 59939.00 I  0.085233 0.000035  0.197365 0.000017  I-0.0172360 0.0000087  0.0551 0.0043  I  -110.785    0.782    -5.648    0.151  0.085204  0.197391 -0.0172323  -110.709    -5.742  
-221227 59940.00 I  0.081986 0.000035  0.197783 0.000016  I-0.0174611 0.0000079  0.3716 0.0051  I  -110.731    0.782    -5.561    0.151  0.082060  0.197809 -0.0174541  -110.623    -5.660  
-221228 59941.00 I  0.078291 0.000036  0.198348 0.000018  I-0.0179218 0.0000053  0.5157 0.0048  I  -110.788    0.802    -5.568    0.131  0.078253  0.198379 -0.0179243  -110.647    -5.673  
-221229 59942.00 I  0.074740 0.000034  0.198594 0.000018  I-0.0184551 0.0000055  0.5474 0.0039  I  -110.857    0.802    -5.482    0.131  0.074744  0.198584 -0.0184719  -110.694    -5.570  
-221230 59943.00 I  0.071196 0.000034  0.199187 0.000016  I-0.0189988 0.0000058  0.5256 0.0043  I  -110.977    0.802    -5.274    0.131  0.071281  0.199199 -0.0190102  -110.793    -5.341  
-221231 59944.00 I  0.067040 0.000034  0.200092 0.000017  I-0.0194831 0.0000067  0.4343 0.0054  I  -111.159    0.802    -5.099    0.131  0.067074  0.200103 -0.0194855  -110.973    -5.182  
-23 1 1 59945.00 I  0.062788 0.000015  0.200914 0.000013  I-0.0198267 0.0000091  0.2210 0.0047  I  -111.344    0.822    -5.052    0.108  0.062699  0.200944 -0.0197967  -111.162    -5.163  
-23 1 2 59946.00 I  0.059053 0.000022  0.201759 0.000019  I-0.0199220 0.0000067 -0.0016 0.0061  I  -111.453    0.606    -5.072    0.061                                                     
-23 1 3 59947.00 I  0.055737 0.000026  0.202457 0.000020  I-0.0198307 0.0000082 -0.2028 0.0056  I  -111.405    0.662    -5.097    0.124                                                     
-23 1 4 59948.00 I  0.052976 0.000026  0.203035 0.000021  I-0.0195087 0.0000089 -0.4273 0.0065  I  -111.171    0.662    -5.180    0.124                                                     
-23 1 5 59949.00 I  0.050801 0.000026  0.203876 0.000021  I-0.0190214 0.0000102 -0.5159 0.0067  I  -110.844    0.662    -5.395    0.124                                                     
-23 1 6 59950.00 I  0.048796 0.000026  0.205073 0.000022  I-0.0184971 0.0000101 -0.5438 0.0071  I  -110.593    0.662    -5.674    0.124                                                     
-23 1 7 59951.00 I  0.046883 0.000025  0.206240 0.000022  I-0.0179489 0.0000099 -0.5265 0.0077  I  -110.480    0.662    -5.846    0.124                                                     
-23 1 8 59952.00 I  0.045143 0.000023  0.207582 0.000023  I-0.0174779 0.0000117 -0.4077 0.0084  I  -110.414    0.919    -5.830    0.206                                                     
-23 1 9 59953.00 I  0.043364 0.000017  0.209046 0.000020  I-0.0171416 0.0000135 -0.2646 0.0084  I  -110.273    0.952    -5.720    0.173                                                     
-23 110 59954.00 I  0.041294 0.000016  0.210280 0.000019  I-0.0169604 0.0000121 -0.0866 0.0078  I  -110.013    0.952    -5.645    0.173                                                     
-23 111 59955.00 I  0.038966 0.000023  0.211092 0.000021  I-0.0169678 0.0000077  0.0895 0.0067  I  -109.664    0.813    -5.602    0.121                                                     
-23 112 59956.00 I  0.036562 0.000022  0.211936 0.000020  I-0.0170932 0.0000059  0.1270 0.0051  I  -109.305    0.813    -5.496    0.121                                                     
-23 113 59957.00 I  0.034181 0.000022  0.213063 0.000020  I-0.0172126 0.0000068  0.1368 0.0057  I  -109.087    0.813    -5.331    0.121                                                     
-23 114 59958.00 I  0.031794 0.000017  0.214410 0.000014  I-0.0173720 0.0000097  0.1620 0.0052  I  -109.176    0.749    -5.255    0.079                                                     
-23 115 59959.00 I  0.029348 0.000025  0.216080 0.000026  I-0.0175356 0.0000079  0.1840 0.0064  I  -109.546    0.723    -5.362    0.086                                                     
-23 116 59960.00 I  0.026874 0.000025  0.217946 0.000026  I-0.0177144 0.0000083  0.1291 0.0067  I  -109.971    0.723    -5.514    0.086                                                     
-23 117 59961.00 I  0.024323 0.000019  0.220275 0.000024  I-0.0177450 0.0000109 -0.0722 0.0061  I  -110.349    0.709    -5.502    0.090                                                     
-23 118 59962.00 I  0.021690 0.000025  0.222425 0.000023  I-0.0175718 0.0000089 -0.2680 0.0069  I  -110.858    0.729    -5.380    0.093                                                     
-23 119 59963.00 I  0.019116 0.000025  0.224220 0.000023  I-0.0172285 0.0000085 -0.4054 0.0060  I  -111.543    0.729    -5.453    0.093                                                     
-23 120 59964.00 I  0.016671 0.000026  0.225637 0.000023  I-0.0167608 0.0000081 -0.5435 0.0075  I  -111.987    0.729    -5.826    0.093                                                     
-23 121 59965.00 I  0.013977 0.000019  0.226846 0.000008  I-0.0161653 0.0000124 -0.6102 0.0048  I  -111.759    0.838    -6.186    0.103                                                     
-23 122 59966.00 I  0.010875 0.000024  0.227750 0.000011  I-0.0156075 0.0000052 -0.4758 0.0066  I  -111.034    0.503    -6.199    0.086                                                     
-23 123 59967.00 I  0.007812 0.000024  0.228852 0.000013  I-0.0152582 0.0000046 -0.2080 0.0037  I  -110.392    0.503    -5.961    0.086                                                     
-23 124 59968.00 I  0.005408 0.000024  0.230236 0.000015  I-0.0152019 0.0000053  0.0911 0.0031  I  -110.130    0.434    -5.803    0.081                                                     
-23 125 59969.00 I  0.003920 0.000029  0.231445 0.000018  I-0.0154044 0.0000043  0.2822 0.0034  I  -110.123    0.571    -5.802    0.157                                                     
-23 126 59970.00 I  0.002885 0.000030  0.233320 0.000021  I-0.0156952 0.0000043  0.2600 0.0030  I  -110.234    0.571    -5.755    0.157                                                     
-23 127 59971.00 I  0.001578 0.000029  0.235886 0.000022  I-0.0158972 0.0000042  0.1561 0.0036  I  -110.455    0.571    -5.591    0.157                                                     
-23 128 59972.00 I  0.000384 0.000026  0.238109 0.000021  I-0.0159850 0.0000057 -0.0149 0.0034  I  -110.717    0.721    -5.501    0.206                                                     
-23 129 59973.00 I -0.000274 0.000028  0.240386 0.000023  I-0.0158764 0.0000053 -0.1588 0.0036  I  -110.881    0.789    -5.640    0.198                                                     
-23 130 59974.00 I -0.000858 0.000026  0.242660 0.000023  I-0.0156646 0.0000045 -0.3112 0.0056  I  -110.901    0.789    -5.901    0.198                                                     
-23 131 59975.00 I -0.001404 0.000021  0.245010 0.000021  I-0.0152267 0.0000098 -0.5456 0.0043  I  -110.812    1.162    -6.086    0.156                                                     
-23 2 1 59976.00 I -0.002310 0.000021  0.247819 0.000019  I-0.0146084 0.0000073 -0.6751 0.0061  I  -110.606    1.127    -6.164    0.178                                                     
-23 2 2 59977.00 I -0.003559 0.000021  0.250309 0.000019  I-0.0138927 0.0000073 -0.7560 0.0052  I  -110.288    1.127    -6.254    0.178                                                     
-23 2 3 59978.00 I -0.004906 0.000022  0.252500 0.000020  I-0.0131186 0.0000074 -0.7703 0.0056  I  -109.970    1.127    -6.407    0.178                                                     
-23 2 4 59979.00 I -0.006474 0.000025  0.254275 0.000021  I-0.0124004 0.0000084 -0.6398 0.0046  I  -109.793    1.093    -6.511    0.198                                                     
-23 2 5 59980.00 I -0.008192 0.000029  0.255941 0.000024  I-0.0118612 0.0000055 -0.4427 0.0050  I  -109.753    0.891    -6.442    0.169                                                     
-23 2 6 59981.00 I -0.009971 0.000037  0.257724 0.000027  I-0.0114989 0.0000055 -0.2937 0.0040  I  -109.709    0.891    -6.241    0.169                                                     
-23 2 7 59982.00 I -0.011949 0.000041  0.259674 0.000028  I-0.0112739 0.0000059 -0.1443 0.0037  I  -109.558    0.704    -6.062    0.141                                                     
-23 2 8 59983.00 I -0.014045 0.000053  0.261632 0.000032  I-0.0112027 0.0000050 -0.0178 0.0037  P  -109.373    0.278    -5.986    0.145                                                     
-23 2 9 59984.00 I -0.015660 0.000053  0.263467 0.000031  I-0.0112392 0.0000046  0.1113 0.0035  P  -109.262    0.288    -5.962    0.148                                                     
-23 210 59985.00 I -0.016707 0.000091  0.265558 0.000091  I-0.0114430 0.0000049  0.2935 0.0073  P  -109.300    0.297    -5.938    0.151                                                     
-23 211 59986.00 I -0.017877 0.000092  0.268000 0.000091  I-0.0117878 0.0000139  0.3604 0.0069  P  -109.502    0.304    -5.962    0.154                                                     
-23 212 59987.00 I -0.019627 0.000093  0.270440 0.000091  I-0.0121218 0.0000128  0.3013 0.0098  P  -109.807    0.309    -6.106    0.155                                                     
-23 213 59988.00 I -0.021927 0.000091  0.273090 0.000091  I-0.0123672 0.0000138  0.1726 0.0105  P  -110.081    0.313    -6.306    0.157                                                     
-23 214 59989.00 I -0.024451 0.000091  0.275689 0.000091  I-0.0124505 0.0000167 -0.0057 0.0111  P  -110.274    0.316    -6.404    0.158                                                     
-23 215 59990.00 I -0.026942 0.000091  0.278189 0.000091  I-0.0123503 0.0000173 -0.2005 0.0118  P  -110.527    0.318    -6.383    0.158                                                     
-23 216 59991.00 I -0.029363 0.000091  0.280693 0.000090  I-0.0120624 0.0000167 -0.3565 0.0125  P  -110.950    0.319    -6.442    0.159                                                     
-23 217 59992.00 I -0.031731 0.000092  0.282891 0.000091  I-0.0116805 0.0000181 -0.3831 0.0120  P  -111.317    0.320    -6.715    0.159                                                     
-23 218 59993.00 I -0.033941 0.000092  0.284861 0.000091  I-0.0113616 0.0000171 -0.2137 0.0132  P  -111.244    0.321    -7.015    0.160                                                     
-23 219 59994.00 I -0.035803 0.000092  0.286849 0.000091  I-0.0113008 0.0000192  0.0989 0.0117  P  -110.711    0.321    -7.047    0.160                                                     
-23 220 59995.00 I -0.037232 0.000092  0.288966 0.000091  I-0.0115652 0.0000159  0.4291 0.0120  P  -110.104    0.321    -6.821    0.160                                                     
-23 221 59996.00 I -0.038206 0.000092  0.291501 0.000091  I-0.0121471 0.0000144  0.7237 0.0103  P  -109.751    0.321    -6.620    0.160                                                     
-23 222 59997.00 I -0.038751 0.000092  0.294629 0.000091  I-0.0129182 0.0000130  0.7352 0.0093  P  -109.675    0.322    -6.590    0.160                                                     
-23 223 59998.00 I -0.038993 0.000091  0.298328 0.000091  I-0.0136878 0.0000118                 P  -109.809    0.322    -6.598    0.160                                                     
-23 224 59999.00 P -0.039465 0.000631  0.301892 0.000479  P-0.0144402 0.0001080                 P  -110.123    0.322    -6.544    0.160                                                     
-23 225 60000.00 P -0.039829 0.000937  0.305526 0.000790  P-0.0150402 0.0002041                 P  -110.491    0.322    -6.557    0.160                                                     
-23 226 60001.00 P -0.040219 0.001181  0.308927 0.001057  P-0.0154032 0.0003028                 P  -110.714    0.322    -6.779    0.160                                                     
-23 227 60002.00 P -0.040565 0.001392  0.312123 0.001300  P-0.0155193 0.0004021                 P  -110.729    0.322    -7.119    0.160                                                     
-23 228 60003.00 P -0.040825 0.001580  0.315144 0.001527  P-0.0154478 0.0005017                 P  -110.614    0.322    -7.348    0.160                                                     
-23 3 1 60004.00 P -0.040991 0.001753  0.318052 0.001741  P-0.0152673 0.0006014                 P  -110.389    0.322    -7.385    0.160                                                     
-23 3 2 60005.00 P -0.041085 0.001914  0.320919 0.001946  P-0.0150321 0.0007012                 P  -110.012    0.322    -7.360    0.160                                                     
-23 3 3 60006.00 P -0.041133 0.002066  0.323780 0.002142  P-0.0148077 0.0007500                 P  -109.551    0.322    -7.407    0.160                                                     
-23 3 4 60007.00 P -0.041147 0.002209  0.326642 0.002332  P-0.0146716 0.0005500                 P  -109.203    0.322    -7.484    0.160                                                     
-23 3 5 60008.00 P -0.041131 0.002346  0.329500 0.002515  P-0.0146751 0.0007548                 P  -109.077    0.322    -7.448    0.160                                                     
-23 3 6 60009.00 P -0.041086 0.002477  0.332354 0.002694  P-0.0148459 0.0009344                 P  -109.075    0.322    -7.258    0.160                                                     
-23 3 7 60010.00 P -0.041005 0.002603  0.335200 0.002868  P-0.0151963 0.0010994                 P  -109.039    0.322    -7.042    0.160                                                     
-23 3 8 60011.00 P -0.040881 0.002724  0.338038 0.003038  P-0.0156854 0.0012543                 P  -108.950    0.322    -6.948    0.160                                                     
-23 3 9 60012.00 P -0.040710 0.002842  0.340870 0.003205  P-0.0162924 0.0014016                 P  -108.907    0.322    -7.003    0.160                                                     
-23 310 60013.00 P -0.040489 0.002956  0.343697 0.003368  P-0.0169429 0.0015429                 P  -108.966    0.322    -7.127    0.160                                                     
-23 311 60014.00 P -0.040221 0.003067  0.346520 0.003528  P-0.0175567 0.0016792                 P  -109.085    0.322    -7.253    0.160                                                     
-23 312 60015.00 P -0.039904 0.003175  0.349340 0.003686  P-0.0180666 0.0018113                 P  -109.200    0.322    -7.376    0.160                                                     
-23 313 60016.00 P -0.039540 0.003280  0.352155 0.003841  P-0.0184074 0.0019399                 P  -109.271    0.322    -7.509    0.160                                                     
-23 314 60017.00 P -0.039130 0.003382  0.354964 0.003993  P-0.0185431 0.0020652                 P  -109.267    0.322    -7.636    0.160                                                     
-23 315 60018.00 P -0.038673 0.003483  0.357766 0.004143  P-0.0184836 0.0021877                 P  -109.176    0.322    -7.748    0.160                                                     
-23 316 60019.00 P -0.038170 0.003581  0.360561 0.004292  P-0.0183225 0.0023077                 P  -109.031    0.322    -7.883    0.160                                                     
-23 317 60020.00 P -0.037621 0.003677  0.363346 0.004438  P-0.0181858 0.0024255                 P  -108.858    0.322    -8.064    0.160                                                     
-23 318 60021.00 P -0.037026 0.003771  0.366123 0.004582  P-0.0182022 0.0025411                 P  -108.647    0.322    -8.199    0.160                                                     
-23 319 60022.00 P -0.036386 0.003864  0.368889 0.004725  P-0.0184832 0.0026548                 P  -108.421    0.322    -8.161    0.160                                                     
-23 320 60023.00 P -0.035699 0.003955  0.371646 0.004866  P-0.0190677 0.0027668                 P  -108.255    0.322    -7.973    0.160                                                     
-23 321 60024.00 P -0.034967 0.004044  0.374391 0.005005  P-0.0198946 0.0028772                 P  -108.186    0.322    -7.809    0.160                                                     
-23 322 60025.00 P -0.034190 0.004132  0.377124 0.005143  P-0.0208441 0.0029860                 P  -108.196    0.322    -7.783    0.160                                                     
-23 323 60026.00 P -0.033369 0.004219  0.379845 0.005279  P-0.0217602 0.0030934                 P  -108.296    0.322    -7.835    0.160                                                     
-23 324 60027.00 P -0.032503 0.004304  0.382553 0.005414  P-0.0225067 0.0031995                 P  -108.526    0.322    -7.881    0.160                                                     
-23 325 60028.00 P -0.031592 0.004388  0.385248 0.005548  P-0.0230107 0.0033043                 P  -108.822    0.322    -7.966    0.160                                                     
-23 326 60029.00 P -0.030637 0.004471  0.387927 0.005681  P-0.0232476 0.0034080                 P  -109.021    0.322    -8.166    0.160                                                     
-23 327 60030.00 P -0.029639 0.004553  0.390592 0.005812  P-0.0232477 0.0035105                 P  -109.032    0.322    -8.421    0.160                                                     
-23 328 60031.00 P -0.028597 0.004633  0.393241 0.005942  P-0.0230748 0.0036120                 P  -108.889    0.322    -8.576    0.160                                                     
-23 329 60032.00 P -0.027512 0.004713  0.395874 0.006071  P-0.0228218 0.0037124                 P  -108.617    0.322    -8.576    0.160                                                     
-23 330 60033.00 P -0.026385 0.004791  0.398490 0.006199  P-0.0225736 0.0038119                 P  -108.185    0.322    -8.538    0.160                                                     
-23 331 60034.00 P -0.025214 0.004869  0.401088 0.006326  P-0.0224015 0.0039105                 P  -107.646    0.322    -8.592    0.160                                                     
-23 4 1 60035.00 P -0.024002 0.004945  0.403668 0.006452  P-0.0223641 0.0040082                 P  -107.206    0.322    -8.718    0.160                                                     
-23 4 2 60036.00 P -0.022748 0.005021  0.406228 0.006578  P-0.0225034 0.0041051                 P  -107.050    0.322    -8.763    0.160                                                     
-23 4 3 60037.00 P -0.021452 0.005096  0.408770 0.006702  P-0.0228415 0.0042012                 P  -107.164    0.322    -8.629    0.160                                                     
-23 4 4 60038.00 P -0.020116 0.005170  0.411291 0.006825  P-0.0233721 0.0042965                 P  -107.370    0.322    -8.388    0.160                                                     
-23 4 5 60039.00 P -0.018739 0.005243  0.413791 0.006947  P-0.0240601 0.0043911                 P  -107.535    0.322    -8.212    0.160                                                     
-23 4 6 60040.00 P -0.017321 0.005316  0.416270 0.007069  P-0.0248410 0.0044849                 P  -107.658    0.322    -8.207    0.160                                                     
-23 4 7 60041.00 P -0.015864 0.005388  0.418727 0.007190  P-0.0256211 0.0045781                 P  -107.788    0.322    -8.343    0.160                                                     
-23 4 8 60042.00 P -0.014367 0.005459  0.421162 0.007310  P-0.0263050 0.0046706                 P  -107.926    0.322    -8.514    0.160                                                     
-23 4 9 60043.00 P -0.012831 0.005529  0.423573 0.007429  P-0.0268078 0.0047625                 P  -108.049    0.322    -8.652    0.160                                                     
-23 410 60044.00 P -0.011256 0.005599  0.425961 0.007547  P-0.0270841 0.0048537                 P  -108.130    0.322    -8.761    0.160                                                     
-23 411 60045.00 P -0.009644 0.005668  0.428324 0.007665  P-0.0271505 0.0049444                 P  -108.117    0.322    -8.884    0.160                                                     
-23 412 60046.00 P -0.007993 0.005736  0.430662 0.007782  P-0.0270752 0.0050344                 P  -107.917    0.322    -9.039    0.160                                                     
-23 413 60047.00 P -0.006306 0.005804  0.432975 0.007899  P-0.0269719 0.0051240                 P  -107.494    0.322    -9.199    0.160                                                     
-23 414 60048.00 P -0.004581 0.005871  0.435262 0.008014  P-0.0269686 0.0052129                 P  -106.962    0.322    -9.308    0.160                                                     
-23 415 60049.00 P -0.002821 0.005938  0.437523 0.008130  P-0.0271780 0.0053014                 P  -106.543    0.322    -9.311    0.160                                                     
-23 416 60050.00 P -0.001024 0.006004  0.439756 0.008244  P-0.0276595 0.0053893                 P  -106.406    0.322    -9.195    0.160                                                     
-23 417 60051.00 P  0.000808 0.006070  0.441962 0.008358  P-0.0284019 0.0054768                 P  -106.544    0.322    -9.015    0.160                                                     
-23 418 60052.00 P  0.002674 0.006135  0.444139 0.008471  P-0.0293191 0.0055637                 P  -106.800    0.322    -8.859    0.160                                                     
-23 419 60053.00 P  0.004575 0.006199  0.446288 0.008584  P-0.0302755 0.0056502                 P  -107.013    0.322    -8.779    0.160                                                     
-23 420 60054.00 P  0.006509 0.006263  0.448408 0.008696  P-0.0311265 0.0057362                 P  -107.144    0.322    -8.770    0.160                                                     
-23 421 60055.00 P  0.008477 0.006327  0.450497 0.008807  P-0.0317608 0.0058218                 P  -107.254    0.322    -8.813    0.160                                                     
-23 422 60056.00 P  0.010478 0.006390  0.452557 0.008918  P-0.0321237 0.0059070                 P  -107.392    0.322    -8.920    0.160                                                     
-23 423 60057.00 P  0.012510 0.006452  0.454586 0.009029  P-0.0322182 0.0059917                 P  -107.526    0.322    -9.089    0.160                                                     
-23 424 60058.00 P  0.014574 0.006514  0.456584 0.009139  P-0.0320950 0.0060760                 P  -107.588    0.322    -9.256    0.160                                                     
-23 425 60059.00 P  0.016670 0.006576  0.458551 0.009248  P-0.0318298 0.0061599                 P  -107.537    0.322    -9.341    0.160                                                     
-23 426 60060.00 P  0.018795 0.006637  0.460485 0.009357  P-0.0315070 0.0062434                 P  -107.353    0.322    -9.351    0.160                                                     
-23 427 60061.00 P  0.020951 0.006698  0.462387 0.009465  P-0.0312071 0.0063266                 P  -107.018    0.322    -9.389    0.160                                                     
-23 428 60062.00 P  0.023135 0.006758  0.464256 0.009573  P-0.0309993 0.0064093                 P  -106.567    0.322    -9.530    0.160                                                     
-23 429 60063.00 P  0.025349 0.006818  0.466091 0.009681  P-0.0309373 0.0064917                 P  -106.140    0.322    -9.719    0.160                                                     
-23 430 60064.00 P  0.027590 0.006878  0.467893 0.009788  P-0.0310527 0.0065737                 P  -105.934    0.322    -9.801    0.160                                                     
-23 5 1 60065.00 P  0.029859 0.006937  0.469660 0.009894  P-0.0313498 0.0066554                 P  -106.059    0.322    -9.680    0.160                                                     
-23 5 2 60066.00 P  0.032155 0.006996  0.471393 0.010001  P-0.0318057 0.0067368                 P  -106.436    0.322    -9.411    0.160                                                     
-23 5 3 60067.00 P  0.034477 0.007055  0.473091 0.010106  P-0.0323643 0.0068177                 P  -106.864    0.322    -9.145    0.160                                                     
-23 5 4 60068.00 P  0.036825 0.007113  0.474753 0.010211  P-0.0329427 0.0068984                 P  -107.185    0.322    -9.008    0.160                                                     
-23 5 5 60069.00 P  0.039198 0.007170  0.476379 0.010316  P-0.0334464 0.0069788                 P  -107.389    0.322    -9.030    0.160                                                     
-23 5 6 60070.00 P  0.041595 0.007228  0.477970 0.010421  P-0.0337847 0.0070588                 P  -107.568    0.322    -9.169    0.160                                                     
-23 5 7 60071.00 P  0.044015 0.007285  0.479524 0.010525  P-0.0338987 0.0071385                 P  -107.771    0.322    -9.367    0.160                                                     
-23 5 8 60072.00 P  0.046459 0.007341  0.481040 0.010628  P-0.0337838 0.0072179                 P  -107.920    0.322    -9.572    0.160                                                     
-23 5 9 60073.00 P  0.048925 0.007398  0.482520 0.010732  P-0.0334962 0.0072970                                                                                                             
-23 510 60074.00 P  0.051413 0.007454  0.483962 0.010834  P-0.0331443 0.0073758                                                                                                             
-23 511 60075.00 P  0.053922 0.007510  0.485367 0.010937  P-0.0328560 0.0074544                                                                                                             
-23 512 60076.00 P  0.056452 0.007565  0.486733 0.011039  P-0.0327393 0.0075326                                                                                                             
-23 513 60077.00 P  0.059001 0.007620  0.488060 0.011141  P-0.0328570 0.0076106                                                                                                             
-23 514 60078.00 P  0.061569 0.007675  0.489349 0.011242  P-0.0332114 0.0076883                                                                                                             
-23 515 60079.00 P  0.064155 0.007730  0.490599 0.011343  P-0.0337392 0.0077657                                                                                                             
-23 516 60080.00 P  0.066760 0.007784  0.491810 0.011444  P-0.0343274 0.0078428                                                                                                             
-23 517 60081.00 P  0.069381 0.007838  0.492981 0.011544  P-0.0348455 0.0079197                                                                                                             
-23 518 60082.00 P  0.072018 0.007892  0.494112 0.011644  P-0.0351786 0.0079964                                                                                                             
-23 519 60083.00 P  0.074671 0.007945  0.495203 0.011744  P-0.0352499 0.0080728                                                                                                             
-23 520 60084.00 P  0.077339 0.007998  0.496254 0.011843  P-0.0350382 0.0081489                                                                                                             
-23 521 60085.00 P  0.080021 0.008051  0.497264 0.011942  P-0.0345722 0.0082248                                                                                                             
-23 522 60086.00 P  0.082717 0.008104  0.498234 0.012041  P-0.0339157 0.0083005                                                                                                             
-23 523 60087.00 P  0.085425 0.008156  0.499163 0.012139  P-0.0331527 0.0083759                                                                                                             
-23 524 60088.00 P  0.088146 0.008208  0.500051 0.012237  P-0.0323691 0.0084511                                                                                                             
-23 525 60089.00 P  0.090878 0.008260  0.500897 0.012335  P-0.0316421 0.0085261                                                                                                             
-23 526 60090.00 P  0.093620 0.008312  0.501702 0.012432  P-0.0310315 0.0086008                                                                                                             
-23 527 60091.00 P  0.096373 0.008363  0.502466 0.012529  P-0.0305741 0.0086754                                                                                                             
-23 528 60092.00 P  0.099134 0.008414  0.503188 0.012626  P-0.0302814 0.0087497                                                                                                             
-23 529 60093.00 P  0.101904 0.008465  0.503868 0.012723  P-0.0301391 0.0088237                                                                                                             
-23 530 60094.00 P  0.104682 0.008516  0.504506 0.012819  P-0.0301080 0.0088976                                                                                                             
-23 531 60095.00 P  0.107467 0.008566  0.505102 0.012915  P-0.0301253 0.0089713                                                                                                             
-23 6 1 60096.00 P  0.110258 0.008616  0.505656 0.013011  P-0.0301075 0.0090448                                                                                                             
-23 6 2 60097.00 P  0.113054 0.008666  0.506168 0.013106  P-0.0299615 0.0091180                                                                                                             
-23 6 3 60098.00 P  0.115856 0.008716  0.506638 0.013201  P-0.0296084 0.0091911                                                                                                             
-23 6 4 60099.00 P  0.118661 0.008766  0.507065 0.013296  P-0.0290126 0.0092639                                                                                                             
-23 6 5 60100.00 P  0.121468 0.008815  0.507447 0.013391  P-0.0282046 0.0093366                                                                                                             
-23 6 6 60101.00 P  0.124278 0.008864  0.507787 0.013485  P-0.0272820 0.0094091                                                                                                             
-23 6 7 60102.00 P  0.127089 0.008913  0.508084 0.013579  P-0.0263809 0.0094814                                                                                                             
-23 6 8 60103.00 P  0.129902 0.008962  0.508339 0.013673  P-0.0256293 0.0095535                                                                                                             
-23 6 9 60104.00 P  0.132715 0.009010  0.508552 0.013767  P-0.0251050 0.0096254                                                                                                             
-23 610 60105.00 P  0.135528 0.009059  0.508721 0.013860  P-0.0248163 0.0096971                                                                                                             
-23 611 60106.00 P  0.138340 0.009107  0.508849 0.013953  P-0.0247040 0.0097686                                                                                                             
-23 612 60107.00 P  0.141150 0.009155  0.508934 0.014046  P-0.0246651 0.0098400                                                                                                             
-23 613 60108.00 P  0.143958 0.009203  0.508977 0.014139  P-0.0245763 0.0099112                                                                                                             
-23 614 60109.00 P  0.146762 0.009250  0.508977 0.014231  P-0.0243289 0.0099822                                                                                                             
-23 615 60110.00 P  0.149563 0.009298  0.508935 0.014324  P-0.0238489 0.0100531                                                                                                             
-23 616 60111.00 P  0.152359 0.009345  0.508851 0.014416  P-0.0231075 0.0101238                                                                                                             
-23 617 60112.00 P  0.155150 0.009392  0.508724 0.014507  P-0.0221207 0.0101943                                                                                                             
-23 618 60113.00 P  0.157934 0.009439  0.508556 0.014599  P-0.0209411 0.0102646                                                                                                             
-23 619 60114.00 P  0.160712 0.009486  0.508346 0.014690  P-0.0196440 0.0103348                                                                                                             
-23 620 60115.00 P  0.163483 0.009532  0.508094 0.014781  P-0.0183126 0.0104048                                                                                                             
-23 621 60116.00 P  0.166245 0.009578  0.507800 0.014872  P-0.0170261 0.0104747                                                                                                             
-23 622 60117.00 P  0.168998 0.009625  0.507465 0.014963  P-0.0158472 0.0105444                                                                                                             
-23 623 60118.00 P  0.171742 0.009671  0.507088 0.015053  P-0.0148173 0.0106139                                                                                                             
-23 624 60119.00 P  0.174476 0.009717  0.506670 0.015143  P-0.0139519 0.0106833                                                                                                             
-23 625 60120.00 P  0.177199 0.009762  0.506211 0.015233  P-0.0132407 0.0107526                                                                                                             
-23 626 60121.00 P  0.179909 0.009808  0.505711 0.015323  P-0.0126501 0.0108216                                                                                                             
-23 627 60122.00 P  0.182608 0.009853  0.505170 0.015413  P-0.0121276 0.0108906                                                                                                             
-23 628 60123.00 P  0.185294 0.009898  0.504589 0.015502  P-0.0116035 0.0109594                                                                                                             
-23 629 60124.00 P  0.187966 0.009943  0.503968 0.015591  P-0.0109971 0.0110280                                                                                                             
-23 630 60125.00 P  0.190623 0.009988  0.503307 0.015680  P-0.0102301 0.0110965                                                                                                             
-23 7 1 60126.00 P  0.193266 0.010033  0.502605 0.015769  P-0.0092506 0.0111649                                                                                                             
-23 7 2 60127.00 P  0.195893 0.010078  0.501864 0.015858  P-0.0080604 0.0112331                                                                                                             
-23 7 3 60128.00 P  0.198503 0.010122  0.501084 0.015946  P-0.0067306 0.0113012                                                                                                             
-23 7 4 60129.00 P  0.201097 0.010166  0.500265 0.016034  P-0.0053910 0.0113691                                                                                                             
-23 7 5 60130.00 P  0.203672 0.010211  0.499407 0.016122  P-0.0041885 0.0114369                                                                                                             
-23 7 6 60131.00 P  0.206230 0.010255  0.498510 0.016210  P-0.0032337 0.0115046                                                                                                             
-23 7 7 60132.00 P  0.208768 0.010298  0.497575 0.016298  P-0.0025598 0.0115721                                                                                                             
-23 7 8 60133.00 P  0.211287 0.010342  0.496602 0.016385  P-0.0021131 0.0116395                                                                                                             
-23 7 9 60134.00 P  0.213786 0.010386  0.495592 0.016473  P-0.0017763 0.0117067                                                                                                             
-23 710 60135.00 P  0.216264 0.010429  0.494544 0.016560  P-0.0014108 0.0117739                                                                                                             
-23 711 60136.00 P  0.218721 0.010473  0.493459 0.016647  P-0.0008961 0.0118409                                                                                                             
-23 712 60137.00 P  0.221155 0.010516  0.492338 0.016734  P-0.0001546 0.0119077                                                                                                             
-23 713 60138.00 P  0.223567 0.010559  0.491180 0.016820  P 0.0008409 0.0119745                                                                                                             
-23 714 60139.00 P  0.225956 0.010602  0.489987 0.016907  P 0.0020742 0.0120411                                                                                                             
-23 715 60140.00 P  0.228321 0.010645  0.488758 0.016993  P 0.0034952 0.0121076                                                                                                             
-23 716 60141.00 P  0.230661 0.010687  0.487493 0.017079  P 0.0050329 0.0121740                                                                                                             
-23 717 60142.00 P  0.232977 0.010730  0.486194 0.017165  P 0.0066079 0.0122402                                                                                                             
-23 718 60143.00 P  0.235266 0.010772  0.484860 0.017251  P 0.0081418 0.0123063                                                                                                             
-23 719 60144.00 P  0.237530 0.010814  0.483493 0.017336  P 0.0095677 0.0123723                                                                                                             
-23 720 60145.00 P  0.239768 0.010857  0.482092 0.017422  P 0.0108388 0.0124382                                                                                                             
-23 721 60146.00 P  0.241978 0.010899  0.480657 0.017507  P 0.0119335 0.0125040                                                                                                             
-23 722 60147.00 P  0.244160 0.010941  0.479190 0.017592  P 0.0128581 0.0125696                                                                                                             
-23 723 60148.00 P  0.246314 0.010982  0.477691 0.017677  P 0.0136443 0.0126352                                                                                                             
-23 724 60149.00 P  0.248440 0.011024  0.476159 0.017762  P 0.0143434 0.0127006                                                                                                             
-23 725 60150.00 P  0.250536 0.011066  0.474596 0.017846  P 0.0150196 0.0127659                                                                                                             
-23 726 60151.00 P  0.252602 0.011107  0.473003 0.017931  P 0.0157429 0.0128311                                                                                                             
-23 727 60152.00 P  0.254638 0.011148  0.471378 0.018015  P 0.0165833 0.0128962                                                                                                             
-23 728 60153.00 P  0.256644 0.011190  0.469724 0.018099  P 0.0175962 0.0129612                                                                                                             
-23 729 60154.00 P  0.258618 0.011231  0.468040 0.018183  P 0.0187999 0.0130260                                                                                                             
-23 730 60155.00 P  0.260560 0.011272  0.466327 0.018267  P 0.0201537 0.0130908                                                                                                             
-23 731 60156.00 P  0.262471 0.011312  0.464586 0.018351  P 0.0215530 0.0131554                                                                                                             
-23 8 1 60157.00 P  0.264348 0.011353  0.462816 0.018434  P 0.0228508 0.0132199                                                                                                             
-23 8 2 60158.00 P  0.266193 0.011394  0.461019 0.018518  P 0.0239072 0.0132844                                                                                                             
-23 8 3 60159.00 P  0.268005 0.011434  0.459195 0.018601  P 0.0246439 0.0133487                                                                                                             
-23 8 4 60160.00 P  0.269782 0.011475  0.457344 0.018684  P 0.0250782 0.0134129                                                                                                             
-23 8 5 60161.00 P  0.271525 0.011515  0.455467 0.018767  P 0.0253188 0.0134770                                                                                                             
-23 8 6 60162.00 P  0.273234 0.011555  0.453565 0.018850  P 0.0255250 0.0135410                                                                                                             
-23 8 7 60163.00 P  0.274907 0.011595  0.451638 0.018932  P 0.0258512 0.0136050                                                                                                             
-23 8 8 60164.00 P  0.276545 0.011635  0.449686 0.019015  P 0.0264041 0.0136688                                                                                                             
-23 8 9 60165.00 P  0.278148 0.011675  0.447711 0.019097  P 0.0272250 0.0137325                                                                                                             
-23 810 60166.00 P  0.279714 0.011715  0.445712 0.019180  P 0.0282975 0.0137961                                                                                                             
-23 811 60167.00 P  0.281244 0.011755  0.443691 0.019262  P 0.0295663 0.0138596                                                                                                             
-23 812 60168.00 P  0.282736 0.011794  0.441647 0.019344  P 0.0309557 0.0139230                                                                                                             
-23 813 60169.00 P  0.284192 0.011834  0.439582 0.019426  P 0.0323847 0.0139863                                                                                                             
-23 814 60170.00 P  0.285610 0.011873  0.437496 0.019507  P 0.0337742 0.0140495                                                                                                             
-23 815 60171.00 P  0.286990 0.011913  0.435389 0.019589  P 0.0350557 0.0141127                                                                                                             
-23 816 60172.00 P  0.288332 0.011952  0.433263 0.019670  P 0.0361774 0.0141757                                                                                                             
-23 817 60173.00 P  0.289636 0.011991  0.431117 0.019752  P 0.0371116 0.0142386                                                                                                             
-23 818 60174.00 P  0.290901 0.012030  0.428953 0.019833  P 0.0378581 0.0143014                                                                                                             
-23 819 60175.00 P  0.292128 0.012069  0.426770 0.019914  P 0.0384434 0.0143642                                                                                                             
-23 820 60176.00 P  0.293315 0.012108  0.424571 0.019995  P 0.0389174 0.0144268                                                                                                             
-23 821 60177.00 P  0.294462 0.012146  0.422354 0.020076  P 0.0393442 0.0144894                                                                                                             
-23 822 60178.00 P  0.295570 0.012185  0.420121 0.020156  P 0.0397924 0.0145519                                                                                                             
-23 823 60179.00 P  0.296638 0.012224  0.417873 0.020237  P 0.0403269 0.0146142                                                                                                             
-23 824 60180.00 P  0.297666 0.012262  0.415609 0.020317  P 0.0409974 0.0146765                                                                                                             
-23 825 60181.00 P  0.298654 0.012300  0.413331 0.020398  P 0.0418258 0.0147387                                                                                                             
-23 826 60182.00 P  0.299601 0.012339  0.411040 0.020478  P 0.0427898 0.0148008                                                                                                             
-23 827 60183.00 P  0.300508 0.012377  0.408735 0.020558  P 0.0438117 0.0148629                                                                                                             
-23 828 60184.00 P  0.301374 0.012415  0.406418 0.020638  P 0.0447645 0.0149248                                                                                                             
-23 829 60185.00 P  0.302199 0.012453  0.404089 0.020718  P 0.0455035 0.0149867                                                                                                             
-23 830 60186.00 P  0.302982 0.012491  0.401748 0.020797  P 0.0459181 0.0150484                                                                                                             
-23 831 60187.00 P  0.303725 0.012529  0.399397 0.020877  P 0.0459817 0.0151101                                                                                                             
-23 9 1 60188.00 P  0.304426 0.012566  0.397037 0.020957  P 0.0457728 0.0151717                                                                                                             
-23 9 2 60189.00 P  0.305086 0.012604  0.394666 0.021036  P 0.0454531 0.0152332                                                                                                             
-23 9 3 60190.00 P  0.305704 0.012642  0.392287 0.021115  P 0.0452124 0.0152946                                                                                                             
-23 9 4 60191.00 P  0.306280 0.012679  0.389901 0.021194  P 0.0452045 0.0153560                                                                                                             
-23 9 5 60192.00 P  0.306815 0.012717  0.387506 0.021273  P 0.0455061 0.0154172                                                                                                             
-23 9 6 60193.00 P  0.307308 0.012754  0.385105 0.021352  P 0.0461107 0.0154784                                                                                                             
-23 9 7 60194.00 P  0.307759 0.012791  0.382698 0.021431  P 0.0469515 0.0155395                                                                                                             
-23 9 8 60195.00 P  0.308168 0.012828  0.380285 0.021510  P 0.0479341 0.0156005                                                                                                             
-23 9 9 60196.00 P  0.308535 0.012865  0.377868 0.021588  P 0.0489634 0.0156614                                                                                                             
-23 910 60197.00 P  0.308861 0.012902  0.375446 0.021667  P 0.0499577 0.0157223                                                                                                             
-23 911 60198.00 P  0.309144 0.012939  0.373021 0.021745  P 0.0508543 0.0157831                                                                                                             
-23 912 60199.00 P  0.309385 0.012976  0.370593 0.021823  P 0.0516097 0.0158438                                                                                                             
-23 913 60200.00 P  0.309585 0.013013  0.368163 0.021901  P 0.0522011 0.0159044                                                                                                             
-23 914 60201.00 P  0.309743 0.013050  0.365731 0.021979  P 0.0526267 0.0159649                                                                                                             
-23 915 60202.00 P  0.309858 0.013086  0.363298 0.022057  P 0.0529065 0.0160254                                                                                                             
-23 916 60203.00 P  0.309932 0.013123  0.360865 0.022135  P 0.0530800 0.0160858                                                                                                             
-23 917 60204.00 P  0.309965 0.013159  0.358433 0.022213  P 0.0532027 0.0161461                                                                                                             
-23 918 60205.00 P  0.309955 0.013195  0.356001 0.022290  P 0.0533382 0.0162063                                                                                                             
-23 919 60206.00 P  0.309904 0.013232  0.353571 0.022368  P 0.0535465 0.0162665                                                                                                             
-23 920 60207.00 P  0.309812 0.013268  0.351143 0.022445  P 0.0538696 0.0163265                                                                                                             
-23 921 60208.00 P  0.309678 0.013304  0.348718 0.022522  P 0.0543192 0.0163866                                                                                                             
-23 922 60209.00 P  0.309503 0.013340  0.346297 0.022600  P 0.0548705 0.0164465                                                                                                             
-23 923 60210.00 P  0.309286 0.013376  0.343880 0.022677  P 0.0554609 0.0165063                                                                                                             
-23 924 60211.00 P  0.309029 0.013412  0.341467 0.022754  P 0.0559953 0.0165661                                                                                                             
-23 925 60212.00 P  0.308731 0.013448  0.339061 0.022830  P 0.0563619 0.0166258                                                                                                             
-23 926 60213.00 P  0.308392 0.013484  0.336660 0.022907  P 0.0564582 0.0166855                                                                                                             
-23 927 60214.00 P  0.308012 0.013520  0.334266 0.022984  P 0.0562244 0.0167451                                                                                                             
-23 928 60215.00 P  0.307593 0.013555  0.331879 0.023060  P 0.0556753 0.0168046                                                                                                             
-23 929 60216.00 P  0.307133 0.013591  0.329500 0.023137  P 0.0549111 0.0168640                                                                                                             
-23 930 60217.00 P  0.306633 0.013626  0.327130 0.023213  P 0.0540986 0.0169233                                                                                                             
-2310 1 60218.00 P  0.306094 0.013662  0.324769 0.023290  P 0.0534092 0.0169826                                                                                                             
-2310 2 60219.00 P  0.305515 0.013697  0.322418 0.023366  P 0.0529614 0.0170419                                                                                                             
-2310 3 60220.00 P  0.304896 0.013732  0.320077 0.023442  P 0.0528128 0.0171010                                                                                                             
-2310 4 60221.00 P  0.304239 0.013768  0.317747 0.023518  P 0.0529763 0.0171601                                                                                                             
-2310 5 60222.00 P  0.303543 0.013803  0.315429 0.023594  P 0.0533332 0.0172191                                                                                                             
-2310 6 60223.00 P  0.302808 0.013838  0.313123 0.023669  P 0.0538302 0.0172780                                                                                                             
-2310 7 60224.00 P  0.302035 0.013873  0.310829 0.023745  P 0.0543504 0.0173369                                                                                                             
-2310 8 60225.00 P  0.301225 0.013908  0.308549 0.023821  P 0.0547262 0.0173957                                                                                                             
-2310 9 60226.00 P  0.300376 0.013943  0.306283 0.023896  P 0.0549269 0.0174545                                                                                                             
-231010 60227.00 P  0.299491 0.013977  0.304032 0.023972  P 0.0549897 0.0175131                                                                                                             
-231011 60228.00 P  0.298568 0.014012  0.301795 0.024047  P 0.0549348 0.0175718                                                                                                             
-231012 60229.00 P  0.297608 0.014047  0.299575 0.024122  P 0.0547332 0.0176303                                                                                                             
-231013 60230.00 P  0.296613 0.014082  0.297370 0.024197  P 0.0544315 0.0176888                                                                                                             
-231014 60231.00 P  0.295581 0.014116  0.295182 0.024272  P 0.0540644 0.0177472                                                                                                             
-231015 60232.00 P  0.294513 0.014151  0.293012 0.024347  P 0.0537081 0.0178055                                                                                                             
-231016 60233.00 P  0.293410 0.014185  0.290859 0.024422  P 0.0534750 0.0178638                                                                                                             
-231017 60234.00 P  0.292273 0.014219  0.288725 0.024497  P 0.0533648 0.0179220                                                                                                             
-231018 60235.00 P  0.291100 0.014254  0.286610 0.024572  P 0.0534631 0.0179802                                                                                                             
-231019 60236.00 P  0.289894 0.014288  0.284514 0.024646  P 0.0537054 0.0180383                                                                                                             
-231020 60237.00 P  0.288654 0.014322  0.282438 0.024721  P 0.0540871 0.0180963                                                                                                             
-231021 60238.00 P  0.287380 0.014356  0.280383 0.024795  P 0.0544590 0.0181543                                                                                                             
-231022 60239.00 P  0.286074 0.014390  0.278349 0.024870  P 0.0548236 0.0182122                                                                                                             
-231023 60240.00 P  0.284734 0.014424  0.276336 0.024944  P 0.0548678 0.0182700                                                                                                             
-231024 60241.00 P  0.283363 0.014458  0.274346 0.025018  P 0.0546272 0.0183278                                                                                                             
-231025 60242.00 P  0.281961 0.014492  0.272377 0.025092  P 0.0541166 0.0183855                                                                                                             
-231026 60243.00 P  0.280527 0.014526  0.270432 0.025166  P 0.0533302 0.0184432                                                                                                             
-231027 60244.00 P  0.279062 0.014560  0.268511 0.025240  P 0.0524004 0.0185008                                                                                                             
-231028 60245.00 P  0.277567 0.014594  0.266613 0.025314  P 0.0514864 0.0185583                                                                                                             
-231029 60246.00 P  0.276042 0.014627  0.264739 0.025388  P 0.0507728 0.0186158                                                                                                             
-231030 60247.00 P  0.274488 0.014661  0.262891 0.025461  P 0.0503153 0.0186732                                                                                                             
-231031 60248.00 P  0.272905 0.014694  0.261067 0.025535  P 0.0501782 0.0187306                                                                                                             
-2311 1 60249.00 P  0.271293 0.014728  0.259270 0.025608  P 0.0503667 0.0187879                                                                                                             
-2311 2 60250.00 P  0.269654 0.014761  0.257498 0.025682  P 0.0507889 0.0188451                                                                                                             
-2311 3 60251.00 P  0.267988 0.014795  0.255754 0.025755  P 0.0512401 0.0189023                                                                                                             
-2311 4 60252.00 P  0.266294 0.014828  0.254036 0.025828  P 0.0516895 0.0189594                                                                                                             
-2311 5 60253.00 P  0.264574 0.014861  0.252345 0.025902  P 0.0520506 0.0190165                                                                                                             
-2311 6 60254.00 P  0.262829 0.014894  0.250683 0.025975  P 0.0522580 0.0190735                                                                                                             
-2311 7 60255.00 P  0.261058 0.014927  0.249048 0.026048  P 0.0522975 0.0191305                                                                                                             
-2311 8 60256.00 P  0.259262 0.014960  0.247442 0.026121  P 0.0522420 0.0191874                                                                                                             
-2311 9 60257.00 P  0.257443 0.014994  0.245865 0.026193  P 0.0520442 0.0192442                                                                                                             
-231110 60258.00 P  0.255599 0.015026  0.244318 0.026266  P 0.0517749 0.0193010                                                                                                             
-231111 60259.00 P  0.253733 0.015059  0.242800 0.026339  P 0.0515263 0.0193577                                                                                                             
-231112 60260.00 P  0.251844 0.015092  0.241312 0.026412  P 0.0512992 0.0194144                                                                                                             
-231113 60261.00 P  0.249933 0.015125  0.239854 0.026484  P 0.0512067 0.0194710                                                                                                             
-231114 60262.00 P  0.248001 0.015158  0.238427 0.026557  P 0.0513491 0.0195276                                                                                                             
-231115 60263.00 P  0.246048 0.015191  0.237031 0.026629  P 0.0517135 0.0195841                                                                                                             
-231116 60264.00 P  0.244075 0.015223  0.235666 0.026701  P 0.0522346 0.0196405                                                                                                             
-231117 60265.00 P  0.242082 0.015256  0.234333 0.026774  P 0.0528450 0.0196969                                                                                                             
-231118 60266.00 P  0.240070 0.015288  0.233032 0.026846  P 0.0534272 0.0197532                                                                                                             
-231119 60267.00 P  0.238039 0.015321  0.231763 0.026918  P 0.0538215 0.0198095                                                                                                             
-231120 60268.00 P  0.235991 0.015353  0.230527 0.026990  P 0.0539101 0.0198658                                                                                                             
-231121 60269.00 P  0.233926 0.015386  0.229323 0.027062  P 0.0536767 0.0199219                                                                                                             
-231122 60270.00 P  0.231844 0.015418  0.228152 0.027134  P 0.0531928 0.0199781                                                                                                             
-231123 60271.00 P  0.229745 0.015450  0.227015 0.027205  P 0.0525905 0.0200341                                                                                                             
-231124 60272.00 P  0.227632 0.015482  0.225910 0.027277  P 0.0520118 0.0200902                                                                                                             
-231125 60273.00 P  0.225503 0.015515  0.224840 0.027349  P 0.0515576 0.0201461                                                                                                             
-231126 60274.00 P  0.223361 0.015547  0.223803 0.027420  P 0.0513870 0.0202021                                                                                                             
-231127 60275.00 P  0.221205 0.015579  0.222801 0.027492  P 0.0514249 0.0202579                                                                                                             
-231128 60276.00 P  0.219036 0.015611  0.221833 0.027563  P 0.0517474 0.0203137                                                                                                             
-231129 60277.00 P  0.216854 0.015643  0.220899 0.027635  P 0.0522705 0.0203695                                                                                                             
-231130 60278.00 P  0.214661 0.015675  0.220001 0.027706  P 0.0528356 0.0204252                                                                                                             
-2312 1 60279.00 P  0.212457 0.015707  0.219136 0.027777  P 0.0534205 0.0204809                                                                                                             
-2312 2 60280.00 P  0.210243 0.015739  0.218307 0.027848  P 0.0539537 0.0205365                                                                                                             
-2312 3 60281.00 P  0.208018 0.015770  0.217514 0.027919  P 0.0543705 0.0205920                                                                                                             
-2312 4 60282.00 P  0.205785 0.015802  0.216755 0.027990  P 0.0546131 0.0206475                                                                                                             
-2312 5 60283.00 P  0.203543 0.015834  0.216032 0.028061  P 0.0546772 0.0207030                                                                                                             
-2312 6 60284.00 P  0.201293 0.015865  0.215344 0.028132  P 0.0545472 0.0207584                                                                                                             
-2312 7 60285.00 P  0.199036 0.015897  0.214692 0.028203  P 0.0542568 0.0208138                                                                                                             
-2312 8 60286.00 P  0.196772 0.015929  0.214076 0.028274  P 0.0538719 0.0208691                                                                                                             
-2312 9 60287.00 P  0.194503 0.015960  0.213496 0.028344  P 0.0534964 0.0209243                                                                                                             
-231210 60288.00 P  0.192228 0.015991  0.212951 0.028415  P 0.0532064 0.0209795                                                                                                             
-231211 60289.00 P  0.189949 0.016023  0.212443 0.028485  P 0.0530850 0.0210347                                                                                                             
-231212 60290.00 P  0.187665 0.016054  0.211970 0.028556  P 0.0531543 0.0210898                                                                                                             
-231213 60291.00 P  0.185378 0.016086  0.211534 0.028626  P 0.0533748 0.0211449                                                                                                             
-231214 60292.00 P  0.183089 0.016117  0.211134 0.028696  P 0.0536963 0.0211999                                                                                                             
-231215 60293.00 P  0.180797 0.016148  0.210770 0.028767  P 0.0539614 0.0212548                                                                                                             
-231216 60294.00 P  0.178504 0.016179  0.210442 0.028837  P 0.0540707 0.0213098                                                                                                             
-231217 60295.00 P  0.176210 0.016210  0.210151 0.028907  P 0.0538724 0.0213646                                                                                                             
-231218 60296.00 P  0.173916 0.016241  0.209895 0.028977  P 0.0533780 0.0214195                                                                                                             
-231219 60297.00 P  0.171622 0.016273  0.209676 0.029047  P 0.0526884 0.0214742                                                                                                             
-231220 60298.00 P  0.169330 0.016304  0.209493 0.029117  P 0.0519334 0.0215290                                                                                                             
-231221 60299.00 P  0.167039 0.016334  0.209346 0.029187  P 0.0512447 0.0215837                                                                                                             
-231222 60300.00 P  0.164751 0.016365  0.209235 0.029256  P 0.0506822 0.0216383                                                                                                             
-231223 60301.00 P  0.162466 0.016396  0.209160 0.029326  P 0.0503702 0.0216929                                                                                                             
-231224 60302.00 P  0.160184 0.016427  0.209121 0.029396  P 0.0503059 0.0217474                                                                                                             
-231225 60303.00 P  0.157907 0.016458  0.209118 0.029465  P 0.0505667 0.0218019                                                                                                             
-231226 60304.00 P  0.155635 0.016489  0.209151 0.029535  P 0.0510804 0.0218564                                                                                                             
-231227 60305.00 P  0.153368 0.016519  0.209220 0.029604  P 0.0517491 0.0219108                                                                                                             
-231228 60306.00 P  0.151108 0.016550  0.209324 0.029674  P 0.0524347 0.0219652                                                                                                             
-231229 60307.00 P  0.148854 0.016581  0.209464 0.029743  P 0.0530407 0.0220195                                                                                                             
-231230 60308.00 P  0.146607 0.016611  0.209639 0.029812  P 0.0535487 0.0220738                                                                                                             
-231231 60309.00 P  0.144369 0.016642  0.209850 0.029882  P 0.0539047 0.0221280                                                                                                             
-24 1 1 60310.00 P  0.142139 0.016672  0.210095 0.029951  P 0.0540927 0.0221822                                                                                                             
-24 1 2 60311.00 P  0.139919 0.016703  0.210376 0.030020  P 0.0542805 0.0222363                                                                                                             
-24 1 3 60312.00 P  0.137708 0.016733  0.210691 0.030089  P 0.0544962 0.0222904                                                                                                             
-24 1 4 60313.00 P  0.135508 0.016763  0.211042 0.030158  P 0.0547489 0.0223444                                                                                                             
-24 1 5 60314.00 P  0.133319 0.016794  0.211426 0.030227  P 0.0550813 0.0223985                                                                                                             
-24 1 6 60315.00 P  0.131141 0.016824  0.211845 0.030296  P 0.0555269 0.0224524                                                                                                             
-24 1 7 60316.00 P  0.128976 0.016854  0.212298 0.030364  P 0.0561288 0.0225063                                                                                                             
-24 1 8 60317.00 P  0.126823 0.016884  0.212785 0.030433  P 0.0569011 0.0225602                                                                                                             
-24 1 9 60318.00 P  0.124684 0.016914  0.213306 0.030502  P 0.0578554 0.0226140                                                                                                             
-24 110 60319.00 P  0.122559 0.016945  0.213860 0.030570  P 0.0589228 0.0226678                                                                                                             
-24 111 60320.00 P  0.120448 0.016975  0.214447 0.030639  P 0.0599648 0.0227216                                                                                                             
-24 112 60321.00 P  0.118353 0.017005  0.215068 0.030707  P 0.0608038 0.0227753                                                                                                             
-24 113 60322.00 P  0.116273 0.017035  0.215721 0.030776  P 0.0613643 0.0228290                                                                                                             
-24 114 60323.00 P  0.114209 0.017065  0.216406 0.030844  P 0.0616062 0.0228826                                                                                                             
-24 115 60324.00 P  0.112162 0.017094  0.217124 0.030912  P 0.0614757 0.0229362                                                                                                             
-24 116 60325.00 P  0.110132 0.017124  0.217874 0.030981  P 0.0611834 0.0229897                                                                                                             
-24 117 60326.00 P  0.108120 0.017154  0.218655 0.031049  P 0.0609144 0.0230432                                                                                                             
-24 118 60327.00 P  0.106126 0.017184  0.219468 0.031117  P 0.0608218 0.0230966                                                                                                             
-24 119 60328.00 P  0.104151 0.017214  0.220312 0.031185  P 0.0610155 0.0231500                                                                                                             
-24 120 60329.00 P  0.102196 0.017243  0.221187 0.031253  P 0.0615200 0.0232034                                                                                                             
-24 121 60330.00 P  0.100260 0.017273  0.222092 0.031321  P 0.0622890 0.0232567                                                                                                             
-24 122 60331.00 P  0.098345 0.017303  0.223027 0.031389  P 0.0633345 0.0233100                                                                                                             
-24 123 60332.00 P  0.096451 0.017332  0.223992 0.031457  P 0.0644509 0.0233633                                                                                                             
-24 124 60333.00 P  0.094578 0.017362  0.224987 0.031525  P 0.0655796 0.0234165                                                                                                             
-24 125 60334.00 P  0.092727 0.017391  0.226011 0.031592  P 0.0666174 0.0234697                                                                                                             
-24 126 60335.00 P  0.090898 0.017421  0.227063 0.031660  P 0.0675376 0.0235228                                                                                                             
-24 127 60336.00 P  0.089092 0.017450  0.228144 0.031728  P 0.0683282 0.0235759                                                                                                             
-24 128 60337.00 P  0.087309 0.017480  0.229253 0.031795  P 0.0689910 0.0236289                                                                                                             
-24 129 60338.00 P  0.085550 0.017509  0.230390 0.031863  P 0.0694970 0.0236819                                                                                                             
-24 130 60339.00 P  0.083816 0.017538  0.231554 0.031930  P 0.0698224 0.0237349                                                                                                             
-24 131 60340.00 P  0.082105 0.017568  0.232744 0.031998  P 0.0701180 0.0237878                                                                                                             
-24 2 1 60341.00 P  0.080420 0.017597  0.233962 0.032065  P 0.0704315 0.0238407                                                                                                             
-24 2 2 60342.00 P  0.078761 0.017626  0.235205 0.032132  P 0.0708510 0.0238935                                                                                                             
-24 2 3 60343.00 P  0.077127 0.017655  0.236474 0.032199  P 0.0714072 0.0239463                                                                                                             
-24 2 4 60344.00 P  0.075519 0.017685  0.237769 0.032267  P 0.0721529 0.0239991                                                                                                             
-24 2 5 60345.00 P  0.073938 0.017714  0.239088 0.032334  P 0.0730490 0.0240518                                                                                                             
-24 2 6 60346.00 P  0.072385 0.017743  0.240432 0.032401  P 0.0739801 0.0241045                                                                                                             
-24 2 7 60347.00 P  0.070858 0.017772  0.241799 0.032468  P 0.0749737 0.0241572                                                                                                             
-24 2 8 60348.00 P  0.069360 0.017801  0.243190 0.032535  P 0.0759111 0.0242098                                                                                                             
-24 2 9 60349.00 P  0.067889 0.017830  0.244605 0.032602  P 0.0766211 0.0242624                                                                                                             
-24 210 60350.00 P  0.066448 0.017859  0.246042 0.032668  P 0.0770085 0.0243149                                                                                                             
-24 211 60351.00 P  0.065035 0.017888  0.247501 0.032735  P 0.0770433 0.0243674                                                                                                             
-24 212 60352.00 P  0.063651 0.017917  0.248982 0.032802  P 0.0768473 0.0244199                                                                                                             
-24 213 60353.00 P  0.062297 0.017945  0.250484 0.032869  P 0.0765228 0.0244723                                                                                                             
-24 214 60354.00 P  0.060973 0.017974  0.252007 0.032935  P 0.0762239 0.0245247                                                                                                             
-24 215 60355.00 P  0.059679 0.018003  0.253550 0.033002  P 0.0762265 0.0245770                                                                                                             
-24 216 60356.00 P  0.058416 0.018032  0.255113 0.033068  P 0.0765923 0.0246293                                                                                                             
-24 217 60357.00 P  0.057183 0.018060  0.256695 0.033135  P 0.0771848 0.0246816                                                                                                             
-24 218 60358.00 P  0.055981 0.018089  0.258296 0.033201  P 0.0780065 0.0247338                                                                                                             
-24 219 60359.00 P  0.054811 0.018118  0.259916 0.033268  P 0.0789791 0.0247860                                                                                                             
-24 220 60360.00 P  0.053672 0.018146  0.261554 0.033334  P 0.0799701 0.0248382                                                                                                             
-24 221 60361.00 P  0.052566 0.018175  0.263208 0.033400  P 0.0808899 0.0248903                                                                                                             
-24 222 60362.00 P  0.051491 0.018203  0.264880 0.033466  P 0.0816553 0.0249424                                                                                                             
-24 223 60363.00 P  0.050449 0.018232  0.266568 0.033533  P 0.0822643 0.0249945                                                                                                             
-24 224 60364.00 P  0.049439 0.018260  0.268272 0.033599  P 0.0827032 0.0250465                                                                                                             
-24 225 60365.00 P  0.048462 0.018289  0.269991 0.033665  P 0.0829866 0.0250985                                                                                                             
-24 226 60366.00 P  0.047518 0.018317  0.271725 0.033731  P 0.0830887 0.0251504                                                                                                             
-24 227 60367.00 P  0.046608 0.018345  0.273473 0.033797  P 0.0830643 0.0252023                                                                                                             
-24 228 60368.00 P  0.045731 0.018374  0.275235 0.033863  P 0.0829718 0.0252542                                                                                                             
-24 229 60369.00 P  0.044887 0.018402  0.277010 0.033929  P 0.0829522 0.0253060                                                                                                             
-24 3 1 60370.00 P  0.044077 0.018430  0.278798 0.033994  P 0.0830012 0.0253578                                                                                                             
-24 3 2 60371.00 P  0.043301 0.018458  0.280597 0.034060  P 0.0831834 0.0254096                                                                                                             
-24 3 3 60372.00                                                                                                                                                                            
-24 3 4 60373.00                                                                                                                                                                            
-24 3 5 60374.00                                                                                                                                                                            
-24 3 6 60375.00                                                                                                                                                                            
-24 3 7 60376.00                                                                                                                                                                            
-24 3 8 60377.00                                                                                                                                                                            
-24 3 9 60378.00                                                                                                                                                                            
-24 310 60379.00                                                                                                                                                                            
-24 311 60380.00                                                                                                                                                                            
-24 312 60381.00                                                                                                                                                                            
-24 313 60382.00                                                                                                                                                                            
-24 314 60383.00                                                                                                                                                                            
-24 315 60384.00                                                                                                                                                                            
-24 316 60385.00                                                                                                                                                                            
-24 317 60386.00                                                                                                                                                                            
-24 318 60387.00                                                                                                                                                                            
-24 319 60388.00                                                                                                                                                                            
-24 320 60389.00                                                                                                                                                                            
-24 321 60390.00                                                                                                                                                                            
-24 322 60391.00                                                                                                                                                                            
-24 323 60392.00                                                                                                                                                                            
-24 324 60393.00                                                                                                                                                                            
-24 325 60394.00                                                                                                                                                                            
-24 326 60395.00                                                                                                                                                                            
-24 327 60396.00                                                                                                                                                                            
-24 328 60397.00                                                                                                                                                                            
-24 329 60398.00                                                                                                                                                                            
-24 330 60399.00                                                                                                                                                                            
-24 331 60400.00                                                                                                                                                                            
-24 4 1 60401.00                                                                                                                                                                            
-24 4 2 60402.00                                                                                                                                                                            
-24 4 3 60403.00                                                                                                                                                                            
-24 4 4 60404.00                                                                                                                                                                            
-24 4 5 60405.00                                                                                                                                                                            
-24 4 6 60406.00                                                                                                                                                                            
+22 2 8 59618.00 I  0.025134 0.000020  0.337306 0.000007  I-0.1075833 0.0000055 -0.1713 0.0031  I  -110.126    0.484    -5.837    0.013  0.025193  0.337374 -0.1075919  -110.126    -5.888  
+22 2 9 59619.00 I  0.024112 0.000020  0.338499 0.000007  I-0.1072954 0.0000039 -0.3920 0.0033  I  -110.187    0.502    -6.026    0.021  0.024114  0.338478 -0.1072977  -110.203    -6.067  
+22 210 59620.00 I  0.022891 0.000019  0.339529 0.000007  I-0.1068102 0.0000037 -0.5800 0.0027  I  -110.037    0.502    -6.107    0.021  0.022952  0.339544 -0.1067962  -110.062    -6.157  
+22 211 59621.00 I  0.021292 0.000019  0.340652 0.000007  I-0.1061227 0.0000036 -0.8061 0.0025  I  -109.675    0.502    -6.143    0.021  0.021317  0.340636 -0.1061126  -109.706    -6.193  
+22 212 59622.00 I  0.019528 0.000014  0.341941 0.000008  I-0.1052490 0.0000035 -0.8793 0.0025  I  -109.225    0.542    -6.268    0.027  0.019510  0.341957 -0.1052912  -109.259    -6.321  
+22 213 59623.00 I  0.018053 0.000016  0.343130 0.000010  I-0.1044122 0.0000035 -0.8084 0.0024  I  -108.888    0.571    -6.506    0.097  0.017952  0.343165 -0.1044265  -108.917    -6.560  
+22 214 59624.00 I  0.017241 0.000016  0.344307 0.000010  I-0.1036357 0.0000034 -0.7272 0.0028  I  -108.746    0.571    -6.738    0.097  0.017178  0.344276 -0.1036375  -108.763    -6.785  
+22 215 59625.00 I  0.016798 0.000015  0.345873 0.000010  I-0.1029904 0.0000044 -0.5481 0.0026  I  -108.687    0.593    -6.834    0.133  0.016814  0.345848 -0.1029937  -108.690    -6.864  
+22 216 59626.00 I  0.016421 0.000022  0.347660 0.000013  I-0.1025441 0.0000039 -0.3550 0.0029  I  -108.562    0.565    -6.770    0.218  0.016373  0.347600 -0.1025279  -108.569    -6.803  
+22 217 59627.00 I  0.016159 0.000022  0.349967 0.000013  I-0.1022883 0.0000039 -0.1382 0.0028  I  -108.360    0.565    -6.659    0.218  0.016174  0.349955 -0.1022855  -108.379    -6.702  
+22 218 59628.00 I  0.015966 0.000020  0.352553 0.000012  I-0.1022741 0.0000039  0.0976 0.0031  I  -108.215    0.565    -6.612    0.218  0.015893  0.352552 -0.1022778  -108.238    -6.679  
+22 219 59629.00 I  0.016039 0.000018  0.354982 0.000013  I-0.1024662 0.0000047  0.2814 0.0029  I  -108.224    0.540    -6.649    0.274  0.016057  0.355009 -0.1024803  -108.239    -6.688  
+22 220 59630.00 I  0.016151 0.000029  0.357317 0.000016  I-0.1028123 0.0000042  0.3915 0.0031  I  -108.366    0.515    -6.713    0.218  0.016152  0.357350 -0.1028229  -108.367    -6.714  
+22 221 59631.00 I  0.016267 0.000030  0.359419 0.000016  I-0.1032028 0.0000041  0.3625 0.0033  I  -108.582    0.515    -6.731    0.218  0.016225  0.359459 -0.1032042  -108.568    -6.699  
+22 222 59632.00 I  0.016726 0.000027  0.361250 0.000014  I-0.1035161 0.0000050  0.2701 0.0027  I  -108.840    0.439    -6.683    0.064  0.016672  0.361277 -0.1035256  -108.817    -6.617  
+22 223 59633.00 I  0.017620 0.000030  0.362774 0.000014  I-0.1037175 0.0000034  0.1014 0.0031  I  -109.095    0.443    -6.615    0.146  0.017619  0.362779 -0.1037081  -109.078    -6.583  
+22 224 59634.00 I  0.018442 0.000030  0.364353 0.000015  I-0.1036983 0.0000035 -0.1292 0.0023  I  -109.261    0.443    -6.601    0.146  0.018496  0.364360 -0.1036928  -109.259    -6.613  
+22 225 59635.00 I  0.018979 0.000030  0.365795 0.000013  I-0.1034719 0.0000031 -0.3215 0.0025  I  -109.219    0.448    -6.729    0.192  0.018931  0.365807 -0.1034734  -109.270    -6.743  
+22 226 59636.00 I  0.019617 0.000020  0.367246 0.000008  I-0.1030795 0.0000035 -0.4411 0.0025  I  -109.056    0.448    -6.878    0.192  0.019607  0.367229 -0.1031018  -109.106    -6.902  
+22 227 59637.00 I  0.020237 0.000029  0.368838 0.000010  I-0.1026452 0.0000038 -0.3943 0.0026  I  -108.805    0.418    -7.028    0.155  0.020241  0.368836 -0.1026797  -108.854    -7.042  
+22 228 59638.00 I  0.020644 0.000029  0.370619 0.000011  I-0.1023227 0.0000039 -0.2523 0.0031  I  -108.575    0.418    -7.105    0.155  0.020656  0.370624 -0.1023250  -108.624    -7.107  
+22 3 1 59639.00 I  0.020988 0.000025  0.372332 0.000010  I-0.1021455 0.0000048 -0.0956 0.0029  I  -108.412    0.383    -7.117    0.104  0.020909  0.372342 -0.1021425  -108.462    -7.107  
+22 3 2 59640.00 I  0.021874 0.000028  0.374021 0.000013  I-0.1021639 0.0000043  0.1583 0.0032  I  -108.285    0.490    -7.126    0.107  0.021778  0.373951 -0.1021944  -108.199    -7.104  
+22 3 3 59641.00 I  0.023306 0.000028  0.376267 0.000013  I-0.1024453 0.0000043  0.3616 0.0030  I  -108.155    0.490    -7.153    0.107  0.023290  0.376273 -0.1024561  -107.898    -7.117  
+22 3 4 59642.00 I  0.025006 0.000028  0.378497 0.000013  I-0.1028385 0.0000043  0.4190 0.0038  I  -108.032    0.762    -7.162    0.115  0.024972  0.378479 -0.1028435  -107.637    -7.109  
+22 3 5 59643.00 I  0.026706 0.000017  0.380551 0.000010  I-0.1032447 0.0000062  0.3607 0.0029  I  -108.082    0.762    -7.127    0.115  0.026774  0.380581 -0.1032424  -107.706    -7.086  
+22 3 6 59644.00 I  0.028126 0.000021  0.382624 0.000013  I-0.1035428 0.0000038  0.2512 0.0036  I  -108.304    0.501    -7.110    0.073  0.028086  0.382600 -0.1035550  -108.027    -7.094  
+22 3 7 59645.00 I  0.029547 0.000020  0.384741 0.000013  I-0.1037273 0.0000038  0.0823 0.0025  I  -108.610    0.501    -7.183    0.073  0.029543  0.384798 -0.1037203  -108.450    -7.191  
+22 3 8 59646.00 I  0.030999 0.000016  0.386703 0.000011  I-0.1036821 0.0000034 -0.1627 0.0024  I  -108.843    0.446    -7.322    0.060  0.031018  0.386712 -0.1036844  -108.826    -7.354  
+22 3 9 59647.00 I  0.032216 0.000019  0.388513 0.000016  I-0.1034078 0.0000028 -0.3902 0.0022  I  -108.861    0.640    -7.427    0.047  0.032281  0.388541 -0.1034089  -108.866    -7.460  
+22 310 59648.00 I  0.033082 0.000019  0.390308 0.000016  I-0.1029230 0.0000027 -0.5539 0.0020  I  -108.353    0.785    -7.426    0.029  0.033104  0.390312 -0.1029383  -108.612    -7.475  
+22 311 59649.00 I  0.033672 0.000020  0.392121 0.000016  I-0.1023276 0.0000028 -0.6347 0.0022  I  -108.004    0.785    -7.446    0.029  0.033708  0.392105 -0.1023346  -108.109    -7.473  
+22 312 59650.00 I  0.034135 0.000018  0.393692 0.000015  I-0.1016713 0.0000035 -0.6624 0.0026  I  -107.521    0.785    -7.560    0.029  0.034130  0.393729 -0.1016864  -107.569    -7.581  
+22 313 59651.00 I  0.034427 0.000025  0.395170 0.000020  I-0.1010163 0.0000044 -0.6498 0.0028  I  -107.088    0.707    -7.795    0.042  0.034502  0.395152 -0.1010372  -107.117    -7.813  
+22 314 59652.00 I  0.034370 0.000025  0.396639 0.000019  I-0.1003898 0.0000043 -0.5831 0.0038  I  -106.859    0.707    -8.049    0.042  0.034354  0.396685 -0.1004104  -106.877    -8.063  
+22 315 59653.00 I  0.034234 0.000023  0.398079 0.000015  I-0.0998758 0.0000061 -0.4393 0.0032  I  -106.851    0.600    -8.190    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
+22 316 59654.00 I  0.033955 0.000033  0.399537 0.000017  I-0.0995328 0.0000048 -0.2306 0.0039  I  -106.943    0.617    -8.165    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
+22 317 59655.00 I  0.033459 0.000033  0.401249 0.000017  I-0.0994310 0.0000047  0.0273 0.0035  I  -106.996    0.617    -8.034    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
+22 318 59656.00 I  0.033076 0.000031  0.402918 0.000017  I-0.0995526 0.0000051  0.1808 0.0034  I  -106.975    0.617    -7.902    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
+22 319 59657.00 I  0.032925 0.000027  0.404429 0.000011  I-0.0997804 0.0000048  0.2976 0.0035  I  -106.979    0.659    -7.847    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
+22 320 59658.00 I  0.033031 0.000027  0.405970 0.000011  I-0.1001533 0.0000047  0.4307 0.0032  I  -107.136    0.659    -7.886    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
+22 321 59659.00 I  0.033373 0.000033  0.407434 0.000014  I-0.1005689 0.0000043  0.3449 0.0036  I  -107.465    0.572    -7.977    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
+22 322 59660.00 I  0.034272 0.000023  0.408886 0.000011  I-0.1007884 0.0000054  0.0948 0.0031  I  -107.842    0.534    -8.059    0.071  0.034163  0.408866 -0.1007374  -107.806    -8.084  
+22 323 59661.00 I  0.035752 0.000024  0.410767 0.000016  I-0.1007727 0.0000045 -0.1128 0.0035  I  -108.082    0.499    -8.100    0.073  0.035739  0.410677 -0.1007668  -108.069    -8.122  
+22 324 59662.00 I  0.037151 0.000025  0.412868 0.000016  I-0.1005690 0.0000044 -0.3019 0.0031  I  -108.059    0.499    -8.123    0.073  0.037184  0.412921 -0.1005632  -108.121    -8.146  
+22 325 59663.00 I  0.038266 0.000024  0.415015 0.000016  I-0.1001862 0.0000042 -0.4391 0.0031  I  -107.763    0.499    -8.166    0.073  0.038276  0.415002 -0.1001852  -107.917    -8.187  
+22 326 59664.00 I  0.039265 0.000024  0.416908 0.000016  I-0.0997291 0.0000044 -0.4614 0.0032  I  -107.292    0.499    -8.238    0.073  0.039275  0.416959 -0.0997325  -107.413    -8.263  
+22 327 59665.00 I  0.040351 0.000019  0.418580 0.000015  I-0.0993023 0.0000047 -0.3669 0.0032  I  -106.803    0.533    -8.319    0.081  0.040293  0.418593 -0.0993188  -106.847    -8.345  
+22 328 59666.00 I  0.041640 0.000019  0.420162 0.000016  I-0.0990358 0.0000047 -0.1510 0.0038  I  -106.442    0.533    -8.383    0.081  0.041691  0.420175 -0.0990554  -106.412    -8.410  
+22 329 59667.00 I  0.042745 0.000018  0.421729 0.000012  I-0.0989806 0.0000059  0.0057 0.0033  I  -106.291    0.625    -8.422    0.085  0.042792  0.421696 -0.0989777  -106.189    -8.449  
+22 330 59668.00 I  0.043409 0.000021  0.423077 0.000019  I-0.0990310 0.0000047  0.1139 0.0039  I  -106.328    0.619    -8.428    0.096  0.043491  0.423055 -0.0990426  -106.244    -8.453  
+22 331 59669.00 I  0.043548 0.000022  0.424808 0.000019  I-0.0992196 0.0000050  0.2557 0.0035  I  -106.443    0.619    -8.390    0.096  0.043570  0.424794 -0.0992346  -106.398    -8.414  
+22 4 1 59670.00 I  0.043351 0.000023  0.426970 0.000020  I-0.0995107 0.0000051  0.3023 0.0038  I  -106.516    0.619    -8.316    0.096  0.043301  0.426919 -0.0995031  -106.506    -8.343  
+22 4 2 59671.00 I  0.043555 0.000018  0.428883 0.000018  I-0.0997950 0.0000058  0.2613 0.0041  I  -106.521    0.617    -8.257    0.101  0.043471  0.428898 -0.0997958  -106.536    -8.278  
+22 4 3 59672.00 I  0.044381 0.000021  0.431006 0.000020  I-0.1000069 0.0000064  0.1413 0.0043  I  -106.546    0.606    -8.280    0.077  0.044401  0.430964 -0.1000185  -106.583    -8.291  
+22 4 4 59673.00 I  0.045130 0.000020  0.433541 0.000020  I-0.1000660 0.0000063 -0.0133 0.0052  I  -106.670    0.606    -8.393    0.077  0.045179  0.433548 -0.1000877  -106.727    -8.395  
+22 4 5 59674.00 I  0.045606 0.000016  0.436188 0.000014  I-0.0999593 0.0000081 -0.2308 0.0049  I  -106.846    0.592    -8.523    0.031  0.045558  0.436184 -0.0999601  -106.928    -8.515  
+22 4 6 59675.00 I  0.046388 0.000019  0.438251 0.000020  I-0.0996011 0.0000075 -0.4581 0.0055  I  -106.936    0.628    -8.593    0.040  0.046324  0.438296 -0.0996161  -107.011    -8.588  
+22 4 7 59676.00 I  0.047706 0.000019  0.440056 0.000020  I-0.0990861 0.0000074 -0.5565 0.0053  I  -106.835    0.628    -8.610    0.040  0.047660  0.440084 -0.0991087  -106.904    -8.610  
+22 4 8 59677.00 I  0.049433 0.000018  0.441873 0.000020  I-0.0985111 0.0000074 -0.5858 0.0053  I  -106.535    0.628    -8.669    0.040  0.049412  0.441800 -0.0985116  -106.602    -8.670  
+22 4 9 59678.00 I  0.051231 0.000015  0.443553 0.000017  I-0.0979307 0.0000077 -0.5666 0.0050  I  -106.076    0.659    -8.845    0.046  0.051279  0.443588 -0.0979207  -106.131    -8.844  
+22 410 59679.00 I  0.052565 0.000016  0.445332 0.000019  I-0.0973866 0.0000066 -0.5212 0.0051  I  -105.537    0.793    -9.111    0.054  0.052631  0.445310 -0.0973816  -105.574    -9.106  
+22 411 59680.00 I  0.053446 0.000015  0.447041 0.000018  I-0.0969113 0.0000066 -0.4066 0.0041  I  -105.077    0.793    -9.359    0.054  0.053447  0.447037 -0.0969159  -105.095    -9.347  
+22 412 59681.00 I  0.054290 0.000013  0.449061 0.000018  I-0.0965831 0.0000048 -0.2628 0.0041  I  -104.899    0.832    -9.512    0.125  0.054284  0.449011 -0.0965845  -104.884    -9.491  
+22 413 59682.00 I  0.055326 0.000012  0.451022 0.000017  I-0.0964189 0.0000047 -0.0194 0.0035  I  -105.058    0.832    -9.557    0.125  0.055292  0.451073 -0.0964523  -105.062    -9.565  
+22 414 59683.00 I  0.056532 0.000013  0.452940 0.000017  I-0.0965550 0.0000050  0.2563 0.0034  I  -105.350    0.832    -9.494    0.125  0.056547  0.452892 -0.0965557  -105.379    -9.547  
+22 415 59684.00 I  0.057880 0.000015  0.454442 0.000018  I-0.0968981 0.0000049  0.4320 0.0032  I  -105.519    0.832    -9.312    0.125  0.057823  0.454485 -0.0968994  -105.550    -9.362  
+22 416 59685.00 I  0.059423 0.000018  0.456177 0.000016  I-0.0974024 0.0000040  0.5580 0.0033  I  -105.579    0.796    -9.059    0.167  0.059424  0.456172 -0.0974129  -105.603    -9.095  
+22 417 59686.00 I  0.061284 0.000019  0.457789 0.000016  I-0.0979718 0.0000043  0.5573 0.0043  I  -105.786    0.796    -8.879    0.167  0.061164  0.457851 -0.0979865  -105.807    -8.908  
+22 418 59687.00 I  0.063722 0.000021  0.459299 0.000016  I-0.0984747 0.0000077  0.4299 0.0045  I  -106.253    0.724    -8.900    0.008  0.063734  0.459266 -0.0985020  -106.274    -8.922  
+22 419 59688.00 I  0.066170 0.000022  0.460804 0.000016  I-0.0988063 0.0000080  0.2268 0.0046  I  -106.739    0.724    -9.095    0.008  0.066192  0.460869 -0.0988272  -106.773    -9.104  
+22 420 59689.00 I  0.068332 0.000025  0.462063 0.000024  I-0.0988957 0.0000051 -0.0742 0.0048  I  -106.903    0.795    -9.308    0.093  0.068329  0.461999 -0.0988949  -106.960    -9.291  
+22 421 59690.00 I  0.070493 0.000024  0.463008 0.000024  I-0.0986776 0.0000052 -0.3163 0.0038  I  -106.654    0.795    -9.426    0.093  0.070468  0.463064 -0.0987060  -106.695    -9.434  
+22 422 59691.00 I  0.072756 0.000021  0.464181 0.000024  I-0.0983201 0.0000055 -0.3874 0.0038  I  -106.197    0.795    -9.466    0.093  0.072707  0.464098 -0.0983386  -106.211    -9.508  
+22 423 59692.00 I  0.075223 0.000020  0.465050 0.000024  I-0.0979197 0.0000055 -0.4077 0.0041  I  -105.774    0.795    -9.494    0.093  0.075204  0.465058 -0.0979051  -105.797    -9.527  
+22 424 59693.00 I  0.077856 0.000017  0.466301 0.000036  I-0.0975340 0.0000060 -0.3402 0.0040  I  -105.461    0.842    -9.540    0.119  0.077859  0.466247 -0.0975194  -105.498    -9.555  
+22 425 59694.00 I  0.080486 0.000016  0.467889 0.000036  I-0.0972694 0.0000059 -0.1825 0.0059  I  -105.224    0.842    -9.588    0.119  0.080557  0.467896 -0.0972632  -105.265    -9.590  
+22 426 59695.00 I  0.082816 0.000010  0.469963 0.000031  I-0.0971736 0.0000101 -0.0109 0.0041  I  -105.067    0.779    -9.602    0.091  0.082859  0.469891 -0.0971847  -105.109    -9.593  
+22 427 59696.00 I  0.084841 0.000017  0.471409 0.000033  I-0.0972287 0.0000057  0.1039 0.0058  I  -105.061    0.809    -9.544    0.149  0.084908  0.471486 -0.0972203  -105.096    -9.548  
+22 428 59697.00 I  0.086493 0.000018  0.472748 0.000033  I-0.0973564 0.0000055  0.1437 0.0042  I  -105.231    0.809    -9.381    0.149  0.086518  0.472819 -0.0973522  -105.258    -9.407  
+22 429 59698.00 I  0.087930 0.000018  0.473584 0.000033  I-0.0974930 0.0000062  0.1143 0.0038  I  -105.466    0.809    -9.148    0.149  0.087895  0.473595 -0.0974914  -105.480    -9.203  
+22 430 59699.00 I  0.089676 0.000018  0.474053 0.000015  I-0.0975660 0.0000052  0.0279 0.0040  I  -105.611    0.840    -8.964    0.195  0.089653  0.474104 -0.0975559  -105.614    -9.011  
+22 5 1 59700.00 I  0.091699 0.000019  0.474622 0.000016  I-0.0975397 0.0000052 -0.0857 0.0037  I  -105.636    0.840    -8.955    0.195  0.091728  0.474632 -0.0975257  -105.627    -8.987  
+22 5 2 59701.00 I  0.093635 0.000023  0.475325 0.000020  I-0.0973966 0.0000054 -0.1934 0.0042  I  -105.635    0.789    -9.133    0.114  0.093634  0.475311 -0.0974187  -105.619    -9.154  
+22 5 3 59702.00 I  0.095564 0.000018  0.476094 0.000017  I-0.0971754 0.0000067 -0.2337 0.0043  I  -105.680    0.775    -9.361    0.031  0.095563  0.476140 -0.0972185  -105.662    -9.372  
+22 5 4 59703.00 I  0.097692 0.000024  0.476997 0.000026  I-0.0969100 0.0000066 -0.3318 0.0047  I  -105.740    0.803    -9.494    0.034  0.097691  0.476906 -0.0969126  -105.734    -9.493  
+22 5 5 59704.00 I  0.099821 0.000024  0.477829 0.000027  I-0.0965002 0.0000065 -0.4648 0.0047  I  -105.760    0.803    -9.532    0.034  0.099882  0.477903 -0.0964992  -105.770    -9.526  
+22 5 6 59705.00 I  0.101673 0.000024  0.478907 0.000026  I-0.0960205 0.0000066 -0.4776 0.0046  I  -105.730    0.803    -9.600    0.034  0.101687  0.478833 -0.0960256  -105.754    -9.581  
+22 5 7 59706.00 I  0.103385 0.000025  0.479460 0.000025  I-0.0955613 0.0000066 -0.4416 0.0046  I  -105.611    0.803    -9.787    0.034  0.103404  0.479538 -0.0955546  -105.646    -9.779  
+22 5 8 59707.00 I  0.105107 0.000024  0.480078 0.000027  I-0.0951513 0.0000064 -0.3637 0.0046  I  -105.317    0.823   -10.025    0.110  0.105117  0.480078 -0.0951550  -105.347   -10.030  
+22 5 9 59708.00 I  0.106696 0.000025  0.480494 0.000027  I-0.0948670 0.0000065 -0.1866 0.0045  I  -104.887    0.823   -10.186    0.110  0.106699  0.480537 -0.0949242  -104.904   -10.197  
+22 510 59709.00 I  0.108517 0.000019  0.481036 0.000018  I-0.0948000 0.0000062  0.0561 0.0040  I  -104.601    0.786   -10.242    0.154  0.108427  0.480933 -0.0948334  -104.607   -10.261  
+22 511 59710.00 I  0.110914 0.000019  0.481745 0.000028  I-0.0949934 0.0000046  0.3415 0.0039  I  -104.724    0.784   -10.269    0.175  0.110941  0.481776 -0.0950144  -104.732   -10.281  
+22 512 59711.00 I  0.113495 0.000018  0.482656 0.000028  I-0.0954568 0.0000047  0.5482 0.0035  I  -105.149    0.784   -10.278    0.175  0.113474  0.482707 -0.0954543  -105.174   -10.290  
+22 513 59712.00 I  0.116067 0.000018  0.483460 0.000028  I-0.0960590 0.0000052  0.6624 0.0038  I  -105.514    0.784   -10.142    0.175  0.116107  0.483379 -0.0960629  -105.566   -10.162  
+22 514 59713.00 I  0.118510 0.000014  0.483903 0.000023  I-0.0967479 0.0000060  0.6753 0.0039  I  -105.714    0.783    -9.781    0.191  0.118527  0.483975 -0.0967431  -105.773    -9.799  
+22 515 59714.00 I  0.120715 0.000021  0.484487 0.000032  I-0.0973706 0.0000059  0.5710 0.0043  I  -106.022    0.853    -9.383    0.166  0.120799  0.484444 -0.0973670  -106.086    -9.399  
+22 516 59715.00 I  0.122299 0.000022  0.485261 0.000032  I-0.0978725 0.0000061  0.4144 0.0054  I  -106.587    0.853    -9.262    0.166  0.122385  0.485333 -0.0978659  -106.653    -9.281  
+22 517 59716.00 I  0.123264 0.000022  0.485918 0.000024  I-0.0981789 0.0000091  0.1963 0.0055  I  -107.086    0.963    -9.493    0.130  0.123240  0.485912 -0.0981728  -107.146    -9.513  
+22 518 59717.00 I  0.124656 0.000028  0.485620 0.000037  I-0.0982664 0.0000091 -0.0180 0.0065  I  -107.099    0.997    -9.832    0.133  0.124614  0.485666 -0.0982338  -107.148    -9.846  
+22 519 59718.00 I  0.126492 0.000027  0.485532 0.000037  I-0.0981548 0.0000092 -0.1965 0.0065  I  -106.634    0.997   -10.029    0.133  0.126492  0.485563 -0.0980742  -106.655   -10.034  
+22 520 59719.00 I  0.128441 0.000027  0.485687 0.000037  I-0.0979230 0.0000093 -0.2261 0.0070  I  -106.083    0.997   -10.073    0.133  0.128370  0.485536 -0.0979421  -106.062   -10.068  
+22 521 59720.00 I  0.130661 0.000022  0.485982 0.000031  I-0.0977430 0.0000105 -0.1346 0.0062  I  -105.784    1.070   -10.077    0.139  0.130677  0.486020 -0.0977739  -105.765   -10.071  
+22 522 59721.00 I  0.132973 0.000024  0.486767 0.000038  I-0.0976719 0.0000081  0.0111 0.0066  I  -105.760    0.848   -10.064    0.091  0.132949  0.486774 -0.0977075  -105.758   -10.059  
+22 523 59722.00 I  0.135353 0.000025  0.487341 0.000038  I-0.0977663 0.0000079  0.1602 0.0055  I  -105.829    0.848    -9.980    0.091  0.135359  0.487350 -0.0977582  -105.848    -9.982  
+22 524 59723.00 I  0.137675 0.000018  0.488221 0.000025  I-0.0979707 0.0000075  0.2447 0.0054  I  -105.844    0.782    -9.818    0.064  0.137703  0.488205 -0.0979698  -105.891    -9.829  
+22 525 59724.00 I  0.139651 0.000020  0.488506 0.000034  I-0.0982390 0.0000075  0.2792 0.0053  I  -105.827    0.831    -9.611    0.068  0.139642  0.488593 -0.0982642  -105.852    -9.614  
+22 526 59725.00 I  0.141660 0.000019  0.488483 0.000034  I-0.0984964 0.0000075  0.2155 0.0053  I  -105.917    0.831    -9.372    0.068  0.141637  0.488529 -0.0985094  -105.918    -9.361  
+22 527 59726.00 I  0.143578 0.000020  0.488526 0.000034  I-0.0986417 0.0000074  0.0667 0.0056  I  -106.168    0.831    -9.113    0.068  0.143638  0.488445 -0.0986407  -106.153    -9.084  
+22 528 59727.00 I  0.145155 0.000016  0.488332 0.000026  I-0.0986054 0.0000084 -0.1553 0.0056  I  -106.455    0.876    -8.932    0.072  0.145102  0.488400 -0.0986068  -106.467    -8.914  
+22 529 59728.00 I  0.146685 0.000015  0.488251 0.000025  I-0.0983125 0.0000083 -0.4331 0.0055  I  -106.618    0.876    -8.975    0.072  0.146706  0.488268 -0.0983314  -106.669    -8.976  
+22 530 59729.00 I  0.148142 0.000026  0.487978 0.000036  I-0.0977393 0.0000070 -0.7107 0.0053  I  -106.623    0.864    -9.282    0.057  0.148067  0.488086 -0.0977877  -106.716    -9.292  
+22 531 59730.00 I  0.149844 0.000025  0.487054 0.000027  I-0.0969106 0.0000065 -0.9298 0.0045  I  -106.562    0.840    -9.686    0.031  0.149795  0.487092 -0.0969563  -106.700    -9.703  
+22 6 1 59731.00 I  0.152000 0.000030  0.486286 0.000038  I-0.0959030 0.0000056 -1.0789 0.0045  I  -106.542    1.030    -9.952    0.050  0.151943  0.486170 -0.0959109  -106.731    -9.971  
+22 6 2 59732.00 I  0.154336 0.000030  0.485357 0.000037  I-0.0947797 0.0000062 -1.1474 0.0044  I  -106.621    1.030   -10.003    0.050  0.154357  0.485426 -0.0947757  -106.670   -10.005  
+22 6 3 59733.00 I  0.156607 0.000030  0.484864 0.000037  I-0.0936407 0.0000067 -1.1184 0.0048  I  -106.804    1.030    -9.972    0.050  0.156589  0.484781 -0.0936356  -106.660    -9.955  
+22 6 4 59734.00 I  0.158875 0.000030  0.484102 0.000037  I-0.0925699 0.0000074 -1.0083 0.0064  I  -106.996    1.030   -10.005    0.050  0.158889  0.484149 -0.0925602  -106.851    -9.984  
+22 6 5 59735.00 I  0.161159 0.000020  0.483633 0.000027  I-0.0916234 0.0000110 -0.9002 0.0056  I  -107.007    1.266   -10.075    0.066  0.161161  0.483622 -0.0916220  -106.921   -10.058  
+22 6 6 59736.00 I  0.163475 0.000027  0.483155 0.000031  I-0.0907778 0.0000085 -0.7673 0.0075  I  -106.756    0.996   -10.057    0.087  0.163382  0.483150 -0.0908246  -106.715   -10.044  
+22 6 7 59737.00 I  0.166256 0.000021  0.482820 0.000018  I-0.0901222 0.0000102 -0.5342 0.0062  I  -106.478    0.872    -9.931    0.096  0.166198  0.482812 -0.0901686  -106.474    -9.925  
+22 6 8 59738.00 I  0.169366 0.000026  0.482909 0.000037  I-0.0896769 0.0000090 -0.3985 0.0068  I  -106.547    0.889    -9.829    0.091  0.169346  0.482843 -0.0896819  -106.581    -9.834  
+22 6 9 59739.00 I  0.172337 0.000026  0.482810 0.000037  I-0.0893174 0.0000089 -0.2862 0.0062  I  -107.042    0.889    -9.826    0.091  0.172338  0.482895 -0.0893344  -107.056    -9.817  
+22 610 59740.00 I  0.175169 0.000026  0.482967 0.000037  I-0.0890922 0.0000084 -0.2109 0.0060  I  -107.668    0.889    -9.774    0.091  0.175150  0.482907 -0.0890843  -107.652    -9.745  
+22 611 59741.00 I  0.177826 0.000026  0.482590 0.000037  I-0.0888448 0.0000081 -0.2879 0.0056  I  -108.215    0.889    -9.495    0.091  0.177834  0.482720 -0.0888551  -108.201    -9.465  
+22 612 59742.00 I  0.180320 0.000023  0.482009 0.000040  I-0.0884905 0.0000073 -0.4424 0.0054  I  -108.808    0.779    -9.107    0.101  0.180290  0.482016 -0.0885165  -108.809    -9.083  
+22 613 59743.00 I  0.182803 0.000023  0.481188 0.000040  I-0.0879264 0.0000071 -0.6975 0.0051  I  -109.514    0.779    -8.964    0.101  0.182826  0.481258 -0.0879480  -109.531    -8.942  
+22 614 59744.00 I  0.185076 0.000015  0.480464 0.000023  I-0.0870865 0.0000072 -0.9795 0.0049  I  -109.993    0.724    -9.208    0.111  0.185100  0.480403 -0.0870940  -110.036    -9.188  
+22 615 59745.00 I  0.187070 0.000034  0.479241 0.000037  I-0.0859877 0.0000068 -1.2005 0.0050  I  -109.870    0.734    -9.587    0.125  0.187052  0.479331 -0.0859830  -109.873    -9.588  
+22 616 59746.00 I  0.189198 0.000034  0.478011 0.000037  I-0.0847345 0.0000068 -1.2746 0.0048  I  -109.272    0.734    -9.808    0.125  0.189149  0.478024 -0.0847332  -109.222    -9.837  
+22 617 59747.00 I  0.191613 0.000034  0.476766 0.000037  I-0.0834981 0.0000068 -1.1698 0.0058  I  -108.690    0.734    -9.874    0.125  0.191602  0.476728 -0.0834949  -108.594    -9.934  
+22 618 59748.00 I  0.194037 0.000032  0.475516 0.000030  I-0.0824293 0.0000093 -0.9619 0.0063  I  -108.460    0.898    -9.926    0.199  0.194019  0.475550 -0.0824189  -108.365    -9.983  
+22 619 59749.00 I  0.196592 0.000032  0.474529 0.000030  I-0.0815690 0.0000106 -0.7700 0.0059  I  -108.584    0.898    -9.932    0.199  0.196541  0.474534 -0.0815575  -108.509    -9.976  
+22 620 59750.00 I  0.199463 0.000034  0.473569 0.000035  I-0.0808708 0.0000072 -0.6337 0.0063  I  -108.896    0.835    -9.762    0.155  0.199454  0.473574 -0.0808812  -108.836    -9.796  
+22 621 59751.00 I  0.202395 0.000013  0.472801 0.000020  I-0.0802855 0.0000069 -0.5458 0.0047  I  -109.207    0.832    -9.441    0.148  0.202403  0.472799 -0.0803109  -109.153    -9.467  
+22 622 59752.00 I  0.205095 0.000018  0.472319 0.000024  I-0.0797453 0.0000060 -0.5596 0.0046  I  -109.400    0.719    -9.156    0.139  0.205128  0.472282 -0.0797589  -109.347    -9.174  
+22 623 59753.00 I  0.207617 0.000019  0.471572 0.000025  I-0.0791174 0.0000062 -0.7200 0.0043  I  -109.533    0.719    -9.018    0.139  0.207619  0.471645 -0.0791011  -109.587    -9.025  
+22 624 59754.00 I  0.210140 0.000019  0.470821 0.000025  I-0.0782998 0.0000063 -0.8969 0.0045  I  -109.766    0.719    -8.977    0.139  0.210148  0.470821 -0.0782976  -109.961    -8.971  
+22 625 59755.00 I  0.212734 0.000020  0.469671 0.000025  I-0.0773292 0.0000064 -1.0569 0.0046  I  -110.124    0.719    -8.981    0.139  0.212693  0.469719 -0.0773260  -110.305    -8.982  
+22 626 59756.00 I  0.215402 0.000024  0.468458 0.000027  I-0.0761675 0.0000067 -1.2726 0.0047  I  -110.449    0.715    -9.097    0.145  0.215376  0.468485 -0.0761726  -110.571    -9.112  
+22 627 59757.00 I  0.218221 0.000024  0.467007 0.000026  I-0.0748089 0.0000069 -1.4138 0.0054  I  -110.584    0.715    -9.400    0.145  0.218164  0.467038 -0.0748406  -110.659    -9.428  
+22 628 59758.00 I  0.221334 0.000020  0.465664 0.000023  I-0.0733568 0.0000085 -1.5042 0.0056  I  -110.546    0.907    -9.791    0.161  0.221330  0.465623 -0.0733645  -110.576    -9.834  
+22 629 59759.00 I  0.224405 0.000022  0.464119 0.000035  I-0.0718014 0.0000088 -1.5917 0.0063  I  -110.489    0.982   -10.034    0.135  0.224443  0.464165 -0.0718011  -110.473   -10.052  
+22 630 59760.00 I  0.227228 0.000021  0.462589 0.000035  I-0.0702026 0.0000093 -1.5914 0.0064  I  -110.549    0.982    -9.993    0.135  0.227220  0.462671 -0.0702118  -110.474    -9.975  
+22 7 1 59761.00 I  0.230016 0.000021  0.460917 0.000035  I-0.0686538 0.0000094 -1.4853 0.0081  I  -110.749    0.982    -9.779    0.135  0.230002  0.460818 -0.0686663  -110.599    -9.722  
+22 7 2 59762.00 I  0.232933 0.000011  0.459176 0.000029  I-0.0672366 0.0000132 -1.3654 0.0073  I  -111.003    1.080    -9.606    0.072  0.232881  0.459225 -0.0672447  -110.959    -9.582  
+22 7 3 59763.00 I  0.236097 0.000015  0.457836 0.000038  I-0.0659447 0.0000112 -1.1804 0.0086  I  -111.152    0.913    -9.542    0.143  0.236109  0.457809 -0.0659625  -111.150    -9.536  
+22 7 4 59764.00 I  0.239192 0.000014  0.456518 0.000038  I-0.0649095 0.0000110 -0.8941 0.0074  I  -111.086    0.913    -9.489    0.143  0.239234  0.456579 -0.0649159  -111.121    -9.498  
+22 7 5 59765.00 I  0.241892 0.000014  0.455215 0.000034  I-0.0641385 0.0000096 -0.6617 0.0071  I  -110.905    0.851    -9.366    0.185  0.241892  0.455171 -0.0641393  -110.976    -9.390  
+22 7 6 59766.00 I  0.244459 0.000014  0.453233 0.000034  I-0.0635508 0.0000090 -0.5352 0.0066  I  -110.908    0.851    -9.242    0.185  0.244450  0.453302 -0.0635337  -110.950    -9.262  
+22 7 7 59767.00 I  0.247123 0.000014  0.451687 0.000034  I-0.0630483 0.0000090 -0.4680 0.0063  I  -111.302    0.851    -9.212    0.185  0.247124  0.451582 -0.0630501  -111.305    -9.226  
+22 7 8 59768.00 I  0.249745 0.000014  0.450070 0.000035  I-0.0625850 0.0000089 -0.4900 0.0065  I  -111.986    0.851    -9.221    0.185  0.249756  0.450120 -0.0625785  -111.978    -9.228  
+22 7 9 59769.00 I  0.252293 0.000011  0.448667 0.000026  I-0.0620259 0.0000094 -0.6391 0.0054  I  -112.729    0.943    -9.129    0.218  0.252297  0.448682 -0.0620271  -112.723    -9.129  
+22 710 59770.00 I  0.254694 0.000017  0.447033 0.000028  I-0.0612786 0.0000060 -0.8727 0.0057  I  -113.425    0.796    -8.964    0.149  0.254733  0.447060 -0.0612967  -113.423    -8.960  
+22 711 59771.00 I  0.256802 0.000016  0.445382 0.000019  I-0.0602832 0.0000066 -1.0982 0.0045  I  -113.995    0.755    -8.945    0.115  0.256857  0.445395 -0.0603249  -114.007    -8.936  
+22 712 59772.00 I  0.258322 0.000016  0.443981 0.000019  I-0.0591150 0.0000066 -1.2252 0.0049  I  -114.213    0.755    -9.158    0.115  0.258411  0.443974 -0.0591324  -114.246    -9.142  
+22 713 59773.00 I  0.259222 0.000017  0.442010 0.000025  I-0.0578239 0.0000072 -1.3788 0.0049  I  -113.935    0.783    -9.395    0.154  0.259174  0.442066 -0.0577813  -113.960    -9.403  
+22 714 59774.00 I  0.260256 0.000017  0.439903 0.000024  I-0.0564317 0.0000073 -1.3096 0.0052  I  -113.405    0.783    -9.444    0.154  0.260201  0.439888 -0.0564587  -113.418    -9.484  
+22 715 59775.00 I  0.261703 0.000017  0.438186 0.000024  I-0.0552591 0.0000074 -1.0771 0.0066  I  -113.034    0.783    -9.394    0.154  0.261642  0.438122 -0.0552630  -113.037    -9.466  
+22 716 59776.00 I  0.263452 0.000013  0.436323 0.000021  I-0.0542689 0.0000110 -0.8702 0.0056  I  -112.981    0.857    -9.438    0.216  0.263441  0.436373 -0.0542876  -112.983    -9.496  
+22 717 59777.00 I  0.265296 0.000017  0.434386 0.000022  I-0.0535129 0.0000084 -0.6806 0.0069  I  -113.167    0.907    -9.519    0.145  0.265267  0.434398 -0.0535228  -113.161    -9.544  
+22 718 59778.00 I  0.267260 0.000018  0.432324 0.000021  I-0.0528768 0.0000083 -0.5837 0.0057  I  -113.524    0.907    -9.408    0.145  0.267234  0.432352 -0.0528927  -113.506    -9.398  
+22 719 59779.00 I  0.269240 0.000018  0.430321 0.000012  I-0.0523099 0.0000076 -0.5937 0.0056  I  -113.990    0.933    -9.085    0.075  0.269260  0.430298 -0.0523068  -113.947    -9.037  
+22 720 59780.00 I  0.270985 0.000026  0.428180 0.000027  I-0.0516585 0.0000074 -0.6963 0.0054  I  -114.395    0.857    -8.814    0.130  0.270974  0.428173 -0.0516628  -114.393    -8.784  
+22 721 59781.00 I  0.272566 0.000027  0.426236 0.000027  I-0.0509072 0.0000076 -0.8291 0.0053  I  -114.621    0.857    -8.807    0.130  0.272574  0.426255 -0.0508922  -114.674    -8.805  
+22 722 59782.00 I  0.274101 0.000027  0.424534 0.000028  I-0.0499780 0.0000075 -1.0288 0.0060  I  -114.773    0.857    -8.993    0.130  0.274053  0.424453 -0.0499591  -114.884    -9.018  
+22 723 59783.00 I  0.275662 0.000024  0.422636 0.000027  I-0.0488588 0.0000093 -1.2010 0.0056  I  -115.013    0.708    -9.183    0.183  0.275681  0.422673 -0.0488673  -115.096    -9.210  
+22 724 59784.00 I  0.277054 0.000025  0.420927 0.000034  I-0.0475836 0.0000082 -1.3506 0.0062  I  -115.302    0.799    -9.322    0.190  0.277006  0.420915 -0.0476028  -115.333    -9.343  
+22 725 59785.00 I  0.278485 0.000025  0.419304 0.000035  I-0.0461801 0.0000082 -1.4329 0.0062  I  -115.469    0.799    -9.504    0.190  0.278471  0.419285 -0.0462003  -115.452    -9.519  
+22 726 59786.00 I  0.279854 0.000015  0.417978 0.000024  I-0.0447424 0.0000093 -1.4416 0.0060  I  -115.459    0.892    -9.758    0.202  0.279867  0.417962 -0.0447491  -115.399    -9.768  
+22 727 59787.00 I  0.281073 0.000025  0.416094 0.000039  I-0.0432971 0.0000088 -1.4499 0.0068  I  -115.382    0.892    -9.944    0.202  0.281044  0.416126 -0.0432579  -115.379    -9.934  
+22 728 59788.00 I  0.282268 0.000025  0.414126 0.000039  I-0.0418445 0.0000100 -1.4525 0.0073  I  -115.353    0.892    -9.901    0.202  0.282267  0.414205 -0.0417953  -115.431    -9.867  
+22 729 59789.00 I  0.283369 0.000024  0.411945 0.000038  I-0.0404251 0.0000117 -1.3560 0.0098  I  -115.381    0.892    -9.653    0.202  0.283345  0.411841 -0.0404282  -115.538    -9.595  
+22 730 59790.00 I  0.284623 0.000023  0.409371 0.000033  I-0.0391786 0.0000168 -1.1211 0.0097  I  -115.415    0.322    -9.394    0.160  0.284587  0.409400 -0.0392089  -115.593    -9.353  
+22 731 59791.00 I  0.285988 0.000034  0.407309 0.000040  I-0.0381710 0.0000156 -0.9219 0.0115  I  -115.418    0.796    -9.280    0.318  0.286000  0.407286 -0.0381849  -115.593    -9.273  
+22 8 1 59792.00 I  0.287131 0.000034  0.405160 0.000040  I-0.0373395 0.0000156 -0.7086 0.0098  I  -115.369    0.796    -9.289    0.318  0.287161  0.405194 -0.0373892  -115.536    -9.320  
+22 8 2 59793.00 I  0.287882 0.000028  0.403351 0.000030  I-0.0367458 0.0000120 -0.5192 0.0097  I  -115.284    0.762    -9.303    0.284  0.287882  0.403262 -0.0367846  -115.439    -9.376  
+22 8 3 59794.00 I  0.288544 0.000029  0.400939 0.000030  I-0.0362599 0.0000117 -0.4532 0.0081  I  -115.273    0.762    -9.263    0.284  0.288468  0.401019 -0.0362792  -115.414    -9.314  
+22 8 4 59795.00 I  0.289525 0.000029  0.398767 0.000029  I-0.0358141 0.0000110 -0.4630 0.0079  I  -115.510    0.762    -9.205    0.284  0.289489  0.398709 -0.0358145  -115.635    -9.222  
+22 8 5 59796.00 I  0.290539 0.000029  0.396534 0.000029  I-0.0353154 0.0000107 -0.5284 0.0066  I  -116.063    0.762    -9.176    0.284  0.290582  0.396579 -0.0353263  -116.154    -9.192  
+22 8 6 59797.00 I  0.291094 0.000015  0.394203 0.000017  I-0.0347291 0.0000074 -0.6785 0.0060  I  -116.788    0.736    -9.177    0.244  0.291080  0.394221 -0.0347316  -116.838    -9.204  
+22 8 7 59798.00 I  0.291546 0.000022  0.391643 0.000020  I-0.0339358 0.0000056 -0.8965 0.0051  I  -117.423    0.716    -9.224    0.251  0.291487  0.391652 -0.0339451  -117.435    -9.261  
+22 8 8 59799.00 I  0.292337 0.000021  0.389012 0.000014  I-0.0329625 0.0000070 -1.0355 0.0045  I  -117.732    0.707    -9.356    0.256  0.292293  0.389056 -0.0329721  -117.715    -9.399  
+22 8 9 59800.00 I  0.293207 0.000021  0.386258 0.000013  I-0.0318899 0.0000071 -1.0994 0.0046  I  -117.614    0.707    -9.521    0.256  0.293211  0.386232 -0.0318918  -117.585    -9.565  
+22 810 59801.00 I  0.293834 0.000023  0.383239 0.000025  I-0.0308023 0.0000059 -1.0476 0.0048  I  -117.209    0.739    -9.544    0.271  0.293803  0.383250 -0.0308088  -117.149    -9.591  
+22 811 59802.00 I  0.294451 0.000023  0.380323 0.000026  I-0.0298462 0.0000064 -0.8412 0.0045  I  -116.855    0.739    -9.347    0.271  0.294459  0.380298 -0.0298577  -116.770    -9.397  
+22 812 59803.00 I  0.295059 0.000023  0.377876 0.000026  I-0.0291298 0.0000067 -0.6051 0.0052  I  -116.787    0.739    -9.113    0.271  0.295055  0.377755 -0.0291384  -116.681    -9.171  
+22 813 59804.00 I  0.295579 0.000015  0.375683 0.000025  I-0.0286213 0.0000083 -0.4130 0.0051  I  -116.918    0.775    -9.085    0.284  0.295537  0.375740 -0.0286307  -116.834    -9.134  
+22 814 59805.00 I  0.296372 0.000014  0.373576 0.000025  I-0.0282774 0.0000076 -0.2999 0.0054  I  -117.059    0.775    -9.225    0.284  0.296313  0.373591 -0.0282983  -117.006    -9.266  
+22 815 59806.00 I  0.297512 0.000016  0.371305 0.000029  I-0.0279768 0.0000068 -0.3208 0.0068  I  -117.234    0.763    -9.267    0.243  0.297500  0.371314 -0.0279699  -117.203    -9.307  
+22 816 59807.00 I  0.298550 0.000014  0.369031 0.000020  I-0.0276026 0.0000112 -0.4412 0.0068  I  -117.579    0.739    -9.095    0.156  0.298583  0.369059 -0.0276395  -117.555    -9.139  
+22 817 59808.00 I  0.299278 0.000021  0.366802 0.000029  I-0.0270777 0.0000118 -0.6117 0.0082  I  -118.035    0.739    -8.900    0.156  0.299254  0.366732 -0.0270866  -118.003    -8.949  
+22 818 59809.00 I  0.299909 0.000021  0.364360 0.000029  I-0.0263509 0.0000119 -0.8670 0.0084  I  -118.387    0.739    -8.906    0.156  0.299866  0.364425 -0.0263517  -118.274    -8.865  
+22 819 59810.00 I  0.300904 0.000021  0.362096 0.000029  I-0.0253533 0.0000120 -1.0936 0.0086  I  -118.557    0.739    -9.087    0.156  0.300823  0.362010 -0.0253455  -118.335    -8.928  
+22 820 59811.00 I  0.302126 0.000021  0.359723 0.000029  I-0.0241783 0.0000125 -1.2766 0.0088  I  -118.646    0.739    -9.236    0.156  0.302176  0.359779 -0.0241871  -118.439    -9.105  
+22 821 59812.00 I  0.303009 0.000022  0.357442 0.000037  I-0.0228204 0.0000128 -1.3987 0.0089  I  -118.711    0.583    -9.251    0.088  0.302992  0.357455 -0.0228266  -118.572    -9.196  
+22 822 59813.00 I  0.303768 0.000022  0.354897 0.000037  I-0.0214092 0.0000127 -1.4359 0.0084  I  -118.688    0.583    -9.228    0.088  0.303769  0.354926 -0.0213929  -118.632    -9.243  
+22 823 59814.00 I  0.304481 0.000015  0.352582 0.000031  I-0.0199839 0.0000110 -1.3673 0.0071  I  -118.541    0.583    -9.300    0.088  0.304513  0.352500 -0.0199836  -118.587    -9.375  
+22 824 59815.00 I  0.304887 0.000016  0.349859 0.000037  I-0.0186814 0.0000065 -1.2785 0.0064  I  -118.346    0.652    -9.436    0.123  0.304896  0.349874 -0.0186613  -118.307    -9.531  
+22 825 59816.00 I  0.305185 0.000015  0.347444 0.000037  I-0.0174153 0.0000066 -1.2246 0.0044  I  -118.187    0.652    -9.478    0.123  0.305201  0.347486 -0.0174037  -118.023    -9.577  
+22 826 59817.00 I  0.305353 0.000014  0.345001 0.000037  I-0.0162761 0.0000059 -1.0389 0.0044  I  -118.052    0.652    -9.337    0.123  0.305398  0.344912 -0.0162851  -117.767    -9.438  
+22 827 59818.00 I  0.305270 0.000010  0.342297 0.000024  I-0.0153423 0.0000057 -0.8389 0.0043  I  -117.902    0.898    -9.106    0.171  0.305290  0.342335 -0.0153482  -117.637    -9.193  
+22 828 59819.00 I  0.304966 0.000019  0.339930 0.000030  I-0.0146069 0.0000063 -0.6130 0.0044  I  -117.764    0.774    -8.964    0.186  0.304974  0.339946 -0.0146136  -117.565    -9.035  
+22 829 59820.00 I  0.304625 0.000019  0.337374 0.000029  I-0.0141121 0.0000066 -0.3995 0.0049  I  -117.692    0.774    -8.995    0.186  0.304586  0.337401 -0.0140968  -117.551    -9.055  
+22 830 59821.00 I  0.304494 0.000019  0.335049 0.000020  I-0.0137905 0.0000075 -0.2380 0.0043  I  -117.681    0.736    -9.122    0.195  0.304464  0.334971 -0.0137838  -117.601    -9.176  
+22 831 59822.00 I  0.304616 0.000021  0.332698 0.000024  I-0.0136131 0.0000054 -0.1454 0.0047  I  -117.698    0.747    -9.208    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
+22 9 1 59823.00 I  0.304752 0.000021  0.330389 0.000024  I-0.0134602 0.0000056 -0.1711 0.0042  I  -117.799    0.747    -9.188    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
+22 9 2 59824.00 I  0.304504 0.000021  0.327695 0.000024  I-0.0132440 0.0000064 -0.2773 0.0043  I  -118.087    0.747    -9.109    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
+22 9 3 59825.00 I  0.304209 0.000012  0.325025 0.000015  I-0.0128866 0.0000064 -0.4403 0.0043  I  -118.530    0.757    -9.073    0.134  0.304186  0.324993 -0.0128821  -118.590    -9.080  
+22 9 4 59826.00 I  0.304086 0.000014  0.322772 0.000023  I-0.0123623 0.0000058 -0.6065 0.0043  I  -118.885    0.735    -9.140    0.190  0.304085  0.322764 -0.0123741  -118.929    -9.170  
+22 9 5 59827.00 I  0.303787 0.000014  0.320435 0.000023  I-0.0117020 0.0000058 -0.6873 0.0060  I  -118.883    0.735    -9.276    0.190  0.303820  0.320481 -0.0117203  -118.916    -9.328  
+22 9 6 59828.00 I  0.303227 0.000012  0.318033 0.000019  I-0.0110167 0.0000104 -0.6810 0.0050  I  -118.484    0.709    -9.345    0.245  0.303248  0.318029 -0.0110190  -118.525    -9.426  
+22 9 7 59829.00 I  0.302620 0.000014  0.314894 0.000027  I-0.0103855 0.0000082 -0.5380 0.0064  I  -117.956    0.865    -9.204    0.195  0.302652  0.314951 -0.0103738  -117.930    -9.248  
+22 9 8 59830.00 I  0.301725 0.000015  0.311753 0.000027  I-0.0099746 0.0000075 -0.2931 0.0059  I  -117.660    0.865    -8.859    0.195  0.301793  0.311758 -0.0099952  -117.557    -8.853  
+22 9 9 59831.00 I  0.300342 0.000016  0.308744 0.000029  I-0.0098010 0.0000085 -0.0431 0.0061  I  -117.717    0.865    -8.517    0.195  0.300297  0.308670 -0.0098037  -117.537    -8.461  
+22 910 59832.00 I  0.299160 0.000014  0.305635 0.000023  I-0.0098892 0.0000096  0.2094 0.0057  I  -117.914    1.166    -8.404    0.074  0.299086  0.305665 -0.0098938  -117.785    -8.354  
+22 911 59833.00 I  0.298571 0.000024  0.302860 0.000034  I-0.0101811 0.0000077  0.3460 0.0062  I  -117.993    0.970    -8.521    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
+22 912 59834.00 I  0.298129 0.000024  0.300249 0.000034  I-0.0105451 0.0000079  0.3744 0.0061  I  -117.974    0.970    -8.669    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
+22 913 59835.00 I  0.297553 0.000024  0.298016 0.000031  I-0.0108732 0.0000094  0.2329 0.0056  I  -118.082    0.886    -8.702    0.168  0.297509  0.297897 -0.0108687  -118.179    -8.722  
+22 914 59836.00 I  0.296978 0.000025  0.295772 0.000049  I-0.0109857 0.0000078  0.0159 0.0061  I  -118.400    0.902    -8.680    0.136  0.296992  0.295809 -0.0110048  -118.515    -8.694  
+22 915 59837.00 I  0.296334 0.000024  0.293794 0.000048  I-0.0108932 0.0000079 -0.2364 0.0055  I  -118.754    0.902    -8.730    0.136  0.296326  0.293853 -0.0109071  -118.881    -8.735  
+22 916 59838.00 I  0.295607 0.000024  0.291776 0.000048  I-0.0105233 0.0000078 -0.4575 0.0059  I  -118.926    0.902    -8.848    0.136  0.295633  0.291666 -0.0105453  -119.064    -8.840  
+22 917 59839.00 I  0.294744 0.000015  0.289567 0.000041  I-0.0099856 0.0000088 -0.6564 0.0056  I  -118.849    0.928    -8.900    0.088  0.294765  0.289613 -0.0099966  -118.954    -8.905  
+22 918 59840.00 I  0.293577 0.000019  0.287802 0.000054  I-0.0092294 0.0000081 -0.7986 0.0059  I  -118.591    0.988    -8.822    0.130  0.293594  0.287789 -0.0092502  -118.640    -8.844  
+22 919 59841.00 I  0.292284 0.000019  0.285822 0.000053  I-0.0084297 0.0000079 -0.8171 0.0059  I  -118.237    0.988    -8.710    0.130  0.292235  0.285928 -0.0084134  -118.223    -8.750  
+22 920 59842.00 I  0.291352 0.000018  0.283591 0.000037  I-0.0075714 0.0000086 -0.9071 0.0051  I  -117.863    1.078    -8.710    0.170  0.291284  0.283515 -0.0075559  -117.778    -8.771  
+22 921 59843.00 I  0.290658 0.000019  0.281017 0.000039  I-0.0066715 0.0000064 -0.8290 0.0052  I  -117.562    0.957    -8.833    0.126  0.290675  0.281089 -0.0066950  -117.531    -8.864  
+22 922 59844.00 I  0.289762 0.000019  0.278371 0.000038  I-0.0059625 0.0000060 -0.6035 0.0046  I  -117.391    0.957    -8.934    0.126  0.289785  0.278400 -0.0059969  -117.441    -8.921  
+22 923 59845.00 I  0.288623 0.000018  0.275583 0.000039  I-0.0054439 0.0000065 -0.4398 0.0046  I  -117.331    0.957    -8.873    0.126  0.288673  0.275532 -0.0054471  -117.457    -8.810  
+22 924 59846.00 I  0.287261 0.000014  0.272920 0.000015  I-0.0050916 0.0000071 -0.2501 0.0048  I  -117.326    0.805    -8.661    0.027  0.287244  0.272949 -0.0051006  -117.468    -8.622  
+22 925 59847.00 I  0.285950 0.000025  0.270442 0.000035  I-0.0049405 0.0000070 -0.0699 0.0050  I  -117.349    0.769    -8.451    0.192  0.285878  0.270404 -0.0049635  -117.484    -8.457  
+22 926 59848.00 I  0.285166 0.000025  0.268138 0.000034  I-0.0049423 0.0000071  0.0818 0.0057  I  -117.406    0.769    -8.388    0.192  0.285103  0.268121 -0.0049793  -117.537    -8.441  
+22 927 59849.00 I  0.284709 0.000024  0.266516 0.000032  I-0.0050966 0.0000089  0.2109 0.0053  I  -117.484    0.744    -8.488    0.260  0.284746  0.266357 -0.0051012  -117.616    -8.597  
+22 928 59850.00 I  0.283877 0.000025  0.264882 0.000033  I-0.0053042 0.0000079  0.1602 0.0058  I  -117.554    0.670    -8.634    0.185  0.283878  0.264953 -0.0053014  -117.693    -8.702  
+22 929 59851.00 I  0.283007 0.000025  0.263313 0.000033  I-0.0053854 0.0000074  0.0148 0.0053  I  -117.617    0.670    -8.699    0.185  0.282943  0.263319 -0.0054180  -117.779    -8.707  
+22 930 59852.00 I  0.282322 0.000024  0.261526 0.000033  I-0.0053250 0.0000071 -0.1570 0.0051  I  -117.701    0.670    -8.656    0.185  0.282338  0.261528 -0.0053388  -117.905    -8.603  
+2210 1 59853.00 I  0.281361 0.000013  0.259737 0.000015  I-0.0050433 0.0000069 -0.4129 0.0049  I  -117.771    0.566    -8.579    0.031  0.281388  0.259744 -0.0049041  -117.934    -8.536  
+2210 2 59854.00 I  0.280043 0.000011  0.257886 0.000015  I-0.0045474 0.0000067 -0.5240 0.0043  I  -117.700    0.566    -8.555    0.031  0.280092  0.257931 -0.0043864  -117.763    -8.633  
+2210 3 59855.00 I  0.278450 0.000017  0.255735 0.000018  I-0.0040462 0.0000051 -0.4823 0.0044  I  -117.362    0.918    -8.587    0.135  0.278478  0.255746 -0.0040146  -117.380    -8.681  
+2210 4 59856.00 I  0.276548 0.000016  0.253507 0.000016  I-0.0035886 0.0000057 -0.4232 0.0034  I  -116.792    1.082    -8.594    0.177  0.276607  0.253527 -0.0035590  -116.777    -8.672  
+2210 5 59857.00 I  0.274392 0.000017  0.251464 0.000021  I-0.0032267 0.0000044 -0.2836 0.0038  I  -116.216    1.068    -8.481    0.157  0.274352  0.251450 -0.0032281  -116.158    -8.550  
+2210 6 59858.00 I  0.272446 0.000021  0.249202 0.000022  I-0.0030613 0.0000049 -0.0244 0.0035  I  -115.894    1.068    -8.245    0.157  0.272409  0.249284 -0.0030816  -115.892    -8.306  
+2210 7 59859.00 I  0.270890 0.000023  0.246768 0.000020  I-0.0031814 0.0000055  0.2454 0.0037  I  -115.901    1.068    -7.990    0.157  0.270869  0.246728 -0.0031810  -115.963    -8.047  
+2210 8 59860.00 I  0.269392 0.000023  0.244256 0.000020  I-0.0035334 0.0000056  0.4593 0.0043  I  -116.075    1.068    -7.832    0.157  0.269464  0.244272 -0.0035337  -116.181    -7.889  
+2210 9 59861.00 I  0.267405 0.000018  0.242156 0.000017  I-0.0040709 0.0000067  0.5859 0.0039  I  -116.191    1.055    -7.793    0.132  0.267436  0.242181 -0.0040628  -116.323    -7.852  
+221010 59862.00 I  0.265325 0.000021  0.239989 0.000018  I-0.0046592 0.0000055  0.5744 0.0048  I  -116.181    0.930    -7.811    0.107  0.265240  0.239987 -0.0046541  -116.330    -7.871  
+221011 59863.00 I  0.263669 0.000020  0.237862 0.000011  I-0.0051762 0.0000069  0.4322 0.0041  I  -116.177    0.772    -7.838    0.071  0.263701  0.237885 -0.0051692  -116.344    -7.899  
+221012 59864.00 I  0.262028 0.000021  0.235769 0.000012  I-0.0054969 0.0000060  0.2098 0.0046  I  -116.323    0.827    -7.890    0.053  0.262046  0.235701 -0.0055011  -116.517    -7.950  
+221013 59865.00 I  0.259882 0.000019  0.233754 0.000012  I-0.0055875 0.0000062 -0.0376 0.0044  I  -116.581    0.827    -7.985    0.053  0.260021  0.233734 -0.0055722  -116.707    -8.023  
+221014 59866.00 I  0.256982 0.000019  0.232122 0.000011  I-0.0054408 0.0000064 -0.2277 0.0045  I  -116.749    0.827    -8.072    0.053  0.256936  0.232102 -0.0054362  -116.793    -8.078  
+221015 59867.00 I  0.254058 0.000019  0.230349 0.000011  I-0.0051764 0.0000064 -0.2850 0.0044  I  -116.645    0.827    -8.072    0.053  0.254063  0.230356 -0.0051876  -116.700    -8.075  
+221016 59868.00 I  0.251193 0.000020  0.228850 0.000025  I-0.0048938 0.0000059 -0.2732 0.0043  I  -116.260    0.986    -7.981    0.107  0.251206  0.228893 -0.0049099  -116.365    -7.987  
+221017 59869.00 I  0.248067 0.000023  0.227215 0.000026  I-0.0046590 0.0000058 -0.1745 0.0043  I  -115.731    0.986    -7.905    0.107  0.248052  0.227286 -0.0046783  -115.804    -7.935  
+221018 59870.00 I  0.245186 0.000019  0.225195 0.000026  I-0.0045591 0.0000062 -0.0330 0.0041  I  -115.203    1.037    -7.949    0.141  0.245102  0.225158 -0.0045660  -115.200    -8.015  
+221019 59871.00 I  0.243016 0.000022  0.222914 0.000030  I-0.0045886 0.0000058  0.0954 0.0042  I  -114.763    1.061    -8.091    0.163  0.243041  0.222898 -0.0045814  -114.747    -8.164  
+221020 59872.00 I  0.240707 0.000023  0.221149 0.000030  I-0.0047679 0.0000057  0.2777 0.0040  I  -114.469    1.061    -8.189    0.163  0.240817  0.221191 -0.0047645  -114.446    -8.265  
+221021 59873.00 I  0.237715 0.000023  0.219364 0.000030  I-0.0051485 0.0000055  0.4735 0.0053  I  -114.391    1.061    -8.113    0.163  0.237688  0.219313 -0.0051434  -114.344    -8.197  
+221022 59874.00 I  0.234654 0.000021  0.217508 0.000019  I-0.0057167 0.0000089  0.6746 0.0045  I  -114.551    1.092    -7.857    0.192  0.234606  0.217522 -0.0057243  -114.532    -7.927  
+221023 59875.00 I  0.232018 0.000021  0.216040 0.000022  I-0.0065038 0.0000072  0.8940 0.0058  I  -114.849    0.936    -7.538    0.157  0.231878  0.216031 -0.0064986  -114.866    -7.589  
+221024 59876.00 I  0.230034 0.000022  0.214631 0.000022  I-0.0074597 0.0000073  0.9785 0.0054  I  -115.109    0.936    -7.306    0.157  0.230043  0.214645 -0.0074339  -115.163    -7.341  
+221025 59877.00 I  0.228132 0.000021  0.213272 0.000022  I-0.0084074 0.0000080  0.9027 0.0054  I  -115.225    0.811    -7.248    0.109  0.228137  0.213232 -0.0084121  -115.318    -7.265  
+221026 59878.00 I  0.226079 0.000021  0.211730 0.000022  I-0.0092409 0.0000079  0.7541 0.0056  I  -115.215    0.811    -7.354    0.109  0.226115  0.211747 -0.0092591  -115.297    -7.349  
+221027 59879.00 I  0.223694 0.000021  0.210442 0.000022  I-0.0098807 0.0000079  0.5008 0.0052  I  -115.158    0.811    -7.525    0.109  0.223756  0.210409 -0.0098856  -115.222    -7.492  
+221028 59880.00 I  0.220829 0.000019  0.208825 0.000022  I-0.0102288 0.0000068  0.2063 0.0061  I  -115.084    0.811    -7.641    0.109  0.220823  0.208832 -0.0102779  -115.143    -7.612  
+221029 59881.00 I  0.217712 0.000017  0.207412 0.000017  I-0.0103283 0.0000094  0.0167 0.0049  I  -114.960    0.852    -7.642    0.076  0.217709  0.207418 -0.0103958  -115.022    -7.628  
+221030 59882.00 I  0.214510 0.000027  0.206266 0.000021  I-0.0102926 0.0000070 -0.0818 0.0057  I  -114.743    0.859    -7.574    0.183  0.214473  0.206229 -0.0103095  -114.810    -7.575  
+221031 59883.00 I  0.211393 0.000025  0.205209 0.000014  I-0.0101979 0.0000063 -0.0806 0.0047  I  -114.422    0.863    -7.519    0.229  0.211345  0.205237 -0.0101927  -114.492    -7.538  
+2211 1 59884.00 I  0.208602 0.000025  0.204260 0.000017  I-0.0101862 0.0000063  0.0850 0.0040  I  -114.034    0.863    -7.499    0.229  0.208514  0.204211 -0.0101774  -114.100    -7.544  
+2211 2 59885.00 I  0.206231 0.000026  0.203464 0.000020  I-0.0104066 0.0000049  0.3665 0.0041  I  -113.657    0.879    -7.466    0.199  0.206235  0.203545 -0.0104065  -113.700    -7.501  
+2211 3 59886.00 I  0.203876 0.000027  0.202375 0.000020  I-0.0109408 0.0000052  0.7126 0.0035  I  -113.389    0.879    -7.375    0.199  0.203841  0.202359 -0.0109528  -113.392    -7.399  
+2211 4 59887.00 I  0.201539 0.000026  0.201384 0.000020  I-0.0118032 0.0000051  0.9730 0.0044  I  -113.302    0.879    -7.229    0.199  0.201477  0.201353 -0.0118134  -113.257    -7.249  
+2211 5 59888.00 I  0.199497 0.000015  0.200681 0.000016  I-0.0128130 0.0000070  1.0122 0.0034  I  -113.393    0.897    -7.050    0.158  0.199403  0.200700 -0.0128173  -113.353    -7.066  
+2211 6 59889.00 I  0.197923 0.000018  0.199805 0.000021  I-0.0138019 0.0000044  0.9743 0.0043  I  -113.557    0.733    -6.858    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
+2211 7 59890.00 I  0.196417 0.000019  0.198990 0.000019  I-0.0147289 0.0000051  0.8384 0.0036  I  -113.646    0.733    -6.684    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
+2211 8 59891.00 I  0.194595 0.000031  0.198441 0.000023  I-0.0154439 0.0000056  0.5982 0.0036  I  -113.613    0.653    -6.592    0.031  0.194574  0.198424 -0.0154466  -113.660    -6.582  
+2211 9 59892.00 I  0.192635 0.000031  0.197558 0.000023  I-0.0159449 0.0000052  0.4169 0.0038  I  -113.554    0.653    -6.639    0.031  0.192696  0.197558 -0.0159684  -113.571    -6.657  
+221110 59893.00 I  0.190363 0.000030  0.196704 0.000023  I-0.0162460 0.0000050  0.1406 0.0034  I  -113.581    0.653    -6.799    0.031  0.190367  0.196722 -0.0162302  -113.564    -6.849  
+221111 59894.00 I  0.187843 0.000030  0.195900 0.000023  I-0.0162279 0.0000043 -0.1304 0.0058  I  -113.653    0.653    -6.956    0.031  0.187822  0.195880 -0.0162520  -113.631    -7.013  
+221112 59895.00 I  0.185419 0.000028  0.195029 0.000018  I-0.0160393 0.0000105 -0.2391 0.0037  I  -113.603    0.322    -7.003    0.160  0.185361  0.195076 -0.0160839  -113.596    -7.056  
+221113 59896.00 I  0.183320 0.000030  0.193966 0.000021  I-0.0157699 0.0000061 -0.2871 0.0059  I  -113.340    0.725    -6.956    0.094  0.183217  0.193981 -0.0158151  -113.352    -6.999  
+221114 59897.00 I  0.181907 0.000014  0.192821 0.000013  I-0.0155034 0.0000055 -0.2201 0.0042  I  -112.932    0.725    -6.928    0.094  0.181786  0.192794 -0.0155444  -112.967    -6.958  
+221115 59898.00 I  0.181149 0.000015  0.192273 0.000014  I-0.0153471 0.0000058 -0.1008 0.0036  I  -112.493    0.725    -6.992    0.094  0.181089  0.192167 -0.0153549  -112.549    -7.008  
+221116 59899.00 I  0.180590 0.000016  0.192094 0.000020  I-0.0153097 0.0000046  0.0422 0.0038  I  -112.067    0.764    -7.082    0.132  0.180613  0.192084 -0.0153236  -112.120    -7.099  
+221117 59900.00 I  0.179830 0.000016  0.192242 0.000021  I-0.0154617 0.0000048  0.2757 0.0034  I  -111.700    0.764    -7.070    0.132  0.179894  0.192217 -0.0154871  -111.735    -7.093  
+221118 59901.00 I  0.178493 0.000016  0.192679 0.000022  I-0.0158540 0.0000049  0.4877 0.0039  I  -111.552    0.764    -6.902    0.132  0.178587  0.192658 -0.0158559  -111.559    -6.936  
+221119 59902.00 I  0.176649 0.000012  0.192913 0.000019  I-0.0164109 0.0000061  0.6210 0.0032  I  -111.773    0.805    -6.643    0.164  0.176631  0.192939 -0.0164100  -111.782    -6.671  
+221120 59903.00 I  0.174676 0.000015  0.192891 0.000022  I-0.0171026 0.0000040  0.7740 0.0036  I  -112.264    0.733    -6.381    0.154  0.174678  0.192941 -0.0171134  -112.283    -6.399  
+221121 59904.00 I  0.172507 0.000014  0.192675 0.000022  I-0.0179203 0.0000038  0.8110 0.0030  I  -112.721    0.733    -6.150    0.154  0.172482  0.192686 -0.0178985  -112.747    -6.164  
+221122 59905.00 I  0.170163 0.000014  0.192562 0.000016  I-0.0186682 0.0000044  0.6787 0.0027  I  -112.943    0.689    -5.986    0.147  0.170135  0.192562 -0.0186627  -112.985    -5.999  
+221123 59906.00 I  0.167913 0.000021  0.192096 0.000033  I-0.0192694 0.0000038  0.5214 0.0029  I  -112.979    0.712    -5.977    0.143  0.167864  0.192125 -0.0192839  -113.015    -5.992  
+221124 59907.00 I  0.165799 0.000021  0.191630 0.000033  I-0.0196788 0.0000039  0.2676 0.0029  I  -112.924    0.712    -6.159    0.143  0.165815  0.191634 -0.0196773  -112.960    -6.178  
+221125 59908.00 I  0.163383 0.000021  0.191487 0.000033  I-0.0198052 0.0000043  0.0155 0.0036  I  -112.760    0.712    -6.396    0.143  0.163449  0.191394 -0.0198119  -112.800    -6.422  
+221126 59909.00 I  0.160411 0.000020  0.191081 0.000031  I-0.0197330 0.0000061 -0.1670 0.0038  I  -112.469    0.748    -6.480    0.139  0.160439  0.191188 -0.0197408  -112.502    -6.504  
+221127 59910.00 I  0.156937 0.000020  0.190795 0.000031  I-0.0195087 0.0000062 -0.2369 0.0039  I  -112.157    0.748    -6.372    0.139  0.156985  0.190819 -0.0195486  -112.173    -6.392  
+221128 59911.00 I  0.153233 0.000021  0.190266 0.000034  I-0.0193093 0.0000047 -0.1563 0.0043  I  -111.944    0.805    -6.232    0.109  0.153168  0.190278 -0.0193141  -111.939    -6.246  
+221129 59912.00 I  0.149941 0.000015  0.189773 0.000016  I-0.0192201 0.0000059 -0.0036 0.0030  I  -111.820    0.870    -6.194    0.069  0.149881  0.189736 -0.0192085  -111.789    -6.198  
+221130 59913.00 I  0.147023 0.000020  0.189891 0.000021  I-0.0193122 0.0000036  0.1794 0.0033  I  -111.712    0.787    -6.215    0.109  0.146998  0.189837 -0.0193120  -111.648    -6.204  
+2212 1 59914.00 I  0.144056 0.000023  0.190049 0.000021  I-0.0195852 0.0000030  0.3812 0.0024  I  -111.605    0.787    -6.182    0.109  0.144039  0.190129 -0.0196037  -111.563    -6.191  
+2212 2 59915.00 I  0.141123 0.000024  0.190001 0.000020  I-0.0200266 0.0000032  0.4391 0.0021  I  -111.546    0.787    -6.068    0.109  0.141086  0.190030 -0.0200182  -111.557    -6.103  
+2212 3 59916.00 I  0.138502 0.000023  0.189600 0.000020  I-0.0204300 0.0000030  0.3969 0.0024  I  -111.575    0.787    -5.915    0.109  0.138520  0.189588 -0.0204483  -111.593    -5.954  
+2212 4 59917.00 I  0.135671 0.000024  0.189559 0.000018  I-0.0208093 0.0000035  0.3216 0.0024  I  -111.680    0.842    -5.751    0.139  0.135739  0.189603 -0.0208072  -111.696    -5.787  
+2212 5 59918.00 I  0.132717 0.000025  0.189087 0.000018  I-0.0210329 0.0000038  0.1256 0.0033  I  -111.752    0.842    -5.590    0.139  0.132595  0.189132 -0.0210271  -111.763    -5.625  
+2212 6 59919.00 I  0.130242 0.000022  0.188827 0.000013  I-0.0210514 0.0000057 -0.0977 0.0034  I  -111.682    0.994    -5.492    0.147  0.130234  0.188807 -0.0210546  -111.664    -5.528  
+2212 7 59920.00 I  0.127861 0.000023  0.188832 0.000018  I-0.0208448 0.0000056 -0.2990 0.0040  I  -111.505    0.846    -5.545    0.123  0.127804  0.188914 -0.0208636  -111.530    -5.568  
+2212 8 59921.00 I  0.125543 0.000022  0.188699 0.000018  I-0.0204734 0.0000057 -0.4404 0.0041  I  -111.365    0.846    -5.762    0.123  0.125550  0.188683 -0.0204842  -111.431    -5.765  
+2212 9 59922.00 I  0.123012 0.000021  0.188942 0.000018  I-0.0199675 0.0000060 -0.5715 0.0047  I  -111.344    0.846    -6.019    0.123  0.123051  0.188943 -0.0199575  -111.450    -5.997  
+221210 59923.00 I  0.120043 0.000019  0.189225 0.000015  I-0.0193441 0.0000075 -0.6617 0.0041  I  -111.356    0.679    -6.161    0.090  0.120023  0.189212 -0.0193465  -111.433    -6.148  
+221211 59924.00 I  0.117117 0.000024  0.189452 0.000023  I-0.0186822 0.0000056 -0.6376 0.0047  I  -111.266    0.747    -6.164    0.166  0.117059  0.189519 -0.0187186  -111.306    -6.171  
+221212 59925.00 I  0.114541 0.000023  0.189301 0.000023  I-0.0181000 0.0000057 -0.5202 0.0036  I  -111.037    0.747    -6.140    0.166  0.114474  0.189311 -0.0181257  -111.063    -6.164  
+221213 59926.00 I  0.112253 0.000019  0.189470 0.000023  I-0.0176358 0.0000045 -0.4209 0.0035  I  -110.703    0.861    -6.170    0.200  0.112235  0.189380 -0.0176371  -110.733    -6.213  
+221214 59927.00 I  0.110085 0.000019  0.189731 0.000022  I-0.0172744 0.0000042 -0.2729 0.0030  I  -110.284    0.861    -6.189    0.200  0.110057  0.189733 -0.0172887  -110.324    -6.215  
+221215 59928.00 I  0.107803 0.000020  0.190663 0.000022  I-0.0170970 0.0000039 -0.1039 0.0028  I  -109.840    0.861    -6.078    0.200  0.107848  0.190644 -0.0170929  -109.882    -6.084  
+221216 59929.00 I  0.105273 0.000020  0.191570 0.000022  I-0.0170756 0.0000038  0.0920 0.0032  I  -109.579    0.861    -5.849    0.200  0.105276  0.191662 -0.0170407  -109.642    -5.845  
+221217 59930.00 I  0.102628 0.000012  0.192140 0.000014  I-0.0172698 0.0000050  0.2544 0.0024  I  -109.724    0.909    -5.650    0.185  0.102588  0.192217 -0.0171383  -109.796    -5.644  
+221218 59931.00 I  0.100234 0.000028  0.192470 0.000032  I-0.0175335 0.0000029  0.2642 0.0029  I  -110.230    0.870    -5.565    0.145  0.100160  0.192490 -0.0173664  -110.291    -5.561  
+221219 59932.00 I  0.098290 0.000027  0.192738 0.000030  I-0.0177794 0.0000029  0.2176 0.0020  I  -110.790    0.836    -5.495    0.096  0.098210  0.192803 -0.0177187  -110.824    -5.496  
+221220 59933.00 I  0.096776 0.000032  0.193200 0.000033  I-0.0179621 0.0000027  0.1511 0.0021  I  -111.222    0.724    -5.338    0.100  0.096711  0.193084 -0.0179634  -111.212    -5.340  
+221221 59934.00 I  0.095784 0.000032  0.193309 0.000033  I-0.0180808 0.0000029  0.0821 0.0020  I  -111.621    0.724    -5.212    0.100  0.095777  0.193348 -0.0181234  -111.654    -5.239  
+221222 59935.00 I  0.094824 0.000032  0.194070 0.000034  I-0.0180953 0.0000029 -0.0800 0.0021  I  -112.006    0.724    -5.343    0.100  0.094877  0.193950 -0.0181060  -112.105    -5.394  
+221223 59936.00 I  0.093412 0.000033  0.194919 0.000034  I-0.0179113 0.0000031 -0.2707 0.0025  I  -112.108    0.724    -5.694    0.100  0.093472  0.194922 -0.0178955  -112.150    -5.759  
+221224 59937.00 I  0.091301 0.000022  0.196106 0.000018  I-0.0176045 0.0000040 -0.3096 0.0026  I  -111.756    0.564    -5.935    0.105  0.091397  0.196126 -0.0175841  -111.706    -6.007  
+221225 59938.00 I  0.088379 0.000022  0.197001 0.000018  I-0.0173382 0.0000041 -0.2103 0.0047  I  -111.221    0.564    -5.867    0.105  0.088402  0.197099 -0.0173115  -111.094    -5.943  
+221226 59939.00 I  0.085231 0.000044  0.197373 0.000036  I-0.0172380 0.0000086  0.0515 0.0046  I  -110.902    0.636    -5.663    0.134  0.085204  0.197391 -0.0172323  -110.709    -5.742  
+221227 59940.00 I  0.081994 0.000044  0.197755 0.000036  I-0.0174611 0.0000082  0.3732 0.0056  I  -110.867    0.636    -5.577    0.134  0.082060  0.197809 -0.0174541  -110.623    -5.660  
+221228 59941.00 I  0.078270 0.000046  0.198455 0.000037  I-0.0179249 0.0000071  0.5163 0.0054  I  -110.929    0.677    -5.586    0.138  0.078253  0.198379 -0.0179243  -110.647    -5.673  
+221229 59942.00 I  0.074738 0.000045  0.198550 0.000037  I-0.0184560 0.0000071  0.5464 0.0050  I  -110.989    0.677    -5.498    0.138  0.074744  0.198584 -0.0184719  -110.694    -5.570  
+221230 59943.00 I  0.071208 0.000045  0.199194 0.000037  I-0.0190009 0.0000071  0.5262 0.0051  I  -111.090    0.677    -5.286    0.138  0.071281  0.199199 -0.0190102  -110.793    -5.341  
+221231 59944.00 I  0.067041 0.000045  0.200093 0.000037  I-0.0194827 0.0000073  0.4288 0.0053  I  -111.251    0.677    -5.104    0.138  0.067074  0.200103 -0.0194855  -110.973    -5.182  
+23 1 1 59945.00 I  0.062785 0.000019  0.200912 0.000015  I-0.0198218 0.0000080  0.2211 0.0049  I  -111.416    0.730    -5.047    0.142  0.062699  0.200944 -0.0197967  -111.162    -5.163  
+23 1 2 59946.00 I  0.059055 0.000026  0.201762 0.000023  I-0.0199203 0.0000065 -0.0006 0.0058  I  -111.505    0.621    -5.057    0.096  0.059003  0.201796 -0.0199243  -111.443    -5.114  
+23 1 3 59947.00 I  0.055737 0.000027  0.202450 0.000033  I-0.0198267 0.0000083 -0.2042 0.0054  I  -111.438    0.659    -5.073    0.126  0.055638  0.202514 -0.0198250  -111.467    -5.128  
+23 1 4 59948.00 I  0.052972 0.000026  0.203064 0.000034  I-0.0195071 0.0000087 -0.4223 0.0063  I  -111.185    0.659    -5.151    0.126  0.052933  0.202990 -0.0195007  -111.313    -5.194  
+23 1 5 59949.00 I  0.050800 0.000027  0.203922 0.000034  I-0.0190229 0.0000095 -0.5179 0.0064  I  -110.842    0.659    -5.367    0.126  0.050795  0.203830 -0.0190232  -110.822    -5.531  
+23 1 6 59950.00 I  0.048797 0.000027  0.205049 0.000034  I-0.0184927 0.0000095 -0.5492 0.0066  I  -110.575    0.659    -5.652    0.126  0.048795  0.205101 -0.0184663  -110.510    -5.834  
+23 1 7 59951.00 I  0.046881 0.000026  0.206245 0.000034  I-0.0179427 0.0000093 -0.5259 0.0066  I  -110.448    0.659    -5.834    0.126  0.046853  0.206221 -0.0179143  -110.392    -5.984  
+23 1 8 59952.00 I  0.045143 0.000025  0.207582 0.000033  I-0.0174730 0.0000091 -0.4062 0.0062  I  -110.370    0.873    -5.828    0.183  0.045146  0.207590 -0.0174487  -110.316    -5.948  
+23 1 9 59953.00 I  0.043365 0.000018  0.209037 0.000021  I-0.0171385 0.0000082 -0.2617 0.0060  I  -110.219    0.866    -5.728    0.162  0.043370  0.209111 -0.0171274  -110.159    -5.821  
+23 110 59954.00 I  0.041291 0.000017  0.210318 0.000019  I-0.0169603 0.0000077 -0.0849 0.0055  I  -109.953    0.866    -5.662    0.162  0.041325  0.210288 -0.0169671  -109.874    -5.733  
+23 111 59955.00 I  0.038966 0.000025  0.211076 0.000021  I-0.0169675 0.0000073  0.0884 0.0050  I  -109.602    0.831    -5.626    0.138  0.038979  0.211134 -0.0169747  -109.583    -5.665  
+23 112 59956.00 I  0.036562 0.000024  0.211937 0.000020  I-0.0170926 0.0000064  0.1281 0.0050  I  -109.241    0.831    -5.526    0.138  0.036547  0.211915 -0.0170559  -109.296    -5.533  
+23 113 59957.00 I  0.034177 0.000024  0.213072 0.000020  I-0.0172135 0.0000069  0.1371 0.0064  I  -109.019    0.831    -5.366    0.138  0.034173  0.213022 -0.0172046  -109.147    -5.343  
+23 114 59958.00 I  0.031794 0.000019  0.214404 0.000013  I-0.0173724 0.0000112  0.1630 0.0058  I  -109.098    0.749    -5.298    0.079  0.031810  0.214393 -0.0173877  -109.253    -5.273  
+23 115 59959.00 I  0.029348 0.000027  0.216085 0.000025  I-0.0175381 0.0000094  0.1848 0.0074  I  -109.453    0.765    -5.412    0.122  0.029351  0.216047 -0.0175710  -109.621    -5.396  
+23 116 59960.00 I  0.026874 0.000027  0.217932 0.000026  I-0.0177154 0.0000098  0.1268 0.0073  I  -109.862    0.765    -5.571    0.122  0.026882  0.217923 -0.0177110  -110.037    -5.563  
+23 117 59961.00 I  0.024325 0.000021  0.220321 0.000024  I-0.0177447 0.0000113 -0.0721 0.0066  I  -110.227    0.772    -5.561    0.141  0.024343  0.220214 -0.0177400  -110.403    -5.564  
+23 118 59962.00 I  0.021690 0.000044  0.222404 0.000023  I-0.0175737 0.0000089 -0.2636 0.0071  I  -110.731    0.782    -5.436    0.127  0.021681  0.222504 -0.0175873  -110.857    -5.445  
+23 119 59963.00 I  0.019115 0.000044  0.224223 0.000023  I-0.0172335 0.0000087 -0.4072 0.0062  I  -111.419    0.782    -5.500    0.127  0.019078  0.224261 -0.0172362  -111.474    -5.516  
+23 120 59964.00 I  0.016659 0.000045  0.225643 0.000023  I-0.0167603 0.0000085 -0.5477 0.0068  I  -111.874    0.782    -5.863    0.127  0.016715  0.225678 -0.0167521  -111.849    -5.887  
+23 121 59965.00 I  0.013979 0.000041  0.226843 0.000009  I-0.0161645 0.0000104 -0.6089 0.0051  I  -111.665    0.801    -6.213    0.103  0.014033  0.226892 -0.0161896  -111.635    -6.235  
+23 122 59966.00 I  0.010876 0.000043  0.227751 0.000011  I-0.0156072 0.0000057 -0.4759 0.0058  I  -110.964    0.577    -6.218    0.090  0.010879  0.227740 -0.0156593  -110.964    -6.230  
+23 123 59967.00 I  0.007811 0.000043  0.228849 0.000013  I-0.0152578 0.0000053 -0.2077 0.0040  I  -110.347    0.577    -5.974    0.090  0.007728  0.228830 -0.0153087  -110.393    -5.970  
+23 124 59968.00 I  0.005404 0.000022  0.230244 0.000015  I-0.0152021 0.0000056  0.0913 0.0035  I  -110.105    0.434    -5.812    0.081  0.005300  0.230244 -0.0152158  -110.223    -5.787  
+23 125 59969.00 I  0.003919 0.000026  0.231443 0.000024  I-0.0154039 0.0000046  0.2806 0.0036  I  -110.109    0.579    -5.809    0.163  0.003852  0.231401 -0.0153642  -110.193    -5.799  
+23 126 59970.00 I  0.002890 0.000027  0.233310 0.000026  I-0.0156939 0.0000046  0.2616 0.0032  I  -110.224    0.579    -5.762    0.163  0.002927  0.233231 -0.0156349  -110.268    -5.775  
+23 127 59971.00 I  0.001577 0.000026  0.235926 0.000027  I-0.0158984 0.0000044  0.1565 0.0038  I  -110.442    0.579    -5.597    0.163  0.001593  0.235918 -0.0158886  -110.468    -5.635  
+23 128 59972.00 I  0.000380 0.000022  0.238091 0.000027  I-0.0159846 0.0000060 -0.0156 0.0036  I  -110.698    0.725    -5.506    0.211  0.000279  0.238107 -0.0159862  -110.687    -5.537  
+23 129 59973.00 I -0.000271 0.000025  0.240389 0.000028  I-0.0158766 0.0000057 -0.1596 0.0039  I  -110.853    0.856    -5.641    0.196 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
+23 130 59974.00 I -0.000861 0.000024  0.242664 0.000028  I-0.0156634 0.0000050 -0.3098 0.0055  I  -110.868    0.856    -5.898    0.196 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
+23 131 59975.00 I -0.001399 0.000020  0.244993 0.000021  I-0.0152294 0.0000094 -0.5429 0.0049  I  -110.779    1.181    -6.079    0.157 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
+23 2 1 59976.00 I -0.002309 0.000021  0.247832 0.000039  I-0.0146104 0.0000084 -0.6778 0.0063  I  -110.583    1.099    -6.154    0.172 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
+23 2 2 59977.00 I -0.003561 0.000021  0.250285 0.000039  I-0.0138920 0.0000084 -0.7582 0.0059  I  -110.280    1.099    -6.242    0.172                                                     
+23 2 3 59978.00 I -0.004906 0.000021  0.252583 0.000039  I-0.0131166 0.0000084 -0.7708 0.0062  I  -109.983    1.099    -6.393    0.172                                                     
+23 2 4 59979.00 I -0.006471 0.000019  0.254237 0.000039  I-0.0123988 0.0000091 -0.6382 0.0049  I  -109.828    1.013    -6.494    0.185                                                     
+23 2 5 59980.00 I -0.008210 0.000022  0.255949 0.000039  I-0.0118614 0.0000052 -0.4421 0.0052  I  -109.805    0.774    -6.423    0.152                                                     
+23 2 6 59981.00 I -0.009960 0.000022  0.257720 0.000039  I-0.0114986 0.0000052 -0.2940 0.0034  I  -109.768    0.774    -6.219    0.152                                                     
+23 2 7 59982.00 I -0.011917 0.000021  0.259705 0.000017  I-0.0112742 0.0000043 -0.1436 0.0033  I  -109.608    0.657    -6.037    0.129                                                     
+23 2 8 59983.00 I -0.014093 0.000034  0.261632 0.000036  I-0.0112016 0.0000042 -0.0227 0.0030  I  -109.356    0.750    -5.959    0.103                                                     
+23 2 9 59984.00 I -0.015724 0.000034  0.263431 0.000035  I-0.0112376 0.0000041  0.1246 0.0030  I  -109.134    0.750    -5.939    0.103                                                     
+23 210 59985.00 I -0.016729 0.000034  0.265667 0.000036  I-0.0114593 0.0000043  0.2974 0.0042  I  -109.041    0.750    -5.922    0.103                                                     
+23 211 59986.00 I -0.017892 0.000030  0.267965 0.000034  I-0.0117914 0.0000074  0.3472 0.0033  I  -109.120    0.917    -5.960    0.043                                                     
+23 212 59987.00 I -0.019635 0.000032  0.270446 0.000035  I-0.0121214 0.0000051  0.3000 0.0044  I  -109.324    0.870    -6.124    0.125                                                     
+23 213 59988.00 I -0.021942 0.000033  0.273074 0.000037  I-0.0123682 0.0000049  0.1832 0.0036  I  -109.526    0.870    -6.349    0.125                                                     
+23 214 59989.00 I -0.024488 0.000019  0.275745 0.000020  I-0.0124643 0.0000050 -0.0043 0.0037  I  -109.671    0.834    -6.476    0.162                                                     
+23 215 59990.00 I -0.026965 0.000029  0.278156 0.000022  I-0.0123530 0.0000055 -0.2118 0.0036  I  -109.897    0.787    -6.485    0.157                                                     
+23 216 59991.00 I -0.029371 0.000029  0.280696 0.000022  I-0.0120637 0.0000053 -0.3504 0.0038  I  -110.308    0.787    -6.575    0.157                                                     
+23 217 59992.00 I -0.031758 0.000029  0.282901 0.000024  I-0.0116875 0.0000052 -0.3829 0.0049  I  -110.665    0.787    -6.879    0.157                                                     
+23 218 59993.00 I -0.033991 0.000024  0.284840 0.000023  I-0.0113639 0.0000083 -0.2172 0.0040  I  -110.582    0.461    -7.209    0.132                                                     
+23 219 59994.00 I -0.035823 0.000035  0.286852 0.000026  I-0.0113035 0.0000061  0.0997 0.0052  I  -110.035    0.806    -7.269    0.232                                                     
+23 220 59995.00 I -0.037241 0.000034  0.288944 0.000025  I-0.0115703 0.0000061  0.4378 0.0042  I  -109.414    0.806    -7.063    0.232                                                     
+23 221 59996.00 I -0.038252 0.000026  0.291554 0.000023  I-0.0121576 0.0000058  0.7116 0.0040  I  -109.046    0.826    -6.870    0.244                                                     
+23 222 59997.00 I -0.038779 0.000031  0.294587 0.000023  I-0.0129265 0.0000053  0.7844 0.0041  I  -108.959    0.820    -6.834    0.218                                                     
+23 223 59998.00 I -0.038963 0.000032  0.298258 0.000021  I-0.0137037 0.0000057  0.7892 0.0042  I  -109.085    0.820    -6.826    0.218                                                     
+23 224 59999.00 I -0.039169 0.000033  0.301880 0.000020  I-0.0144905 0.0000064  0.7510 0.0054  I  -109.393    0.820    -6.749    0.218                                                     
+23 225 60000.00 I -0.039675 0.000022  0.305084 0.000010  I-0.0151479 0.0000091  0.5395 0.0050  I  -109.758    0.761    -6.738    0.065                                                     
+23 226 60001.00 I -0.040937 0.000025  0.308181 0.000012  I-0.0155312 0.0000076  0.2133 0.0059  I  -109.980    0.864    -6.938    0.047                                                     
+23 227 60002.00 I -0.042707 0.000025  0.310711 0.000012  I-0.0156026 0.0000074 -0.0284 0.0059  I  -109.998    0.864    -7.258    0.047                                                     
+23 228 60003.00 I -0.044027 0.000019  0.313341 0.000010  I-0.0155053 0.0000090 -0.1773 0.0053  I  -109.887    0.924    -7.471    0.027                                                     
+23 3 1 60004.00 I -0.045093 0.000020  0.316292 0.000018  I-0.0152896 0.0000076 -0.2013 0.0056  I  -109.672    0.924    -7.496    0.027                                                     
+23 3 2 60005.00 I -0.046060 0.000020  0.318731 0.000019  I-0.0151046 0.0000068 -0.2196 0.0051  I  -109.305    0.924    -7.463    0.027                                                     
+23 3 3 60006.00 I -0.046664 0.000018  0.321152 0.000019  I-0.0148508 0.0000069 -0.2368 0.0061  I  -108.857    0.924    -7.504    0.027                                                     
+23 3 4 60007.00 I -0.046921 0.000015  0.323781 0.000020  I-0.0146829 0.0000102 -0.0982 0.0051  I  -108.521    0.322    -7.577    0.160                                                     
+23 3 5 60008.00 I -0.046595 0.000038  0.326597 0.000022  I-0.0146855 0.0000076  0.1337 0.0062  I  -108.407    0.943    -7.539    0.052                                                     
+23 3 6 60009.00 I -0.045654 0.000038  0.329761 0.000022  I-0.0149448 0.0000072  0.3491 0.0054  I  -108.414    0.943    -7.349    0.052                                                     
+23 3 7 60010.00 I -0.044610 0.000036  0.333355 0.000016  I-0.0153706 0.0000078  0.5251 0.0050  I  -108.385    0.943    -7.132    0.052                                                     
+23 3 8 60011.00 I -0.043512 0.000039  0.336613 0.000015  I-0.0159988 0.0000070  0.7125 0.0052  I  -108.301    0.916    -7.037    0.051                                                     
+23 3 9 60012.00 I -0.042352 0.000039  0.339813 0.000014  I-0.0167717 0.0000068  0.8282 0.0045  I  -108.258    0.916    -7.092    0.051                                                     
+23 310 60013.00 I -0.041307 0.000042  0.343088 0.000014  I-0.0176165 0.0000056  0.8277 0.0043  I  -108.313    0.916    -7.216    0.051                                                     
+23 311 60014.00 I -0.040753 0.000021  0.346408 0.000010  I-0.0184001 0.0000053  0.7461 0.0041  I  -108.424    0.853    -7.342    0.049                                                     
+23 312 60015.00 I -0.040508 0.000024  0.349531 0.000013  I-0.0190888 0.0000060  0.6049 0.0040  I  -108.525    0.914    -7.467    0.059                                                     
+23 313 60016.00 I -0.040071 0.000027  0.352565 0.000014  I-0.0195856 0.0000060  0.3909 0.0046  I  -108.580    0.914    -7.604    0.059                                                     
+23 314 60017.00 I -0.039712 0.000022  0.356013 0.000016  I-0.0198997 0.0000069  0.2642 0.0048  I  -108.558    0.975    -7.736    0.067                                                     
+23 315 60018.00 I -0.039666 0.000025  0.359413 0.000019  I-0.0200943 0.0000074  0.0785 0.0052  I  -108.455    0.975    -7.850    0.067                                                     
+23 316 60019.00 I -0.039787 0.000024  0.362290 0.000019  I-0.0200729 0.0000079 -0.0585 0.0055  I  -108.301    0.975    -7.989    0.067                                                     
+23 317 60020.00 I -0.039643 0.000022  0.364626 0.000020  I-0.0200420 0.0000081 -0.0014 0.0062  P  -108.177    0.278    -8.167    0.145                                                     
+23 318 60021.00 I -0.039037 0.000019  0.366856 0.000012  I-0.0201168 0.0000095  0.1959 0.0062  P  -108.066    0.288    -8.292    0.148                                                     
+23 319 60022.00 I -0.038084 0.000091  0.369004 0.000091  I-0.0204769 0.0000094  0.5226 0.0074  P  -107.967    0.297    -8.241    0.151                                                     
+23 320 60023.00 I -0.036882 0.000091  0.371270 0.000091  I-0.0211387 0.0000113  0.7792 0.0070  P  -107.927    0.304    -8.041    0.154                                                     
+23 321 60024.00 I -0.035468 0.000092  0.373949 0.000091  I-0.0219984 0.0000105  0.9249 0.0080  P  -107.965    0.309    -7.867    0.155                                                     
+23 322 60025.00 I -0.033934 0.000091  0.377079 0.000091  I-0.0229498 0.0000113  0.9545 0.0080  P  -108.051    0.313    -7.833    0.157                                                     
+23 323 60026.00 I -0.032488 0.000091  0.380234 0.000090  I-0.0238725 0.0000122  0.8795 0.0088  P  -108.199    0.316    -7.877    0.158                                                     
+23 324 60027.00 I -0.031160 0.000091  0.383304 0.000091  I-0.0246722 0.0000136  0.6948 0.0088  P  -108.455    0.318    -7.917    0.158                                                     
+23 325 60028.00 I -0.029845 0.000091  0.386413 0.000091  I-0.0252185 0.0000127  0.3792 0.0093  P  -108.763    0.319    -7.996    0.159                                                     
+23 326 60029.00 I -0.028351 0.000091  0.389518 0.000091  I-0.0254306 0.0000127  0.0635 0.0086  P  -108.967    0.320    -8.191    0.159                                                     
+23 327 60030.00 I -0.026565 0.000090  0.392645 0.000091  I-0.0253814 0.0000117 -0.1445 0.0087  P  -108.982    0.321    -8.441    0.160                                                     
+23 328 60031.00 I -0.024691 0.000091  0.395441 0.000091  I-0.0251694 0.0000118 -0.2690 0.0081  P  -108.844    0.321    -8.593    0.160                                                     
+23 329 60032.00 I -0.023033 0.000090  0.397906 0.000091  I-0.0248763 0.0000111 -0.2947 0.0078  P  -108.579    0.321    -8.590    0.160                                                     
+23 330 60033.00 I -0.021728 0.000090  0.400145 0.000090  I-0.0245876 0.0000102                 P  -108.155    0.321    -8.550    0.160                                                     
+23 331 60034.00 P -0.020328 0.000632  0.402343 0.000402  P-0.0243815 0.0001080                 P  -107.624    0.322    -8.602    0.160                                                     
+23 4 1 60035.00 P -0.019069 0.000938  0.404490 0.000663  P-0.0243045 0.0002041                 P  -107.189    0.322    -8.726    0.160                                                     
+23 4 2 60036.00 P -0.017744 0.001182  0.406627 0.000887  P-0.0243797 0.0003028                 P  -107.039    0.322    -8.770    0.160                                                     
+23 4 3 60037.00 P -0.016366 0.001392  0.408824 0.001092  P-0.0246181 0.0004021                 P  -107.156    0.322    -8.635    0.160                                                     
+23 4 4 60038.00 P -0.014956 0.001581  0.411084 0.001282  P-0.0250215 0.0005017                 P  -107.364    0.322    -8.393    0.160                                                     
+23 4 5 60039.00 P -0.013504 0.001754  0.413424 0.001462  P-0.0255725 0.0006014                 P  -107.530    0.322    -8.216    0.160                                                     
+23 4 6 60040.00 P -0.012020 0.001915  0.415790 0.001633  P-0.0262092 0.0007012                 P  -107.654    0.322    -8.211    0.160                                                     
+23 4 7 60041.00 P -0.010486 0.002067  0.418145 0.001798  P-0.0268385 0.0007500                 P  -107.784    0.322    -8.346    0.160                                                     
+23 4 8 60042.00 P -0.008915 0.002210  0.420466 0.001957  P-0.0273638 0.0005500                 P  -107.923    0.322    -8.516    0.160                                                     
+23 4 9 60043.00 P -0.007308 0.002347  0.422744 0.002112  P-0.0277033 0.0007548                 P  -108.046    0.322    -8.653    0.160                                                     
+23 410 60044.00 P -0.005666 0.002478  0.424993 0.002262  P-0.0278329 0.0009344                 P  -108.128    0.322    -8.763    0.160                                                     
+23 411 60045.00 P -0.003996 0.002604  0.427203 0.002408  P-0.0277760 0.0010994                 P  -108.115    0.322    -8.885    0.160                                                     
+23 412 60046.00 P -0.002298 0.002726  0.429377 0.002551  P-0.0275815 0.0012543                 P  -107.916    0.322    -9.039    0.160                                                     
+23 413 60047.00 P -0.000575 0.002843  0.431513 0.002690  P-0.0273482 0.0014016                 P  -107.493    0.322    -9.199    0.160                                                     
+23 414 60048.00 P  0.001177 0.002957  0.433618 0.002827  P-0.0272123 0.0015429                 P  -106.961    0.322    -9.308    0.160                                                     
+23 415 60049.00 P  0.002959 0.003068  0.435695 0.002962  P-0.0272968 0.0016792                 P  -106.542    0.322    -9.311    0.160                                                     
+23 416 60050.00 P  0.004774 0.003176  0.437746 0.003094  P-0.0276587 0.0018113                 P  -106.405    0.322    -9.196    0.160                                                     
+23 417 60051.00 P  0.006625 0.003281  0.439775 0.003224  P-0.0283032 0.0019399                 P  -106.544    0.322    -9.016    0.160                                                     
+23 418 60052.00 P  0.008508 0.003384  0.441781 0.003352  P-0.0291458 0.0020652                 P  -106.800    0.322    -8.859    0.160                                                     
+23 419 60053.00 P  0.010423 0.003484  0.443762 0.003478  P-0.0300608 0.0021877                 P  -107.013    0.322    -8.779    0.160                                                     
+23 420 60054.00 P  0.012368 0.003582  0.445717 0.003602  P-0.0309027 0.0023077                 P  -107.144    0.322    -8.770    0.160                                                     
+23 421 60055.00 P  0.014345 0.003679  0.447642 0.003725  P-0.0315476 0.0024255                 P  -107.254    0.322    -8.813    0.160                                                     
+23 422 60056.00 P  0.016351 0.003773  0.449537 0.003846  P-0.0319355 0.0025411                 P  -107.392    0.322    -8.920    0.160                                                     
+23 423 60057.00 P  0.018388 0.003866  0.451401 0.003966  P-0.0320641 0.0026548                 P  -107.526    0.322    -9.089    0.160                                                     
+23 424 60058.00 P  0.020453 0.003957  0.453232 0.004084  P-0.0319798 0.0027668                 P  -107.588    0.322    -9.256    0.160                                                     
+23 425 60059.00 P  0.022548 0.004046  0.455029 0.004201  P-0.0317505 0.0028772                 P  -107.537    0.322    -9.341    0.160                                                     
+23 426 60060.00 P  0.024671 0.004134  0.456794 0.004317  P-0.0314645 0.0029860                 P  -107.353    0.322    -9.351    0.160                                                     
+23 427 60061.00 P  0.026821 0.004221  0.458526 0.004431  P-0.0311954 0.0030934                 P  -107.018    0.322    -9.389    0.160                                                     
+23 428 60062.00 P  0.028998 0.004306  0.460224 0.004545  P-0.0310158 0.0031995                 P  -106.567    0.322    -9.530    0.160                                                     
+23 429 60063.00 P  0.031202 0.004390  0.461889 0.004657  P-0.0309729 0.0033043                 P  -106.140    0.322    -9.719    0.160                                                     
+23 430 60064.00 P  0.033432 0.004473  0.463520 0.004768  P-0.0310918 0.0034080                 P  -105.934    0.322    -9.801    0.160                                                     
+23 5 1 60065.00 P  0.035687 0.004555  0.465117 0.004879  P-0.0313780 0.0035105                 P  -106.058    0.322    -9.680    0.160                                                     
+23 5 2 60066.00 P  0.037968 0.004635  0.466679 0.004988  P-0.0318057 0.0036120                 P  -106.436    0.322    -9.411    0.160                                                     
+23 5 3 60067.00 P  0.040272 0.004715  0.468207 0.005096  P-0.0323266 0.0037124                 P  -106.864    0.322    -9.145    0.160                                                     
+23 5 4 60068.00 P  0.042601 0.004793  0.469699 0.005204  P-0.0328644 0.0038119                 P  -107.185    0.322    -9.008    0.160                                                     
+23 5 5 60069.00 P  0.044952 0.004871  0.471155 0.005310  P-0.0333214 0.0039105                 P  -107.389    0.322    -9.030    0.160                                                     
+23 5 6 60070.00 P  0.047325 0.004948  0.472576 0.005416  P-0.0335999 0.0040082                 P  -107.568    0.322    -9.169    0.160                                                     
+23 5 7 60071.00 P  0.049720 0.005023  0.473960 0.005521  P-0.0336392 0.0041051                 P  -107.771    0.322    -9.367    0.160                                                     
+23 5 8 60072.00 P  0.052137 0.005098  0.475307 0.005626  P-0.0334394 0.0042012                 P  -107.920    0.322    -9.572    0.160                                                     
+23 5 9 60073.00 P  0.054573 0.005172  0.476617 0.005729  P-0.0330542 0.0042965                 P  -107.884    0.322    -9.740    0.160                                                     
+23 510 60074.00 P  0.057030 0.005246  0.477889 0.005832  P-0.0325904 0.0043911                 P  -107.610    0.322    -9.846    0.160                                                     
+23 511 60075.00 P  0.059506 0.005318  0.479124 0.005934  P-0.0321779 0.0044849                 P  -107.176    0.322    -9.889    0.160                                                     
+23 512 60076.00 P  0.062000 0.005390  0.480321 0.006035  P-0.0319248 0.0045781                 P  -106.735    0.322    -9.875    0.160                                                     
+23 513 60077.00 P  0.064511 0.005461  0.481479 0.006136  P-0.0318955 0.0046706                 P  -106.431    0.322    -9.806    0.160                                                     
+23 514 60078.00 P  0.067040 0.005532  0.482600 0.006236  P-0.0320960 0.0047625                 P  -106.341    0.322    -9.687    0.160                                                     
+23 515 60079.00 P  0.069585 0.005601  0.483681 0.006336  P-0.0324647 0.0048537                 P  -106.468    0.322    -9.531    0.160                                                     
+23 516 60080.00 P  0.072146 0.005670  0.484724 0.006434  P-0.0328981 0.0049444                 P  -106.743    0.322    -9.351    0.160                                                     
+23 517 60081.00 P  0.074722 0.005739  0.485727 0.006533  P-0.0332704 0.0050344                 P  -107.050    0.322    -9.174    0.160                                                     
+23 518 60082.00 P  0.077313 0.005807  0.486692 0.006630  P-0.0334638 0.0051240                 P  -107.269    0.322    -9.054    0.160                                                     
+23 519 60083.00 P  0.079916 0.005874  0.487616 0.006728  P-0.0334017 0.0052129                 P  -107.352    0.322    -9.061    0.160                                                     
+23 520 60084.00 P  0.082533 0.005941  0.488502 0.006824  P-0.0330674 0.0053014                 P  -107.355    0.322    -9.222    0.160                                                     
+23 521 60085.00 P  0.085162 0.006007  0.489347 0.006920  P-0.0324981 0.0053893                 P  -107.379    0.322    -9.471    0.160                                                     
+23 522 60086.00 P  0.087803 0.006072  0.490152 0.007016  P-0.0317587 0.0054768                 P  -107.461    0.322    -9.677    0.160                                                     
+23 523 60087.00 P  0.090454 0.006137  0.490917 0.007111  P-0.0309290 0.0055637                 P  -107.552    0.322    -9.754    0.160                                                     
+23 524 60088.00 P  0.093115 0.006202  0.491641 0.007205  P-0.0300902 0.0056502                 P  -107.581    0.322    -9.748    0.160                                                     
+23 525 60089.00 P  0.095786 0.006266  0.492325 0.007299  P-0.0293170 0.0057362                 P  -107.508    0.322    -9.780    0.160                                                     
+23 526 60090.00 P  0.098466 0.006329  0.492968 0.007393  P-0.0286675 0.0058218                 P  -107.312    0.322    -9.904    0.160                                                     
+23 527 60091.00 P  0.101153 0.006393  0.493571 0.007486  P-0.0281770 0.0059070                 P  -107.017    0.322   -10.030    0.160                                                     
+23 528 60092.00 P  0.103848 0.006455  0.494133 0.007579  P-0.0278594 0.0059917                 P  -106.763    0.322   -10.018    0.160                                                     
+23 529 60093.00 P  0.106549 0.006517  0.494654 0.007671  P-0.0276978 0.0060760                 P  -106.784    0.322    -9.825    0.160                                                     
+23 530 60094.00 P  0.109255 0.006579  0.495134 0.007763  P-0.0276510 0.0061599                 P  -107.211    0.322    -9.546    0.160                                                     
+23 531 60095.00 P  0.111967 0.006640  0.495573 0.007854  P-0.0276541 0.0062434                 P  -107.889    0.322    -9.304    0.160                                                     
+23 6 1 60096.00 P  0.114684 0.006701  0.495970 0.007946  P-0.0276163 0.0063266                 P  -108.498    0.322    -9.148    0.160                                                     
+23 6 2 60097.00 P  0.117404 0.006761  0.496327 0.008036  P-0.0274449 0.0064093                 P  -108.877    0.322    -9.082    0.160                                                     
+23 6 3 60098.00 P  0.120126 0.006821  0.496643 0.008126  P-0.0270623 0.0064917                 P  -109.134    0.322    -9.140    0.160                                                     
+23 6 4 60099.00 P  0.122851 0.006881  0.496917 0.008216  P-0.0264360 0.0065737                 P  -109.381    0.322    -9.359    0.160                                                     
+23 6 5 60100.00 P  0.125578 0.006940  0.497150 0.008306  P-0.0256000 0.0066554                 P  -109.512    0.322    -9.662    0.160                                                     
+23 6 6 60101.00 P  0.128305 0.006999  0.497341 0.008395  P-0.0246517 0.0067368                 P  -109.359    0.322    -9.875    0.160                                                     
+23 6 7 60102.00 P  0.131032 0.007058  0.497492 0.008483  P-0.0237260 0.0068177                 P  -108.978    0.322    -9.887    0.160                                                     
+23 6 8 60103.00 P  0.133759 0.007116  0.497601 0.008572  P-0.0229500 0.0068984                 P  -108.642    0.322    -9.755    0.160                                                     
+23 6 9 60104.00 P  0.136484 0.007174  0.497669 0.008660  P-0.0224032 0.0069788                 P  -108.551    0.322    -9.608    0.160                                                     
+23 610 60105.00 P  0.139206 0.007231  0.497696 0.008747  P-0.0220943 0.0070588                 P  -108.661    0.322    -9.507    0.160                                                     
+23 611 60106.00 P  0.141926 0.007288  0.497682 0.008835  P-0.0219634 0.0071385                 P  -108.809    0.322    -9.424    0.160                                                     
+23 612 60107.00 P  0.144643 0.007345  0.497627 0.008922  P-0.0219064 0.0072179                 P  -108.920    0.322    -9.315    0.160                                                     
+23 613 60108.00 P  0.147355 0.007401  0.497531 0.009008  P-0.0218041 0.0072970                 P  -109.070    0.322    -9.157    0.160                                                     
+23 614 60109.00 P  0.150062 0.007457  0.497394 0.009095  P-0.0215485 0.0073758                 P  -109.341    0.322    -8.969    0.160                                                     
+23 615 60110.00 P  0.152764 0.007513  0.497216 0.009181  P-0.0210649 0.0074544                                                                                                             
+23 616 60111.00 P  0.155459 0.007569  0.496998 0.009266  P-0.0203238 0.0075326                                                                                                             
+23 617 60112.00 P  0.158146 0.007624  0.496739 0.009352  P-0.0193416 0.0076106                                                                                                             
+23 618 60113.00 P  0.160827 0.007679  0.496440 0.009437  P-0.0181698 0.0076883                                                                                                             
+23 619 60114.00 P  0.163498 0.007733  0.496100 0.009522  P-0.0168833 0.0077657                                                                                                             
+23 620 60115.00 P  0.166160 0.007787  0.495721 0.009606  P-0.0155653 0.0078428                                                                                                             
+23 621 60116.00 P  0.168813 0.007841  0.495301 0.009690  P-0.0142968 0.0079197                                                                                                             
+23 622 60117.00 P  0.171455 0.007895  0.494841 0.009774  P-0.0131412 0.0079964                                                                                                             
+23 623 60118.00 P  0.174085 0.007949  0.494342 0.009858  P-0.0121406 0.0080728                                                                                                             
+23 624 60119.00 P  0.176704 0.008002  0.493804 0.009941  P-0.0113101 0.0081489                                                                                                             
+23 625 60120.00 P  0.179310 0.008055  0.493226 0.010024  P-0.0106351 0.0082248                                                                                                             
+23 626 60121.00 P  0.181902 0.008107  0.492609 0.010107  P-0.0100819 0.0083005                                                                                                             
+23 627 60122.00 P  0.184481 0.008160  0.491954 0.010190  P-0.0095985 0.0083759                                                                                                             
+23 628 60123.00 P  0.187045 0.008212  0.491259 0.010272  P-0.0091171 0.0084511                                                                                                             
+23 629 60124.00 P  0.189594 0.008264  0.490527 0.010354  P-0.0085582 0.0085261                                                                                                             
+23 630 60125.00 P  0.192126 0.008315  0.489756 0.010436  P-0.0078433 0.0086008                                                                                                             
+23 7 1 60126.00 P  0.194642 0.008367  0.488948 0.010517  P-0.0069197 0.0086754                                                                                                             
+23 7 2 60127.00 P  0.197141 0.008418  0.488102 0.010599  P-0.0057898 0.0087497                                                                                                             
+23 7 3 60128.00 P  0.199622 0.008469  0.487219 0.010680  P-0.0045226 0.0088237                                                                                                             
+23 7 4 60129.00 P  0.202085 0.008519  0.486298 0.010760  P-0.0032438 0.0088976                                                                                                             
+23 7 5 60130.00 P  0.204528 0.008570  0.485342 0.010841  P-0.0020990 0.0089713                                                                                                             
+23 7 6 60131.00 P  0.206951 0.008620  0.484348 0.010921  P-0.0011992 0.0090448                                                                                                             
+23 7 7 60132.00 P  0.209354 0.008670  0.483319 0.011002  P-0.0005764 0.0091180                                                                                                             
+23 7 8 60133.00 P  0.211736 0.008720  0.482254 0.011081  P-0.0001758 0.0091911                                                                                                             
+23 7 9 60134.00 P  0.214097 0.008770  0.481153 0.011161  P 0.0001189 0.0092639                                                                                                             
+23 710 60135.00 P  0.216437 0.008819  0.480018 0.011241  P 0.0004462 0.0093366                                                                                                             
+23 711 60136.00 P  0.218755 0.008868  0.478848 0.011320  P 0.0009277 0.0094091                                                                                                             
+23 712 60137.00 P  0.221049 0.008917  0.477644 0.011399  P 0.0016409 0.0094814                                                                                                             
+23 713 60138.00 P  0.223319 0.008966  0.476406 0.011478  P 0.0026146 0.0095535                                                                                                             
+23 714 60139.00 P  0.225564 0.009015  0.475135 0.011556  P 0.0038325 0.0096254                                                                                                             
+23 715 60140.00 P  0.227785 0.009063  0.473830 0.011635  P 0.0052436 0.0096971                                                                                                             
+23 716 60141.00 P  0.229980 0.009111  0.472492 0.011713  P 0.0067771 0.0097686                                                                                                             
+23 717 60142.00 P  0.232149 0.009159  0.471122 0.011791  P 0.0083633 0.0098400                                                                                                             
+23 718 60143.00 P  0.234291 0.009207  0.469720 0.011869  P 0.0099095 0.0099112                                                                                                             
+23 719 60144.00 P  0.236405 0.009254  0.468286 0.011946  P 0.0113483 0.0099822                                                                                                             
+23 720 60145.00 P  0.238492 0.009302  0.466821 0.012024  P 0.0126329 0.0100531                                                                                                             
+23 721 60146.00 P  0.240551 0.009349  0.465326 0.012101  P 0.0137415 0.0101238                                                                                                             
+23 722 60147.00 P  0.242581 0.009396  0.463800 0.012178  P 0.0146808 0.0101943                                                                                                             
+23 723 60148.00 P  0.244581 0.009443  0.462245 0.012255  P 0.0154818 0.0102646                                                                                                             
+23 724 60149.00 P  0.246552 0.009490  0.460660 0.012331  P 0.0161953 0.0103348                                                                                                             
+23 725 60150.00 P  0.248493 0.009536  0.459046 0.012408  P 0.0168844 0.0104048                                                                                                             
+23 726 60151.00 P  0.250402 0.009583  0.457404 0.012484  P 0.0176193 0.0104747                                                                                                             
+23 727 60152.00 P  0.252281 0.009629  0.455734 0.012560  P 0.0184697 0.0105444                                                                                                             
+23 728 60153.00 P  0.254128 0.009675  0.454036 0.012636  P 0.0194906 0.0106139                                                                                                             
+23 729 60154.00 P  0.255942 0.009721  0.452312 0.012712  P 0.0207004 0.0106833                                                                                                             
+23 730 60155.00 P  0.257725 0.009767  0.450561 0.012787  P 0.0220586 0.0107526                                                                                                             
+23 731 60156.00 P  0.259474 0.009812  0.448784 0.012863  P 0.0234605 0.0108216                                                                                                             
+23 8 1 60157.00 P  0.261190 0.009858  0.446982 0.012938  P 0.0247588 0.0108906                                                                                                             
+23 8 2 60158.00 P  0.262872 0.009903  0.445154 0.013013  P 0.0258128 0.0109594                                                                                                             
+23 8 3 60159.00 P  0.264520 0.009948  0.443303 0.013088  P 0.0265439 0.0110280                                                                                                             
+23 8 4 60160.00 P  0.266133 0.009993  0.441427 0.013162  P 0.0269703 0.0110965                                                                                                             
+23 8 5 60161.00 P  0.267712 0.010038  0.439529 0.013237  P 0.0272012 0.0111649                                                                                                             
+23 8 6 60162.00 P  0.269255 0.010082  0.437607 0.013311  P 0.0273963 0.0112331                                                                                                             
+23 8 7 60163.00 P  0.270762 0.010127  0.435663 0.013386  P 0.0277104 0.0113012                                                                                                             
+23 8 8 60164.00 P  0.272233 0.010171  0.433698 0.013460  P 0.0282509 0.0113691                                                                                                             
+23 8 9 60165.00 P  0.273668 0.010215  0.431712 0.013533  P 0.0290596 0.0114369                                                                                                             
+23 810 60166.00 P  0.275067 0.010259  0.429705 0.013607  P 0.0301205 0.0115046                                                                                                             
+23 811 60167.00 P  0.276428 0.010303  0.427678 0.013681  P 0.0313782 0.0115721                                                                                                             
+23 812 60168.00 P  0.277752 0.010347  0.425631 0.013754  P 0.0327573 0.0116395                                                                                                             
+23 813 60169.00 P  0.279038 0.010390  0.423566 0.013828  P 0.0341774 0.0117067                                                                                                             
+23 814 60170.00 P  0.280286 0.010434  0.421483 0.013901  P 0.0355602 0.0117739                                                                                                             
+23 815 60171.00 P  0.281497 0.010477  0.419381 0.013974  P 0.0368375 0.0118409                                                                                                             
+23 816 60172.00 P  0.282668 0.010520  0.417263 0.014046  P 0.0379578 0.0119077                                                                                                             
+23 817 60173.00 P  0.283801 0.010564  0.415129 0.014119  P 0.0388935 0.0119745                                                                                                             
+23 818 60174.00 P  0.284896 0.010607  0.412978 0.014192  P 0.0396445 0.0120411                                                                                                             
+23 819 60175.00 P  0.285950 0.010649  0.410812 0.014264  P 0.0402391 0.0121076                                                                                                             
+23 820 60176.00 P  0.286966 0.010692  0.408632 0.014336  P 0.0407274 0.0121740                                                                                                             
+23 821 60177.00 P  0.287942 0.010735  0.406437 0.014408  P 0.0411743 0.0122402                                                                                                             
+23 822 60178.00 P  0.288878 0.010777  0.404229 0.014480  P 0.0416499 0.0123063                                                                                                             
+23 823 60179.00 P  0.289774 0.010819  0.402008 0.014552  P 0.0422202 0.0123723                                                                                                             
+23 824 60180.00 P  0.290630 0.010861  0.399775 0.014624  P 0.0429366 0.0124382                                                                                                             
+23 825 60181.00 P  0.291446 0.010904  0.397531 0.014696  P 0.0438227 0.0125040                                                                                                             
+23 826 60182.00 P  0.292221 0.010945  0.395275 0.014767  P 0.0448575 0.0125696                                                                                                             
+23 827 60183.00 P  0.292955 0.010987  0.393009 0.014838  P 0.0459643 0.0126352                                                                                                             
+23 828 60184.00 P  0.293649 0.011029  0.390733 0.014909  P 0.0470154 0.0127006                                                                                                             
+23 829 60185.00 P  0.294302 0.011071  0.388448 0.014980  P 0.0478631 0.0127659                                                                                                             
+23 830 60186.00 P  0.294914 0.011112  0.386155 0.015051  P 0.0483904 0.0128311                                                                                                             
+23 831 60187.00 P  0.295485 0.011153  0.383854 0.015122  P 0.0485617 0.0128962                                                                                                             
+23 9 1 60188.00 P  0.296014 0.011195  0.381545 0.015193  P 0.0484432 0.0129612                                                                                                             
+23 9 2 60189.00 P  0.296503 0.011236  0.379230 0.015263  P 0.0481845 0.0130260                                                                                                             
+23 9 3 60190.00 P  0.296950 0.011277  0.376909 0.015334  P 0.0479657 0.0130908                                                                                                             
+23 9 4 60191.00 P  0.297355 0.011318  0.374583 0.015404  P 0.0479391 0.0131554                                                                                                             
+23 9 5 60192.00 P  0.297719 0.011358  0.372252 0.015474  P 0.0481878 0.0132199                                                                                                             
+23 9 6 60193.00 P  0.298042 0.011399  0.369917 0.015544  P 0.0487189 0.0132844                                                                                                             
+23 9 7 60194.00 P  0.298324 0.011440  0.367578 0.015614  P 0.0494804 0.0133487                                                                                                             
+23 9 8 60195.00 P  0.298563 0.011480  0.365237 0.015684  P 0.0503895 0.0134129                                                                                                             
+23 9 9 60196.00 P  0.298762 0.011520  0.362893 0.015753  P 0.0513555 0.0134770                                                                                                             
+23 910 60197.00 P  0.298919 0.011561  0.360548 0.015823  P 0.0522941 0.0135410                                                                                                             
+23 911 60198.00 P  0.299034 0.011601  0.358203 0.015892  P 0.0531333 0.0136050                                                                                                             
+23 912 60199.00 P  0.299108 0.011641  0.355856 0.015962  P 0.0538175 0.0136688                                                                                                             
+23 913 60200.00 P  0.299141 0.011681  0.353511 0.016031  P 0.0543130 0.0137325                                                                                                             
+23 914 60201.00 P  0.299133 0.011720  0.351166 0.016100  P 0.0546131 0.0137961                                                                                                             
+23 915 60202.00 P  0.299083 0.011760  0.348823 0.016169  P 0.0547391 0.0138596                                                                                                             
+23 916 60203.00 P  0.298992 0.011800  0.346482 0.016238  P 0.0547387 0.0139230                                                                                                             
+23 917 60204.00 P  0.298860 0.011839  0.344144 0.016306  P 0.0546784 0.0139863                                                                                                             
+23 918 60205.00 P  0.298688 0.011879  0.341810 0.016375  P 0.0546338 0.0140495                                                                                                             
+23 919 60206.00 P  0.298474 0.011918  0.339479 0.016443  P 0.0546769 0.0141127                                                                                                             
+23 920 60207.00 P  0.298220 0.011957  0.337154 0.016512  P 0.0548633 0.0141757                                                                                                             
+23 921 60208.00 P  0.297925 0.011996  0.334834 0.016580  P 0.0552192 0.0142386                                                                                                             
+23 922 60209.00 P  0.297590 0.012035  0.332520 0.016648  P 0.0557310 0.0143014                                                                                                             
+23 923 60210.00 P  0.297214 0.012074  0.330212 0.016716  P 0.0563370 0.0143642                                                                                                             
+23 924 60211.00 P  0.296799 0.012113  0.327912 0.016784  P 0.0569295 0.0144268                                                                                                             
+23 925 60212.00 P  0.296344 0.012152  0.325620 0.016852  P 0.0573734 0.0144894                                                                                                             
+23 926 60213.00 P  0.295849 0.012191  0.323336 0.016920  P 0.0575398 0.0145519                                                                                                             
+23 927 60214.00 P  0.295314 0.012229  0.321061 0.016987  P 0.0573522 0.0146142                                                                                                             
+23 928 60215.00 P  0.294741 0.012268  0.318795 0.017055  P 0.0568209 0.0146765                                                                                                             
+23 929 60216.00 P  0.294128 0.012306  0.316540 0.017122  P 0.0560498 0.0147387                                                                                                             
+23 930 60217.00 P  0.293476 0.012344  0.314296 0.017190  P 0.0552066 0.0148008                                                                                                             
+2310 1 60218.00 P  0.292786 0.012382  0.312063 0.017257  P 0.0544678 0.0148629                                                                                                             
+2310 2 60219.00 P  0.292058 0.012421  0.309843 0.017324  P 0.0539626 0.0149248                                                                                                             
+2310 3 60220.00 P  0.291291 0.012459  0.307635 0.017391  P 0.0537418 0.0149867                                                                                                             
+2310 4 60221.00 P  0.290487 0.012496  0.305440 0.017458  P 0.0537793 0.0150484                                                                                                             
+2310 5 60222.00 P  0.289645 0.012534  0.303258 0.017525  P 0.0539979 0.0151101                                                                                                             
+2310 6 60223.00 P  0.288766 0.012572  0.301091 0.017591  P 0.0543017 0.0151717                                                                                                             
+2310 7 60224.00 P  0.287851 0.012610  0.298939 0.017658  P 0.0545995 0.0152332                                                                                                             
+2310 8 60225.00 P  0.286898 0.012647  0.296803 0.017724  P 0.0548174 0.0152946                                                                                                             
+2310 9 60226.00 P  0.285910 0.012685  0.294682 0.017791  P 0.0549031 0.0153560                                                                                                             
+231010 60227.00 P  0.284885 0.012722  0.292578 0.017857  P 0.0548288 0.0154172                                                                                                             
+231011 60228.00 P  0.283825 0.012760  0.290491 0.017923  P 0.0545923 0.0154784                                                                                                             
+231012 60229.00 P  0.282730 0.012797  0.288422 0.017990  P 0.0542184 0.0155395                                                                                                             
+231013 60230.00 P  0.281600 0.012834  0.286371 0.018056  P 0.0537557 0.0156005                                                                                                             
+231014 60231.00 P  0.280435 0.012871  0.284338 0.018122  P 0.0532722 0.0156614                                                                                                             
+231015 60232.00 P  0.279237 0.012908  0.282325 0.018187  P 0.0528471 0.0157223                                                                                                             
+231016 60233.00 P  0.278004 0.012945  0.280331 0.018253  P 0.0525590 0.0157831                                                                                                             
+231017 60234.00 P  0.276739 0.012982  0.278358 0.018319  P 0.0524701 0.0158438                                                                                                             
+231018 60235.00 P  0.275440 0.013019  0.276405 0.018384  P 0.0526096 0.0159044                                                                                                             
+231019 60236.00 P  0.274109 0.013055  0.274473 0.018450  P 0.0529618 0.0159649                                                                                                             
+231020 60237.00 P  0.272746 0.013092  0.272564 0.018515  P 0.0534630 0.0160254                                                                                                             
+231021 60238.00 P  0.271352 0.013129  0.270676 0.018581  P 0.0540085 0.0160858                                                                                                             
+231022 60239.00 P  0.269926 0.013165  0.268811 0.018646  P 0.0544691 0.0161461                                                                                                             
+231023 60240.00 P  0.268469 0.013201  0.266969 0.018711  P 0.0547161 0.0162063                                                                                                             
+231024 60241.00 P  0.266983 0.013238  0.265151 0.018776  P 0.0546528 0.0162665                                                                                                             
+231025 60242.00 P  0.265466 0.013274  0.263357 0.018841  P 0.0542464 0.0163265                                                                                                             
+231026 60243.00 P  0.263920 0.013310  0.261587 0.018906  P 0.0535463 0.0163866                                                                                                             
+231027 60244.00 P  0.262345 0.013346  0.259842 0.018971  P 0.0526787 0.0164465                                                                                                             
+231028 60245.00 P  0.260742 0.013382  0.258123 0.019035  P 0.0518105 0.0165063                                                                                                             
+231029 60246.00 P  0.259111 0.013418  0.256429 0.019100  P 0.0510984 0.0165661                                                                                                             
+231030 60247.00 P  0.257453 0.013454  0.254762 0.019164  P 0.0506420 0.0166258                                                                                                             
+231031 60248.00 P  0.255767 0.013490  0.253121 0.019229  P 0.0504628 0.0166855                                                                                                             
+2311 1 60249.00 P  0.254056 0.013526  0.251507 0.019293  P 0.0505165 0.0167451                                                                                                             
+2311 2 60250.00 P  0.252318 0.013561  0.249921 0.019357  P 0.0507203 0.0168046                                                                                                             
+2311 3 60251.00 P  0.250555 0.013597  0.248362 0.019422  P 0.0509764 0.0168640                                                                                                             
+2311 4 60252.00 P  0.248768 0.013632  0.246832 0.019486  P 0.0511873 0.0169233                                                                                                             
+2311 5 60253.00 P  0.246956 0.013668  0.245330 0.019550  P 0.0512771 0.0169826                                                                                                             
+2311 6 60254.00 P  0.245120 0.013703  0.243857 0.019614  P 0.0512116 0.0170419                                                                                                             
+2311 7 60255.00 P  0.243262 0.013738  0.242413 0.019678  P 0.0509708 0.0171010                                                                                                             
+2311 8 60256.00 P  0.241381 0.013774  0.240999 0.019741  P 0.0505782 0.0171601                                                                                                             
+2311 9 60257.00 P  0.239477 0.013809  0.239615 0.019805  P 0.0500653 0.0172191                                                                                                             
+231110 60258.00 P  0.237553 0.013844  0.238261 0.019869  P 0.0494916 0.0172780                                                                                                             
+231111 60259.00 P  0.235607 0.013879  0.236937 0.019932  P 0.0489388 0.0173369                                                                                                             
+231112 60260.00 P  0.233641 0.013914  0.235645 0.019996  P 0.0485036 0.0173957                                                                                                             
+231113 60261.00 P  0.231656 0.013949  0.234384 0.020059  P 0.0482618 0.0174545                                                                                                             
+231114 60262.00 P  0.229651 0.013984  0.233154 0.020122  P 0.0482924 0.0175131                                                                                                             
+231115 60263.00 P  0.227628 0.014019  0.231955 0.020186  P 0.0485563 0.0175718                                                                                                             
+231116 60264.00 P  0.225587 0.014053  0.230789 0.020249  P 0.0490282 0.0176303                                                                                                             
+231117 60265.00 P  0.223529 0.014088  0.229655 0.020312  P 0.0495574 0.0176888                                                                                                             
+231118 60266.00 P  0.221453 0.014122  0.228554 0.020375  P 0.0500460 0.0177472                                                                                                             
+231119 60267.00 P  0.219362 0.014157  0.227486 0.020438  P 0.0503385 0.0178055                                                                                                             
+231120 60268.00 P  0.217255 0.014191  0.226450 0.020501  P 0.0503187 0.0178638                                                                                                             
+231121 60269.00 P  0.215134 0.014226  0.225448 0.020563  P 0.0501147 0.0179220                                                                                                             
+231122 60270.00 P  0.212998 0.014260  0.224479 0.020626  P 0.0497002 0.0179802                                                                                                             
+231123 60271.00 P  0.210848 0.014294  0.223544 0.020689  P 0.0492021 0.0180383                                                                                                             
+231124 60272.00 P  0.208686 0.014329  0.222642 0.020751  P 0.0486819 0.0180963                                                                                                             
+231125 60273.00 P  0.206511 0.014363  0.221775 0.020814  P 0.0483208 0.0181543                                                                                                             
+231126 60274.00 P  0.204324 0.014397  0.220942 0.020876  P 0.0481401 0.0182122                                                                                                             
+231127 60275.00 P  0.202126 0.014431  0.220143 0.020938  P 0.0482268 0.0182700                                                                                                             
+231128 60276.00 P  0.199918 0.014465  0.219379 0.021001  P 0.0485402 0.0183278                                                                                                             
+231129 60277.00 P  0.197699 0.014499  0.218649 0.021063  P 0.0489747 0.0183855                                                                                                             
+231130 60278.00 P  0.195472 0.014533  0.217955 0.021125  P 0.0494227 0.0184432                                                                                                             
+2312 1 60279.00 P  0.193236 0.014566  0.217295 0.021187  P 0.0498048 0.0185008                                                                                                             
+2312 2 60280.00 P  0.190992 0.014600  0.216670 0.021249  P 0.0500445 0.0185583                                                                                                             
+2312 3 60281.00 P  0.188741 0.014634  0.216080 0.021311  P 0.0501621 0.0186158                                                                                                             
+2312 4 60282.00 P  0.186483 0.014667  0.215526 0.021373  P 0.0501348 0.0186732                                                                                                             
+2312 5 60283.00 P  0.184219 0.014701  0.215007 0.021434  P 0.0499551 0.0187306                                                                                                             
+2312 6 60284.00 P  0.181950 0.014734  0.214524 0.021496  P 0.0496786 0.0187879                                                                                                             
+2312 7 60285.00 P  0.179676 0.014768  0.214076 0.021558  P 0.0493266 0.0188451                                                                                                             
+2312 8 60286.00 P  0.177398 0.014801  0.213663 0.021619  P 0.0489229 0.0189023                                                                                                             
+2312 9 60287.00 P  0.175116 0.014834  0.213287 0.021681  P 0.0485963 0.0189594                                                                                                             
+231210 60288.00 P  0.172832 0.014868  0.212945 0.021742  P 0.0483677 0.0190165                                                                                                             
+231211 60289.00 P  0.170546 0.014901  0.212640 0.021804  P 0.0483031 0.0190735                                                                                                             
+231212 60290.00 P  0.168258 0.014934  0.212370 0.021865  P 0.0484269 0.0191305                                                                                                             
+231213 60291.00 P  0.165969 0.014967  0.212136 0.021926  P 0.0487995 0.0191874                                                                                                             
+231214 60292.00 P  0.163680 0.015000  0.211938 0.021987  P 0.0492605 0.0192442                                                                                                             
+231215 60293.00 P  0.161392 0.015033  0.211775 0.022048  P 0.0497595 0.0193010                                                                                                             
+231216 60294.00 P  0.159105 0.015066  0.211648 0.022109  P 0.0501340 0.0193577                                                                                                             
+231217 60295.00 P  0.156819 0.015099  0.211556 0.022170  P 0.0501999 0.0194144                                                                                                             
+231218 60296.00 P  0.154536 0.015132  0.211501 0.022231  P 0.0499481 0.0194710                                                                                                             
+231219 60297.00 P  0.152256 0.015165  0.211480 0.022292  P 0.0494864 0.0195276                                                                                                             
+231220 60298.00 P  0.149980 0.015197  0.211495 0.022353  P 0.0489513 0.0195841                                                                                                             
+231221 60299.00 P  0.147708 0.015230  0.211546 0.022414  P 0.0484313 0.0196405                                                                                                             
+231222 60300.00 P  0.145441 0.015263  0.211632 0.022474  P 0.0480623 0.0196969                                                                                                             
+231223 60301.00 P  0.143179 0.015295  0.211753 0.022535  P 0.0479217 0.0197532                                                                                                             
+231224 60302.00 P  0.140924 0.015328  0.211909 0.022595  P 0.0480566 0.0198095                                                                                                             
+231225 60303.00 P  0.138675 0.015360  0.212101 0.022656  P 0.0484915 0.0198658                                                                                                             
+231226 60304.00 P  0.136434 0.015393  0.212327 0.022716  P 0.0491044 0.0199219                                                                                                             
+231227 60305.00 P  0.134201 0.015425  0.212588 0.022776  P 0.0498551 0.0199781                                                                                                             
+231228 60306.00 P  0.131977 0.015457  0.212883 0.022837  P 0.0505910 0.0200341                                                                                                             
+231229 60307.00 P  0.129762 0.015489  0.213213 0.022897  P 0.0512715 0.0200902                                                                                                             
+231230 60308.00 P  0.127557 0.015522  0.213578 0.022957  P 0.0517838 0.0201461                                                                                                             
+231231 60309.00 P  0.125363 0.015554  0.213976 0.023017  P 0.0522116 0.0202021                                                                                                             
+24 1 1 60310.00 P  0.123179 0.015586  0.214409 0.023077  P 0.0523631 0.0202579                                                                                                             
+24 1 2 60311.00 P  0.121007 0.015618  0.214875 0.023137  P 0.0523738 0.0203137                                                                                                             
+24 1 3 60312.00 P  0.118848 0.015650  0.215375 0.023197  P 0.0523231 0.0203695                                                                                                             
+24 1 4 60313.00 P  0.116702 0.015682  0.215909 0.023257  P 0.0522029 0.0204252                                                                                                             
+24 1 5 60314.00 P  0.114569 0.015714  0.216475 0.023317  P 0.0520780 0.0204809                                                                                                             
+24 1 6 60315.00 P  0.112450 0.015746  0.217075 0.023376  P 0.0520078 0.0205365                                                                                                             
+24 1 7 60316.00 P  0.110346 0.015777  0.217707 0.023436  P 0.0520849 0.0205920                                                                                                             
+24 1 8 60317.00 P  0.108257 0.015809  0.218372 0.023496  P 0.0523144 0.0206475                                                                                                             
+24 1 9 60318.00 P  0.106183 0.015841  0.219069 0.023555  P 0.0527459 0.0207030                                                                                                             
+24 110 60319.00 P  0.104127 0.015873  0.219798 0.023615  P 0.0533876 0.0207584                                                                                                             
+24 111 60320.00 P  0.102087 0.015904  0.220558 0.023674  P 0.0541302 0.0208138                                                                                                             
+24 112 60321.00 P  0.100064 0.015936  0.221350 0.023733  P 0.0547331 0.0208691                                                                                                             
+24 113 60322.00 P  0.098060 0.015967  0.222174 0.023793  P 0.0551267 0.0209243                                                                                                             
+24 114 60323.00 P  0.096074 0.015999  0.223028 0.023852  P 0.0552283 0.0209795                                                                                                             
+24 115 60324.00 P  0.094107 0.016030  0.223913 0.023911  P 0.0550364 0.0210347                                                                                                             
+24 116 60325.00 P  0.092160 0.016061  0.224828 0.023970  P 0.0546602 0.0210898                                                                                                             
+24 117 60326.00 P  0.090233 0.016093  0.225773 0.024029  P 0.0543109 0.0211449                                                                                                             
+24 118 60327.00 P  0.088326 0.016124  0.226747 0.024088  P 0.0540668 0.0211999                                                                                                             
+24 119 60328.00 P  0.086441 0.016155  0.227751 0.024147  P 0.0540528 0.0212548                                                                                                             
+24 120 60329.00 P  0.084577 0.016187  0.228784 0.024206  P 0.0543434 0.0213098                                                                                                             
+24 121 60330.00 P  0.082735 0.016218  0.229846 0.024265  P 0.0548542 0.0213646                                                                                                             
+24 122 60331.00 P  0.080917 0.016249  0.230935 0.024324  P 0.0555676 0.0214195                                                                                                             
+24 123 60332.00 P  0.079121 0.016280  0.232053 0.024383  P 0.0564479 0.0214742                                                                                                             
+24 124 60333.00 P  0.077348 0.016311  0.233198 0.024441  P 0.0573771 0.0215290                                                                                                             
+24 125 60334.00 P  0.075600 0.016342  0.234371 0.024500  P 0.0582431 0.0215837                                                                                                             
+24 126 60335.00 P  0.073876 0.016373  0.235570 0.024558  P 0.0589979 0.0216383                                                                                                             
+24 127 60336.00 P  0.072178 0.016404  0.236795 0.024617  P 0.0596027 0.0216929                                                                                                             
+24 128 60337.00 P  0.070504 0.016434  0.238047 0.024675  P 0.0600032 0.0217474                                                                                                             
+24 129 60338.00 P  0.068857 0.016465  0.239324 0.024734  P 0.0601838 0.0218019                                                                                                             
+24 130 60339.00 P  0.067235 0.016496  0.240626 0.024792  P 0.0601972 0.0218564                                                                                                             
+24 131 60340.00 P  0.065641 0.016527  0.241953 0.024851  P 0.0601323 0.0219108                                                                                                             
+24 2 1 60341.00 P  0.064073 0.016557  0.243304 0.024909  P 0.0600850 0.0219652                                                                                                             
+24 2 2 60342.00 P  0.062533 0.016588  0.244680 0.024967  P 0.0601229 0.0220195                                                                                                             
+24 2 3 60343.00 P  0.061021 0.016619  0.246078 0.025025  P 0.0602644 0.0220738                                                                                                             
+24 2 4 60344.00 P  0.059537 0.016649  0.247500 0.025083  P 0.0606006 0.0221280                                                                                                             
+24 2 5 60345.00 P  0.058081 0.016680  0.248945 0.025141  P 0.0610290 0.0221822                                                                                                             
+24 2 6 60346.00 P  0.056655 0.016710  0.250411 0.025199  P 0.0616178 0.0222363                                                                                                             
+24 2 7 60347.00 P  0.055258 0.016740  0.251899 0.025257  P 0.0622696 0.0222904                                                                                                             
+24 2 8 60348.00 P  0.053891 0.016771  0.253408 0.025315  P 0.0627957 0.0223444                                                                                                             
+24 2 9 60349.00 P  0.052554 0.016801  0.254939 0.025373  P 0.0631241 0.0223985                                                                                                             
+24 210 60350.00 P  0.051247 0.016831  0.256489 0.025431  P 0.0631540 0.0224524                                                                                                             
+24 211 60351.00 P  0.049971 0.016862  0.258059 0.025488  P 0.0628483 0.0225063                                                                                                             
+24 212 60352.00 P  0.048725 0.016892  0.259649 0.025546  P 0.0622533 0.0225602                                                                                                             
+24 213 60353.00 P  0.047512 0.016922  0.261257 0.025604  P 0.0615197 0.0226140                                                                                                             
+24 214 60354.00 P  0.046329 0.016952  0.262883 0.025661  P 0.0607901 0.0226678                                                                                                             
+24 215 60355.00 P  0.045179 0.016982  0.264528 0.025719  P 0.0602016 0.0227216                                                                                                             
+24 216 60356.00 P  0.044061 0.017012  0.266190 0.025776  P 0.0598424 0.0227753                                                                                                             
+24 217 60357.00 P  0.042975 0.017042  0.267868 0.025834  P 0.0597476 0.0228290                                                                                                             
+24 218 60358.00 P  0.041922 0.017072  0.269563 0.025891  P 0.0598644 0.0228826                                                                                                             
+24 219 60359.00 P  0.040902 0.017102  0.271274 0.025949  P 0.0601242 0.0229362                                                                                                             
+24 220 60360.00 P  0.039915 0.017132  0.273000 0.026006  P 0.0604207 0.0229897                                                                                                             
+24 221 60361.00 P  0.038962 0.017162  0.274740 0.026063  P 0.0606420 0.0230432                                                                                                             
+24 222 60362.00 P  0.038042 0.017192  0.276495 0.026120  P 0.0607394 0.0230966                                                                                                             
+24 223 60363.00 P  0.037156 0.017221  0.278264 0.026177  P 0.0606299 0.0231500                                                                                                             
+24 224 60364.00 P  0.036304 0.017251  0.280046 0.026234  P 0.0603173 0.0232034                                                                                                             
+24 225 60365.00 P  0.035486 0.017281  0.281840 0.026292  P 0.0597616 0.0232567                                                                                                             
+24 226 60366.00 P  0.034702 0.017311  0.283647 0.026349  P 0.0590465 0.0233100                                                                                                             
+24 227 60367.00 P  0.033953 0.017340  0.285465 0.026405  P 0.0582919 0.0233633                                                                                                             
+24 228 60368.00 P  0.033239 0.017370  0.287294 0.026462  P 0.0575959 0.0234165                                                                                                             
+24 229 60369.00 P  0.032560 0.017399  0.289134 0.026519  P 0.0570284 0.0234697                                                                                                             
+24 3 1 60370.00 P  0.031916 0.017429  0.290983 0.026576  P 0.0565793 0.0235228                                                                                                             
+24 3 2 60371.00 P  0.031306 0.017458  0.292842 0.026633  P 0.0563132 0.0235759                                                                                                             
+24 3 3 60372.00 P  0.030733 0.017488  0.294710 0.026689  P 0.0562005 0.0236289                                                                                                             
+24 3 4 60373.00 P  0.030194 0.017517  0.296586 0.026746  P 0.0563053 0.0236819                                                                                                             
+24 3 5 60374.00 P  0.029691 0.017546  0.298470 0.026803  P 0.0565527 0.0237349                                                                                                             
+24 3 6 60375.00 P  0.029223 0.017576  0.300361 0.026859  P 0.0568205 0.0237878                                                                                                             
+24 3 7 60376.00 P  0.028791 0.017605  0.302259 0.026916  P 0.0569281 0.0238407                                                                                                             
+24 3 8 60377.00 P  0.028395 0.017634  0.304163 0.026972  P 0.0567295 0.0238935                                                                                                             
+24 3 9 60378.00 P  0.028034 0.017663  0.306072 0.027029  P 0.0561918 0.0239463                                                                                                             
+24 310 60379.00 P  0.027709 0.017693  0.307986 0.027085  P 0.0553172 0.0239991                                                                                                             
+24 311 60380.00 P  0.027420 0.017722  0.309905 0.027141  P 0.0542178 0.0240518                                                                                                             
+24 312 60381.00 P  0.027167 0.017751  0.311828 0.027198  P 0.0532283 0.0241045                                                                                                             
+24 313 60382.00 P  0.026950 0.017780  0.313753 0.027254  P 0.0525270 0.0241572                                                                                                             
+24 314 60383.00 P  0.026768 0.017809  0.315682 0.027310  P 0.0522001 0.0242098                                                                                                             
+24 315 60384.00 P  0.026622 0.017838  0.317613 0.027366  P 0.0522693 0.0242624                                                                                                             
+24 316 60385.00 P  0.026512 0.017867  0.319545 0.027423  P 0.0526628 0.0243149                                                                                                             
+24 317 60386.00 P  0.026438 0.017896  0.321478 0.027479  P 0.0532734 0.0243674                                                                                                             
+24 318 60387.00 P  0.026400 0.017925  0.323412 0.027535  P 0.0539657 0.0244199                                                                                                             
+24 319 60388.00 P  0.026397 0.017953  0.325346 0.027591  P 0.0546456 0.0244723                                                                                                             
+24 320 60389.00 P  0.026430 0.017982  0.327279 0.027647  P 0.0552173 0.0245247                                                                                                             
+24 321 60390.00 P  0.026498 0.018011  0.329211 0.027702  P 0.0555947 0.0245770                                                                                                             
+24 322 60391.00 P  0.026602 0.018040  0.331142 0.027758  P 0.0557116 0.0246293                                                                                                             
+24 323 60392.00 P  0.026742 0.018068  0.333070 0.027814  P 0.0556182 0.0246816                                                                                                             
+24 324 60393.00 P  0.026916 0.018097  0.334995 0.027870  P 0.0553662 0.0247338                                                                                                             
+24 325 60394.00 P  0.027126 0.018126  0.336917 0.027926  P 0.0549364 0.0247860                                                                                                             
+24 326 60395.00 P  0.027371 0.018154  0.338835 0.027981  P 0.0545022 0.0248382                                                                                                             
+24 327 60396.00 P  0.027651 0.018183  0.340748 0.028037  P 0.0541737 0.0248903                                                                                                             
+24 328 60397.00 P  0.027966 0.018211  0.342657 0.028092  P 0.0540236 0.0249424                                                                                                             
+24 329 60398.00 P  0.028315 0.018240  0.344560 0.028148  P 0.0541015 0.0249945                                                                                                             
+24 330 60399.00 P  0.028699 0.018268  0.346457 0.028203  P 0.0544037 0.0250465                                                                                                             
+24 331 60400.00 P  0.029117 0.018297  0.348347 0.028259  P 0.0548837 0.0250985                                                                                                             
+24 4 1 60401.00 P  0.029569 0.018325  0.350230 0.028314  P 0.0555562 0.0251504                                                                                                             
+24 4 2 60402.00 P  0.030056 0.018354  0.352106 0.028370  P 0.0562120 0.0252023                                                                                                             
+24 4 3 60403.00 P  0.030576 0.018382  0.353973 0.028425  P 0.0567599 0.0252542                                                                                                             
+24 4 4 60404.00 P  0.031129 0.018410  0.355831 0.028480  P 0.0570555 0.0253060                                                                                                             
+24 4 5 60405.00 P  0.031716 0.018439  0.357681 0.028536  P 0.0570363 0.0253578                                                                                                             
+24 4 6 60406.00 P  0.032336 0.018467  0.359520 0.028591  P 0.0567030 0.0254096                                                                                                             
 24 4 7 60407.00                                                                                                                                                                            
 24 4 8 60408.00                                                                                                                                                                            
 24 4 9 60409.00                                                                                                                                                                            
 24 410 60410.00                                                                                                                                                                            
 24 411 60411.00                                                                                                                                                                            
 24 412 60412.00                                                                                                                                                                            
 24 413 60413.00                                                                                                                                                                            
@@ -18732,7 +18732,42 @@
 24 415 60415.00                                                                                                                                                                            
 24 416 60416.00                                                                                                                                                                            
 24 417 60417.00                                                                                                                                                                            
 24 418 60418.00                                                                                                                                                                            
 24 419 60419.00                                                                                                                                                                            
 24 420 60420.00                                                                                                                                                                            
 24 421 60421.00                                                                                                                                                                            
+24 422 60422.00                                                                                                                                                                            
+24 423 60423.00                                                                                                                                                                            
+24 424 60424.00                                                                                                                                                                            
+24 425 60425.00                                                                                                                                                                            
+24 426 60426.00                                                                                                                                                                            
+24 427 60427.00                                                                                                                                                                            
+24 428 60428.00                                                                                                                                                                            
+24 429 60429.00                                                                                                                                                                            
+24 430 60430.00                                                                                                                                                                            
+24 5 1 60431.00                                                                                                                                                                            
+24 5 2 60432.00                                                                                                                                                                            
+24 5 3 60433.00                                                                                                                                                                            
+24 5 4 60434.00                                                                                                                                                                            
+24 5 5 60435.00                                                                                                                                                                            
+24 5 6 60436.00                                                                                                                                                                            
+24 5 7 60437.00                                                                                                                                                                            
+24 5 8 60438.00                                                                                                                                                                            
+24 5 9 60439.00                                                                                                                                                                            
+24 510 60440.00                                                                                                                                                                            
+24 511 60441.00                                                                                                                                                                            
+24 512 60442.00                                                                                                                                                                            
+24 513 60443.00                                                                                                                                                                            
+24 514 60444.00                                                                                                                                                                            
+24 515 60445.00                                                                                                                                                                            
+24 516 60446.00                                                                                                                                                                            
+24 517 60447.00                                                                                                                                                                            
+24 518 60448.00                                                                                                                                                                            
+24 519 60449.00                                                                                                                                                                            
+24 520 60450.00                                                                                                                                                                            
+24 521 60451.00                                                                                                                                                                            
+24 522 60452.00                                                                                                                                                                            
+24 523 60453.00                                                                                                                                                                            
+24 524 60454.00                                                                                                                                                                            
+24 525 60455.00                                                                                                                                                                            
+24 526 60456.00
```

### Comparing `pyTMD-2.0.2/pyTMD/data/historic_deltat.data` & `pyTMD-2.0.3/pyTMD/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/data/iers_deltat.data` & `pyTMD-2.0.3/pyTMD/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/data/leap-seconds.list` & `pyTMD-2.0.3/pyTMD/data/leap-seconds.list`

 * *Files 2% similar despite different names*

```diff
@@ -200,18 +200,18 @@
 #	(whichever is later).
 #	If an announcement by the IERS specifies that no leap second is
 #	scheduled, then only the expiration date of the file will
 #	be advanced to show that the information in the file is still
 #	current -- the update time stamp, the data and the name of the file
 #	will not change.
 #
-#	Updated through IERS Bulletin C64
-#	File expires on:  28 June 2023
+#	Updated through IERS Bulletin C65
+#	File expires on:  28 December 2023
 #
-#@	3896899200
+#@	3912710400
 #
 2272060800	10	# 1 Jan 1972
 2287785600	11	# 1 Jul 1972
 2303683200	12	# 1 Jan 1973
 2335219200	13	# 1 Jan 1974
 2366755200	14	# 1 Jan 1975
 2398291200	15	# 1 Jan 1976
@@ -248,8 +248,8 @@
 #	in data lines. It includes the NTP values
 #	of both the last modification time and the
 #	expiration time of the file, but not the
 #	white space on those lines.
 #	the hash line is also ignored in the
 #	computation.
 #
-#h 	2c413af9 124e1031 f165174 ff527c6b 756ae00b
+#h 	e76a99dc 65f15cc7 e613e040 f5078b5e b23834fe
```

### Comparing `pyTMD-2.0.2/pyTMD/data/mean-pole.tab` & `pyTMD-2.0.3/pyTMD/data/mean-pole.tab`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/data/merged_deltat.data` & `pyTMD-2.0.3/pyTMD/data/merged_deltat.data`

 * *Files 1% similar despite different names*

```diff
@@ -7644,7 +7644,35 @@
  2023  3  3 69.1989
  2023  3  4 69.1987
  2023  3  5 69.1987
  2023  3  6 69.1989
  2023  3  7 69.1994
  2023  3  8 69.2000
  2023  3  9 69.2008
+ 2023  3 10 69.2016
+ 2023  3 11 69.2024
+ 2023  3 12 69.2031
+ 2023  3 13 69.2036
+ 2023  3 14 69.2039
+ 2023  3 15 69.2041
+ 2023  3 16 69.2041
+ 2023  3 17 69.2040
+ 2023  3 18 69.2041
+ 2023  3 19 69.2045
+ 2023  3 20 69.2051
+ 2023  3 21 69.2060
+ 2023  3 22 69.2069
+ 2023  3 23 69.2079
+ 2023  3 24 69.2087
+ 2023  3 25 69.2092
+ 2023  3 26 69.2094
+ 2023  3 27 69.2094
+ 2023  3 28 69.2092
+ 2023  3 29 69.2089
+ 2023  3 30 69.2086
+ 2023  3 31 69.2084
+ 2023  4  1 69.2083
+ 2023  4  2 69.2084
+ 2023  4  3 69.2087
+ 2023  4  4 69.2092
+ 2023  4  5 69.2098
+ 2023  4  6 69.2105
```

### Comparing `pyTMD-2.0.2/pyTMD/data/opoleloadcoefcmcor.txt.gz` & `pyTMD-2.0.3/pyTMD/data/opoleloadcoefcmcor.txt.gz`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/data/ser7.dat` & `pyTMD-2.0.3/pyTMD/data/ser7.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      9 March 2023                                        Vol. XXXVI No. 010   
+      6 April 2023                                        Vol. XXXVI No. 014   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
@@ -49,425 +49,518 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   23  3  3  60006 -.04665 .00009 0.32113 .00009 -0.014874 0.000011          
-   23  3  4  60007 -.04689 .00009 0.32382 .00009 -0.014686 0.000012          
-   23  3  5  60008 -.04656 .00009 0.32663 .00009 -0.014684 0.000012          
-   23  3  6  60009 -.04567 .00009 0.32982 .00009 -0.014948 0.000010          
-   23  3  7  60010 -.04460 .00009 0.33332 .00009 -0.015354 0.000010          
-   23  3  8  60011 -.04349 .00009 0.33664 .00009 -0.015999 0.000010          
-   23  3  9  60012 -.04235 .00009 0.33992 .00009 -0.016763 0.000055          
+   23  3 31  60034 -.02035 .00009 0.40219 .00009 -0.024413 0.000012          
+   23  4  1  60035 -.01885 .00009 0.40461 .00009 -0.024328 0.000012          
+   23  4  2  60036 -.01730 .00009 0.40738 .00009 -0.024399 0.000012          
+   23  4  3  60037 -.01561 .00009 0.41000 .00009 -0.024715 0.000008          
+   23  4  4  60038 -.01384 .00009 0.41265 .00009 -0.025218 0.000007          
+   23  4  5  60039 -.01224 .00009 0.41546 .00009 -0.025822 0.000007          
+   23  4  6  60040 -.01072 .00009 0.41839 .00009 -0.026508 0.000007          
+                                                                               
+                              IERS Final Values                                
+                               MJD        x        y      UT1-UTC              
+                                          "        "         s                 
+           23  2  2           59977   -0.0035   0.2503  -0.01386       
+           23  2  3           59978   -0.0049   0.2526  -0.01310       
+           23  2  4           59979   -0.0064   0.2543  -0.01242       
+           23  2  5           59980   -0.0082   0.2559  -0.01188       
+           23  2  6           59981   -0.0100   0.2577  -0.01150       
+           23  2  7           59982   -0.0119   0.2597  -0.01127       
+           23  2  8           59983   -0.0142   0.2617  -0.01120       
+           23  2  9           59984   -0.0158   0.2634  -0.01124       
+           23  2 10           59985   -0.0167   0.2655  -0.01147       
+           23  2 11           59986   -0.0178   0.2680  -0.01179       
+           23  2 12           59987   -0.0196   0.2704  -0.01213       
+           23  2 13           59988   -0.0219   0.2731  -0.01236       
+           23  2 14           59989   -0.0245   0.2757  -0.01246       
+           23  2 15           59990   -0.0270   0.2782  -0.01235       
+           23  2 16           59991   -0.0294   0.2807  -0.01206       
+           23  2 17           59992   -0.0318   0.2829  -0.01169       
+           23  2 18           59993   -0.0341   0.2849  -0.01136       
+           23  2 19           59994   -0.0359   0.2868  -0.01131       
+           23  2 20           59995   -0.0373   0.2889  -0.01157       
+           23  2 21           59996   -0.0383   0.2914  -0.01216       
+           23  2 22           59997   -0.0389   0.2946  -0.01293       
+           23  2 23           59998   -0.0390   0.2983  -0.01371       
+           23  2 24           59999   -0.0391   0.3019  -0.01450       
+           23  2 25           60000   -0.0396   0.3051  -0.01514       
+           23  2 26           60001   -0.0409   0.3082  -0.01554       
+           23  2 27           60002   -0.0428   0.3108  -0.01561       
+           23  2 28           60003   -0.0441   0.3133  -0.01550       
+           23  3  1           60004   -0.0451   0.3164  -0.01528       
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1417 - 0.1056 cos A - 0.0442 sin A - 0.0813 cos C + 0.0376 sin C  
-      y =  0.3512 - 0.0426 cos A + 0.0972 sin A + 0.0376 cos C + 0.0813 sin C  
-         UT1-UTC = -0.0170 + 0.00023 (MJD - 60020) - (UT2-UT1)                 
+      x =  0.1589 - 0.1152 cos A + 0.0163 sin A - 0.0532 cos C + 0.0623 sin C  
+      y =  0.3443 + 0.0143 cos A + 0.1096 sin A + 0.0623 cos C + 0.0532 sin C  
+         UT1-UTC = -0.0075 + 0.00020 (MJD - 60048) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60012)/365.25 and C = 2*pi*(MJD-60012)/435.          
+      where A = 2*pi*(MJD-60040)/365.25 and C = 2*pi*(MJD-60040)/435.          
                                                                                
-         TAI-UTC(MJD 60013) = 37.0                                             
+         TAI-UTC(MJD 60041) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60012)**0.80   S t = 0.00025 (MJD-60012)**0.75      
+      S x,y = 0.00068 (MJD-60040)**0.80   S t = 0.00025 (MJD-60040)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2023  3 10  60013      -0.0415      0.3431     -0.01751         
-       2023  3 11  60014      -0.0408      0.3463     -0.01821         
-       2023  3 12  60015      -0.0402      0.3493     -0.01879         
-       2023  3 13  60016      -0.0396      0.3521     -0.01918         
-       2023  3 14  60017      -0.0390      0.3549     -0.01934         
-       2023  3 15  60018      -0.0384      0.3576     -0.01928         
-       2023  3 16  60019      -0.0377      0.3603     -0.01909         
-       2023  3 17  60020      -0.0370      0.3630     -0.01892         
-       2023  3 18  60021      -0.0363      0.3657     -0.01891         
-       2023  3 19  60022      -0.0356      0.3683     -0.01922         
-       2023  3 20  60023      -0.0348      0.3710     -0.01989         
-       2023  3 21  60024      -0.0340      0.3737     -0.02085         
-       2023  3 22  60025      -0.0332      0.3763     -0.02200         
-       2023  3 23  60026      -0.0324      0.3790     -0.02314         
-       2023  3 24  60027      -0.0315      0.3816     -0.02412         
-       2023  3 25  60028      -0.0305      0.3842     -0.02486         
-       2023  3 26  60029      -0.0295      0.3868     -0.02531         
-       2023  3 27  60030      -0.0285      0.3894     -0.02551         
-       2023  3 28  60031      -0.0274      0.3920     -0.02553         
-       2023  3 29  60032      -0.0263      0.3946     -0.02543         
-       2023  3 30  60033      -0.0252      0.3971     -0.02530         
-       2023  3 31  60034      -0.0240      0.3996     -0.02521         
-       2023  4  1  60035      -0.0227      0.4021     -0.02523         
-       2023  4  2  60036      -0.0215      0.4046     -0.02541         
-       2023  4  3  60037      -0.0202      0.4071     -0.02578         
-       2023  4  4  60038      -0.0188      0.4095     -0.02632         
-       2023  4  5  60039      -0.0174      0.4120     -0.02700         
-       2023  4  6  60040      -0.0160      0.4144     -0.02774         
-       2023  4  7  60041      -0.0145      0.4168     -0.02847         
-       2023  4  8  60042      -0.0130      0.4191     -0.02909         
-       2023  4  9  60043      -0.0114      0.4215     -0.02952         
-       2023  4 10  60044      -0.0098      0.4238     -0.02971         
-       2023  4 11  60045      -0.0082      0.4261     -0.02968         
-       2023  4 12  60046      -0.0065      0.4283     -0.02951         
-       2023  4 13  60047      -0.0048      0.4305     -0.02929         
-       2023  4 14  60048      -0.0031      0.4328     -0.02917         
-       2023  4 15  60049      -0.0013      0.4349     -0.02928         
-       2023  4 16  60050       0.0005      0.4371     -0.02966         
-       2023  4 17  60051       0.0023      0.4392     -0.03031         
-       2023  4 18  60052       0.0042      0.4413     -0.03115         
-       2023  4 19  60053       0.0061      0.4434     -0.03204         
-       2023  4 20  60054       0.0080      0.4454     -0.03284         
-       2023  4 21  60055       0.0100      0.4474     -0.03344         
-       2023  4 22  60056       0.0120      0.4494     -0.03378         
-       2023  4 23  60057       0.0140      0.4514     -0.03384         
-       2023  4 24  60058       0.0161      0.4533     -0.03369         
-       2023  4 25  60059       0.0182      0.4552     -0.03340         
-       2023  4 26  60060       0.0203      0.4570     -0.03305         
-       2023  4 27  60061       0.0225      0.4589     -0.03273         
-       2023  4 28  60062       0.0246      0.4606     -0.03251         
-       2023  4 29  60063       0.0268      0.4624     -0.03244         
-       2023  4 30  60064       0.0291      0.4641     -0.03254         
-       2023  5  1  60065       0.0313      0.4658     -0.03280         
-       2023  5  2  60066       0.0336      0.4675     -0.03321         
-       2023  5  3  60067       0.0359      0.4691     -0.03372         
-       2023  5  4  60068       0.0383      0.4707     -0.03424         
-       2023  5  5  60069       0.0406      0.4722     -0.03468         
-       2023  5  6  60070       0.0430      0.4737     -0.03495         
-       2023  5  7  60071       0.0454      0.4752     -0.03499         
-       2023  5  8  60072       0.0478      0.4766     -0.03479         
-       2023  5  9  60073       0.0503      0.4780     -0.03440         
-       2023  5 10  60074       0.0528      0.4794     -0.03395         
-       2023  5 11  60075       0.0552      0.4807     -0.03355         
-       2023  5 12  60076       0.0578      0.4820     -0.03332         
-       2023  5 13  60077       0.0603      0.4833     -0.03335         
-       2023  5 14  60078       0.0628      0.4845     -0.03361         
-       2023  5 15  60079       0.0654      0.4856     -0.03406         
-       2023  5 16  60080       0.0680      0.4868     -0.03458         
-       2023  5 17  60081       0.0706      0.4879     -0.03505         
-       2023  5 18  60082       0.0732      0.4889     -0.03533         
-       2023  5 19  60083       0.0758      0.4899     -0.03536         
-       2023  5 20  60084       0.0784      0.4909     -0.03512         
-       2023  5 21  60085       0.0811      0.4918     -0.03464         
-       2023  5 22  60086       0.0837      0.4927     -0.03399         
-       2023  5 23  60087       0.0864      0.4936     -0.03324         
-       2023  5 24  60088       0.0891      0.4944     -0.03248         
-       2023  5 25  60089       0.0918      0.4952     -0.03178         
-       2023  5 26  60090       0.0945      0.4959     -0.03120         
-       2023  5 27  60091       0.0972      0.4966     -0.03078         
-       2023  5 28  60092       0.0999      0.4973     -0.03053         
-       2023  5 29  60093       0.1026      0.4979     -0.03043         
-       2023  5 30  60094       0.1054      0.4984     -0.03045         
-       2023  5 31  60095       0.1081      0.4990     -0.03051         
-       2023  6  1  60096       0.1109      0.4995     -0.03055         
-       2023  6  2  60097       0.1136      0.4999     -0.03045         
-       2023  6  3  60098       0.1164      0.5003     -0.03015         
-       2023  6  4  60099       0.1191      0.5007     -0.02960         
-       2023  6  5  60100       0.1219      0.5010     -0.02884         
-       2023  6  6  60101       0.1246      0.5013     -0.02796         
-       2023  6  7  60102       0.1274      0.5015     -0.02711         
-       2023  6  8  60103       0.1302      0.5017     -0.02640         
-       2023  6  9  60104       0.1329      0.5019     -0.02592         
-       2023  6 10  60105       0.1357      0.5020     -0.02567         
-       2023  6 11  60106       0.1385      0.5021     -0.02560         
-       2023  6 12  60107       0.1412      0.5021     -0.02560         
-       2023  6 13  60108       0.1440      0.5021     -0.02554         
-       2023  6 14  60109       0.1467      0.5020     -0.02531         
-       2023  6 15  60110       0.1495      0.5019     -0.02485         
-       2023  6 16  60111       0.1522      0.5018     -0.02413         
-       2023  6 17  60112       0.1549      0.5016     -0.02316         
-       2023  6 18  60113       0.1576      0.5014     -0.02199         
-       2023  6 19  60114       0.1604      0.5011     -0.02072         
-       2023  6 20  60115       0.1631      0.5008     -0.01940         
-       2023  6 21  60116       0.1658      0.5005     -0.01814         
-       2023  6 22  60117       0.1685      0.5001     -0.01698         
-       2023  6 23  60118       0.1711      0.4997     -0.01598         
-       2023  6 24  60119       0.1738      0.4992     -0.01514         
-       2023  6 25  60120       0.1765      0.4987     -0.01445         
-       2023  6 26  60121       0.1791      0.4982     -0.01387         
-       2023  6 27  60122       0.1817      0.4976     -0.01335         
-       2023  6 28  60123       0.1843      0.4970     -0.01284         
-       2023  6 29  60124       0.1869      0.4963     -0.01224         
-       2023  6 30  60125       0.1895      0.4956     -0.01148         
-       2023  7  1  60126       0.1921      0.4949     -0.01050         
-       2023  7  2  60127       0.1946      0.4941     -0.00932         
-       2023  7  3  60128       0.1972      0.4933     -0.00799         
-       2023  7  4  60129       0.1997      0.4925     -0.00665         
-       2023  7  5  60130       0.2022      0.4916     -0.00544         
-       2023  7  6  60131       0.2047      0.4907     -0.00448         
-       2023  7  7  60132       0.2071      0.4897     -0.00380         
-       2023  7  8  60133       0.2096      0.4887     -0.00335         
-       2023  7  9  60134       0.2120      0.4877     -0.00300         
-       2023  7 10  60135       0.2144      0.4866     -0.00262         
-       2023  7 11  60136       0.2168      0.4855     -0.00210         
-       2023  7 12  60137       0.2191      0.4844     -0.00135         
-       2023  7 13  60138       0.2215      0.4832     -0.00034         
-       2023  7 14  60139       0.2238      0.4820      0.00091         
-       2023  7 15  60140       0.2261      0.4807      0.00234         
-       2023  7 16  60141       0.2283      0.4795      0.00389         
-       2023  7 17  60142       0.2306      0.4781      0.00548         
-       2023  7 18  60143       0.2328      0.4768      0.00703         
-       2023  7 19  60144       0.2350      0.4754      0.00847         
-       2023  7 20  60145       0.2371      0.4740      0.00976         
-       2023  7 21  60146       0.2392      0.4726      0.01087         
-       2023  7 22  60147       0.2413      0.4711      0.01181         
-       2023  7 23  60148       0.2434      0.4696      0.01262         
-       2023  7 24  60149       0.2454      0.4681      0.01334         
-       2023  7 25  60150       0.2475      0.4665      0.01403         
-       2023  7 26  60151       0.2494      0.4649      0.01477         
-       2023  7 27  60152       0.2514      0.4633      0.01563         
-       2023  7 28  60153       0.2533      0.4616      0.01666         
-       2023  7 29  60154       0.2552      0.4600      0.01788         
-       2023  7 30  60155       0.2571      0.4583      0.01924         
-       2023  7 31  60156       0.2589      0.4565      0.02066         
-       2023  8  1  60157       0.2607      0.4548      0.02197         
-       2023  8  2  60158       0.2624      0.4530      0.02303         
-       2023  8  3  60159       0.2642      0.4512      0.02377         
-       2023  8  4  60160       0.2658      0.4493      0.02421         
-       2023  8  5  60161       0.2675      0.4475      0.02446         
-       2023  8  6  60162       0.2691      0.4456      0.02466         
-       2023  8  7  60163       0.2707      0.4437      0.02499         
-       2023  8  8  60164       0.2723      0.4418      0.02554         
-       2023  8  9  60165       0.2738      0.4398      0.02635         
-       2023  8 10  60166       0.2753      0.4378      0.02742         
-       2023  8 11  60167       0.2767      0.4358      0.02868         
-       2023  8 12  60168       0.2781      0.4338      0.03006         
-       2023  8 13  60169       0.2795      0.4318      0.03148         
-       2023  8 14  60170       0.2808      0.4297      0.03285         
-       2023  8 15  60171       0.2821      0.4277      0.03412         
-       2023  8 16  60172       0.2834      0.4256      0.03523         
-       2023  8 17  60173       0.2846      0.4235      0.03615         
-       2023  8 18  60174       0.2858      0.4213      0.03688         
-       2023  8 19  60175       0.2869      0.4192      0.03745         
-       2023  8 20  60176       0.2880      0.4170      0.03792         
-       2023  8 21  60177       0.2891      0.4148      0.03834         
-       2023  8 22  60178       0.2901      0.4127      0.03879         
-       2023  8 23  60179       0.2911      0.4104      0.03933         
-       2023  8 24  60180       0.2920      0.4082      0.04002         
-       2023  8 25  60181       0.2929      0.4060      0.04088         
-       2023  8 26  60182       0.2938      0.4038      0.04189         
-       2023  8 27  60183       0.2946      0.4015      0.04297         
-       2023  8 28  60184       0.2954      0.3992      0.04399         
-       2023  8 29  60185       0.2961      0.3970      0.04481         
-       2023  8 30  60186       0.2968      0.3947      0.04532         
-       2023  8 31  60187       0.2975      0.3924      0.04546         
-       2023  9  1  60188       0.2981      0.3901      0.04532         
-       2023  9  2  60189       0.2987      0.3878      0.04503         
-       2023  9  3  60190       0.2992      0.3854      0.04479         
-       2023  9  4  60191       0.2997      0.3831      0.04473         
-       2023  9  5  60192       0.3002      0.3808      0.04495         
-       2023  9  6  60193       0.3006      0.3784      0.04544         
-       2023  9  7  60194       0.3010      0.3761      0.04615         
-       2023  9  8  60195       0.3013      0.3738      0.04700         
-       2023  9  9  60196       0.3016      0.3714      0.04790         
-       2023  9 10  60197       0.3019      0.3690      0.04875         
-       2023  9 11  60198       0.3021      0.3667      0.04949         
-       2023  9 12  60199       0.3022      0.3643      0.05006         
-       2023  9 13  60200       0.3024      0.3620      0.05043         
-       2023  9 14  60201       0.3024      0.3596      0.05060         
-       2023  9 15  60202       0.3025      0.3573      0.05060         
-       2023  9 16  60203       0.3025      0.3549      0.05048         
-       2023  9 17  60204       0.3025      0.3525      0.05034         
-       2023  9 18  60205       0.3024      0.3502      0.05024         
-       2023  9 19  60206       0.3023      0.3478      0.05028         
-       2023  9 20  60207       0.3021      0.3455      0.05051         
-       2023  9 21  60208       0.3019      0.3431      0.05094         
-       2023  9 22  60209       0.3017      0.3408      0.05155         
-       2023  9 23  60210       0.3014      0.3385      0.05226         
-       2023  9 24  60211       0.3011      0.3361      0.05295         
-       2023  9 25  60212       0.3007      0.3338      0.05347         
-       2023  9 26  60213       0.3003      0.3315      0.05369         
-       2023  9 27  60214       0.2999      0.3292      0.05353         
-       2023  9 28  60215       0.2994      0.3269      0.05302         
-       2023  9 29  60216       0.2989      0.3246      0.05226         
-       2023  9 30  60217       0.2983      0.3223      0.05144         
-       2023 10  1  60218       0.2977      0.3201      0.05075         
-       2023 10  2  60219       0.2971      0.3178      0.05035         
-       2023 10  3  60220       0.2964      0.3156      0.05028         
-       2023 10  4  60221       0.2957      0.3133      0.05053         
-       2023 10  5  60222       0.2949      0.3111      0.05103         
-       2023 10  6  60223       0.2942      0.3089      0.05167         
-       2023 10  7  60224       0.2933      0.3067      0.05234         
-       2023 10  8  60225       0.2925      0.3045      0.05294         
-       2023 10  9  60226       0.2916      0.3023      0.05341         
-       2023 10 10  60227       0.2906      0.3002      0.05372         
-       2023 10 11  60228       0.2897      0.2980      0.05386         
-       2023 10 12  60229       0.2887      0.2959      0.05387         
-       2023 10 13  60230       0.2876      0.2938      0.05375         
-       2023 10 14  60231       0.2866      0.2917      0.05356         
-       2023 10 15  60232       0.2854      0.2897      0.05334         
-       2023 10 16  60233       0.2843      0.2876      0.05317         
-       2023 10 17  60234       0.2831      0.2856      0.05311         
-       2023 10 18  60235       0.2819      0.2836      0.05317         
-       2023 10 19  60236       0.2807      0.2816      0.05332         
-       2023 10 20  60237       0.2794      0.2796      0.05354         
-       2023 10 21  60238       0.2781      0.2777      0.05373         
-       2023 10 22  60239       0.2768      0.2757      0.05384         
-       2023 10 23  60240       0.2754      0.2738      0.05376         
-       2023 10 24  60241       0.2740      0.2719      0.05340         
-       2023 10 25  60242       0.2726      0.2701      0.05276         
-       2023 10 26  60243       0.2711      0.2682      0.05188         
-       2023 10 27  60244       0.2696      0.2664      0.05086         
-       2023 10 28  60245       0.2681      0.2646      0.04992         
-       2023 10 29  60246       0.2665      0.2629      0.04916         
-       2023 10 30  60247       0.2650      0.2611      0.04867         
-       2023 10 31  60248       0.2634      0.2594      0.04847         
-       2023 11  1  60249       0.2617      0.2577      0.04858         
-       2023 11  2  60250       0.2601      0.2561      0.04883         
-       2023 11  3  60251       0.2584      0.2544      0.04917         
-       2023 11  4  60252       0.2567      0.2528      0.04950         
-       2023 11  5  60253       0.2549      0.2512      0.04965         
-       2023 11  6  60254       0.2532      0.2497      0.04961         
-       2023 11  7  60255       0.2514      0.2482      0.04943         
-       2023 11  8  60256       0.2496      0.2467      0.04916         
-       2023 11  9  60257       0.2478      0.2452      0.04878         
-       2023 11 10  60258       0.2459      0.2438      0.04835         
-       2023 11 11  60259       0.2440      0.2423      0.04791         
-       2023 11 12  60260       0.2422      0.2410      0.04754         
-       2023 11 13  60261       0.2402      0.2396      0.04736         
-       2023 11 14  60262       0.2383      0.2383      0.04734         
-       2023 11 15  60263       0.2364      0.2370      0.04754         
-       2023 11 16  60264       0.2344      0.2358      0.04788         
-       2023 11 17  60265       0.2324      0.2345      0.04830         
-       2023 11 18  60266       0.2304      0.2333      0.04863         
-       2023 11 19  60267       0.2284      0.2322      0.04888         
-       2023 11 20  60268       0.2263      0.2311      0.04877         
-       2023 11 21  60269       0.2243      0.2300      0.04839         
-       2023 11 22  60270       0.2222      0.2289      0.04780         
-       2023 11 23  60271       0.2201      0.2279      0.04706         
-       2023 11 24  60272       0.2180      0.2269      0.04630         
-       2023 11 25  60273       0.2159      0.2259      0.04565         
-       2023 11 26  60274       0.2138      0.2250      0.04526         
-       2023 11 27  60275       0.2116      0.2241      0.04512         
-       2023 11 28  60276       0.2095      0.2232      0.04527         
-       2023 11 29  60277       0.2073      0.2224      0.04569         
-       2023 11 30  60278       0.2052      0.2216      0.04629         
-       2023 12  1  60279       0.2030      0.2208      0.04686         
-       2023 12  2  60280       0.2008      0.2201      0.04739         
-       2023 12  3  60281       0.1986      0.2194      0.04780         
-       2023 12  4  60282       0.1964      0.2188      0.04804         
-       2023 12  5  60283       0.1942      0.2181      0.04813         
-       2023 12  6  60284       0.1920      0.2176      0.04816         
-       2023 12  7  60285       0.1897      0.2170      0.04808         
-       2023 12  8  60286       0.1875      0.2165      0.04799         
-       2023 12  9  60287       0.1853      0.2160      0.04797         
-       2023 12 10  60288       0.1830      0.2156      0.04802         
-       2023 12 11  60289       0.1808      0.2151      0.04823         
-       2023 12 12  60290       0.1785      0.2148      0.04869         
-       2023 12 13  60291       0.1763      0.2144      0.04936         
-       2023 12 14  60292       0.1740      0.2141      0.05012         
-       2023 12 15  60293       0.1718      0.2139      0.05089         
-       2023 12 16  60294       0.1695      0.2136      0.05154         
-       2023 12 17  60295       0.1673      0.2134      0.05192         
-       2023 12 18  60296       0.1651      0.2133      0.05196         
-       2023 12 19  60297       0.1628      0.2131      0.05172         
-       2023 12 20  60298       0.1606      0.2130      0.05133         
-       2023 12 21  60299       0.1583      0.2130      0.05095         
-       2023 12 22  60300       0.1561      0.2130      0.05071         
-       2023 12 23  60301       0.1539      0.2130      0.05068         
-       2023 12 24  60302       0.1516      0.2130      0.05095         
-       2023 12 25  60303       0.1494      0.2131      0.05140         
-       2023 12 26  60304       0.1472      0.2132      0.05207         
-       2023 12 27  60305       0.1450      0.2134      0.05287         
-       2023 12 28  60306       0.1428      0.2136      0.05363         
-       2023 12 29  60307       0.1406      0.2138      0.05435         
-       2023 12 30  60308       0.1384      0.2140      0.05497         
-       2023 12 31  60309       0.1362      0.2143      0.05544         
-       2024  1  1  60310       0.1341      0.2147      0.05574         
-       2024  1  2  60311       0.1319      0.2150      0.05587         
-       2024  1  3  60312       0.1298      0.2154      0.05583         
-       2024  1  4  60313       0.1276      0.2158      0.05568         
-       2024  1  5  60314       0.1255      0.2163      0.05549         
-       2024  1  6  60315       0.1234      0.2168      0.05534         
-       2024  1  7  60316       0.1213      0.2173      0.05531         
-       2024  1  8  60317       0.1192      0.2179      0.05545         
-       2024  1  9  60318       0.1172      0.2184      0.05577         
-       2024  1 10  60319       0.1151      0.2191      0.05618         
-       2024  1 11  60320       0.1131      0.2197      0.05660         
-       2024  1 12  60321       0.1111      0.2204      0.05687         
-       2024  1 13  60322       0.1091      0.2211      0.05687         
-       2024  1 14  60323       0.1071      0.2219      0.05650         
-       2024  1 15  60324       0.1051      0.2226      0.05582         
-       2024  1 16  60325       0.1032      0.2235      0.05500         
-       2024  1 17  60326       0.1012      0.2243      0.05421         
-       2024  1 18  60327       0.0993      0.2252      0.05361         
-       2024  1 19  60328       0.0974      0.2261      0.05324         
-       2024  1 20  60329       0.0956      0.2270      0.05317         
-       2024  1 21  60330       0.0937      0.2279      0.05335         
-       2024  1 22  60331       0.0919      0.2289      0.05379         
-       2024  1 23  60332       0.0901      0.2299      0.05441         
-       2024  1 24  60333       0.0883      0.2310      0.05510         
-       2024  1 25  60334       0.0865      0.2321      0.05573         
-       2024  1 26  60335       0.0848      0.2332      0.05622         
-       2024  1 27  60336       0.0831      0.2343      0.05658         
-       2024  1 28  60337       0.0814      0.2354      0.05676         
-       2024  1 29  60338       0.0797      0.2366      0.05677         
-       2024  1 30  60339       0.0781      0.2378      0.05681         
-       2024  1 31  60340       0.0765      0.2390      0.05692         
-       2024  2  1  60341       0.0749      0.2403      0.05710         
-       2024  2  2  60342       0.0733      0.2416      0.05742         
-       2024  2  3  60343       0.0718      0.2429      0.05788         
-       2024  2  4  60344       0.0703      0.2442      0.05851         
-       2024  2  5  60345       0.0688      0.2455      0.05931         
-       2024  2  6  60346       0.0673      0.2469      0.06025         
-       2024  2  7  60347       0.0659      0.2483      0.06123         
-       2024  2  8  60348       0.0645      0.2497      0.06208         
-       2024  2  9  60349       0.0631      0.2512      0.06263         
-       2024  2 10  60350       0.0618      0.2526      0.06282         
-       2024  2 11  60351       0.0605      0.2541      0.06265         
-       2024  2 12  60352       0.0592      0.2556      0.06212         
-       2024  2 13  60353       0.0580      0.2571      0.06150         
-       2024  2 14  60354       0.0567      0.2587      0.06100         
-       2024  2 15  60355       0.0555      0.2602      0.06078         
-       2024  2 16  60356       0.0544      0.2618      0.06092         
-       2024  2 17  60357       0.0533      0.2634      0.06140         
-       2024  2 18  60358       0.0522      0.2650      0.06211         
-       2024  2 19  60359       0.0511      0.2666      0.06304         
-       2024  2 20  60360       0.0501      0.2683      0.06396         
-       2024  2 21  60361       0.0491      0.2699      0.06483         
-       2024  2 22  60362       0.0481      0.2716      0.06554         
-       2024  2 23  60363       0.0472      0.2733      0.06610         
-       2024  2 24  60364       0.0462      0.2750      0.06651         
-       2024  2 25  60365       0.0454      0.2767      0.06680         
-       2024  2 26  60366       0.0445      0.2784      0.06695         
-       2024  2 27  60367       0.0437      0.2802      0.06695         
-       2024  2 28  60368       0.0430      0.2819      0.06698         
-       2024  2 29  60369       0.0422      0.2837      0.06708         
-       2024  3  1  60370       0.0415      0.2855      0.06734         
-       2024  3  2  60371       0.0409      0.2873      0.06776         
-       2024  3  3  60372       0.0402      0.2891      0.06839         
-       2024  3  4  60373       0.0396      0.2909      0.06916         
-       2024  3  5  60374       0.0391      0.2927      0.06991         
-       2024  3  6  60375       0.0385      0.2945      0.07064         
-       2024  3  7  60376       0.0380      0.2963      0.07124         
-       2024  3  8  60377       0.0376      0.2982      0.07153         
+       2023  4  7  60041      -0.0092      0.4211     -0.02720         
+       2023  4  8  60042      -0.0077      0.4237     -0.02785         
+       2023  4  9  60043      -0.0061      0.4261     -0.02836         
+       2023  4 10  60044      -0.0044      0.4285     -0.02868         
+       2023  4 11  60045      -0.0027      0.4307     -0.02882         
+       2023  4 12  60046      -0.0010      0.4329     -0.02880         
+       2023  4 13  60047       0.0008      0.4351     -0.02875         
+       2023  4 14  60048       0.0026      0.4372     -0.02879         
+       2023  4 15  60049       0.0045      0.4393     -0.02904         
+       2023  4 16  60050       0.0064      0.4413     -0.02959         
+       2023  4 17  60051       0.0083      0.4434     -0.03041         
+       2023  4 18  60052       0.0102      0.4454     -0.03137         
+       2023  4 19  60053       0.0122      0.4474     -0.03233         
+       2023  4 20  60054       0.0142      0.4494     -0.03318         
+       2023  4 21  60055       0.0162      0.4513     -0.03378         
+       2023  4 22  60056       0.0183      0.4532     -0.03410         
+       2023  4 23  60057       0.0203      0.4550     -0.03413         
+       2023  4 24  60058       0.0224      0.4568     -0.03392         
+       2023  4 25  60059       0.0246      0.4586     -0.03355         
+       2023  4 26  60060       0.0267      0.4603     -0.03311         
+       2023  4 27  60061       0.0289      0.4620     -0.03270         
+       2023  4 28  60062       0.0311      0.4637     -0.03238         
+       2023  4 29  60063       0.0334      0.4653     -0.03222         
+       2023  4 30  60064       0.0357      0.4669     -0.03226         
+       2023  5  1  60065       0.0379      0.4684     -0.03249         
+       2023  5  2  60066       0.0403      0.4700     -0.03289         
+       2023  5  3  60067       0.0426      0.4714     -0.03341         
+       2023  5  4  60068       0.0450      0.4729     -0.03395         
+       2023  5  5  60069       0.0473      0.4743     -0.03443         
+       2023  5  6  60070       0.0498      0.4757     -0.03474         
+       2023  5  7  60071       0.0522      0.4770     -0.03483         
+       2023  5  8  60072       0.0546      0.4783     -0.03468         
+       2023  5  9  60073       0.0571      0.4796     -0.03435         
+       2023  5 10  60074       0.0596      0.4808     -0.03395         
+       2023  5 11  60075       0.0621      0.4820     -0.03360         
+       2023  5 12  60076       0.0646      0.4831     -0.03341         
+       2023  5 13  60077       0.0672      0.4842     -0.03346         
+       2023  5 14  60078       0.0697      0.4853     -0.03375         
+       2023  5 15  60079       0.0723      0.4863     -0.03421         
+       2023  5 16  60080       0.0749      0.4873     -0.03473         
+       2023  5 17  60081       0.0775      0.4883     -0.03518         
+       2023  5 18  60082       0.0801      0.4892     -0.03544         
+       2023  5 19  60083       0.0827      0.4900     -0.03544         
+       2023  5 20  60084       0.0854      0.4909     -0.03516         
+       2023  5 21  60085       0.0880      0.4917     -0.03462         
+       2023  5 22  60086       0.0907      0.4924     -0.03389         
+       2023  5 23  60087       0.0933      0.4931     -0.03304         
+       2023  5 24  60088       0.0960      0.4938     -0.03217         
+       2023  5 25  60089       0.0987      0.4944     -0.03136         
+       2023  5 26  60090       0.1014      0.4950     -0.03065         
+       2023  5 27  60091       0.1041      0.4956     -0.03010         
+       2023  5 28  60092       0.1068      0.4961     -0.02971         
+       2023  5 29  60093       0.1096      0.4965     -0.02947         
+       2023  5 30  60094       0.1123      0.4970     -0.02935         
+       2023  5 31  60095       0.1150      0.4973     -0.02928         
+       2023  6  1  60096       0.1177      0.4977     -0.02918         
+       2023  6  2  60097       0.1205      0.4980     -0.02896         
+       2023  6  3  60098       0.1232      0.4982     -0.02855         
+       2023  6  4  60099       0.1260      0.4984     -0.02789         
+       2023  6  5  60100       0.1287      0.4986     -0.02704         
+       2023  6  6  60101       0.1314      0.4988     -0.02608         
+       2023  6  7  60102       0.1342      0.4988     -0.02515         
+       2023  6  8  60103       0.1369      0.4989     -0.02438         
+       2023  6  9  60104       0.1397      0.4989     -0.02385         
+       2023  6 10  60105       0.1424      0.4989     -0.02357         
+       2023  6 11  60106       0.1451      0.4988     -0.02347         
+       2023  6 12  60107       0.1478      0.4987     -0.02343         
+       2023  6 13  60108       0.1506      0.4985     -0.02335         
+       2023  6 14  60109       0.1533      0.4983     -0.02310         
+       2023  6 15  60110       0.1560      0.4981     -0.02261         
+       2023  6 16  60111       0.1587      0.4978     -0.02186         
+       2023  6 17  60112       0.1614      0.4975     -0.02087         
+       2023  6 18  60113       0.1641      0.4971     -0.01968         
+       2023  6 19  60114       0.1667      0.4967     -0.01837         
+       2023  6 20  60115       0.1694      0.4963     -0.01702         
+       2023  6 21  60116       0.1721      0.4958     -0.01571         
+       2023  6 22  60117       0.1747      0.4953     -0.01451         
+       2023  6 23  60118       0.1773      0.4947     -0.01346         
+       2023  6 24  60119       0.1799      0.4942     -0.01258         
+       2023  6 25  60120       0.1826      0.4935     -0.01185         
+       2023  6 26  60121       0.1851      0.4928     -0.01125         
+       2023  6 27  60122       0.1877      0.4921     -0.01073         
+       2023  6 28  60123       0.1903      0.4914     -0.01020         
+       2023  6 29  60124       0.1928      0.4906     -0.00960         
+       2023  6 30  60125       0.1954      0.4897     -0.00884         
+       2023  7  1  60126       0.1979      0.4889     -0.00786         
+       2023  7  2  60127       0.2004      0.4880     -0.00669         
+       2023  7  3  60128       0.2028      0.4870     -0.00538         
+       2023  7  4  60129       0.2053      0.4861     -0.00406         
+       2023  7  5  60130       0.2077      0.4850     -0.00289         
+       2023  7  6  60131       0.2101      0.4840     -0.00196         
+       2023  7  7  60132       0.2125      0.4829     -0.00132         
+       2023  7  8  60133       0.2149      0.4818     -0.00091         
+       2023  7  9  60134       0.2173      0.4806     -0.00061         
+       2023  7 10  60135       0.2196      0.4794     -0.00029         
+       2023  7 11  60136       0.2219      0.4782      0.00018         
+       2023  7 12  60137       0.2242      0.4769      0.00087         
+       2023  7 13  60138       0.2264      0.4756      0.00181         
+       2023  7 14  60139       0.2286      0.4743      0.00299         
+       2023  7 15  60140       0.2309      0.4730      0.00435         
+       2023  7 16  60141       0.2330      0.4716      0.00584         
+       2023  7 17  60142       0.2352      0.4701      0.00737         
+       2023  7 18  60143       0.2373      0.4687      0.00887         
+       2023  7 19  60144       0.2394      0.4672      0.01026         
+       2023  7 20  60145       0.2415      0.4657      0.01150         
+       2023  7 21  60146       0.2435      0.4641      0.01257         
+       2023  7 22  60147       0.2455      0.4625      0.01348         
+       2023  7 23  60148       0.2475      0.4609      0.01426         
+       2023  7 24  60149       0.2494      0.4593      0.01496         
+       2023  7 25  60150       0.2514      0.4576      0.01565         
+       2023  7 26  60151       0.2532      0.4559      0.01639         
+       2023  7 27  60152       0.2551      0.4542      0.01724         
+       2023  7 28  60153       0.2569      0.4524      0.01827         
+       2023  7 29  60154       0.2587      0.4507      0.01949         
+       2023  7 30  60155       0.2605      0.4489      0.02086         
+       2023  7 31  60156       0.2622      0.4470      0.02227         
+       2023  8  1  60157       0.2639      0.4452      0.02358         
+       2023  8  2  60158       0.2655      0.4433      0.02465         
+       2023  8  3  60159       0.2671      0.4414      0.02540         
+       2023  8  4  60160       0.2687      0.4395      0.02584         
+       2023  8  5  60161       0.2703      0.4375      0.02608         
+       2023  8  6  60162       0.2718      0.4356      0.02629         
+       2023  8  7  60163       0.2733      0.4336      0.02662         
+       2023  8  8  60164       0.2747      0.4315      0.02717         
+       2023  8  9  60165       0.2761      0.4295      0.02798         
+       2023  8 10  60166       0.2775      0.4275      0.02905         
+       2023  8 11  60167       0.2788      0.4254      0.03030         
+       2023  8 12  60168       0.2801      0.4233      0.03168         
+       2023  8 13  60169       0.2813      0.4212      0.03310         
+       2023  8 14  60170       0.2825      0.4191      0.03447         
+       2023  8 15  60171       0.2837      0.4169      0.03574         
+       2023  8 16  60172       0.2849      0.4147      0.03684         
+       2023  8 17  60173       0.2859      0.4126      0.03776         
+       2023  8 18  60174       0.2870      0.4104      0.03849         
+       2023  8 19  60175       0.2880      0.4082      0.03907         
+       2023  8 20  60176       0.2890      0.4059      0.03953         
+       2023  8 21  60177       0.2899      0.4037      0.03996         
+       2023  8 22  60178       0.2908      0.4015      0.04041         
+       2023  8 23  60179       0.2917      0.3992      0.04097         
+       2023  8 24  60180       0.2925      0.3969      0.04166         
+       2023  8 25  60181       0.2933      0.3946      0.04254         
+       2023  8 26  60182       0.2940      0.3923      0.04356         
+       2023  8 27  60183       0.2947      0.3900      0.04465         
+       2023  8 28  60184       0.2954      0.3877      0.04570         
+       2023  8 29  60185       0.2960      0.3854      0.04654         
+       2023  8 30  60186       0.2965      0.3831      0.04706         
+       2023  8 31  60187       0.2971      0.3807      0.04723         
+       2023  9  1  60188       0.2975      0.3784      0.04711         
+       2023  9  2  60189       0.2980      0.3761      0.04686         
+       2023  9  3  60190       0.2984      0.3737      0.04664         
+       2023  9  4  60191       0.2987      0.3713      0.04662         
+       2023  9  5  60192       0.2991      0.3690      0.04688         
+       2023  9  6  60193       0.2993      0.3666      0.04742         
+       2023  9  7  60194       0.2996      0.3643      0.04818         
+       2023  9  8  60195       0.2998      0.3619      0.04910         
+       2023  9  9  60196       0.2999      0.3595      0.05007         
+       2023  9 10  60197       0.3000      0.3571      0.05102         
+       2023  9 11  60198       0.3001      0.3548      0.05187         
+       2023  9 12  60199       0.3001      0.3524      0.05256         
+       2023  9 13  60200       0.3001      0.3500      0.05307         
+       2023  9 14  60201       0.3000      0.3477      0.05337         
+       2023  9 15  60202       0.2999      0.3453      0.05351         
+       2023  9 16  60203       0.2998      0.3429      0.05352         
+       2023  9 17  60204       0.2996      0.3406      0.05347         
+       2023  9 18  60205       0.2994      0.3382      0.05343         
+       2023  9 19  60206       0.2991      0.3359      0.05349         
+       2023  9 20  60207       0.2988      0.3335      0.05369         
+       2023  9 21  60208       0.2985      0.3312      0.05406         
+       2023  9 22  60209       0.2981      0.3288      0.05459         
+       2023  9 23  60210       0.2977      0.3265      0.05522         
+       2023  9 24  60211       0.2972      0.3242      0.05583         
+       2023  9 25  60212       0.2967      0.3219      0.05631         
+       2023  9 26  60213       0.2961      0.3196      0.05651         
+       2023  9 27  60214       0.2956      0.3173      0.05637         
+       2023  9 28  60215       0.2949      0.3150      0.05589         
+       2023  9 29  60216       0.2943      0.3128      0.05517         
+       2023  9 30  60217       0.2936      0.3105      0.05440         
+       2023 10  1  60218       0.2928      0.3083      0.05375         
+       2023 10  2  60219       0.2920      0.3060      0.05334         
+       2023 10  3  60220       0.2912      0.3038      0.05322         
+       2023 10  4  60221       0.2904      0.3016      0.05338         
+       2023 10  5  60222       0.2895      0.2994      0.05372         
+       2023 10  6  60223       0.2885      0.2972      0.05416         
+       2023 10  7  60224       0.2876      0.2951      0.05460         
+       2023 10  8  60225       0.2866      0.2929      0.05494         
+       2023 10  9  60226       0.2855      0.2908      0.05513         
+       2023 10 10  60227       0.2844      0.2887      0.05512         
+       2023 10 11  60228       0.2833      0.2866      0.05491         
+       2023 10 12  60229       0.2822      0.2845      0.05450         
+       2023 10 13  60230       0.2810      0.2825      0.05393         
+       2023 10 14  60231       0.2798      0.2805      0.05327         
+       2023 10 15  60232       0.2785      0.2784      0.05259         
+       2023 10 16  60233       0.2772      0.2765      0.05199         
+       2023 10 17  60234       0.2759      0.2745      0.05154         
+       2023 10 18  60235       0.2745      0.2725      0.05128         
+       2023 10 19  60236       0.2732      0.2706      0.05123         
+       2023 10 20  60237       0.2717      0.2687      0.05133         
+       2023 10 21  60238       0.2703      0.2668      0.05151         
+       2023 10 22  60239       0.2688      0.2650      0.05164         
+       2023 10 23  60240       0.2673      0.2631      0.05161         
+       2023 10 24  60241       0.2658      0.2613      0.05134         
+       2023 10 25  60242       0.2642      0.2595      0.05080         
+       2023 10 26  60243       0.2626      0.2578      0.05006         
+       2023 10 27  60244       0.2610      0.2560      0.04923         
+       2023 10 28  60245       0.2593      0.2543      0.04847         
+       2023 10 29  60246       0.2576      0.2526      0.04793         
+       2023 10 30  60247       0.2559      0.2510      0.04769         
+       2023 10 31  60248       0.2542      0.2494      0.04777         
+       2023 11  1  60249       0.2524      0.2478      0.04811         
+       2023 11  2  60250       0.2506      0.2462      0.04862         
+       2023 11  3  60251       0.2488      0.2446      0.04920         
+       2023 11  4  60252       0.2469      0.2431      0.04975         
+       2023 11  5  60253       0.2451      0.2416      0.05018         
+       2023 11  6  60254       0.2432      0.2402      0.05042         
+       2023 11  7  60255       0.2413      0.2388      0.05046         
+       2023 11  8  60256       0.2393      0.2374      0.05029         
+       2023 11  9  60257       0.2374      0.2360      0.04994         
+       2023 11 10  60258       0.2354      0.2347      0.04948         
+       2023 11 11  60259       0.2334      0.2334      0.04896         
+       2023 11 12  60260       0.2314      0.2321      0.04849         
+       2023 11 13  60261       0.2294      0.2309      0.04813         
+       2023 11 14  60262       0.2273      0.2296      0.04794         
+       2023 11 15  60263       0.2252      0.2285      0.04794         
+       2023 11 16  60264       0.2231      0.2273      0.04812         
+       2023 11 17  60265       0.2210      0.2262      0.04837         
+       2023 11 18  60266       0.2189      0.2251      0.04857         
+       2023 11 19  60267       0.2168      0.2241      0.04858         
+       2023 11 20  60268       0.2146      0.2231      0.04835         
+       2023 11 21  60269       0.2124      0.2221      0.04782         
+       2023 11 22  60270       0.2102      0.2212      0.04708         
+       2023 11 23  60271       0.2080      0.2203      0.04621         
+       2023 11 24  60272       0.2058      0.2194      0.04536         
+       2023 11 25  60273       0.2036      0.2186      0.04468         
+       2023 11 26  60274       0.2014      0.2178      0.04431         
+       2023 11 27  60275       0.1991      0.2170      0.04427         
+       2023 11 28  60276       0.1969      0.2163      0.04459         
+       2023 11 29  60277       0.1946      0.2156      0.04512         
+       2023 11 30  60278       0.1923      0.2149      0.04580         
+       2023 12  1  60279       0.1901      0.2143      0.04645         
+       2023 12  2  60280       0.1878      0.2137      0.04703         
+       2023 12  3  60281       0.1855      0.2131      0.04744         
+       2023 12  4  60282       0.1832      0.2126      0.04764         
+       2023 12  5  60283       0.1809      0.2121      0.04776         
+       2023 12  6  60284       0.1785      0.2117      0.04778         
+       2023 12  7  60285       0.1762      0.2113      0.04776         
+       2023 12  8  60286       0.1739      0.2109      0.04769         
+       2023 12  9  60287       0.1716      0.2106      0.04768         
+       2023 12 10  60288       0.1693      0.2103      0.04772         
+       2023 12 11  60289       0.1669      0.2100      0.04790         
+       2023 12 12  60290       0.1646      0.2098      0.04825         
+       2023 12 13  60291       0.1623      0.2096      0.04872         
+       2023 12 14  60292       0.1599      0.2094      0.04921         
+       2023 12 15  60293       0.1576      0.2093      0.04962         
+       2023 12 16  60294       0.1553      0.2092      0.04983         
+       2023 12 17  60295       0.1530      0.2092      0.04982         
+       2023 12 18  60296       0.1506      0.2092      0.04954         
+       2023 12 19  60297       0.1483      0.2092      0.04902         
+       2023 12 20  60298       0.1460      0.2092      0.04840         
+       2023 12 21  60299       0.1437      0.2093      0.04779         
+       2023 12 22  60300       0.1414      0.2095      0.04727         
+       2023 12 23  60301       0.1391      0.2096      0.04702         
+       2023 12 24  60302       0.1368      0.2098      0.04702         
+       2023 12 25  60303       0.1345      0.2101      0.04726         
+       2023 12 26  60304       0.1322      0.2104      0.04770         
+       2023 12 27  60305       0.1300      0.2107      0.04832         
+       2023 12 28  60306       0.1277      0.2110      0.04893         
+       2023 12 29  60307       0.1255      0.2114      0.04953         
+       2023 12 30  60308       0.1232      0.2118      0.05002         
+       2023 12 31  60309       0.1210      0.2122      0.05028         
+       2024  1  1  60310       0.1188      0.2127      0.05033         
+       2024  1  2  60311       0.1166      0.2132      0.05027         
+       2024  1  3  60312       0.1144      0.2138      0.05018         
+       2024  1  4  60313       0.1122      0.2144      0.05006         
+       2024  1  5  60314       0.1101      0.2150      0.04999         
+       2024  1  6  60315       0.1079      0.2156      0.05001         
+       2024  1  7  60316       0.1058      0.2163      0.05017         
+       2024  1  8  60317       0.1037      0.2170      0.05056         
+       2024  1  9  60318       0.1016      0.2178      0.05111         
+       2024  1 10  60319       0.0995      0.2186      0.05180         
+       2024  1 11  60320       0.0974      0.2194      0.05249         
+       2024  1 12  60321       0.0954      0.2202      0.05307         
+       2024  1 13  60322       0.0934      0.2211      0.05336         
+       2024  1 14  60323       0.0913      0.2220      0.05342         
+       2024  1 15  60324       0.0894      0.2230      0.05308         
+       2024  1 16  60325       0.0874      0.2239      0.05256         
+       2024  1 17  60326       0.0854      0.2249      0.05204         
+       2024  1 18  60327       0.0835      0.2259      0.05161         
+       2024  1 19  60328       0.0816      0.2270      0.05138         
+       2024  1 20  60329       0.0797      0.2281      0.05139         
+       2024  1 21  60330       0.0779      0.2292      0.05167         
+       2024  1 22  60331       0.0760      0.2303      0.05213         
+       2024  1 23  60332       0.0742      0.2315      0.05274         
+       2024  1 24  60333       0.0724      0.2327      0.05345         
+       2024  1 25  60334       0.0707      0.2339      0.05419         
+       2024  1 26  60335       0.0689      0.2352      0.05478         
+       2024  1 27  60336       0.0672      0.2365      0.05524         
+       2024  1 28  60337       0.0655      0.2378      0.05554         
+       2024  1 29  60338       0.0639      0.2391      0.05567         
+       2024  1 30  60339       0.0622      0.2405      0.05567         
+       2024  1 31  60340       0.0606      0.2419      0.05568         
+       2024  2  1  60341       0.0590      0.2433      0.05568         
+       2024  2  2  60342       0.0575      0.2447      0.05575         
+       2024  2  3  60343       0.0560      0.2461      0.05598         
+       2024  2  4  60344       0.0545      0.2476      0.05632         
+       2024  2  5  60345       0.0530      0.2491      0.05682         
+       2024  2  6  60346       0.0516      0.2506      0.05751         
+       2024  2  7  60347       0.0502      0.2522      0.05828         
+       2024  2  8  60348       0.0488      0.2537      0.05896         
+       2024  2  9  60349       0.0475      0.2553      0.05944         
+       2024  2 10  60350       0.0462      0.2569      0.05961         
+       2024  2 11  60351       0.0449      0.2586      0.05941         
+       2024  2 12  60352       0.0436      0.2602      0.05887         
+       2024  2 13  60353       0.0424      0.2619      0.05817         
+       2024  2 14  60354       0.0412      0.2635      0.05752         
+       2024  2 15  60355       0.0401      0.2652      0.05710         
+       2024  2 16  60356       0.0390      0.2670      0.05699         
+       2024  2 17  60357       0.0379      0.2687      0.05717         
+       2024  2 18  60358       0.0368      0.2704      0.05762         
+       2024  2 19  60359       0.0358      0.2722      0.05814         
+       2024  2 20  60360       0.0348      0.2740      0.05873         
+       2024  2 21  60361       0.0339      0.2758      0.05928         
+       2024  2 22  60362       0.0329      0.2776      0.05966         
+       2024  2 23  60363       0.0321      0.2794      0.05990         
+       2024  2 24  60364       0.0312      0.2812      0.05999         
+       2024  2 25  60365       0.0304      0.2831      0.05991         
+       2024  2 26  60366       0.0296      0.2849      0.05968         
+       2024  2 27  60367       0.0289      0.2868      0.05935         
+       2024  2 28  60368       0.0282      0.2887      0.05893         
+       2024  2 29  60369       0.0275      0.2906      0.05850         
+       2024  3  1  60370       0.0269      0.2925      0.05812         
+       2024  3  2  60371       0.0263      0.2944      0.05786         
+       2024  3  3  60372       0.0257      0.2963      0.05775         
+       2024  3  4  60373       0.0252      0.2982      0.05779         
+       2024  3  5  60374       0.0247      0.3002      0.05790         
+       2024  3  6  60375       0.0242      0.3021      0.05796         
+       2024  3  7  60376       0.0238      0.3041      0.05786         
+       2024  3  8  60377       0.0234      0.3060      0.05742         
+       2024  3  9  60378       0.0231      0.3080      0.05660         
+       2024  3 10  60379       0.0228      0.3099      0.05537         
+       2024  3 11  60380       0.0225      0.3119      0.05389         
+       2024  3 12  60381       0.0223      0.3139      0.05242         
+       2024  3 13  60382       0.0221      0.3158      0.05119         
+       2024  3 14  60383       0.0219      0.3178      0.05032         
+       2024  3 15  60384       0.0218      0.3198      0.04980         
+       2024  3 16  60385       0.0217      0.3218      0.04959         
+       2024  3 17  60386       0.0216      0.3237      0.04957         
+       2024  3 18  60387       0.0216      0.3257      0.04970         
+       2024  3 19  60388       0.0216      0.3277      0.04987         
+       2024  3 20  60389       0.0217      0.3297      0.04999         
+       2024  3 21  60390       0.0218      0.3316      0.04996         
+       2024  3 22  60391       0.0219      0.3336      0.04974         
+       2024  3 23  60392       0.0221      0.3356      0.04938         
+       2024  3 24  60393       0.0222      0.3376      0.04887         
+       2024  3 25  60394       0.0225      0.3395      0.04827         
+       2024  3 26  60395       0.0228      0.3415      0.04778         
+       2024  3 27  60396       0.0231      0.3434      0.04747         
+       2024  3 28  60397       0.0234      0.3454      0.04735         
+       2024  3 29  60398       0.0238      0.3473      0.04746         
+       2024  3 30  60399       0.0242      0.3493      0.04779         
+       2024  3 31  60400       0.0246      0.3512      0.04831         
+       2024  4  1  60401       0.0251      0.3531      0.04894         
+       2024  4  2  60402       0.0256      0.3550      0.04961         
+       2024  4  3  60403       0.0262      0.3569      0.05017         
+       2024  4  4  60404       0.0267      0.3588      0.05046         
+       2024  4  5  60405       0.0274      0.3607      0.05035         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      59990  -109.92    0.73   -6.45    0.14   
-                      59991  -110.34    0.73   -6.52    0.14   
-                      59992  -110.70    0.73   -6.82    0.14   
-                      59993  -110.62    0.50   -7.14    0.11   
-                      59994  -110.08    0.70   -7.19    0.18   
-                      59995  -109.46    0.70   -6.99    0.18   
-                      59996  -109.10    0.78   -6.82    0.21   
+                      60020  -108.26    0.97   -8.18    0.07   
+                      60021  -108.08    0.32   -8.33    0.16   
+                      60022  -107.89    0.61   -8.30    0.09   
+                      60023  -107.76    0.61   -8.12    0.09   
+                      60024  -107.74    0.61   -7.97    0.09   
+                                                                               
+                     IERS Celestial Pole Offset Final Series                   
+                           MJD          dpsi      deps                         
+                                        (msec. of arc)                         
+                          59977      -110.2      -6.3                      
+                          59978      -110.0      -6.4                      
+                          59979      -109.9      -6.5                      
+                          59980      -109.9      -6.5                      
+                          59981      -109.9      -6.3                      
+                          59982      -109.7      -6.1                      
+                          59983      -109.4      -6.0                      
+                          59984      -109.1      -5.9                      
+                          59985      -109.0      -5.9                      
+                          59986      -109.0      -5.9                      
+                          59987      -109.3      -6.1                      
+                          59988      -109.5      -6.4                      
+                          59989      -109.6      -6.5                      
+                          59990      -110.0      -6.5                      
+                          59991      -110.6      -6.6                      
+                          59992      -111.1      -6.8                      
+                          59993      -110.9      -7.1                      
+                          59994      -110.3      -7.2                      
+                          59995      -109.5      -7.0                      
+                          59996      -109.0      -6.9                      
+                          59997      -108.9      -6.8                      
+                          59998      -109.1      -6.8                      
+                          59999      -109.4      -6.7                      
+                          60000      -109.8      -6.7                      
+                          60001      -110.0      -6.9                      
+                          60002      -110.0      -7.2                      
+                          60003      -109.9      -7.5                      
+                          60004      -109.7      -7.4                      
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      59990    0.299  0.291   -0.126   0.142          
-                      59991    0.292  0.291   -0.134   0.142          
-                      59992    0.287  0.291   -0.143   0.142          
-                      59993    0.284  0.199   -0.154   0.107          
-                      59994    0.284  0.279   -0.167   0.183          
-                      59995    0.285  0.279   -0.182   0.183          
-                      59996    0.288  0.309   -0.197   0.213          
+                      60020    0.320  0.388   -0.076   0.067          
+                      60021    0.306  0.128   -0.079   0.160          
+                      60022    0.292  0.243   -0.083   0.090          
+                      60023    0.276  0.243   -0.086   0.090          
+                      60024    0.260  0.243   -0.090   0.090          
+                                                                               
+                                                                               
+                 IAU2000A Celestial Pole Offset Final Series 
+                             MJD     dX         dY           
+                             (msec. of arc)          
+                           59977     0.41      -0.16
+                           59978     0.37      -0.17
+                           59979     0.34      -0.16
+                           59980     0.31      -0.15
+                           59981     0.28      -0.13
+                           59982     0.25      -0.12
+                           59983     0.27      -0.09
+                           59984     0.30      -0.06
+                           59985     0.33      -0.02
+                           59986     0.34      -0.04
+                           59987     0.34      -0.08
+                           59988     0.33      -0.11
+                           59989     0.33      -0.15
+                           59990     0.27      -0.14
+                           59991     0.20      -0.12
+                           59992     0.13      -0.10
+                           59993     0.15      -0.12
+                           59994     0.21      -0.15
+                           59995     0.26      -0.18
+                           59996     0.31      -0.21
+                           59997     0.32      -0.17
+                           59998     0.32      -0.12
+                           59999     0.31      -0.07
+                           60000     0.32      -0.05
+                           60001     0.32      -0.04
+                           60002     0.33      -0.02
+                           60003     0.33      -0.00
+                           60004     0.33       0.06
```

### Comparing `pyTMD-2.0.2/pyTMD/eop.py` & `pyTMD-2.0.3/pyTMD/eop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!/usr/bin/env python
 u"""
 eop.py
-Written by Tyler Sutterley (11/2022)
+Written by Tyler Sutterley (03/2023)
 Utilities for maintaining and calculating Earth Orientation Parameters (EOP)
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 03/2023: add secular pole model from IERS 2018 conventions
     Updated 11/2022: added encoding for writing ascii files
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
     Written 11/2020
 """
+from __future__ import annotations
+
 import os
 import logging
 import numpy as np
 import pyTMD.utilities
 
 # PURPOSE: connects to servers and downloads mean pole files
-def update_mean_pole(verbose=False, mode=0o775):
+def update_mean_pole(verbose: bool = False, mode: oct = 0o775):
     """
     Connects to servers to download mean-pole.tab files from HPIERS servers
 
     - ftp://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.readme
 
     Servers and Mirrors
 
@@ -69,15 +72,15 @@
     else:
         return
 
     # raise exception
     raise RuntimeError(f'Unable to download {FILE}')
 
 # PURPOSE: read table of IERS pole coordinates and calculate Gaussian average
-def calculate_mean_pole(verbose=False, mode=0o775):
+def calculate_mean_pole(verbose: bool = False, mode: oct = 0o775):
     """
     Calculates the mean pole coordinates x and y are obtained by a
     Gaussian-weighted average of the IERS pole coordinates
 
     - ftp://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.readme
 
     Servers and Mirrors
@@ -125,15 +128,15 @@
         print('{0:6.2f} {1:11.7f} {2:11.7f}'.format(T,xm[i],ym[i]),file=fid)
     # close the output file
     fid.close()
     # change the permissions mode of the output mean pole file
     os.chmod(LOCAL, mode)
 
 # PURPOSE: connects to servers and downloads IERS pole coordinates files
-def pull_pole_coordinates(FILE, verbose=False):
+def pull_pole_coordinates(FILE: str, verbose: bool = False):
     """
     Connects to servers and downloads IERS pole coordinate files
 
     Servers and Mirrors
 
     - ftp://ftp.iers.org/products/eop/long-term/c01/eopc01.iau2000.1900-now.dat
     - ftp://hpiers.obspm.fr/iers/eop/eopc01/eopc01.iau2000.1900-now.dat
@@ -178,15 +181,21 @@
     else:
         return buffer
 
     # raise exception
     raise RuntimeError(f'Unable to download {FILE}')
 
 # PURPOSE: connects to servers and downloads finals files
-def update_finals_file(username=None, password=None, verbose=False, mode=0o775):
+def update_finals_file(
+        username: str or None = None,
+        password: str or None = None,
+        timeout: int or None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to servers and downloads finals EOP files
 
     Servers and Mirrors
 
     - http://maia.usno.navy.mil/ser7/
     - https://cddis.nasa.gov/archive/products/iers/
@@ -195,129 +204,160 @@
 
     Parameters
     ----------
     username: str or NoneType, default None
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
+    timeout: int or NoneType, default 20
+        timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
     # local version of file
     LOCAL = pyTMD.utilities.get_data_path(['data','finals.all'])
     HASH = pyTMD.utilities.get_hash(LOCAL)
 
     # try downloading from US Naval Oceanography Portal
     HOST = ['http://maia.usno.navy.mil','ser7','finals.all']
     try:
-        pyTMD.utilities.from_http(HOST, timeout=5, local=LOCAL,
-            hash=HASH, verbose=verbose, mode=mode)
+        pyTMD.utilities.from_http(HOST,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode
+        )
     except Exception as exc:
         pass
     else:
         return
 
     # try downloading from NASA Crustal Dynamics Data Information System
     # note: anonymous ftp access will be discontinued on 2020-10-31
     # will require using the following https Earthdata server after that date
     server = []
     server.append(['cddis.nasa.gov','pub','products','iers','finals.all'])
     server.append(['cddis.gsfc.nasa.gov','products','iers','finals.all'])
     for HOST in server:
         try:
-            pyTMD.utilities.from_ftp(HOST, timeout=20, local=LOCAL,
-                hash=HASH, verbose=verbose, mode=mode)
+            pyTMD.utilities.from_ftp(HOST,
+                timeout=timeout,
+                local=LOCAL,
+                hash=HASH,
+                verbose=verbose,
+                mode=mode)
         except Exception as exc:
             pass
         else:
             return
 
     # try downloading from NASA Crustal Dynamics Data Information System
     # using NASA Earthdata credentials stored in netrc file
     HOST = ['https://cddis.nasa.gov','archive','products','iers','finals.all']
     try:
-        pyTMD.utilities.from_cddis(HOST, username=username, password=password,
-            timeout=20, local=LOCAL, hash=HASH, verbose=verbose, mode=mode)
+        pyTMD.utilities.from_cddis(HOST,
+            username=username,
+            password=password,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode
+        )
     except Exception as exc:
         pass
     else:
         return
 
+# IERS mean or secular pole conventions
+_conventions = ('2003','2010','2015','2018')
 # read table of mean pole values, calculate angular coordinates at epoch
-def iers_mean_pole(input_file, input_epoch, version, **kwargs):
+def iers_mean_pole(
+        input_file: str,
+        input_epoch: np.ndarray,
+        convention: str,
+        **kwargs
+    ):
     """
     Calculates the angular coordinates of the IERS Conventional Mean Pole (CMP)
+    or IERS Secular Pole (2018 convention)
 
     Parameters
     ----------
     input_file: str
         Full path to mean-pole.tab file provided by IERS
-    input_epoch: float
+    input_epoch: np.ndarray
         Dates for the angular coordinates of the Conventional Mean Pole
         in decimal years
-    version: str
-        Year of the conventional model
+    convention: str
+        IERS Mean or Secular Pole Convention
+
+            - ``'2003'``
+            - ``'2010'``
+            - ``'2015'``
+            - ``'2018'``
     fill_value: float, default np.nan
         Value for invalid flags
 
     Returns
     -------
-    x: float
-        Angular coordinate x of conventional mean pole
-    y: float
-        Angular coordinate y of conventional mean pole
-    flag: bool
+    x: np.ndarray
+        Angular coordinate x of conventional mean pole or secular pole
+    y: np.ndarray
+        Angular coordinate y of conventional mean pole or secular pole
+    flag: np.ndarray
         epoch is valid for version and version number is valid
 
     References
     ----------
     .. [1] G. Petit and B. Luzum (eds.), *IERS Conventions (2010)*,
         International Earth Rotation and Reference Systems Service (IERS),
         `IERS Technical Note No. 36 <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
     """
     # set default keyword arguments
     kwargs.setdefault('fill_value', np.nan)
     # verify IERS model version
-    assert version in ('2003','2010','2015'), "Incorrect IERS model version"
+    assert convention in _conventions, "Incorrect IERS model convention"
     # read mean pole file
     table = np.loadtxt(os.path.expanduser(input_file))
     # reduce to 1971 to end date
     ii, = np.nonzero(table[:,0] >= 1971)
     table = np.copy(table[ii,:])
     # reduce to yearly values
     jj, = np.nonzero((table[:,0] % 1) == 0.0)
     table = np.copy(table[jj,:])
     end_time = table[-1,0] + 0.2
     # final shape of the table
-    nrows, ncols = np.shape(table)
+    nrows, *_ = np.shape(table)
     # allocate for output arrays
     x = np.full_like(input_epoch, kwargs['fill_value'])
     y = np.full_like(input_epoch, kwargs['fill_value'])
     flag = np.zeros_like(input_epoch, dtype=bool)
-    for t,epoch in enumerate(input_epoch):
+    for t, epoch in enumerate(input_epoch):
         # Conventional mean pole model in IERS Conventions 2003
-        if (version == '2003') and (epoch >= 1975) and (epoch < 2004):
-            x[t] = 0.054 + 0.00083*(epoch-2000.0)
-            y[t] = 0.357 + 0.00395*(epoch-2000.0)
+        if (convention == '2003') and (epoch >= 1975) and (epoch < end_time):
+            x[t] = 0.054 + 0.00083*(epoch - 2000.0)
+            y[t] = 0.357 + 0.00395*(epoch - 2000.0)
             flag[t] = True
         # Conventional mean pole model in IERS Conventions 2010
-        elif (version == '2010') and (epoch >= 1975) and (epoch < 2011):
-            dx = epoch-2000.0
+        elif (convention == '2010') and (epoch >= 1975) and (epoch < end_time):
+            dx = epoch - 2000.0
             if (dx < 10.0):
                 x[t] = 0.055974 + 1.8243e-3*dx + 1.8413e-4*dx**2 + 7.024e-6*dx**3
-                y[t] = 0.346346 + 1.7896e-3*dx + 1.0729e-4*dx**2 + 0.908e-6*dx**3
+                y[t] = 0.346346 + 1.7896e-3*dx - 1.0729e-4*dx**2 - 0.908e-6*dx**3
             else:
                 x[t] = 0.023513 + 0.0076141*dx
                 y[t] = 0.358891 - 0.0006287*dx
             flag[t] = True
         # Conventional mean pole model in IERS Conventions 2015
         # must be below maximum valid date within file (e.g. 2015.2 for 2015)
-        elif (version == '2015') and (epoch >= 1975) and (epoch < end_time):
+        elif (convention == '2015') and (epoch >= 1975) and (epoch < end_time):
             # find epoch within mean pole table
             i = 1
             j = nrows+1
             while (j > (i+1)):
                 k = (i+j)//2
                 if (epoch < table[k,0]):
                     j = k
@@ -328,34 +368,40 @@
             if (i == (nrows-1)):
                 x[t] = table[i,1] + dx*(table[nrows-1,1]-table[nrows-2,1])
                 y[t] = table[i,2] + dx*(table[nrows-1,1]-table[nrows-2,2])
             else:
                 x[t] = table[i,1] + dx*(table[i+1,1]-table[i,1])
                 y[t] = table[i,2] + dx*(table[i+1,2]-table[i,2])
             flag[t] = True
-    # return mean pole values
+        # Secular pole model in IERS Conventions 2018
+        elif (convention == '2018'):
+            # calculate secular pole
+            x[t] = 0.055 + 0.001677*(epoch - 2000.0)
+            y[t] = 0.3205 + 0.00346*(epoch - 2000.0)
+            flag[t] = True
+    # return mean/secular pole values
     return (x, y, flag)
 
 # PURPOSE: read daily earth orientation parameters (EOP) file from IERS
-def iers_daily_EOP(input_file):
+def iers_daily_EOP(input_file: str):
     """
     Read daily earth orientation parameters (EOP) file from IERS
 
     Parameters
     ----------
     input_file: str
         full path to IERS EOP "finals" file
 
     Returns
     -------
-    MJD: float
+    MJD: np.ndarray
         modified Julian date of EOP measurements
-    x: float
+    x: np.ndarray
         Angular coordinate x [arcsec]
-    y: float
+    y: np.ndarray
         Angular coordinate y [arcsec]
 
     References
     ----------
     .. [1] G. Petit and B. Luzum (eds.), *IERS Conventions (2010)*,
         International Earth Rotation and Reference Systems Service (IERS),
         `IERS Technical Note No. 36 <https://iers-conventions.obspm.fr/content/tn36.pdf>`_
```

### Comparing `pyTMD-2.0.2/pyTMD/interpolate.py` & `pyTMD-2.0.3/pyTMD/interpolate.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,46 +10,54 @@
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     scipy: Scientific Tools for Python
         https://docs.scipy.org/doc/
 
 UPDATE HISTORY:
     Written 12/2022
 """
+from __future__ import annotations
+
 import numpy as np
 import scipy.spatial
 import scipy.interpolate
 import pyTMD.spatial
 
 # PURPOSE: bilinear interpolation of input data to output data
-def bilinear(ilon, ilat, idata, lon, lat,
-             fill_value=np.nan,
-             dtype=np.float64):
+def bilinear(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        idata: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        fill_value: float = np.nan,
+        dtype: str | np.dtype = np.float64
+    ):
     """
     Bilinear interpolation of input data to output coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude of tidal model
-    ilat: float
+    ilat: np.ndarray
         latitude of tidal model
-    idata: float
+    idata: np.ndarray
         tide model data
-    lat: float
+    lat: np.ndarray
         output latitude
-    lon: float
+    lon: np.ndarray
         output longitude
     fill_value: float, default np.nan
         invalid value
-    dtype: obj, default np.float64
+    dtype: np.dtype, default np.float64
         output data type
 
     Returns
     -------
-    data: float
+    data: np.ndarray
         interpolated data
     """
     # verify that input data is masked array
     if not isinstance(idata, np.ma.MaskedArray):
         idata = np.ma.array(idata)
         idata.mask = np.zeros_like(idata, dtype=bool)
     # find valid points (within bounds)
@@ -95,53 +103,60 @@
             ii, = np.nonzero(np.isfinite(IM) & (~IM.mask))
             # calculate interpolated value for i
             data.data[i] = np.sum(WM[ii]*IM[ii])/np.sum(WM[ii])
             data.mask[i] = np.all(IM.mask[ii])
     # return interpolated values
     return data
 
-def spline(ilon, ilat, idata, lon, lat,
-           fill_value=None,
-           dtype=np.float64,
-           reducer=np.ceil,
-           **kwargs):
+
+def spline(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        idata: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        fill_value: float = None,
+        dtype: str | np.dtype = np.float64,
+        reducer=np.ceil,
+        **kwargs
+    ):
     """
     `Bivariate spline interpolation
     <https://docs.scipy.org/doc/scipy/reference/generated/
     scipy.interpolate.RectBivariateSpline.html>`_
     of input data to output coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude of tidal model
-    ilat: float
+    ilat: np.ndarray
         latitude of tidal model
-    idata: float
+    idata: np.ndarray
         tide model data
-    lat: float
+    lat: np.ndarray
         output latitude
-    lon: float
+    lon: np.ndarray
         output longitude
     fill_value: float or NoneType, default None
         invalid value
-    dtype: obj, default np.float64
+    dtype: np.dtype, default np.float64
         output data type
     reducer: obj, default np.ceil
         operation for converting mask to boolean
     kx: int, default 1
         degree of the bivariate spline in the x-dimension
     ky: int, default 1
         degree of the bivariate spline in the y-dimension
     kwargs: dict
         additional arguments for ``scipy.interpolate.RectBivariateSpline``
 
     Returns
     -------
-    data: float
+    data: np.ndarray
         interpolated data
     """
     # set default keyword arguments
     kwargs.setdefault('kx', 1)
     kwargs.setdefault('ky', 1)
     # verify that input data is masked array
     if not isinstance(idata, np.ma.MaskedArray):
@@ -171,40 +186,46 @@
             idata.mask.T, **kwargs)
         # evaluate the spline at input coordinates
         data.data[:] = s1.ev(lon, lat).astype(dtype)
         data.mask[:] = reducer(s2.ev(lon, lat)).astype(bool)
     # return interpolated values
     return data
 
-def regulargrid(ilon, ilat, idata, lon, lat,
-                fill_value=None,
-                dtype=np.float64,
-                reducer=np.ceil,
-                **kwargs):
+def regulargrid(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        idata: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        fill_value: float = None,
+        dtype: str | np.dtype = np.float64,
+        reducer=np.ceil,
+        **kwargs
+    ):
     """
     `Regular grid interpolation
     <https://docs.scipy.org/doc/scipy/reference/generated/
     scipy.interpolate.RegularGridInterpolator.html>`_
     of input data to output coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude of tidal model
-    ilat: float
+    ilat: np.ndarray
         latitude of tidal model
-    idata: float
+    idata: np.ndarray
         tide model data
-    lat: float
+    lat: np.ndarray
         output latitude
-    lon: float
+    lon: np.ndarray
         output longitude
     fill_value: float or NoneType, default None
         invalid value
-    dtype: obj, default np.float64
+    dtype: np.dtype, default np.float64
         output data type
     reducer: obj, default np.ceil
         operation for converting mask to boolean
     bounds_error: bool, default False
         raise Exception when values are requested outside domain
     method: str, default 'linear'
         Method of interpolation
@@ -215,15 +236,15 @@
             - ``'cubic'``
             - ``'quintic'``
     kwargs: dict
         additional arguments for ``scipy.interpolate.RegularGridInterpolator``
 
     Returns
     -------
-    data: float
+    data: np.ndarray
         interpolated data
     """
     # set default keyword arguments
     kwargs.setdefault('bounds_error', False)
     kwargs.setdefault('method', 'linear')
     # verify that input data is masked array
     if not isinstance(idata, np.ma.MaskedArray):
@@ -242,50 +263,57 @@
     # evaluate the interpolator at input coordinates
     data.data[:] = r1.__call__(np.c_[lat, lon])
     data.mask[:] = reducer(r2.__call__(np.c_[lat, lon])).astype(bool)
     # return interpolated values
     return data
 
 # PURPOSE: Nearest-neighbor extrapolation of valid data to output data
-def extrapolate(ilon, ilat, idata, lon, lat,
-                fill_value=np.nan,
-                dtype=np.float64,
-                cutoff=np.inf,
-                EPSG='4326'):
+def extrapolate(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        idata: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        fill_value: float = None,
+        dtype: str | np.dtype = np.float64,
+        cutoff: int | float = np.inf,
+        EPSG: str or int = '4326',
+        **kwargs
+    ):
     """
     Nearest-neighbor (`NN`) extrapolation of valid model data using `kd-trees
     <https://docs.scipy.org/doc/scipy/reference/generated/
     scipy.spatial.cKDTree.html>`_
 
     Parameters
     ----------
-    x: float
+    x: np.ndarray
         x-coordinates of tidal model
-    y: float
+    y: np.ndarray
         y-coordinates of tidal model
-    data: float
+    data: np.ndarray
         Tide model data
-    XI: float
+    XI: np.ndarray
         Output x-coordinates
-    YI: float
+    YI: np.ndarray
         Output y-coordinates
     fill_value: float, default np.nan
         Invalid value
-    dtype: obj, default np.float64
+    dtype: np.dtype, default np.float64
         Output data type
     cutoff: float, default np.inf
         return only neighbors within distance [km]
 
         Set to ``np.inf`` to extrapolate for all points
     EPSG: str, default '4326'
         projection of tide model data
 
     Returns
     -------
-    DATA: float
+    DATA: np.ndarray
         interpolated data
     """
     # verify output dimensions
     lon = np.atleast_1d(lon)
     lat = np.atleast_1d(lat)
     # extrapolate valid data values to data
     npts = len(lon)
@@ -376,28 +404,28 @@
         ind, = np.nonzero(np.isfinite(dd))
         data.data[ind] = flattened[ii[ind]]
         data.mask[ind] = False
     # return extrapolated values
     return data
 
 # PURPOSE: calculate Euclidean distances between points
-def _distance(c1, c2):
+def _distance(c1: np.ndarray, c2: np.ndarray):
     """
     Calculate Euclidean distances between points
 
     Parameters
     ----------
-    c1: float
+    c1: np.ndarray
         first set of coordinates
-    c2: float
+    c2: np.ndarray
         second set of coordinates
 
     Returns
     -------
-    c: float
+    c: np.ndarray
         Euclidean distance
     """
     # decompose Euclidean distance: (x-y)^2 = x^2 - 2xy + y^2
     dx2 = np.sum(c1**2)
     dxy = np.dot(c1[np.newaxis,:], c2.T)
     dy2 = np.sum(c2**2, axis=1)
     # calculate Euclidean distance
```

### Comparing `pyTMD-2.0.2/pyTMD/io/ATLAS.py` & `pyTMD-2.0.3/pyTMD/io/ATLAS.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 ATLAS.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 netCDF4 files can be been compressed using gzip
 
 Reads netCDF4 ATLAS tidal solutions provided by Ohio State University and ESR
@@ -51,14 +51,15 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output ATLAS formatted netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 07/2022: fix setting of masked array data to NaN
@@ -83,14 +84,16 @@
         reduce number of interpolations by copying bathymetry mask to variables
     Updated 08/2020: replaced griddata with scipy regular grid interpolators
     Updated 07/2020: added function docstrings. separate bilinear interpolation
         changed TYPE variable to keyword argument. update griddata interpolation
     Updated 06/2020: use argmin and argmax in bilinear interpolation
     Written 09/2019
 """
+from __future__ import division, annotations
+
 import os
 import copy
 import gzip
 import uuid
 import logging
 import datetime
 import warnings
@@ -105,30 +108,32 @@
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
-def extract_constants(ilon, ilat,
-    grid_file=None,
-    model_files=None,
-    **kwargs):
+def extract_constants(
+        ilon: np.ndarray, ilat: np.ndarray,
+        grid_file: str | None = None,
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for ATLAS netCDF4 tidal models
 
     Makes initial calculations to run the tide program
 
     Spatially interpolates tidal constituents to input coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     grid_file: str or NoneType, default None
         grid file for model
     model_files: list or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
@@ -153,19 +158,19 @@
     compressed: bool, default False
         Input files are gzip compressed
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
-    D: float
+    D: np.ndarray
         bathymetry of tide model
     constituents: list
         Tide model constituent names
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('method', 'spline')
@@ -181,15 +186,15 @@
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
     # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    if isinstance(model_files, str):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # check that grid file is accessible
     if not os.access(os.path.expanduser(grid_file), os.F_OK):
         raise FileNotFoundError(os.path.expanduser(grid_file))
 
@@ -338,15 +343,19 @@
     # convert phase to degrees
     phase = ph*180.0/np.pi
     phase[phase < 0] += 360.0
     # return the interpolated values
     return (amplitude, phase, D, constituents)
 
 # PURPOSE: read harmonic constants from tide models
-def read_constants(grid_file=None, model_files=None, **kwargs):
+def read_constants(
+        grid_file: str | None = None,
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for ATLAS netCDF4 tidal models
 
     Parameters
     ----------
     grid_file: str or NoneType, default None
         grid file for model
@@ -369,15 +378,15 @@
         complex form of tide model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('compressed', True)
 
     # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    if isinstance(model_files, str):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # check that grid file is accessible
     if not os.access(os.path.expanduser(grid_file), os.F_OK):
         raise FileNotFoundError(os.path.expanduser(grid_file))
 
@@ -417,25 +426,30 @@
         # append extended constituent
         constituents.append(cons,  hc)
 
     # return the complex form of the model constituents
     return constituents
 
 # PURPOSE: interpolate constants from tide models to input coordinates
-def interpolate_constants(ilon, ilat, constituents, **kwargs):
+def interpolate_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        constituents,
+        **kwargs
+    ):
     """
     Interpolate constants from ATLAS tidal models to input coordinates
 
     Makes initial calculations to run the tide program
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     constituents: obj
         Tide model constituents (complex form)
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
@@ -456,19 +470,19 @@
 
         Set to ``np.inf`` to extrapolate for all points
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
-    D: float
+    D: np.ndarray
         bathymetry of tide model
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
     kwargs.setdefault('cutoff', 10.0)
@@ -601,62 +615,66 @@
     # convert phase to degrees
     phase = ph*180.0/np.pi
     phase[phase < 0] += 360.0
     # return the interpolated values
     return (amplitude, phase, D)
 
 # PURPOSE: Extend a longitude array
-def extend_array(input_array, step_size):
+def extend_array(input_array: np.ndarray, step_size: float):
     """
     Extends a longitude array
 
     Parameters
     ----------
-    input_array: float
+    input_array: np.ndarray
         array to extend
     step_size: float
         step size between elements of array
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended array
     """
     n = len(input_array)
     temp = np.zeros((n+2), dtype=input_array.dtype)
     # extended array [x-1,x0,...,xN,xN+1]
     temp[0] = input_array[0] - step_size
     temp[1:-1] = input_array[:]
     temp[-1] = input_array[-1] + step_size
     return temp
 
 # PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix):
+def extend_matrix(input_matrix: np.ndarray):
     """
     Extends a global matrix
 
     Parameters
     ----------
-    input_matrix: float
+    input_matrix: np.ndarray
         matrix to extend
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended matrix
     """
     ny, nx = np.shape(input_matrix)
     temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read grid file
-def read_netcdf_grid(input_file, variable, **kwargs):
+def read_netcdf_grid(
+        input_file: str,
+        variable: str,
+        **kwargs
+    ):
     """
     Read grid file to extract model coordinates and bathymetry
 
     Parameters
     ----------
     input_file: str
         input grid file
@@ -670,19 +688,19 @@
             - ``'V'``: vertical depth-averaged transport
 
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    lon: float
+    lon: np.ndarray
         longitudinal coordinates of input grid
-    lat: float
+    lat: np.ndarray
         latitudinal coordinates of input grid
-    bathymetry: float
+    bathymetry: np.ndarray
         model bathymetry
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide grid file
     # reading a combined global solution with localized solutions
     if kwargs['compressed']:
@@ -720,28 +738,31 @@
     # close the grid file
     fileID.close()
     f.close() if kwargs['compressed'] else None
     return (lon, lat, bathymetry)
 
 # PURPOSE: read elevation file to extract real and imaginary components for
 # constituent
-def read_netcdf_elevation(input_file, **kwargs):
+def read_netcdf_elevation(
+        input_file: str,
+        **kwargs
+    ):
     """
     Read elevation file to extract real and imaginary components for constituent
 
     Parameters
     ----------
     input_file: str
         input elevation file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    h: float
+    h: np.ndarray
         tidal elevation
     con: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide elevation file
@@ -766,15 +787,19 @@
     fileID.close()
     f.close() if kwargs['compressed'] else None
     # return the elevation and constituent
     return (h, con.strip())
 
 # PURPOSE: read transport file to extract real and imaginary components for
 # constituent
-def read_netcdf_transport(input_file, variable, **kwargs):
+def read_netcdf_transport(
+        input_file: str,
+        variable: str,
+        **kwargs
+    ):
     """
     Read transport file to extract real and imaginary components for constituent
 
     Parameters
     ----------
     input_file: str
         input transport file
@@ -787,15 +812,15 @@
             - ``'V'``: vertical depth-averaged transport
 
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    tr: float
+    tr: np.ndarray
         tidal transport
     con: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide transport file
@@ -823,41 +848,50 @@
     # close the file
     fileID.close()
     f.close() if kwargs['compressed'] else None
     # return the transport components and constituent
     return (tr, con.strip())
 
 # PURPOSE: output grid file in ATLAS netCDF format
-def output_netcdf_grid(FILE, hz, hu, hv,
-                       lon_z, lat_z, lon_u,
-                       lat_u, lon_v, lat_v):
+def output_netcdf_grid(
+        FILE: str,
+        hz: np.ndarray,
+        hu: np.ndarray,
+        hv: np.ndarray,
+        lon_z: np.ndarray,
+        lat_z: np.ndarray,
+        lon_u: np.ndarray,
+        lat_u: np.ndarray,
+        lon_v: np.ndarray,
+        lat_v: np.ndarray
+    ):
     """
     Writes grid files in ATLAS netCDF format
 
     Parameters
     ----------
     FILE: str
         output ATLAS grid file name
-    hz: float
+    hz: np.ndarray
         model bathymetry at z-nodes
-    hu: float
+    hu: np.ndarray
         model bathymetry at u-nodes
-    hv: float
+    hv: np.ndarray
         model bathymetry at v-nodes
-    lon_z: float
+    lon_z: np.ndarray
         longitude coordinates at z-nodes
-    lat_z: float
+    lat_z: np.ndarray
         latitude coordinates at z-nodes
-    lon_u: float
+    lon_u: np.ndarray
         longitude coordinates at u-nodes
-    lat_u: float
+    lat_u: np.ndarray
         latitude coordinates at u-nodes
-    lon_v: float
+    lon_v: np.ndarray
         longitude coordinates at v-nodes
-    lat_v: float
+    lat_v: np.ndarray
         latitude coordinates at v-nodes
     """
     # opening NetCDF file for writing
     fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
     # define the NetCDF dimensions
     ny, nx = np.shape(hz)
     fileID.createDimension('nx', nx)
@@ -911,27 +945,33 @@
     # Output NetCDF structure information
     logging.info(FILE)
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
 # PURPOSE: output elevation file in ATLAS netCDF format
-def output_netcdf_elevation(FILE, h, lon_z, lat_z, constituent):
+def output_netcdf_elevation(
+        FILE: str,
+        h: np.ndarray,
+        lon_z: np.ndarray,
+        lat_z: np.ndarray,
+        constituent: str
+    ):
     """
     Writes elevation files in ATLAS netCDF format
 
     Parameters
     ----------
     FILE: str
         output ATLAS elevation file name
-    h: complex
+    h: np.ndarray
         Eulerian form of tidal elevation oscillation
-    lon_z: float
+    lon_z: np.ndarray
         longitude coordinates at z-nodes
-    lat_z: float
+    lat_z: np.ndarray
         latitude coordinates at z-nodes
     constituent: str
         tidal constituent ID
     """
     # opening NetCDF file for writing
     fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
     # define the NetCDF dimensions
@@ -952,15 +992,15 @@
     nc['lat_z'][:] = lat_z[:]
     nc['hRe'][:] = h.real[:]
     nc['hIm'][:] = h.imag[:]
     # define variable attributes
     complexpart = dict(Re='Real part', Im='Imag part')
     # set variable attributes for coordinates
     nc['lon_z'].setncattr('units', 'degrees_east')
-    nc['lon_z'].setncattr('long_name', 'longitude of Z nodes')
+    nc['lon_z'].setncattr('long_name', 'longitude of Z nofloatdes')
     nc['lat_z'].setncattr('units', 'degrees_north')
     nc['lat_z'].setncattr('long_name', 'latitude of Z nodes')
     # set variable attributes for tidal constituents
     for COMP in ('Re','Im'):
         key = f'h{COMP}'
         long_name = f'Tidal elevation complex amplitude, {complexpart[COMP]}'
         field = (f'{COMP}(h), scalar; '
@@ -987,34 +1027,42 @@
     # Output NetCDF structure information
     logging.info(FILE)
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
 # PURPOSE: output transport file in ATLAS netCDF format
-def output_netcdf_transport(FILE, u, v, lon_u, lat_u,
-                            lon_v, lat_v, constituent):
+def output_netcdf_transport(
+        FILE: str,
+        u: np.ndarray,
+        v: np.ndarray,
+        lon_u: np.ndarray,
+        lat_u: np.ndarray,
+        lon_v: np.ndarray,
+        lat_v: np.ndarray,
+        constituent: str
+    ):
     """
     Writes transport files in ATLAS netCDF format
 
     Parameters
     ----------
     FILE: str
         output ATLAS transport file name
-    u: complex
+    u: np.ndarray
         Eulerian form of tidal zonal transport oscillation
-    v: complex
+    v: np.ndarray
         Eulerian form of tidal meridional transport oscillation
-    lon_u: float
+    lon_u: np.ndarray
         longitude coordinates at u-nodes
-    lat_u: float
+    lat_u: np.ndarray
         latitude coordinates at u-nodes
-    lon_v: float
+    lon_v: np.ndarray
         longitude coordinates at v-nodes
-    lat_v: float
+    lat_v: np.ndarray
         latitude coordinates at v-nodes
     constituents: str
         tidal constituent ID
     """
     # opening NetCDF file for writing
     fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
     # define the NetCDF dimensions
```

### Comparing `pyTMD-2.0.2/pyTMD/io/FES.py` & `pyTMD-2.0.3/pyTMD/io/FES.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 FES.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (04/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from the
     FES (Finite Element Solution) tide models for given locations
 ascii and netCDF4 files can be been compressed using gzip
 
 Reads ascii and netCDF4 FES tidal solutions provided by AVISO
@@ -24,14 +24,15 @@
         v: vertical transport velocities
     version: model version to run
         FES1999
         FES2004
         FES2012
         FES2014
         EOT20
+        HAMTIDE11
     method: interpolation method
         bilinear: quick bilinear interpolation
         spline: scipy bivariate spline interpolation
         linear, nearest: scipy regular grid interpolations
     extrapolate: extrapolate model using nearest-neighbors
     cutoff: extrapolation cutoff in kilometers
         set to np.inf to extrapolate for all points
@@ -51,14 +52,16 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 04/2023: added global HAMTIDE11 model
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output FES formatted netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 05/2022: reformat arguments to extract_FES_constants definition
@@ -80,14 +83,16 @@
         replaced numpy bool to prevent deprecation warning
     Updated 12/2020: added nearest-neighbor data extrapolation
     Updated 09/2020: set bounds error to false for regular grid interpolations
         adjust dimensions of input coordinates to be iterable
     Updated 08/2020: replaced griddata with scipy regular grid interpolators
     Written 07/2020
 """
+from __future__ import division, annotations
+
 import os
 import copy
 import gzip
 import uuid
 import logging
 import datetime
 import warnings
@@ -102,27 +107,32 @@
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
-def extract_constants(ilon, ilat, model_files=None, **kwargs):
+def extract_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for a FES ascii or netCDF4 tidal model
 
     Makes initial calculations to run the tide program
 
     Spatially interpolates tidal constituents to input coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     model_files: list or NoneType, default None
         list of model files for each constituent
     type: str, default 'z'
         Tidal variable to read
 
             - ``'z'``: heights
@@ -132,14 +142,15 @@
         Model version to read
 
             - ``'FES1999'``
             - ``'FES2004'``
             - ``'FES2012'``
             - ``'FES2014'``
             - ``'EOT20'``
+            - ``'HAMTIDE11'``
     method: str, default 'spline'
         Interpolation method
 
             - ``'bilinear'``: quick bilinear interpolation
             - ``'spline'``: scipy bivariate spline interpolation
             - ``'linear'``, ``'nearest'``: scipy regular grid interpolations
     extrapolate: bool, default False
@@ -151,17 +162,17 @@
     compressed: bool, default False
         Input files are gzip compressed
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('version', None)
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
@@ -176,15 +187,15 @@
         if old in kwargs.keys():
             warnings.warn(f"""Deprecated keyword argument {old}.
                 Changed to '{new}'""", DeprecationWarning)
             # set renamed argument to not break workflows
             kwargs[new] = copy.copy(kwargs[old])
 
     # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    if isinstance(model_files, str):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
     ilat = np.atleast_1d(np.copy(ilat))
     # number of points
@@ -202,15 +213,15 @@
         # check that model file is accessible
         if not os.access(os.path.expanduser(fi), os.F_OK):
             raise FileNotFoundError(os.path.expanduser(fi))
         # read constituent from elevation file
         if kwargs['version'] in ('FES1999','FES2004'):
             # FES ascii constituent files
             hc,lon,lat = read_ascii_file(os.path.expanduser(fi), **kwargs)
-        elif kwargs['version'] in ('FES2012','FES2014','EOT20'):
+        elif kwargs['version'] in ('FES2012','FES2014','EOT20','HAMTIDE11'):
             # FES netCDF4 constituent files
             hc,lon,lat = read_netcdf_file(os.path.expanduser(fi), **kwargs)
         # adjust longitudinal convention of input latitude and longitude
         # to fit tide model convention
         if (np.min(ilon) < 0.0) & (np.max(lon) > 180.0):
             # input points convention (-180:180)
             # tide model convention (0:360)
@@ -286,15 +297,18 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
 # PURPOSE: read harmonic constants from tide models
-def read_constants(model_files=None, **kwargs):
+def read_constants(
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for a FES ascii or netCDF4 tidal model
 
     Parameters
     ----------
     model_files: list or NoneType, default None
         list of model files for each constituent
@@ -308,44 +322,45 @@
         Model version to read
 
             - ``'FES1999'``
             - ``'FES2004'``
             - ``'FES2012'``
             - ``'FES2014'``
             - ``'EOT20'``
+            - ``'HAMTIDE11'``
     compressed: bool, default False
         Input files are gzip compressed
 
     Returns
     -------
     constituents: obj
         complex form of tide model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('version', None)
     kwargs.setdefault('compressed', False)
 
     # raise warning if model files are entered as a string
-    if isinstance(model_files,str):
+    if isinstance(model_files, str):
         warnings.warn("Tide model is entered as a string")
         model_files = [model_files]
 
     # save output constituents
     constituents = pyTMD.io.constituents()
     # read each model constituent
     for i, fi in enumerate(model_files):
         # check that model file is accessible
         if not os.access(os.path.expanduser(fi), os.F_OK):
             raise FileNotFoundError(os.path.expanduser(fi))
         # read constituent from elevation file
         if kwargs['version'] in ('FES1999','FES2004'):
             # FES ascii constituent files
             hc,lon,lat = read_ascii_file(os.path.expanduser(fi), **kwargs)
-        elif kwargs['version'] in ('FES2012','FES2014','EOT20'):
+        elif kwargs['version'] in ('FES2012','FES2014','EOT20','HAMTIDE11'):
             # FES netCDF4 constituent files
             hc,lon,lat = read_netcdf_file(os.path.expanduser(fi), **kwargs)
         # grid step size of tide model
         dlon = lon[1] - lon[0]
         # replace original values with extend arrays/matrices
         if np.isclose(lon[-1] - lon[0], 360.0 - dlon):
             lon = extend_array(lon, dlon)
@@ -356,25 +371,30 @@
         setattr(constituents, 'longitude', lon)
         setattr(constituents, 'latitude', lat)
 
     # return the complex form of the model constituents
     return constituents
 
 # PURPOSE: interpolate constants from tide models to input coordinates
-def interpolate_constants(ilon, ilat, constituents, **kwargs):
+def interpolate_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        constituents,
+        **kwargs
+    ):
     """
     Interpolate constants from FES tidal models to input coordinates
 
     Makes initial calculations to run the tide program
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     constituents: obj
         Tide model constituents (complex form)
     method: str, default 'spline'
         Interpolation method
 
             - ``'bilinear'``: quick bilinear interpolation
@@ -387,17 +407,17 @@
 
         Set to ``np.inf`` to extrapolate for all points
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
     """
     # set default keyword arguments
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
     kwargs.setdefault('cutoff', 10.0)
     kwargs.setdefault('scale', 1.0)
@@ -502,77 +522,80 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
 # PURPOSE: Extend a longitude array
-def extend_array(input_array, step_size):
+def extend_array(input_array: np.ndarray, step_size: float):
     """
     Extends a longitude array
 
     Parameters
     ----------
-    input_array: float
+    input_array: np.ndarray
         array to extend
     step_size: float
         step size between elements of array
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended array
     """
     n = len(input_array)
     temp = np.zeros((n+2), dtype=input_array.dtype)
     # extended array [x-1,x0,...,xN,xN+1]
     temp[0] = input_array[0] - step_size
     temp[1:-1] = input_array[:]
     temp[-1] = input_array[-1] + step_size
     return temp
 
 # PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix):
+def extend_matrix(input_matrix: np.ndarray):
     """
     Extends a global matrix
 
     Parameters
     ----------
-    input_matrix: float
+    input_matrix: np.ndarray
         matrix to extend
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended matrix
     """
     ny, nx = np.shape(input_matrix)
     temp = np.ma.zeros((ny,nx+2), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read FES ascii tide model grid files
-def read_ascii_file(input_file, **kwargs):
+def read_ascii_file(input_file: str, **kwargs):
     """
     Read FES (Finite Element Solution) tide model file
 
     Parameters
     ----------
     input_file: str
         model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    hc: complex form of tidal constituent oscillation
-    lon: longitude of tidal model
-    lat: latitude of tidal model
+    hc: np.ndarray
+        complex form of tidal constituent oscillation
+    lon: np.ndarray
+        longitude of tidal model
+    lat: np.ndarray
+        latitude of tidal model
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # tilde-expand input file
     input_file = os.path.expanduser(input_file)
     # read input tide model file
     if kwargs['compressed']:
@@ -625,15 +648,18 @@
     mask = (amp.data == amp.fill_value) | (ph.data == ph.fill_value)
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat)
 
 # PURPOSE: read FES netCDF4 tide model files
-def read_netcdf_file(input_file, **kwargs):
+def read_netcdf_file(
+        input_file: str,
+        **kwargs
+    ):
     """
     Read FES (Finite Element Solution) tide model netCDF4 file
 
     Parameters
     ----------
     input_file: str
         model file
@@ -641,54 +667,59 @@
         Tidal variable to read
 
             - ``'z'``: heights
             - ``'u'``: horizontal transport velocities
             - ``'v'``: vertical transport velocities
     version: str or NoneType, default None
         FES model version
+
+            - ``'FES2012'``
+            - ``'FES2014'``
+            - ``'EOT20'``
+            - ``'HAMTIDE11'``
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    hc: complex
+    hc: np.ndarray
         complex form of tidal constituent oscillation
-    lon: float
+    lon: np.ndarray
         longitude of tidal model
-    lat: float
+    lat: np.ndarray
         latitude of tidal model
     """
     # set default keyword arguments
     kwargs.setdefault('type', None)
     kwargs.setdefault('version', None)
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide elevation file
     if kwargs['compressed']:
         # read gzipped netCDF4 file
         f = gzip.open(os.path.expanduser(input_file),'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
         fileID = netCDF4.Dataset(os.path.expanduser(input_file), 'r')
     # variable dimensions for each model
+    # amplitude and phase components for each type
     if kwargs['version'] in ('FES2012',):
         lon = fileID.variables['longitude'][:]
         lat = fileID.variables['latitude'][:]
+        amp_key = dict(z='amplitude', u='Ua', v='Va')[kwargs['type']]
+        phase_key = dict(z='phase', u='Ug', v='Vg')[kwargs['type']]
     elif kwargs['version'] in ('FES2014','EOT20'):
         lon = fileID.variables['lon'][:]
         lat = fileID.variables['lat'][:]
-    # amplitude and phase components for each type
-    if (kwargs['type'] == 'z'):
-        amp_key = 'amplitude'
-        phase_key = 'phase'
-    elif (kwargs['type'] == 'u'):
-        amp_key = 'Ua'
-        phase_key = 'Ug'
-    elif (kwargs['type'] == 'v'):
-        amp_key = 'Va'
-        phase_key = 'Vg'
+        amp_key = dict(z='amplitude', u='Ua', v='Va')[kwargs['type']]
+        phase_key = dict(z='phase', u='Ug', v='Vg')[kwargs['type']]
+    elif kwargs['version'] in ('HAMTIDE11',):
+        lon = fileID.variables['LON'][:]
+        lat = fileID.variables['LAT'][:]
+        amp_key = dict(z='AMPL', u='UAMP', v='VAMP')[kwargs['type']]
+        phase_key = dict(z='PHAS', u='UPHA', v='VPHA')[kwargs['type']]
     # get amplitude and phase components
     amp = fileID.variables[amp_key][:]
     ph = fileID.variables[phase_key][:]
     # close the file
     fileID.close()
     f.close() if kwargs['compressed'] else None
     # calculate complex form of constituent oscillation
@@ -697,27 +728,34 @@
         np.isnan(amp.data) | np.isnan(ph.data)
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat)
 
 # PURPOSE: output tidal constituent file in FES2014 format
-def output_netcdf_file(FILE, hc, lon, lat, constituent, **kwargs):
+def output_netcdf_file(
+        FILE: str,
+        hc: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        constituent: str,
+        **kwargs
+    ):
     """
     Writes tidal constituent files in FES2014 netCDF format
 
     Parameters
     ----------
     FILE: str
         output FES model file name
-    hc: complex
+    hc: np.ndarray
         Eulerian form of tidal constituent
-    lon: float
+    lon: np.ndarray
         longitude coordinates
-    lat: float
+    lat: np.ndarray
         latitude coordinates
     constituent: str
         tidal constituent ID
     type: str or NoneType, default None
         Tidal variable to output
 
             - ``'z'``: heights
```

### Comparing `pyTMD-2.0.2/pyTMD/io/GOT.py` & `pyTMD-2.0.3/pyTMD/io/GOT.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 GOT.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (04/2023)
 
 Reads files for Richard Ray's Global Ocean Tide (GOT) models and makes initial
     calculations to run the tide program
 Includes functions to extract tidal harmonic constants out of a tidal model for
     given locations
 
 INPUTS:
@@ -38,14 +38,16 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 04/2023: fix repeated longitudinal convention adjustment
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to read and write GOT netCDF4 files
         refactored interpolation routines into new module
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 05/2022: reformat arguments to extract_GOT_constants definition
         changed keyword arguments to camel case
@@ -72,15 +74,15 @@
     Updated 09/2019: output as numpy masked arrays instead of nan-filled arrays
     Updated 07/2019: interpolate fill value mask with bivariate splines
     Updated 12/2018: python3 compatibility updates for division and zip
     Updated 10/2018: added scale as load tides are in mm and ocean are in cm
     Updated 08/2018: added multivariate spline interpolation option
     Written 07/2018
 """
-from __future__ import division
+from __future__ import division, annotations
 
 import os
 import re
 import copy
 import gzip
 import uuid
 import logging
@@ -97,27 +99,32 @@
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
-def extract_constants(ilon, ilat, model_files=None, **kwargs):
+def extract_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for Richard Ray's Global Ocean Tide (GOT) models
 
     Makes initial calculations to run the tide program
 
     Spatially interpolates tidal constituents to input coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     model_files: list or NoneType, default None
         list of model files for each constituent
     method: str, default 'spline'
         Interpolation method
 
             - ``'bilinear'``: quick bilinear interpolation
@@ -137,19 +144,19 @@
     compressed: bool, default False
         Input files are gzip compressed
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
-    constituents: list
+    constituents: np.ndarray
         list of model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
     kwargs.setdefault('cutoff', 10.0)
     kwargs.setdefault('grid', 'ascii')
@@ -266,15 +273,18 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, constituents)
 
 # PURPOSE: read harmonic constants from tide models
-def read_constants(model_files=None, **kwargs):
+def read_constants(
+        model_files: str | list | None = None,
+        **kwargs
+    ):
     """
     Reads files for Richard Ray's Global Ocean Tide (GOT) models
 
     Parameters
     ----------
     model_files: list or NoneType, default None
         list of model files for each constituent
@@ -327,25 +337,30 @@
         setattr(constituents, 'longitude', lon)
         setattr(constituents, 'latitude', lat)
 
     # return the complex form of the model constituents
     return constituents
 
 # PURPOSE: interpolate constants from tide models to input coordinates
-def interpolate_constants(ilon, ilat, constituents, **kwargs):
+def interpolate_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        constituents,
+        **kwargs
+    ):
     """
     Interpolate constants from GOT tidal models to input coordinates
 
     Makes initial calculations to run the tide program
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     constituents: obj
         Tide model constituents (complex form)
     method: str, default 'spline'
         Interpolation method
 
             - ``'bilinear'``: quick bilinear interpolation
@@ -358,17 +373,17 @@
 
         Set to ``np.inf`` to extrapolate for all points
     scale: float, default 1.0
         Scaling factor for converting to output units
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
     """
     # set default keyword arguments
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
     kwargs.setdefault('cutoff', 10.0)
     kwargs.setdefault('scale', 1.0)
@@ -393,25 +408,14 @@
         # tide model convention (-180:180)
         ilon[ilon>180.0] -= 360.0
     # number of points
     npts = len(ilon)
     # number of constituents
     nc = len(constituents)
 
-    # adjust longitudinal convention of input latitude and longitude
-    # to fit tide model convention
-    if (np.min(ilon) < 0.0) & (np.max(lon) > 180.0):
-        # input points convention (-180:180)
-        # tide model convention (0:360)
-        ilon[ilon<0.0] += 360.0
-    elif (np.max(ilon) > 180.0) & (np.min(lon) < 0.0):
-        # input points convention (0:360)
-        # tide model convention (-180:180)
-        ilon[ilon>180.0] -= 360.0
-
     # amplitude and phase
     amplitude = np.ma.zeros((npts,nc))
     amplitude.mask = np.zeros((npts,nc),dtype=bool)
     ph = np.ma.zeros((npts,nc))
     ph.mask = np.zeros((npts,nc),dtype=bool)
     # default complex fill value
     fill_value = np.ma.default_fill_value(np.dtype(complex))
@@ -479,81 +483,84 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase)
 
 # PURPOSE: Extend a longitude array
-def extend_array(input_array, step_size):
+def extend_array(input_array: np.ndarray, step_size: float):
     """
     Extends a longitude array
 
     Parameters
     ----------
-    input_array: float
+    input_array: np.ndarray
         array to extend
     step_size: float
         step size between elements of array
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended array
     """
     n = len(input_array)
     temp = np.zeros((n+3), dtype=input_array.dtype)
     # extended array [x-1,x0,...,xN,xN+1,xN+2]
     temp[0] = input_array[0] - step_size
     temp[1:-2] = input_array[:]
     temp[-2] = input_array[-1] + step_size
     temp[-1] = input_array[-1] + 2.0*step_size
     return temp
 
 # PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix):
+def extend_matrix(input_matrix: np.ndarray):
     """
     Extends a global matrix
 
     Parameters
     ----------
-    input_matrix: float
+    input_matrix: np.ndarray
         matrix to extend
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended matrix
     """
     ny, nx = np.shape(input_matrix)
     temp = np.ma.zeros((ny,nx+3), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-2] = input_matrix[:,:]
     temp[:,-2] = input_matrix[:,0]
     temp[:,-1] = input_matrix[:,1]
     return temp
 
 # PURPOSE: read GOT model grid files
-def read_ascii_file(input_file, **kwargs):
+def read_ascii_file(
+        input_file: str,
+        **kwargs
+    ):
     """
     Read Richard Ray's Global Ocean Tide (GOT) model file
 
     Parameters
     ----------
     input_file: str
         Model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    hc: complex
+    hc: np.ndarray
         complex form of tidal constituent oscillation
-    lon: float
+    lon: np.ndarray
         longitude of tidal model
-    lat: float
+    lat: np.ndarray
         latitude of tidal model
     cons: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # tilde-expand input file
@@ -606,32 +613,35 @@
     hc = amp*np.exp(-1j*ph*np.pi/180.0)
     # set masks
     hc.mask = (amp.data == amp.fill_value) | (ph.data == ph.fill_value)
     # return output variables
     return (hc, lon, lat, cons)
 
 # PURPOSE: read GOT netCDF4 tide model files
-def read_netcdf_file(input_file, **kwargs):
+def read_netcdf_file(
+        input_file: str,
+        **kwargs
+    ):
     """
     Read Richard Ray's Global Ocean Tide (GOT) netCDF4 model file
 
     Parameters
     ----------
     input_file: str
         model file
     compressed: bool, default False
         Input file is gzip compressed
 
     Returns
     -------
-    hc: complex
+    hc: np.ndarray
         complex form of tidal constituent oscillation
-    lon: float
+    lon: np.ndarray
         longitude of tidal model
-    lat: float
+    lat: np.ndarray
         latitude of tidal model
     cons: str
         tidal constituent ID
     """
     # set default keyword arguments
     kwargs.setdefault('compressed', False)
     # read the netcdf format tide elevation file
@@ -658,27 +668,33 @@
         np.isnan(amp.data) | np.isnan(ph.data)
     hc = np.ma.array(amp*np.exp(-1j*ph*np.pi/180.0), mask=mask,
         fill_value=np.ma.default_fill_value(np.dtype(complex)))
     # return output variables
     return (hc, lon, lat, cons)
 
 # PURPOSE: output tidal constituent file in GOT format
-def output_netcdf_file(FILE, hc, lon, lat, constituent):
+def output_netcdf_file(
+        FILE: str,
+        hc: np.ndarray,
+        lon: np.ndarray,
+        lat: np.ndarray,
+        constituent: str
+    ):
     """
     Writes tidal constituent files in GOT netCDF format
 
     Parameters
     ----------
     FILE: str
         output GOT model file name
-    hc: complex
+    hc: np.ndarray
         Eulerian form of tidal constituent
-    lon: float
+    lon: np.ndarray
         longitude coordinates
-    lat: float
+    lat: np.ndarray
         latitude coordinates
     constituent: str
         tidal constituent ID
     """
     # opening NetCDF file for writing
     fileID = netCDF4.Dataset(os.path.expanduser(FILE), 'w', format="NETCDF4")
     # define the NetCDF dimensions
```

### Comparing `pyTMD-2.0.2/pyTMD/io/OTIS.py` & `pyTMD-2.0.3/pyTMD/io/OTIS.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 OTIS.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from OTIS tide models for
     given locations
 
 Reads OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
@@ -51,18 +51,20 @@
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     scipy: Scientific Tools for Python
         https://docs.scipy.org/doc/
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
-    convert_ll_xy.py: converts lat/lon points to and from projected coordinates
+    convert_crs.py: converts lat/lon points to and from projected coordinates
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
+        new function name for converting coordinate reference systems
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         refactored interpolation routines into new module
     Updated 11/2022: place some imports within try/except statements
         fix variable reads for ATLAS compact data formats
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: invert current tide masks to be True for invalid points
@@ -101,51 +103,56 @@
     Updated 01/2019: decode constituents for Python3 compatibility
     Updated 08/2018: added option grid for using ATLAS outputs that
         combine both global and localized tidal solutions
         added multivariate spline interpolation option
     Updated 07/2018: added different interpolation methods
     Updated 09/2017: Adapted for Python
 """
+from __future__ import division, annotations
+
 import os
 import copy
 import struct
 import warnings
 import numpy as np
 import scipy.interpolate
 import pyTMD.interpolate
 import pyTMD.io.constituents
-from pyTMD.convert_ll_xy import convert_ll_xy
+from pyTMD.convert_crs import convert_crs
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
-def extract_constants(ilon, ilat,
-    grid_file=None,
-    model_file=None,
-    EPSG=None,
-    **kwargs):
+def extract_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        grid_file: str | None = None,
+        model_file: str | list | None = None,
+        EPSG: str | int | None = None,
+        **kwargs
+    ):
     """
     Reads files from tide models in OTIS and ATLAS-compact formats
 
     Makes initial calculations to run the tide program
 
     Spatially interpolates tidal constituents to input coordinates
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     grid_file: str or NoneType, default None
         grid file for model
     model_file: str, list or NoneType, default None
         model file containing each constituent
     EPSG: str or NoneType, default None,
         projection of tide model data
@@ -176,19 +183,19 @@
             - ``'ESR'``: combined global or local netCDF4 solution
             - ``'OTIS'``: combined global or local solution
     apply_flexure: bool, default False
         Apply ice flexure scaling factor to height constituents
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
-    D: float
+    D: np.ndarray
         bathymetry of tide model
     constituents: list
         list of model constituents
     """
     # set default keyword arguments
     kwargs.setdefault('type', 'z')
     kwargs.setdefault('method', 'spline')
@@ -224,15 +231,15 @@
     # invert tide mask to be True for invalid points
     mz = np.logical_not(mz).astype(mz.dtype)
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
     ilat = np.atleast_1d(np.copy(ilat))
     # run wrapper function to convert coordinate systems of input lat/lon
-    x,y = convert_ll_xy(ilon, ilat, EPSG, 'F')
+    x,y = convert_crs(ilon, ilat, EPSG, 'F')
     # grid step size of tide model
     dx = xi[1] - xi[0]
     dy = yi[1] - yi[0]
 
     # create current masks and bathymetry estimates
     if (kwargs['type'] != 'z'):
         mz,mu,mv = Muv(hz)
@@ -443,15 +450,20 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, D, constituents)
 
 # PURPOSE: read harmonic constants from tide models
-def read_constants(grid_file=None, model_file=None, EPSG=None, **kwargs):
+def read_constants(
+        grid_file: str | None = None,
+        model_file: str | list | None = None,
+        EPSG: str | int | None = None,
+        **kwargs
+    ):
     """
     Reads files from tide models in OTIS and ATLAS-compact formats
 
     Parameters
     ----------
     grid_file: str or NoneType, default None
         grid file for model
@@ -630,28 +642,32 @@
             # append extended constituent
             constituents.append(c, v)
 
     # return the complex form of the model constituents
     return constituents
 
 # PURPOSE: interpolate constants from tide models to input coordinates
-def interpolate_constants(ilon, ilat, constituents,
-    EPSG=None,
-    **kwargs):
+def interpolate_constants(
+        ilon: np.ndarray,
+        ilat: np.ndarray,
+        constituents,
+        EPSG: str | int | None = None,
+        **kwargs
+    ):
     """
     Interpolate constants from OTIS/ATLAS-compact tidal models to input
     coordinates
 
     Makes initial calculations to run the tide program
 
     Parameters
     ----------
-    ilon: float
+    ilon: np.ndarray
         longitude to interpolate
-    ilat: float
+    ilat: np.ndarray
         latitude to interpolate
     constituents: obj
         Tide model constituents (complex form)
     EPSG: str or NoneType, default None,
         projection of tide model data
     type: str, default 'z'
         Tidal variable to read
@@ -672,19 +688,19 @@
     cutoff: float, default 10.0
         Extrapolation cutoff in kilometers
 
         Set to ``np.inf`` to extrapolate for all points
 
     Returns
     -------
-    amplitude: float
+    amplitude: np.ndarray
         amplitudes of tidal constituents
-    phase: float
+    phase: np.ndarray
         phases of tidal constituents
-    D: float
+    D: np.ndarray
         bathymetry of tide model
     """
     # set default keyword arguments
     kwargs.setdefault('method', 'spline')
     kwargs.setdefault('extrapolate', False)
     kwargs.setdefault('cutoff', 10.0)
     # verify that constituents are valid class instance
@@ -693,15 +709,15 @@
     xi = np.copy(constituents.x)
     yi = np.copy(constituents.y)
 
     # adjust dimensions of input coordinates to be iterable
     ilon = np.atleast_1d(np.copy(ilon))
     ilat = np.atleast_1d(np.copy(ilat))
     # run wrapper function to convert coordinate systems of input lat/lon
-    x,y = convert_ll_xy(ilon, ilat, EPSG, 'F')
+    x,y = convert_crs(ilon, ilat, EPSG, 'F')
     # adjust longitudinal convention of input latitude and longitude
     # to fit tide model convention
     if (np.min(x) < np.min(xi)) & (EPSG == '4326'):
         x[x < 0] += 360.0
     if (np.max(x) > np.max(xi)) & (EPSG == '4326'):
         x[x > 180] -= 360.0
     # determine if any input points are outside of the model bounds
@@ -805,83 +821,83 @@
     # replace data for invalid mask values
     amplitude.data[amplitude.mask] = amplitude.fill_value
     phase.data[phase.mask] = phase.fill_value
     # return the interpolated values
     return (amplitude, phase, D)
 
 # PURPOSE: Extend a longitude array
-def extend_array(input_array, step_size):
+def extend_array(input_array: np.ndarray, step_size: float):
     """
     Extends a longitude array
 
     Parameters
     ----------
-    input_array: float
+    input_array: np.ndarray
         array to extend
     step_size: float
         step size between elements of array
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended array
     """
     n = len(input_array)
     temp = np.zeros((n+2), dtype=input_array.dtype)
     # extended array [x-1,x0,...,xN,xN+1]
     temp[0] = input_array[0] - step_size
     temp[1:-1] = input_array[:]
     temp[-1] = input_array[-1] + step_size
     return temp
 
 # PURPOSE: Extend a global matrix
-def extend_matrix(input_matrix):
+def extend_matrix(input_matrix: np.ndarray):
     """
     Extends a global matrix
 
     Parameters
     ----------
-    input_matrix: float
+    input_matrix: np.ndarray
         matrix to extend
 
     Returns
     -------
-    temp: float
+    temp: np.ndarray
         extended matrix
     """
     ny, nx = np.shape(input_matrix)
     temp = np.ma.zeros((ny, nx+2), dtype=input_matrix.dtype)
     temp[:,0] = input_matrix[:,-1]
     temp[:,1:-1] = input_matrix[:,:]
     temp[:,-1] = input_matrix[:,0]
     return temp
 
 # PURPOSE: read tide grid file
-def read_otis_grid(input_file):
+def read_otis_grid(input_file: str):
     """
     Read grid file to extract model coordinates, bathymetry, masks and indices
 
     Parameters
     ----------
     input_file: str
         input grid file
 
     Returns
     -------
-    x: float
+    x: np.ndarray
         x-coordinates of input grid
-    y: float
+    y: np.ndarray
         y-coordinates of input grid
-    hz: float
+    hz: np.ndarray
         model bathymetry
-    mz: int
+    mz: np.ndarray
         land/water mask
-    iob: int
+    iob: np.ndarray
         open boundary index
-    dt: float
+    dt: np.ndarray
         time step
     """
     # open the file
     fid = open(os.path.expanduser(input_file),'rb')
     fid.seek(4,0)
     # read data as big endian
     # get model dimensions and limits
@@ -915,39 +931,39 @@
     mz = np.fromfile(fid, dtype=np.dtype('>i4'), count=nx*ny).reshape(ny, nx)
     # close the file
     fid.close()
     # return values
     return (x, y, hz, mz, iob, dt)
 
 # PURPOSE: read tide grid file with localized solutions
-def read_atlas_grid(input_file):
+def read_atlas_grid(input_file: str):
     """
     Read ATLAS grid file to extract model coordinates, bathymetry, masks and
     indices for both global and local solutions
 
     Parameters
     ----------
     input_file: str
         input ATLAS grid file
 
     Returns
     -------
-    x: float
+    x: np.ndarray
         x-coordinates of input ATLAS grid
-    y: float
+    y: np.ndarray
         y-coordinates of input ATLAS grid
-    hz: float
+    hz: np.ndarray
         model bathymetry
-    mz: int
+    mz: np.ndarray
         land/water mask
-    iob: int
+    iob: np.ndarray
         open boundary index
     dt: float
         time step
-    pmask: int
+    pmask: np.ndarray
         global mask
     local: dict
         dictionary of local tidal solutions for grid variables
 
             - ``'depth'``: model bathymetry
     """
     # read the input file to get file information
@@ -1016,35 +1032,35 @@
         local[name] = dict(lon=ln1, lat=lt1, depth=depth)
     # close the file
     fid.close()
     # return values
     return (x, y, hz, mz, iob, dt, pmask, local)
 
 # PURPOSE: read grid file
-def read_netcdf_grid(input_file):
+def read_netcdf_grid(input_file: str):
     """
     Read netCDF4 grid file to extract model coordinates, bathymetry,
     masks and flexure scaling factors
 
     Parameters
     ----------
     input_file: str
         input grid file
 
     Returns
     -------
-    x: float
+    x: np.ndarray
         x-coordinates of input grid
-    y: float
+    y: np.ndarray
         y-coordinates of input grid
-    hz: float
+    hz: np.ndarray
         model bathymetry
-    mz: int
+    mz: np.ndarray
         land/water mask
-    sf: float
+    sf: np.ndarray
         scaling factor for applying ice flexure
     """
     # read the netcdf format tide grid file
     fileID = netCDF4.Dataset(os.path.expanduser(input_file),'r')
     # read coordinates and flip y orientation
     x = fileID.variables['x'][:].copy()
     y = fileID.variables['y'][::-1].copy()
@@ -1059,15 +1075,18 @@
     sf.mask = (sf.data == 0.0)
     # close the grid file
     fileID.close()
     # return values
     return (x, y, hz, mz, sf)
 
 # PURPOSE: read list of constituents from an elevation or transport file
-def read_constituents(input_file, grid='OTIS'):
+def read_constituents(
+        input_file: str,
+        grid: str = 'OTIS'
+    ):
     """
     Read the list of constituents from an elevation or transport file
 
     Parameters
     ----------
     input_file: str
         input tidal file
@@ -1102,28 +1121,31 @@
         fid.seek(16,1)
         constituents = [c.decode("utf8").rstrip() for c in fid.read(nc*4).split()]
         fid.close()
     return (constituents, nc)
 
 # PURPOSE: read elevation file to extract real and imaginary components for
 # constituent
-def read_otis_elevation(input_file,ic):
+def read_otis_elevation(
+        input_file: str,
+        ic: int
+    ):
     """
     Read elevation file to extract real and imaginary components for constituent
 
     Parameters
     ----------
     input_file: str
         input elevation file
     ic: int
         index of consituent
 
     Returns
     -------
-    h: float
+    h: np.ndarray
         tidal elevation
     """
     # open the file
     fid = open(os.path.expanduser(input_file),'rb')
     ll, = np.fromfile(fid, dtype=np.dtype('>i4'), count=1)
     nx,ny,nc = np.fromfile(fid, dtype=np.dtype('>i4'), count=3)
     # extract x and y limits
@@ -1146,15 +1168,19 @@
     # close the file
     fid.close()
     # return the elevation
     return h
 
 # PURPOSE: read elevation file with localized solutions to extract real and
 # imaginary components for constituent
-def read_atlas_elevation(input_file, ic, constituent):
+def read_atlas_elevation(
+        input_file: str,
+        ic: int,
+        constituent: str
+    ):
     """
     Read elevation file with localized solutions to extract real and imaginary
     components for constituent
 
     Parameters
     ----------
     input_file: str
@@ -1243,15 +1269,18 @@
     # close the file
     fid.close()
     # return the elevation
     return (h, local)
 
 # PURPOSE: read transport file to extract real and imaginary components for
 # constituent
-def read_otis_transport(input_file,ic):
+def read_otis_transport(
+        input_file: str,
+        ic: int
+    ):
     """
     Read transport file to extract real and imaginary components for constituent
 
     Parameters
     ----------
     input_file: str
         input transport file
@@ -1295,15 +1324,19 @@
     # close the file
     fid.close()
     # return the transport components
     return (u, v)
 
 # PURPOSE: read transport file with localized solutions to extract real and
 # imaginary components for constituent
-def read_atlas_transport(input_file, ic, constituent):
+def read_atlas_transport(
+        input_file: str,
+        ic: int,
+        constituent: str
+    ):
     """
     Read transport file with localized solutions to extract real and imaginary
     components for constituent
 
     Parameters
     ----------
     input_file: str
@@ -1311,17 +1344,17 @@
     ic: int
         index of consituent
     constituent: str
         tidal constituent ID
 
     Returns
     -------
-    u: float
+    u: np.ndarray
         global zonal tidal transport
-    v: float
+    v: np.ndarray
         global meridional zonal transport
     local: dict
         dictionary of local tidal solutions for transport variables
 
             - ``'u'``: zonal tidal transport
             - ``'v'``: meridional zonal transport
     """
@@ -1410,43 +1443,49 @@
             fid.seek(nskip,1)
     # close the file
     fid.close()
     # return the transport components
     return (u, v, local)
 
 # PURPOSE: create a 2 arc-minute grid mask from mz and depth variables
-def create_atlas_mask(xi, yi, mz, local, variable=None):
+def create_atlas_mask(
+        xi: np.ndarray,
+        yi: np.ndarray,
+        mz: np.ndarray,
+        local: dict,
+        variable: str | None = None
+    ):
     """
     Creates a high-resolution grid mask from model variables
 
     Parameters
     ----------
-    xi: float
+    xi: np.ndarray
         input x-coordinates of global tide model
-    yi: float
+    yi: np.ndarray
         input y-coordinates of global tide model
-    mz: int
+    mz: np.ndarray
         global land/water mask
     local: dict
         dictionary of local tidal solutions
     variable: str or NoneType, default None
         key for variable within each local solution
 
             - ``'depth'``: model bathymetry
             - ``'z'``: tidal elevation
             - ``'u'``: zonal tidal transport
             - ``'v'``: meridional zonal transport
 
     Returns
     -------
-    x30: float
+    x30: np.ndarray
         x-coordinates of high-resolution tide model
-    y30: float
+    y30: np.ndarray
         y-coordinates of high-resolution tide model
-    m30: int
+    m30: np.ndarray
         high-resolution land/water mask
     """
     # create 2 arc-minute grid dimensions
     d30 = 1.0/30.0
     x30 = np.arange(d30/2.0, 360.0+d30/2.0, d30)
     y30 = np.arange(-90.0+d30/2.0, 90.0+d30/2.0, d30)
     # interpolate global mask to create initial 2 arc-minute mask
@@ -1478,37 +1517,42 @@
         # fill global mask with regional solution
         m30[jj,ii] = 1
     # return the 2 arc-minute mask
     m30.mask = (m30.data == m30.fill_value)
     return m30
 
 # PURPOSE: resample global solution to higher-resolution
-def interpolate_atlas_model(xi, yi, zi, spacing=1.0/30.0):
+def interpolate_atlas_model(
+        xi: np.ndarray,
+        yi: np.ndarray,
+        zi: np.ndarray,
+        spacing: float = 1.0/30.0
+    ):
     """
     Interpolates global ATLAS tidal solutions into a
     higher-resolution sampling
 
     Parameters
     ----------
-    xi: float
+    xi: np.ndarray
         input x-coordinates of global tide model
-    yi: float
+    yi: np.ndarray
         input y-coordinates of global tide model
-    zi: float
+    zi: np.ndarray
         global tide model data
     spacing: float
         output grid spacing
 
     Returns
     -------
-    xs: float
+    xs: np.ndarray
         x-coordinates of high-resolution tide model
-    ys: float
+    ys: np.ndarray
         y-coordinates of high-resolution tide model
-    zs: float
+    zs: np.ndarray
         high-resolution tidal solution for variable
     """
     # create resampled grid dimensions
     xs = np.arange(spacing/2.0, 360.0+spacing/2.0, spacing)
     ys = np.arange(-90.0+spacing/2.0, 90.0+spacing/2.0, spacing)
     # interpolate global solution
     zs = np.ma.zeros((len(ys),len(xs)), dtype=zi.dtype)
@@ -1522,46 +1566,53 @@
     else:
         f = scipy.interpolate.RectBivariateSpline(xi, yi, zi.T, kx=1,ky=1)
         zs.data[:,:] = f(xs,ys).T
     # return resampled solution and coordinates
     return (xs, ys, zs)
 
 # PURPOSE: combines global and local atlas solutions
-def combine_atlas_model(xi, yi, zi, pmask, local, variable=None):
+def combine_atlas_model(
+        xi: np.ndarray,
+        yi: np.ndarray,
+        zi: np.ndarray,
+        pmask: np.ndarray,
+        local: dict,
+        variable: str | None = None
+    ):
     """
     Combines global and local ATLAS tidal solutions into a single
     high-resolution solution
 
     Parameters
     ----------
-    xi: float
+    xi: np.ndarray
         input x-coordinates of global tide model
-    yi: float
+    yi: np.ndarray
         input y-coordinates of global tide model
-    zi: float
+    zi: np.ndarray
         global tide model data
-    pmask: int
+    pmask: np.ndarray
         global mask
     local: dict
         dictionary of local tidal solutions
     variable: str or NoneType, default None
         key for variable within each local solution
 
             - ``'depth'``: model bathymetry
             - ``'z'``: tidal elevation
             - ``'u'``: zonal tidal transport
             - ``'v'``: meridional zonal transport
 
     Returns
     -------
-    x30: float
+    x30: np.ndarray
         x-coordinates of high-resolution tide model
-    y30: float
+    y30: np.ndarray
         y-coordinates of high-resolution tide model
-    z30: float
+    z30: np.ndarray
         combined high-resolution tidal solution for variable
     """
     # create 2 arc-minute grid dimensions
     d30 = 1.0/30.0
     # interpolate global solution to 2 arc-minute solution
     x30, y30, z30 = interpolate_atlas_model(xi, yi, zi, spacing=d30)
     # iterate over localized solutions
@@ -1586,15 +1637,19 @@
         # fill global mask with regional solution
         z30.data[jj,ii] = val[variable][validy,validx]
     # return 2 arc-minute solution and coordinates
     return (x30, y30, z30)
 
 # PURPOSE: read netCDF4 file to extract real and imaginary components for
 # constituent
-def read_netcdf_file(input_file, ic, variable=None):
+def read_netcdf_file(
+        input_file: str,
+        ic: int,
+        variable: str | None = None
+    ):
     """
     Read netCDF4 file to extract real and imaginary components for constituent
 
     Parameters
     ----------
     input_file: str
         input transport file
@@ -1634,31 +1689,39 @@
         hc.data.imag[:,:] = -fileID.variables['vIm'][ic,::-1,:]
     # close the file
     fileID.close()
     # return output variables
     return hc
 
 # PURPOSE: output grid file in OTIS format
-def output_otis_grid(FILE, xlim, ylim, hz, mz, iob, dt):
+def output_otis_grid(
+        FILE: str,
+        xlim: np.ndarray | list,
+        ylim: np.ndarray | list,
+        hz: np.ndarray,
+        mz: np.ndarray,
+        iob: np.ndarray,
+        dt: float
+    ):
     """
     Writes OTIS-format grid files
 
     Parameters
     ----------
     FILE: str
         output OTIS grid file name
-    xlim: float
+    xlim: np.ndarray
         x-coordinate grid-cell edges of output grid
-    ylim: float
+    ylim: np.ndarray
         y-coordinate grid-cell edges of output grid
-    hz:float
+    hz: np.ndarray
         bathymetry
-    mz: int
+    mz: np.ndarray
         land/water mask
-    iob: int
+    iob: np.ndarray
         open boundary index
     dt: float
         time step
     """
     # open this way for files
     fid = open(os.path.expanduser(FILE), 'wb')
     nob = len(iob)
@@ -1692,27 +1755,33 @@
     for m in range(ny):
         mz[m,:].tofile(fid,format='>i4')
     fid.write(struct.pack('>i',reclen))
     # close the output OTIS file
     fid.close()
 
 # PURPOSE: output elevation file in OTIS format
-def output_otis_elevation(FILE, h, xlim, ylim, constituents):
+def output_otis_elevation(
+        FILE: str,
+        h: np.ndarray,
+        xlim: np.ndarray | list,
+        ylim: np.ndarray | list,
+        constituents: list
+    ):
     """
     Writes OTIS-format elevation files
 
     Parameters
     ----------
     FILE: str
         output OTIS elevation file name
-    h: complex
+    h: np.ndarray
         Eulerian form of tidal height oscillation
-    xlim: float
+    xlim: np.ndarray
         x-coordinate grid-cell edges of output grid
-    ylim: float
+    ylim: np.ndarray
         y-coordinate grid-cell edges of output grid
     constituents: list
         tidal constituent IDs
     """
     fid = open(os.path.expanduser(FILE), 'wb')
     ny, nx, nc = np.shape(h)
     # length of header: allow for 4 character >i c_id strings
@@ -1736,15 +1805,22 @@
             temp[1:2*nx:2] = h.imag[m,:,ic]
             temp.tofile(fid,format='>f4')
         fid.write(struct.pack('>i',constituent_header))
     # close the output OTIS file
     fid.close()
 
 # PURPOSE: output transport file in OTIS format
-def output_otis_transport(FILE, u, v, xlim, ylim, constituents):
+def output_otis_transport(
+        FILE: str,
+        u: np.ndarray,
+        v: np.ndarray,
+        xlim: np.ndarray | list,
+        ylim: np.ndarray | list,
+        constituents: list
+    ):
     """
     Writes OTIS-format transport files
 
     Parameters
     ----------
     FILE: str
         output OTIS transport file name
@@ -1785,15 +1861,15 @@
             temp.tofile(fid,format='>f4')
         fid.write(struct.pack('>i',constituent_header))
     # close the output OTIS file
     fid.close()
 
 # For a rectangular bathymetry grid:
 # construct masks for zeta, u and v nodes on a C-grid
-def Muv(hz):
+def Muv(hz: np.ndarray):
     """
     Construct masks for zeta, u and v nodes on a C-grid
     """
     ny, nx = np.shape(hz)
     mz = (hz > 0).astype(int)
     # x-indices
     indx = np.zeros((nx), dtype=int)
@@ -1807,15 +1883,15 @@
     mu = np.zeros((ny, nx), dtype=int)
     mv = np.zeros((ny, nx), dtype=int)
     mu[indy,:] = mz*mz[indy,:]
     mv[:,indx] = mz*mz[:,indx]
     return (mu, mv, mz)
 
 # PURPOSE: Interpolate bathymetry to zeta, u and v nodes on a C-grid
-def Huv(hz):
+def Huv(hz: np.ndarray):
     """
     Interpolate bathymetry to zeta, u and v nodes on a C-grid
     """
     ny, nx = np.shape(hz)
     mu, mv, mz = Muv(hz)
     # x-indices
     indx = np.zeros((nx), dtype=int)
```

### Comparing `pyTMD-2.0.2/pyTMD/io/constituents.py` & `pyTMD-2.0.3/pyTMD/io/constituents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python
 u"""
 constituents.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 Basic tide model constituent class
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Written 12/2022
 """
+from __future__ import division, annotations
+
 import numpy as np
 
 class constituents:
     """
     Class for tide model constituents
 
     Attributes
@@ -27,106 +30,106 @@
         # set initial attributes
         self.fields = []
         self.__index__ = 0
         # set optional fields
         for key, val in kwargs.items():
             setattr(self, key, val)
 
-    def append(self, field, constituent):
+    def append(self, field: str, constituent: np.ndarray):
         """
         Append a tide model constituent
 
         Parameters
         ----------
         field: str
             Tide model constituent name
-        constituent: float
+        constituent: np.ndarray
             Tide model constituent (complex form)
         """
         # append field
         self.fields.append(field)
         setattr(self, field, constituent)
         return self
 
-    def get(self, field):
+    def get(self, field: str):
         """
         Get a tide model constituent
 
         Parameters
         ----------
         field: str
             Tide model constituent name
 
         Returns
         -------
-        constituent: float
+        constituent: np.ndarray
             Tide model constituent (complex form)
         """
         return getattr(self, field)
 
-    def pop(self, field):
+    def pop(self, field: str):
         """
         Retrieve a tide model constituent and remove from list
 
         Parameters
         ----------
         field: str
             Tide model constituent name
 
         Returns
         -------
-        constituent: float
+        constituent: np.ndarray
             Tide model constituent (complex form)
         """
         self.fields.remove(field)
         constituent = getattr(self, field)
         delattr(self, field)
         return constituent
 
-    def update(self, field, constituent):
+    def update(self, field: str, constituent: np.ndarray):
         """
         Update a tide model constituent
 
         Parameters
         ----------
         field: str
             Tide model constituent name
-        constituent: float
+        constituent: np.ndarray
             Tide model constituent (complex form)
         """
         # raise exception if field not in list
         if not hasattr(self, field):
             raise KeyError(f'Constituent {field}')
         # update the constituent
         setattr(self, field, constituent)
         return self
 
-    def amplitude(self, field):
+    def amplitude(self, field: str):
         """
         Calculate the amplitude of a tide model constituent
 
         Parameters
         ----------
         field: str
             Tide model constituent name
 
         Returns
         -------
-        amp: float
+        amp: np.ndarray
             Tide model constituent amplitude
         """
         constituent = getattr(self, field)
         # calculate constituent amplitude
         amp = np.sqrt(constituent.real**2 + constituent.imag**2)
         # update mask and fill values
         amp.mask = np.copy(constituent.mask)
         amp.data[amp.mask] = amp.fill_value
         return amp
 
-    def phase(self, field):
+    def phase(self, field: str):
         """
         Calculate the phase of a tide model constituent
 
         Parameters
         ----------
         field: str
             Tide model constituent name
```

### Comparing `pyTMD-2.0.2/pyTMD/io/model.py` & `pyTMD-2.0.3/pyTMD/io/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 u"""
 model.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (04/2023)
 Retrieves tide model parameters for named tide models and
     from model definition files
 
 UPDATE HISTORY:
+    Updated 04/2023: added global HAMTIDE11 model
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: moved to io and added deprecation warning to old
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 06/2022: added Greenland 1km model (Gr1kmTM) to list of models
         updated citation url for Global Ocean Tide (GOT) models
     Updated 05/2022: added ESR CATS2022 to list of models
         added attribute for flexure fields being available for model
     Updated 04/2022: updated docstrings to numpy documentation format
@@ -18,14 +20,16 @@
     Updated 03/2022: added static decorators to define model lists
     Updated 02/2022: added Arctic 2km model (Arc2kmTM) to list of models
     Updated 01/2022: added global Empirical Ocean Tide model (EOT20)
     Updated 12/2021: added TPXO9-atlas-v5 to list of available tide models
         added atl10 attributes for tidal elevation files
     Written 09/2021
 """
+from __future__ import annotations
+
 import os
 import re
 import io
 import copy
 
 class model:
     """Retrieves tide model parameters for named models or
@@ -128,15 +132,15 @@
         self.reference = None
         self.scale = None
         self.type = None
         self.variable = None
         self.verify = copy.copy(kwargs['verify'])
         self.version = None
 
-    def grid(self, m):
+    def grid(self, m: str):
         """
         Create a model object from known tide grid files
 
         Parameters
         ----------
         m: str
             model name
@@ -228,15 +232,15 @@
             self.grid_file = self.pathfinder('grid_Greenland8.v2')
             self.version = 'v2'
         else:
             raise Exception("Unlisted tide model")
         # return the model parameters
         return self
 
-    def elevation(self, m):
+    def elevation(self, m: str):
         """
         Create a model object from known tidal elevation models
 
         Parameters
         ----------
         m: str
             model name
@@ -958,20 +962,44 @@
             self.atl11 = 'tide_load'
             self.atl12 = 'tide_load_seg'
             self.gla12 = 'd_ldElv'
             self.variable = 'tide_load'
             self.long_name = "Load Tide"
             self.description = ("Local displacement due to Ocean "
                 "Loading (-6 to 0 cm)")
+        elif (m == 'HAMTIDE11'):
+            self.format = 'FES'
+            self.model_directory = os.path.join(self.directory,'hamtide')
+            model_files = ['2n.hamtide11a.nc','k1.hamtide11a.nc','k2.hamtide11a.nc',
+                'm2.hamtide11a.nc','n2.hamtide11a.nc','o1.hamtide11a.nc',
+                'p1.hamtide11a.nc','q1.hamtide11a.nc','s2.hamtide11a.nc']
+            self.model_file = self.pathfinder(model_files)
+            self.constituents = ['2n2','k1','k2','m2','n2','o1','p1','q1','s2']
+            self.scale = 1.0/100.0
+            self.version = 'HAMTIDE11'
+            # model description and references
+            self.reference = 'https://doi.org/10.1002/2013JC009766'
+            self.atl03 = 'tide_ocean'
+            self.atl06 = 'tide_ocean'
+            self.atl07 = 'height_segment_ocean'
+            self.atl10 = 'height_segment_ocean'
+            self.atl11 = 'tide_ocean'
+            self.atl12 = 'tide_ocean_seg'
+            self.gla12 = 'd_ocElv'
+            self.variable = 'tide_ocean'
+            self.long_name = "Ocean Tide"
+            self.description = ("Ocean Tides including diurnal and "
+                "semi-diurnal (harmonic analysis), and longer period "
+                "tides (dynamic and self-consistent equilibrium).")
         else:
             raise Exception("Unlisted tide model")
         # return the model parameters
         return self
 
-    def current(self, m):
+    def current(self, m: str):
         """
         Create a model object from known tidal current models
 
         Parameters
         ----------
         m: str
             model name
@@ -1225,191 +1253,212 @@
                 'm6.nc','m8.nc','mf.nc','mks2.nc','mm.nc',
                 'mn4.nc','ms4.nc','msf.nc','msqm.nc','mtm.nc',
                 'mu2.nc','n2.nc','n4.nc','nu2.nc','o1.nc','p1.nc',
                 'q1.nc','r2.nc','s1.nc','s2.nc','s4.nc','sa.nc',
                 'ssa.nc','t2.nc']
             self.model_file = {}
             for key,val in model_directory.items():
-                self.model_directory = os.path.expanduser(model_directory)
-                self.model_file[key] = self.pathfinder(val)
+                self.model_directory = os.path.expanduser(val)
+                self.model_file[key] = self.pathfinder(model_files)
             self.constituents = ['2n2','eps2','j1','k1','k2','l2','lambda2',
                 'm2','m3','m4','m6','m8','mf','mks2','mm','mn4','ms4','msf',
                 'msqm','mtm','mu2','n2','n4','nu2','o1','p1','q1','r2','s1',
                 's2','s4','sa','ssa','t2']
             self.scale = 1.0
             self.version = 'FES2014'
             # model description and references
             self.reference = ('https://www.aviso.altimetry.fr/en/data/products'
                 'auxiliary-products/global-tide-fes.html')
+        elif (m == 'HAMTIDE11'):
+            self.format = 'FES'
+            model_directory = {}
+            model_directory['u'] = os.path.join(self.directory,'hamtide')
+            model_directory['v'] = os.path.join(self.directory,'hamtide')
+            model_files = ['HAMcurrent11a_2n.nc','HAMcurrent11a_k1.nc',
+                'HAMcurrent11a_k2.nc','HAMcurrent11a_m2.nc',
+                'HAMcurrent11a_n2.nc','HAMcurrent11a_o1.nc',
+                'HAMcurrent11a_p1.nc','HAMcurrent11a_q1.nc',
+                'HAMcurrent11a_s2.nc']
+            self.model_file = {}
+            for key,val in model_directory.items():
+                self.model_directory = os.path.expanduser(val)
+                self.model_file[key] = self.pathfinder(model_files)
+            self.constituents = ['2n2','k1','k2','m2','n2','o1','p1','q1','s2']
+            self.scale = 1.0
+            self.version = 'HAMTIDE11'
+            # model description and references
+            self.reference = 'https://doi.org/10.1002/2013JC009766'
         else:
             raise Exception("Unlisted tide model")
         # return the model parameters
         return self
 
     @property
-    def gzip(self):
+    def gzip(self) -> str:
         """
         Returns suffix for gzip compression
         """
         return '.gz' if self.compressed else ''
 
     @property
-    def suffix(self):
+    def suffix(self) -> str:
         """
         Returns format suffix for netCDF4 ATLAS files
         """
         return '.nc' if (self.format == 'netcdf') else ''
 
     @staticmethod
-    def global_ocean():
+    def global_ocean() -> list:
         """
         Returns list of global ocean tide elevation models
         """
         return ['TPXO9-atlas','TPXO9-atlas-v2','TPXO9-atlas-v3',
             'TPXO9-atlas-v4','TPXO9-atlas-v5','TPXO9.1','TPXO8-atlas',
-            'TPXO7.2','GOT4.7','GOT4.8','GOT4.10','FES2014','EOT20']
+            'TPXO7.2','GOT4.7','GOT4.8','GOT4.10','FES2014','EOT20',
+            'HAMTIDE11']
 
     @staticmethod
-    def global_load():
+    def global_load() -> list:
         """
         Returns list of global load tide elevation models
         """
         return ['TPXO7.2_load','GOT4.7_load','GOT4.8_load',
             'GOT4.10_load','FES2014_load','EOT20_load']
 
     @staticmethod
-    def global_current():
+    def global_current() -> list:
         """
         Returns list of global tidal current models
         """
         return ['TPXO9-atlas','TPXO9-atlas-v2',
             'TPXO9-atlas-v3','TPXO9-atlas-v4','TPXO9-atlas-v5',
-            'TPXO9.1','TPXO8-atlas','TPXO7.2','FES2014']
+            'TPXO9.1','TPXO8-atlas','TPXO7.2','FES2014','HAMTIDE11']
 
     @staticmethod
-    def antarctic_ocean():
+    def antarctic_ocean() -> list:
         """
         Returns list of Antarctic ocean tide elevation models
         """
         return ['CATS0201','CATS2008','CATS2022']
 
     @staticmethod
-    def antarctic_load():
+    def antarctic_load() -> list:
         """
         Returns list of Antarctic load tide elevation models
         """
         return ['CATS2008_load']
 
     @staticmethod
-    def antarctic_current():
+    def antarctic_current() -> list:
         """
         Returns list of Antarctic tidal current models
         """
         return ['CATS0201','CATS2008','CATS2022']
 
     @staticmethod
-    def arctic_ocean():
+    def arctic_ocean() -> list:
         """
         Returns list of Arctic ocean tide elevation models
         """
         return ['AODTM-5','AOTIM-5','AOTIM-5-2018','Arc2kmTM',
             'Gr1kmTM','Gr1km-v2']
 
     @staticmethod
-    def arctic_load():
+    def arctic_load() -> list:
         """
         Returns list of Arctic load tide elevation models
         """
         return []
 
     @staticmethod
-    def arctic_current():
+    def arctic_current() -> list:
         """
         Returns list of Arctic tidal current models
         """
         return ['AODTM-5','AOTIM-5','AOTIM-5-2018','Arc2kmTM',
             'Gr1kmTM','Gr1km-v2']
 
     @staticmethod
-    def ocean_elevation():
+    def ocean_elevation() -> list:
         """
         Returns list of ocean tide elevation models
         """
         return ['CATS0201','CATS2008','CATS2022','TPXO9-atlas',
             'TPXO9-atlas-v2','TPXO9-atlas-v3','TPXO9-atlas-v4',
             'TPXO9-atlas-v5','TPXO9.1','TPXO8-atlas','TPXO7.2',
             'AODTM-5','AOTIM-5','AOTIM-5-2018','Arc2kmTM','Gr1kmTM',
-            'Gr1km-v2','GOT4.7','GOT4.8','GOT4.10','FES2014','EOT20']
+            'Gr1km-v2','GOT4.7','GOT4.8','GOT4.10','FES2014','EOT20',
+            'HAMTIDE11']
 
     @staticmethod
-    def load_elevation():
+    def load_elevation() -> list:
         """
         Returns list of load tide elevation models
         """
         return ['CATS2008_load','TPXO7.2_load','GOT4.7_load',
             'GOT4.8_load','GOT4.10_load','FES2014_load','EOT20_load']
 
     @staticmethod
-    def ocean_current():
+    def ocean_current() -> list:
         """
         Returns list of tidal current models
         """
         return ['CATS0201','CATS2008','CATS2022''TPXO9-atlas',
             'TPXO9-atlas-v2','TPXO9-atlas-v3','TPXO9-atlas-v4',
             'TPXO9-atlas-v5','TPXO9.1','TPXO8-atlas','TPXO7.2',
             'AODTM-5','AOTIM-5','AOTIM-5-2018',
-            'Arc2kmTM','Gr1kmTM','Gr1km-v2','FES2014']
+            'Arc2kmTM','Gr1kmTM','Gr1km-v2','FES2014','HAMTIDE11']
 
     @staticmethod
-    def OTIS():
+    def OTIS() -> list:
         """
         Returns list of OTIS format models
         """
         return ['CATS0201','CATS2008','CATS2008_load','TPXO9.1',
             'TPXO7.2','TPXO7.2_load','AODTM-5','AOTIM-5',
             'AOTIM-5-2018','Arc2kmTM','Gr1kmTM','Gr1km-v2']
 
     @staticmethod
-    def ATLAS_compact():
+    def ATLAS_compact() -> list:
         """
         Returns list of ATLAS compact format models
         """
         return ['TPXO8-atlas']
 
     @staticmethod
-    def ESR():
+    def ESR() -> list:
         """
         Returns list of ESR format models
         """
         return ['CATS2022']
 
     @staticmethod
-    def ATLAS():
+    def ATLAS() -> list:
         """
         Returns list of ATLAS format models
         """
         return ['TPXO9-atlas','TPXO9-atlas-v2','TPXO9-atlas-v3',
             'TPXO9-atlas-v4','TPXO9-atlas-v5']
 
     @staticmethod
-    def GOT():
+    def GOT() -> list:
         """
         Returns list of GOT format models
         """
         return ['GOT4.7','GOT4.7_load','GOT4.8','GOT4.8_load',
             'GOT4.10','GOT4.10_load']
 
     @staticmethod
-    def FES():
+    def FES() -> list:
         """
         Returns list of FES format models
         """
-        return ['FES2014','FES2014_load','EOT20','EOT20_load']
+        return ['FES2014','FES2014_load','EOT20','EOT20_load','HAMTIDE11']
 
-    def pathfinder(self, model_file):
+    def pathfinder(self, model_file: str | list):
         """
         Completes file paths and appends file and gzip suffixes
 
         Parameters
         ----------
         model_file: str or list
             model file(s) to complete
@@ -1424,15 +1473,15 @@
             valid = os.access(output_file, os.F_OK)
         # check that (all) output files exist
         if self.verify and not valid:
             raise FileNotFoundError(output_file)
         # return the complete output path
         return output_file
 
-    def from_file(self, definition_file):
+    def from_file(self, definition_file: str):
         """
         Create a model object from an input definition file
 
         Parameters
         ----------
         definition_file: str
             model definition file for creating model object
@@ -1488,29 +1537,29 @@
             temp.type = re.split(r'[\s\,]+',temp.type)
         # convert boolean strings
         if isinstance(temp.compressed,str):
             temp.compressed = self.to_bool(temp.compressed)
         # return the model parameters
         return temp
 
-    def from_dict(self, d):
+    def from_dict(self, d: dict):
         """
         Create a model object from a python dictionary
 
         Parameters
         ----------
         d: dict
             Python dictionary for creating model object
         """
         for key,val in d.items():
             setattr(self,key,copy.copy(val))
         # return the model parameters
         return self
 
-    def to_bool(self, val):
+    def to_bool(self, val: str) -> bool:
         """
         Converts strings of True/False to a boolean values
 
         Parameters
         ----------
         val: str
             string for converting to True/False
```

### Comparing `pyTMD-2.0.2/pyTMD/io/ocean_pole_tide.py` & `pyTMD-2.0.3/pyTMD/io/ocean_pole_tide.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 ocean_pole_tide.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 
 Reads ocean pole load tide coefficients provided by IERS
 http://maia.usno.navy.mil/conventions/2010/2010_official/chapter7/tn36_c7.pdf
 http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/icc7.pdf
 
 IERS 0.5x0.5 map of ocean pole tide coefficients:
 ftp://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/
@@ -27,50 +27,53 @@
     S Desai, "Observing the pole tide with satellite altimetry", Journal of
         Geophysical Research: Oceans, 107(C11), 2002. doi: 10.1029/2001JC001224
     S Desai, J Wahr and B Beckley "Revisiting the pole tide for and from
         satellite altimetry", Journal of Geodesy, 89(12), p1233-1243, 2015.
         doi: 10.1007/s00190-015-0848-7
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor ocean pole tide read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
         use longcomplex data format to be windows compliant
     Updated 07/2021: added check that ocean pole tide file is accessible
     Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
     Updated 08/2020: output north load and east load deformation components
     Updated 07/2020: added function docstrings
     Updated 12/2018: Compatibility updates for Python3
     Written 09/2017
 """
+from __future__ import annotations
+
 import os
 import re
 import gzip
 import numpy as np
 
 # PURPOSE: read real and imaginary ocean pole tide coefficients
-def ocean_pole_tide(input_file):
+def ocean_pole_tide(input_file: str):
     """
     Read real and imaginary ocean pole tide coefficients
 
     Parameters
     ----------
     input_file: str
         IERS map of ocean pole tide coefficients
 
     Returns
     -------
-    ur: float
+    ur: np.ndarray
         radial ocean pole tide coefficients
-    un: float
+    un: np.ndarray
         north ocean pole tide coefficients
-    ue: float
+    ue: np.ndarray
         east ocean pole tide coefficients
-    glon: float
+    glon: np.ndarray
         ocean grid longitude
-    glat: float
+    glat: np.ndarray
         ocean grid latitude
 
     References
     ----------
     .. [1] S Desai, "Observing the pole tide with satellite altimetry", *Journal of
         Geophysical Research: Oceans*, 107(C11), (2002).
         `doi: 10.1029/2001JC001224 <https://doi.org/10.1029/2001JC001224>`_
@@ -121,48 +124,53 @@
     glon = extend_array(glon,dlon)
     ur = extend_matrix(ur)
     un = extend_matrix(un)
     ue = extend_matrix(ue)
     # return values
     return (ur, un, ue, glon, glat)
 
-# PURPOSE: wrapper function to extend an array
-def extend_array(input_array,step_size):
+# PURPOSE: Extend a longitude array
+def extend_array(input_array: np.ndarray, step_size: float):
     """
-    Wrapper function to extend an array
+    Extends a longitude array
 
     Parameters
     ----------
-    input_array: array to extend
-    step_size: step size between elements of array
+    input_array: np.ndarray
+        array to extend
+    step_size: float
+        step size between elements of array
 
     Returns
     -------
-    temp: extended array
+    temp: np.ndarray
+        extended array
     """
     n = len(input_array)
-    temp = np.zeros((n+2),dtype=input_array.dtype)
+    temp = np.zeros((n+2), dtype=input_array.dtype)
     # extended array [x-1,x0,...,xN,xN+1]
     temp[0] = input_array[0] - step_size
     temp[1:-1] = input_array[:]
     temp[-1] = input_array[-1] + step_size
     return temp
 
-# PURPOSE: wrapper function to extend a matrix
-def extend_matrix(input_matrix):
+# PURPOSE: Extend a global matrix
+def extend_matrix(input_matrix: np.ndarray):
     """
-    Wrapper function to extend a matrix
+    Extends a global matrix
 
     Parameters
     ----------
-    input_matrix: matrix to extend
+    input_matrix: np.ndarray
+        matrix to extend
 
     Returns
     -------
-    temp: extended matrix
+    temp: np.ndarray
+        extended matrix
     """
     nx,ny = np.shape(input_matrix)
-    temp = np.zeros((nx+2,ny),dtype=input_matrix.dtype)
+    temp = np.zeros((nx+2,ny), dtype=input_matrix.dtype)
     temp[0,:] = input_matrix[-1,:]
     temp[1:-1,:] = input_matrix[:,:]
     temp[-1,:] = input_matrix[0,:]
     return temp
```

### Comparing `pyTMD-2.0.2/pyTMD/load_constituent.py` & `pyTMD-2.0.3/pyTMD/load_constituent.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,8 +106,8 @@
         phase, = phase_all[j]
         omega, = omega_all[j]
         alpha, = alpha_all[j]
         species, = species_all[j]
     else:
         amplitude = 0.0; phase = 0.0; omega = 0.0; alpha = 0.0; species = 0
     # return the values for the constituent
-    return (amplitude,phase,omega,alpha,species)
+    return (amplitude, phase, omega, alpha, species)
```

### Comparing `pyTMD-2.0.2/pyTMD/load_nodal_corrections.py` & `pyTMD-2.0.3/pyTMD/load_nodal_corrections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 u"""
-load_nodal_corrections.py (11/2022)
+load_nodal_corrections.py
+Written by Tyler Sutterley (04/2023)
 Calculates the nodal corrections for tidal constituents
 Modification of ARGUMENTS fortran subroutine by Richard Ray 03/1999
 
 CALLING SEQUENCE:
-    pu,pf,G = load_nodal_corrections(MJD,constituents)
+    pu,pf,G = load_nodal_corrections(MJD, constituents)
 
 INPUTS:
     MJD: Modified Julian Day of input date
     constituents: tidal constituent IDs
 
 OUTPUTS:
     pu,pf: nodal corrections for the constituents
@@ -21,26 +22,28 @@
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 PROGRAM DEPENDENCIES:
-    calc_astrol_longitudes.py: computes the basic astronomical mean longitudes
+    astro.py: computes the basic astronomical mean longitudes
 
 REFERENCES:
     A. T. Doodson and H. Warburg, "Admiralty Manual of Tides", HMSO, (1941).
     P. Schureman, "Manual of Harmonic Analysis and Prediction of Tides"
         US Coast and Geodetic Survey, Special Publication, 98, (1958).
     M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal model
         time series", Advances in Water Resources, 12, (1989).
     G. D. Egbert and S. Erofeeva, "Efficient Inverse Modeling of Barotropic
         Ocean Tides", Journal of Atmospheric and Oceanic Technology, (2002).
 
 UPDATE HISTORY:
+    Updated 04/2023: using renamed astro mean_longitudes function
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 05/2022: added ESR netCDF4 formats to list of model types
         changed keyword arguments to camel case
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 12/2020: fix k1 for FES models
     Updated 08/2020: change time variable names to not overwrite functions
         update nodal corrections for FES models
@@ -48,41 +51,47 @@
     Updated 09/2019: added netcdf option to corrections option
     Updated 08/2018: added correction option ATLAS for localized OTIS solutions
     Updated 07/2018: added option to use GSFC GOT nodal corrections
     Updated 09/2017: Rewritten in Python
     Rewritten in Matlab by Lana Erofeeva 01/2003
     Written by Richard Ray 03/1999
 """
+from __future__ import annotations
+
 import copy
 import warnings
 import numpy as np
-from pyTMD.calc_astrol_longitudes import calc_astrol_longitudes
+import pyTMD.astro
 
-def load_nodal_corrections(MJD, constituents, **kwargs):
+def load_nodal_corrections(
+        MJD: np.ndarray,
+        constituents: list | np.ndarray,
+        **kwargs
+    ):
     """
     Calculates the nodal corrections for tidal constituents
 
     Parameters
     ----------
-    MJD: float
+    MJD: np.ndarray
         modified julian day of input date
     constituents: list
         tidal constituent IDs
-    deltat: float, default 0.0
+    deltat: float or np.ndarray, default 0.0
         time correction for converting to Ephemeris Time (days)
     corrections: str, default 'OTIS'
         use nodal corrections from OTIS/ATLAS or GOT models
 
     Returns
     -------
-    pu: float
+    pu: np.ndarray
         nodal correction for the constituent amplitude
-    pf: float
+    pf: np.ndarray
         nodal correction for the constituent phase
-    G: float
+    G: np.ndarray
         phase correction in degrees
 
     References
     ----------
     .. [1] Doodson and Warburg, "Admiralty Manual of Tides", HMSO, (1941).
     .. [2] Schureman, "Manual of Harmonic Analysis and Prediction of Tides,"
         *US Coast and Geodetic Survey*, Special Publication, 98, (1958).
@@ -119,15 +128,15 @@
 
     # degrees to radians
     dtr = np.pi/180.0
 
     # set function for astronomical longitudes
     ASTRO5 = True if kwargs['corrections'] in ('GOT','FES') else False
     # convert from Modified Julian Dates into Ephemeris Time
-    s,h,p,omega,pp = calc_astrol_longitudes(MJD + kwargs['deltat'],
+    s,h,p,omega,pp = pyTMD.astro.mean_longitudes(MJD + kwargs['deltat'],
         ASTRO5=ASTRO5)
     hour = (MJD % 1)*24.0
     t1 = 15.0*hour
     t2 = 30.0*hour
     nt = len(np.atleast_1d(MJD))
 
     # Determine equilibrium arguments
```

### Comparing `pyTMD-2.0.2/pyTMD/spatial.py` & `pyTMD-2.0.3/pyTMD/spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 spatial.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (04/2023)
 
 Utilities for reading, writing and operating on spatial data
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -14,15 +14,20 @@
     h5py: Pythonic interface to the HDF5 binary data format
         https://www.h5py.org/
     gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL)
         https://pypi.python.org/pypi/GDAL
     PyYAML: YAML parser and emitter for Python
         https://github.com/yaml/pyyaml
 
+PROGRAM DEPENDENCIES:
+    constants.py: calculate reference parameters for common ellipsoids
+
 UPDATE HISTORY:
+    Updated 04/2023: copy inputs in cartesian to not modify original arrays
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 02/2023: use outputs from constants class for WGS84 parameters
         include more possible dimension names for gridded and drift outputs
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         split netCDF4 output into separate functions for grid and drift types
     Updated 12/2022: add software information to output HDF5 and netCDF4
     Updated 11/2022: place some imports within try/except statements
         added encoding for writing ascii files
@@ -49,14 +54,16 @@
     Updated 01/2021: add streaming from bytes for ascii, netCDF4, HDF5, geotiff
         set default time for geotiff files to 0
     Updated 12/2020: added module for converting ellipsoids
     Updated 11/2020: output data as masked arrays if containing fill values
         add functions to read from and write to geotiff image formats
     Written 09/2020
 """
+from __future__ import annotations
+
 import os
 import re
 import io
 import copy
 import gzip
 import uuid
 import yaml
@@ -82,15 +89,15 @@
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
-def case_insensitive_filename(filename):
+def case_insensitive_filename(filename: str) -> str:
     """
     Searches a directory for a filename without case dependence
 
     Parameters
     ----------
     filename: str
         input filename
@@ -102,25 +109,25 @@
         directory = os.path.dirname(os.path.expanduser(filename))
         f = [f for f in os.listdir(directory) if re.match(basename,f,re.I)]
         if not f:
             raise FileNotFoundError(f'{filename} not found in file system')
         filename = os.path.join(directory,f.pop())
     return os.path.expanduser(filename)
 
-def data_type(x, y, t):
+def data_type(x: np.ndarray, y: np.ndarray, t: np.ndarray) -> str:
     """
     Determines input data type based on variable dimensions
 
     Parameters
     ----------
-    x: float
+    x: np.ndarray
         x-dimension coordinates
-    y: float
+    y: np.ndarray
         y-dimension coordinates
-    t: float
+    t: np.ndarray
         time-dimension coordinates
 
     Returns
     -------
     string denoting input data type
 
         - ``'time series'``
@@ -137,15 +144,15 @@
     elif (np.ndim(x) > 1) & (xsize == ysize):
         return 'grid'
     elif (xsize != ysize):
         return 'grid'
     else:
         raise ValueError('Unknown data type')
 
-def from_file(filename, format, **kwargs):
+def from_file(filename: str, format: str, **kwargs):
     """
     Wrapper function for reading data from an input format
 
     Parameters
     ----------
     filename: str
         full path of input file
@@ -163,15 +170,15 @@
         dinput = from_HDF5(filename, **kwargs)
     elif (format == 'geotiff'):
         dinput = from_geotiff(filename, **kwargs)
     else:
         raise ValueError(f'Invalid format {format}')
     return dinput
 
-def from_ascii(filename, **kwargs):
+def from_ascii(filename: str, **kwargs):
     """
     Read data from an ascii file
 
     Parameters
     ----------
     filename: str
         full path of input ascii file
@@ -274,15 +281,15 @@
     if 'data' in dinput.keys() and '_FillValue' in dinput['attributes']['data'].keys():
         dinput['data'] = np.ma.asarray(dinput['data'])
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # return the spatial variables
     return dinput
 
-def from_netCDF4(filename, **kwargs):
+def from_netCDF4(filename: str, **kwargs):
     """
     Read data from a netCDF4 file
 
     Parameters
     ----------
     filename: str
         full path of input netCDF4 file
@@ -378,15 +385,15 @@
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # Closing the NetCDF file
     fileID.close()
     # return the spatial variables
     return dinput
 
-def from_HDF5(filename, **kwargs):
+def from_HDF5(filename: str, **kwargs):
     """
     Read data from a HDF5 file
 
     Parameters
     ----------
     filename: str
         full path of input HDF5 file
@@ -483,15 +490,15 @@
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # Closing the HDF5 file
     fileID.close()
     # return the spatial variables
     return dinput
 
-def from_geotiff(filename, **kwargs):
+def from_geotiff(filename: str, **kwargs):
     """
     Read data from a geotiff file
 
     Parameters
     ----------
     filename: str
         full path of input geotiff file
@@ -583,15 +590,15 @@
         # set attribute for fill value
         dinput['attributes']['data']['_FillValue'] = dinput['data'].fill_value
     # close the dataset
     ds = None
     # return the spatial variables
     return dinput
 
-def to_ascii(output, attributes, filename, **kwargs):
+def to_ascii(output: dict, attributes: dict, filename: str, **kwargs):
     """
     Write data to an ascii file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -650,15 +657,15 @@
     # write to file for each data point
     for line in range(nrow):
         line_contents = [f'{d:0.8f}' for d in data_stack[:,line]]
         print(kwargs['delimiter'].join(line_contents), file=fid)
     # close the output file
     fid.close()
 
-def to_netCDF4(output, attributes, filename, **kwargs):
+def to_netCDF4(output: dict, attributes: dict, filename: str, **kwargs):
     """
     Wrapper function for writing data to a netCDF4 file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -698,15 +705,15 @@
             fileID.setncattr(att_name,att_val)
     # Output NetCDF structure information
     logging.info(filename)
     logging.info(list(fileID.variables.keys()))
     # Closing the NetCDF file
     fileID.close()
 
-def _drift_netCDF4(fileID, output, attributes, **kwargs):
+def _drift_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write drift data variables to a netCDF4 file object
 
     Parameters
     ----------
     fileID: obj
         open netCDF4 file object
@@ -731,15 +738,15 @@
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
         for att_name,att_val in attributes[key].items():
             nc[key].setncattr(att_name,att_val)
 
-def _grid_netCDF4(fileID, output, attributes, **kwargs):
+def _grid_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write gridded data variables to a netCDF4 file object
 
     Parameters
     ----------
     fileID: obj
         open netCDF4 file object
@@ -777,15 +784,15 @@
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
         for att_name,att_val in attributes[key].items():
             nc[key].setncattr(att_name,att_val)
 
-def _time_series_netCDF4(fileID, output, attributes, **kwargs):
+def _time_series_netCDF4(fileID, output: dict, attributes: dict, **kwargs):
     """
     Write time series data variables to a netCDF4 file object
 
     Parameters
     ----------
     fileID: obj
         open netCDF4 file object
@@ -818,15 +825,15 @@
             nc[key] = fileID.createVariable(key, val.dtype, ())
         # filling NetCDF variables
         nc[key][:] = val
         # Defining attributes for variable
         for att_name,att_val in attributes[key].items():
             nc[key].setncattr(att_name,att_val)
 
-def to_HDF5(output, attributes, filename, **kwargs):
+def to_HDF5(output: dict, attributes: dict, filename: str, **kwargs):
     """
     Write data to a HDF5 file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -866,15 +873,15 @@
             fileID.attrs[att_name] = att_val
     # Output HDF5 structure information
     logging.info(filename)
     logging.info(list(fileID.keys()))
     # Closing the HDF5 file
     fileID.close()
 
-def to_geotiff(output, attributes, filename, **kwargs):
+def to_geotiff(output: dict, attributes: dict, filename: str, **kwargs):
     """
     Write data to a geotiff file
 
     Parameters
     ----------
     output: dict
         python dictionary of output data
@@ -928,15 +935,15 @@
         # write band to geotiff array
         ds.GetRasterBand(band+1).WriteArray(output[varname][:,:,band])
     # print filename if verbose
     logging.info(filename)
     # close dataset
     ds.FlushCache()
 
-def expand_dims(obj, varname='data'):
+def expand_dims(obj: dict, varname: str = 'data'):
     """
     Add a singleton dimension to a spatial dictionary if non-existent
 
     Parameters
     ----------
     obj: dict
         python dictionary of data
@@ -953,15 +960,15 @@
         for v in varname:
             obj[v] = np.atleast_3d(obj[v])
     elif isinstance(varname,str):
         obj[varname] = np.atleast_3d(obj[varname])
     # return reformed spatial dictionary
     return obj
 
-def default_field_mapping(variables):
+def default_field_mapping(variables: list | np.ndarray):
     """
     Builds field mappings from a variable list
 
 
     Parameters
     ----------
     variables: list
@@ -983,23 +990,32 @@
         try:
             field_mapping[var] = copy.copy(variables[i])
         except IndexError as exc:
             pass
     # return the field mapping
     return field_mapping
 
-def convert_ellipsoid(phi1, h1, a1, f1, a2, f2, eps=1e-12, itmax=10):
+def convert_ellipsoid(
+        phi1: np.ndarray,
+        h1: np.ndarray,
+        a1: float,
+        f1: float,
+        a2: float,
+        f2: float,
+        eps: float = 1e-12,
+        itmax: int = 10
+    ):
     """
     Convert latitudes and heights to a different ellipsoid using Newton-Raphson
 
     Parameters
     ----------
-    phi1: float
+    phi1: np.ndarray
         latitude of input ellipsoid in degrees
-    h1: float
+    h1: np.ndarray
         height above input ellipsoid in meters
     a1: float
         semi-major axis of input ellipsoid
     f1: float
         flattening of input ellipsoid
     a2: float
         semi-major axis of output ellipsoid
@@ -1009,17 +1025,17 @@
         tolerance to prevent division by small numbers and
         to determine convergence
     itmax: int, default 10
         maximum number of iterations to use in Newton-Raphson
 
     Returns
     -------
-    phi2: float
+    phi2: np.ndarray
         latitude of output ellipsoid in degrees
-    h2: float
+    h2: np.ndarray
         height above output ellipsoid in meters
 
     References
     ----------
     .. [1] J Meeus, *Astronomical Algorithms*, pp. 77--82, (1991).
     """
     if (len(phi1) != len(h1)):
@@ -1126,35 +1142,41 @@
                 phi2[N] = np.sign(phi2[N])*90.0
             # calculate height
             h2[N] = (hpr1sin - b2 * np.sin(u2)) / np.sin(phi2r)
 
     # return the latitude and height
     return (phi2, h2)
 
-def compute_delta_h(a1, f1, a2, f2, lat):
+def compute_delta_h(
+        a1: float,
+        f1: float,
+        a2: float,
+        f2: float,
+        lat: np.ndarray
+    ):
     """
     Compute difference in elevation for two ellipsoids at a given
         latitude using a simplified empirical equation
 
     Parameters
     ----------
     a1: float
         semi-major axis of input ellipsoid
     f1: float
         flattening of input ellipsoid
     a2: float
         semi-major axis of output ellipsoid
     f2: float
         flattening of output ellipsoid
-    lat: float
+    lat: np.ndarray
         latitudes (degrees north)
 
     Returns
     -------
-    delta_h: float
+    delta_h: np.ndarray
         difference in elevation for two ellipsoids
 
     References
     ----------
     .. [1] J Meeus, *Astronomical Algorithms*, pp. 77--82, (1991).
     """
     # force phi into range -90 <= phi <= 90
@@ -1168,54 +1190,60 @@
     delta_b = b2 - b1
     # compute differences between ellipsoids
     # delta_h = -(delta_a * cos(phi)^2 + delta_b * sin(phi)^2)
     phi = lat * np.pi/180.0
     delta_h = -(delta_a*np.cos(phi)**2 + delta_b*np.sin(phi)**2)
     return delta_h
 
-def wrap_longitudes(lon):
+def wrap_longitudes(lon: float | np.ndarray):
     """
     Wraps longitudes to range from -180 to +180
 
     Parameters
     ----------
-    lon: float
+    lon: float or np.ndarray
         longitude (degrees east)
     """
     phi = np.arctan2(np.sin(lon*np.pi/180.0), np.cos(lon*np.pi/180.0))
     # convert phi from radians to degrees
     return phi*180.0/np.pi
 
 # get WGS84 parameters
 _wgs84 = constants(ellipsoid='WGS84', units='MKS')
 
-def to_cartesian(lon, lat, h=0.0, a_axis=_wgs84.a_axis, flat=_wgs84.flat):
+def to_cartesian(
+        lon: np.ndarray,
+        lat: np.ndarray,
+        h: float | np.ndarray = 0.0,
+        a_axis: float = _wgs84.a_axis,
+        flat: float = _wgs84.flat
+    ):
     """
     Converts geodetic coordinates to Cartesian coordinates
 
     Parameters
     ----------
-    lon: float
+    lon: np.ndarray
         longitude (degrees east)
-    lat: float
+    lat: np.ndarray
         latitude (degrees north)
-    h: float, default 0.0
+    h: float or np.ndarray, default 0.0
         height above ellipsoid (or sphere)
     a_axis: float, default 6378137.0
         semimajor axis of the ellipsoid
 
         for spherical coordinates set to radius of the Earth
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
 
         for spherical coordinates set to 0
     """
-    # verify axes
-    lon = np.atleast_1d(lon)
-    lat = np.atleast_1d(lat)
+    # verify axes and copy to not modify inputs
+    lon = np.atleast_1d(np.copy(lon))
+    lat = np.atleast_1d(np.copy(lat))
     # fix coordinates to be 0:360
     lon[lon < 0] += 360.0
     # Linear eccentricity and first numerical eccentricity
     lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
     ecc1 = lin_ecc/a_axis
     # convert from geodetic latitude to geocentric latitude
     dtr = np.pi/180.0
@@ -1224,29 +1252,33 @@
     # prime vertical radius of curvature
     N = a_axis/np.sqrt(1.0 - ecc1**2.0*np.sin(latitude_geodetic_rad)**2.0)
     # calculate X, Y and Z from geodetic latitude and longitude
     X = (N + h) * np.cos(latitude_geodetic_rad) * np.cos(lon*dtr)
     Y = (N + h) * np.cos(latitude_geodetic_rad) * np.sin(lon*dtr)
     Z = (N * (1.0 - ecc1**2.0) + h) * np.sin(latitude_geodetic_rad)
     # return the cartesian coordinates
-    return (X,Y,Z)
+    return (X, Y, Z)
 
-def to_sphere(x, y, z):
+def to_sphere(x: np.ndarray, y: np.ndarray, z: np.ndarray):
     """
     Convert from cartesian coordinates to spherical coordinates
 
     Parameters
     ----------
-    x, float
+    x, np.ndarray
         cartesian x-coordinates
-    y, float
+    y, np.ndarray
         cartesian y-coordinates
-    z, float
+    z, np.ndarray
         cartesian z-coordinates
     """
+    # verify axes and copy to not modify inputs
+    x = np.atleast_1d(np.copy(x))
+    y = np.atleast_1d(np.copy(y))
+    z = np.atleast_1d(np.copy(z))
     # calculate radius
     rad = np.sqrt(x**2.0 + y**2.0 + z**2.0)
     # calculate angular coordinates
     # phi: azimuthal angle
     phi = np.arctan2(y,x)
     # th: polar angle
     th = np.arccos(z/rad)
@@ -1255,17 +1287,23 @@
     if np.any(lon < 0):
         lt0 = np.nonzero(lon < 0)
         lon[lt0] += 360.0
     # convert to degrees and fix to -90:90
     lat = 90.0 - (180.0*th/np.pi)
     np.clip(lat, -90, 90, out=lat)
     # return latitude, longitude and radius
-    return (lon,lat,rad)
+    return (lon, lat, rad)
 
-def to_geodetic(x, y, z, a_axis=_wgs84.a_axis, flat=_wgs84.flat):
+def to_geodetic(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = _wgs84.a_axis,
+        flat: float = _wgs84.flat
+    ):
     """
     Convert from cartesian coordinates to geodetic coordinates
     using a closed form solution
 
     Parameters
     ----------
     x, float
@@ -1283,14 +1321,18 @@
     ----------
     .. [1] J Zhu "Exact conversion of Earth-centered, Earth-fixed
         coordinates to geodetic coordinates,"
         *Journal of Guidance, Control, and Dynamics*,
         16(2), 389--391, (1993). `doi: 10.2514/3.21016
         <https://arc.aiaa.org/doi/abs/10.2514/3.21016>`_
     """
+    # verify axes and copy to not modify inputs
+    x = np.atleast_1d(np.copy(x))
+    y = np.atleast_1d(np.copy(y))
+    z = np.atleast_1d(np.copy(z))
     # semiminor axis of the WGS84 ellipsoid [m]
     b_axis = (1.0 - flat)*a_axis
     # Linear eccentricity and first numerical eccentricity
     lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
     ecc1 = lin_ecc/a_axis
     # square of first numerical eccentricity
     e12 = ecc1**2
@@ -1298,54 +1340,61 @@
     dtr = np.pi/180.0
     # calculate distance
     w = np.sqrt(x**2 + y**2)
     # calculate longitude
     lon = np.arctan2(y,x)/dtr
     lat = np.zeros_like(lon)
     h = np.zeros_like(lon)
-    if (w == 0):
+    if np.any(w == 0):
         # special case where w == 0 (exact polar solution)
-        h = np.sign(z)*z - b_axis
-        lat = 90.0*np.sign(z)
+        ind, = np.nonzero(w == 0)
+        h[ind] = np.sign(z[ind])*z[ind] - b_axis
+        lat[ind] = 90.0*np.sign(z[ind])
     else:
         # all other cases
+        ind, = np.nonzero(w != 0)
         l = e12/2.0
-        m = (w/a_axis)**2.0
-        n = ((1.0-e12)*z/b_axis)**2.0
+        m = (w[ind]/a_axis)**2.0
+        n = ((1.0 - e12)*z[ind]/b_axis)**2.0
         i = -(2.0*l**2 + m + n)/2.0
         k = (l**2.0 - m - n)*l**2.0
         q = (1.0/216.0)*(m + n - 4.0*l**2)**3.0 + m*n*l**2.0
         D = np.sqrt((2.0*q - m*n*l**2)*m*n*l**2)
-        B = i/3.0 - (q+D)**(1.0/3.0) - (q-D)**(1.0/3.0)
-        t = np.sqrt(np.sqrt(B**2-k) - (B+i)/2.0)-np.sign(m-n)*np.sqrt((B-i)/2.0)
-        wi = w/(t+l)
-        zi = (1.0-e12)*z/(t-l)
+        B = i/3.0 - (q + D)**(1.0/3.0) - (q - D)**(1.0/3.0)
+        t = np.sqrt(np.sqrt(B**2-k) - (B + i)/2.0) - \
+            np.sign(m - n)*np.sqrt((B - i)/2.0)
+        wi = w/(t + l)
+        zi = (1.0 - e12)*z[ind]/(t - l)
         # calculate latitude and height
-        lat = np.arctan2(zi,((1.0-e12)*wi))/dtr
-        h = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z-zi)**2.0)
+        lat[ind] = np.arctan2(zi, ((1.0 - e12)*wi))/dtr
+        h[ind] = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z[ind]-zi)**2.0)
     # return latitude, longitude and height
-    return (lon,lat,h)
+    return (lon, lat, h)
 
-def scale_areas(lat, flat=_wgs84.flat, ref=70.0):
+def scale_areas(
+        lat: np.ndarray,
+        flat: float=_wgs84.flat,
+        ref: float=70.0
+    ):
     """
     Calculates area scaling factors for a polar stereographic projection
     including special case of at the exact pole
 
     Parameters
     ----------
-    lat: float,
+    lat: np.ndarray
         latitude (degrees north)
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
     ref: float, default 70.0
         reference latitude (true scale latitude)
 
     Returns
     -------
-    scale: float
+    scale: np.ndarray
         area scaling factors at input latitudes
 
     References
     ----------
     .. [1] J P Snyder, *Map Projections used by the U.S. Geological Survey*,
         Geological Survey Bulletin 1532, U.S. Government Printing Office, (1982).
     .. [2] JPL Technical Memorandum 3349-85-101
```

### Comparing `pyTMD-2.0.2/pyTMD/tidal_ellipse.py` & `pyTMD-2.0.3/pyTMD/tidal_ellipse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 u"""
-tidal_ellipse.py (04/2022)
+tidal_ellipse.py (03/2023)
 Expresses the amplitudes and phases for the u and v components in terms of
     four ellipse parameters using Foreman's formula
 
 CALLING SEQUENCE:
     umajor,uminor,uincl,uphase = tidal_ellipse(u,v)
 
 INPUTS:
@@ -20,29 +20,32 @@
 
 REFERENCE:
     M. G. G. Foreman and R. F. Henry, "The harmonic analysis of tidal model time
         series", Advances in Water Resources, 12(3), 109-120, (1989).
         https://doi.org/10.1016/0309-1708(89)90017-1
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 04/2022: updated docstrings to numpy documentation format
     Written 07/2020
 """
+from __future__ import annotations
+
 import numpy as np
 
-def tidal_ellipse(u, v):
+def tidal_ellipse(u: np.ndarray, v: np.ndarray):
     """
     Expresses the amplitudes and phases for the u and v components in terms of
     four ellipse parameters using Foreman's formula
 
     Parameters
     ----------
-    u: float
+    u: np.ndarray
         zonal current (EW)
-    v: float
+    v: np.ndarray
         meridional current (NS)
 
     Returns
     -------
     umajor: float
         amplitude of the semimajor semi-axis
     uminor: float
```

### Comparing `pyTMD-2.0.2/pyTMD/time.py` & `pyTMD-2.0.3/pyTMD/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 u"""
 time.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (03/2023)
 Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: added interpolation for delta time (TT - UT1)
         output variables for some standard epochs used within tide programs
     Updated 11/2022: use IERS https server as default for Bulletin-A files
         added download function for latest Bulletin-A file from IERS
         added function to append from existing merged delta time file
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added encoding for reading leap seconds ascii files
@@ -35,14 +36,16 @@
     Updated 12/2020: merged with convert_julian and convert_calendar_decimal
         added calendar_days routine to get number of days per month
     Updated 09/2020: added wrapper function for merging Bulletin-A files
         can parse date strings in form "time-units since yyyy-mm-dd hh:mm:ss"
     Updated 08/2020: added NASA Earthdata routines for downloading from CDDIS
     Written 07/2020
 """
+from __future__ import annotations
+
 import os
 import re
 import copy
 import logging
 import warnings
 import datetime
 import traceback
@@ -71,15 +74,15 @@
 _unix_epoch = (1970, 1, 1, 0, 0, 0)
 _gps_epoch = (1980, 1, 6, 0, 0, 0)
 _tide_epoch = (1992, 1, 1, 0, 0, 0)
 _j2000_epoch = (2000, 1, 1, 12, 0, 0)
 _atlas_sdp_epoch = (2018, 1, 1, 0, 0, 0)
 
 # PURPOSE: parse a date string into epoch and units scale
-def parse_date_string(date_string):
+def parse_date_string(date_string: str):
     """
     parse a date string of the form
 
     - time-units since ``yyyy-mm-dd hh:mm:ss``
     - ``yyyy-mm-dd hh:mm:ss`` for exact calendar dates
 
     Parameters
@@ -106,15 +109,15 @@
     units,epoch = split_date_string(date_string)
     if units not in _to_sec.keys():
         raise ValueError(f'Invalid units: {units}')
     # return the epoch (as list) and the time unit conversion factors
     return (datetime_to_list(epoch), _to_sec[units])
 
 # PURPOSE: split a date string into units and epoch
-def split_date_string(date_string):
+def split_date_string(date_string: str):
     """
     split a date string into units and epoch
 
     Parameters
     ----------
     date_string: str
         time-units since yyyy-mm-dd hh:mm:ss
@@ -145,21 +148,21 @@
 
 # days per month in a leap and a standard year
 # only difference is February (29 vs. 28)
 _dpm_leap = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 _dpm_stnd = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
 # PURPOSE: gets the number of days per month for a given year
-def calendar_days(year):
+def calendar_days(year: int | float | np.ndarray) -> np.ndarray:
     """
     Calculates the number of days per month for a given year
 
     Parameters
     ----------
-    year: int or float
+    year: int, float or np.ndarray
         calendar year
 
     Returns
     -------
     dpm: list
         number of days for each month
     """
@@ -197,21 +200,26 @@
     delta_time: float
         seconds since epoch
     """
     epoch = datetime.datetime(*epoch)
     return (date - np.datetime64(epoch)) / np.timedelta64(1, 's')
 
 # PURPOSE: convert times from seconds since epoch1 to time since epoch2
-def convert_delta_time(delta_time, epoch1=None, epoch2=None, scale=1.0):
+def convert_delta_time(
+        delta_time: np.ndarray,
+        epoch1: tuple | list | None = None,
+        epoch2: tuple | list | None = None,
+        scale: float = 1.0
+    ):
     """
     Convert delta time from seconds since ``epoch1`` to time since ``epoch2``
 
     Parameters
     ----------
-    delta_time: float
+    delta_time: np.ndarray
         seconds since epoch1
     epoch1: tuple or NoneType, default None
         epoch for input delta_time
     epoch2: tuple or NoneType, default None
         epoch for output delta_time
     scale: float, default 1.0
         scaling factor for converting time to output units
@@ -220,41 +228,49 @@
     epoch2 = datetime.datetime(*epoch2)
     delta_time_epochs = (epoch2 - epoch1).total_seconds()
     # subtract difference in time and rescale to output units
     return scale*(delta_time - delta_time_epochs)
 
 # PURPOSE: calculate the delta time from calendar date
 # http://scienceworld.wolfram.com/astronomy/JulianDate.html
-def convert_calendar_dates(year, month, day, hour=0.0, minute=0.0, second=0.0,
-    epoch=(1992, 1, 1, 0, 0, 0), scale=1.0):
+def convert_calendar_dates(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float = 0.0,
+        minute: np.ndarray | float = 0.0,
+        second: np.ndarray | float = 0.0,
+        epoch: tuple | list = _tide_epoch,
+        scale: float = 1.0
+    ) -> np.ndarray:
     """
     Calculate the time in time units since ``epoch`` from calendar dates
 
     Parameters
     ----------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         month of the year
-    day: float
+    day: np.ndarray
         day of the month
-    hour: float, default 0.0
+    hour: np.ndarray or float, default 0.0
         hour of the day
-    minute: float, default 0.0
+    minute: np.ndarray or float, default 0.0
         minute of the hour
-    second: float, default 0.0
+    second: np.ndarray or float, default 0.0
         second of the minute
-    epoch: tuple, default pyTMD.time._tide_epoch
+    epoch: tuple or list, default pyTMD.time._tide_epoch
         epoch for output delta_time
     scale: float, default 1.0
         scaling factor for converting time to output units
 
     Returns
     -------
-    delta_time: float
+    delta_time: np.ndarray
         days since epoch
     """
     # calculate date in Modified Julian Days (MJD) from calendar date
     # MJD: days since November 17, 1858 (1858-11-17T00:00:00)
     MJD = 367.0*year - np.floor(7.0*(year + np.floor((month+9.0)/12.0))/4.0) - \
         np.floor(3.0*(np.floor((year + (month - 9.0)/7.0)/100.0) + 1.0)/4.0) + \
         np.floor(275.0*month/9.0) + day + hour/24.0 + minute/1440.0 + \
@@ -262,40 +278,47 @@
     epoch1 = datetime.datetime(*_mjd_epoch)
     epoch2 = datetime.datetime(*epoch)
     delta_time_epochs = (epoch2 - epoch1).total_seconds()
     # return the date in days since epoch
     return scale*np.array(MJD - delta_time_epochs/86400.0, dtype=np.float64)
 
 # PURPOSE: Converts from calendar dates into decimal years
-def convert_calendar_decimal(year, month, day=None, hour=None, minute=None,
-    second=None, DofY=None):
+def convert_calendar_decimal(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float | None = None,
+        minute: np.ndarray | float | None = None,
+        second: np.ndarray | float | None = None,
+        DofY: np.ndarray | float | None = None,
+    ) -> np.ndarray:
     """
     Converts from calendar date into decimal years taking into
     account leap years
 
     Parameters
     ----------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         calendar month
-    day: float or NoneType, default None
+    day: np.ndarray, float or NoneType, default None
         day of the month
-    hour: float or NoneType, default None
+    hour: np.ndarray, float or NoneType, default None
         hour of the day
-    minute: float or NoneType, default None
+    minute: np.ndarray, float or NoneType, default None
         minute of the hour
-    second: float or NoneType, default None
+    second: np.ndarray, float or NoneType, default None
         second of the minute
-    DofY: float or NoneType, default None
+    DofY: np.ndarray, float or NoneType, default None
         day of the year (January 1 = 1)
 
     Returns
     -------
-    t_date: float
+    t_date: np.ndarray
         date in decimal-year format
 
     References
     ----------
     .. [1] N. Dershowitz, and E. M. Reingold.
         *Calendrical Calculations*,
         Cambridge: Cambridge University Press, (2008).
@@ -411,44 +434,44 @@
         (cal_date['DofY'][stnd] + cal_date['hour'][stnd]/24. + \
         cal_date['minute'][stnd]/1440. + \
         cal_date['second'][stnd]/86400.)/np.sum(dpm_stnd)
 
     return t_date
 
 # PURPOSE: Converts from Julian day to calendar date and time
-def convert_julian(JD, **kwargs):
+def convert_julian(JD: np.ndarray, **kwargs):
     """
     Converts from Julian day to calendar date and time
 
     Parameters
     ----------
-    JD: float
+    JD: np.ndarray
         Julian Day (days since 01-01-4713 BCE at 12:00:00)
     astype: str or NoneType, default None
         convert output to variable type
     format: str, default 'dict'
         format of output variables
 
             - ``'dict'``: dictionary with variable keys
             - ``'tuple'``: tuple in most-to-least-significant order
             - ``'zip'``: aggregated variable sets
 
     Returns
     -------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         calendar month
-    day: float
+    day: np.ndarray
         day of the month
-    hour: float
+    hour: np.ndarray
         hour of the day
-    minute: float
+    minute: np.ndarray
         minute of the hour
-    second: float
+    second: np.ndarray
         second of the minute
 
     References
     ----------
     .. [1] W. H. Press, *Numerical Recipes in C*,
         Brian P. Flannery, Saul A. Teukolsky, and William T. Vetterling.
         Cambridge University Press, (1988).
@@ -524,15 +547,15 @@
     elif (kwargs['format'] == 'tuple'):
         return (year, month, day, hour, minute, second)
     elif (kwargs['format'] == 'zip'):
         return zip(year, month, day, hour, minute, second)
 
 # PURPOSE: calculate the difference between universal time and dynamical time
 # by interpolating a delta time file to a given date
-def interpolate_delta_time(delta_file, idays):
+def interpolate_delta_time(delta_file: str, idays: np.ndarray):
     """
     Calculates the difference between universal time (UT) and
     dynamical time (TT)
 
     Parameters
     ----------
     delta_file: str
@@ -556,21 +579,24 @@
         epoch=_tide_epoch)
     # use scipy interpolating splines to interpolate delta times
     spl = scipy.interpolate.UnivariateSpline(days,dinput[:,3],k=1,s=0,ext=0)
     # return the delta time for the input date converted to days
     return spl(idays)/86400.0
 
 # PURPOSE: Count number of leap seconds that have passed for each GPS time
-def count_leap_seconds(GPS_Time, truncate=True):
+def count_leap_seconds(
+        GPS_Time: np.ndarray | float,
+        truncate: bool = True
+    ):
     """
     Counts the number of leap seconds between a given GPS time and UTC
 
     Parameters
     ----------
-    GPS_Time: float
+    GPS_Time: np.ndarray or float
         seconds since January 6, 1980 at 00:00:00
     truncate: bool, default True
         Reduce list of leap seconds to positive GPS times
 
     Returns
     -------
     n_leaps: float
@@ -585,15 +611,15 @@
         if (count > 0):
             indices = np.nonzero(GPS_Time >= leap)
             n_leaps[indices] += 1.0
     # return the number of leap seconds for converting to UTC
     return n_leaps
 
 # PURPOSE: Define GPS leap seconds
-def get_leap_seconds(truncate=True):
+def get_leap_seconds(truncate: bool = True):
     """
     Gets a list of GPS times for when leap seconds occurred
 
     Parameters
     ----------
     truncate: bool, default True
         Reduce list of leap seconds to positive GPS times
@@ -623,28 +649,32 @@
     # return the GPS times of leap second occurance
     if truncate:
         return leap_GPS[leap_GPS >= 0].astype(np.float64)
     else:
         return leap_GPS.astype(np.float64)
 
 # PURPOSE: connects to servers and downloads leap second files
-def update_leap_seconds(timeout=20, verbose=False, mode=0o775):
+def update_leap_seconds(
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to servers to download leap-seconds.list files from NIST servers
 
     - https://www.nist.gov/pml/time-and-frequency-division/leap-seconds-faqs
 
     Servers and Mirrors
 
     - ftp://ftp.nist.gov/pub/time/leap-seconds.list
     - https://www.ietf.org/timezones/data/leap-seconds.list
 
     Parameters
     ----------
-    timeout: int, default 20
+    timeout: int or None, default 20
         timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
     # local version of file
@@ -672,15 +702,20 @@
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
 # PURPOSE: Download delta time files and merge into a single
-def merge_delta_time(username=None, password=None, verbose=False, mode=0o775):
+def merge_delta_time(
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to servers to download historic_deltat.data and deltat.data files
 
     Reads IERS Bulletin-A produced iers_deltat.data files
 
     Creates a merged file combining the historic, monthly and daily files
 
@@ -748,15 +783,15 @@
         args = (daily[i,0],daily[i,1],daily[i,2],daily[i,3])
         print(file_format.format(*args),file=fid)
     # close the merged file and change the permissions mode
     fid.close()
     os.chmod(merged_file,mode)
 
 # PURPOSE: Append Bulletin-A file to merged delta time file
-def append_delta_time(verbose=False, mode=0o775):
+def append_delta_time(verbose: bool = False, mode: oct = 0o775):
     """
     Appends merged delta time file with values from latest Bulletin-A file
 
     Parameters
     ----------
     verbose: bool, default False
         print file information about output file
@@ -782,16 +817,20 @@
     for Y,M,D,T in zip(YY,MM,DD,DELTAT):
         print(file_format.format(Y,M,D,T), file=fid)
     # close the merged file and change the permissions mode
     fid.close()
     os.chmod(merged_file,mode)
 
 # PURPOSE: connect to IERS or CDDIS server and merge Bulletin-A files
-def merge_bulletin_a_files(username=None,password=None,
-    verbose=False,mode=0o775):
+def merge_bulletin_a_files(
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Attempt to connects to the IERS server and the CDDIS Earthdata server
     to download and merge Bulletin-A files
 
     Reads the IERS Bulletin-A files and calculates the daily delta times
 
     Servers and Mirrors
@@ -849,15 +888,20 @@
         os.remove(COPY) if os.access(COPY, os.F_OK) else None
         pass
     else:
         pyTMD.utilities.copy(COPY, LOCAL, move=True)
         return
 
 # PURPOSE: connects to IERS ftp servers and finds Bulletin-A files
-def iers_ftp_delta_time(daily_file, timeout=120, verbose=False, mode=0o775):
+def iers_ftp_delta_time(
+        daily_file: str,
+        timeout: int | None = 120,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to the IERS ftp server to download Bulletin-A files
 
     - https://datacenter.iers.org/productMetadata.php?id=6
 
     Reads the IERS Bulletin-A files and calculates the daily delta times
 
@@ -918,15 +962,20 @@
         HOST.remove(SUB)
     # close the output file
     fid.close()
     # change the permissions mode
     os.chmod(daily_file,mode)
 
 # PURPOSE: connects to IERS http servers and finds Bulletin-A files
-def iers_delta_time(daily_file, timeout=120, verbose=False, mode=0o775):
+def iers_delta_time(
+        daily_file: str,
+        timeout: int | None = 120,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to the IERS server to download Bulletin-A files
 
     - https://datacenter.iers.org/productMetadata.php?id=6
 
     Reads the IERS Bulletin-A files and calculates the daily delta times
 
@@ -969,16 +1018,21 @@
         remote_buffer.close()
     # close the output file
     fid.close()
     # change the permissions mode
     os.chmod(daily_file, mode)
 
 # PURPOSE: connects to CDDIS Earthdata https server and finds Bulletin-A files
-def cddis_delta_time(daily_file, username=None, password=None,
-    verbose=False, mode=0o775):
+def cddis_delta_time(
+        daily_file: str,
+        username: str | None = None,
+        password: str | None = None,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to the CDDIS Earthdata server to download Bulletin-A files
 
     Reads the IERS Bulletin-A files and calculates the daily delta times
 
     Servers and Mirrors
 
@@ -1136,28 +1190,32 @@
     # (TT-TAI) + (TAI-GPS) + (GPS-UTC) - (UT1-UTC)
     DELTAT = TT_TAI + TAI_GPS + GPS_UTC - UT1_UTC[:valid]
 
     # return dates and delta times
     return (Y,M,D,DELTAT)
 
 # PURPOSE: connects to servers and downloads latest Bulletin-A file
-def update_bulletin_a(timeout=20, verbose=False, mode=0o775):
+def update_bulletin_a(
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to IERS Rapid Service/Prediction Center (RS/PC) and
     downloads latest Bulletin-A file
 
     - https://maia.usno.navy.mil/ser7/readme.bulla
 
     Servers and Mirrors
 
     - https://maia.usno.navy.mil/ser7/ser7.dat
 
     Parameters
     ----------
-    timeout: int, default 20
+    timeout: int or NoneType, default 20
         timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
     # local version of file
@@ -1172,15 +1230,22 @@
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
 # PURPOSE: connects to servers and downloads delta time files
-def pull_deltat_file(FILE,username=None,password=None,verbose=False,mode=0o775):
+def pull_deltat_file(
+        FILE: str,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to servers and downloads delta time files
 
     Servers and Mirrors
 
     - http://maia.usno.navy.mil/ser7/
     - https://cddis.nasa.gov/archive/products/iers/
@@ -1194,14 +1259,16 @@
 
             - deltat.data: monthly deltat file
             - historic_deltat.data: historic deltat file
     username: str or NoneType, default None
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
+    timeout: int or NoneType, default 20
+        timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
 
     Notes
     -----
@@ -1210,16 +1277,20 @@
     # local version of file
     LOCAL = pyTMD.utilities.get_data_path(['data',FILE])
     HASH = pyTMD.utilities.get_hash(LOCAL)
 
     # try downloading from US Naval Oceanography Portal
     HOST = ['http://maia.usno.navy.mil','ser7',FILE]
     try:
-        pyTMD.utilities.from_http(HOST,timeout=5,local=LOCAL,hash=HASH,
-            verbose=verbose,mode=mode)
+        pyTMD.utilities.from_http(HOST,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
     # try downloading from NASA Crustal Dynamics Data Information System
@@ -1227,26 +1298,36 @@
     # requires using the following https Earthdata server
     server = []
     # server.append(['cddis.nasa.gov','pub','products','iers',FILE])
     # server.append(['cddis.gsfc.nasa.gov','products','iers',FILE])
     for HOST in server:
         try:
             pyTMD.utilities.check_ftp_connection(HOST[0])
-            pyTMD.utilities.from_ftp(HOST,timeout=20,local=LOCAL,hash=HASH,
-                verbose=verbose,mode=mode)
+            pyTMD.utilities.from_ftp(HOST,
+                timeout=timeout,
+                local=LOCAL,
+                hash=HASH,
+                verbose=verbose,
+                mode=mode)
         except Exception as exc:
             logging.debug(traceback.format_exc())
             pass
         else:
             return
 
     # try downloading from NASA Crustal Dynamics Data Information System
     # using NASA Earthdata credentials stored in netrc file
     HOST = ['https://cddis.nasa.gov','archive','products','iers',FILE]
     try:
-        pyTMD.utilities.from_cddis(HOST,username=username,password=password,
-            timeout=20,local=LOCAL,hash=HASH,verbose=verbose,mode=mode)
+        pyTMD.utilities.from_cddis(HOST,
+            username=username,
+            password=password,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
```

### Comparing `pyTMD-2.0.2/pyTMD/tools.py` & `pyTMD-2.0.3/pyTMD/tools.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/pyTMD/utilities.py` & `pyTMD-2.0.3/pyTMD/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (01/2023)
+Written by Tyler Sutterley (03/2023)
 Download and management utilities for syncing time and auxiliary files
 
 PYTHON DEPENDENCIES:
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 UPDATE HISTORY:
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 01/2023: updated SSL context to fix some deprecation warnings
     Updated 11/2022: added list program for IERS Bulletin-A https server
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: build python logging instance for handling verbose output
     Updated 09/2021: added generic list from Apache http server
     Updated 08/2021: added function to open a file path
@@ -26,15 +27,15 @@
         make context an optional keyword argument in from_http
     Updated 09/2020: copy from http and https to bytesIO object in chunks
         use netrc credentials if not entered from CDDIS functions
         generalize build opener function for different Earthdata instances
     Updated 08/2020: add GSFC CDDIS opener, login and download functions
     Written 08/2020
 """
-from __future__ import print_function, division
+from __future__ import print_function, division, annotations
 
 import sys
 import os
 import re
 import io
 import ssl
 import netrc
@@ -57,34 +58,34 @@
     import urllib2
 else:
     from urllib.parse import quote_plus
     from http.cookiejar import CookieJar
     import urllib.request as urllib2
 
 # PURPOSE: get absolute path within a package from a relative path
-def get_data_path(relpath):
+def get_data_path(relpath: list | str):
     """
     Get the absolute path within a package from a relative path
 
     Parameters
     ----------
-    relpath: str,
+    relpath: list or str
         relative path
     """
     # current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
     filepath = os.path.dirname(os.path.abspath(filename))
-    if isinstance(relpath,list):
+    if isinstance(relpath, list):
         # use *splat operator to extract from list
         return os.path.join(filepath,*relpath)
-    elif isinstance(relpath,str):
+    elif isinstance(relpath, str):
         return os.path.join(filepath,relpath)
 
 # PURPOSE: platform independent file opener
-def file_opener(filename):
+def file_opener(filename: str):
     """
     Platform independent file opener
 
     Parameters
     ----------
     filename: str
         path to file
@@ -93,15 +94,18 @@
         os.startfile(os.path.expanduser(filename), "explore")
     elif (sys.platform == "darwin"):
         subprocess.call(["open", os.path.expanduser(filename)])
     else:
         subprocess.call(["xdg-open", os.path.expanduser(filename)])
 
 # PURPOSE: get the hash value of a file
-def get_hash(local, algorithm='MD5'):
+def get_hash(
+        local: str | io.IOBase,
+        algorithm: str = 'MD5'
+    ):
     """
     Get the hash value from a local file or ``BytesIO`` object
 
     Parameters
     ----------
     local: obj or str
         BytesIO object or path to file
@@ -126,15 +130,18 @@
                 return hashlib.md5(local_buffer.read()).hexdigest()
             elif (algorithm == 'sha1'):
                 return hashlib.sha1(local_buffer.read()).hexdigest()
     else:
         return ''
 
 # PURPOSE: get the git hash value
-def get_git_revision_hash(refname='HEAD', short=False):
+def get_git_revision_hash(
+        refname: str = 'HEAD',
+        short: bool = False
+    ):
     """
     Get the ``git`` hash value for a particular reference
 
     Parameters
     ----------
     refname: str, default HEAD
         Symbolic reference name
@@ -163,15 +170,15 @@
     gitpath = os.path.join(basepath,'.git')
     # build command
     cmd = ['git', f'--git-dir={gitpath}', 'status', '--porcelain']
     with warnings.catch_warnings():
         return bool(subprocess.check_output(cmd))
 
 # PURPOSE: recursively split a url path
-def url_split(s):
+def url_split(s: str):
     """
     Recursively split a url path into a list
 
     Parameters
     ----------
     s: str
         url string
@@ -196,15 +203,15 @@
     # remove commented lines and after argument comments
     for arg in re.sub(r'\#(.*?)$',r'',arg_line).split():
         if not arg.strip():
             continue
         yield arg
 
 # PURPOSE: build a logging instance with a specified name
-def build_logger(name, **kwargs):
+def build_logger(name: str, **kwargs):
     """
     Builds a logging instance with the specified name
 
     Parameters
     ----------
     name: str
         name of the logger
@@ -233,15 +240,15 @@
         formatter = logging.Formatter(kwargs['format'])
         handler.setFormatter(formatter)
         # add handler to logger
         logger.addHandler(handler)
     return logger
 
 # PURPOSE: convert Roman numerals to (Arabic) integers
-def roman_to_int(roman):
+def roman_to_int(roman: str):
     """
     Converts a string from Roman numerals into an integer (Arabic)
 
     Parameters
     ----------
     roman: str
         Roman numeral string
@@ -257,15 +264,18 @@
             output += roman_map[s] - 2*roman_map[roman[i-1]]
         else:
             output += roman_map[s]
     # return the integer value
     return output
 
 # PURPOSE: returns the Unix timestamp value for a formatted date string
-def get_unix_time(time_string, format='%Y-%m-%d %H:%M:%S'):
+def get_unix_time(
+        time_string: str,
+        format: str = '%Y-%m-%d %H:%M:%S'
+    ):
     """
     Get the Unix timestamp value for a formatted date string
 
     Parameters
     ----------
     time_string: str
         formatted time string to parse
@@ -283,15 +293,15 @@
         parsed_time = dateutil.parser.parse(time_string.rstrip())
     except (TypeError, ValueError):
         return None
     else:
         return parsed_time.timestamp()
 
 # PURPOSE: output a time string in isoformat
-def isoformat(time_string):
+def isoformat(time_string: str):
     """
     Reformat a date string to ISO formatting
 
     Parameters
     ----------
     time_string: str
         formatted time string to parse
@@ -301,39 +311,44 @@
         parsed_time = dateutil.parser.parse(time_string.rstrip())
     except (TypeError, ValueError):
         return None
     else:
         return parsed_time.isoformat()
 
 # PURPOSE: rounds a number to an even number less than or equal to original
-def even(value):
+def even(value: float):
     """
     Rounds a number to an even number less than or equal to original
 
     Parameters
     ----------
     value: float
         number to be rounded
     """
     return 2*int(value//2)
 
 # PURPOSE: rounds a number upward to its nearest integer
-def ceil(value):
+def ceil(value: float):
     """
     Rounds a number upward to its nearest integer
 
     Parameters
     ----------
     value: float
         number to be rounded upward
     """
     return -int(-value//1)
 
 # PURPOSE: make a copy of a file with all system information
-def copy(source, destination, move=False, **kwargs):
+def copy(
+        source: str,
+        destination: str,
+        move: bool = False,
+        **kwargs
+    ):
     """
     Copy or move a file with all system information
 
     Parameters
     ----------
     source: str
         source file
@@ -348,15 +363,19 @@
     logging.info(f'{source} -->\n\t{destination}')
     shutil.copyfile(source, destination)
     shutil.copystat(source, destination)
     if move:
         os.remove(source)
 
 # PURPOSE: check ftp connection
-def check_ftp_connection(HOST, username=None, password=None):
+def check_ftp_connection(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None
+    ):
     """
     Check internet connection with ftp host
 
     Parameters
     ----------
     HOST: str
         remote ftp host
@@ -374,16 +393,23 @@
         raise RuntimeError('Check internet connection')
     except ftplib.error_perm:
         raise RuntimeError('Check login credentials')
     else:
         return True
 
 # PURPOSE: list a directory on a ftp host
-def ftp_list(HOST, username=None, password=None, timeout=None,
-    basename=False, pattern=None, sort=False):
+def ftp_list(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = None,
+        basename: bool = False,
+        pattern: str | None = None,
+        sort: bool = False
+    ):
     """
     List a directory on a ftp host
 
     Parameters
     ----------
     HOST: str or list
         remote ftp host path split as list
@@ -449,17 +475,26 @@
             mtimes = [mtimes[indice] for indice in i]
         # close the ftp connection
         ftp.close()
         # return the list of items and last modified times
         return (output, mtimes)
 
 # PURPOSE: download a file from a ftp host
-def from_ftp(HOST, username=None, password=None, timeout=None,
-    local=None, hash='', chunk=8192, verbose=False, fid=sys.stdout,
-    mode=0o775):
+def from_ftp(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = None,
+        local: str | None = None,
+        hash: str = '',
+        chunk: int = 8192,
+        verbose: bool = False,
+        fid=sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from a ftp host
 
     Parameters
     ----------
     HOST: str or list
         remote ftp host path
@@ -539,15 +574,15 @@
         remote_buffer.seek(0)
         return remote_buffer
 
 # default ssl context
 _default_ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
 
 # PURPOSE: check internet connection
-def check_connection(HOST, context=_default_ssl_context):
+def check_connection(HOST: str, context=_default_ssl_context):
     """
     Check internet connection with http host
 
     Parameters
     ----------
     HOST: str
         remote http host
@@ -559,17 +594,23 @@
         urllib2.urlopen(HOST, timeout=20, context=context)
     except urllib2.URLError as exc:
         raise RuntimeError('Check internet connection') from exc
     else:
         return True
 
 # PURPOSE: list a directory on an Apache http Server
-def http_list(HOST, timeout=None, context=_default_ssl_context,
-    parser=lxml.etree.HTMLParser(), format='%Y-%m-%d %H:%M',
-    pattern='', sort=False):
+def http_list(
+        HOST: str,
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        parser = lxml.etree.HTMLParser(),
+        format: str = '%Y-%m-%d %H:%M',
+        pattern: str = '',
+        sort: bool = False
+    ):
     """
     List a directory on an Apache http Server
 
     Parameters
     ----------
     HOST: str or list
         remote http host path
@@ -622,30 +663,36 @@
             # sort list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a http host
-def from_http(HOST, timeout=None, context=_default_ssl_context,
-    local=None, hash='', chunk=16384, verbose=False, fid=sys.stdout,
-    mode=0o775):
+def from_http(
+        HOST: str,
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        local: str | None = None,
+        hash: str = '',
+        chunk: int = 16384,
+        verbose: bool = False,
+        fid = sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from a http host
 
     Parameters
     ----------
     HOST: str or list
         remote http host path split as list
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
     context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
         SSL context for ``urllib`` opener object
-    timeout: int or NoneType, default None
-        timeout in seconds for blocking operations
     local: str or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
@@ -699,17 +746,24 @@
             # change the permissions mode
             os.chmod(local,mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: "login" to NASA Earthdata with supplied credentials
-def build_opener(username, password, context=_default_ssl_context,
-    password_manager=True, get_ca_certs=True, redirect=True,
-    authorization_header=False, urs='https://urs.earthdata.nasa.gov'):
+def build_opener(
+        username: str,
+        password: str,
+        context=_default_ssl_context,
+        password_manager: bool = True,
+        get_ca_certs: bool = True,
+        redirect: bool = True,
+        authorization_header: bool = False,
+        urs: str = 'https://urs.earthdata.nasa.gov'
+    ):
     """
     Build ``urllib`` opener for NASA Earthdata with supplied credentials
 
     Parameters
     ----------
     username: str or NoneType, default None
         NASA Earthdata username
@@ -775,17 +829,24 @@
         raise RuntimeError('Check your NASA Earthdata credentials')
     except urllib2.URLError:
         raise RuntimeError('Check internet connection')
     else:
         return True
 
 # PURPOSE: list a directory on GSFC CDDIS https server
-def cddis_list(HOST, username=None, password=None, build=True,
-    timeout=None, parser=lxml.etree.HTMLParser(), pattern='',
-    sort=False):
+def cddis_list(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        timeout: int | None = None,
+        parser=lxml.etree.HTMLParser(),
+        pattern: str = '',
+        sort: bool = False
+    ):
     """
     List a directory on GSFC CDDIS archive server
 
     Parameters
     ----------
     HOST: str or list
         remote https host
@@ -857,17 +918,27 @@
             # sort list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a GSFC CDDIS https server
-def from_cddis(HOST, username=None, password=None, build=True,
-    timeout=None, local=None, hash='', chunk=16384, verbose=False,
-    fid=sys.stdout, mode=0o775):
+def from_cddis(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        timeout: int | None = None,
+        local: str | None = None,
+        hash: str = '',
+        chunk: int = 16384,
+        verbose: bool = False,
+        fid=sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from GSFC CDDIS archive server
 
     Parameters
     ----------
     HOST: str or list
         remote https host
@@ -950,16 +1021,20 @@
             # change the permissions mode
             os.chmod(local,mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: list a directory on IERS https Server
-def iers_list(HOST, timeout=None, context=_default_ssl_context,
-    parser=lxml.etree.HTMLParser()):
+def iers_list(
+        HOST: str,
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        parser = lxml.etree.HTMLParser()
+    ):
     """
     List a directory on IERS Bulletin-A https server
 
     Parameters
     ----------
     HOST: str or list
         remote http host path
```

### Comparing `pyTMD-2.0.2/pyTMD.egg-info/PKG-INFO` & `pyTMD-2.0.3/pyTMD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.2
+Version: 2.0.3
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -57,26 +57,29 @@
 
 .. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
    :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/pyTMD/main?urlpath=lab
 
 .. |zenodo| image:: https://zenodo.org/badge/107997403.svg
    :target: https://zenodo.org/badge/latestdoi/107997403
 
-Python-based tidal prediction software that reads OTIS, GOT and FES formatted tidal solutions for calculating ocean and load tides
+
+Python-based tidal prediction software for estimating ocean, load, solid Earth and pole tides
+
+Ocean and load tidal predictions using OTIS, GOT and FES formatted tidal solutions
 
 - `OSU Tidal Prediction Software (OTPS) <https://www.tpxo.net/otps>`_
 - `ESR Tide Model Driver (TMD) Matlab Toolbox <https://www.esr.org/research/polar-tide-models/tmd-software/>`_
 - `OSU Global and Regional Tide Models <https://www.tpxo.net>`_
 - `ESR Polar Tide Models <https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/>`_
 - `A Global Ocean Tide Model From TOPEX/POSEIDON Altimetry: GOT99.2 <https://ntrs.nasa.gov/citations/19990089548>`_
 - `Finite Element Solution (FES) tide models <https://www.aviso.altimetry.fr/en/data/products/auxiliary-products/global-tide-fes.html>`_
 - `Delta times from US Naval Observatory (USNO) Earth Orientation Products <http://maia.usno.navy.mil/ser7/deltat.data>`_
 - `Delta times from NASA Crustal Dynamics Data Information System (CDDIS) <ftp://cddis.nasa.gov/products/iers/deltat.data>`_
 
-Pole tide prediction software for calculating radial pole tide displacements
+Radial solid Earth and pole tide displacements following IERS conventions
 
 - `IERS Conventions (2010) <http://iers-conventions.obspm.fr/>`_
 - `IERS Mean Pole Location <https://hpiers.obspm.fr/iers/eop/eopc01/mean-pole.tab>`_
 - `IERS Pole Coordinates to Calculate Mean Pole <https://hpiers.obspm.fr/iers/eop/eopc01/eopc01.1900-now.dat>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from USNO <http://www.usno.navy.mil/USNO/earth-orientation/eo-products/weekly>`_
 - `IERS Daily Earth Orientation Parameters (EOP) from NASA CDDIS <ftp://cddis.nasa.gov/products/iers/finals.all>`_
 - `IERS Ocean Pole Load Tide Coefficients Map <http://maia.usno.navy.mil/conventions/2010/2010_update/chapter7/additional_info/opoleloadcoefcmcor.txt.gz>`_
```

### Comparing `pyTMD-2.0.2/pyTMD.egg-info/SOURCES.txt` & `pyTMD-2.0.3/pyTMD.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 README.rst
 postBuild
 requirements-dev.txt
 requirements.txt
 setup.py
 version.txt
 pyTMD/__init__.py
+pyTMD/astro.py
 pyTMD/calc_astrol_longitudes.py
 pyTMD/check_tide_points.py
 pyTMD/compute_tide_corrections.py
 pyTMD/constants.py
+pyTMD/convert_crs.py
 pyTMD/convert_ll_xy.py
 pyTMD/eop.py
 pyTMD/interpolate.py
 pyTMD/load_constituent.py
 pyTMD/load_nodal_corrections.py
 pyTMD/predict.py
 pyTMD/spatial.py
@@ -49,12 +51,13 @@
 pyTMD/io/model.py
 pyTMD/io/ocean_pole_tide.py
 scripts/arcticdata_tides.py
 scripts/aviso_fes_tides.py
 scripts/compute_LPET_elevations.py
 scripts/compute_LPT_displacements.py
 scripts/compute_OPT_displacements.py
+scripts/compute_SET_displacements.py
 scripts/compute_tidal_currents.py
 scripts/compute_tidal_elevations.py
 scripts/reduce_OTIS_files.py
 scripts/usap_cats_tides.py
 scripts/verify_box_tpxo.py
```

### Comparing `pyTMD-2.0.2/scripts/arcticdata_tides.py` & `pyTMD-2.0.3/scripts/arcticdata_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/scripts/aviso_fes_tides.py` & `pyTMD-2.0.3/scripts/aviso_fes_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/scripts/compute_LPET_elevations.py` & `pyTMD-2.0.3/scripts/compute_LPET_elevations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_LPET_elevations.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (04/2023)
 Calculates long-period equilibrium tidal elevations for an input file
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
     netCDF4 file with variables for spatial and temporal coordinates
     geotiff file with bands in spatial coordinates
@@ -20,14 +20,15 @@
         for csv files: the order of the columns within the file
         for HDF5 and netCDF4 files: time, y, x and data variable names
     -H X, --header X: number of header lines for csv files
     --delimiter X: Delimiter for csv or ascii files
     -t X, --type X: input data type
         drift: drift buoys or satellite/airborne altimetry (time per data point)
         grid: spatial grids or images (single time for all data points)
+        time series: time series at a single point
     -e X, --epoch X: Reference epoch of input time (default Modified Julian Day)
         days since 1858-11-17T00:00:00
     -d X, --deltatime X: Input delta time for files without date information
         can be set to 0 to use exact calendar date from epoch
     -s X, --standard X: Input time standard for delta times or input time type
         UTC: Coordinate Universal Time
         GPS: GPS Time
@@ -59,14 +60,15 @@
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial.py: utilities for reading and writing spatial data
     utilities.py: download and management utilities for syncing files
     predict.py: calculates long-period equilibrium ocean tides
 
 UPDATE HISTORY:
+    Updated 04/2023: check if datetime before converting to seconds
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added delimiter option and datetime parsing for ascii files
@@ -209,15 +211,16 @@
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
     # convert time to seconds
-    delta_time = to_secs*dinput['time'].flatten()
+    if (TIME_STANDARD.lower() != 'datetime'):
+        delta_time = to_secs*dinput['time'].flatten()
 
     # calculate leap seconds if specified
     if (TIME_STANDARD.upper() == 'GPS'):
         GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
         GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
@@ -244,15 +247,15 @@
             pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
     else:
         leap_seconds = 0.0
 
     if (TIME_STANDARD.lower() == 'datetime'):
         # convert delta time array from datetime object
         # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(delta_time,
+        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
             epoch=pyTMD.time._tide_epoch)/86400.0
     else:
         # convert time from units to days since 1992-01-01T00:00:00 (UTC)
         tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
             epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
 
     # interpolate delta times from calendar dates to tide time
```

### Comparing `pyTMD-2.0.2/scripts/compute_LPT_displacements.py` & `pyTMD-2.0.3/scripts/compute_LPT_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 u"""
 compute_LPT_displacements.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (04/2023)
 Calculates radial load pole tide displacements for an input file
     following IERS Convention (2010) guidelines
-    http://maia.usno.navy.mil/conventions/2010officialinfo.php
-    http://maia.usno.navy.mil/conventions/chapter7.php
-    https://iers-conventions.obspm.fr/content/chapter7/icc7.pdf
+    https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
     netCDF4 file with variables for spatial and temporal coordinates
     geotiff file with bands in spatial coordinates
 
@@ -24,26 +22,33 @@
         for csv files: the order of the columns within the file
         for HDF5 and netCDF4 files: time, y, x and data variable names
     -H X, --header X: number of header lines for csv files
     --delimiter X: Delimiter for csv or ascii files
     -t X, --type X: input data type
         drift: drift buoys or satellite/airborne altimetry (time per data point)
         grid: spatial grids or images (single time for all data points)
+        time series: time series at a single point
     -e X, --epoch X: Reference epoch of input time (default Modified Julian Day)
         days since 1858-11-17T00:00:00
     -d X, --deltatime X: Input delta time for files without date information
         can be set to 0 to use exact calendar date from epoch
     -s X, --standard X: Input time standard for delta times or input time type
         UTC: Coordinate Universal Time
         GPS: GPS Time
         LORAN: Long Range Navigator Time
         TAI: International Atomic Time
         datetime: formatted datetime string in UTC
+    -c X, --convention X: IERS mean or secular pole convention
+        2003
+        2010
+        2015
+        2018
     -P X, --projection X: spatial projection as EPSG code or PROJ4 string
         4326: latitude and longitude coordinates on WGS84 reference ellipsoid
+    -E X, --ellipsoid X: Ellipsoid for calculating load pole tide parameters
     -V, --verbose: Verbose output of processing run
     -M X, --mode X: Permission mode of output file
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -57,20 +62,23 @@
         https://pypi.python.org/pypi/GDAL
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
+    constants.py: gravitational and ellipsoidal parameters
+    eop.py: utilities for calculating Earth Orientation Parameters (EOP)
+    spatial: utilities for reading, writing and operating on spatial data
     time.py: utilities for calculating time operations
-    spatial.py: utilities for reading and writing spatial data
     utilities.py: download and management utilities for syncing files
-    eop.py: utilities for calculating Earth Orientation Parameters (EOP)
 
 UPDATE HISTORY:
+    Updated 04/2023: check if datetime before converting to seconds
+    Updated 03/2023: added option for changing the IERS mean pole convention
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
         use constants class for ellipsoidal parameters
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
@@ -145,14 +153,15 @@
     DELIMITER=',',
     TYPE='drift',
     TIME_UNITS='days since 1858-11-17T00:00:00',
     TIME=None,
     TIME_STANDARD='UTC',
     PROJECTION='4326',
     ELLIPSOID='WGS84',
+    CONVENTION='2018',
     VERBOSE=False,
     MODE=0o775):
 
     # create logger for verbosity level
     loglevel = logging.INFO if VERBOSE else logging.CRITICAL
     logging.basicConfig(level=loglevel)
 
@@ -224,15 +233,16 @@
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
     # convert time to seconds
-    delta_time = to_secs*dinput['time'].flatten()
+    if (TIME_STANDARD.lower() != 'datetime'):
+        delta_time = to_secs*dinput['time'].flatten()
 
     # calculate leap seconds if specified
     if (TIME_STANDARD.upper() == 'GPS'):
         GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
         GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
@@ -259,29 +269,29 @@
             pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
     else:
         leap_seconds = 0.0
 
     if (TIME_STANDARD.lower() == 'datetime'):
         # convert delta time array from datetime object
         # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(delta_time,
+        MJD = pyTMD.time.convert_datetime(dinput['time'].flatten(),
             epoch=pyTMD.time._mjd_epoch)/86400.0
     else:
         # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
         MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
             epoch1=epoch1, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
     # add offset to convert to Julian days and then convert to calendar dates
     Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
     # calculate time in year-decimal format
     time_decimal = pyTMD.time.convert_calendar_decimal(Y,M,day=D,
         hour=h,minute=m,second=s)
     # number of time points
     nt = len(time_decimal)
 
-    # degrees to radians
+    # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
     units = pyTMD.constants(ELLIPSOID)
     # tidal love number appropriate for the load tide
     hb2 = 0.6207
 
@@ -302,24 +312,25 @@
     # Normal gravity at height h. p. 82, Eqn.(2-215)
     gamma_h = units.gamma_h(theta, h)
     dfactor = -hb2*atr*(units.omega**2*rr**2)/(2.0*gamma_h)
 
     # pole tide files (mean and daily)
     mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
     pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
-    # calculate angular coordinates of mean pole at time
-    mpx,mpy,fl = pyTMD.eop.iers_mean_pole(mean_pole_file,time_decimal,'2015')
+    # calculate angular coordinates of mean/secular pole at time
+    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
+        CONVENTION)
     # read IERS daily polar motion values
     EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
     # interpolate daily polar motion values to MJD using cubic splines
     xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
     ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
     px = xSPL(MJD)
     py = ySPL(MJD)
-    # calculate differentials from mean pole positions
+    # calculate differentials from mean/secular pole positions
     mx = px - mpx
     my = -(py - mpy)
 
     # calculate radial displacement at time
     if (TYPE == 'grid'):
         Srad = np.ma.zeros((ny,nx,nt),fill_value=fill_value)
         Srad.mask = np.zeros((ny,nx,nt),dtype=bool)
@@ -416,14 +427,18 @@
     parser.add_argument('--projection','-P',
         type=str, default='4326',
         help='Spatial projection as EPSG code or PROJ4 string')
     # ellipsoid for calculating load pole tide parameters
     parser.add_argument('--ellipsoid','-E',
         type=str, choices=pyTMD._ellipsoids, default='WGS84',
         help='Ellipsoid for calculating load pole tide parameters')
+    # Earth orientation parameters
+    parser.add_argument('--convention','-c',
+        type=str, choices=pyTMD.eop._conventions, default='2018',
+        help='IERS mean or secular pole convention')
     # verbose output of processing run
     # print information about each input and output file
     parser.add_argument('--verbose','-V',
         default=False, action='store_true',
         help='Verbose output of run')
     # permissions mode of the local files (number in octal)
     parser.add_argument('--mode','-M',
@@ -452,13 +467,14 @@
         DELIMITER=args.delimiter,
         TYPE=args.type,
         TIME_UNITS=args.epoch,
         TIME=args.deltatime,
         TIME_STANDARD=args.standard,
         PROJECTION=args.projection,
         ELLIPSOID=args.ellipsoid,
+        CONVENTION=args.convention,
         VERBOSE=args.verbose,
         MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.2/scripts/compute_OPT_displacements.py` & `pyTMD-2.0.3/scripts/compute_OPT_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 u"""
 compute_OPT_displacements.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (04/2023)
 Calculates radial ocean pole load tide displacements for an input file
     following IERS Convention (2010) guidelines
-    http://maia.usno.navy.mil/conventions/2010officialinfo.php
-    http://maia.usno.navy.mil/conventions/chapter7.php
-    https://iers-conventions.obspm.fr/content/chapter7/icc7.pdf
+    https://iers-conventions.obspm.fr/chapter7.php
 
 INPUTS:
     csv file with columns for spatial and temporal coordinates
     HDF5 file with variables for spatial and temporal coordinates
     netCDF4 file with variables for spatial and temporal coordinates
     geotiff file with bands in spatial coordinates
 
@@ -24,26 +22,33 @@
         for csv files: the order of the columns within the file
         for HDF5 and netCDF4 files: time, y, x and data variable names
     -H X, --header X: number of header lines for csv files
     --delimiter X: Delimiter for csv or ascii files
     -t X, --type X: input data type
         drift: drift buoys or satellite/airborne altimetry (time per data point)
         grid: spatial grids or images (single time for all data points)
+        time series: time series at a single point
     -e X, --epoch X: Reference epoch of input time (default Modified Julian Day)
         days since 1858-11-17T00:00:00
     -d X, --deltatime X: Input delta time for files without date information
         can be set to 0 to use exact calendar date from epoch
     -s X, --standard X: Input time standard for delta times or input time type
         UTC: Coordinate Universal Time
         GPS: GPS Time
         LORAN: Long Range Navigator Time
         TAI: International Atomic Time
         datetime: formatted datetime string in UTC
     -P X, --projection X: spatial projection as EPSG code or PROJ4 string
         4326: latitude and longitude coordinates on WGS84 reference ellipsoid
+    -E X, --ellipsoid X: Ellipsoid for calculating load pole tide parameters
+    -c X, --convention X: IERS mean or secular pole convention
+        2003
+        2010
+        2015
+        2018
     -I X, --interpolate X: Interpolation method
         spline
         linear
         nearest
     -V, --verbose: Verbose output of processing run
     -M X, --mode X: Permission mode of output file
 
@@ -75,14 +80,16 @@
     S Desai, "Observing the pole tide with satellite altimetry", Journal of
         Geophysical Research: Oceans, 107(C11), 2002. doi: 10.1029/2001JC001224
     S Desai, J Wahr and B Beckley "Revisiting the pole tide for and from
         satellite altimetry", Journal of Geodesy, 89(12), p1233-1243, 2015.
         doi: 10.1007/s00190-015-0848-7
 
 UPDATE HISTORY:
+    Updated 04/2023: check if datetime before converting to seconds
+    Updated 03/2023: added option for changing the IERS mean pole convention
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
         use constants class for ellipsoidal parameters
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
@@ -162,14 +169,15 @@
     DELIMITER=',',
     TYPE='drift',
     TIME_UNITS='days since 1858-11-17T00:00:00',
     TIME=None,
     TIME_STANDARD='UTC',
     PROJECTION='4326',
     ELLIPSOID='WGS84',
+    CONVENTION='2018',
     METHOD='spline',
     VERBOSE=False,
     MODE=0o775):
 
     # create logger for verbosity level
     loglevel = logging.INFO if VERBOSE else logging.CRITICAL
     logging.basicConfig(level=loglevel)
@@ -242,15 +250,16 @@
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
     # convert time to seconds
-    delta_time = to_secs*dinput['time'].flatten()
+    if (TIME_STANDARD.lower() != 'datetime'):
+        delta_time = to_secs*dinput['time'].flatten()
 
     # calculate leap seconds if specified
     if (TIME_STANDARD.upper() == 'GPS'):
         GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
         GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
@@ -277,29 +286,29 @@
             pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
     else:
         leap_seconds = 0.0
 
     if (TIME_STANDARD.lower() == 'datetime'):
         # convert delta time array from datetime object
         # to Modified Julian days (days since 1858-11-17T00:00:00)
-        MJD = pyTMD.time.convert_datetime(delta_time,
+        MJD = pyTMD.time.convert_datetime(dinput['time'].flatten(),
             epoch=pyTMD.time._mjd_epoch)/86400.0
     else:
         # convert dates to Modified Julian days (days since 1858-11-17T00:00:00)
         MJD = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
             epoch1=epoch1, epoch2=pyTMD.time._mjd_epoch, scale=1.0/86400.0)
     # add offset to convert to Julian days and then convert to calendar dates
     Y,M,D,h,m,s = pyTMD.time.convert_julian(2400000.5 + MJD, format='tuple')
     # calculate time in year-decimal format
     time_decimal = pyTMD.time.convert_calendar_decimal(Y,M,day=D,
         hour=h,minute=m,second=s)
     # number of time points
     nt = len(time_decimal)
 
-    # degrees to radians and arcseconds to radians
+    # degrees and arcseconds to radians
     dtr = np.pi/180.0
     atr = np.pi/648000.0
     # earth and physical parameters for ellipsoid
     units = pyTMD.constants(ELLIPSOID)
     # mean equatorial gravitational acceleration [m/s^2]
     ge = 9.7803278
     # density of sea water [kg/m^3]
@@ -320,27 +329,27 @@
     Hp = np.sqrt(8.0*np.pi/15.0)*(units.omega**2*units.a_axis**4)/units.GM
     K = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis/(3.0*ge)
     K1 = 4.0*np.pi*units.G*rho_w*Hp*units.a_axis**3/(3.0*units.GM)
 
     # pole tide files (mean and daily)
     mean_pole_file = pyTMD.utilities.get_data_path(['data','mean-pole.tab'])
     pole_tide_file = pyTMD.utilities.get_data_path(['data','finals.all'])
-    # calculate angular coordinates of mean pole at time
-    mpx,mpy,fl = pyTMD.eop.iers_mean_pole(mean_pole_file,time_decimal,'2015')
+    # calculate angular coordinates of mean/secular pole at time
+    mpx, mpy, fl = pyTMD.eop.iers_mean_pole(mean_pole_file, time_decimal,
+        CONVENTION)
     # read IERS daily polar motion values
     EOP = pyTMD.eop.iers_daily_EOP(pole_tide_file)
     # interpolate daily polar motion values to t1 using cubic splines
     xSPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['x'],k=3,s=0)
     ySPL = scipy.interpolate.UnivariateSpline(EOP['MJD'],EOP['y'],k=3,s=0)
     px = xSPL(MJD)
     py = ySPL(MJD)
-    # calculate differentials from mean pole positions
+    # calculate differentials from mean/secular pole positions
     mx = px - mpx
     my = -(py - mpy)
-    print(mpx, mpy, px, py)
 
     # read ocean pole tide map from Desai (2002)
     ocean_pole_tide_file = pyTMD.utilities.get_data_path(['data',
         'opoleloadcoefcmcor.txt.gz'])
     iur,iun,iue,ilon,ilat = pyTMD.io.ocean_pole_tide(ocean_pole_tide_file)
     # interpolate ocean pole tide map from Desai (2002)
     if (METHOD == 'spline'):
@@ -458,14 +467,18 @@
     parser.add_argument('--projection','-P',
         type=str, default='4326',
         help='Spatial projection as EPSG code or PROJ4 string')
     # ellipsoid for calculating load pole tide parameters
     parser.add_argument('--ellipsoid','-E',
         type=str, choices=pyTMD._ellipsoids, default='WGS84',
         help='Ellipsoid for calculating load pole tide parameters')
+    # Earth orientation parameters
+    parser.add_argument('--convention','-c',
+        type=str, choices=pyTMD.eop._conventions, default='2018',
+        help='IERS mean or secular pole convention')
     # interpolation method
     parser.add_argument('--interpolate','-I',
         metavar='METHOD', type=str, default='spline',
         choices=('spline','linear','nearest'),
         help='Spatial interpolation method')
     # verbose output of processing run
     # print information about each input and output file
@@ -499,14 +512,15 @@
         DELIMITER=args.delimiter,
         TYPE=args.type,
         TIME_UNITS=args.epoch,
         TIME=args.deltatime,
         TIME_STANDARD=args.standard,
         PROJECTION=args.projection,
         ELLIPSOID=args.ellipsoid,
+        CONVENTION=args.convention,
         METHOD=args.interpolate,
         VERBOSE=args.verbose,
         MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.2/scripts/compute_tidal_currents.py` & `pyTMD-2.0.3/scripts/compute_tidal_currents.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial: utilities for reading, writing and operating on spatial data
     utilities.py: download and management utilities for syncing files
-    calc_astrol_longitudes.py: computes the basic astronomical mean longitudes
-    convert_ll_xy.py: convert lat/lon points to and from projected coordinates
+    astro.py: computes the basic astronomical mean longitudes
+    convert_crs.py: convert points to and from Coordinates Reference Systems
     load_constituent.py: loads parameters for a given tidal constituent
     load_nodal_corrections.py: load the nodal corrections for tidal constituents
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
```

### Comparing `pyTMD-2.0.2/scripts/compute_tidal_elevations.py` & `pyTMD-2.0.3/scripts/compute_tidal_elevations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 compute_tidal_elevations.py
-Written by Tyler Sutterley (02/2023)
+Written by Tyler Sutterley (04/2023)
 Calculates tidal elevations for an input file
 
 Uses OTIS format tidal solutions provided by Ohio State University and ESR
     http://volkov.oce.orst.edu/tides/region.html
     https://www.esr.org/research/polar-tide-models/list-of-polar-tide-models/
     ftp://ftp.esr.org/pub/datasets/tmd/
 Global Tide Model (GOT) solutions provided by Richard Ray at GSFC
@@ -78,26 +78,27 @@
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
     time.py: utilities for calculating time operations
     spatial: utilities for reading, writing and operating on spatial data
     utilities.py: download and management utilities for syncing files
-    calc_astrol_longitudes.py: computes the basic astronomical mean longitudes
-    convert_ll_xy.py: convert lat/lon points to and from projected coordinates
+    astro.py: computes the basic astronomical mean longitudes
+    convert_crs.py: convert points to and from Coordinates Reference Systems
     load_constituent.py: loads parameters for a given tidal constituent
     load_nodal_corrections.py: load the nodal corrections for tidal constituents
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     io/ATLAS.py: extract tidal harmonic constants from netcdf models
     io/FES.py: extract tidal harmonic constants from FES tide models
     interpolate.py: interpolation routines for spatial data
     predict.py: predict tidal values using harmonic constants
 
 UPDATE HISTORY:
+    Updated 04/2023: check if datetime before converting to seconds
     Updated 02/2023: added functionality for time series type
     Updated 01/2023: added default field mapping for reading from netCDF4/HDF5
         added data type keyword for netCDF4 output
     Updated 12/2022: single implicit import of pyTMD tools
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 10/2022: added delimiter option and datetime parsing for ascii files
@@ -279,15 +280,16 @@
     # extract time units from netCDF4 and HDF5 attributes or from TIME_UNITS
     try:
         time_string = dinput['attributes']['time']['units']
         epoch1, to_secs = pyTMD.time.parse_date_string(time_string)
     except (TypeError, KeyError, ValueError):
         epoch1, to_secs = pyTMD.time.parse_date_string(TIME_UNITS)
     # convert time to seconds
-    delta_time = to_secs*dinput['time'].flatten()
+    if (TIME_STANDARD.lower() != 'datetime'):
+        delta_time = to_secs*dinput['time'].flatten()
 
     # calculate leap seconds if specified
     if (TIME_STANDARD.upper() == 'GPS'):
         GPS_Epoch_Time = pyTMD.time.convert_delta_time(0, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
         GPS_Time = pyTMD.time.convert_delta_time(delta_time, epoch1=epoch1,
             epoch2=pyTMD.time._gps_epoch, scale=1.0)
@@ -314,15 +316,15 @@
             pyTMD.time.count_leap_seconds(np.atleast_1d(GPS_Epoch_Time))
     else:
         leap_seconds = 0.0
 
     if (TIME_STANDARD.lower() == 'datetime'):
         # convert delta time array from datetime object
         # to days relative to 1992-01-01T00:00:00
-        tide_time = pyTMD.time.convert_datetime(delta_time,
+        tide_time = pyTMD.time.convert_datetime(dinput['time'].flatten(),
             epoch=pyTMD.time._tide_epoch)/86400.0
     else:
         # convert time from units to days since 1992-01-01T00:00:00
         tide_time = pyTMD.time.convert_delta_time(delta_time-leap_seconds,
             epoch1=epoch1, epoch2=pyTMD.time._tide_epoch, scale=1.0/86400.0)
     # number of time points
     nt = len(tide_time)
```

### Comparing `pyTMD-2.0.2/scripts/reduce_OTIS_files.py` & `pyTMD-2.0.3/scripts/reduce_OTIS_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
     pyproj: Python interface to PROJ library
         https://pypi.org/project/pyproj/
 
 PROGRAM DEPENDENCIES:
     io/model.py: retrieves tide model parameters for named tide models
     io/OTIS.py: extract tidal harmonic constants from OTIS tide models
     utilities.py: download and management utilities for syncing files
-    convert_ll_xy.py: converts lat/lon points to and from projected coordinates
+    convert_crs.py: converts lat/lon points to and from projected coordinates
 
 UPDATE HISTORY:
+    Updated 03/2023: new function name for coordinate reference systems
     Updated 12/2022: refactored OTIS model input and output
     Updated 11/2022: place some imports within try/except statements
         use f-strings for formatting verbose or ascii output
     Updated 05/2022: updated keyword arguments to read tide model programs
     Updated 04/2022: use argparse descriptions within documentation
     Updated 11/2021: add function for attempting to extract projection
     Updated 09/2021: refactor to use model class for files and attributes
@@ -50,15 +51,15 @@
 import sys
 import os
 import warnings
 import argparse
 import numpy as np
 import pyTMD.io
 import pyTMD.utilities
-from pyTMD.convert_ll_xy import convert_ll_xy
+from pyTMD.convert_crs import convert_crs
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("pyproj not available", ImportWarning)
@@ -111,15 +112,15 @@
     crs2 = pyproj.CRS.from_epsg(4326)
     transformer = pyproj.Transformer.from_crs(crs1, crs2, always_xy=True)
     xbox = np.array([BOUNDS[0],BOUNDS[1],BOUNDS[1],BOUNDS[0],BOUNDS[0]])
     ybox = np.array([BOUNDS[2],BOUNDS[2],BOUNDS[3],BOUNDS[3],BOUNDS[2]])
     lon,lat = transformer.transform(xbox,ybox)
 
     # convert bounds from latitude/longitude to model coordinates
-    x,y = convert_ll_xy(lon,lat,model.projection,'F')
+    x,y = convert_crs(lon,lat,model.projection,'F')
 
     # find indices to reduce to xmin,xmax,ymin,ymax
     gridx,gridy = np.meshgrid(xi,yi)
     indy,indx = np.nonzero((gridx >= x.min()) & (gridx <= x.max()) &
         (gridy >= y.min()) & (gridy <= y.max()))
     nx = np.count_nonzero((xi >= x.min()) & (xi <= x.max()))
     ny = np.count_nonzero((yi >= y.min()) & (yi <= y.max()))
```

### Comparing `pyTMD-2.0.2/scripts/usap_cats_tides.py` & `pyTMD-2.0.3/scripts/usap_cats_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/scripts/verify_box_tpxo.py` & `pyTMD-2.0.3/scripts/verify_box_tpxo.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.2/setup.py` & `pyTMD-2.0.3/setup.py`

 * *Files identical despite different names*

