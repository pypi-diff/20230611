# Comparing `tmp/ml-starter-0.0.52.tar.gz` & `tmp/ml-starter-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.52.tar", last modified: Wed Jun  7 00:25:36 2023, max compression
+gzip compressed data, was "ml-starter-0.0.54.tar", last modified: Sun Jun 11 15:56:31 2023, max compression
```

## Comparing `ml-starter-0.0.52.tar` & `ml-starter-0.0.54.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.211776 ml-starter-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 00:25:21.000000 ml-starter-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 00:25:21.000000 ml-starter-0.0.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 00:25:36.211776 ml-starter-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 00:25:21.000000 ml-starter-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.199776 ml-starter-0.0.52/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.203776 ml-starter-0.0.52/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47531 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.203776 ml-starter-0.0.52/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.203776 ml-starter-0.0.52/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.203776 ml-starter-0.0.52/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.203776 ml-starter-0.0.52/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.207776 ml-starter-0.0.52/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.211776 ml-starter-0.0.52/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.211776 ml-starter-0.0.52/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-07 00:25:21.000000 ml-starter-0.0.52/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:25:36.211776 ml-starter-0.0.52/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 00:25:36.000000 ml-starter-0.0.52/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-07 00:25:36.000000 ml-starter-0.0.52/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:25:36.000000 ml-starter-0.0.52/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-07 00:25:36.000000 ml-starter-0.0.52/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 00:25:36.000000 ml-starter-0.0.52/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-07 00:25:21.000000 ml-starter-0.0.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 00:25:21.000000 ml-starter-0.0.52/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 00:25:21.000000 ml-starter-0.0.52/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 00:25:21.000000 ml-starter-0.0.52/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 00:25:36.215776 ml-starter-0.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-07 00:25:21.000000 ml-starter-0.0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.428037 ml-starter-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 15:56:19.000000 ml-starter-0.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 15:56:19.000000 ml-starter-0.0.54/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-11 15:56:31.428037 ml-starter-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-11 15:56:19.000000 ml-starter-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.412037 ml-starter-0.0.54/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.412037 ml-starter-0.0.54/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.412037 ml-starter-0.0.54/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.416037 ml-starter-0.0.54/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.420037 ml-starter-0.0.54/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.424037 ml-starter-0.0.54/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.424037 ml-starter-0.0.54/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.428037 ml-starter-0.0.54/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-11 15:56:19.000000 ml-starter-0.0.54/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:56:31.428037 ml-starter-0.0.54/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-11 15:56:31.000000 ml-starter-0.0.54/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-11 15:56:31.000000 ml-starter-0.0.54/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:56:31.000000 ml-starter-0.0.54/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-11 15:56:31.000000 ml-starter-0.0.54/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 15:56:31.000000 ml-starter-0.0.54/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-11 15:56:19.000000 ml-starter-0.0.54/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 15:56:19.000000 ml-starter-0.0.54/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-11 15:56:19.000000 ml-starter-0.0.54/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 15:56:19.000000 ml-starter-0.0.54/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 15:56:31.428037 ml-starter-0.0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-11 15:56:19.000000 ml-starter-0.0.54/setup.py
```

### Comparing `ml-starter-0.0.52/LICENSE` & `ml-starter-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/PKG-INFO` & `ml-starter-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.52
+Version: 0.0.54
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.52/README.md` & `ml-starter-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/api.py` & `ml-starter-0.0.54/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
     "SupervisedLearningTrainerConfig",
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
     "test_environment",
     "timeout",
     "Timer",
+    "TokenReader",
+    "TokenWriter",
     "transforms",
     "VideoFileDataset",
     "WorkerPool",
     "write_audio",
     "write_gif",
     "write_video",
 ]
@@ -282,14 +284,15 @@
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
 from ml.utils.parallel import init_parallelism, parallel_group_info, parallelism_is_initialized, reset_parallelism
 from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
