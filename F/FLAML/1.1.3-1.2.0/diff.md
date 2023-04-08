# Comparing `tmp/FLAML-1.1.3.tar.gz` & `tmp/FLAML-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.1.3.tar", last modified: Wed Mar  1 21:35:09 2023, max compression
+gzip compressed data, was "FLAML-1.2.0.tar", last modified: Sat Apr  8 18:29:51 2023, max compression
```

## Comparing `FLAML-1.1.3.tar` & `FLAML-1.2.0.tar`

### file list

```diff
@@ -1,109 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.865531 FLAML-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.857531 FLAML-1.1.3/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-03-01 21:35:09.000000 FLAML-1.1.3/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-01 21:35:09.000000 FLAML-1.1.3/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 21:35:09.000000 FLAML-1.1.3/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-01 21:35:09.000000 FLAML-1.1.3/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 21:35:09.000000 FLAML-1.1.3/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-01 21:34:15.000000 FLAML-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-03-01 21:34:15.000000 FLAML-1.1.3/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-03-01 21:35:09.865531 FLAML-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-03-01 21:34:15.000000 FLAML-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.857531 FLAML-1.1.3/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.857531 FLAML-1.1.3/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   177345 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26666 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    89832 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.857531 FLAML-1.1.3/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.857531 FLAML-1.1.3/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21611 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/default/xgboost/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/integrations/oai/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/integrations/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/integrations/oai/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.861531 FLAML-1.1.3/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.865531 FLAML-1.1.3/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.865531 FLAML-1.1.3/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    32267 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.865531 FLAML-1.1.3/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    36898 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 21:34:15.000000 FLAML-1.1.3/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 21:35:09.865531 FLAML-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-01 21:34:15.000000 FLAML-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 21:35:09.865531 FLAML-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-03-01 21:34:15.000000 FLAML-1.1.3/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-01 21:34:15.000000 FLAML-1.1.3/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-01 21:34:15.000000 FLAML-1.1.3/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-01 21:34:15.000000 FLAML-1.1.3/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-01 21:34:15.000000 FLAML-1.1.3/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.743425 FLAML-1.2.0/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-08 18:28:47.000000 FLAML-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-08 18:28:47.000000 FLAML-1.2.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-04-08 18:29:51.755425 FLAML-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-08 18:28:47.000000 FLAML-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37455 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/oai/completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132360 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107198 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46906 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32267 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:29:51.755425 FLAML-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-08 18:28:47.000000 FLAML-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_version.py
```

### Comparing `FLAML-1.1.3/FLAML.egg-info/PKG-INFO` & `FLAML-1.2.0/FLAML.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.1.3
+Version: 1.2.0
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Provides-Extra: test
 Provides-Extra: catboost
 Provides-Extra: blendsearch
 Provides-Extra: ray
 Provides-Extra: azureml
 Provides-Extra: nni
 Provides-Extra: vw
+Provides-Extra: hf
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: synapse
 License-File: LICENSE
