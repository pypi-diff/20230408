# Comparing `tmp/ml-starter-0.0.6.tar.gz` & `tmp/ml-starter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.6.tar", last modified: Fri Apr  7 17:49:49 2023, max compression
+gzip compressed data, was "ml-starter-0.0.7.tar", last modified: Fri Apr  7 22:47:01 2023, max compression
```

## Comparing `ml-starter-0.0.6.tar` & `ml-starter-0.0.7.tar`

### file list

```diff
@@ -1,149 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.768759 ml-starter-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 17:49:36.000000 ml-starter-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 17:49:49.768759 ml-starter-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-07 17:49:36.000000 ml-starter-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.736759 ml-starter-0.0.6/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.740759 ml-starter-0.0.6/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.740759 ml-starter-0.0.6/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.744759 ml-starter-0.0.6/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.744759 ml-starter-0.0.6/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.744759 ml-starter-0.0.6/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.748759 ml-starter-0.0.6/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.748759 ml-starter-0.0.6/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.748759 ml-starter-0.0.6/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.752759 ml-starter-0.0.6/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.752759 ml-starter-0.0.6/ml/tasks/datasets/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/impl/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/impl/pretraining.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/impl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/impl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.752759 ml-starter-0.0.6/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.756759 ml-starter-0.0.6/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.756759 ml-starter-0.0.6/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.756759 ml-starter-0.0.6/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.756759 ml-starter-0.0.6/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.760759 ml-starter-0.0.6/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/cpu_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.760759 ml-starter-0.0.6/ml/trainers/mixins/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.768759 ml-starter-0.0.6/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-07 17:49:36.000000 ml-starter-0.0.6/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:49:49.768759 ml-starter-0.0.6/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-07 17:49:49.000000 ml-starter-0.0.6/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-07 17:49:36.000000 ml-starter-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 17:49:36.000000 ml-starter-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 17:49:36.000000 ml-starter-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 17:49:49.768759 ml-starter-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 17:49:36.000000 ml-starter-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 22:46:49.000000 ml-starter-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 22:47:01.902388 ml-starter-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-07 22:46:49.000000 ml-starter-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.870387 ml-starter-0.0.7/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.874387 ml-starter-0.0.7/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.878388 ml-starter-0.0.7/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.878388 ml-starter-0.0.7/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.882387 ml-starter-0.0.7/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.886387 ml-starter-0.0.7/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.890388 ml-starter-0.0.7/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.890388 ml-starter-0.0.7/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.894388 ml-starter-0.0.7/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.894388 ml-starter-0.0.7/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/cpu_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.898388 ml-starter-0.0.7/ml/trainers/mixins/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-07 22:46:49.000000 ml-starter-0.0.7/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:47:01.902388 ml-starter-0.0.7/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-07 22:47:01.000000 ml-starter-0.0.7/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-07 22:46:49.000000 ml-starter-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 22:46:49.000000 ml-starter-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 22:46:49.000000 ml-starter-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 22:47:01.906388 ml-starter-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 22:46:49.000000 ml-starter-0.0.7/setup.py
```

### Comparing `ml-starter-0.0.6/PKG-INFO` & `ml-starter-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.6
+Version: 0.0.7
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.6/README.md` & `ml-starter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/core/config.py` & `ml-starter-0.0.7/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/core/env.py` & `ml-starter-0.0.7/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/core/registry.py` & `ml-starter-0.0.7/ml/core/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,21 @@
         with Timer(f"building {reg_name} from '{cls.REGISTRY_LOCATIONS[reg_name]}'"):
             reg_obj = reg_cls(reg_cfg)
         if isinstance(reg_obj, BaseObjectWithPointers):
             reg_obj.set_raw_config(raw_config)
         return reg_obj
 
     @classmethod