+from ml.utils.tokens import TokenReader, TokenWriter
 from ml.utils.torch_distributed import (
     MultiprocessConfig,
     get_distributed_backend,
     init_and_run,
     init_dist,
     launch_subprocesses,
     set_distributed_backend,
```

### Comparing `ml-starter-0.0.52/ml/core/common_types.py` & `ml-starter-0.0.54/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/core/config.py` & `ml-starter-0.0.54/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/core/env.py` & `ml-starter-0.0.54/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/core/registry.py` & `ml-starter-0.0.54/ml/core/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,11 +660,11 @@
         )
 
         logger.info("%s", objs.summarize())
 
         return objs
 
     @classmethod
-    def from_config_file(cls, config_path: str | Path, **overrides: Any) -> "Objects":
+    def from_config_file(cls, config_path: str | Path, **overrides: Any) -> "Objects":  # noqa: ANN401
         config = OmegaConf.load(config_path)
         config = OmegaConf.merge(config, DictConfig(overrides))
         return cls.parse_raw_config(cast(DictConfig, config))
```

### Comparing `ml-starter-0.0.52/ml/core/state.py` & `ml-starter-0.0.54/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/launchers/base.py` & `ml-starter-0.0.54/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/launchers/mp.py` & `ml-starter-0.0.54/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/launchers/slurm.py` & `ml-starter-0.0.54/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/launchers/torchrun.py` & `ml-starter-0.0.54/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/loggers/base.py` & `ml-starter-0.0.54/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/loggers/meter.py` & `ml-starter-0.0.54/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/loggers/multi.py` & `ml-starter-0.0.54/ml/loggers/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 """
 
 import functools
 import logging
 import math
 import re
 from collections import defaultdict
-from typing import Any, Callable, Iterator, Literal, Sequence, TypeVar
+from typing import Callable, Iterator, Literal, Sequence, TypeVar
 
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 from PIL import Image, ImageDraw, ImageFont
 from torch import Tensor
 from torchvision.transforms import InterpolationMode
 
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.utils.logging import IntervalTicker
 
 logger = logging.getLogger(__name__)
 
+T = TypeVar("T")
 LogT = TypeVar("LogT")
 Number = int | float | Tensor
 
 ChannelSelectMode = Literal["first", "last", "mean"]
 
 VALID_VIDEO_CHANNEL_COUNTS = {1, 3}
 VALID_AUDIO_CHANNEL_COUNTS = {1, 2}
@@ -538,17 +539,17 @@
     a, b = sep // 2, (sep + 1) // 2
     image_list = [F.pad(image, (a, b, a, b)) for image in image_list]
     wconcat = [torch.cat(image_list[i : i + wside], dim=-1) for i in range(0, len(image_list), wside)]
     new_image = torch.cat(wconcat, dim=-2)
     return new_image[..., a : new_image.shape[-2] - b, a : new_image.shape[-1] - b]
 
 
-def cast_fp32(value: Any) -> Any:
+def cast_fp32(value: T) -> T:
     if isinstance(value, Tensor) and value.is_floating_point():
-        value = value.detach().float().cpu()
+        return value.detach().float().cpu()  # type: ignore[return-value]
     return value
 
 
 class MultiLogger:
     """Defines an intermediate container which holds values to log somewhere else."""
 
     def __init__(self, default_namespace: str = DEFAULT_NAMESPACE) -> None:
```

### Comparing `ml-starter-0.0.52/ml/loggers/stdout.py` & `ml-starter-0.0.54/ml/loggers/stdout.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def format_number(value: int | float, precision: int) -> str:
     if isinstance(value, int):
         return str(value)
     return f"{value:.{precision}g}"
 
 
-def as_str(value: Any, precision: int) -> str:
+def as_str(value: Any, precision: int) -> str:  # noqa: ANN401
     if isinstance(value, str):
         return f'"{value}"'
     if isinstance(value, Tensor):
         value = value.detach().float().cpu().item()
     if isinstance(value, (int, float)):
         return format_number(value, precision)
     raise TypeError(f"Unexpected log type: {type(value)}")
```

### Comparing `ml-starter-0.0.52/ml/loggers/tensorboard.py` & `ml-starter-0.0.54/ml/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 logger: logging.Logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 WRITE_PROC_TEXT_EVERY_N_SECONDS: int = 60 * 2
 
 
-def format_as_string(value: Any) -> str:
+def format_as_string(value: Any) -> str:  # noqa: ANN401
     if isinstance(value, str):
         return value
     if isinstance(value, Tensor):
         value = value.detach().float().cpu().item()
     if isinstance(value, (int, float)):
         return f"{value:.4g}"
     if isinstance(value, bool):
```

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/base.py` & `ml-starter-0.0.54/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/constant.py` & `ml-starter-0.0.54/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.54/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.54/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/linear.py` & `ml-starter-0.0.54/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.54/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.54/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/activations.py` & `ml-starter-0.0.54/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/base.py` & `ml-starter-0.0.54/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/embeddings.py` & `ml-starter-0.0.54/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/init.py` & `ml-starter-0.0.54/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/kmeans.py` & `ml-starter-0.0.54/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/lora.py` & `ml-starter-0.0.54/ml/models/lora.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 def _lora_post_hook(module: "_Lora", incompatible_keys: _IncompatibleKeys) -> None:
     lora_keys = [k for k in incompatible_keys.missing_keys if k.split(".")[-1].startswith("lora_")]
     for lora_key in lora_keys:
         incompatible_keys.missing_keys.remove(lora_key)
 
 
 class _Lora(nn.Module):
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:  # noqa: ANN401
         super().__init__(*args, **kwargs)
 
         # This allows modules to use LoRA layers as drop-in replacements for
         # non-LoRA pretrained models without throwing annoying errors for
         # state dict incompatibility.
         self.register_load_state_dict_post_hook(_lora_post_hook)
```

### Comparing `ml-starter-0.0.52/ml/models/norms.py` & `ml-starter-0.0.54/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/models/parallel.py` & `ml-starter-0.0.54/ml/models/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,24 +69,28 @@
 
 from ml.models.init import InitializationType, init_
 from ml.utils.parallel import parallel_group_info
 
 
 class _ModelParallelCopy(torch.autograd.Function):
     @staticmethod
-    def forward(ctx: FunctionCtx, x: Tensor, op: Any) -> Tensor:  # type: ignore[override]
+    def forward(  # type: ignore[override]
+        ctx: FunctionCtx,
+        x: Tensor,
+        op: Any,  # noqa: ANN401
+    ) -> Tensor:
         ctx.op = op
         return x
 
     @staticmethod
     def backward(ctx: FunctionCtx, grad: Tensor) -> tuple[Tensor, None]:  # type: ignore[override]
         return parallel_group_info().mp.reduce(grad, op=ctx.op), None
 
 
-def mp_copy(x: Tensor, op: Any = ReduceOp.SUM) -> Tensor:
+def mp_copy(x: Tensor, op: Any = ReduceOp.SUM) -> Tensor:  # noqa: ANN401
     """Copies the input to the model parallel region.
 
     Forward this is a no-op, but backward it reduces the gradient across
     model parallel replicas (i.e., it is a cross-replica sum).
 
     Args:
         x: Input tensor, with shape ``(*)``.
