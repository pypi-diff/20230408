# Comparing `tmp/python-allib-0.3.4.0.tar.gz` & `tmp/python-allib-0.3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-allib-0.3.4.0.tar", last modified: Fri Mar 31 14:47:22 2023, max compression
+gzip compressed data, was "python-allib-0.3.5.0.tar", last modified: Fri Apr  7 22:16:35 2023, max compression
```

## Comparing `python-allib-0.3.4.0.tar` & `python-allib-0.3.5.0.tar`

### file list

```diff
@@ -1,202 +1,159 @@
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3142 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/.gitignore
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1392 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/.gitlab-ci.yml
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/CHANGELOG
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/CONTRIBUTING.md
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7651 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/LICENSE
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      488 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/PKG-INFO
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/README.md
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.076999 python-allib-0.3.4.0/allib/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       96 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2019 2023-03-31 14:45:11.000000 python-allib-0.3.4.0/allib/__main__.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.080999 python-allib-0.3.4.0/allib/activelearning/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      234 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/activelearning/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9998 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/ats.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7291 2023-02-21 08:34:49.000000 python-allib-0.3.4.0/allib/activelearning/autostop.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11146 2023-03-31 12:03:12.000000 python-allib-0.3.4.0/allib/activelearning/autotar.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3410 2023-03-30 14:45:29.000000 python-allib-0.3.4.0/allib/activelearning/autotarensemble.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9002 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1469 2023-03-30 13:09:14.000000 python-allib-0.3.4.0/allib/activelearning/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9293 2023-03-30 11:40:31.000000 python-allib-0.3.4.0/allib/activelearning/ensembles.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      132 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/activelearning/estimate.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4018 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/estimator.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    14632 2023-03-31 12:05:19.000000 python-allib-0.3.4.0/allib/activelearning/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1111 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/fixed.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/activelearning/helperfunctions.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    15492 2022-11-22 09:59:54.000000 python-allib-0.3.4.0/allib/activelearning/insclass.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4697 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/labelmethods.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4486 2023-03-30 09:34:31.000000 python-allib-0.3.4.0/allib/activelearning/learnersequence.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    16302 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/ml_based.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2228 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/mostcertain.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2191 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/activelearning/oracles.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5556 2023-03-31 11:52:35.000000 python-allib-0.3.4.0/allib/activelearning/poolbased.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10769 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/prob_ensembles.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3222 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/qbc.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      416 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/random.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      815 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/selectioncriterion.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2840 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/sequence.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1652 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/activelearning/synthetictrain.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1418 2023-03-30 12:45:14.000000 python-allib-0.3.4.0/allib/activelearning/target.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4824 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/tsvm.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2893 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/activelearning/uncertainty.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.080999 python-allib-0.3.4.0/allib/analysis/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/analysis/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8466 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/analysis/analysis.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8679 2023-03-29 13:37:22.000000 python-allib-0.3.4.0/allib/analysis/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7853 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/analysis/classificationplotter.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10456 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/analysis/experiments.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7435 2023-03-30 13:52:49.000000 python-allib-0.3.4.0/allib/analysis/initialization.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5564 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/analysis/plotter.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7213 2023-03-29 07:42:54.000000 python-allib-0.3.4.0/allib/analysis/simulation.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4736 2023-03-31 14:11:38.000000 python-allib-0.3.4.0/allib/analysis/statistics.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2563 2023-03-28 12:33:01.000000 python-allib-0.3.4.0/allib/analysis/summarize.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6516 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/analysis/tablecollector.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    15875 2023-03-31 14:42:59.000000 python-allib-0.3.4.0/allib/analysis/tarplotter.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2997 2023-03-31 14:44:56.000000 python-allib-0.3.4.0/allib/app.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.084999 python-allib-0.3.4.0/allib/balancing/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      253 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/balancing/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1484 2022-11-22 09:59:54.000000 python-allib-0.3.4.0/allib/balancing/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      223 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/balancing/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5563 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/balancing/double.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1106 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/balancing/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      707 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/balancing/randomoversampling.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8651 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/balancing/triple.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2752 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/balancing/undersample.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.084999 python-allib-0.3.4.0/allib/benchmarking/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/benchmarking/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      958 2023-02-17 14:15:15.000000 python-allib-0.3.4.0/allib/benchmarking/datasets.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3781 2023-03-29 08:15:55.000000 python-allib-0.3.4.0/allib/benchmarking/reviews.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.084999 python-allib-0.3.4.0/allib/configurations/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      100 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/configurations/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11519 2023-03-30 14:53:51.000000 python-allib-0.3.4.0/allib/configurations/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1812 2023-03-30 13:54:12.000000 python-allib-0.3.4.0/allib/configurations/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    17776 2023-03-30 14:54:04.000000 python-allib-0.3.4.0/allib/configurations/ensemble.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      626 2023-01-11 13:33:33.000000 python-allib-0.3.4.0/allib/configurations/tarbaselines.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.084999 python-allib-0.3.4.0/allib/environment/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      158 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/environment/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3073 2023-01-11 13:33:33.000000 python-allib-0.3.4.0/allib/environment/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      124 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/environment/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      618 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/environment/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5839 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/environment/hdf5.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11221 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/environment/memory.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.088999 python-allib-0.3.4.0/allib/estimation/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/estimation/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4241 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/autostop.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1292 2023-01-29 09:19:34.000000 python-allib-0.3.4.0/allib/estimation/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8776 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/loglinear.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1127 2023-03-30 14:13:43.000000 python-allib-0.3.4.0/allib/estimation/mhmodel.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8693 2023-03-30 13:41:28.000000 python-allib-0.3.4.0/allib/estimation/mhmodel.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      821 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/multiple_estimate.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    18610 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2744 2022-05-04 18:43:11.000000 python-allib-0.3.4.0/allib/estimation/rasch_bruteforce.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    17839 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_comb_parametric.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5317 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/estimation/rasch_em.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11617 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_em_comb.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      426 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/estimation/rasch_estimate.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4459 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_estimate_bootstrap.R
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    42067 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_multiple.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5469 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_parametric.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12015 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rasch_python.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12830 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/rcapture.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4772 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/estimation/semi.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.088999 python-allib-0.3.4.0/allib/exceptions/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      107 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/exceptions/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      823 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/exceptions/base.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.088999 python-allib-0.3.4.0/allib/factory/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       66 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/factory/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1795 2021-12-06 14:27:10.000000 python-allib-0.3.4.0/allib/factory/factory.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.092999 python-allib-0.3.4.0/allib/feature_extraction/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      193 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/feature_extraction/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11513 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/feature_extraction/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      445 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/feature_extraction/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1718 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/feature_extraction/contextinstance.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2740 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/feature_extraction/doc2vec.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3566 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/feature_extraction/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1200 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/feature_extraction/textinstance.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1530 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/feature_extraction/textsklearn.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.092999 python-allib-0.3.4.0/allib/history/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       61 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/history/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1369 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/history/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6083 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/history/memory.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.092999 python-allib-0.3.4.0/allib/machinelearning/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      214 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/machinelearning/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3659 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/balanced_il.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2168 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      562 2023-01-11 13:33:33.000000 python-allib-0.3.4.0/allib/machinelearning/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4830 2023-01-11 13:33:33.000000 python-allib-0.3.4.0/allib/machinelearning/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6199 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/sklearn.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    20600 2023-01-17 15:54:58.000000 python-allib-0.3.4.0/allib/machinelearning/sparse.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    13318 2023-03-30 11:46:56.000000 python-allib-0.3.4.0/allib/machinelearning/taroptimized.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.092999 python-allib-0.3.4.0/allib/machinelearning/transductive/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/transductive/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1028 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/transductive/il_tsvm.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    37551 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/transductive/qns3vm.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4839 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/machinelearning/transductive/tsvm_sklearn.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.092999 python-allib-0.3.4.0/allib/module/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      101 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/module/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      563 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/module/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      317 2022-11-22 10:08:33.000000 python-allib-0.3.4.0/allib/module/component.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      495 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/module/factory.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/py.typed
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.097000 python-allib-0.3.4.0/allib/stopcriterion/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/stopcriterion/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      748 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/stopcriterion/apriori.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      854 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/stopcriterion/base.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      181 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/stopcriterion/catalog.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10960 2023-01-11 13:33:33.000000 python-allib-0.3.4.0/allib/stopcriterion/estimation.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3959 2023-03-30 14:15:09.000000 python-allib-0.3.4.0/allib/stopcriterion/heuristic.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8296 2023-03-29 13:54:41.000000 python-allib-0.3.4.0/allib/stopcriterion/others.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1319 2023-03-30 12:14:13.000000 python-allib-0.3.4.0/allib/stopcriterion/target.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.097000 python-allib-0.3.4.0/allib/typehints/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      137 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/typehints/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1407 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/typehints/typevars.py
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.097000 python-allib-0.3.4.0/allib/utils/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      191 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/__init__.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1454 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/chunks.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12439 2022-11-22 09:59:54.000000 python-allib-0.3.4.0/allib/utils/func.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      217 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/utils/io.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3258 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib/utils/numpy.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2589 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/producer_consumer.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      288 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/random.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2688 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/saveablemodel.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      714 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/allib/utils/to_key.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      280 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/allib.Rproj
--rwxrwxr-x   0 michielbron  (1000) michielbron  (1000)       67 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/benchmark.sh
--rwxrwxr-x   0 michielbron  (1000) michielbron  (1000)       84 2022-11-03 16:59:21.000000 python-allib-0.3.4.0/benchmark_dir.sh
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.097000 python-allib-0.3.4.0/docs/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      638 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/Makefile
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      799 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/make.bat
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/docs/source/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3027 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.activelearning.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1163 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.analysis.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1327 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.balancing.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      996 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.environment.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1186 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.estimation.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      337 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.factory.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1571 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.feature_extraction.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      355 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.functions.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      477 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.history.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      987 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.instances.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      468 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.labels.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      904 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.machinelearning.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      635 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.module.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      607 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1229 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/allib.utils.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2893 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/conf.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      988 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/index.rst
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/docs/source/introduction/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       47 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/introduction/about.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       23 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/introduction/components.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1419 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/introduction/installation.rst
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       52 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/docs/source/modules.rst
-drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/python_allib.egg-info/
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      488 2023-03-31 14:47:22.000000 python-allib-0.3.4.0/python_allib.egg-info/PKG-INFO
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5251 2023-03-31 14:47:22.000000 python-allib-0.3.4.0/python_allib.egg-info/SOURCES.txt
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        1 2023-03-31 14:47:22.000000 python-allib-0.3.4.0/python_allib.egg-info/dependency_links.txt
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      170 2023-03-31 14:47:22.000000 python-allib-0.3.4.0/python_allib.egg-info/requires.txt
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        6 2023-03-31 14:47:22.000000 python-allib-0.3.4.0/python_allib.egg-info/top_level.txt
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      152 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/requirements.txt
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       38 2023-03-31 14:47:22.100999 python-allib-0.3.4.0/setup.cfg
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1809 2023-03-31 14:38:20.000000 python-allib-0.3.4.0/setup.py
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      259 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/tox.ini
--rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       60 2021-11-03 17:48:02.000000 python-allib-0.3.4.0/workspace.code-workspace
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.020179 python-allib-0.3.5.0/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7651 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/LICENSE
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      488 2023-04-07 22:16:35.020179 python-allib-0.3.5.0/PKG-INFO
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/README.md
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.980179 python-allib-0.3.5.0/allib/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       96 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2019 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/__main__.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.988180 python-allib-0.3.5.0/allib/activelearning/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      234 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/activelearning/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9998 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/ats.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7291 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/autostop.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11146 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/autotar.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3410 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/autotarensemble.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9002 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1469 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     9293 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/ensembles.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4018 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/estimator.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    14632 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1111 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/fixed.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/activelearning/helperfunctions.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    15492 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/insclass.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4697 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/labelmethods.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4486 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/learnersequence.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    16302 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/ml_based.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2228 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/mostcertain.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2191 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/activelearning/oracles.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5556 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/poolbased.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10769 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/prob_ensembles.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3222 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/qbc.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      416 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/random.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      815 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/selectioncriterion.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2840 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/sequence.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1652 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/activelearning/synthetictrain.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1418 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/target.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4824 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/tsvm.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2893 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/activelearning/uncertainty.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.992179 python-allib-0.3.5.0/allib/analysis/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/analysis/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8466 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/analysis.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8679 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7853 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/classificationplotter.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10456 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/experiments.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7435 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/initialization.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5564 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/plotter.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     7213 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/simulation.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4736 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/statistics.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2563 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/summarize.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6516 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/tablecollector.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    15875 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/analysis/tarplotter.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2997 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/app.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.996179 python-allib-0.3.5.0/allib/balancing/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      253 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/balancing/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1484 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/balancing/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      223 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/balancing/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5563 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/balancing/double.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1106 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/balancing/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      707 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/balancing/randomoversampling.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8651 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/balancing/triple.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2752 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/balancing/undersample.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.996179 python-allib-0.3.5.0/allib/benchmarking/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/benchmarking/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      958 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/benchmarking/datasets.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3781 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/benchmarking/reviews.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:34.996179 python-allib-0.3.5.0/allib/configurations/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      100 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/configurations/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11519 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/configurations/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1812 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/configurations/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    17776 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/configurations/ensemble.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      626 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/configurations/tarbaselines.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.000179 python-allib-0.3.5.0/allib/environment/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      158 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/environment/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3073 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/environment/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      124 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/environment/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      618 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/environment/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5839 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/environment/hdf5.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11221 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/environment/memory.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.000179 python-allib-0.3.5.0/allib/estimation/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/estimation/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4241 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/autostop.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1292 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8776 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/loglinear.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1127 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/mhmodel.R
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8693 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/mhmodel.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    18610 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rasch.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    17839 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rasch_comb_parametric.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    42067 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rasch_multiple.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     5469 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rasch_parametric.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12015 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rasch_python.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12830 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/rcapture.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4772 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/estimation/semi.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.004179 python-allib-0.3.5.0/allib/exceptions/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      107 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/exceptions/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      823 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/exceptions/base.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.004179 python-allib-0.3.5.0/allib/factory/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       66 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/factory/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1795 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/factory/factory.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.008180 python-allib-0.3.5.0/allib/feature_extraction/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      193 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/feature_extraction/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    11513 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/feature_extraction/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      445 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/feature_extraction/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1718 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/feature_extraction/contextinstance.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2740 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/feature_extraction/doc2vec.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3566 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/feature_extraction/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1200 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/feature_extraction/textinstance.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1530 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/feature_extraction/textsklearn.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.008180 python-allib-0.3.5.0/allib/history/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       61 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/history/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1369 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/history/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6083 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/history/memory.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.008180 python-allib-0.3.5.0/allib/machinelearning/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      214 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/machinelearning/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3659 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/balanced_il.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2168 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      562 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4830 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     6199 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/sklearn.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    20600 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/sparse.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    13318 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/taroptimized.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.012179 python-allib-0.3.5.0/allib/machinelearning/transductive/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/transductive/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1028 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/transductive/il_tsvm.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    37551 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/transductive/qns3vm.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4839 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/machinelearning/transductive/tsvm_sklearn.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.012179 python-allib-0.3.5.0/allib/module/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      101 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/module/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      563 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/module/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      317 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/module/component.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      495 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/module/factory.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/py.typed
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.016179 python-allib-0.3.5.0/allib/stopcriterion/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        0 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/stopcriterion/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      748 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/stopcriterion/apriori.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      854 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/stopcriterion/base.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      181 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/stopcriterion/catalog.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    10960 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/stopcriterion/estimation.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3959 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/stopcriterion/heuristic.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     8296 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/stopcriterion/others.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1319 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/stopcriterion/target.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.016179 python-allib-0.3.5.0/allib/typehints/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      137 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/typehints/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1407 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/typehints/typevars.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.020179 python-allib-0.3.5.0/allib/utils/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      191 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/__init__.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1454 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/chunks.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)    12439 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/utils/func.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      217 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/utils/io.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     3258 2023-04-07 21:20:09.000000 python-allib-0.3.5.0/allib/utils/numpy.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2589 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/producer_consumer.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      288 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/random.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     2688 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/saveablemodel.py
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      714 2022-05-12 10:36:06.000000 python-allib-0.3.5.0/allib/utils/to_key.py
+drwxrwxr-x   0 michielbron  (1000) michielbron  (1000)        0 2023-04-07 22:16:35.020179 python-allib-0.3.5.0/python_allib.egg-info/
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      488 2023-04-07 22:16:34.000000 python-allib-0.3.5.0/python_allib.egg-info/PKG-INFO
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     4174 2023-04-07 22:16:34.000000 python-allib-0.3.5.0/python_allib.egg-info/SOURCES.txt
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        1 2023-04-07 22:16:34.000000 python-allib-0.3.5.0/python_allib.egg-info/dependency_links.txt
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)      191 2023-04-07 22:16:34.000000 python-allib-0.3.5.0/python_allib.egg-info/requires.txt
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)        6 2023-04-07 22:16:34.000000 python-allib-0.3.5.0/python_allib.egg-info/top_level.txt
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)       38 2023-04-07 22:16:35.020179 python-allib-0.3.5.0/setup.cfg
+-rw-rw-r--   0 michielbron  (1000) michielbron  (1000)     1851 2023-04-07 22:15:46.000000 python-allib-0.3.5.0/setup.py
```

### Comparing `python-allib-0.3.4.0/LICENSE` & `python-allib-0.3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/__main__.py` & `python-allib-0.3.5.0/allib/__main__.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/ats.py` & `python-allib-0.3.5.0/allib/activelearning/ats.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/autostop.py` & `python-allib-0.3.5.0/allib/activelearning/autostop.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/autotar.py` & `python-allib-0.3.5.0/allib/activelearning/autotar.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/autotarensemble.py` & `python-allib-0.3.5.0/allib/activelearning/autotarensemble.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/base.py` & `python-allib-0.3.5.0/allib/activelearning/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/catalog.py` & `python-allib-0.3.5.0/allib/activelearning/catalog.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/ensembles.py` & `python-allib-0.3.5.0/allib/activelearning/ensembles.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/estimator.py` & `python-allib-0.3.5.0/allib/activelearning/estimator.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/factory.py` & `python-allib-0.3.5.0/allib/activelearning/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/fixed.py` & `python-allib-0.3.5.0/allib/activelearning/fixed.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/insclass.py` & `python-allib-0.3.5.0/allib/activelearning/insclass.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/labelmethods.py` & `python-allib-0.3.5.0/allib/activelearning/labelmethods.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/learnersequence.py` & `python-allib-0.3.5.0/allib/activelearning/learnersequence.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/ml_based.py` & `python-allib-0.3.5.0/allib/activelearning/ml_based.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/mostcertain.py` & `python-allib-0.3.5.0/allib/activelearning/mostcertain.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/oracles.py` & `python-allib-0.3.5.0/allib/activelearning/oracles.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/poolbased.py` & `python-allib-0.3.5.0/allib/activelearning/poolbased.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/prob_ensembles.py` & `python-allib-0.3.5.0/allib/activelearning/prob_ensembles.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/qbc.py` & `python-allib-0.3.5.0/allib/activelearning/qbc.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/selectioncriterion.py` & `python-allib-0.3.5.0/allib/activelearning/selectioncriterion.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/sequence.py` & `python-allib-0.3.5.0/allib/activelearning/sequence.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/synthetictrain.py` & `python-allib-0.3.5.0/allib/activelearning/synthetictrain.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/target.py` & `python-allib-0.3.5.0/allib/activelearning/target.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/tsvm.py` & `python-allib-0.3.5.0/allib/activelearning/tsvm.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/activelearning/uncertainty.py` & `python-allib-0.3.5.0/allib/activelearning/uncertainty.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/analysis.py` & `python-allib-0.3.5.0/allib/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/base.py` & `python-allib-0.3.5.0/allib/analysis/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/classificationplotter.py` & `python-allib-0.3.5.0/allib/analysis/classificationplotter.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/experiments.py` & `python-allib-0.3.5.0/allib/analysis/experiments.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/initialization.py` & `python-allib-0.3.5.0/allib/analysis/initialization.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/plotter.py` & `python-allib-0.3.5.0/allib/analysis/plotter.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/simulation.py` & `python-allib-0.3.5.0/allib/analysis/simulation.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/statistics.py` & `python-allib-0.3.5.0/allib/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/summarize.py` & `python-allib-0.3.5.0/allib/analysis/summarize.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/tablecollector.py` & `python-allib-0.3.5.0/allib/analysis/tablecollector.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/analysis/tarplotter.py` & `python-allib-0.3.5.0/allib/analysis/tarplotter.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/app.py` & `python-allib-0.3.5.0/allib/app.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/base.py` & `python-allib-0.3.5.0/allib/balancing/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/double.py` & `python-allib-0.3.5.0/allib/balancing/double.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/factory.py` & `python-allib-0.3.5.0/allib/balancing/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/randomoversampling.py` & `python-allib-0.3.5.0/allib/balancing/randomoversampling.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/triple.py` & `python-allib-0.3.5.0/allib/balancing/triple.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/balancing/undersample.py` & `python-allib-0.3.5.0/allib/balancing/undersample.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/benchmarking/datasets.py` & `python-allib-0.3.5.0/allib/benchmarking/datasets.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/benchmarking/reviews.py` & `python-allib-0.3.5.0/allib/benchmarking/reviews.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/configurations/base.py` & `python-allib-0.3.5.0/allib/configurations/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/configurations/catalog.py` & `python-allib-0.3.5.0/allib/configurations/catalog.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/configurations/ensemble.py` & `python-allib-0.3.5.0/allib/configurations/ensemble.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/configurations/tarbaselines.py` & `python-allib-0.3.5.0/allib/configurations/tarbaselines.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/environment/base.py` & `python-allib-0.3.5.0/allib/environment/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/environment/factory.py` & `python-allib-0.3.5.0/allib/environment/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/environment/hdf5.py` & `python-allib-0.3.5.0/allib/environment/hdf5.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/environment/memory.py` & `python-allib-0.3.5.0/allib/environment/memory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/autostop.py` & `python-allib-0.3.5.0/allib/estimation/autostop.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/base.py` & `python-allib-0.3.5.0/allib/estimation/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/loglinear.py` & `python-allib-0.3.5.0/allib/estimation/loglinear.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/mhmodel.R` & `python-allib-0.3.5.0/allib/estimation/mhmodel.R`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/mhmodel.py` & `python-allib-0.3.5.0/allib/estimation/mhmodel.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rasch.py` & `python-allib-0.3.5.0/allib/estimation/rasch.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rasch_comb_parametric.py` & `python-allib-0.3.5.0/allib/estimation/rasch_comb_parametric.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rasch_multiple.py` & `python-allib-0.3.5.0/allib/estimation/rasch_multiple.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rasch_parametric.py` & `python-allib-0.3.5.0/allib/estimation/rasch_parametric.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rasch_python.py` & `python-allib-0.3.5.0/allib/estimation/rasch_python.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/rcapture.py` & `python-allib-0.3.5.0/allib/estimation/rcapture.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/estimation/semi.py` & `python-allib-0.3.5.0/allib/estimation/semi.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/exceptions/base.py` & `python-allib-0.3.5.0/allib/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/factory/factory.py` & `python-allib-0.3.5.0/allib/factory/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/base.py` & `python-allib-0.3.5.0/allib/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/contextinstance.py` & `python-allib-0.3.5.0/allib/feature_extraction/contextinstance.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/doc2vec.py` & `python-allib-0.3.5.0/allib/feature_extraction/doc2vec.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/factory.py` & `python-allib-0.3.5.0/allib/feature_extraction/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/textinstance.py` & `python-allib-0.3.5.0/allib/feature_extraction/textinstance.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/feature_extraction/textsklearn.py` & `python-allib-0.3.5.0/allib/feature_extraction/textsklearn.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/history/base.py` & `python-allib-0.3.5.0/allib/history/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/history/memory.py` & `python-allib-0.3.5.0/allib/history/memory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/balanced_il.py` & `python-allib-0.3.5.0/allib/machinelearning/balanced_il.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/base.py` & `python-allib-0.3.5.0/allib/machinelearning/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/catalog.py` & `python-allib-0.3.5.0/allib/machinelearning/catalog.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/factory.py` & `python-allib-0.3.5.0/allib/machinelearning/factory.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/sklearn.py` & `python-allib-0.3.5.0/allib/machinelearning/sklearn.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/sparse.py` & `python-allib-0.3.5.0/allib/machinelearning/sparse.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/taroptimized.py` & `python-allib-0.3.5.0/allib/machinelearning/taroptimized.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/transductive/il_tsvm.py` & `python-allib-0.3.5.0/allib/machinelearning/transductive/il_tsvm.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/transductive/qns3vm.py` & `python-allib-0.3.5.0/allib/machinelearning/transductive/qns3vm.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/machinelearning/transductive/tsvm_sklearn.py` & `python-allib-0.3.5.0/allib/machinelearning/transductive/tsvm_sklearn.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/module/catalog.py` & `python-allib-0.3.5.0/allib/module/catalog.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/apriori.py` & `python-allib-0.3.5.0/allib/stopcriterion/apriori.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/base.py` & `python-allib-0.3.5.0/allib/stopcriterion/base.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/estimation.py` & `python-allib-0.3.5.0/allib/stopcriterion/estimation.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/heuristic.py` & `python-allib-0.3.5.0/allib/stopcriterion/heuristic.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/others.py` & `python-allib-0.3.5.0/allib/stopcriterion/others.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/stopcriterion/target.py` & `python-allib-0.3.5.0/allib/stopcriterion/target.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/typehints/typevars.py` & `python-allib-0.3.5.0/allib/typehints/typevars.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/chunks.py` & `python-allib-0.3.5.0/allib/utils/chunks.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/func.py` & `python-allib-0.3.5.0/allib/utils/func.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/numpy.py` & `python-allib-0.3.5.0/allib/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/producer_consumer.py` & `python-allib-0.3.5.0/allib/utils/producer_consumer.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/saveablemodel.py` & `python-allib-0.3.5.0/allib/utils/saveablemodel.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/allib/utils/to_key.py` & `python-allib-0.3.5.0/allib/utils/to_key.py`

 * *Files identical despite different names*

### Comparing `python-allib-0.3.4.0/setup.py` & `python-allib-0.3.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setuptools.setup(  # type: ignore
     name="python-allib",
-    version="0.3.4.0",  # NOSONAR
+    version="0.3.5.0",  # NOSONAR
     description="A typed Active Learning Library",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Michiel Bron",
     author_email="m.p.bron@uu.nl",
     license="GNU LGPL v3",
     classifiers=[
@@ -47,10 +47,12 @@
         "instancelib",
         "imblearn",
         "lightgbm",
         "gensim",
         "more-itertools",
         "matplotlib",
         "typing_extensions>=4.4.0",
+        "pylatex",
+        "scienceplots"
     ],
     extras_require={"doc2vec": ["gensim"]},
 )
```