+    def build_entry_non_null(cls, raw_config: DictConfig) -> Entry:
+        entry = cls.build_entry(raw_config)
+        if entry is None:
+            raise ValueError(f"Missing {cls.config_key()} in config")
+        return entry
+
+    @classmethod
     def update_config(cls, raw_config: DictConfig) -> None:
         if cls.config_key() not in raw_config:
             return
         reg_cfg = raw_config[cls.config_key()]
         reg_name = get_name(cls.config_key(), reg_cfg)
         _, reg_cfg_cls = cls.lookup(reg_name)
         reg_cfg = OmegaConf.merge(OmegaConf.structured(reg_cfg_cls), reg_cfg)
```

### Comparing `ml-starter-0.0.6/ml/core/state.py` & `ml-starter-0.0.7/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/loggers/base.py` & `ml-starter-0.0.7/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/loggers/meter.py` & `ml-starter-0.0.7/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/loggers/multi.py` & `ml-starter-0.0.7/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/loggers/stdout.py` & `ml-starter-0.0.7/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/loggers/tensorboard.py` & `ml-starter-0.0.7/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/base.py` & `ml-starter-0.0.7/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.7/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.7/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/linear.py` & `ml-starter-0.0.7/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.7/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.7/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/models/activations.py` & `ml-starter-0.0.7/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/models/base.py` & `ml-starter-0.0.7/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/models/init.py` & `ml-starter-0.0.7/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/models/norms.py` & `ml-starter-0.0.7/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/adam.py` & `ml-starter-0.0.7/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/adamw.py` & `ml-starter-0.0.7/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/adan.py` & `ml-starter-0.0.7/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/base.py` & `ml-starter-0.0.7/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/sgd.py` & `ml-starter-0.0.7/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/optimizers/shampoo.py` & `ml-starter-0.0.7/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/scripts/cli.py` & `ml-starter-0.0.7/ml/scripts/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Callable
 
 from omegaconf import DictConfig
 
 from ml.core.env import add_global_tag, set_project_root
 from ml.core.registry import Objects
-from ml.scripts import compiler, mp_train, stage, train
+from ml.scripts import compiler, mp_train, resolve, stage, train
 from ml.utils.cli import parse_cli
 from ml.utils.colors import colorize
 from ml.utils.distributed import get_rank_optional, get_world_size_optional
 from ml.utils.logging import configure_logging
 from ml.utils.random import set_random_seed
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -27,31 +27,32 @@
 
     set_random_seed()
 
     without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
         "compile": compiler.compile_main,
         "mp_train": mp_train.mp_train_main,
         "stage": stage.stage_main,
+        "resolve": resolve.resolve_main,
     }
 
     with_objects_scripts: dict[str, Callable[[Objects], None]] = {
         "train": train.train_main,
     }
 
     scripts: dict[str, Callable[..., None]] = {**with_objects_scripts, **without_objects_scripts}
 
     def show_help() -> None:
         script_names = (colorize(script_name, "cyan") for script_name in scripts)
         print(f"Usage: ml < {' / '.join(script_names)} > ...\n", file=sys.stderr)
         for key, func in sorted(scripts.items()):
             if func.__doc__ is None:
-                print(f"* {colorize(key, 'green')}", file=sys.stderr)
+                print(f" ↪ {colorize(key, 'green')}", file=sys.stderr)
             else:
                 docstring = func.__doc__.strip().split("\n")[0]