@@ -96,24 +100,28 @@
         Output tensor, with shape ``(*)``.
     """
     return _ModelParallelCopy.apply(x, op)
 
 
 class _ModelParallelReduce(torch.autograd.Function):
     @staticmethod
-    def forward(ctx: FunctionCtx, x: Tensor, op: Any) -> Tensor:  # type: ignore[override]
+    def forward(  # type: ignore[override]
+        ctx: FunctionCtx,
+        x: Tensor,
+        op: Any,  # noqa: ANN401
+    ) -> Tensor:
         ctx.mark_dirty(x)
         return parallel_group_info().mp.reduce(x, op=op)
 
     @staticmethod
     def backward(ctx: FunctionCtx, grad: Tensor) -> tuple[Tensor, None]:  # type: ignore[override]
         return grad, None
 
 
-def mp_reduce(x: Tensor, op: Any = ReduceOp.SUM) -> Tensor:
+def mp_reduce(x: Tensor, op: Any = ReduceOp.SUM) -> Tensor:  # noqa: ANN401
     """Reduces the input from the model parallel region.
 
     Forward this reduces the input across model parallel replicas (i.e., it is
     a cross-replica sum), but backward it is a no-op.
 
     Args:
         x: Input tensor, with shape ``(*)``.
```

### Comparing `ml-starter-0.0.52/ml/optimizers/adam.py` & `ml-starter-0.0.54/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/adamw.py` & `ml-starter-0.0.54/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/adan.py` & `ml-starter-0.0.54/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/base.py` & `ml-starter-0.0.54/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/common.py` & `ml-starter-0.0.54/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/sgd.py` & `ml-starter-0.0.54/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/optimizers/shampoo.py` & `ml-starter-0.0.54/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/scripts/cli.py` & `ml-starter-0.0.54/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/scripts/stage.py` & `ml-starter-0.0.54/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/scripts/train.py` & `ml-starter-0.0.54/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/base.py` & `ml-starter-0.0.54/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.54/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.54/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/collate.py` & `ml-starter-0.0.54/ml/tasks/datasets/collate.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torchvision.transforms.functional as V
 from PIL.Image import Image as PILImage
 from torch import Tensor
 
 CollateMode = Literal["stack", "concat"]
 
 