@@ -40,28 +41,30 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: An [upcoming tutorial on FLAML](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) at [AAAI-23](https://aaai.org/Conferences/AAAI-23/aaai23tutorials/) (to be held on Feb 08, 2023)
+:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+
+:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
 learning models automatically, efficiently and economically. It frees users from selecting
-learners and hyperparameters for each learner. It can also be used to tune generic hyperparameters for MLOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
+models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
 
-1. For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It supports both classifcal machine learning models and deep neural networks.
+1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
 1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
 1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
-and learner selection method invented by Microsoft Research.
+and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
 
 ### Python
@@ -119,14 +122,30 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
```

### Comparing `FLAML-1.1.3/FLAML.egg-info/SOURCES.txt` & `FLAML-1.2.0/FLAML.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,43 @@
 FLAML.egg-info/top_level.txt
 flaml/__init__.py
 flaml/config.py
 flaml/data.py
 flaml/ml.py
 flaml/model.py
 flaml/version.py
+flaml/autogen/__init__.py
+flaml/autogen/code_utils.py
+flaml/autogen/math_utils.py
+flaml/autogen/oai/__init__.py
+flaml/autogen/oai/completion.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
 flaml/automl/data.py
+flaml/automl/logger.py
 flaml/automl/ml.py
 flaml/automl/model.py
+flaml/automl/state.py
 flaml/automl/training_log.py
+flaml/automl/utils.py
 flaml/automl/nlp/__init__.py
 flaml/automl/nlp/utils.py
 flaml/automl/nlp/huggingface/__init__.py
 flaml/automl/nlp/huggingface/data_collator.py
 flaml/automl/nlp/huggingface/trainer.py
 flaml/automl/nlp/huggingface/training_args.py
 flaml/automl/nlp/huggingface/utils.py
+flaml/automl/spark/__init__.py
+flaml/automl/spark/configs.py
+flaml/automl/spark/metrics.py
+flaml/automl/spark/utils.py
+flaml/automl/task/__init__.py
+flaml/automl/task/factory.py
+flaml/automl/task/generic_task.py
+flaml/automl/task/task.py
 flaml/default/__init__.py
 flaml/default/estimator.py
 flaml/default/greedy.py
 flaml/default/portfolio.py
 flaml/default/regret.py
 flaml/default/suggest.py
 flaml/default/all/binary.json
@@ -46,17 +62,14 @@
 flaml/default/rf/regression.json
 flaml/default/xgb_limitdepth/binary.json
 flaml/default/xgb_limitdepth/multiclass.json
 flaml/default/xgb_limitdepth/regression.json
 flaml/default/xgboost/binary.json
 flaml/default/xgboost/multiclass.json
 flaml/default/xgboost/regression.json
-flaml/integrations/__init__.py
-flaml/integrations/oai/__init__.py
-flaml/integrations/oai/completion.py
 flaml/onlineml/__init__.py
 flaml/onlineml/autovw.py
 flaml/onlineml/trial.py
 flaml/onlineml/trial_runner.py
 flaml/tune/__init__.py
 flaml/tune/analysis.py
 flaml/tune/result.py
```

### Comparing `FLAML-1.1.3/FLAML.egg-info/requires.txt` & `FLAML-1.2.0/FLAML.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 [forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
 pytorch-forecasting>=0.9.0
 
+[hf]
+transformers[torch]==4.26
+datasets
+nltk
+rouge_score
+seqeval
+
 [nlp]
 transformers[torch]==4.26
 datasets
 nltk
 rouge_score
 seqeval
 
@@ -38,29 +45,29 @@
 
 [notebook]
 jupyter
 matplotlib
 openml==0.10.2
 
 [openai]
-openai==0.23.1
+openai==0.27.4
 diskcache
 optuna==2.8.0
 
 [ray]
 ray[tune]~=1.13
 
 [spark]
-pyspark>=3.0.0
+pyspark>=3.2.0
 joblibspark>=0.5.0
 
 [synapse]
 joblibspark>=0.5.0
 optuna==2.8.0
-pyspark>=3.0.0
+pyspark>=3.2.0
 
 [test]
 flake8>=3.8.4
 thop
 pytest>=6.1.1
 coverage>=5.3
 pre-commit
@@ -77,15 +84,15 @@
 datasets
 nltk
 rouge_score
 hcrystalball==0.1.10
 seqeval
 pytorch-forecasting<=0.10.1,>=0.9.0
 mlflow
-pyspark>=3.0.0
+pyspark>=3.2.0
 joblibspark>=0.5.0
 nbconvert
 nbformat
 ipykernel
 pytorch-lightning<1.9.1
 
 [ts_forecast]
```

### Comparing `FLAML-1.1.3/LICENSE` & `FLAML-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/NOTICE.md` & `FLAML-1.2.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/PKG-INFO` & `FLAML-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.1.3
+Version: 1.2.0
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Provides-Extra: test
 Provides-Extra: catboost
 Provides-Extra: blendsearch
 Provides-Extra: ray
 Provides-Extra: azureml
 Provides-Extra: nni
 Provides-Extra: vw
+Provides-Extra: hf
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
 Provides-Extra: synapse
 License-File: LICENSE
@@ -40,28 +41,30 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: An [upcoming tutorial on FLAML](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) at [AAAI-23](https://aaai.org/Conferences/AAAI-23/aaai23tutorials/) (to be held on Feb 08, 2023)
+:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+
+:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
 learning models automatically, efficiently and economically. It frees users from selecting
-learners and hyperparameters for each learner. It can also be used to tune generic hyperparameters for MLOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
+models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
 
-1. For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It supports both classifcal machine learning models and deep neural networks.
+1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
 1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
 1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
-and learner selection method invented by Microsoft Research.
+and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
 
 ### Python
@@ -119,14 +122,30 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
```

### Comparing `FLAML-1.1.3/README.md` & `FLAML-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: An [upcoming tutorial on FLAML](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) at [AAAI-23](https://aaai.org/Conferences/AAAI-23/aaai23tutorials/) (to be held on Feb 08, 2023)
+:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+
+:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
 learning models automatically, efficiently and economically. It frees users from selecting
-learners and hyperparameters for each learner. It can also be used to tune generic hyperparameters for MLOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
+models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
 
-1. For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources. It supports both classifcal machine learning models and deep neural networks.
+1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
 1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
 1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
-and learner selection method invented by Microsoft Research.
+and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
 
 ### Python
@@ -89,14 +91,30 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
```

### Comparing `FLAML-1.1.3/flaml/automl/automl.py` & `FLAML-1.2.0/flaml/automl/automl.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,72 +2,76 @@
 #  * Copyright (c) FLAML authors. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
 from __future__ import annotations
 import time
 import os
 import sys
-from typing import Callable, Optional, List, Union, Any
-import inspect
+from typing import Callable, List, Union, Optional
 from functools import partial
 import numpy as np
-from scipy.sparse import issparse
-from sklearn.model_selection import (
-    train_test_split,
-    RepeatedStratifiedKFold,
-    RepeatedKFold,
-    GroupKFold,
-    TimeSeriesSplit,
-    GroupShuffleSplit,
-    StratifiedGroupKFold,
-)
-from sklearn.utils import shuffle
 from sklearn.base import BaseEstimator
 import pandas as pd
 import logging
 import json
+
+from flaml.automl.state import SearchState, AutoMLState
 from flaml.automl.ml import (
-    compute_estimator,
     train_estimator,
     get_estimator_class,
-    get_classification_objective,
 )
 from flaml.config import (
     MIN_SAMPLE_TRAIN,
     MEM_THRES,
     RANDOM_SEED,
     SMALL_LARGE_THRES,
     CV_HOLDOUT_THRESHOLD,
     SPLIT_RATIO,
     N_SPLITS,
     SAMPLE_MULTIPLY_FACTOR,
 )
-from flaml.automl.data import (
-    concat,
-    CLASSIFICATION,
-    TOKENCLASSIFICATION,
-    TS_FORECAST,
-    TS_FORECASTREGRESSION,
-    TS_FORECASTPANEL,
-    TS_TIMESTAMP_COL,
-    REGRESSION,
-    _is_nlp_task,
-    NLG_TASKS,
-)
+
+# TODO check to see when we can remove these
+from flaml.automl.task.task import CLASSIFICATION, TS_FORECAST, Task
+from flaml.automl.task.factory import task_factory
 from flaml import tune
+from flaml.automl.logger import logger, logger_formatter
 from flaml.automl.training_log import training_log_reader, training_log_writer
 from flaml.default import suggest_learner
 from flaml.version import __version__ as flaml_version
 from flaml.tune.spark.utils import check_spark, get_broadcast_data
 
-logger = logging.getLogger(__name__)
-logger_formatter = logging.Formatter(
-    "[%(name)s: %(asctime)s] {%(lineno)d} %(levelname)s - %(message)s", "%m-%d %H:%M:%S"
-)
-logger.propagate = False
+try:
+    from flaml.automl.spark.utils import (
+        train_test_split_pyspark,
+        unique_pandas_on_spark,
+        len_labels,
+        unique_value_first_index,
+    )
+except ImportError:
+    train_test_split_pyspark = None
+    unique_pandas_on_spark = None
+    from flaml.automl.utils import (
+        len_labels,
+        unique_value_first_index,
+    )
+try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
+    import pyspark.pandas as ps
+    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+    from pyspark.pandas.config import set_option, reset_option
+except ImportError:
+    ps = None
+
+    class psDataFrame:
+        pass
+
+    class psSeries:
+        pass
+
 
 try:
     import mlflow
 except ImportError:
     mlflow = None
 
 try:
@@ -76,429 +80,14 @@
     assert ray_version >= "1.10.0"
 
     ray_available = True
 except (ImportError, AssertionError):
     ray_available = False
 
 
-class SearchState:
-    @property
-    def search_space(self):
-        return self._search_space_domain
-
-    @property
-    def estimated_cost4improvement(self):
-        return max(
-            self.time_best_found - self.time_best_found_old,
-            self.total_time_used - self.time_best_found,
-        )
-
-    def valid_starting_point_one_dim(self, value_one_dim, domain_one_dim):
-        from flaml.tune.space import sample
-
-        """
-            For each hp in the starting point, check the following 3 conditions:
-            (1) If the type of the starting point does not match the required type in search space, return false
-            (2) If the starting point is not in the required search space, return false
-            (3) If the search space is a value instead of domain, and the value is not equal to the starting point
-            Notice (2) include the case starting point not in user specified search space custom_hp
-        """
-        if isinstance(domain_one_dim, sample.Domain):
-            renamed_type = list(
-                inspect.signature(domain_one_dim.is_valid).parameters.values()
-            )[0].annotation
-            type_match = (
-                renamed_type == Any
-                or isinstance(value_one_dim, renamed_type)
-                or isinstance(value_one_dim, int)
-                and renamed_type is float
-            )
-            if not (type_match and domain_one_dim.is_valid(value_one_dim)):
-                return False
-        elif value_one_dim != domain_one_dim:
-            return False
-        return True
-
-    def valid_starting_point(self, starting_point, search_space):
-        return all(
-            self.valid_starting_point_one_dim(value, search_space[name].get("domain"))
-            for name, value in starting_point.items()
-            if name != "FLAML_sample_size"
-        )
-
-    def __init__(
-        self,
-        learner_class,
-        data_size,
-        task,
-        starting_point=None,
-        period=None,
-        custom_hp=None,
-        max_iter=None,
-        budget=None,
-    ):
-        self.init_eci = learner_class.cost_relative2lgbm() if budget >= 0 else 1
-        self._search_space_domain = {}
-        self.init_config = None
-        self.low_cost_partial_config = {}
-        self.cat_hp_cost = {}
-        self.data_size = data_size
-        self.ls_ever_converged = False
-        self.learner_class = learner_class
-        self._budget = budget
-        if task in TS_FORECAST:
-            search_space = learner_class.search_space(
-                data_size=data_size, task=task, pred_horizon=period
-            )
-        else:
-            search_space = learner_class.search_space(data_size=data_size, task=task)
-
-        if custom_hp is not None:
-            search_space.update(custom_hp)
-
-        if isinstance(starting_point, dict):
-            starting_point = AutoMLState.sanitize(starting_point)
-            if max_iter > 1 and not self.valid_starting_point(
-                starting_point, search_space
-            ):
-                # If the number of iterations is larger than 1, remove invalid point
-                logger.warning(
-                    "Starting point {} removed because it is outside of the search space".format(
-                        starting_point
-                    )
-                )
-                starting_point = None
-        elif isinstance(starting_point, list):
-            starting_point = [AutoMLState.sanitize(x) for x in starting_point]
-            if max_iter > len(starting_point):
-                # If the number of starting points is no smaller than max iter, avoid the checking
-                starting_point_len = len(starting_point)
-                starting_point = [
-                    x
-                    for x in starting_point
-                    if self.valid_starting_point(x, search_space)
-                ]
-                if starting_point_len > len(starting_point):
-                    logger.warning(
-                        "Starting points outside of the search space are removed. "
-                        f"Remaining starting points for {learner_class}: {starting_point}"
-                    )
-                starting_point = starting_point or None
-
-        for name, space in search_space.items():
-            assert (
-                "domain" in space
-            ), f"{name}'s domain is missing in the search space spec {space}"
-            if space["domain"] is None:
-                # don't search this hp
-                continue
-            self._search_space_domain[name] = space["domain"]
-
-            if "low_cost_init_value" in space:
-                self.low_cost_partial_config[name] = space["low_cost_init_value"]
-            if "cat_hp_cost" in space:
-                self.cat_hp_cost[name] = space["cat_hp_cost"]
-            # if a starting point is provided, set the init config to be
-            # the starting point provided
-            if (
-                isinstance(starting_point, dict)
-                and starting_point.get(name) is not None
-            ):
-                if self.init_config is None:
-                    self.init_config = {}
-                self.init_config[name] = starting_point[name]
-            elif (
-                not isinstance(starting_point, list)
-                and "init_value" in space
-                and self.valid_starting_point_one_dim(
-                    space["init_value"], space["domain"]
-                )
-            ):
-                if self.init_config is None:
-                    self.init_config = {}
-                self.init_config[name] = space["init_value"]
-
-        if isinstance(starting_point, list):
-            self.init_config = starting_point
-        else:
-            self.init_config = [] if self.init_config is None else [self.init_config]
-
-        self._hp_names = list(self._search_space_domain.keys())
-        self.search_alg = None
-        self.best_config = None
-        self.best_result = None
-        self.best_loss = self.best_loss_old = np.inf
-        self.total_time_used = 0
-        self.total_iter = 0
-        self.base_eci = None
-        self.time_best_found = self.time_best_found_old = 0
-        self.time2eval_best = 0
-        self.time2eval_best_old = 0
-        self.trained_estimator = None
-        self.sample_size = None
-        self.trial_time = 0
-
-    def update(self, result, time_used):
-        if result:
-            config = result["config"]
-            if config and "FLAML_sample_size" in config:
-                self.sample_size = config["FLAML_sample_size"]
-            else:
-                self.sample_size = self.data_size[0]
-            obj = result["val_loss"]
-            metric_for_logging = result["metric_for_logging"]
-            time2eval = result["time_total_s"]
-            trained_estimator = result["trained_estimator"]
-            del result["trained_estimator"]  # free up RAM
-            n_iter = (
-                trained_estimator
-                and hasattr(trained_estimator, "ITER_HP")
-                and trained_estimator.params.get(trained_estimator.ITER_HP)
-            )
-            if n_iter:
-                if "ml" in config:
-                    config["ml"][trained_estimator.ITER_HP] = n_iter
-                else:
-                    config[trained_estimator.ITER_HP] = n_iter
-        else:
-            obj, time2eval, trained_estimator = np.inf, 0.0, None
-            metric_for_logging = config = None
-        self.trial_time = time2eval
-        self.total_time_used += time_used if self._budget >= 0 else 1
-        self.total_iter += 1
-
-        if self.base_eci is None:
-            self.base_eci = time_used
-        if (obj is not None) and (obj < self.best_loss):
-            self.best_loss_old = self.best_loss if self.best_loss < np.inf else 2 * obj
-            self.best_loss = obj
-            self.best_result = result
-            self.time_best_found_old = self.time_best_found
-            self.time_best_found = self.total_time_used
-            self.iter_best_found = self.total_iter
-            self.best_config = config
-            self.best_config_sample_size = self.sample_size
-            self.best_config_train_time = time_used
-            if time2eval:
-                self.time2eval_best_old = self.time2eval_best
-                self.time2eval_best = time2eval
-            if (
-                self.trained_estimator
-                and trained_estimator
-                and self.trained_estimator != trained_estimator
-            ):
-                self.trained_estimator.cleanup()
-            if trained_estimator:
-                self.trained_estimator = trained_estimator
-        elif trained_estimator:
-            trained_estimator.cleanup()
-        self.metric_for_logging = metric_for_logging
-        self.val_loss, self.config = obj, config
-
-    def get_hist_config_sig(self, sample_size, config):
-        config_values = tuple([config[k] for k in self._hp_names if k in config])
-        config_sig = str(sample_size) + "_" + str(config_values)
-        return config_sig
-
-    def est_retrain_time(self, retrain_sample_size):
-        assert (
-            self.best_config_sample_size is not None
-        ), "need to first get best_config_sample_size"
-        return self.time2eval_best * retrain_sample_size / self.best_config_sample_size
-
-
-class AutoMLState:
-    def _prepare_sample_train_data(self, sample_size: int):
-        sampled_weight = groups = None
-        if sample_size <= self.data_size[0]:
-            if isinstance(self.X_train, pd.DataFrame):
-                sampled_X_train = self.X_train.iloc[:sample_size]
-            else:
-                sampled_X_train = self.X_train[:sample_size]
-            if isinstance(self.y_train, pd.Series):
-                sampled_y_train = self.y_train.iloc[:sample_size]
-            else:
-                sampled_y_train = self.y_train[:sample_size]
-            weight = self.fit_kwargs.get(
-                "sample_weight"
-            )  # NOTE: _prepare_sample_train_data is before kwargs is updated to fit_kwargs_by_estimator
-            if weight is not None:
-                sampled_weight = (
-                    weight.iloc[:sample_size]
-                    if isinstance(weight, pd.Series)
-                    else weight[:sample_size]
-                )
-            if self.groups is not None:
-                groups = (
-                    self.groups.iloc[:sample_size]
-                    if isinstance(self.groups, pd.Series)
-                    else self.groups[:sample_size]
-                )
-        else:
-            sampled_X_train = self.X_train_all
-            sampled_y_train = self.y_train_all
-            if (
-                "sample_weight" in self.fit_kwargs
-            ):  # NOTE: _prepare_sample_train_data is before kwargs is updated to fit_kwargs_by_estimator
-                sampled_weight = self.sample_weight_all
-            if self.groups is not None:
-                groups = self.groups_all
-        return sampled_X_train, sampled_y_train, sampled_weight, groups
-
-    @staticmethod
-    def _compute_with_config_base(
-        config_w_resource: dict, state: AutoMLState, estimator: str, is_report: bool = True
-    ) -> dict:
-        if "FLAML_sample_size" in config_w_resource:
-            sample_size = int(config_w_resource["FLAML_sample_size"])
-        else:
-            sample_size = state.data_size[0]
-
-        this_estimator_kwargs = state.fit_kwargs_by_estimator.get(
-            estimator
-        ).copy()  # NOTE: _compute_with_config_base is after kwargs is updated to fit_kwargs_by_estimator
-        (
-            sampled_X_train,
-            sampled_y_train,
-            sampled_weight,
-            groups,
-        ) = state._prepare_sample_train_data(sample_size)
-        if sampled_weight is not None:
-            weight = this_estimator_kwargs["sample_weight"]
-            this_estimator_kwargs["sample_weight"] = sampled_weight
-        if groups is not None:
-            this_estimator_kwargs["groups"] = groups
-        config = config_w_resource.copy()
-        if "FLAML_sample_size" in config:
-            del config["FLAML_sample_size"]
-        budget = (
-            None
-            if state.time_budget < 0
-            else state.time_budget - state.time_from_start
-            if sample_size == state.data_size[0]
-            else (state.time_budget - state.time_from_start)
-            / 2
-            * sample_size
-            / state.data_size[0]
-        )
-
-        (
-            trained_estimator,
-            val_loss,
-            metric_for_logging,
-            _,
-            pred_time,
-        ) = compute_estimator(
-            sampled_X_train,
-            sampled_y_train,
-            state.X_val,
-            state.y_val,
-            state.weight_val,
-            state.groups_val,
-            state.train_time_limit
-            if budget is None
-            else min(budget, state.train_time_limit or np.inf),
-            state.kf,
-            config,
-            state.task,
-            estimator,
-            state.eval_method,
-            state.metric,
-            state.best_loss,
-            state.n_jobs,
-            state.learner_classes.get(estimator),
-            state.cv_score_agg_func,
-            state.log_training_metric,
-            this_estimator_kwargs,
-            state.free_mem_ratio,
-        )
-        if state.retrain_final and not state.model_history:
-            trained_estimator.cleanup()
-
-        result = {
-            "pred_time": pred_time,
-            "wall_clock_time": time.time() - state._start_time_flag,
-            "metric_for_logging": metric_for_logging,
-            "val_loss": val_loss,
-            "trained_estimator": trained_estimator,
-        }
-        if sampled_weight is not None:
-            this_estimator_kwargs["sample_weight"] = weight
-        if is_report is True:
-            tune.report(**result)
-        return result
-
-    @classmethod
-    def sanitize(cls, config: dict) -> dict:
-        """Make a config ready for passing to estimator."""
-        config = config.get("ml", config).copy()
-        config.pop("FLAML_sample_size", None)
-        config.pop("learner", None)
-        config.pop("_choice_", None)
-        return config
-
-    def _train_with_config(
-        self,
-        estimator: str,
-        config_w_resource: dict,
-        sample_size: Optional[int] = None,
-    ):
-        if not sample_size:
-            sample_size = config_w_resource.get(
-                "FLAML_sample_size", len(self.y_train_all)
-            )
-        config = AutoMLState.sanitize(config_w_resource)
-
-        this_estimator_kwargs = self.fit_kwargs_by_estimator.get(
-            estimator
-        ).copy()  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-        (
-            sampled_X_train,
-            sampled_y_train,
-            sampled_weight,
-            groups,
-        ) = self._prepare_sample_train_data(sample_size)
-        if sampled_weight is not None:
-            weight = this_estimator_kwargs[
-                "sample_weight"
-            ]  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-            this_estimator_kwargs[
-                "sample_weight"
-            ] = sampled_weight  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-        if groups is not None:
-            this_estimator_kwargs[
-                "groups"
-            ] = groups  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-
-        budget = (
-            None if self.time_budget < 0 else self.time_budget - self.time_from_start
-        )
-
-        estimator, train_time = train_estimator(
-            X_train=sampled_X_train,
-            y_train=sampled_y_train,
-            config_dic=config,
-            task=self.task,
-            estimator_name=estimator,
-            n_jobs=self.n_jobs,
-            estimator_class=self.learner_classes.get(estimator),
-            budget=budget,
-            fit_kwargs=this_estimator_kwargs,  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-            eval_metric=self.metric if hasattr(self, "metric") else "train_time",
-            free_mem_ratio=self.free_mem_ratio,
-        )
-
-        if sampled_weight is not None:
-            this_estimator_kwargs[
-                "sample_weight"
-            ] = weight  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
-
-        return estimator, train_time
-
-
 def size(learner_classes: dict, config: dict) -> float:
     """Size function.
 
     Returns:
         The mem size in bytes for a config.
     """
     config = config.get("ml", config)
@@ -572,15 +161,16 @@
                 "val_loss": val_loss,
                 "train_loss": train_loss,
                 "pred_time": pred_time,
             }
         ```
             task: A string of the task type, e.g.,
                 'classification', 'regression', 'ts_forecast', 'rank',
-                'seq-classification', 'seq-regression', 'summarization'.
+                'seq-classification', 'seq-regression', 'summarization',
+                or an instance of the Task class.
             n_jobs: An integer of the number of threads for training | default=-1.
                 Use all available resources when n_jobs == -1.
             log_file_name: A string of the log file name | default="". To disable logging,
                 set it to be an empty string "".
             estimator_list: A list of strings for estimator names, or 'auto'.
                 e.g., ```['lgbm', 'xgboost', 'xgb_limitdepth', 'catboost', 'rf', 'extra_tree']```.
             time_budget: A float number of the time budget in seconds.
@@ -942,35 +532,41 @@
         return attr
 
     @property
     def time_to_find_best_model(self) -> float:
         """Time taken to find best model in seconds."""
         return self.__dict__.get("_time_taken_best_iter")
 
-    def score(self, X: pd.DataFrame, y: pd.Series, **kwargs):
+    def score(
+        self,
+        X: Union[pd.DataFrame, psDataFrame],
+        y: Union[pd.Series, psSeries],
+        **kwargs,
+    ):
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
             logger.warning(
                 "No estimator is trained. Please run fit with enough budget."
             )
             return None
-        X = self._preprocess(X)
+        X = self._state.task.preprocess(X, self._transformer)
         if self._label_transformer:
             y = self._label_transformer.transform(y)
         return estimator.score(X, y, **kwargs)
 
     def predict(
         self,
-        X: Union[np.array, pd.DataFrame, List[str], List[List[str]]],
+        X: Union[np.array, pd.DataFrame, List[str], List[List[str]], psDataFrame],
         **pred_kwargs,
     ):
         """Predict label from features.
 
         Args:
-            X: A numpy array of featurized instances, shape n * m,
+            X: A numpy array or pandas dataframe or pyspark.pandas dataframe
+            of featurized instances, shape n * m,
                 or for time series forcast tasks:
                     a pandas dataframe with the first column containing
                     timestamp values (datetime type) or an integer n for
                     the predict steps (only valid when the estimator is
                     arima or sarimax). Other columns in the dataframe
                     are assumed to be exogenous variables (categorical
                     or numeric).
@@ -992,15 +588,15 @@
         """
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
             logger.warning(
                 "No estimator is trained. Please run fit with enough budget."
             )
             return None
-        X = self._preprocess(X)
+        X = self._state.task.preprocess(X, self._transformer)
         y_pred = estimator.predict(X, **pred_kwargs)
         if (
             isinstance(y_pred, np.ndarray)
             and y_pred.ndim > 1
             and isinstance(y_pred, np.ndarray)
         ):
             y_pred = y_pred.flatten()
@@ -1026,596 +622,52 @@
         """
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
             logger.warning(
                 "No estimator is trained. Please run fit with enough budget."
             )
             return None
-        X = self._preprocess(X)
+        X = self._state.task.preprocess(X, self._transformer)
         proba = self._trained_estimator.predict_proba(X, **pred_kwargs)
         return proba
 
-    def _preprocess(self, X):
-        if isinstance(X, List):
-            try:
-                if isinstance(X[0], List):
-                    X = [x for x in zip(*X)]
-                X = pd.DataFrame(
-                    dict(
-                        [
-                            (self._transformer._str_columns[idx], X[idx])
-                            if isinstance(X[0], List)
-                            else (self._transformer._str_columns[idx], [X[idx]])
-                            for idx in range(len(X))
-                        ]
-                    )
-                )
-            except IndexError:
-                raise IndexError(
-                    "Test data contains more columns than training data, exiting"
-                )
-        elif isinstance(X, int):
-            return X
-        elif issparse(X):
-            X = X.tocsr()
-        if self._state.task in TS_FORECAST:
-            X = pd.DataFrame(X)
-        if self._transformer:
-            X = self._transformer.transform(X)
-        return X
-
-    def _validate_ts_data(
-        self,
-        dataframe,
-        y_train_all=None,
-    ):
-        assert (
-            dataframe[dataframe.columns[0]].dtype.name == "datetime64[ns]"
-        ), f"For '{TS_FORECAST}' task, the first column must contain timestamp values."
-        if y_train_all is not None:
-            y_df = (
-                pd.DataFrame(y_train_all)
-                if isinstance(y_train_all, pd.Series)
-                else pd.DataFrame(y_train_all, columns=["labels"])
-            )
-            dataframe = dataframe.join(y_df)
-        duplicates = dataframe.duplicated()
-        if any(duplicates):
-            logger.warning(
-                "Duplicate timestamp values found in timestamp column. "
-                f"\n{dataframe.loc[duplicates, dataframe][dataframe.columns[0]]}"
-            )
-            dataframe = dataframe.drop_duplicates()
-            logger.warning("Removed duplicate rows based on all columns")
-            assert (
-                dataframe[[dataframe.columns[0]]].duplicated() is None
-            ), "Duplicate timestamp values with different values for other columns."
-        ts_series = pd.to_datetime(dataframe[dataframe.columns[0]])
-        inferred_freq = pd.infer_freq(ts_series)
-        if inferred_freq is None:
-            logger.warning(
-                "Missing timestamps detected. To avoid error with estimators, set estimator list to ['prophet']. "
-            )
-        if y_train_all is not None:
-            return dataframe.iloc[:, :-1], dataframe.iloc[:, -1]
-        return dataframe
-
-    def _validate_data(
-        self,
-        X_train_all,
-        y_train_all,
-        dataframe,
-        label,
-        X_val=None,
-        y_val=None,
-        groups_val=None,
-        groups=None,
-    ):
-        if X_train_all is not None and y_train_all is not None:
-            assert (
-                isinstance(X_train_all, np.ndarray)
-                or issparse(X_train_all)
-                or isinstance(X_train_all, pd.DataFrame)
-            ), (
-                "X_train_all must be a numpy array, a pandas dataframe, "
-                "or Scipy sparse matrix."
-            )
-            assert isinstance(y_train_all, np.ndarray) or isinstance(
-                y_train_all, pd.Series
-            ), "y_train_all must be a numpy array or a pandas series."
-            assert (
-                X_train_all.size != 0 and y_train_all.size != 0
-            ), "Input data must not be empty."
-            if isinstance(X_train_all, np.ndarray) and len(X_train_all.shape) == 1:
-                X_train_all = np.reshape(X_train_all, (X_train_all.size, 1))
-            if isinstance(y_train_all, np.ndarray):
-                y_train_all = y_train_all.flatten()
-            assert (
-                X_train_all.shape[0] == y_train_all.shape[0]
-            ), "# rows in X_train must match length of y_train."
-            self._df = isinstance(X_train_all, pd.DataFrame)
-            self._nrow, self._ndim = X_train_all.shape
-            if self._state.task in TS_FORECAST:
-                X_train_all = pd.DataFrame(X_train_all)
-                X_train_all, y_train_all = self._validate_ts_data(
-                    X_train_all, y_train_all
-                )
-            X, y = X_train_all, y_train_all
-        elif dataframe is not None and label is not None:
-            assert isinstance(
-                dataframe, pd.DataFrame
-            ), "dataframe must be a pandas DataFrame"
-            assert label in dataframe.columns, "label must a column name in dataframe"
-            self._df = True
-            if self._state.task in TS_FORECAST:
-                dataframe = self._validate_ts_data(dataframe)
-            X = dataframe.drop(columns=label)
-            self._nrow, self._ndim = X.shape
-            y = dataframe[label]
-        else:
-            raise ValueError("either X_train+y_train or dataframe+label are required")
-
-        # check the validity of input dimensions for NLP tasks, so need to check _is_nlp_task not estimator
-        if _is_nlp_task(self._state.task):
-            from .nlp.utils import is_a_list_of_str
-
-            is_all_str = True
-            is_all_list = True
-            for column in X.columns:
-                assert X[column].dtype.name in (
-                    "object",
-                    "string",
-                ), "If the task is an NLP task, X can only contain text columns"
-                for each_cell in X[column]:
-                    if each_cell is not None:
-                        is_str = isinstance(each_cell, str)
-                        is_list_of_int = isinstance(each_cell, list) and all(
-                            isinstance(x, int) for x in each_cell
-                        )
-                        is_list_of_str = is_a_list_of_str(each_cell)
-                        if self._state.task == TOKENCLASSIFICATION:
-                            assert is_list_of_str, (
-                                "For the token-classification task, the input column needs to be a list of string,"
-                                "instead of string, e.g., ['EU', 'rejects','German', 'call','to','boycott','British','lamb','.',].",
-                                "For more examples, please refer to test/nlp/test_autohf_tokenclassification.py",
-                            )
-                        else:
-                            assert is_str or is_list_of_int, (
-                                "Each column of the input must either be str (untokenized) "
-                                "or a list of integers (tokenized)"
-                            )
-                        is_all_str &= is_str
-                        is_all_list &= is_list_of_int or is_list_of_str
-            assert is_all_str or is_all_list, (
-                "Currently FLAML only supports two modes for NLP: either all columns of X are string (non-tokenized), "
-                "or all columns of X are integer ids (tokenized)"
-            )
-
-        if issparse(X_train_all) or self._skip_transform:
-            self._transformer = self._label_transformer = False
-            self._X_train_all, self._y_train_all = X, y
-        else:
-            from .data import DataTransformer
-
-            self._transformer = DataTransformer()
-
-            self._X_train_all, self._y_train_all = self._transformer.fit_transform(
-                X, y, self._state.task
-            )
-            self._label_transformer = self._transformer.label_transformer
-            if self._state.task == TOKENCLASSIFICATION:
-                if hasattr(self._label_transformer, "label_list"):
-                    self._state.fit_kwargs.update(
-                        {"label_list": self._label_transformer.label_list}
-                    )
-                elif "label_list" not in self._state.fit_kwargs:
-                    for each_fit_kwargs in self._state.fit_kwargs_by_estimator.values():
-                        assert (
-                            "label_list" in each_fit_kwargs
-                        ), "For the token-classification task, you must either (1) pass token labels; or (2) pass id labels and the label list. "
-                        "Please refer to the documentation for more details: https://microsoft.github.io/FLAML/docs/Examples/AutoML-NLP#a-simple-token-classification-example"
-            self._feature_names_in_ = (
-                self._X_train_all.columns.to_list()
-                if hasattr(self._X_train_all, "columns")
-                else None
-            )
-
-        self._sample_weight_full = self._state.fit_kwargs.get(
-            "sample_weight"
-        )  # NOTE: _validate_data is before kwargs is updated to fit_kwargs_by_estimator
-        if X_val is not None and y_val is not None:
-            assert (
-                isinstance(X_val, np.ndarray)
-                or issparse(X_val)
-                or isinstance(X_val, pd.DataFrame)
-            ), (
-                "X_val must be None, a numpy array, a pandas dataframe, "
-                "or Scipy sparse matrix."
-            )
-            assert isinstance(y_val, np.ndarray) or isinstance(
-                y_val, pd.Series
-            ), "y_val must be None, a numpy array or a pandas series."
-            assert X_val.size != 0 and y_val.size != 0, (
-                "Validation data are expected to be nonempty. "
-                "Use None for X_val and y_val if no validation data."
-            )
-            if isinstance(y_val, np.ndarray):
-                y_val = y_val.flatten()
-            assert (
-                X_val.shape[0] == y_val.shape[0]
-            ), "# rows in X_val must match length of y_val."
-            if self._transformer:
-                self._state.X_val = self._transformer.transform(X_val)
-            else:
-                self._state.X_val = X_val
-            # If it's NLG_TASKS, y_val is a pandas series containing the output sequence tokens,
-            # so we cannot use label_transformer.transform to process it
-            if self._label_transformer:
-                self._state.y_val = self._label_transformer.transform(y_val)
-            else:
-                self._state.y_val = y_val
-        else:
-            self._state.X_val = self._state.y_val = None
-        if groups is not None and len(groups) != self._nrow:
-            # groups is given as group counts
-            self._state.groups = np.concatenate([[i] * c for i, c in enumerate(groups)])
-            assert (
-                len(self._state.groups) == self._nrow
-            ), "the sum of group counts must match the number of examples"
-            self._state.groups_val = (
-                np.concatenate([[i] * c for i, c in enumerate(groups_val)])
-                if groups_val is not None
-                else None
-            )
-        else:
-            self._state.groups_val = groups_val
-            self._state.groups = groups
-
-    def _prepare_data(self, eval_method, split_ratio, n_splits):
-        X_val, y_val = self._state.X_val, self._state.y_val
-        if issparse(X_val):
-            X_val = X_val.tocsr()
-        X_train_all, y_train_all = self._X_train_all, self._y_train_all
-        if issparse(X_train_all):
-            X_train_all = X_train_all.tocsr()
-        if (
-            self._state.task in CLASSIFICATION
-            and self._auto_augment
-            and self._state.fit_kwargs.get("sample_weight")
-            is None  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-            and self._split_type in ["stratified", "uniform"]
-            and self._state.task != TOKENCLASSIFICATION
-        ):
-            # logger.info(f"label {pd.unique(y_train_all)}")
-            label_set, counts = np.unique(y_train_all, return_counts=True)
-            # augment rare classes
-            rare_threshld = 20
-            rare = counts < rare_threshld
-            rare_label, rare_counts = label_set[rare], counts[rare]
-            for i, label in enumerate(rare_label):
-                count = rare_count = rare_counts[i]
-                rare_index = y_train_all == label
-                n = len(y_train_all)
-                while count < rare_threshld:
-                    if self._df:
-                        X_train_all = concat(
-                            X_train_all, X_train_all.iloc[:n].loc[rare_index]
-                        )
-                    else:
-                        X_train_all = concat(
-                            X_train_all, X_train_all[:n][rare_index, :]
-                        )
-                    if isinstance(y_train_all, pd.Series):
-                        y_train_all = concat(
-                            y_train_all, y_train_all.iloc[:n].loc[rare_index]
-                        )
-                    else:
-                        y_train_all = np.concatenate(
-                            [y_train_all, y_train_all[:n][rare_index]]
-                        )
-                    count += rare_count
-                logger.info(f"class {label} augmented from {rare_count} to {count}")
-        SHUFFLE_SPLIT_TYPES = ["uniform", "stratified"]
-        if self._split_type in SHUFFLE_SPLIT_TYPES:
-            if self._sample_weight_full is not None:
-                X_train_all, y_train_all, self._state.sample_weight_all = shuffle(
-                    X_train_all,
-                    y_train_all,
-                    self._sample_weight_full,
-                    random_state=RANDOM_SEED,
-                )
-                self._state.fit_kwargs[
-                    "sample_weight"
-                ] = (
-                    self._state.sample_weight_all
-                )  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                if isinstance(self._state.sample_weight_all, pd.Series):
-                    self._state.sample_weight_all.reset_index(drop=True, inplace=True)
-            else:
-                X_train_all, y_train_all = shuffle(
-                    X_train_all, y_train_all, random_state=RANDOM_SEED
-                )
-            if self._df:
-                X_train_all.reset_index(drop=True, inplace=True)
-            if isinstance(y_train_all, pd.Series):
-                y_train_all.reset_index(drop=True, inplace=True)
-
-        X_train, y_train = X_train_all, y_train_all
-        self._state.groups_all = self._state.groups
-        if X_val is None and eval_method == "holdout":
-            # if eval_method = holdout, make holdout data
-            if self._split_type == "time":
-                if self._state.task in TS_FORECAST:
-                    period = self._state.fit_kwargs[
-                        "period"
-                    ]  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                    if self._state.task == TS_FORECASTPANEL:
-                        X_train_all["time_idx"] -= X_train_all["time_idx"].min()
-                        X_train_all["time_idx"] = X_train_all["time_idx"].astype("int")
-                        ids = self._state.fit_kwargs["group_ids"].copy()
-                        ids.append(TS_TIMESTAMP_COL)
-                        ids.append("time_idx")
-                        y_train_all = pd.DataFrame(y_train_all)
-                        y_train_all[ids] = X_train_all[ids]
-                        X_train_all = X_train_all.sort_values(ids)
-                        y_train_all = y_train_all.sort_values(ids)
-                        training_cutoff = X_train_all["time_idx"].max() - period
-                        X_train = X_train_all[lambda x: x.time_idx <= training_cutoff]
-                        y_train = y_train_all[
-                            lambda x: x.time_idx <= training_cutoff
-                        ].drop(columns=ids)
-                        X_val = X_train_all[lambda x: x.time_idx > training_cutoff]
-                        y_val = y_train_all[
-                            lambda x: x.time_idx > training_cutoff
-                        ].drop(columns=ids)
-                    else:
-                        num_samples = X_train_all.shape[0]
-                        assert (
-                            period < num_samples
-                        ), f"period={period}>#examples={num_samples}"
-                        split_idx = num_samples - period
-                        X_train = X_train_all[:split_idx]
-                        y_train = y_train_all[:split_idx]
-                        X_val = X_train_all[split_idx:]
-                        y_val = y_train_all[split_idx:]
-                else:
-                    if (
-                        "sample_weight" in self._state.fit_kwargs
-                    ):  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                        (
-                            X_train,
-                            X_val,
-                            y_train,
-                            y_val,
-                            self._state.fit_kwargs[
-                                "sample_weight"
-                            ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                            self._state.weight_val,
-                        ) = train_test_split(
-                            X_train_all,
-                            y_train_all,
-                            self._state.fit_kwargs[
-                                "sample_weight"
-                            ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                            test_size=split_ratio,
-                            shuffle=False,
-                        )
-                    else:
-                        X_train, X_val, y_train, y_val = train_test_split(
-                            X_train_all,
-                            y_train_all,
-                            test_size=split_ratio,
-                            shuffle=False,
-                        )
-            elif self._split_type == "group":
-                gss = GroupShuffleSplit(
-                    n_splits=1, test_size=split_ratio, random_state=RANDOM_SEED
-                )
-                for train_idx, val_idx in gss.split(
-                    X_train_all, y_train_all, self._state.groups_all
-                ):
-                    if self._df:
-                        X_train = X_train_all.iloc[train_idx]
-                        X_val = X_train_all.iloc[val_idx]
-                    else:
-                        X_train, X_val = X_train_all[train_idx], X_train_all[val_idx]
-                    y_train, y_val = y_train_all[train_idx], y_train_all[val_idx]
-                    self._state.groups = self._state.groups_all[train_idx]
-                    self._state.groups_val = self._state.groups_all[val_idx]
-            elif self._state.task in CLASSIFICATION:
-                # for classification, make sure the labels are complete in both
-                # training and validation data
-                label_set, first = np.unique(y_train_all, return_index=True)
-                rest = []
-                last = 0
-                first.sort()
-                for i in range(len(first)):
-                    rest.extend(range(last, first[i]))
-                    last = first[i] + 1
-                rest.extend(range(last, len(y_train_all)))
-                X_first = X_train_all.iloc[first] if self._df else X_train_all[first]
-                X_rest = X_train_all.iloc[rest] if self._df else X_train_all[rest]
-                y_rest = y_train_all[rest]
-                stratify = y_rest if self._split_type == "stratified" else None
-                if (
-                    "sample_weight" in self._state.fit_kwargs
-                ):  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                    (
-                        X_train,
-                        X_val,
-                        y_train,
-                        y_val,
-                        weight_train,
-                        weight_val,
-                    ) = train_test_split(
-                        X_rest,
-                        y_rest,
-                        self._state.fit_kwargs["sample_weight"][
-                            rest
-                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                        test_size=split_ratio,
-                        stratify=stratify,
-                        random_state=RANDOM_SEED,
-                    )
-                    weight1 = self._state.fit_kwargs["sample_weight"][
-                        first
-                    ]  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                    self._state.weight_val = concat(weight1, weight_val)
-                    self._state.fit_kwargs[
-                        "sample_weight"
-                    ] = concat(  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                        weight1, weight_train
-                    )
-                else:
-                    X_train, X_val, y_train, y_val = train_test_split(
-                        X_rest,
-                        y_rest,
-                        test_size=split_ratio,
-                        stratify=stratify,
-                        random_state=RANDOM_SEED,
-                    )
-                X_train = concat(X_first, X_train)
-                y_train = (
-                    concat(label_set, y_train)
-                    if self._df
-                    else np.concatenate([label_set, y_train])
-                )
-                X_val = concat(X_first, X_val)
-                y_val = (
-                    concat(label_set, y_val)
-                    if self._df
-                    else np.concatenate([label_set, y_val])
-                )
-            elif self._state.task in REGRESSION:
-                if (
-                    "sample_weight" in self._state.fit_kwargs
-                ):  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                    (
-                        X_train,
-                        X_val,
-                        y_train,
-                        y_val,
-                        self._state.fit_kwargs[
-                            "sample_weight"
-                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                        self._state.weight_val,
-                    ) = train_test_split(
-                        X_train_all,
-                        y_train_all,
-                        self._state.fit_kwargs[
-                            "sample_weight"
-                        ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                        test_size=split_ratio,
-                        random_state=RANDOM_SEED,
-                    )
-                else:
-                    X_train, X_val, y_train, y_val = train_test_split(
-                        X_train_all,
-                        y_train_all,
-                        test_size=split_ratio,
-                        random_state=RANDOM_SEED,
-                    )
-        self._state.data_size = X_train.shape
-        self.data_size_full = len(y_train_all)
-        self._state.X_train, self._state.y_train = X_train, y_train
-        self._state.X_val, self._state.y_val = X_val, y_val
-        self._state.X_train_all = X_train_all
-        self._state.y_train_all = y_train_all
-        if eval_method == "holdout":
-            self._state.kf = None
-            return
-        if self._split_type == "group":
-            # logger.info("Using GroupKFold")
-            assert (
-                len(self._state.groups_all) == y_train_all.size
-            ), "the length of groups must match the number of examples"
-            assert (
-                len(np.unique(self._state.groups_all)) >= n_splits
-            ), "the number of groups must be equal or larger than n_splits"
-            self._state.kf = GroupKFold(n_splits)
-        elif self._split_type == "stratified":
-            # logger.info("Using StratifiedKFold")
-            assert y_train_all.size >= n_splits, (
-                f"{n_splits}-fold cross validation"
-                f" requires input data with at least {n_splits} examples."
-            )
-            assert y_train_all.size >= 2 * n_splits, (
-                f"{n_splits}-fold cross validation with metric=r2 "
-                f"requires input data with at least {n_splits*2} examples."
-            )
-            self._state.kf = RepeatedStratifiedKFold(
-                n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED
-            )
-        elif self._split_type == "time":
-            # logger.info("Using TimeSeriesSplit")
-            if (
-                self._state.task in TS_FORECAST
-                and self._state.task is not TS_FORECASTPANEL
-            ):
-                period = self._state.fit_kwargs[
-                    "period"
-                ]  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
-                if period * (n_splits + 1) > y_train_all.size:
-                    n_splits = int(y_train_all.size / period - 1)
-                    assert n_splits >= 2, (
-                        f"cross validation for forecasting period={period}"
-                        f" requires input data with at least {3 * period} examples."
-                    )
-                    logger.info(f"Using nsplits={n_splits} due to data size limit.")
-                self._state.kf = TimeSeriesSplit(n_splits=n_splits, test_size=period)
-            elif self._state.task is TS_FORECASTPANEL:
-                n_groups = X_train.groupby(
-                    self._state.fit_kwargs.get("group_ids")
-                ).ngroups
-                period = self._state.fit_kwargs.get("period")
-                self._state.kf = TimeSeriesSplit(
-                    n_splits=n_splits, test_size=period * n_groups
-                )
-            else:
-                self._state.kf = TimeSeriesSplit(n_splits=n_splits)
-        elif isinstance(self._split_type, str):
-            # logger.info("Using RepeatedKFold")
-            self._state.kf = RepeatedKFold(
-                n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED
-            )
-        else:
-            # logger.info("Using splitter object")
-            self._state.kf = self._split_type
-        if isinstance(self._state.kf, (GroupKFold, StratifiedGroupKFold)):
-            # self._split_type is either "group", a GroupKFold object, or a StratifiedGroupKFold object
-            self._state.kf.groups = self._state.groups_all
-
     def add_learner(self, learner_name, learner_class):
         """Add a customized learner.
 
         Args:
             learner_name: A string of the learner's name.
             learner_class: A subclass of flaml.model.BaseEstimator.
         """
         self._state.learner_classes[learner_name] = learner_class
 
-    def get_estimator_from_log(self, log_file_name: str, record_id: int, task: str):
+    def get_estimator_from_log(
+        self, log_file_name: str, record_id: int, task: Union[str, Task]
+    ):
         """Get the estimator from log file.
 
         Args:
             log_file_name: A string of the log file name.
             record_id: An integer of the record ID in the file,
                 0 corresponds to the first trial.
             task: A string of the task type,
-                'binary', 'multiclass', 'regression', 'ts_forecast', 'rank'.
+                'binary', 'multiclass', 'regression', 'ts_forecast', 'rank',
+                or an instance of the Task class.
 
         Returns:
             An estimator object for the given configuration.
         """
 
         with training_log_reader(log_file_name) as reader:
             record = reader.get_record(record_id)
             estimator = record.learner
             config = AutoMLState.sanitize(record.config)
 
+        if isinstance(task, str):
+            task = task_factory(task)
+
         estimator, _ = train_estimator(
             X_train=None,
             y_train=None,
             config_dic=config,
             task=task,
             estimator_name=estimator,
             estimator_class=self._state.learner_classes.get(estimator),
@@ -1627,15 +679,15 @@
         self,
         log_file_name,
         X_train=None,
         y_train=None,
         dataframe=None,
         label=None,
         time_budget=np.inf,
-        task=None,
+        task: Optional[Union[str, Task]] = None,
         eval_method=None,
         split_ratio=None,
         n_splits=None,
         split_type=None,
         groups=None,
         n_jobs=-1,
         # gpu_per_trial=0,
@@ -1654,33 +706,31 @@
         This function is intended to retrain the logged configurations.
         NOTE: In some rare case, the last config is early stopped to meet time_budget and it's the best config.
         But the logged config's ITER_HP (e.g., n_estimators) is not reduced.
 
         Args:
             log_file_name: A string of the log file name.
             X_train: A numpy array or dataframe of training data in shape n*m.
-                For time series forecast tasks, the first column of X_train
-                must be the timestamp column (datetime type). Other
-                columns in the dataframe are assumed to be exogenous
-                variables (categorical or numeric).
+                For time series forecast tasks, the first column of X_train must be the timestamp column (datetime type). Other columns in the dataframe are assumed to be exogenous variables (categorical or numeric).
             y_train: A numpy array or series of labels in shape n*1.
             dataframe: A dataframe of training data including label column.
                 For time series forecast tasks, dataframe must be specified and should
                 have at least two columns: timestamp and label, where the first
                 column is the timestamp column (datetime type). Other columns
                 in the dataframe are assumed to be exogenous variables
                 (categorical or numeric).
             label: A str of the label column name, e.g., 'label';
                 Note: If X_train and y_train are provided,
                 dataframe and label are ignored;
                 If not, dataframe and label must be provided.
             time_budget: A float number of the time budget in seconds.
             task: A string of the task type, e.g.,
                 'classification', 'regression', 'ts_forecast', 'rank',
-                'seq-classification', 'seq-regression', 'summarization'.
+                'seq-classification', 'seq-regression', 'summarization',
+                or an instance of Task class.
             eval_method: A string of resampling strategy, one of
                 ['auto', 'cv', 'holdout'].
             split_ratio: A float of the validation data percentage for holdout.
             n_splits: An integer of the number of folds for cross-validation.
             split_type: str or splitter object, default="auto" | the data split type.
                 * A valid splitter object is an instance of a derived class of scikit-learn
                 [KFold](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.KFold.html#sklearn.model_selection.KFold)
@@ -1758,23 +808,26 @@
                         for tensorboard, only used by TemporalFusionTransformerEstimator.
                     max_epochs: int, default = 20 | Maximum number of epochs to run training,
                         only used by TemporalFusionTransformerEstimator.
                     batch_size: int, default = 64 | Batch size for training model, only
                         used by TemporalFusionTransformerEstimator.
         """
         task = task or self._settings.get("task")
+        if isinstance(task, str):
+            task = task_factory(task)
+
         eval_method = eval_method or self._settings.get("eval_method")
         split_ratio = split_ratio or self._settings.get("split_ratio")
         n_splits = n_splits or self._settings.get("n_splits")
         split_type = split_type or self._settings.get("split_type")
         auto_augment = (
             self._settings.get("auto_augment") if auto_augment is None else auto_augment
         )
         self._state.task = task
-        self._estimator_type = "classifier" if task in CLASSIFICATION else "regressor"
+        self._estimator_type = "classifier" if task.is_classification() else "regressor"
 
         self._state.fit_kwargs = fit_kwargs
         self._state.custom_hp = custom_hp or self._settings.get("custom_hp")
         self._skip_transform = (
             self._settings.get("skip_transform")
             if skip_transform is None
             else skip_transform
@@ -1783,15 +836,17 @@
             fit_kwargs_by_estimator or self._settings.get("fit_kwargs_by_estimator")
         )
         self.preserve_checkpoint = (
             self._settings.get("preserve_checkpoint")
             if preserve_checkpoint is None
             else preserve_checkpoint
         )
-        self._validate_data(X_train, y_train, dataframe, label, groups=groups)
+        task.validate_data(
+            self, self._state, X_train, y_train, dataframe, label, groups=groups
+        )
 
         logger.info("log file name {}".format(log_file_name))
 
         best_config = None
         best_val_loss = float("+inf")
         best_estimator = None
         sample_size = None
@@ -1847,15 +902,20 @@
         logger.info(
             "estimator = {}, config = {}, #training instances = {}".format(
                 best_estimator, best_config, sample_size
             )
         )
         # Partially copied from fit() function
         # Initilize some attributes required for retrain_from_log
-        self._decide_split_type(split_type)
+        self._split_type = task.decide_split_type(
+            split_type,
+            self._y_train_all,
+            self._state.fit_kwargs,
+            self._state.groups,
+        )
         eval_method = self._decide_eval_method(eval_method, time_budget)
         self.modelcount = 0
         self._auto_augment = auto_augment
         self._prepare_data(eval_method, split_ratio, n_splits)
         self._state.time_budget = -1
         self._state.free_mem_ratio = 0
         self._state.n_jobs = n_jobs
@@ -1873,59 +933,14 @@
             best_estimator,
             best_config,
             sample_size=sample_size,
         )[0]
         logger.info("retrain from log succeeded")
         return training_duration
 
-    def _decide_split_type(self, split_type):
-        if self._state.task == "classification":
-            self._state.task = get_classification_objective(
-                len(np.unique(self._y_train_all))
-            )
-        if not isinstance(split_type, str):
-            assert hasattr(split_type, "split") and hasattr(
-                split_type, "get_n_splits"
-            ), "split_type must be a string or a splitter object with split and get_n_splits methods."
-            assert (
-                not isinstance(split_type, GroupKFold) or self._state.groups is not None
-            ), "GroupKFold requires groups to be provided."
-            self._split_type = split_type
-        elif self._state.task in CLASSIFICATION:
-            assert split_type in ["auto", "stratified", "uniform", "time", "group"]
-            self._split_type = (
-                split_type
-                if split_type != "auto"
-                else self._state.groups is None and "stratified" or "group"
-            )
-        elif self._state.task in REGRESSION:
-            assert split_type in ["auto", "uniform", "time", "group"]
-            self._split_type = split_type if split_type != "auto" else "uniform"
-        elif self._state.task in TS_FORECAST:
-            assert split_type in ["auto", "time"]
-            self._split_type = "time"
-            assert isinstance(
-                self._state.fit_kwargs.get("period"),
-                int,  # NOTE: _decide_split_type is before kwargs is updated to fit_kwargs_by_estimator
-            ), f"missing a required integer 'period' for '{TS_FORECAST}' task."
-            if self._state.fit_kwargs.get("group_ids"):
-                self._state.task == TS_FORECASTPANEL
-                assert isinstance(
-                    self._state.fit_kwargs.get("group_ids"), list
-                ), f"missing a required List[str] 'group_ids' for '{TS_FORECASTPANEL}' task."
-        elif self._state.task == "rank":
-            assert (
-                self._state.groups is not None
-            ), "groups must be specified for ranking task."
-            assert split_type in ["auto", "group"]
-            self._split_type = "group"
-        elif self._state.task in NLG_TASKS:
-            assert split_type in ["auto", "uniform", "time", "group"]
-            self._split_type = split_type if split_type != "auto" else "uniform"
-
     def _decide_eval_method(self, eval_method, time_budget):
         if not isinstance(self._split_type, str):
             assert eval_method in [
                 "auto",
                 "cv",
             ], "eval_method must be 'auto' or 'cv' for custom data splitter."
             assert (
@@ -2165,22 +1180,37 @@
         """Metric constraints.
 
         Returns:
             A list of the metric constraints.
         """
         return self._metric_constraints
 
+    def _prepare_data(self, eval_method, split_ratio, n_splits):
+        self._state.task.prepare_data(
+            self._state,
+            self._X_train_all,
+            self._y_train_all,
+            self._auto_augment,
+            eval_method,
+            self._split_type,
+            split_ratio,
+            n_splits,
+            self._df,
+            self._sample_weight_full,
+        )
+        self.data_size_full = len(self._state.y_train_all)
+
     def fit(
         self,
         X_train=None,
         y_train=None,
         dataframe=None,
         label=None,
         metric=None,
-        task=None,
+        task: Optional[Union[str, Task]] = None,
         n_jobs=None,
         # gpu_per_trial=0,
         log_file_name=None,
         estimator_list=None,
         time_budget=None,
         max_iter=None,
         sample=None,
@@ -2282,15 +1312,15 @@
                 "train_loss": train_loss,
                 "pred_time": pred_time,
             }
         ```
             task: A string of the task type, e.g.,
                 'classification', 'regression', 'ts_forecast_regression',
                 'ts_forecast_classification', 'rank', 'seq-classification',
-                'seq-regression', 'summarization'.
+                'seq-regression', 'summarization', or an instance of Task class
             n_jobs: An integer of the number of threads for training | default=-1.
                 Use all available resources when n_jobs == -1.
             log_file_name: A string of the log file name | default="". To disable logging,
                 set it to be an empty string "".
             estimator_list: A list of strings for estimator names, or 'auto'.
                 e.g., ```['lgbm', 'xgboost', 'xgb_limitdepth', 'catboost', 'rf', 'extra_tree']```.
             time_budget: A float number of the time budget in seconds.
@@ -2532,15 +1562,18 @@
                         only used by TemporalFusionTransformerEstimator.
                     batch_size: int, default = 64 | Batch size for training model, only
                         used by TemporalFusionTransformerEstimator.
         """
 
         self._state._start_time_flag = self._start_time_flag = time.time()
         task = task or self._settings.get("task")
-        self._estimator_type = "classifier" if task in CLASSIFICATION else "regressor"
+        if isinstance(task, str):
+            task = task_factory(task, X_train, y_train)
+        self._state.task = task
+        self._estimator_type = "classifier" if task.is_classification() else "regressor"
         time_budget = time_budget or self._settings.get("time_budget")
         n_jobs = n_jobs or self._settings.get("n_jobs")
         gpu_per_trial = fit_kwargs.get("gpu_per_trial", 0)
         eval_method = eval_method or self._settings.get("eval_method")
         split_ratio = split_ratio or self._settings.get("split_ratio")
         n_splits = n_splits or self._settings.get("n_splits")
         auto_augment = (
@@ -2712,23 +1745,37 @@
             "fit_kwargs_by_estimator"
         )
         self._state.fit_kwargs_by_estimator = (
             fit_kwargs_by_estimator.copy()
         )  # shallow copy of fit_kwargs_by_estimator
         self._state.weight_val = sample_weight_val
 
-        self._validate_data(
-            X_train, y_train, dataframe, label, X_val, y_val, groups_val, groups
+        task.validate_data(
+            self,
+            self._state,
+            X_train,
+            y_train,
+            dataframe,
+            label,
+            X_val,
+            y_val,
+            groups_val,
+            groups,
         )
         self._search_states = {}  # key: estimator name; value: SearchState
         self._random = np.random.RandomState(RANDOM_SEED)
         self._seed = seed if seed is not None else 20
         self._learner_selector = learner_selector
         logger.info(f"task = {task}")
-        self._decide_split_type(split_type)
+        self._split_type = self._state.task.decide_split_type(
+            split_type,
+            self._y_train_all,
+            self._state.fit_kwargs,
+            self._state.groups,
+        )
         logger.info(f"Data split method: {self._split_type}")
         eval_method = self._decide_eval_method(eval_method, time_budget)
         self._state.eval_method = eval_method
         logger.info("Evaluation method: {}".format(eval_method))
         self._state.cv_score_agg_func = cv_score_agg_func or self._settings.get(
             "cv_score_agg_func"
         )
@@ -2771,58 +1818,44 @@
             assert (
                 not _sample_size_from_starting_points
             ), "When subsampling is disabled, do not include FLAML_sample_size in the starting point."
         self._min_sample_size = _sample_size_from_starting_points or min_sample_size
         self._min_sample_size_input = min_sample_size
         self._prepare_data(eval_method, split_ratio, n_splits)
 
+        # TODO pull this to task as decide_sample_size
         if isinstance(self._min_sample_size, dict):
             self._sample = {
                 (
                     k,
                     sample
-                    and task != "rank"
+                    and not task.is_rank()
                     and eval_method != "cv"
                     and (
                         self._min_sample_size[k] * SAMPLE_MULTIPLY_FACTOR
                         < self._state.data_size[0]
                     ),
                 )
                 for k in self._min_sample_size.keys()
             }
         else:
             self._sample = (
                 sample
-                and task != "rank"
+                and not task.is_rank()
                 and eval_method != "cv"
                 and (
                     self._min_sample_size * SAMPLE_MULTIPLY_FACTOR
                     < self._state.data_size[0]
                 )
             )
-        if "auto" == metric:
-            if _is_nlp_task(self._state.task):
-                from flaml.automl.nlp.utils import (
-                    load_default_huggingface_metric_for_task,
-                )
-
-                metric = load_default_huggingface_metric_for_task(self._state.task)
-            elif "binary" in self._state.task:
-                metric = "roc_auc"
-            elif "multiclass" in self._state.task:
-                metric = "log_loss"
-            elif self._state.task in TS_FORECAST:
-                metric = "mape"
-            elif self._state.task == "rank":
-                metric = "ndcg"
-            else:
-                metric = "r2"
 
+        metric = task.default_metric(metric)
         self._state.metric = metric
 
+        # TODO pull this to task
         def is_to_reverse_metric(metric, task):
             if metric.startswith("ndcg"):
                 return True, f"1-{metric}"
             if metric in [
                 "r2",
                 "accuracy",
                 "roc_auc",
@@ -2833,15 +1866,15 @@
                 "roc_auc_ovo_weighted",
                 "f1",
                 "ap",
                 "micro_f1",
                 "macro_f1",
             ]:
                 return True, f"1-{metric}"
-            if _is_nlp_task(task):
+            if task.is_nlp():
                 from flaml.automl.ml import huggingface_metric_to_mode
 
                 if (
                     metric in huggingface_metric_to_mode
                     and huggingface_metric_to_mode[metric] == "max"
                 ):
                     return True, f"-{metric}"
@@ -2853,54 +1886,28 @@
                 error_metric = reverse_metric
             else:
                 error_metric = metric
         else:
             error_metric = "customized metric"
         logger.info(f"Minimizing error metric: {error_metric}")
 
-        if "auto" == estimator_list:
-            if self._state.task == "rank":
-                estimator_list = ["lgbm", "xgboost", "xgb_limitdepth"]
-            elif _is_nlp_task(self._state.task):
-                estimator_list = ["transformer"]
-            elif self._state.task == TS_FORECASTPANEL:
-                estimator_list = ["tft"]
-            else:
-                try:
-                    import catboost
+        is_spark_dataframe = isinstance(X_train, psDataFrame) or isinstance(
+            dataframe, psDataFrame
+        )
+        estimator_list = task.default_estimator_list(estimator_list, is_spark_dataframe)
+
+        if is_spark_dataframe and self._use_spark:
+            # For spark dataframe, use_spark must be False because spark models are trained in parallel themselves
+            self._use_spark = False
+            logger.warning(
+                "Spark dataframes support only spark.ml type models, which will be trained "
+                "with spark themselves, no need to start spark trials in flaml. "
+                "`use_spark` is set to False."
+            )
 
-                    estimator_list = [
-                        "lgbm",
-                        "rf",
-                        "catboost",
-                        "xgboost",
-                        "extra_tree",
-                        "xgb_limitdepth",
-                    ]
-                except ImportError:
-                    estimator_list = [
-                        "lgbm",
-                        "rf",
-                        "xgboost",
-                        "extra_tree",
-                        "xgb_limitdepth",
-                    ]
-                if self._state.task in TS_FORECAST:
-                    # catboost is removed because it has a `name` parameter, making it incompatible with hcrystalball
-                    if "catboost" in estimator_list:
-                        estimator_list.remove("catboost")
-                    if self._state.task in TS_FORECASTREGRESSION:
-                        try:
-                            import prophet
-
-                            estimator_list += ["prophet", "arima", "sarimax"]
-                        except ImportError:
-                            estimator_list += ["arima", "sarimax"]
-                elif "regression" != self._state.task:
-                    estimator_list += ["lrl1"]
         # When no search budget is specified
         if no_budget:
             max_iter = len(estimator_list)
             self._learner_selector = "roundrobin"
             if sample_is_none:
                 self._sample = False
             if no_starting_points:
@@ -3666,15 +2673,15 @@
                     for x in search_states[2:]
                     if x[1].best_loss < 4 * self._selected.best_loss
                 ]
                 logger.info(
                     [(estimator[0], estimator[1].params) for estimator in estimators]
                 )
             if len(estimators) > 1:
-                if self._state.task in CLASSIFICATION:
+                if self._state.task.is_classification():
                     from sklearn.ensemble import StackingClassifier as Stacker
                 else:
                     from sklearn.ensemble import StackingRegressor as Stacker
                 if self._use_ray is not False:
                     import ray
 
                     n_cpus = (
```

### Comparing `FLAML-1.1.3/flaml/automl/data.py` & `FLAML-1.2.0/flaml/automl/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,59 +6,37 @@
 from scipy.sparse import vstack, issparse
 import pandas as pd
 from pandas import DataFrame, Series
 
 from flaml.automl.training_log import training_log_reader
 
 from datetime import datetime
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
-# TODO: if your task is not specified in here, define your task as an all-capitalized word
-SEQCLASSIFICATION = "seq-classification"
-MULTICHOICECLASSIFICATION = "multichoice-classification"
-TOKENCLASSIFICATION = "token-classification"
-CLASSIFICATION = (
-    "binary",
-    "multiclass",
-    "classification",
-    SEQCLASSIFICATION,
-    MULTICHOICECLASSIFICATION,
-    TOKENCLASSIFICATION,
-)
-SEQREGRESSION = "seq-regression"
-REGRESSION = ("regression", SEQREGRESSION)
-TS_FORECASTREGRESSION = (
-    "forecast",
-    "ts_forecast",
-    "ts_forecast_regression",
-)
-TS_FORECASTCLASSIFICATION = "ts_forecast_classification"
-TS_FORECASTPANEL = "ts_forecast_panel"
-TS_FORECAST = (
-    *TS_FORECASTREGRESSION,
-    TS_FORECASTCLASSIFICATION,
-    TS_FORECASTPANEL,
-)
-TS_TIMESTAMP_COL = "ds"
-TS_VALUE_COL = "y"
-SUMMARIZATION = "summarization"
-NLG_TASKS = (SUMMARIZATION,)
-NLU_TASKS = (
-    SEQREGRESSION,
-    SEQCLASSIFICATION,
-    MULTICHOICECLASSIFICATION,
-    TOKENCLASSIFICATION,
-)
+import os
 
+try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
+    import pyspark.pandas as ps
+    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+except ImportError:
+    ps = None
 
-def _is_nlp_task(task):
-    if task in NLU_TASKS or task in NLG_TASKS:
-        return True
-    else:
-        return False
+    class psDataFrame:
+        pass
+
+    class psSeries:
+        pass
+
+
+if TYPE_CHECKING:
+    from flaml.automl.task import Task
+
+TS_TIMESTAMP_COL = "ds"
+TS_VALUE_COL = "y"
 
 
 def load_openml_dataset(
     dataset_id, data_dir=None, random_state=0, dataset_format="dataframe"
 ):
     """Load dataset from open ML.
 
@@ -232,22 +210,38 @@
         config_list,
         logged_metric_list,
     )
 
 
 def concat(X1, X2):
     """concatenate two matrices vertically."""
+    if type(X1) != type(X2):
+        if isinstance(X2, (psDataFrame, psSeries)):
+            X1 = ps.from_pandas(pd.DataFrame(X1))
+        elif isinstance(X1, (psDataFrame, psSeries)):
+            X2 = ps.from_pandas(pd.DataFrame(X2))
+        else:
+            X1 = pd.DataFrame(X1)
+            X2 = pd.DataFrame(X2)
+
     if isinstance(X1, (DataFrame, Series)):
         df = pd.concat([X1, X2], sort=False)
         df.reset_index(drop=True, inplace=True)
         if isinstance(X1, DataFrame):
             cat_columns = X1.select_dtypes(include="category").columns
             if len(cat_columns):
                 df[cat_columns] = df[cat_columns].astype("category")
         return df
+    if isinstance(X1, (psDataFrame, psSeries)):
+        df = ps.concat([X1, X2], ignore_index=True)
+        if isinstance(X1, psDataFrame):
+            cat_columns = X1.select_dtypes(include="category").columns.values.tolist()
+            if len(cat_columns):
+                df[cat_columns] = df[cat_columns].astype("category")
+        return df
     if issparse(X1):
         return vstack((X1, X2))
     else:
         return np.concatenate([X1, X2])
 
 
 def add_time_idx_col(X):
@@ -269,45 +263,51 @@
         X["time_idx"] = X["time_idx"].astype("int")
     return X
 
 
 class DataTransformer:
     """Transform input training data."""
 
-    def fit_transform(self, X: Union[DataFrame, np.array], y, task):
+    def fit_transform(
+        self, X: Union[DataFrame, np.ndarray], y, task: Union[str, "Task"]
+    ):
         """Fit transformer and process the input training data according to the task type.
 
         Args:
             X: A numpy array or a pandas dataframe of training data.
             y: A numpy array or a pandas series of labels.
-            task: A string of the task type, e.g.,
-                'classification', 'regression', 'ts_forecast', 'rank'.
+            task: An instance of type Task, or a str such as 'classification', 'regression'.
 
         Returns:
             X: Processed numpy array or pandas dataframe of training data.
             y: Processed numpy array or pandas series of labels.
         """
-        if _is_nlp_task(task):
+        if isinstance(task, str):
+            from flaml.automl.task.factory import task_factory
+
+            task = task_factory(task, X, y)
+
+        if task.is_nlp():
             # if the mode is NLP, check the type of input, each column must be either string or
             # ids (input ids, token type id, attention mask, etc.)
             str_columns = []
             for column in X.columns:
                 if isinstance(X[column].iloc[0], str):
                     str_columns.append(column)
             if len(str_columns) > 0:
                 X[str_columns] = X[str_columns].astype("string")
             self._str_columns = str_columns
         elif isinstance(X, DataFrame):
             X = X.copy()
             n = X.shape[0]
             cat_columns, num_columns, datetime_columns = [], [], []
             drop = False
-            if task in TS_FORECAST:
+            if task.is_ts_forecast():
                 X = X.rename(columns={X.columns[0]: TS_TIMESTAMP_COL})
-                if task is TS_FORECASTPANEL:
+                if task.is_ts_forecastpanel():
                     if "time_idx" not in X:
                         X = add_time_idx_col(X)
                 ds_col = X.pop(TS_TIMESTAMP_COL)
                 if isinstance(y, Series):
                     y = y.rename(TS_VALUE_COL)
             for column in X.columns:
                 # sklearn\utils\validation.py needs int/float values
@@ -357,15 +357,15 @@
                                 num_columns.append(key)
                         X[column] = X[column].map(datetime.toordinal)
                         datetime_columns.append(column)
                         del tmp_dt
                     X[column] = X[column].fillna(np.nan)
                     num_columns.append(column)
             X = X[cat_columns + num_columns]
-            if task in TS_FORECAST:
+            if task.is_ts_forecast():
                 X.insert(0, TS_TIMESTAMP_COL, ds_col)
             if cat_columns:
                 X[cat_columns] = X[cat_columns].astype("category")
             if num_columns:
                 X_num = X[num_columns]
                 if np.issubdtype(X_num.columns.dtype, np.integer) and (
                     drop
@@ -392,28 +392,27 @@
             self._cat_columns, self._num_columns, self._datetime_columns = (
                 cat_columns,
                 num_columns,
                 datetime_columns,
             )
             self._drop = drop
         if (
-            task in CLASSIFICATION
+            task.is_classification()
             or not pd.api.types.is_numeric_dtype(y)
-            and task not in NLG_TASKS
+            and not task.is_nlg()
         ):
-            if task != TOKENCLASSIFICATION:
+            if not task.is_token_classification():
                 from sklearn.preprocessing import LabelEncoder
 
                 self.label_transformer = LabelEncoder()
             else:
                 from flaml.automl.nlp.utils import LabelEncoderforTokenClassification
 
                 self.label_transformer = LabelEncoderforTokenClassification()
             y = self.label_transformer.fit_transform(y)
-
         else:
             self.label_transformer = None
         self._task = task
         return X, y
 
     def transform(self, X: Union[DataFrame, np.array]):
         """Process data using fit transformer.
@@ -422,26 +421,26 @@
             X: A numpy array or a pandas dataframe of training data.
 
         Returns:
             X: Processed numpy array or pandas dataframe of training data.
         """
         X = X.copy()
 
-        if _is_nlp_task(self._task):
+        if self._task.is_nlp():
             # if the mode is NLP, check the type of input, each column must be either string or
             # ids (input ids, token type id, attention mask, etc.)
             if len(self._str_columns) > 0:
                 X[self._str_columns] = X[self._str_columns].astype("string")
         elif isinstance(X, DataFrame):
             cat_columns, num_columns, datetime_columns = (
                 self._cat_columns,
                 self._num_columns,
                 self._datetime_columns,
             )
-            if self._task in TS_FORECAST:
+            if self._task.is_ts_forecast():
                 X = X.rename(columns={X.columns[0]: TS_TIMESTAMP_COL})
                 ds_col = X.pop(TS_TIMESTAMP_COL)
             for column in datetime_columns:
                 tmp_dt = X[column].dt
                 new_columns_dict = {
                     f"year_{column}": tmp_dt.year,
                     f"month_{column}": tmp_dt.month,
@@ -455,15 +454,15 @@
                 }
                 for new_col_name, new_col_value in new_columns_dict.items():
                     if new_col_name not in X.columns and new_col_name in num_columns:
                         X[new_col_name] = new_col_value
                 X[column] = X[column].map(datetime.toordinal)
                 del tmp_dt
             X = X[cat_columns + num_columns].copy()
-            if self._task in TS_FORECAST:
+            if self._task.is_ts_forecast():
                 X.insert(0, TS_TIMESTAMP_COL, ds_col)
             for column in cat_columns:
                 if X[column].dtype.name == "object":
                     X[column] = X[column].fillna("__NAN__")
                 elif X[column].dtype.name == "category":
                     current_categories = X[column].cat.categories
                     if "__NAN__" not in current_categories:
```

### Comparing `FLAML-1.1.3/flaml/automl/ml.py` & `FLAML-1.2.0/flaml/automl/ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # !
 #  * Copyright (c) FLAML authors. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
+import os
 import time
 import numpy as np
 import pandas as pd
 from typing import Union, Callable, TypeVar, Optional, Tuple
 
 from sklearn.metrics import (
     mean_squared_error,
@@ -15,20 +16,14 @@
     mean_absolute_error,
     log_loss,
     average_precision_score,
     f1_score,
     mean_absolute_percentage_error,
     ndcg_score,
 )
-from sklearn.model_selection import (
-    RepeatedStratifiedKFold,
-    GroupKFold,
-    TimeSeriesSplit,
-    StratifiedGroupKFold,
-)
 from flaml.automl.model import (
     XGBoostSklearnEstimator,
     XGBoost_TS,
     XGBoostLimitDepthEstimator,
     XGBoostLimitDepth_TS,
     RandomForestEstimator,
     RF_TS,
@@ -39,23 +34,45 @@
     CatBoostEstimator,
     ExtraTreesEstimator,
     ExtraTrees_TS,
     KNeighborsEstimator,
     Prophet,
     ARIMA,
     SARIMAX,
+    HoltWinters,
     TransformersEstimator,
     TemporalFusionTransformerEstimator,
     TransformersEstimatorModelSelection,
+    SparkLGBMEstimator,
 )
-from flaml.automl.data import CLASSIFICATION, group_counts, TS_FORECAST
+from flaml.automl.data import group_counts
+from flaml.automl.task.task import TS_FORECAST, Task
 from flaml.automl.model import BaseEstimator
-import logging
 
-logger = logging.getLogger(__name__)
+try:
+    from flaml.automl.spark.utils import len_labels
+except ImportError:
+    from flaml.automl.utils import len_labels
+try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
+    from pyspark.sql.functions import col
+    import pyspark.pandas as ps
+    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+    from flaml.automl.spark.utils import to_pandas_on_spark, iloc_pandas_on_spark
+    from flaml.automl.spark.metrics import spark_metric_loss_score
+except ImportError:
+    ps = None
+
+    class psDataFrame:
+        pass
+
+    class psSeries:
+        pass
+
+
 EstimatorSubclass = TypeVar("EstimatorSubclass", bound=BaseEstimator)
 
 sklearn_metric_name_set = {
     "r2",
     "rmse",
     "mae",
     "mse",
@@ -118,14 +135,16 @@
         estimator_class = (
             XGBoostLimitDepth_TS if task in TS_FORECAST else XGBoostLimitDepthEstimator
         )
     elif "rf" == estimator_name:
         estimator_class = RF_TS if task in TS_FORECAST else RandomForestEstimator
     elif "lgbm" == estimator_name:
         estimator_class = LGBM_TS if task in TS_FORECAST else LGBMEstimator
+    elif "lgbm_spark" == estimator_name:
+        estimator_class = SparkLGBMEstimator
     elif "lrl1" == estimator_name:
         estimator_class = LRL1Classifier
     elif "lrl2" == estimator_name:
         estimator_class = LRL2Classifier
     elif "catboost" == estimator_name:
         estimator_class = CatBoostEstimator
     elif "extra_tree" == estimator_name:
@@ -134,14 +153,16 @@
         estimator_class = KNeighborsEstimator
     elif "prophet" in estimator_name:
         estimator_class = Prophet
     elif estimator_name == "arima":
         estimator_class = ARIMA
     elif estimator_name == "sarimax":
         estimator_class = SARIMAX
+    elif estimator_name == "holt-winters":
+        estimator_class = HoltWinters
     elif estimator_name == "transformer":
         estimator_class = TransformersEstimator
     elif estimator_name == "tft":
         estimator_class = TemporalFusionTransformerEstimator
     elif estimator_name == "transformer_ms":
         estimator_class = TransformersEstimatorModelSelection
     else:
@@ -157,15 +178,23 @@
     y_processed_predict,
     y_processed_true,
     labels=None,
     sample_weight=None,
     groups=None,
 ):
     # y_processed_predict and y_processed_true are processed id labels if the original were the token labels
-    if is_in_sklearn_metric_name_set(metric_name):
+    if isinstance(y_processed_predict, (psDataFrame, psSeries)):
+        return spark_metric_loss_score(
+            metric_name,
+            y_processed_predict,
+            y_processed_true,
+            sample_weight,
+            groups,
+        )
+    elif is_in_sklearn_metric_name_set(metric_name):
         return sklearn_metric_loss_score(
             metric_name,
             y_processed_predict,
             y_processed_true,
             labels,
             sample_weight,
             groups,
@@ -203,19 +232,19 @@
                     else "overall_accuracy"
                 ]
             else:
                 score = score_dict[metric_name]
         except ImportError:
             raise ValueError(
                 metric_name
-                + " is not an built-in sklearn metric and nlp is not installed. "
+                + " is not an built-in sklearn metric and [hf] is not installed. "
                 "Currently built-in sklearn metrics are: "
                 "r2, rmse, mae, mse, accuracy, roc_auc, roc_auc_ovr, roc_auc_ovo,"
                 "log_loss, mape, f1, micro_f1, macro_f1, ap. "
-                "If the metric is an nlp metric, please pip install flaml[nlp] ",
+                "If the metric is a huggingface metric, please pip install flaml[hf] ",
                 "or pass a customized metric function to AutoML.fit(metric=func)",
             )
         # If the metric is not found from huggingface dataset metric list (i.e., FileNotFoundError)
         # ask the user to provide a custom metric
         except FileNotFoundError:
             raise ValueError(
                 metric_name + " is neither an sklearn metric nor a huggingface metric. "
@@ -350,18 +379,21 @@
             score /= len(counts)
             score += 1
         else:
             score = 1 - ndcg_score([y_true], [y_predict])
     return score
 
 
-def get_y_pred(estimator, X, eval_metric, obj):
-    if eval_metric in ["roc_auc", "ap", "roc_auc_weighted"] and "binary" in obj:
+def get_y_pred(estimator, X, eval_metric, task: Task):
+    if eval_metric in ["roc_auc", "ap", "roc_auc_weighted"] and task.is_binary():
         y_pred_classes = estimator.predict_proba(X)
-        y_pred = y_pred_classes[:, 1] if y_pred_classes.ndim > 1 else y_pred_classes
+        if isinstance(y_pred_classes, (psSeries, psDataFrame)):
+            y_pred = y_pred_classes
+        else:
+            y_pred = y_pred_classes[:, 1] if y_pred_classes.ndim > 1 else y_pred_classes
     elif eval_metric in [
         "log_loss",
         "roc_auc",
         "roc_auc_ovr",
         "roc_auc_ovo",
         "roc_auc_ovo_weighted",
         "roc_auc_ovr_weighted",
@@ -378,37 +410,37 @@
     X_train,
     y_train,
     X_val,
     y_val,
     weight_val,
     groups_val,
     eval_metric: Union[str, Callable],
-    obj,
+    task,
     labels=None,
     log_training_metric=False,
     fit_kwargs: Optional[dict] = None,
 ):
     if fit_kwargs is None:
         fit_kwargs = {}
     if isinstance(eval_metric, str):
         pred_start = time.time()
-        val_pred_y = get_y_pred(estimator, X_val, eval_metric, obj)
+        val_pred_y = get_y_pred(estimator, X_val, eval_metric, task)
         pred_time = (time.time() - pred_start) / X_val.shape[0]
 
         val_loss = metric_loss_score(
             eval_metric,
             y_processed_predict=val_pred_y,
             y_processed_true=y_val,
             labels=labels,
             sample_weight=weight_val,
             groups=groups_val,
         )
         metric_for_logging = {"pred_time": pred_time}
         if log_training_metric:
-            train_pred_y = get_y_pred(estimator, X_train, eval_metric, obj)
+            train_pred_y = get_y_pred(estimator, X_train, eval_metric, task)
             metric_for_logging["train_loss"] = metric_loss_score(
                 eval_metric,
                 train_pred_y,
                 y_train,
                 labels,
                 fit_kwargs.get("sample_weight"),
                 fit_kwargs.get("groups"),
@@ -495,128 +527,14 @@
             {k: v / n for k, v in metrics_to_log.items()}
             if isinstance(metrics_to_log, dict)
             else metrics_to_log / n
         )
     return metric_to_minimize, metrics_to_log
 
 
-def evaluate_model_CV(
-    config: dict,
-    estimator: EstimatorSubclass,
-    X_train_all,
-    y_train_all,
-    budget,
-    kf,
-    task: str,
-    eval_metric,
-    best_val_loss,
-    cv_score_agg_func=None,
-    log_training_metric=False,
-    fit_kwargs: Optional[dict] = None,
-    free_mem_ratio=0,
-):
-    if fit_kwargs is None:
-        fit_kwargs = {}
-    if cv_score_agg_func is None:
-        cv_score_agg_func = default_cv_score_agg_func
-    start_time = time.time()
-    val_loss_folds = []
-    log_metric_folds = []
-    metric = None
-    train_time = pred_time = 0
-    total_fold_num = 0
-    n = kf.get_n_splits()
-    X_train_split, y_train_split = X_train_all, y_train_all
-    if task in CLASSIFICATION:
-        labels = np.unique(y_train_all)
-    else:
-        labels = fit_kwargs.get(
-            "label_list"
-        )  # pass the label list on to compute the evaluation metric
-    groups = None
-    shuffle = getattr(kf, "shuffle", task not in TS_FORECAST)
-    if isinstance(kf, RepeatedStratifiedKFold):
-        kf = kf.split(X_train_split, y_train_split)
-    elif isinstance(kf, (GroupKFold, StratifiedGroupKFold)):
-        groups = kf.groups
-        kf = kf.split(X_train_split, y_train_split, groups)
-        shuffle = False
-    elif isinstance(kf, TimeSeriesSplit):
-        kf = kf.split(X_train_split, y_train_split)
-    else:
-        kf = kf.split(X_train_split)
-    rng = np.random.RandomState(2020)
-    budget_per_train = budget and budget / n
-    if "sample_weight" in fit_kwargs:
-        weight = fit_kwargs["sample_weight"]
-        weight_val = None
-    else:
-        weight = weight_val = None
-    for train_index, val_index in kf:
-        if shuffle:
-            train_index = rng.permutation(train_index)
-        if isinstance(X_train_all, pd.DataFrame):
-            X_train = X_train_split.iloc[train_index]
-            X_val = X_train_split.iloc[val_index]
-        else:
-            X_train, X_val = X_train_split[train_index], X_train_split[val_index]
-        y_train, y_val = y_train_split[train_index], y_train_split[val_index]
-        estimator.cleanup()
-        if weight is not None:
-            fit_kwargs["sample_weight"], weight_val = (
-                weight[train_index],
-                weight[val_index],
-            )
-        if groups is not None:
-            fit_kwargs["groups"] = (
-                groups[train_index]
-                if isinstance(groups, np.ndarray)
-                else groups.iloc[train_index]
-            )
-            groups_val = (
-                groups[val_index]
-                if isinstance(groups, np.ndarray)
-                else groups.iloc[val_index]
-            )
-        else:
-            groups_val = None
-        val_loss_i, metric_i, train_time_i, pred_time_i = get_val_loss(
-            config,
-            estimator,
-            X_train,
-            y_train,
-            X_val,
-            y_val,
-            weight_val,
-            groups_val,
-            eval_metric,
-            task,
-            labels,
-            budget_per_train,
-            log_training_metric=log_training_metric,
-            fit_kwargs=fit_kwargs,
-            free_mem_ratio=free_mem_ratio,
-        )
-        if isinstance(metric_i, dict) and "intermediate_results" in metric_i.keys():
-            del metric_i["intermediate_results"]
-        if weight is not None:
-            fit_kwargs["sample_weight"] = weight
-        total_fold_num += 1
-        val_loss_folds.append(val_loss_i)
-        log_metric_folds.append(metric_i)
-        train_time += train_time_i
-        pred_time += pred_time_i
-        if budget and time.time() - start_time >= budget:
-            break
-    val_loss, metric = cv_score_agg_func(val_loss_folds, log_metric_folds)
-    n = total_fold_num
-    pred_time /= n
-    return val_loss, metric, train_time, pred_time
-
-
 def compute_estimator(
     X_train,
     y_train,
     X_val,
     y_val,
     weight_val,
     groups_val,
@@ -633,15 +551,15 @@
     ] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
     estimator_class: Optional[EstimatorSubclass] = None,
     cv_score_agg_func: Optional[callable] = None,
     log_training_metric: Optional[bool] = False,
     fit_kwargs: Optional[dict] = None,
     free_mem_ratio=0,
 ):
-    if not fit_kwargs:
+    if fit_kwargs is None:
         fit_kwargs = {}
 
     estimator_class = estimator_class or get_estimator_class(task, estimator_name)
     estimator = estimator_class(
         **config_dic,
         task=task,
         n_jobs=n_jobs,
@@ -670,22 +588,21 @@
             ),  # pass the label list on to compute the evaluation metric
             budget=budget,
             log_training_metric=log_training_metric,
             fit_kwargs=fit_kwargs,
             free_mem_ratio=0,
         )
     else:
-        val_loss, metric_for_logging, train_time, pred_time = evaluate_model_CV(
+        val_loss, metric_for_logging, train_time, pred_time = task.evaluate_model_CV(
             config_dic,
             estimator,
             X_train,
             y_train,
             budget,
             kf,
-            task,
             eval_metric,
             best_val_loss,
             cv_score_agg_func,
             log_training_metric=log_training_metric,
             fit_kwargs=fit_kwargs,
             free_mem_ratio=0,
         )
@@ -714,15 +631,15 @@
     start_time = time.time()
     estimator_class = estimator_class or get_estimator_class(task, estimator_name)
     estimator = estimator_class(
         **config_dic,
         task=task,
         n_jobs=n_jobs,
     )
-    if not fit_kwargs:
+    if fit_kwargs is None:
         fit_kwargs = {}
 
     if isinstance(estimator, TransformersEstimator):
         fit_kwargs["metric"] = eval_metric
 
     if X_train is not None:
         train_time = estimator.fit(
@@ -730,22 +647,14 @@
         )
     else:
         estimator = estimator.estimator_class(**estimator.params)
     train_time = time.time() - start_time
     return estimator, train_time
 
 
-def get_classification_objective(num_labels: int) -> str:
-    if num_labels == 2:
-        objective_name = "binary"
-    else:
-        objective_name = "multiclass"
-    return objective_name
-
-
 def norm_confusion_matrix(
     y_true: Union[np.array, pd.Series], y_pred: Union[np.array, pd.Series]
 ):
     """normalized confusion matrix.
 
     Args:
         estimator: A multi-class classification estimator.
```

### Comparing `FLAML-1.1.3/flaml/automl/model.py` & `FLAML-1.2.0/flaml/automl/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  * Copyright (c) FLAML authors. All rights reserved.
 #  * Licensed under the MIT License. See LICENSE file in the
 #  * project root for license information.
 from contextlib import contextmanager
 from functools import partial
 import signal
 import os
-from typing import Callable, List
+from typing import Callable, List, Union
 import numpy as np
 import time
 from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
 from sklearn.ensemble import ExtraTreesRegressor, ExtraTreesClassifier
 from sklearn.linear_model import LogisticRegression
 from sklearn.dummy import DummyClassifier, DummyRegressor
 from scipy.sparse import issparse
@@ -18,27 +18,61 @@
 import shutil
 from pandas import DataFrame, Series, to_datetime
 import sys
 import math
 from flaml import tune
 from flaml.automl.data import (
     group_counts,
-    CLASSIFICATION,
     add_time_idx_col,
-    TS_FORECASTREGRESSION,
     TS_TIMESTAMP_COL,
     TS_VALUE_COL,
+)
+from flaml.automl.task.task import (
+    CLASSIFICATION,
+    TS_FORECASTREGRESSION,
     SEQCLASSIFICATION,
     SEQREGRESSION,
     TOKENCLASSIFICATION,
     SUMMARIZATION,
     NLG_TASKS,
 )
 
 try:
+    from flaml.automl.spark.utils import len_labels, to_pandas_on_spark
+except ImportError:
+    from flaml.automl.utils import len_labels
+
+    to_pandas_on_spark = None
+from flaml.automl.spark.configs import (
+    ParamList_LightGBM_Classifier,
+    ParamList_LightGBM_Regressor,
+    ParamList_LightGBM_Ranker,
+)
+
+try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
+    from pyspark.sql.dataframe import DataFrame as sparkDataFrame
+    from pyspark.sql import SparkSession
+    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+
+    _have_spark = True
+except ImportError:
+    _have_spark = False
+
+    class psDataFrame:
+        pass
+
+    class psSeries:
+        pass
+
+    class sparkDataFrame:
+        pass
+
+
+try:
     import psutil
 except ImportError:
     psutil = None
 try:
     import resource
 except ImportError:
     resource = None
@@ -382,14 +416,331 @@
         """
         params = config.copy()
         if "FLAML_sample_size" in params:
             params.pop("FLAML_sample_size")
         return params
 
 
+class SparkEstimator(BaseEstimator):
+    """The base class for fine-tuning spark models, using pyspark.ml and SynapseML API."""
+
+    def __init__(self, task="binary", **config):
+        if not _have_spark:
+            raise ImportError(
+                "pyspark is not installed. Try `pip install flaml[spark]`."
+            )
+        super().__init__(task, **config)
+        self.df_train = None
+
+    def _preprocess(
+        self,
+        X_train: Union[psDataFrame, sparkDataFrame],
+        y_train: psSeries = None,
+        index_col: str = "tmp_index_col",
+    ):
+        # TODO: optimize this, support pyspark.sql.DataFrame
+        if y_train is not None:
+            self.df_train = X_train.join(y_train)
+        else:
+            self.df_train = X_train
+        if isinstance(self.df_train, psDataFrame):
+            self.df_train = self.df_train.to_spark(index_col=index_col)
+        return self.df_train
+
+    def fit(
+        self,
+        X_train: psDataFrame,
+        y_train: psSeries = None,
+        budget=None,
+        free_mem_ratio=0,
+        index_col: str = "tmp_index_col",
+        **kwargs,
+    ):
+        """Train the model from given training data.
+        Args:
+            X_train: A pyspark.pandas DataFrame of training data in shape n*m.
+            y_train: A pyspark.pandas Series in shape n*1. None if X_train is a pyspark.pandas
+                Dataframe contains y_train.
+            budget: A float of the time budget in seconds.
+            free_mem_ratio: A float between 0 and 1 for the free memory ratio to keep during training.
+        Returns:
+            train_time: A float of the training time in seconds.
+        """
+        df_train = self._preprocess(X_train, y_train, index_col=index_col)
+        train_time = self._fit(df_train, **kwargs)
+        return train_time
+
+    def _fit(self, df_train: sparkDataFrame, **kwargs):
+        current_time = time.time()
+        pipeline_model = self.estimator_class(**self.params, **kwargs)
+        if logger.level == logging.DEBUG:
+            logger.debug(
+                f"flaml.model - {pipeline_model} fit started with params {self.params}"
+            )
+        pipeline_model.fit(df_train)
+        if logger.level == logging.DEBUG:
+            logger.debug(f"flaml.model - {pipeline_model} fit finished")
+        train_time = time.time() - current_time
+        self._model = pipeline_model
+        return train_time
+
+    def predict(self, X, index_col="tmp_index_col", return_all=False, **kwargs):
+        """Predict label from features.
+        Args:
+            X: A pyspark or pyspark.pandas dataframe of featurized instances, shape n*m.
+            index_col: A str of the index column name. Default to "tmp_index_col".
+            return_all: A bool of whether to return all the prediction results. Default to False.
+        Returns:
+            A pyspark.pandas series of shape n*1 if return_all is False. Otherwise, a pyspark.pandas dataframe.
+        """
+        if self._model is not None:
+            X = self._preprocess(X, index_col=index_col)
+            predictions = to_pandas_on_spark(
+                self._model.transform(X), index_col=index_col
+            )
+            predictions.index.name = None
+            pred_y = predictions["prediction"]
+            if return_all:
+                return predictions
+            else:
+                return pred_y
+        else:
+            logger.warning(
+                "Estimator is not fit yet. Please run fit() before predict()."
+            )
+            return np.ones(X.shape[0])
+
+    def predict_proba(self, X, index_col="tmp_index_col", return_all=False, **kwargs):
+        """Predict the probability of each class from features.
+        Only works for classification problems
+        Args:
+            X: A pyspark or pyspark.pandas dataframe of featurized instances, shape n*m.
+            index_col: A str of the index column name. Default to "tmp_index_col".
+            return_all: A bool of whether to return all the prediction results. Default to False.
+        Returns:
+            A pyspark.pandas dataframe of shape n*c. c is the # classes.
+            Each element at (i,j) is the probability for instance i to be in
+                class j.
+        """
+        assert self._task in CLASSIFICATION, "predict_proba() only for classification."
+        if self._model is not None:
+            X = self._preprocess(X, index_col=index_col)
+            predictions = to_pandas_on_spark(
+                self._model.transform(X), index_col=index_col
+            )
+            predictions.index.name = None
+            pred_y = predictions["probability"]
+
+            if return_all:
+                return predictions
+            else:
+                return pred_y
+        else:
+            logger.warning(
+                "Estimator is not fit yet. Please run fit() before predict()."
+            )
+            return np.ones(X.shape[0])
+
+
+class SparkLGBMEstimator(SparkEstimator):
+    """The class for fine-tuning spark version lightgbm models, using SynapseML API."""
+
+    """The class for tuning LGBM, using sklearn API."""
+
+    ITER_HP = "numIterations"
+    DEFAULT_ITER = 100
+
+    @classmethod
+    def search_space(cls, data_size, **params):
+        upper = max(5, min(32768, int(data_size[0])))  # upper must be larger than lower
+        # https://github.com/microsoft/SynapseML/blob/master/lightgbm/src/main/scala/com/microsoft/azure/synapse/ml/lightgbm/LightGBMBase.scala
+        return {
+            "numIterations": {
+                "domain": tune.lograndint(lower=4, upper=upper),
+                "init_value": 4,
+                "low_cost_init_value": 4,
+            },
+            "numLeaves": {
+                "domain": tune.lograndint(lower=4, upper=upper),
+                "init_value": 4,
+                "low_cost_init_value": 4,
+            },
+            "minDataInLeaf": {
+                "domain": tune.lograndint(lower=2, upper=2**7 + 1),
+                "init_value": 20,
+            },
+            "learningRate": {
+                "domain": tune.loguniform(lower=1 / 1024, upper=1.0),
+                "init_value": 0.1,
+            },
+            "log_max_bin": {  # log transformed with base 2
+                "domain": tune.lograndint(lower=3, upper=11),
+                "init_value": 8,
+            },
+            "featureFraction": {
+                "domain": tune.uniform(lower=0.01, upper=1.0),
+                "init_value": 1.0,
+            },
+            "lambdaL1": {
+                "domain": tune.loguniform(lower=1 / 1024, upper=1024),
+                "init_value": 1 / 1024,
+            },
+            "lambdaL2": {
+                "domain": tune.loguniform(lower=1 / 1024, upper=1024),
+                "init_value": 1.0,
+            },
+        }
+
+    def config2params(self, config: dict) -> dict:
+        params = super().config2params(config)
+        if "n_jobs" in params:
+            params.pop("n_jobs")
+        if "log_max_bin" in params:
+            params["maxBin"] = (1 << params.pop("log_max_bin")) - 1
+        return params
+
+    @classmethod
+    def size(cls, config):
+        num_leaves = int(
+            round(config.get("numLeaves") or 1 << config.get("maxDepth", 16))
+        )
+        n_estimators = int(round(config["numIterations"]))
+        return (num_leaves * 3 + (num_leaves - 1) * 4 + 1.0) * n_estimators * 8
+
+    def __init__(self, task="binary", **config):
+        super().__init__(task, **config)
+        err_msg = (
+            "SynapseML is not installed. Please refer to [SynapseML]"
+            + "(https://github.com/microsoft/SynapseML) for installation instructions."
+        )
+        if "regression" == task:
+            try:
+                from synapse.ml.lightgbm import LightGBMRegressor
+            except ImportError:
+                raise ImportError(err_msg)
+
+            self.estimator_class = LightGBMRegressor
+            self.estimator_params = ParamList_LightGBM_Regressor
+        elif "rank" == task:
+            try:
+                from synapse.ml.lightgbm import LightGBMRanker
+            except ImportError:
+                raise ImportError(err_msg)
+
+            self.estimator_class = LightGBMRanker
+            self.estimator_params = ParamList_LightGBM_Ranker
+        else:
+            try:
+                from synapse.ml.lightgbm import LightGBMClassifier
+            except ImportError:
+                raise ImportError(err_msg)
+
+            self.estimator_class = LightGBMClassifier
+            self.estimator_params = ParamList_LightGBM_Classifier
+        self._time_per_iter = None
+        self._train_size = 0
+        self._mem_per_iter = -1
+        self.model_classes_ = None
+        self.model_n_classes_ = None
+
+    def fit(
+        self,
+        X_train,
+        y_train=None,
+        budget=None,
+        free_mem_ratio=0,
+        index_col="tmp_index_col",
+        **kwargs,
+    ):
+        start_time = time.time()
+        if self.model_n_classes_ is None and self._task not in ["regression", "rank"]:
+            self.model_n_classes_, self.model_classes_ = len_labels(
+                y_train, return_labels=True
+            )
+        df_train = self._preprocess(X_train, y_train, index_col=index_col)
+        # n_iter = self.params.get(self.ITER_HP, self.DEFAULT_ITER)
+        # trained = False
+        # mem0 = psutil.virtual_memory().available if psutil is not None else 1
+        _kwargs = kwargs.copy()
+        if self._task not in ["regression", "rank"] and "objective" not in _kwargs:
+            _kwargs["objective"] = (
+                "binary" if self.model_n_classes_ == 2 else "multiclass"
+            )
+        for k in list(_kwargs.keys()):
+            if k not in self.estimator_params:
+                logger.warning(
+                    f"[SparkLGBMEstimator] [Warning] Ignored unknown parameter: {k}"
+                )
+                _kwargs.pop(k)
+        # TODO: find a better estimation of early stopping
+        # if (
+        #     (not self._time_per_iter or abs(self._train_size - df_train.count()) > 4)
+        #     and budget is not None
+        #     or self._mem_per_iter < 0
+        #     and psutil is not None
+        # ) and n_iter > 1:
+        #     self.params[self.ITER_HP] = 1
+        #     self._t1 = self._fit(df_train, **_kwargs)
+        #     if budget is not None and self._t1 >= budget or n_iter == 1:
+        #         return self._t1
+        #     mem1 = psutil.virtual_memory().available if psutil is not None else 1
+        #     self._mem1 = mem0 - mem1
+        #     self.params[self.ITER_HP] = min(n_iter, 4)
+        #     self._t2 = self._fit(df_train, **_kwargs)
+        #     mem2 = psutil.virtual_memory().available if psutil is not None else 1
+        #     self._mem2 = max(mem0 - mem2, self._mem1)
+        #     self._mem_per_iter = min(self._mem1, self._mem2 / self.params[self.ITER_HP])
+        #     self._time_per_iter = (
+        #         (self._t2 - self._t1) / (self.params[self.ITER_HP] - 1)
+        #         if self._t2 > self._t1
+        #         else self._t1
+        #         if self._t1
+        #         else 0.001
+        #     )
+        #     self._train_size = df_train.count()
+        #     if (
+        #         budget is not None
+        #         and self._t1 + self._t2 >= budget
+        #         or n_iter == self.params[self.ITER_HP]
+        #     ):
+        #         # self.params[self.ITER_HP] = n_iter
+        #         return time.time() - start_time
+        #     trained = True
+        # if n_iter > 1:
+        #     max_iter = min(
+        #         n_iter,
+        #         int(
+        #             (budget - time.time() + start_time - self._t1) / self._time_per_iter
+        #             + 1
+        #         )
+        #         if budget is not None
+        #         else n_iter,
+        #     )
+        #     if trained and max_iter <= self.params[self.ITER_HP]:
+        #         return time.time() - start_time
+        #     # when not trained, train at least one iter
+        #     self.params[self.ITER_HP] = max(max_iter, 1)
+        self._fit(df_train, **_kwargs)
+        train_time = time.time() - start_time
+        return train_time
+
+    def _fit(self, df_train: sparkDataFrame, **kwargs):
+        current_time = time.time()
+        model = self.estimator_class(**self.params, **kwargs)
+        if logger.level == logging.DEBUG:
+            logger.debug(f"flaml.model - {model} fit started with params {self.params}")
+        self._model = model.fit(df_train)
+        self._model.classes_ = self.model_classes_
+        self._model.n_classes_ = self.model_n_classes_
+        if logger.level == logging.DEBUG:
+            logger.debug(f"flaml.model - {model} fit finished")
+        train_time = time.time() - current_time
+        return train_time
+
+
 class TransformersEstimator(BaseEstimator):
     """The class for fine-tuning language models, using huggingface transformers API."""
 
     ITER_HP = "global_max_steps"
 
     def __init__(self, task="seq-classification", **config):
         super().__init__(task, **config)
@@ -563,17 +914,22 @@
                 self._training_args.model_path,
                 use_fast=True,
                 add_prefix_space=self._add_prefix_space,
             )
 
     @property
     def data_collator(self):
-        from .nlp.huggingface.data_collator import task_to_datacollator_class
+        from flaml.automl.task.task import Task
+        from flaml.automl.nlp.huggingface.data_collator import (
+            task_to_datacollator_class,
+        )
 
-        data_collator_class = task_to_datacollator_class.get(self._task)
+        data_collator_class = task_to_datacollator_class.get(
+            self._task.name if isinstance(self._task, Task) else self._task
+        )
 
         if data_collator_class:
             kwargs = {
                 "model": self._model_init(),
                 # need to set model, or there's ValueError: Expected input batch_size (..) to match target batch_size (..)
                 "label_pad_token_id": -100,  # pad with token id -100
                 "pad_to_multiple_of": 8,
@@ -721,18 +1077,16 @@
             ]
         self._trainer = None
 
         return time.time() - start_time
 
     def _delete_one_ckpt(self, ckpt_location):
         if self._use_ray is False:
-            try:
+            if os.path.exists(ckpt_location):
                 shutil.rmtree(ckpt_location)
-            except FileNotFoundError:
-                logger.warning("checkpoint {} not found".format(ckpt_location))
 
     def cleanup(self):
         super().cleanup()
         if hasattr(self, "_ckpt_remains"):
             for each_ckpt in self._ckpt_remains:
                 self._delete_one_ckpt(each_ckpt)
 
@@ -1482,16 +1836,20 @@
     """The class for tuning Extra Trees."""
 
     @classmethod
     def cost_relative2lgbm(cls):
         return 1.9
 
     def __init__(self, task="binary", **params):
+        if isinstance(task, str):
+            from flaml.automl.task.factory import task_factory
+
+            task = task_factory(task)
         super().__init__(task, **params)
-        if "regression" in task:
+        if task.is_regression():
             self.estimator_class = ExtraTreesRegressor
         else:
             self.estimator_class = ExtraTreesClassifier
 
 
 class LRL1Classifier(SKLearnEstimator):
     """The class for tuning Logistic Regression with L1 regularization."""
@@ -2015,14 +2373,102 @@
         with suppress_stdout_stderr():
             model = model.fit()
         train_time = time.time() - current_time
         self._model = model
         return train_time
 
 
+class HoltWinters(ARIMA):
+    """
+    The class for tuning Holt Winters model, aka 'Triple Exponential Smoothing'.
+    """
+
+    @classmethod
+    def search_space(cls, **params):
+        space = {
+            "damped_trend": {"domain": tune.choice([True, False]), "init_value": False},
+            "trend": {"domain": tune.choice(["add", "mul", None]), "init_value": "add"},
+            "seasonal": {
+                "domain": tune.choice(["add", "mul", None]),
+                "init_value": "add",
+            },
+            "use_boxcox": {"domain": tune.choice([False, True]), "init_value": False},
+            "seasonal_periods": {  # statsmodels casts this to None if "seasonal" is None
+                "domain": tune.choice(
+                    [7, 12, 4, 52, 6]
+                ),  # weekly, yearly, quarterly, weekly w yearly data
+                "init_value": 7,
+            },
+        }
+        return space
+
+    def fit(self, X_train, y_train, budget=None, free_mem_ratio=0, **kwargs):
+        import warnings
+
+        warnings.filterwarnings("ignore")
+        from statsmodels.tsa.holtwinters import (
+            ExponentialSmoothing as HWExponentialSmoothing,
+        )
+
+        current_time = time.time()
+        train_df = self._join(X_train, y_train)
+        train_df = self._preprocess(train_df)
+        regressors = list(train_df)
+        regressors.remove(TS_VALUE_COL)
+        if regressors:
+            logger.warning("Regressors are ignored for Holt-Winters ETS models.")
+
+        # Override incompatible parameters
+        if (
+            X_train.shape[0] < 2 * self.params["seasonal_periods"]
+        ):  # this would prevent heuristic initialization to work properly
+            self.params["seasonal"] = None
+        if (
+            self.params["seasonal"] == "mul" and (train_df.y == 0).sum() > 0
+        ):  # cannot have multiplicative seasonality in this case
+            self.params["seasonal"] = "add"
+        if self.params["trend"] == "mul" and (train_df.y == 0).sum() > 0:
+            self.params["trend"] = "add"
+
+        if not self.params["seasonal"] or not self.params["trend"] in [
+            "mul",
+            "add",
+        ]:
+            self.params["damped_trend"] = False
+
+        model = HWExponentialSmoothing(
+            train_df[[TS_VALUE_COL]],
+            damped_trend=self.params["damped_trend"],
+            seasonal=self.params["seasonal"],
+            trend=self.params["trend"],
+        )
+        with suppress_stdout_stderr():
+            model = model.fit()
+        train_time = time.time() - current_time
+        self._model = model
+        return train_time
+
+    def predict(self, X, **kwargs):
+        if self._model is not None:
+            if isinstance(X, int):
+                forecast = self._model.forecast(steps=X)
+            elif isinstance(X, DataFrame):
+                start = X[TS_TIMESTAMP_COL].iloc[0]
+                end = X[TS_TIMESTAMP_COL].iloc[-1]
+                forecast = self._model.predict(start=start, end=end, **kwargs)
+            else:
+                raise ValueError(
+                    "X needs to be either a pandas Dataframe with dates as the first column"
+                    " or an int number of periods for predict()."
+                )
+            return forecast
+        else:
+            return np.ones(X if isinstance(X, int) else X.shape[0])
+
+
 class TS_SKLearn(SKLearnEstimator):
     """The class for tuning SKLearn Regressors for time-series forecasting, using hcrystalball"""
 
     base_class = SKLearnEstimator
 
     @classmethod
     def search_space(cls, data_size, pred_horizon, **params):
@@ -2118,19 +2564,15 @@
                     (
                         X_pred,
                         _,
                     ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(
                         X.iloc[:i, :]
                     )
                     preds.append(self._model[i - 1].predict(X_pred, **kwargs)[-1])
-                forecast = DataFrame(
-                    data=np.asarray(preds).reshape(-1, 1),
-                    columns=[self.hcrystaball_model.name],
-                    index=X.index,
-                )
+                forecast = Series(preds)
             else:
                 (
                     X_pred,
                     _,
                 ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(X)
                 forecast = self._model.predict(X_pred, **kwargs)
             return forecast
```

### Comparing `FLAML-1.1.3/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-1.2.0/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from transformers.data.data_collator import (
     DataCollatorWithPadding,
     DataCollatorForTokenClassification,
     DataCollatorForSeq2Seq,
 )
 from collections import OrderedDict
 
-from flaml.automl.data import (
+from flaml.automl.task.task import (
     TOKENCLASSIFICATION,
     MULTICHOICECLASSIFICATION,
     SUMMARIZATION,
     SEQCLASSIFICATION,
     SEQREGRESSION,
 )
```

### Comparing `FLAML-1.1.3/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-1.2.0/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-1.2.0/flaml/automl/nlp/huggingface/training_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
 from dataclasses import dataclass, field
 
-from flaml.automl.data import (
-    NLG_TASKS,
-)
+from flaml.automl.task.task import NLG_TASKS
 from typing import Optional, List
 
 try:
     from transformers import TrainingArguments
 except ImportError:
     TrainingArguments = object
```

### Comparing `FLAML-1.1.3/flaml/automl/nlp/huggingface/utils.py` & `FLAML-1.2.0/flaml/automl/nlp/huggingface/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from itertools import chain
 import numpy as np
 
-from flaml.automl.data import (
+from flaml.automl.task.task import (
     SUMMARIZATION,
     SEQREGRESSION,
     SEQCLASSIFICATION,
     MULTICHOICECLASSIFICATION,
     TOKENCLASSIFICATION,
     NLG_TASKS,
 )
@@ -398,15 +398,19 @@
 
 def load_model(checkpoint_path, task, num_labels=None):
     import transformers
 
     transformers.logging.set_verbosity_error()
 
     from transformers import AutoConfig
-    from ...data import SEQCLASSIFICATION, SEQREGRESSION, TOKENCLASSIFICATION
+    from flaml.automl.task.task import (
+        SEQCLASSIFICATION,
+        SEQREGRESSION,
+        TOKENCLASSIFICATION,
+    )
 
     def get_this_model(checkpoint_path, task, model_config):
         from transformers import AutoModelForSequenceClassification
         from transformers import AutoModelForSeq2SeqLM
         from transformers import AutoModelForMultipleChoice
         from transformers import AutoModelForTokenClassification
```

### Comparing `FLAML-1.1.3/flaml/automl/nlp/utils.py` & `FLAML-1.2.0/flaml/automl/nlp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Any
 import numpy as np
 
-from flaml.automl.data import (
+from flaml.automl.task.task import (
     SUMMARIZATION,
     SEQREGRESSION,
     SEQCLASSIFICATION,
     MULTICHOICECLASSIFICATION,
     TOKENCLASSIFICATION,
 )
```

### Comparing `FLAML-1.1.3/flaml/automl/training_log.py` & `FLAML-1.2.0/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/default/all/binary.json` & `FLAML-1.2.0/flaml/default/all/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1410,8 +1410,8 @@
 00005810: 652f 4865 6c65 6e61 222c 0a20 2020 2020  e/Helena",.     
 00005820: 2020 2022 6578 7472 615f 7472 6565 2f6b     "extra_tree/k
 00005830: 722d 7673 2d6b 7022 2c0a 2020 2020 2020  r-vs-kp",.      
 00005840: 2020 2265 7874 7261 5f74 7265 652f 6261    "extra_tree/ba
 00005850: 6e6b 2d6d 6172 6b65 7469 6e67 222c 0a20  nk-marketing",. 
 00005860: 2020 2020 2020 2022 6578 7472 615f 7472         "extra_tr
 00005870: 6565 2f64 6566 6175 6c74 220a 2020 2020  ee/default".    
-00005880: 5d0a 7d                                  ].}
+00005880: 5d0a 7d0a                                ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/all/multiclass.json` & `FLAML-1.2.0/flaml/default/all/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -2124,8 +2124,8 @@
 000084b0: 652f 436f 7665 7274 7970 6522 2c0a 2020  e/Covertype",.  
 000084c0: 2020 2020 2020 2265 7874 7261 5f74 7265        "extra_tre
 000084d0: 652f 416d 617a 6f6e 5f65 6d70 6c6f 7965  e/Amazon_employe
 000084e0: 655f 6163 6365 7373 222c 0a20 2020 2020  e_access",.     
 000084f0: 2020 2022 6578 7472 615f 7472 6565 2f66     "extra_tree/f
 00008500: 7269 6564 222c 0a20 2020 2020 2020 2022  ried",.        "
 00008510: 6578 7472 615f 7472 6565 2f64 6566 6175  extra_tree/defau
-00008520: 6c74 220a 2020 2020 5d0a 7d              lt".    ].}
+00008520: 6c74 220a 2020 2020 5d0a 7d0a            lt".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/all/regression.json` & `FLAML-1.2.0/flaml/default/all/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1344,8 +1344,8 @@
 000053f0: 7265 652f 686f 7573 655f 3136 4822 2c0a  ree/house_16H",.
 00005400: 2020 2020 2020 2020 2265 7874 7261 5f74          "extra_t
 00005410: 7265 652f 6465 6661 756c 7422 2c0a 2020  ree/default",.  
 00005420: 2020 2020 2020 2265 7874 7261 5f74 7265        "extra_tre
 00005430: 652f 6469 6c62 6572 7422 2c0a 2020 2020  e/dilbert",.    
 00005440: 2020 2020 2265 7874 7261 5f74 7265 652f      "extra_tree/
 00005450: 7061 7274 6963 756c 6174 652d 6d61 7474  particulate-matt
-00005460: 6572 220a 2020 2020 5d0a 7d              er".    ].}
+00005460: 6572 220a 2020 2020 5d0a 7d0a            er".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/estimator.py` & `FLAML-1.2.0/flaml/default/estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sklearn.ensemble as ensemble
 from functools import wraps
-from flaml.automl.data import CLASSIFICATION
+from flaml.automl.task.task import CLASSIFICATION
 from .suggest import preprocess_and_suggest_hyperparams
 
 DEFAULT_LOCATION = "default_location"
 
 
 def flamlize_estimator(super_class, name: str, task: str, alternatives=None):
     """Enhance an estimator class with flaml's data-dependent default hyperparameter settings.
```

### Comparing `FLAML-1.1.3/flaml/default/extra_tree/binary.json` & `FLAML-1.2.0/flaml/default/extra_tree/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -494,8 +494,8 @@
 00001ed0: 6f6e 6669 6773 6f75 7263 6522 3a20 5b0a  onfigsource": [.
 00001ee0: 2020 2020 2020 2020 2273 6567 6d65 6e74          "segment
 00001ef0: 222c 0a20 2020 2020 2020 2022 4865 6c65  ",.        "Hele
 00001f00: 6e61 222c 0a20 2020 2020 2020 2022 6b72  na",.        "kr
 00001f10: 2d76 732d 6b70 222c 0a20 2020 2020 2020  -vs-kp",.       
 00001f20: 2022 6261 6e6b 2d6d 6172 6b65 7469 6e67   "bank-marketing
 00001f30: 222c 0a20 2020 2020 2020 2022 6465 6661  ",.        "defa
-00001f40: 756c 7422 0a20 2020 205d 0a7d            ult".    ].}
+00001f40: 756c 7422 0a20 2020 205d 0a7d 0a         ult".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/extra_tree/multiclass.json` & `FLAML-1.2.0/flaml/default/extra_tree/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -416,8 +416,8 @@
 000019f0: 2268 6f75 7365 7322 2c0a 2020 2020 2020  "houses",.      
 00001a00: 2020 2266 6162 6572 7422 2c0a 2020 2020    "fabert",.    
 00001a10: 2020 2020 2243 6f76 6572 7479 7065 222c      "Covertype",
 00001a20: 0a20 2020 2020 2020 2022 416d 617a 6f6e  .        "Amazon
 00001a30: 5f65 6d70 6c6f 7965 655f 6163 6365 7373  _employee_access
 00001a40: 222c 0a20 2020 2020 2020 2022 6672 6965  ",.        "frie
 00001a50: 6422 2c0a 2020 2020 2020 2020 2264 6566  d",.        "def
-00001a60: 6175 6c74 220a 2020 2020 5d0a 7d         ault".    ].}
+00001a60: 6175 6c74 220a 2020 2020 5d0a 7d0a       ault".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/extra_tree/regression.json` & `FLAML-1.2.0/flaml/default/extra_tree/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -406,8 +406,8 @@
 00001950: 2020 2263 6f6e 6669 6773 6f75 7263 6522    "configsource"
 00001960: 3a20 5b0a 2020 2020 2020 2020 2268 6f75  : [.        "hou
 00001970: 7365 5f31 3648 222c 0a20 2020 2020 2020  se_16H",.       
 00001980: 2022 6465 6661 756c 7422 2c0a 2020 2020   "default",.    
 00001990: 2020 2020 2264 696c 6265 7274 222c 0a20      "dilbert",. 
 000019a0: 2020 2020 2020 2022 7061 7274 6963 756c         "particul
 000019b0: 6174 652d 6d61 7474 6572 220a 2020 2020  ate-matter".    
-000019c0: 5d0a 7d                                  ].}
+000019c0: 5d0a 7d0a                                ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/greedy.py` & `FLAML-1.2.0/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/default/lgbm/binary.json` & `FLAML-1.2.0/flaml/default/lgbm/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -537,7 +537,8 @@
 00002180: 6773 6f75 7263 6522 3a20 5b0a 2020 2020  gsource": [.    
 00002190: 2020 2020 2241 6972 6c69 6e65 7322 2c0a      "Airlines",.
 000021a0: 2020 2020 2020 2020 2272 6963 6361 7264          "riccard
 000021b0: 6f22 2c0a 2020 2020 2020 2020 2266 7269  o",.        "fri
 000021c0: 6564 222c 0a20 2020 2020 2020 2022 4469  ed",.        "Di
 000021d0: 6f6e 6973 222c 0a20 2020 2020 2020 2022  onis",.        "
 000021e0: 6465 6661 756c 7422 0a20 2020 205d 0a7d  default".    ].}
+000021f0: 0a                                       .
```

### Comparing `FLAML-1.1.3/flaml/default/lgbm/multiclass.json` & `FLAML-1.2.0/flaml/default/lgbm/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -620,8 +620,8 @@
 000026b0: 2022 4a61 6e6e 6973 222c 0a20 2020 2020   "Jannis",.     
 000026c0: 2020 2022 6661 6265 7274 222c 0a20 2020     "fabert",.   
 000026d0: 2020 2020 2022 436f 7665 7274 7970 6522       "Covertype"
 000026e0: 2c0a 2020 2020 2020 2020 2273 6567 6d65  ,.        "segme
 000026f0: 6e74 222c 0a20 2020 2020 2020 2022 4150  nt",.        "AP
 00002700: 5346 6169 6c75 7265 222c 0a20 2020 2020  SFailure",.     
 00002710: 2020 2022 6465 6661 756c 7422 0a20 2020     "default".   
-00002720: 205d 0a7d                                 ].}
+00002720: 205d 0a7d 0a                              ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/lgbm/regression.json` & `FLAML-1.2.0/flaml/default/lgbm/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -385,8 +385,8 @@
 00001800: 2020 2020 2020 2020 7d0a 2020 2020 5d2c          }.    ],
 00001810: 0a20 2020 2022 636f 6e66 6967 736f 7572  .    "configsour
 00001820: 6365 223a 205b 0a20 2020 2020 2020 2022  ce": [.        "
 00001830: 686f 7573 6573 222c 0a20 2020 2020 2020  houses",.       
 00001840: 2022 686f 7573 655f 384c 222c 0a20 2020   "house_8L",.   
 00001850: 2020 2020 2022 706f 6b65 7222 2c0a 2020       "poker",.  
 00001860: 2020 2020 2020 2264 6566 6175 6c74 220a        "default".
-00001870: 2020 2020 5d0a 7d                            ].}
+00001870: 2020 2020 5d0a 7d0a                          ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/portfolio.py` & `FLAML-1.2.0/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/default/regret.py` & `FLAML-1.2.0/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/default/rf/binary.json` & `FLAML-1.2.0/flaml/default/rf/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -453,8 +453,8 @@
 00001c40: 2020 205d 2c0a 2020 2020 2263 6f6e 6669     ],.    "confi
 00001c50: 6773 6f75 7263 6522 3a20 5b0a 2020 2020  gsource": [.    
 00001c60: 2020 2020 2241 6d61 7a6f 6e5f 656d 706c      "Amazon_empl
 00001c70: 6f79 6565 5f61 6363 6573 7322 2c0a 2020  oyee_access",.  
 00001c80: 2020 2020 2020 226b 6331 222c 0a20 2020        "kc1",.   
 00001c90: 2020 2020 2022 4865 6c65 6e61 222c 0a20       "Helena",. 
 00001ca0: 2020 2020 2020 2022 6465 6661 756c 7422         "default"
-00001cb0: 0a20 2020 205d 0a7d                      .    ].}
+00001cb0: 0a20 2020 205d 0a7d 0a                   .    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/rf/multiclass.json` & `FLAML-1.2.0/flaml/default/rf/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -442,8 +442,8 @@
 00001b90: 2020 2246 6173 6869 6f6e 2d4d 4e49 5354    "Fashion-MNIST
 00001ba0: 222c 0a20 2020 2020 2020 2022 6a75 6e67  ",.        "jung
 00001bb0: 6c65 5f63 6865 7373 5f32 7063 735f 7261  le_chess_2pcs_ra
 00001bc0: 775f 656e 6467 616d 655f 636f 6d70 6c65  w_endgame_comple
 00001bd0: 7465 222c 0a20 2020 2020 2020 2022 4d69  te",.        "Mi
 00001be0: 6e69 426f 6f4e 4522 2c0a 2020 2020 2020  niBooNE",.      
 00001bf0: 2020 2264 6566 6175 6c74 220a 2020 2020    "default".    
-00001c00: 5d0a 7d                                  ].}
+00001c00: 5d0a 7d0a                                ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/rf/regression.json` & `FLAML-1.2.0/flaml/default/rf/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -391,8 +391,8 @@
 00001860: 0a20 2020 205d 2c0a 2020 2020 2263 6f6e  .    ],.    "con
 00001870: 6669 6773 6f75 7263 6522 3a20 5b0a 2020  figsource": [.  
 00001880: 2020 2020 2020 2268 6f75 7365 7322 2c0a        "houses",.
 00001890: 2020 2020 2020 2020 2270 6f6b 6572 222c          "poker",
 000018a0: 0a20 2020 2020 2020 2022 6261 6e6b 2d6d  .        "bank-m
 000018b0: 6172 6b65 7469 6e67 222c 0a20 2020 2020  arketing",.     
 000018c0: 2020 2022 6465 6661 756c 7422 0a20 2020     "default".   
-000018d0: 205d 0a7d                                 ].}
+000018d0: 205d 0a7d 0a                              ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/suggest.py` & `FLAML-1.2.0/flaml/default/suggest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,36 @@
+import os
 import numpy as np
 from sklearn.neighbors import NearestNeighbors
 import logging
 import pathlib
 import json
-from flaml.automl.data import CLASSIFICATION, DataTransformer
-from flaml.automl.ml import get_estimator_class, get_classification_objective
+from flaml.automl.data import DataTransformer
+from flaml.automl.task.task import CLASSIFICATION, get_classification_objective
+from flaml.automl.ml import get_estimator_class
 from flaml.version import __version__
 
+try:
+    from flaml.automl.spark.utils import len_labels
+except ImportError:
+    from flaml.automl.utils import len_labels
+try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
+    import pyspark.pandas as ps
+    from pyspark.pandas import DataFrame as psDataFrame, Series as psSeries
+except ImportError:
+    ps = None
+
+    class psDataFrame:
+        pass
+
+    class psSeries:
+        pass
+
+
 LOCATION = pathlib.Path(__file__).parent.resolve()
 logger = logging.getLogger(__name__)
 CONFIG_PREDICTORS = {}
 
 
 def version_parse(version):
     return tuple(map(int, (version.split("."))))
@@ -24,31 +44,35 @@
     is_classification = task in CLASSIFICATION
     for each_feature_name in meta_feature_names:
         if each_feature_name == "NumberOfInstances":
             this_feature.append(n_row)
         elif each_feature_name == "NumberOfFeatures":
             this_feature.append(n_feat)
         elif each_feature_name == "NumberOfClasses":
-            this_feature.append(len(np.unique(y_train)) if is_classification else 0)
+            this_feature.append(len_labels(y_train) if is_classification else 0)
         elif each_feature_name == "PercentageOfNumericFeatures":
             try:
-                # this is feature is only supported for dataframe
+                # this feature is only supported for dataframe
                 this_feature.append(
-                    X_train.select_dtypes(include=np.number).shape[1] / n_feat
+                    X_train.select_dtypes(
+                        include=[np.number, "float", "int", "long"]
+                    ).shape[1]
+                    / n_feat
                 )
             except AttributeError:
                 # 'numpy.ndarray' object has no attribute 'select_dtypes'
                 this_feature.append(1)  # all features are numeric
         else:
             raise ValueError("Feature {} not implemented. ".format(each_feature_name))
 
     return this_feature
 
 
 def load_config_predictor(estimator_name, task, location=None):
+    task = str(task)
     key = f"{location}/{estimator_name}/{task}"
     predictor = CONFIG_PREDICTORS.get(key)
     if predictor:
         return predictor
     task = "multiclass" if task == "multi" else task  # TODO: multi -> multiclass?
     try:
         location = location or LOCATION
@@ -57,23 +81,30 @@
     except FileNotFoundError:
         raise FileNotFoundError(
             f"Portfolio has not been built for {estimator_name} on {task} task."
         )
     return predictor
 
 
-def suggest_config(task, X, y, estimator_or_predictor, location=None, k=None, meta_feature_fn=meta_feature):
-
+def suggest_config(
+    task,
+    X,
+    y,
+    estimator_or_predictor,
+    location=None,
+    k=None,
+    meta_feature_fn=meta_feature,
+):
     """Suggest a list of configs for the given task and training data.
 
     The returned configs can be used as starting points for AutoML.fit().
     `FLAML_sample_size` is removed from the configs.
     """
     task = (
-        get_classification_objective(len(np.unique(y)))
+        get_classification_objective(len_labels(y))
         if task == "classification" and y is not None
         else task
     )
     predictor = (
         load_config_predictor(estimator_or_predictor, task, location)
         if isinstance(estimator_or_predictor, str)
         else estimator_or_predictor
```

### Comparing `FLAML-1.1.3/flaml/default/xgb_limitdepth/binary.json` & `FLAML-1.2.0/flaml/default/xgb_limitdepth/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -480,8 +480,8 @@
 00001df0: 205d 2c0a 2020 2020 2263 6f6e 6669 6773   ],.    "configs
 00001e00: 6f75 7263 6522 3a20 5b0a 2020 2020 2020  ource": [.      
 00001e10: 2020 224a 616e 6e69 7322 2c0a 2020 2020    "Jannis",.    
 00001e20: 2020 2020 2261 6475 6c74 222c 0a20 2020      "adult",.   
 00001e30: 2020 2020 2022 416d 617a 6f6e 5f65 6d70       "Amazon_emp
 00001e40: 6c6f 7965 655f 6163 6365 7373 222c 0a20  loyee_access",. 
 00001e50: 2020 2020 2020 2022 6465 6661 756c 7422         "default"
-00001e60: 0a20 2020 205d 0a7d                      .    ].}
+00001e60: 0a20 2020 205d 0a7d 0a                   .    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-1.2.0/flaml/default/xgb_limitdepth/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -565,8 +565,8 @@
 00002340: 2022 4865 6c65 6e61 222c 0a20 2020 2020   "Helena",.     
 00002350: 2020 2022 436f 7665 7274 7970 6522 2c0a     "Covertype",.
 00002360: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
 00002370: 222c 0a20 2020 2020 2020 2022 636e 6165  ",.        "cnae
 00002380: 2d39 222c 0a20 2020 2020 2020 2022 7665  -9",.        "ve
 00002390: 6869 636c 6522 2c0a 2020 2020 2020 2020  hicle",.        
 000023a0: 226d 6665 6174 2d66 6163 746f 7273 220a  "mfeat-factors".
-000023b0: 2020 2020 5d0a 7d                            ].}
+000023b0: 2020 2020 5d0a 7d0a                          ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/xgb_limitdepth/regression.json` & `FLAML-1.2.0/flaml/default/xgb_limitdepth/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -509,8 +509,8 @@
 00001fc0: 2268 6967 6773 222c 0a20 2020 2020 2020  "higgs",.       
 00001fd0: 2022 626e 675f 7068 6172 796e 7822 2c0a   "bng_pharynx",.
 00001fe0: 2020 2020 2020 2020 2263 6f6e 6e65 6374          "connect
 00001ff0: 2d34 222c 0a20 2020 2020 2020 2022 686f  -4",.        "ho
 00002000: 7573 655f 3136 4822 2c0a 2020 2020 2020  use_16H",.      
 00002010: 2020 2262 6e67 5f65 6368 6f6d 6f6e 7468    "bng_echomonth
 00002020: 7322 2c0a 2020 2020 2020 2020 2264 6566  s",.        "def
-00002030: 6175 6c74 220a 2020 2020 5d0a 7d         ault".    ].}
+00002030: 6175 6c74 220a 2020 2020 5d0a 7d0a       ault".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/xgboost/binary.json` & `FLAML-1.2.0/flaml/default/xgboost/binary.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -555,8 +555,8 @@
 000022a0: 205d 2c0a 2020 2020 2263 6f6e 6669 6773   ],.    "configs
 000022b0: 6f75 7263 6522 3a20 5b0a 2020 2020 2020  ource": [.      
 000022c0: 2020 2266 6162 6572 7422 2c0a 2020 2020    "fabert",.    
 000022d0: 2020 2020 2262 6e67 5f6c 6f77 6277 7422      "bng_lowbwt"
 000022e0: 2c0a 2020 2020 2020 2020 2270 6f6c 222c  ,.        "pol",
 000022f0: 0a20 2020 2020 2020 2022 416d 617a 6f6e  .        "Amazon
 00002300: 5f65 6d70 6c6f 7965 655f 6163 6365 7373  _employee_access
-00002310: 220a 2020 2020 5d0a 7d                   ".    ].}
+00002310: 220a 2020 2020 5d0a 7d0a                 ".    ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/xgboost/multiclass.json` & `FLAML-1.2.0/flaml/default/xgboost/multiclass.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -816,8 +816,8 @@
 000032f0: 2020 2022 4b44 4443 7570 3039 5f61 7070     "KDDCup09_app
 00003300: 6574 656e 6379 222c 0a20 2020 2020 2020  etency",.       
 00003310: 2022 6661 6265 7274 222c 0a20 2020 2020   "fabert",.     
 00003320: 2020 2022 6469 6c62 6572 7422 2c0a 2020     "dilbert",.  
 00003330: 2020 2020 2020 226a 756e 676c 655f 6368        "jungle_ch
 00003340: 6573 735f 3270 6373 5f72 6177 5f65 6e64  ess_2pcs_raw_end
 00003350: 6761 6d65 5f63 6f6d 706c 6574 6522 0a20  game_complete". 
-00003360: 2020 205d 0a7d                              ].}
+00003360: 2020 205d 0a7d 0a                           ].}.
```

### Comparing `FLAML-1.1.3/flaml/default/xgboost/regression.json` & `FLAML-1.2.0/flaml/default/xgboost/regression.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -444,8 +444,8 @@
 00001bb0: 2020 2020 5d2c 0a20 2020 2022 636f 6e66      ],.    "conf
 00001bc0: 6967 736f 7572 6365 223a 205b 0a20 2020  igsource": [.   
 00001bd0: 2020 2020 2022 416c 6265 7274 222c 0a20       "Albert",. 
 00001be0: 2020 2020 2020 2022 6d76 222c 0a20 2020         "mv",.   
 00001bf0: 2020 2020 2022 626e 675f 6563 686f 6d6f       "bng_echomo
 00001c00: 6e74 6873 222c 0a20 2020 2020 2020 2022  nths",.        "
 00001c10: 686f 7573 655f 3136 4822 0a20 2020 205d  house_16H".    ]
-00001c20: 0a7d                                     .}
+00001c20: 0a7d 0a                                  .}.
```

### Comparing `FLAML-1.1.3/flaml/onlineml/autovw.py` & `FLAML-1.2.0/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/onlineml/trial.py` & `FLAML-1.2.0/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/onlineml/trial_runner.py` & `FLAML-1.2.0/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/__init__.py` & `FLAML-1.2.0/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/analysis.py` & `FLAML-1.2.0/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/result.py` & `FLAML-1.2.0/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/sample.py` & `FLAML-1.2.0/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/scheduler/online_scheduler.py` & `FLAML-1.2.0/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-1.2.0/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/blendsearch.py` & `FLAML-1.2.0/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/cfo_cat.py` & `FLAML-1.2.0/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/flow2.py` & `FLAML-1.2.0/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/online_searcher.py` & `FLAML-1.2.0/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/search_thread.py` & `FLAML-1.2.0/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/suggestion.py` & `FLAML-1.2.0/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/searcher/variant_generator.py` & `FLAML-1.2.0/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/space.py` & `FLAML-1.2.0/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/spark/utils.py` & `FLAML-1.2.0/flaml/tune/spark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from functools import lru_cache, partial
 
 
 logger = logging.getLogger(__name__)
 logger_formatter = logging.Formatter(
     "[%(name)s: %(asctime)s] {%(lineno)d} %(levelname)s - %(message)s", "%m-%d %H:%M:%S"
 )
-
+logger.propagate = False
 try:
+    os.environ["PYARROW_IGNORE_TIMEZONE"] = "1"
     import pyspark
     from pyspark.sql import SparkSession
     from pyspark.util import VersionUtils
     import py4j
 
     _have_spark = True
     _spark_major_minor_version = VersionUtils.majorMinorVersion(pyspark.__version__)
@@ -277,15 +278,16 @@
         if self.sc:
             self.sc.setLogLevel(level)
         else:
             pyspark.SparkContext.getOrCreate().setLogLevel(level)
 
     def __enter__(self):
         """Enter the context manager.
-        This will start a monitor thread if spark is available and force_cancel is True."""
+        This will start a monitor thread if spark is available and force_cancel is True.
+        """
         if self._force_cancel and _have_spark:
             self._monitor_daemon = threading.Thread(target=self._monitor_overtime)
             # logger.setLevel("INFO")
             logger.info("monitor started")
             self._setLogLevel("OFF")
             self._monitor_daemon.start()
```

### Comparing `FLAML-1.1.3/flaml/tune/trial.py` & `FLAML-1.2.0/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/trial_runner.py` & `FLAML-1.2.0/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/flaml/tune/tune.py` & `FLAML-1.2.0/flaml/tune/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,15 @@
     max_failure: Optional[int] = 100,
     use_ray: Optional[bool] = False,
     use_spark: Optional[bool] = False,
     use_incumbent_result_in_evaluation: Optional[bool] = None,
     log_file_name: Optional[str] = None,
     lexico_objectives: Optional[dict] = None,
     force_cancel: Optional[bool] = False,
+    n_concurrent_trials: Optional[int] = 0,
     **ray_args,
 ):
     """The trigger for HPO.
 
     Example:
 
     ```python
@@ -433,14 +434,22 @@
     lexico_objectives = {
         "metrics": ["error_rate", "pred_time"],
         "modes": ["min", "min"],
         "tolerances": {"error_rate": "5%", "pred_time": "0%"},
         "targets": {"error_rate": 0.0},
     }
     ```
+        force_cancel: boolean, default=False | Whether to forcely cancel the PySpark job if overtime.
+        n_concurrent_trials: int, default=0 | The number of concurrent trials when perform hyperparameter
+            tuning with Spark. Only valid when use_spark=True and spark is required:
+            `pip install flaml[spark]`. Please check
+            [here](https://spark.apache.org/docs/latest/api/python/getting_started/install.html)
+            for more details about installing Spark. When tune.run() is called from AutoML, it will be
+            overwritten by the value of `n_concurrent_trials` in AutoML. When <= 0, the concurrent trials
+            will be set to the number of executors.
         **ray_args: keyword arguments to pass to ray.tune.run().
             Only valid when use_ray=True.
     """
     global _use_ray
     global _verbose
     global _running_trial
     global _training_iteration
@@ -670,26 +679,38 @@
         variable `FLAML_MAX_CONCURRENT` to override the detected `num_executors`.
 
         `max_concurrent` is the maximum number of concurrent trials defined by `search_alg`,
         `FLAML_MAX_CONCURRENT` will also be used to override `max_concurrent` if `search_alg`
         is not an instance of `ConcurrencyLimiter`.
 
         The final number of concurrent trials is the minimum of `max_concurrent` and
-        `num_executors`.
+        `num_executors` if `n_concurrent_trials<=0` (default, automl cases), otherwise the
+        minimum of `max_concurrent` and `n_concurrent_trials` (tuning cases).
         """
-        num_executors = max(num_executors, int(os.getenv("FLAML_MAX_CONCURRENT", 1)), 1)
         time_start = time.time()
+        try:
+            FLAML_MAX_CONCURRENT = int(os.getenv("FLAML_MAX_CONCURRENT", 0))
+            num_executors = max(num_executors, FLAML_MAX_CONCURRENT, 1)
+        except ValueError:
+            FLAML_MAX_CONCURRENT = 0
+        max_spark_parallelism = (
+            min(spark.sparkContext.defaultParallelism, FLAML_MAX_CONCURRENT)
+            if FLAML_MAX_CONCURRENT > 0
+            else spark.sparkContext.defaultParallelism
+        )
         if scheduler:
             scheduler.set_search_properties(metric=metric, mode=mode)
         if isinstance(search_alg, ConcurrencyLimiter):
             max_concurrent = max(1, search_alg.max_concurrent)
         else:
-            max_concurrent = max(1, int(os.getenv("FLAML_MAX_CONCURRENT", 1)))
-
-        n_concurrent_trials = min(num_executors, max_concurrent)
+            max_concurrent = max(1, max_spark_parallelism)
+        n_concurrent_trials = min(
+            n_concurrent_trials if n_concurrent_trials > 0 else num_executors,
+            max_concurrent,
+        )
         with parallel_backend("spark"):
             with Parallel(
                 n_jobs=n_concurrent_trials, verbose=max(0, (verbose - 1) * 50)
             ) as parallel:
                 try:
                     _runner = SparkTrialRunner(
                         search_alg=search_alg,
```

### Comparing `FLAML-1.1.3/flaml/tune/utils.py` & `FLAML-1.2.0/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/setup.py` & `FLAML-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     extras_require={
         "notebook": [
             "jupyter",
             "matplotlib",
             "openml==0.10.2",
         ],
         "spark": [
-            "pyspark>=3.0.0",
+            "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
         ],
         "test": [
             "flake8>=3.8.4",
             "thop",
             "pytest>=6.1.1",
             "coverage>=5.3",
@@ -67,15 +67,15 @@
             "datasets",
             "nltk",
             "rouge_score",
             "hcrystalball==0.1.10",
             "seqeval",
             "pytorch-forecasting>=0.9.0,<=0.10.1",
             "mlflow",
-            "pyspark>=3.0.0",
+            "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
             "nbconvert",
             "nbformat",
             "ipykernel",
             "pytorch-lightning<1.9.1",  # test_forecast_panel
         ],
         "catboost": ["catboost>=0.26"],
@@ -88,15 +88,22 @@
         ],
         "nni": [
             "nni",
         ],
         "vw": [
             "vowpalwabbit>=8.10.0, <9.0.0",
         ],
-        "nlp": [
+        "hf": [
+            "transformers[torch]==4.26",
+            "datasets",
+            "nltk",
+            "rouge_score",
+            "seqeval",
+        ],
+        "nlp": [  # for backward compatibility; hf is the new option name
             "transformers[torch]==4.26",
             "datasets",
             "nltk",
             "rouge_score",
             "seqeval",
         ],
         "ts_forecast": [
@@ -109,16 +116,16 @@
             "holidays<0.14",  # to prevent installation error for prophet
             "prophet>=1.0.1",
             "statsmodels>=0.12.2",
             "hcrystalball==0.1.10",
             "pytorch-forecasting>=0.9.0",
         ],
         "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3"],
-        "openai": ["openai==0.23.1", "diskcache", "optuna==2.8.0"],
-        "synapse": ["joblibspark>=0.5.0", "optuna==2.8.0", "pyspark>=3.0.0"],
+        "openai": ["openai==0.27.4", "diskcache", "optuna==2.8.0"],
+        "synapse": ["joblibspark>=0.5.0", "optuna==2.8.0", "pyspark>=3.2.0"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

### Comparing `FLAML-1.1.3/test/test_autovw.py` & `FLAML-1.2.0/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/test/test_conda_distribution.py` & `FLAML-1.2.0/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/test/test_gpu.py` & `FLAML-1.2.0/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.1.3/test/test_model.py` & `FLAML-1.2.0/test/test_model.py`

 * *Files identical despite different names*