-                print(f"* {colorize(key, 'green')}: {docstring}", file=sys.stderr)
+                print(f" ↪ {colorize(key, 'green')}: {docstring}", file=sys.stderr)
         print()
         sys.exit(1)
 
     # Parses the raw command line options.
     args = sys.argv[1:]
     if len(args) == 0:
         show_help()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.0.6/ml/scripts/compiler.py` & `ml-starter-0.0.7/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/scripts/stage.py` & `ml-starter-0.0.7/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/scripts/train.py` & `ml-starter-0.0.7/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/base.py` & `ml-starter-0.0.7/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.7/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.7/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/collate.py` & `ml-starter-0.0.7/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.7/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/impl/utils.py` & `ml-starter-0.0.7/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.7/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.7/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.7/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.7/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.7/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/environments/base.py` & `ml-starter-0.0.7/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/environments/utils.py` & `ml-starter-0.0.7/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/environments/worker.py` & `ml-starter-0.0.7/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/losses/reduce.py` & `ml-starter-0.0.7/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/rl/base.py` & `ml-starter-0.0.7/ml/tasks/rl/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import logging
 import multiprocessing as mp
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Generic, Iterator, TypeVar, overload
+from typing import Generic, Iterator, Literal, TypeVar, overload
 
 import numpy as np
 import torch
 import tqdm
 from omegaconf import MISSING
 from torch import Tensor
 from torch.utils.data.dataset import Dataset
@@ -268,69 +268,139 @@
         return state.num_epoch_steps >= self.config.dataset.num_update_steps
 
     @overload
     def sample_clip(
         self,
         *,
         save_path: str | Path,
+        return_images: Literal[True] = True,
+        return_states: Literal[False] = False,
         model: ModelT | None = None,
         writer: Writer = "ffmpeg",
         use_tqdm: bool = True,
+        standardize_images: bool = True,
+        optimal: bool = True,
     ) -> None:
         ...
 
     @overload
     def sample_clip(
         self,
         *,
+        return_images: Literal[True] = True,
+        return_states: Literal[False] = False,
         model: ModelT | None = None,
         use_tqdm: bool = True,
+        standardize_images: bool = True,
+        optimal: bool = True,
     ) -> Tensor:
         ...
 
+    @overload
+    def sample_clip(
+        self,
+        *,
+        return_images: Literal[True] = True,
+        return_states: Literal[True],
+        model: ModelT | None = None,
+        use_tqdm: bool = True,
+        standardize_images: bool = True,
+        optimal: bool = True,
+    ) -> tuple[Tensor, list[tuple[RLState, RLAction]]]:
+        ...
+
+    @overload
+    def sample_clip(
+        self,
+        *,
+        return_images: Literal[False],
+        return_states: Literal[True],
+        model: ModelT | None = None,
+        use_tqdm: bool = True,
+        optimal: bool = True,
+    ) -> list[tuple[RLState, RLAction]]:
+        ...
+
     def sample_clip(
         self,
         *,
         save_path: str | Path | None = None,
+        return_images: bool = True,
+        return_states: bool = False,
         model: ModelT | None = None,
         writer: Writer = "ffmpeg",
         use_tqdm: bool = True,
-    ) -> Tensor | None:
+        standardize_images: bool = True,
+        optimal: bool = True,
+    ) -> Tensor | list[tuple[RLState, RLAction]] | tuple[Tensor, list[tuple[RLState, RLAction]]] | None:
         """Samples a clip for a given model.
 
         Args:
             save_path: Where to save the sampled clips
+            return_images: Whether to return the images
+            return_states: Whether to return the states
             model: The model to sample from; if not provided, samples actions
                 randomly from the model
             writer: The writer to use to save the clip
             use_tqdm: Whether to use tqdm to display the progress
+            standardize_images: Whether to standardize the images
+            optimal: Whether to sample actions optimally
 
         Returns:
             The sampled clip, if `save_path` is not provided, otherwise `None`
             (the clip is saved to `save_path`).
+
+        Raises:
+            ValueError: If `save_path` is provided and `return_states` is `True`
         """
 
         env_cfg = self.config.environment
 