-def is_named_tuple(obj: Any) -> bool:
+def is_named_tuple(obj: Any) -> bool:  # noqa: ANN401
     return isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
 
 
 def pad_sequence(
     tensors: list[Tensor],
     *,
     dim: int = 0,
@@ -207,11 +207,11 @@
 
 
 def collate_non_null(
     items: list[Any],
     *,
     mode: CollateMode | Callable[[list[Tensor]], Tensor] = "stack",
     pad: bool | Callable[[list[Tensor]], list[Tensor]] = False,
-) -> Any:
+) -> Any:  # noqa: ANN401
     collated = collate(items, mode=mode, pad=pad)
     assert collated is not None
     return collated
```

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.54/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.54/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.54/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.54/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.54/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/utils.py` & `ml-starter-0.0.54/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.54/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/environments/base.py` & `ml-starter-0.0.54/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/environments/utils.py` & `ml-starter-0.0.54/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/environments/worker.py` & `ml-starter-0.0.54/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/losses/reduce.py` & `ml-starter-0.0.54/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/rl/base.py` & `ml-starter-0.0.54/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/rl/replay.py` & `ml-starter-0.0.54/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/tasks/sl/base.py` & `ml-starter-0.0.54/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/base.py` & `ml-starter-0.0.54/ml/trainers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,20 +132,20 @@
         second: The second (new) config
         prefix: The prefix to check (used for recursion, not main call)
 
     Returns:
         Two lists of lines describing the diff between the two configs
     """
 
-    def get_diff_string(prefix: str | None, val: Any) -> str:
+    def get_diff_string(prefix: str | None, val: Any) -> str:  # noqa: ANN401
         if isinstance(val, (str, float, int)):
             return f"{prefix}={val}"
         return f"{prefix}= ... ({type(val)})"
 
-    def cast_enums(k: Any) -> Any:
+    def cast_enums(k: Any) -> Any:  # noqa: ANN401
         return k.name if isinstance(k, enum.Enum) else k
 
     new_first: list[str] = []
     new_second: list[str] = []
 
     any_config = (ListConfig, DictConfig)
```

