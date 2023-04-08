# Comparing `tmp/seismon-0.0.5.tar.gz` & `tmp/seismon-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismon-0.0.5.tar", last modified: Sat Apr  8 18:12:01 2023, max compression
+gzip compressed data, was "seismon-0.0.6.tar", last modified: Sat Apr  8 19:03:32 2023, max compression
```

## Comparing `seismon-0.0.5.tar` & `seismon-0.0.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 18:12:01.660879 seismon-0.0.5/
--rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2022-08-09 21:11:44.000000 seismon-0.0.5/LICENSE
--rw-r--r--   0 mcoughlin   (501) staff       (20)      127 2022-08-09 21:11:44.000000 seismon-0.0.5/MANIFEST.in
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1264 2023-04-08 18:12:01.660962 seismon-0.0.5/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)      613 2023-04-08 18:02:18.000000 seismon-0.0.5/README.md
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 18:12:01.656177 seismon-0.0.5/bin/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2771 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/cause_lockstate.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1753 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/cause_lockstate_timeseries.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     8857 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_compare_eventfiles
--rw-r--r--   0 mcoughlin   (501) staff       (20)    11944 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_epics
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)    12433 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_epics_client.py
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3089 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_epics_ioc.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6401 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_fake_events
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5341 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_info
--rw-r--r--   0 mcoughlin   (501) staff       (20)      605 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_lockloss_prediction.sh
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4063 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_pdlclient
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4111 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_pdlclient_root
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4723 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_performance
--rw-r--r--   0 mcoughlin   (501) staff       (20)    15594 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_prediction_vs_actual
--rw-r--r--   0 mcoughlin   (501) staff       (20)    12342 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_prediction_vs_actual_combine
--rw-r--r--   0 mcoughlin   (501) staff       (20)    17248 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_prediction_vs_actual_combine_gpr
--rw-r--r--   0 mcoughlin   (501) staff       (20)     6725 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_prediction_vs_actual_diagnostic
--rw-r--r--   0 mcoughlin   (501) staff       (20)    22279 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     1928 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_info
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13303 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_prediction_vs_actual
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3221 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_prediction_vs_actual_diagnostic
--rw-r--r--   0 mcoughlin   (501) staff       (20)    11153 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_prediction_vs_actual_ec
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5227 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_prediction_vs_actual_postO1
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1301 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2327 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_H1O1
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2294 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_H1O1_lockloss
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2808 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_H1O1_rms
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1946 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_L1O1
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1913 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_L1O1_lockloss
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2427 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_L1O1_rms
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1531 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_V1O1O2
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1339 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_run_frames
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     1371 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_run_traveltimes
--rw-r--r--   0 mcoughlin   (501) staff       (20)      341 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_setup_epics.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    25519 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_traveltimes
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13691 2022-08-09 21:11:44.000000 seismon-0.0.5/bin/seismon_traveltimes_analysis
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 18:12:01.661436 seismon-0.0.5/seismon/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2139 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/NLNM.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1034 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)      497 2023-04-08 18:12:01.661471 seismon-0.0.5/seismon/_version.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     9896 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/beamforming.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    22194 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/bits.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     8613 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/coherence.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     2639 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/config.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)   118488 2023-04-08 18:02:18.000000 seismon-0.0.5/seismon/eqmon.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    57952 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/eqmon_plot.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13642 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/hilbert.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 18:12:01.660765 seismon-0.0.5/seismon/input/
--rw-r--r--   0 mcoughlin   (501) staff       (20)   626085 2023-04-08 18:02:18.000000 seismon-0.0.5/seismon/input/LHO_processed_USGS_global_EQ_catalogue.csv
--rw-r--r--   0 mcoughlin   (501) staff       (20)   613475 2023-04-08 18:02:18.000000 seismon-0.0.5/seismon/input/LLO_processed_USGS_global_EQ_catalogue.csv
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1034 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/input/__init__.py
--rwxr-xr-x   0 mcoughlin   (501) staff       (20)     8559 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/input/config.ini
--rw-r--r--   0 mcoughlin   (501) staff       (20)      531 2023-04-08 18:02:18.000000 seismon-0.0.5/seismon/input/config.yaml
--rw-r--r--   0 mcoughlin   (501) staff       (20)      540 2023-04-08 18:02:18.000000 seismon-0.0.5/seismon/input/config_carleton.yaml
--rw-r--r--   0 mcoughlin   (501) staff       (20)     8295 2022-08-09 21:11:44.000000 seismon-0.0.5/seismon/input/countries.csv
--rw-r--r--   0 mcoughlin   (501) staff       (20)    28101 2023-04-08 18:02:19.000000 seismon-0.0.5/seismon/models.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     7031 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/omicron.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    52740 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/psd.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5100 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/trend.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    52043 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/utils.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     4604 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/views.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5576 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/viz.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    25537 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/wiener.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    13235 2022-08-09 21:11:45.000000 seismon-0.0.5/seismon/wiener_fft.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 18:12:01.659220 seismon-0.0.5/seismon.egg-info/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1264 2023-04-08 18:12:01.000000 seismon-0.0.5/seismon.egg-info/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1859 2023-04-08 18:12:01.000000 seismon-0.0.5/seismon.egg-info/SOURCES.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-04-08 18:12:01.000000 seismon-0.0.5/seismon.egg-info/dependency_links.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      219 2023-04-08 18:12:01.000000 seismon-0.0.5/seismon.egg-info/requires.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        8 2023-04-08 18:12:01.000000 seismon-0.0.5/seismon.egg-info/top_level.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-04-08 18:12:01.661274 seismon-0.0.5/setup.cfg
--rw-r--r--   0 mcoughlin   (501) staff       (20)     3986 2022-08-09 21:11:45.000000 seismon-0.0.5/setup.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2022-08-09 21:11:45.000000 seismon-0.0.5/versioneer.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 19:03:32.879014 seismon-0.0.6/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    35147 2022-08-09 21:11:44.000000 seismon-0.0.6/LICENSE
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      127 2022-08-09 21:11:44.000000 seismon-0.0.6/MANIFEST.in
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1264 2023-04-08 19:03:32.879101 seismon-0.0.6/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      613 2023-04-08 18:02:18.000000 seismon-0.0.6/README.md
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 19:03:32.870315 seismon-0.0.6/bin/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2771 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/cause_lockstate.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1753 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/cause_lockstate_timeseries.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     8857 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_compare_eventfiles
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    11944 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_epics
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)    12433 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_epics_client.py
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     3089 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_epics_ioc.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6401 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_fake_events
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5341 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_info
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      605 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_lockloss_prediction.sh
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4063 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_pdlclient
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4111 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_pdlclient_root
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4723 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_performance
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    15594 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_prediction_vs_actual
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    12342 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_prediction_vs_actual_combine
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    17248 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_prediction_vs_actual_combine_gpr
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     6725 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_prediction_vs_actual_diagnostic
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    22279 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     1928 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_info
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13303 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_prediction_vs_actual
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     3221 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_prediction_vs_actual_diagnostic
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    11153 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_prediction_vs_actual_ec
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5227 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_prediction_vs_actual_postO1
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1301 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2327 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_H1O1
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2294 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_H1O1_lockloss
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2808 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_H1O1_rms
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1946 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_L1O1
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1913 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_L1O1_lockloss
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2427 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_L1O1_rms
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1531 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_V1O1O2
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1339 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_run_frames
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     1371 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_run_traveltimes
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      341 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_setup_epics.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    25519 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_traveltimes
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13691 2022-08-09 21:11:44.000000 seismon-0.0.6/bin/seismon_traveltimes_analysis
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 19:03:32.879776 seismon-0.0.6/seismon/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2139 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/NLNM.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1034 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      497 2023-04-08 19:03:32.879809 seismon-0.0.6/seismon/_version.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     9896 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/beamforming.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    22194 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/bits.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     8613 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/coherence.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     2639 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/config.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)   118488 2023-04-08 18:02:18.000000 seismon-0.0.6/seismon/eqmon.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    57952 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/eqmon_plot.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13642 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/hilbert.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 19:03:32.878872 seismon-0.0.6/seismon/input/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)   626085 2023-04-08 18:02:18.000000 seismon-0.0.6/seismon/input/LHO_processed_USGS_global_EQ_catalogue.csv
+-rw-r--r--   0 mcoughlin   (501) staff       (20)   613475 2023-04-08 18:02:18.000000 seismon-0.0.6/seismon/input/LLO_processed_USGS_global_EQ_catalogue.csv
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1034 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/input/__init__.py
+-rwxr-xr-x   0 mcoughlin   (501) staff       (20)     8559 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/input/config.ini
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      531 2023-04-08 18:02:18.000000 seismon-0.0.6/seismon/input/config.yaml
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      540 2023-04-08 18:02:18.000000 seismon-0.0.6/seismon/input/config_carleton.yaml
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     8295 2022-08-09 21:11:44.000000 seismon-0.0.6/seismon/input/countries.csv
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    28101 2023-04-08 18:02:19.000000 seismon-0.0.6/seismon/models.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     7031 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/omicron.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    52740 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/psd.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5100 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/trend.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    52043 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/utils.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4604 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/views.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5576 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/viz.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    25537 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/wiener.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    13235 2022-08-09 21:11:45.000000 seismon-0.0.6/seismon/wiener_fft.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2023-04-08 19:03:32.875346 seismon-0.0.6/seismon.egg-info/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1264 2023-04-08 19:03:32.000000 seismon-0.0.6/seismon.egg-info/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1859 2023-04-08 19:03:32.000000 seismon-0.0.6/seismon.egg-info/SOURCES.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2023-04-08 19:03:32.000000 seismon-0.0.6/seismon.egg-info/dependency_links.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      228 2023-04-08 19:03:32.000000 seismon-0.0.6/seismon.egg-info/requires.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        8 2023-04-08 19:03:32.000000 seismon-0.0.6/seismon.egg-info/top_level.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      402 2023-04-08 19:03:32.879607 seismon-0.0.6/setup.cfg
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     4002 2023-04-08 19:02:29.000000 seismon-0.0.6/setup.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    68611 2022-08-09 21:11:45.000000 seismon-0.0.6/versioneer.py
```

### Comparing `seismon-0.0.5/LICENSE` & `seismon-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/PKG-INFO` & `seismon-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismon
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for mitigating the effects of earthquakes on GW detectors
 Home-page: https://github.com/gwdetchar/seismon/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPL-2.0-or-later
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `seismon-0.0.5/README.md` & `seismon-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/cause_lockstate.py` & `seismon-0.0.6/bin/cause_lockstate.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/cause_lockstate_timeseries.py` & `seismon-0.0.6/bin/cause_lockstate_timeseries.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_compare_eventfiles` & `seismon-0.0.6/bin/seismon_compare_eventfiles`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_epics` & `seismon-0.0.6/bin/seismon_epics`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_epics_client.py` & `seismon-0.0.6/bin/seismon_epics_client.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_epics_ioc.py` & `seismon-0.0.6/bin/seismon_epics_ioc.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_fake_events` & `seismon-0.0.6/bin/seismon_fake_events`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_info` & `seismon-0.0.6/bin/seismon_info`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_lockloss_prediction.sh` & `seismon-0.0.6/bin/seismon_lockloss_prediction.sh`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_pdlclient` & `seismon-0.0.6/bin/seismon_pdlclient`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_pdlclient_root` & `seismon-0.0.6/bin/seismon_pdlclient_root`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_performance` & `seismon-0.0.6/bin/seismon_performance`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_prediction_vs_actual` & `seismon-0.0.6/bin/seismon_prediction_vs_actual`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_prediction_vs_actual_combine` & `seismon-0.0.6/bin/seismon_prediction_vs_actual_combine`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_prediction_vs_actual_combine_gpr` & `seismon-0.0.6/bin/seismon_prediction_vs_actual_combine_gpr`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_prediction_vs_actual_diagnostic` & `seismon-0.0.6/bin/seismon_prediction_vs_actual_diagnostic`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run` & `seismon-0.0.6/bin/seismon_run`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_info` & `seismon-0.0.6/bin/seismon_run_info`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_prediction_vs_actual` & `seismon-0.0.6/bin/seismon_run_prediction_vs_actual`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_prediction_vs_actual_diagnostic` & `seismon-0.0.6/bin/seismon_run_prediction_vs_actual_diagnostic`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_prediction_vs_actual_ec` & `seismon-0.0.6/bin/seismon_run_prediction_vs_actual_ec`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_prediction_vs_actual_postO1` & `seismon-0.0.6/bin/seismon_run_prediction_vs_actual_postO1`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run` & `seismon-0.0.6/bin/seismon_run_run`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_H1O1` & `seismon-0.0.6/bin/seismon_run_run_H1O1`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_H1O1_lockloss` & `seismon-0.0.6/bin/seismon_run_run_H1O1_lockloss`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_H1O1_rms` & `seismon-0.0.6/bin/seismon_run_run_H1O1_rms`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_L1O1` & `seismon-0.0.6/bin/seismon_run_run_L1O1`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_L1O1_lockloss` & `seismon-0.0.6/bin/seismon_run_run_L1O1_lockloss`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_L1O1_rms` & `seismon-0.0.6/bin/seismon_run_run_L1O1_rms`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_V1O1O2` & `seismon-0.0.6/bin/seismon_run_run_V1O1O2`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_run_frames` & `seismon-0.0.6/bin/seismon_run_run_frames`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_run_traveltimes` & `seismon-0.0.6/bin/seismon_run_traveltimes`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_traveltimes` & `seismon-0.0.6/bin/seismon_traveltimes`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/bin/seismon_traveltimes_analysis` & `seismon-0.0.6/bin/seismon_traveltimes_analysis`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/NLNM.py` & `seismon-0.0.6/seismon/NLNM.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/__init__.py` & `seismon-0.0.6/seismon/__init__.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/beamforming.py` & `seismon-0.0.6/seismon/beamforming.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/bits.py` & `seismon-0.0.6/seismon/bits.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/coherence.py` & `seismon-0.0.6/seismon/coherence.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/config.py` & `seismon-0.0.6/seismon/config.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/eqmon.py` & `seismon-0.0.6/seismon/eqmon.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/eqmon_plot.py` & `seismon-0.0.6/seismon/eqmon_plot.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/hilbert.py` & `seismon-0.0.6/seismon/hilbert.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/LHO_processed_USGS_global_EQ_catalogue.csv` & `seismon-0.0.6/seismon/input/LHO_processed_USGS_global_EQ_catalogue.csv`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/LLO_processed_USGS_global_EQ_catalogue.csv` & `seismon-0.0.6/seismon/input/LLO_processed_USGS_global_EQ_catalogue.csv`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/__init__.py` & `seismon-0.0.6/seismon/input/__init__.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/config.ini` & `seismon-0.0.6/seismon/input/config.ini`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/config.yaml` & `seismon-0.0.6/seismon/input/config.yaml`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/config_carleton.yaml` & `seismon-0.0.6/seismon/input/config_carleton.yaml`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/input/countries.csv` & `seismon-0.0.6/seismon/input/countries.csv`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/models.py` & `seismon-0.0.6/seismon/models.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/omicron.py` & `seismon-0.0.6/seismon/omicron.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/psd.py` & `seismon-0.0.6/seismon/psd.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/trend.py` & `seismon-0.0.6/seismon/trend.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/utils.py` & `seismon-0.0.6/seismon/utils.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/views.py` & `seismon-0.0.6/seismon/views.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/viz.py` & `seismon-0.0.6/seismon/viz.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/wiener.py` & `seismon-0.0.6/seismon/wiener.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon/wiener_fft.py` & `seismon-0.0.6/seismon/wiener_fft.py`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/seismon.egg-info/PKG-INFO` & `seismon-0.0.6/seismon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismon
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for mitigating the effects of earthquakes on GW detectors
 Home-page: https://github.com/gwdetchar/seismon/
 Author: Michael Coughlin
 Author-email: michael.coughlin@ligo.org
 License: GPL-2.0-or-later
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `seismon-0.0.5/seismon.egg-info/SOURCES.txt` & `seismon-0.0.6/seismon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seismon-0.0.5/setup.py` & `seismon-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     'flask_wtf',
     'gwpy',
     'lxml',
     'matplotlib>=2.2.0',
     'numpy>=1.7.1',
     'obspy',
     'passlib',
+    'psycopg2',
     'redis',
     'scipy>=0.12.1',
     'simplejson',
     'sqlalchemy',
 ]
 
 # test dependencies
```

### Comparing `seismon-0.0.5/versioneer.py` & `seismon-0.0.6/versioneer.py`

 * *Files identical despite different names*