-        def iter_environment() -> Iterator[np.ndarray | Tensor]:
-            environment = self.get_environment_cached()
+        if not return_states and not return_images:
+            raise ValueError("Must return states, images or both")
+
+        environment = self.get_environment_cached()
+
+        def iter_states() -> Iterator[tuple[RLState, RLAction]]:
             state = environment.reset()
             if environment.terminated(state):
                 raise RuntimeError("Initial state is terminated")
             iterator = tqdm.trange(env_cfg.max_steps) if use_tqdm else range(env_cfg.max_steps)
             for i in iterator:
                 if environment.terminated(state):
                     logger.info("Terminating environment early, after %d / %d steps", i, env_cfg.max_steps)
                     break
                 if model is None:
                     action = environment.sample_action()
                 else:
-                    (action,) = self.get_actions(model, [state], True)
+                    (action,) = self.get_actions(model, [state], optimal)
                 state = environment.step(action)
+                yield (state, action)
+
+        def iter_images() -> Iterator[np.ndarray | Tensor]:
+            for state, _ in iter_states():
                 yield environment.render(state)
 
+        def iter_images_and_states() -> Iterator[tuple[np.ndarray | Tensor, tuple[RLState, RLAction]]]:
+            for state, action in iter_states():
+                image = environment.render(state)
+                if standardize_images:
+                    image = standardize_image(image)
+                yield image, (state, action)
+
         if save_path is None:
-            images_np = [standardize_image(image) for image in iter_environment()]
+            if return_images and return_states:
+                images, states = zip(*iter_images_and_states())
+                images_np = [standardize_image(image) for image in images]
+                return torch.from_numpy(np.stack(images_np)), list(states)
+
+            if return_states:
+                return list(iter_states())
+
+            images_np = [standardize_image(image) for image in iter_images()]
             return torch.from_numpy(np.stack(images_np))
 
-        VIDEO_WRITERS[writer](iter_environment(), save_path)
+        if return_states:
+            raise ValueError("Cannot return states when saving to a file")
+
+        VIDEO_WRITERS[writer](iter_images(), save_path)
         return None
```

### Comparing `ml-starter-0.0.6/ml/tasks/rl/replay.py` & `ml-starter-0.0.7/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/tasks/sl/base.py` & `ml-starter-0.0.7/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/base.py` & `ml-starter-0.0.7/ml/trainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,16 +188,15 @@
     else:
         new_first += [get_diff_string(prefix, first)]
         new_second += [get_diff_string(prefix, second)]
 
     return new_first, new_second
 
 
-def save_config(exp_dir: Path, raw_config: DictConfig) -> None:
-    config_path = exp_dir / "config.yaml"
+def save_config(config_path: Path, raw_config: DictConfig) -> None:
     if config_path.exists():
         added_keys, deleted_keys = diff_configs(raw_config, cast(DictConfig, OmegaConf.load(config_path)))
         if added_keys or deleted_keys:
             change_lines: list[str] = []
             change_lines += [f" ↪ {colorize('+', 'green')} {added_key}" for added_key in added_keys]
             change_lines += [f" ↪ {colorize('-', 'red')} {deleted_key}" for deleted_key in deleted_keys]
             change_summary = "\n".join(change_lines)
@@ -273,28 +272,36 @@
         sublogger.initialize(self.log_dir)
         self.loggers += [sublogger]
 
     def add_loggers(self, subloggers: list[BaseLogger]) -> None:
         for sublogger in subloggers:
             self.add_logger(sublogger)
 
+    @property
+    def config_path(self) -> Path:
+        return self.exp_dir / "config.yaml"
+
     def save_config(self) -> None:
-        save_config(self.exp_dir, self.raw_config)
+        save_config(self.config_path, self.raw_config)
 
     def add_lock_file(self, lock_type: LockType, *, exists_ok: bool = False) -> None:
         add_lock_file(self.exp_dir, lock_type=lock_type, exists_ok=exists_ok)
         logger.debug("Added %s lock file to experiment directory %s", lock_type, self.exp_dir)
 
     def remove_lock_file(self, lock_type: LockType, *, missing_ok: bool = False) -> None:
         if remove_lock_file(self.exp_dir, lock_type=lock_type, missing_ok=missing_ok):
             logger.debug("Removed %s lock file in %s", lock_type, self.exp_dir)
 
     def get_ckpt_path(self, state: State | None = None) -> Path:
         return get_ckpt_path(self.exp_dir, state)
 