### Comparing `ml-starter-0.0.52/ml/trainers/learning.py` & `ml-starter-0.0.54/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/compile.py` & `ml-starter-0.0.54/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.54/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.54/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.54/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.54/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.54/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.54/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.54/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.54/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.54/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/rl.py` & `ml-starter-0.0.54/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/trainers/sl.py` & `ml-starter-0.0.54/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/argparse.py` & `ml-starter-0.0.54/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/atomic.py` & `ml-starter-0.0.54/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/audio.py` & `ml-starter-0.0.54/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/augmentation.py` & `ml-starter-0.0.54/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/caching.py` & `ml-starter-0.0.54/ml/utils/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             func: The function to cache, which returns the object to load
 
         Returns:
             A cached version of the same function
         """
 
         @functools.wraps(func)
-        def call_function_cached(*args: Any, **kwargs: Any) -> Object:
+        def call_function_cached(*args: Any, **kwargs: Any) -> Object:  # noqa: ANN401
             if self.obj is not None:
                 return self.obj
 
             keys: list[str] = []
             for arg in args:
                 keys += [str(arg)]
             for key, val in sorted(kwargs.items()):
```

### Comparing `ml-starter-0.0.52/ml/utils/checkpoint.py` & `ml-starter-0.0.54/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/cli.py` & `ml-starter-0.0.54/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/colors.py` & `ml-starter-0.0.54/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/config.py` & `ml-starter-0.0.54/ml/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities for working with OmegaConf configs."""
 
 from typing import Any
 
 from omegaconf import MISSING, Container, OmegaConf
 
 
-def is_missing(cfg: Any, key: str) -> bool:
+def is_missing(cfg: Any, key: str) -> bool:  # noqa: ANN401
     """Utility function for checking if a config key is missing.
 
     This is for cases when you are using a raw dataclass rather than an
     OmegaConf container but want to treat them the same way.
 
     Args:
         cfg: The config to check
```

### Comparing `ml-starter-0.0.52/ml/utils/data.py` & `ml-starter-0.0.54/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/datetime.py` & `ml-starter-0.0.54/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/device/auto.py` & `ml-starter-0.0.54/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/device/base.py` & `ml-starter-0.0.54/ml/utils/device/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,46 +15,47 @@
     device.tensor_to(some_tensor)
     device.get_prefetcher(some_dataloader)
     device.recursive_apply(some_container, some_func)
 """
 
 import contextlib
 import functools
-import threading
 from abc import ABC, abstractmethod
 from dataclasses import is_dataclass
-from typing import Any, Callable, ContextManager, Iterable, Iterator, Mapping, Sequence
+from typing import Any, Callable, ContextManager, Iterable, Iterator, Mapping, Sequence, TypeVar
 
 import numpy as np
 import torch
 from torch import Tensor, nn
 from torch.utils.data.dataloader import DataLoader, _BaseDataLoaderIter
 
 from ml.core.common_types import Batch
 from ml.utils.timer import Timer
 
+T = TypeVar("T")
+
 
 def allow_nonblocking(device_a: torch.device, device_b: torch.device) -> bool:
     return device_a.type in ("cpu", "cuda") and device_b.type in ("cpu", "cuda")
 
 
-def recursive_apply(item: Any, func: Callable[[Tensor], Tensor]) -> Any:
+def recursive_apply(item: Any, func: Callable[[Tensor], Tensor]) -> Any:  # noqa: ANN401
     """Applies a function recursively to tensors in an item.
 
     Args:
         item: The item to apply the function to
         func: The function to apply (for the tensor)
 
     Returns:
         The same item, with the function applied
     """
     if isinstance(item, (str, int, float)):
         return item
     if isinstance(item, np.ndarray):
-        item = torch.from_numpy(item)
+        return func(torch.from_numpy(item))
     if isinstance(item, Tensor):
         return func(item)
     if is_dataclass(item):
         return item.__class__(**{k: recursive_apply(v, func) for k, v in item.__dict__.items()})
     if isinstance(item, Mapping):
         return {k: recursive_apply(v, func) for k, v in item.items()}
     if isinstance(item, Sequence):
@@ -75,45 +76,35 @@
 
         self.to_device_func = to_device_func
         self.dataloader = dataloader
         self.raise_stop_iter = raise_stop_iter
         self.next_sample = None
         self.get_batch_time = 0.0
         self.to_device_time = 0.0
-
-        # Start the dataloader in a separate thread.
-        self._dataloader_iter_ready = threading.Event()
         self._dataloader_iter: _BaseDataLoaderIter | None = None
-        threading.Thread(target=self.start_dataloader).start()
-
-    def start_dataloader(self) -> None:
-        self._dataloader_iter = iter(self.dataloader)
-        self._dataloader_iter_ready.set()
-        self.prefetch()
 
     @property
     def dataloader_iter(self) -> _BaseDataLoaderIter:
         if self._dataloader_iter is None:
             with Timer("starting dataloader", spinner=True):
-                self._dataloader_iter_ready.wait()
-                assert self._dataloader_iter is not None
+                self._dataloader_iter = iter(self.dataloader)
         return self._dataloader_iter
 
     def prefetch(self) -> None:
         try:
             with Timer("getting sample from dataloader") as timer:
                 next_sample = next(self.dataloader_iter)
             self.get_batch_time = timer.elapsed_time
             with Timer("moving sample to device") as timer:
                 self.next_sample = self.to_device_func(next_sample)
             self.to_device_time = timer.elapsed_time
         except StopIteration:
             self.next_sample = None
 