+    @property
+    def ckpt_path(self) -> Path:
+        return self.get_ckpt_path()
+
     def should_checkpoint(self, state: State) -> bool:
         if self.checkpoint_config.save_every_n_steps is not None:
             if state.num_steps % self.checkpoint_config.save_every_n_steps == 0:
                 return True
         return False
 
     def load_checkpoint(
```

### Comparing `ml-starter-0.0.6/ml/trainers/ddp.py` & `ml-starter-0.0.7/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.7/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/device/auto.py` & `ml-starter-0.0.7/ml/trainers/mixins/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/device/base.py` & `ml-starter-0.0.7/ml/trainers/mixins/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/device/cpu.py` & `ml-starter-0.0.7/ml/trainers/mixins/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/device/gpu.py` & `ml-starter-0.0.7/ml/trainers/mixins/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/device/metal.py` & `ml-starter-0.0.7/ml/trainers/mixins/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.7/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.7/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.7/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.7/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.7/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/rl.py` & `ml-starter-0.0.7/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/sl.py` & `ml-starter-0.0.7/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/slurm.py` & `ml-starter-0.0.7/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/trainers/vanilla.py` & `ml-starter-0.0.7/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/argparse.py` & `ml-starter-0.0.7/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/atomic.py` & `ml-starter-0.0.7/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/augmentation.py` & `ml-starter-0.0.7/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/caching.py` & `ml-starter-0.0.7/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/call_train.py` & `ml-starter-0.0.7/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/cli.py` & `ml-starter-0.0.7/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/colors.py` & `ml-starter-0.0.7/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/compiler.py` & `ml-starter-0.0.7/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/data.py` & `ml-starter-0.0.7/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/datetime.py` & `ml-starter-0.0.7/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/distributed.py` & `ml-starter-0.0.7/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/io.py` & `ml-starter-0.0.7/ml/utils/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
-def check_built(obj: T | None, name: str) -> T:
-    if obj is None:
-        raise RuntimeError(f"Could not build {name}")
-    return obj
-
-
 def get_checkpoint_path(
     trainer: DummyBaseTrainer,
     config_path: str | Path,
     ckpt_path: str | Path | None,
 ) -> Path:
     if ckpt_path is not None:
         ckpt_path = Path(ckpt_path)
@@ -36,59 +30,72 @@
     # Tries loading the checkpoint that the trainer thinks exists.
     ckpt_path = trainer.get_ckpt_path()
     if ckpt_path.exists():
         return ckpt_path
     logger.warning("Could not find trainer checkpoint at %s", ckpt_path)
 
     # Tries loading other checkpoints.
-    ckpt_path = trainer.exp_dir / "ckpt.pt"
+    config_path = Path(config_path)
+    ckpt_path = config_path.parent / "ckpt.pt"
     if ckpt_path.exists():
         return ckpt_path
     logger.warning("Could not find checkpoint at %s", ckpt_path)
 
     # Searches for a checkpoint in the same directory as the config.
-    config_path = Path(config_path)
     ckpt_paths = list(config_path.parent.rglob("ckpt*.pt"))
     if ckpt_paths:
         return max(ckpt_paths, key=lambda p: p.stat().st_mtime)
     logger.warning("Could not find checkpoints in config directory %s", config_path.parent)
 
     raise RuntimeError("Could not find a checkpoint to load")
 
 
 def load_model_and_task(
     config_path: str | Path,
     ckpt_path: str | Path | None = None,
     to_device: bool = True,
+    missing_ckpt_okay: bool = False,
 ) -> tuple[BaseModel, BaseTask]:
     """Loads a trained checkpoint from a config, and optional checkpoint path.
 
     Args:
         config_path: The path to the config file.
         ckpt_path: The path to the checkpoint file; if None, the latest
             checkpoint will be used. This defaults to first checking in an
             adjacent `checkpoints` directory for a `ckpt.pt` file, or else
             checking for the checkpoint file in the same directory as the
             config.
         to_device: Whether to move the model to the device specified in the
             config.
+        missing_ckpt_okay: Whether to return a model and task even if the
+            checkpoint is missing.
 
     Returns:
         The model and task loaded from the checkpoint
+
+    Raises:
+        RuntimeError: If the checkpoint is missing and `missing_ckpt_okay` is
+            False.
     """
 
     with Timer("loading checkpoint"):
         config = cast(DictConfig, OmegaConf.load(config_path))
-        model = check_built(register_model.build_entry(config), "model")
-        task = check_built(register_task.build_entry(config), "task")
-        trainer = DummyBaseTrainer(config)
+        model = register_model.build_entry_non_null(config)
+        task = register_task.build_entry_non_null(config)
+        trainer = DummyBaseTrainer(config.trainer)
 
         # Uses the dummy trainer to load the checkpoint.
-        ckpt_path = get_checkpoint_path(trainer, config_path, ckpt_path)
-        trainer.load_checkpoint(ckpt_path, task, model)
+        try:
+            ckpt_path = get_checkpoint_path(trainer, config_path, ckpt_path)
+            trainer.load_checkpoint(ckpt_path, task, model)
+        except RuntimeError:
+            if missing_ckpt_okay:
+                logger.exception("Could not load checkpoint")
+            else:
+                raise
 
         if to_device:
             device = AutoDevice.detect_device()
             device.module_to(model)
             device.module_to(task)
 
     return model, task
```

### Comparing `ml-starter-0.0.6/ml/utils/large_models.py` & `ml-starter-0.0.7/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/logging.py` & `ml-starter-0.0.7/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/meter.py` & `ml-starter-0.0.7/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/timer.py` & `ml-starter-0.0.7/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml/utils/video.py` & `ml-starter-0.0.7/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.7/ml_starter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.6
+Version: 0.0.7
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.6/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.7/ml_starter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,33 +43,30 @@
 ml/optimizers/sgd.py
 ml/optimizers/shampoo.py
 ml/optimizers/types.py
 ml/scripts/__init__.py
 ml/scripts/cli.py
 ml/scripts/compiler.py
 ml/scripts/mp_train.py
+ml/scripts/resolve.py
 ml/scripts/stage.py
 ml/scripts/train.py
 ml/tasks/__init__.py
 ml/tasks/base.py
 ml/tasks/datasets/__init__.py
 ml/tasks/datasets/async_iterable.py
 ml/tasks/datasets/clippify.py
 ml/tasks/datasets/collate.py
 ml/tasks/datasets/error_handling.py
 ml/tasks/datasets/multi_iter.py
 ml/tasks/datasets/samplers.py
 ml/tasks/datasets/streaming.py
 ml/tasks/datasets/transforms.py
+ml/tasks/datasets/utils.py
 ml/tasks/datasets/video_file.py
-ml/tasks/datasets/impl/__init__.py
-ml/tasks/datasets/impl/kinetics.py
-ml/tasks/datasets/impl/pretraining.py
-ml/tasks/datasets/impl/types.py
-ml/tasks/datasets/impl/utils.py
 ml/tasks/environments/__init__.py
 ml/tasks/environments/base.py
 ml/tasks/environments/utils.py
 ml/tasks/environments/worker.py
 ml/tasks/losses/__init__.py
 ml/tasks/losses/reduce.py
 ml/tasks/rl/__init__.py
```

### Comparing `ml-starter-0.0.6/pyproject.toml` & `ml-starter-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.6/setup.py` & `ml-starter-0.0.7/setup.py`

 * *Files identical despite different names*