-    def recursive_chunk(self, item: Any, chunks: int) -> list[Any]:
+    def recursive_chunk(self, item: Any, chunks: int) -> list[Any]:  # noqa: ANN401
         """Applies a function recursively to tensors in an item.
 
         Args:
             item: The item to apply the function to
             chunks: The number of output chunks
 
         Returns:
@@ -135,15 +126,15 @@
             return [{k: v[i] for k, v in item_chunk_dict.items()} for i in range(chunks)]
         if isinstance(item, Sequence):
             item_chunk_lists = [self.recursive_chunk(i, chunks) for i in item]
             return [[k[i] for k in item_chunk_lists] for i in range(chunks)]
         return item
 
     @classmethod
-    def recursive_apply(cls, item: Any, func: Callable[[Tensor], Tensor]) -> Any:
+    def recursive_apply(cls, item: Any, func: Callable[[Tensor], Tensor]) -> Any:  # noqa: ANN401
         return recursive_apply(item, func)
 
     def __iter__(self) -> Iterator[Batch]:
         # Yields one sample quickly.
         next_sample = next(self.dataloader_iter)
         yield self.to_device_func(next_sample)
 
@@ -209,15 +200,15 @@
         """Returns the backend to use for Torch compile.
 
         Returns:
             The backend
         """
 
     @classmethod
-    def sample_to_device(cls, sample: Any) -> Any:
+    def sample_to_device(cls, sample: T) -> T:
         device = cls.get_device()
         dtype_fp = cls.get_floating_point_type()
         return Prefetcher.recursive_apply(
             sample,
             lambda t: t.to(
                 device,
                 dtype_fp if t.is_floating_point() else t.dtype,
@@ -239,21 +230,18 @@
             tensor = torch.from_numpy(tensor)
         device = cls.get_device()
         if tensor.is_floating_point():
             return tensor.to(device, cls.get_floating_point_type())
         return tensor.to(device)
 
     @classmethod
-    def recursive_apply(cls, item: Any) -> Any:
-        def func(i: Any) -> Any:
+    def recursive_apply(cls, item: T) -> T:
+        def func(i: Tensor) -> Tensor:
             if isinstance(i, Tensor):
                 return cls.tensor_to(i)
-            if isinstance(i, nn.Module):
-                cls.module_to(i)
-                return i
             return i
 
         return recursive_apply(item, func)
 
     @classmethod
     def autocast_context(cls, enabled: bool = True) -> ContextManager:
         device_type = cls.get_device().type
```

### Comparing `ml-starter-0.0.52/ml/utils/device/cpu.py` & `ml-starter-0.0.54/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/device/gpu.py` & `ml-starter-0.0.54/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/device/metal.py` & `ml-starter-0.0.54/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/distributed.py` & `ml-starter-0.0.54/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/image.py` & `ml-starter-0.0.54/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/large_models.py` & `ml-starter-0.0.54/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/logging.py` & `ml-starter-0.0.54/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/meter.py` & `ml-starter-0.0.54/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/parallel.py` & `ml-starter-0.0.54/ml/utils/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,22 +83,40 @@
 
     group: ProcessGroup
     global_ranks: list[int]
     rank: int
     world_size: int
 
     @overload
-    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: Literal[False] = False) -> Tensor:
+    def reduce(
+        self,
+        tensor: Tensor,
+        op: Any = ReduceOp.SUM,  # noqa: ANN401
+        *,
+        async_op: Literal[False] = False,
+    ) -> Tensor:
         ...
 
     @overload
-    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: Literal[True]) -> Work:
+    def reduce(
+        self,
+        tensor: Tensor,
+        op: Any = ReduceOp.SUM,  # noqa: ANN401
+        *,
+        async_op: Literal[True],
+    ) -> Work:
         ...
 
-    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: bool = False) -> Tensor | Work:
+    def reduce(
+        self,
+        tensor: Tensor,
+        op: Any = ReduceOp.SUM,
+        *,
+        async_op: bool = False,
+    ) -> Tensor | Work:  # noqa: ANN401
         """Reduces the tensor across all processes in the group.
 
         Consider two tensors in the same process group on different processes,
         with values ``[1, 2, 3]`` and ``[4, 5, 6]``. After calling this
         function, both tensors will have the value ``[5, 7, 9]``.
 
         Args:
```

### Comparing `ml-starter-0.0.52/ml/utils/staging.py` & `ml-starter-0.0.54/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/timer.py` & `ml-starter-0.0.54/ml/utils/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,30 +33,34 @@
         and is_master()
     )
 
 
 class Spinner:
     def __init__(self, text: str | None = None) -> None:
         self._text = "" if text is None else text
+        self._max_line_len = 0
         self._spinner_stop = False
         self._spinner_close = False
         self._flag = threading.Event()
         self._thread = Thread(target=self._spinner, daemon=True)
         self._thread.start()
 
         # If we're in a breakpoint, we want to close the spinner when we exit
         # the breakpoint.
         self._original_breakpointhook = sys.breakpointhook
 
-    def _breakpointhook(self, *args: Any, **kwargs: Any) -> None:
+    def _breakpointhook(self, *args: Any, **kwargs: Any) -> None:  # noqa: ANN401
         warnings.warn("Breakpoint hit inside spinner; run `up 1` to see where it was hit")
         self.stop()
         sys.breakpointhook(*args, **kwargs)
 
     def set_text(self, text: str) -> "Spinner":
+        sys.stderr.write(" " * (self._max_line_len + 1) + "\r")
+        sys.stderr.flush()
+        self._max_line_len = 0
         self._text = colorize(text, "grey")
         return self
 
     def start(self) -> None:
         self._spinner_stop = False
         self._flag.set()
         sys.breakpointhook = self._breakpointhook
@@ -73,22 +77,21 @@
     def _spinner(self) -> None:
         chars = [colorize(c, "light-yellow") for c in ("|", "/", "-", "\\")]
         while not self._spinner_close:
             self._flag.wait()
             start_time = time.time()
             while not self._spinner_stop:
                 time.sleep(0.1)
-                max_line_len = 0
                 char = chars[int((time.time() * 10) % len(chars))]
                 elapsed_secs = time.time() - start_time
                 line = f"[ {char} {elapsed_secs:.1f} ] {self._text}\r"
-                max_line_len = max(max_line_len, len(line))
+                self._max_line_len = max(self._max_line_len, len(line))
                 sys.stderr.write(line)
                 sys.stderr.flush()
-            sys.stderr.write(" " * (max_line_len + 1) + "\r")
+            sys.stderr.write(" " * (self._max_line_len + 1) + "\r")
             sys.stderr.flush()
             self._flag.clear()
 
 
 @functools.lru_cache
 def spinner() -> Spinner:
     return Spinner()
@@ -118,15 +121,15 @@
 
     def __enter__(self) -> "Timer":
         self._start_time = time.time()
         if self._use_spinner:
             spinner().set_text(self.description).start()
         return self
 
-    def __exit__(self, *args: Any, **kwargs: Any) -> None:
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:  # noqa: ANN401
         assert self._start_time is not None
         self._elapsed_time = time.time() - self._start_time
         if self._elapsed_time > self.min_seconds_to_print:
             self._logger.warning("Finished %s in %.3g seconds", self.description, self._elapsed_time)
         spinner().stop()
 
 
@@ -140,19 +143,19 @@
         error_message: Error message to pass to TimeoutError
 
     Returns:
         Decorator function
     """
 
     def decorator(func: TimeoutFunc) -> TimeoutFunc:
-        def _handle_timeout(*_: Any) -> None:
+        def _handle_timeout(*_: Any) -> None:  # noqa: ANN401
             raise TimeoutError(error_message)
 
         @functools.wraps(func)
-        def wrapper(*args: Any, **kwargs: Any) -> Any:
+        def wrapper(*args: Any, **kwargs: Any) -> Any:  # noqa: ANN401
             signal.signal(signal.SIGALRM, _handle_timeout)
             signal.alarm(seconds)
             try:
                 result = func(*args, **kwargs)
             finally:
                 signal.alarm(0)
             return result
```

### Comparing `ml-starter-0.0.52/ml/utils/torch_distributed.py` & `ml-starter-0.0.54/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml/utils/video.py` & `ml-starter-0.0.54/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.52/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.54/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.52
+Version: 0.0.54
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.52/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.54/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/parallel.py
 ml/utils/random.py
 ml/utils/staging.py
 ml/utils/timer.py
+ml/utils/tokens.py
 ml/utils/torch_distributed.py
 ml/utils/video.py
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
 ml/utils/device/cpu.py
 ml/utils/device/gpu.py
```

### Comparing `ml-starter-0.0.52/pyproject.toml` & `ml-starter-0.0.54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 
 warn_unused_ignores = true
 warn_redundant_casts = true
 
 incremental = true
 namespace_packages = false
 
-exclude = ["^ml/api.py$"]
-
 # For TorchScript stuff.
 disable_error_code = ["attr-defined"]
 
 [[tool.mypy.overrides]]
 
 module = [
     "av.*",
@@ -56,15 +54,15 @@
 profile = "black"
 
 [tool.ruff]
 
 select = ["ANN", "D", "E", "F", "I", "N", "PGH", "PLC", "PLE", "PLR", "PLW", "W"]
 
 ignore = [
-    "ANN101", "ANN102", "ANN401",
+    "ANN101", "ANN102",
     "D101", "D102", "D103", "D104", "D105", "D106", "D107",
     "N812", "N817",
     "PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004",
     "PLW0603", "PLW2901",
 ]
 
 line-length = 120
```

### Comparing `ml-starter-0.0.52/setup.py` & `ml-starter-0.0.54/setup.py`

 * *Files identical despite different names*

