# Comparing `tmp/ml-starter-0.0.24.tar.gz` & `tmp/ml-starter-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.24.tar", last modified: Wed Apr 26 21:40:08 2023, max compression
+gzip compressed data, was "ml-starter-0.0.25.tar", last modified: Tue May  2 21:28:22 2023, max compression
```

## Comparing `ml-starter-0.0.24.tar` & `ml-starter-0.0.25.tar`

### file list

```diff
@@ -1,151 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 21:39:56.000000 ml-starter-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 21:39:56.000000 ml-starter-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-26 21:40:08.886796 ml-starter-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 21:39:56.000000 ml-starter-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.866796 ml-starter-0.0.24/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.870796 ml-starter-0.0.24/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.874796 ml-starter-0.0.24/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.878796 ml-starter-0.0.24/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.882796 ml-starter-0.0.24/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-26 21:39:56.000000 ml-starter-0.0.24/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:40:08.886796 ml-starter-0.0.24/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-26 21:40:08.000000 ml-starter-0.0.24/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-26 21:39:56.000000 ml-starter-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 21:39:56.000000 ml-starter-0.0.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 21:40:08.886796 ml-starter-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-26 21:39:56.000000 ml-starter-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 21:28:05.000000 ml-starter-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 21:28:05.000000 ml-starter-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-02 21:28:22.834049 ml-starter-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-02 21:28:05.000000 ml-starter-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.818049 ml-starter-0.0.25/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23447 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-02 21:28:05.000000 ml-starter-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:28:22.834049 ml-starter-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-02 21:28:05.000000 ml-starter-0.0.25/setup.py
```

### Comparing `ml-starter-0.0.24/LICENSE` & `ml-starter-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/api.py` & `ml-starter-0.0.25/ml/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     "ClippifyDataset",
     "collate_non_null",
     "collate",
     "CollateMode",
     "colorize",
     "conf_field",
     "configure_logging",
-    "DDPTrainer",
+    "DDPLauncher",
+    "DDPLauncherConfig",
     "DictIndex",
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
     "get_args",
     "get_cache_dir",
@@ -101,39 +102,33 @@
     "reduce",
     "register_logger",
     "register_lr_scheduler",
     "register_model",
     "register_optimizer",
     "register_task",
     "register_trainer",
-    "ReinforcementLearningDDPTrainer",
-    "ReinforcementLearningSlurmTrainer",
-    "ReinforcementLearningSlurmTrainerConfig",
     "ReinforcementLearningTask",
     "ReinforcementLearningTaskConfig",
+    "ReinforcementLearningTrainer",
     "ReinforcementLearningTrainerConfig",
-    "ReinforcementLearningVanillaTrainer",
     "RotaryEmbeddings",
     "set_random_seed",
     "set_slurm_master_addr",
     "set_slurm_rank_and_world_size",
     "SinusoidalEmbeddings",
-    "SlurmTrainer",
-    "SlurmTrainerConfig",
+    "SlurmLauncher",
+    "SlurmLauncherConfig",
     "stage_environment",
     "State",
     "StreamingDataset",
     "StreamingDatasetNoIndex",
-    "SupervisedLearningDDPTrainer",
-    "SupervisedLearningSlurmTrainer",
-    "SupervisedLearningSlurmTrainerConfig",
     "SupervisedLearningTask",
     "SupervisedLearningTaskConfig",
+    "SupervisedLearningTrainer",
     "SupervisedLearningTrainerConfig",
-    "SupervisedLearningVanillaTrainer",
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
     "timeout",
     "Timer",
     "transforms",
     "VanillaTrainer",
@@ -162,14 +157,16 @@
     register_lr_scheduler,
     register_model,
     register_optimizer,
     register_task,
     register_trainer,
 )
 from ml.core.state import Phase, State
+from ml.launchers.ddp import DDPLauncher, DDPLauncherConfig
+from ml.launchers.slurm import SlurmLauncher, SlurmLauncherConfig, set_slurm_master_addr, set_slurm_rank_and_world_size
 from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
 from ml.models.activations import ActivationType, Clamp, cast_activation_type, get_activation
 from ml.models.base import BaseModel, BaseModelConfig
 from ml.models.embeddings import (
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
@@ -205,30 +202,16 @@
     SyncWorkerPool,
     WorkerPool,
 )
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
 from ml.tasks.rl.base import ReinforcementLearningTask, ReinforcementLearningTaskConfig
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
-from ml.trainers.ddp import DDPTrainer
-from ml.trainers.rl import (
-    ReinforcementLearningDDPTrainer,
-    ReinforcementLearningSlurmTrainer,
-    ReinforcementLearningSlurmTrainerConfig,
-    ReinforcementLearningTrainerConfig,
-    ReinforcementLearningVanillaTrainer,
-)
-from ml.trainers.sl import (
-    SupervisedLearningDDPTrainer,
-    SupervisedLearningSlurmTrainer,
-    SupervisedLearningSlurmTrainerConfig,
-    SupervisedLearningTrainerConfig,
-    SupervisedLearningVanillaTrainer,
-)
-from ml.trainers.slurm import SlurmTrainer, SlurmTrainerConfig, set_slurm_master_addr, set_slurm_rank_and_world_size
+from ml.trainers.rl import ReinforcementLearningTrainer, ReinforcementLearningTrainerConfig
+from ml.trainers.sl import SupervisedLearningTrainer, SupervisedLearningTrainerConfig
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import DictIndex, cached_object
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
```

### Comparing `ml-starter-0.0.24/ml/core/config.py` & `ml-starter-0.0.25/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/core/env.py` & `ml-starter-0.0.25/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/core/registry.py` & `ml-starter-0.0.25/ml/core/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from omegaconf.basecontainer import BaseContainer
 
 from ml.core.config import BaseConfig, BaseObject, BaseObjectWithPointers
 from ml.utils.colors import colorize
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
+    from ml.launchers.base import BaseLauncher, BaseLauncherConfig
     from ml.loggers.base import BaseLogger, BaseLoggerConfig
     from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
     from ml.models.base import BaseModel, BaseModelConfig
     from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
     from ml.tasks.base import BaseTask, BaseTaskConfig
     from ml.trainers.base import BaseTrainer, BaseTrainerConfig
 
@@ -450,23 +451,37 @@
         return Path("loggers")
 
     @classmethod
     def config_key(cls) -> str:
         return "logger"
 
 
+class register_launcher(register_base["BaseLauncher", "BaseLauncherConfig"]):  # pylint: disable=invalid-name
+    REGISTRY: dict[str, tuple[type["BaseLauncher"], type["BaseLauncherConfig"]]] = {}
+    REGISTRY_LOCATIONS: dict[str, Path] = {}
+
+    @classmethod
+    def search_directory(cls) -> Path:
+        return Path("launchers")
+
+    @classmethod
+    def config_key(cls) -> str:
+        return "launcher"
+
+
 @dataclass(frozen=True)
 class Objects:
     raw_config: DictConfig
     model: "BaseModel | None" = None
     task: "BaseTask | None" = None
     trainer: "BaseTrainer | None" = None
     optimizer: "BaseOptimizer | None" = None
     lr_scheduler: "BaseLRScheduler | None" = None
     logger: "list[BaseLogger] | None" = None
+    launcher: "BaseLauncher | None" = None
 
     def __post_init__(self) -> None:
         # After initializing the object container, we add a pointer to the
         # current container to each of the constructed objects.
         if self.task is not None:
             self.task.set_objects(self)
         if self.trainer is not None:
@@ -476,14 +491,16 @@
         if self.optimizer is not None:
             self.optimizer.set_objects(self)
         if self.lr_scheduler is not None:
             self.lr_scheduler.set_objects(self)
         if self.logger is not None:
             for sublogger in self.logger:
                 sublogger.set_objects(self)
+        if self.launcher is not None:
+            self.launcher.set_objects(self)
 
     def summarize(self) -> str:
         parts: dict[str, tuple[str, str]] = {}
         if self.model is not None:
             parts["Model"] = (
                 inspect.getfile(self.model.__class__),
                 f"{self.model.__class__.__module__}.{self.model.__class__.__name__}",
@@ -504,14 +521,19 @@
                 f"{self.optimizer.__class__.__module__}.{self.optimizer.__class__.__name__}",
             )
         if self.lr_scheduler is not None:
             parts["LR Scheduler"] = (
                 inspect.getfile(self.lr_scheduler.__class__),
                 f"{self.lr_scheduler.__class__.__module__}.{self.lr_scheduler.__class__.__name__}",
             )
+        if self.launcher is not None:
+            parts["Launcher"] = (
+                inspect.getfile(self.launcher.__class__),
+                f"{self.launcher.__class__.__module__}.{self.launcher.__class__.__name__}",
+            )
         return "Components:" + "".join(
             f"\n ↪ {colorize(k, 'green')}: {colorize(v[1], 'cyan')} ({colorize(v[0], 'blue')})"
             for k, v in parts.items()
         )
 
     @classmethod
     def resolve_config(cls, config: DictConfig) -> None:
@@ -525,26 +547,28 @@
             # Pre-builds the config using the structured configs.
             register_model.update_config(config)
             register_task.update_config(config)
             register_trainer.update_config(config)
             register_optimizer.update_config(config)
             register_lr_scheduler.update_config(config)
             register_logger.update_config(config)
+            register_launcher.update_config(config)
 
         with Timer("resolving configs", spinner=True):
             # Resolves the final config once all structured configs have been merged.
             OmegaConf.resolve(config)
 
             # Runs object-specific resolutions.
             register_model.resolve_config(config)
             register_task.resolve_config(config)
             register_trainer.resolve_config(config)
             register_optimizer.resolve_config(config)
             register_lr_scheduler.resolve_config(config)
             register_logger.resolve_config(config)
+            register_launcher.resolve_config(config)
 
     @classmethod
     def parse_raw_config(cls, config: DictConfig) -> "Objects":
         """Parses a raw config to the objects it contains.
 
         Args:
             config: The raw DictConfig to parse
@@ -561,23 +585,26 @@
             trainer = register_trainer.build_entry(config)
         with Timer("building optimizer", spinner=True):
             optimizer = register_optimizer.build_entry(config)
         with Timer("building lr scheduler", spinner=True):
             lr_scheduler = register_lr_scheduler.build_entry(config)
         with Timer("building loggers", spinner=True):
             loggers = register_logger.build_entry(config)
+        with Timer("building launcher", spinner=True):
+            launcher = register_launcher.build_entry(config)
 
         objs = Objects(
             raw_config=config,
             model=model,
             task=task,
             trainer=trainer,
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
             logger=loggers,
+            launcher=launcher,
         )
 
         logger.info("%s", objs.summarize())
 
         return objs
 
     @classmethod
```

### Comparing `ml-starter-0.0.24/ml/core/state.py` & `ml-starter-0.0.25/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/loggers/base.py` & `ml-starter-0.0.25/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/loggers/meter.py` & `ml-starter-0.0.25/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/loggers/multi.py` & `ml-starter-0.0.25/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/loggers/stdout.py` & `ml-starter-0.0.25/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/loggers/tensorboard.py` & `ml-starter-0.0.25/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/base.py` & `ml-starter-0.0.25/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.25/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.25/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/linear.py` & `ml-starter-0.0.25/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.25/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.25/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/models/activations.py` & `ml-starter-0.0.25/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/models/base.py` & `ml-starter-0.0.25/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/models/embeddings.py` & `ml-starter-0.0.25/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/models/init.py` & `ml-starter-0.0.25/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/models/norms.py` & `ml-starter-0.0.25/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/optimizers/adam.py` & `ml-starter-0.0.25/ml/optimizers/adam.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 @dataclass
 class AdamOptimizerConfig(BaseOptimizerConfig):
     lr: float = conf_field(1e-3, help="Learning rate")
     betas: tuple[float, float] = conf_field((0.9, 0.999), help="Beta coefficients")
     eps: float = conf_field(1e-4, help="Epsilon term to add to the denominator for stability")
     weight_decay: float = conf_field(0.0, help="Weight decay regularization to use")
     amsgrad: bool = conf_field(False, help="Whether to use the AMSGrad variant of the algorithm")
+    foreach: bool = conf_field(False, help="Whether to use the foreach variant of the optimizer")
+    capturable: bool = conf_field(False, help="Whether to use capturable AdamW pathway")
+    differentiable: bool = conf_field(False, help="Whether to use differentiable AdamW")
+    fused: bool = conf_field(False, help="Whether to use the fused optimizer")
 
 
 @register_optimizer("adam", AdamOptimizerConfig)
 class AdamOptimizer(BaseOptimizer[AdamOptimizerConfig]):
     def get(self, model: nn.Module) -> Adam:
         b1, b2 = self.config.betas
 
         return Adam(
             model.parameters(),
             lr=self.config.lr,
             betas=(b1, b2),
             eps=self.config.eps,
             weight_decay=self.config.weight_decay,
             amsgrad=self.config.amsgrad,
+            foreach=self.config.foreach,
+            capturable=self.config.capturable,
+            differentiable=self.config.differentiable,
+            fused=self.config.fused,
             **self.common_kwargs,
         )
```

### Comparing `ml-starter-0.0.24/ml/optimizers/adan.py` & `ml-starter-0.0.25/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/optimizers/base.py` & `ml-starter-0.0.25/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/optimizers/sgd.py` & `ml-starter-0.0.25/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/optimizers/shampoo.py` & `ml-starter-0.0.25/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/scripts/cli.py` & `ml-starter-0.0.25/ml/scripts/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import shlex
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable
 
+from ml.scripts import launch
 from ml.utils.distributed import get_rank_optional, get_world_size_optional
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
@@ -18,27 +19,27 @@
     configure_logging(rank=get_rank_optional(), world_size=get_world_size_optional())
     logger.info("Command: %s", shlex.join(sys.argv))
 
     # Import here to avoid slow startup time.
     with Timer("importing", spinner=True):
         from ml.core.env import add_global_tag
         from ml.core.registry import Objects, add_project_dir
-        from ml.scripts import compiler, mp_train, resolve, stage, train
+        from ml.scripts import compiler, resolve, stage, train
         from ml.utils.cli import parse_cli
         from ml.utils.colors import colorize
         from ml.utils.random import set_random_seed
 
     if project_root is not None:
         add_project_dir(Path(project_root).resolve())
 
     set_random_seed()
 
     without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
         "compile": compiler.compile_main,
-        "mp_train": mp_train.mp_train_main,
+        "launch": launch.launch_main,
         "stage": stage.stage_main,
         "resolve": resolve.resolve_main,
     }
 
     with_objects_scripts: dict[str, Callable[[Objects], None]] = {
         "train": train.train_main,
     }
```

### Comparing `ml-starter-0.0.24/ml/scripts/compiler.py` & `ml-starter-0.0.25/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/scripts/stage.py` & `ml-starter-0.0.25/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/scripts/train.py` & `ml-starter-0.0.25/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/base.py` & `ml-starter-0.0.25/ml/tasks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,25 +463,23 @@
 
     def on_after_compute_loss(self, model: ModelT, batch: Batch, output: Output, loss: Loss, state: State) -> None:
         pass
 
     def on_step_start(
         self,
         state: State,
-        train_batch: Batch,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
         pass
 
     def on_step_end(
         self,
         state: State,
-        train_batch: Batch,
         loss_dict: dict[str, Tensor],
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
         pass
```

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.25/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.25/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/collate.py` & `ml-starter-0.0.25/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.25/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.25/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.25/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.25/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.25/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/utils.py` & `ml-starter-0.0.25/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.25/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/environments/base.py` & `ml-starter-0.0.25/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/environments/utils.py` & `ml-starter-0.0.25/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/environments/worker.py` & `ml-starter-0.0.25/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/losses/reduce.py` & `ml-starter-0.0.25/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/rl/base.py` & `ml-starter-0.0.25/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/rl/replay.py` & `ml-starter-0.0.25/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/tasks/sl/base.py` & `ml-starter-0.0.25/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/trainers/base.py` & `ml-starter-0.0.25/ml/trainers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import enum
 import functools
 import logging
 import os
-from abc import ABC, abstractmethod
+import signal
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from pickle import UnpicklingError
-from typing import Any, Generic, Literal, TypeVar, cast, get_args
+from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
 
-from ml.core.common_types import Batch
 from ml.core.config import BaseConfig, BaseObjectWithPointers, conf_field
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
 from ml.models.base import BaseModel
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.base import BaseTask
 from ml.utils.colors import colorize
 from ml.utils.device.auto import AutoDevice
-from ml.utils.device.base import BaseDevice
+from ml.utils.device.base import BaseDevice, Prefetcher
 from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -237,28 +236,29 @@
 
 
 TrainerConfigT = TypeVar("TrainerConfigT", bound=BaseTrainerConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 TaskT = TypeVar("TaskT", bound=BaseTask)
 
 
-class BaseTrainer(BaseObjectWithPointers[TrainerConfigT], Generic[TrainerConfigT, ModelT, TaskT], ABC):
+class BaseTrainer(BaseObjectWithPointers[TrainerConfigT], Generic[TrainerConfigT, ModelT, TaskT]):
     """Defines the base trainer type."""
 
     logger: MultiLogger
     loggers: list[BaseLogger]
 
     def __init__(self, config: TrainerConfigT) -> None:
         super().__init__(config)
 
         self.exp_dir = get_exp_dir(Path(config.base_run_dir), config.exp_name, config.run_id)
         self.log_dir = self.exp_dir / config.log_dir_name
         self.checkpoint_config = config.checkpoint
         self.loggers = []
         self.logger = MultiLogger(default_namespace="trainer")
+        self.signal_handlers: dict[signal.Signals, list[Callable[[], None]]] = {}
 
         logger.info("Experiment directory: %s", self.exp_dir)
 
     @functools.cached_property
     def _device(self) -> type[BaseDevice]:
         return AutoDevice.detect_device()
 
@@ -408,29 +408,29 @@
                     last_ckpt_path.symlink_to(ckpt_path)
                 except FileExistsError:
                     logger.exception("Exception while trying to update %s", ckpt_path)
                 self.add_lock_file("ckpt", exists_ok=True)
                 task.on_after_save_checkpoint(ckpt_path)
         return ckpt_path
 
-    @abstractmethod
-    def launch(self) -> None:
-        """Launches a multiprocess command."""
-
-    @abstractmethod
     def train(self, model: ModelT, task: TaskT, optimizer: BaseOptimizer, lr_scheduler: BaseLRScheduler) -> None:
         """Runs the training loop.
 
         Args:
             model: The current model
             task: The current task
             optimizer: The current optimizer
             lr_scheduler: The current learning rate scheduler
+
+        Raises:
+            NotImplementedError: If the subclass does not implement this method
         """
 
+        raise NotImplementedError
+
     def write_logs(self, task: TaskT, model: ModelT, state: State) -> None:
         model.logger.write(self.loggers, state)
         task.logger.write(self.loggers, state)
         self.logger.write(self.loggers, state)
         for value_logger in self.loggers:
             if value_logger.should_write(state):
                 value_logger.write(state)
@@ -446,40 +446,59 @@
     def update_state_dict(self, ckpt: dict[str, Any]) -> None:
         """Function for getting the checkpoint to save.
 
         Args:
             ckpt: The checkpoint being saved (overriders should mutate inplace)
         """
 
+    def on_exit(
+        self,
+        sig: signal.Signals,
+        state: State,
+        task: TaskT,
+        model: ModelT,
+        optim: Optimizer,
+        lr_scheduler: SchedulerAdapter,
+    ) -> None:
+        logger.info("Handling interrupt %s", sig.name)
+        self.save_checkpoint(state, task, model, optim, lr_scheduler)
+        for signal_handler in self.signal_handlers.get(sig, []):
+            signal_handler()
+
+    def add_signal_handler(self, sig: signal.Signals, handler: Callable[[], None]) -> None:
+        self.signal_handlers[sig].append(handler)
+
+    def _log_prefetcher_stats(self, pf: Prefetcher) -> None:
+        self.logger.log_scalar("dt/get_batch", pf.get_batch_time, namespace="timers")
+        self.logger.log_scalar("dt/to_device", pf.to_device_time, namespace="timers")
+
     # -----
     # Hooks
     # -----
 
     def on_step_start(
         self,
         state: State,
-        train_batch: Batch,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
-        task.on_step_start(state, train_batch, model, optim, lr_sched)
+        task.on_step_start(state, model, optim, lr_sched)
 
     def on_step_end(
         self,
         state: State,
-        train_batch: Batch,
         loss_dict: dict[str, Tensor],
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
-        task.on_step_end(state, train_batch, loss_dict, model, optim, lr_sched)
+        task.on_step_end(state, loss_dict, model, optim, lr_sched)
 
     def on_epoch_start(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
@@ -515,21 +534,7 @@
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
         task.on_training_end(state, model, optim, lr_sched)
         self.remove_lock_file("running", missing_ok=True)
         logger.info("Exiting training job for %s", self.exp_dir / "config.yaml")
-
-
-class DummyBaseTrainer(BaseTrainer):
-    """Defines a dummy trainer that does nothing.
-
-    This trainer can be used to access the base trainer's utility functions,
-    such as saving and loading checkpoints.
-    """
-
-    def launch(self) -> None:
-        raise NotImplementedError
-
-    def train(self, model: ModelT, task: TaskT, optimizer: BaseOptimizer, lr_scheduler: BaseLRScheduler) -> None:
-        raise NotImplementedError
```

### Comparing `ml-starter-0.0.24/ml/trainers/ddp.py` & `ml-starter-0.0.25/ml/launchers/ddp.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 """
 
 import functools
 import logging
 import os
 import sys
 import traceback
-from abc import ABC
-from typing import Callable, Generic
+from dataclasses import dataclass
+from typing import Callable
 
+import torch
 import torch.multiprocessing as mp
 from omegaconf import DictConfig
-from torch import nn
 
-from ml.core.registry import Objects
+from ml.core.registry import Objects, register_launcher
+from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.scripts.train import train_main
-from ml.trainers.base import ModelT, MultiprocessConfig, TaskT
-from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfigT
+from ml.trainers.base import MultiprocessConfig
 from ml.utils.distributed import (
-    get_world_size,
     set_init_method,
     set_master_addr,
     set_master_port,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
@@ -64,27 +63,26 @@
     except KeyboardInterrupt:
         pass
     except Exception:
         error_queue.put(traceback.format_exc())
         sys.exit(1)
 
 
-class DDPTrainer(
-    VanillaTrainer[VanillaTrainerConfigT, ModelT, TaskT],
-    Generic[VanillaTrainerConfigT, ModelT, TaskT],
-    ABC,
-):
-    def get_task_model(self, task: TaskT, model: ModelT) -> nn.Module:
-        task_model = super().get_task_model(task, model)
-        if get_world_size() > 1:
-            task_model = nn.parallel.DistributedDataParallel(task_model)
-        return task_model
+@dataclass
+class DDPLauncherConfig(BaseLauncherConfig):
+    pass
 
+
+@register_launcher("ddp", DDPLauncherConfig)
+class DDPLauncher(BaseLauncher[DDPLauncherConfig]):
     def launch(self) -> None:
-        device_count = self._device.device_count()
+        if not torch.cuda.is_available():
+            raise RuntimeError("DDPLauncher requires CUDA")
+        device_count = torch.cuda.device_count()
+
         func = functools.partial(process_main, raw_config=self.raw_config)
 
         cfg = MultiprocessConfig(
             rank=-1,
             world_size=device_count,
             devices_per_rank=1,
             master_addr="localhost",
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.25/ml/trainers/mixins/cpu_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from multiprocessing.managers import SyncManager, ValueProxy
 from multiprocessing.synchronize import Event
 from typing import TypeVar
 
 import psutil
 from torch.optim.optimizer import Optimizer
 
-from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.mixins.monitor_process import MonitorProcessConfig, MonitorProcessMixin
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -224,21 +223,20 @@
         super().on_training_end(state, task, model, optim, lr_sched)
 
         self._cpu_stats_monitor.stop()
 
     def on_step_start(
         self,
         state: State,
-        train_batch: Batch,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
-        super().on_step_start(state, train_batch, task, model, optim, lr_sched)
+        super().on_step_start(state, task, model, optim, lr_sched)
 
         monitor = self._cpu_stats_monitor
         stats = monitor.get_if_set() if self.config.cpu_stats_only_log_once else monitor.get()
 
         if stats is not None:
             self.logger.log_scalar("cpu/child_procs", stats.num_child_procs, namespace="trainer")
             self.logger.log_scalar("cpu/percent", stats.cpu_percent, namespace="trainer")
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.25/ml/trainers/mixins/gpu_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from dataclasses import dataclass
 from multiprocessing.managers import SyncManager, ValueProxy
 from multiprocessing.synchronize import Event
 from typing import Iterable, Pattern, TypeVar
 
 from torch.optim.optimizer import Optimizer
 
-from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.mixins.monitor_process import MonitorProcessConfig, MonitorProcessMixin
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -242,21 +241,20 @@
 
         if self._gpu_stats_monitor is not None:
             self._gpu_stats_monitor.stop()
 
     def on_step_start(
         self,
         state: State,
-        train_batch: Batch,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
-        super().on_step_start(state, train_batch, task, model, optim, lr_sched)
+        super().on_step_start(state, task, model, optim, lr_sched)
 
         if (monitor := self._gpu_stats_monitor) is None:
             return
 
         stats = monitor.get_if_set() if self.config.gpu_stats_only_log_once else monitor.get()
 
         for gpu_stat in stats.values():
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.25/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.25/ml/trainers/mixins/heartbeat.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from multiprocessing.managers import SyncManager
 from multiprocessing.synchronize import Event
 from typing import Callable, TypeVar
 
 import psutil
 from torch.optim.optimizer import Optimizer
 
-from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.state import State
 from ml.lr_schedulers.base import SchedulerAdapter
 from ml.trainers.base import ModelT, TaskT
 from ml.trainers.mixins.monitor_process import MonitorProcessConfig, MonitorProcessMixin
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -135,16 +134,15 @@
         super().on_training_end(state, task, model, optim, lr_sched)
 
         self._heartbeat_monitor.stop()
 
     def on_step_start(
         self,
         state: State,
-        train_batch: Batch,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> None:
-        super().on_step_start(state, train_batch, task, model, optim, lr_sched)
+        super().on_step_start(state, task, model, optim, lr_sched)
 
         self._heartbeat_monitor.beat()
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.25/ml/trainers/mixins/mixed_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.grad_scaler: torch.cuda.amp.GradScaler | None
         if self._device_type == "cuda" and self.config.fp16.enabled:
             self.grad_scaler = torch.cuda.amp.GradScaler(
                 init_scale=self.config.fp16.init_scale,
                 growth_factor=self.config.fp16.growth_factor,
                 backoff_factor=self.config.fp16.backoff_factor,
                 growth_interval=self.config.fp16.growth_interval,
-                enabled=self.config.fp16.enabled,
+                enabled=self.config.fp16.enabled and self._device.supports_grad_scaler(),
             )
         else:
             self.grad_scaler = None
 
     def scale_mixed_precision(self, tensor: Tensor) -> Tensor:
         if self.grad_scaler is not None:
             return self.grad_scaler.scale(tensor)
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.25/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.25/ml/trainers/mixins/profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             if self.config.profiler.enabled:
                 with ctx as a, torch.profiler.record_function(step) as b:
                     yield a, b
             else:
                 with ctx as a:
                     yield a
 
-            self.step_times[step] = time.time() - start_time
+            step_time = time.time() - start_time
+            self.step_times[step] = step_time + self.step_times.get(step, 0.0)
 
         return wrapped_ctx()
 
     def write_logs(self, task: TaskT, model: ModelT, state: State) -> None:
         for step, step_time in self.step_times.items():
             self.logger.log_scalar(f"dt/{step}", step_time, namespace="timers")
```

### Comparing `ml-starter-0.0.24/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.25/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/trainers/rl.py` & `ml-starter-0.0.25/ml/trainers/rl.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.rl.base import ReinforcementLearningTask
 from ml.trainers.base import ModelT
-from ml.trainers.ddp import DDPTrainer
-from ml.trainers.slurm import SlurmTrainer, SlurmTrainerConfig
 from ml.trainers.vanilla import TrainingFinishedException, VanillaTrainer, VanillaTrainerConfig
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -49,16 +47,16 @@
 ReinforcementLearningTrainerConfigT = TypeVar(
     "ReinforcementLearningTrainerConfigT",
     bound=ReinforcementLearningTrainerConfig,
 )
 ReinforcementLearningTaskT = TypeVar("ReinforcementLearningTaskT", bound=ReinforcementLearningTask)
 
 
-@register_trainer("vanilla_rl", ReinforcementLearningTrainerConfig)
-class ReinforcementLearningVanillaTrainer(
+@register_trainer("rl", ReinforcementLearningTrainerConfig)
+class ReinforcementLearningTrainer(
     VanillaTrainer[ReinforcementLearningTrainerConfigT, ModelT, ReinforcementLearningTaskT],
     Generic[ReinforcementLearningTrainerConfigT, ModelT, ReinforcementLearningTaskT],
 ):
     def train(
         self,
         model: ModelT,
         task: ReinforcementLearningTaskT,
@@ -86,16 +84,14 @@
         optim, lr_sched = self._get_optim_and_lr_sched(model, optimizer, lr_scheduler)
         state = self._get_state(task, model, optim, lr_sched)
 
         def on_exit(signum: int, _: FrameType | None) -> None:
             sig = signal.Signals(signum)
             self.on_exit(sig, state, task, model, optim, lr_sched)
 
-        self.set_signal_handler(on_exit)
-
         def on_finish_training() -> None:
             self.save_checkpoint(state, task, model, optim, lr_sched)
             raise TrainingFinishedException
 
         # Handle user-defined interrupts.
         signal.signal(signal.SIGUSR1, on_exit)
 
@@ -141,34 +137,34 @@
                     for train_batch in train_pf:
                         self._log_prefetcher_stats(train_pf)
 
                         if task.is_training_over(state):
                             on_finish_training()
 
                         with self.step_context("on_step_start"):
-                            self.on_step_start(state, train_batch, task, model, optim, lr_sched)
+                            self.on_step_start(state, task, model, optim, lr_sched)
 
                         loss_dict = self.train_step(
                             task_model=task_model,
-                            batch=train_batch,
+                            batches=iter([train_batch]),
                             state=state,
                             task=task,
                             model=model,
                             optim=optim,
                             lr_sched=lr_sched,
                         )
 
                         if self.should_checkpoint(state):
                             self.save_checkpoint(state, task, model, optim, lr_sched)
 
                         if profile is not None:
                             profile.step()
 
                         with self.step_context("on_step_end"):
-                            self.on_step_end(state, train_batch, loss_dict, task, model, optim, lr_sched)
+                            self.on_step_end(state, loss_dict, task, model, optim, lr_sched)
 
                         if task.epoch_is_over(state):
                             break
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
@@ -183,31 +179,7 @@
             )
 
         except Exception:
             logger.exception("Caught exception during training loop")
 
         finally:
             self.on_training_end(state, task, model, optim, lr_sched)
-
-
-@register_trainer("ddp_rl", ReinforcementLearningTrainerConfig)
-class ReinforcementLearningDDPTrainer(
-    ReinforcementLearningVanillaTrainer[ReinforcementLearningTrainerConfig, ModelT, ReinforcementLearningTaskT],
-    DDPTrainer[ReinforcementLearningTrainerConfig, ModelT, ReinforcementLearningTaskT],
-):
-    pass
-
-
-@dataclass
-class ReinforcementLearningSlurmTrainerConfig(
-    ReinforcementLearningTrainerConfig,
-    SlurmTrainerConfig,
-):
-    pass
-
-
-@register_trainer("slurm_rl", ReinforcementLearningSlurmTrainerConfig)
-class ReinforcementLearningSlurmTrainer(
-    ReinforcementLearningVanillaTrainer[ReinforcementLearningSlurmTrainerConfig, ModelT, ReinforcementLearningTaskT],
-    SlurmTrainer[ReinforcementLearningSlurmTrainerConfig, ModelT, ReinforcementLearningTaskT],
-):
-    pass
```

### Comparing `ml-starter-0.0.24/ml/trainers/sl.py` & `ml-starter-0.0.25/ml/trainers/sl.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,48 +6,52 @@
 """
 
 import contextlib
 import logging
 import signal
 from dataclasses import dataclass
 from types import FrameType
-from typing import Generic, TypeVar
+from typing import Generic, Iterator, TypeVar
 
+from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.sl.base import SupervisedLearningTask
 from ml.trainers.base import ModelT
-from ml.trainers.ddp import DDPTrainer
-from ml.trainers.slurm import SlurmTrainer, SlurmTrainerConfig
 from ml.trainers.vanilla import TrainingFinishedException, VanillaTrainer, VanillaTrainerConfig
 from ml.utils.device.base import InfinitePrefetcher
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+class EpochDoneException(Exception):
+    """Raised when an epoch is done."""
+
+
 @dataclass
 class ValidationConfig:
     valid_every_n_steps: int | None = conf_field(100, help="Number of training steps to run per test step")
     num_init_valid_steps: int | None = conf_field(2, help="Number of initial validation steps")
 
 
 @dataclass
 class SupervisedLearningTrainerConfig(VanillaTrainerConfig):
     validation: ValidationConfig = conf_field(ValidationConfig())
+    batches_per_step: int = conf_field(1, help="Batches per training step, to simulate larger effective batch sizes")
 
 
 SupervisedLearningTrainerConfigT = TypeVar("SupervisedLearningTrainerConfigT", bound=SupervisedLearningTrainerConfig)
 SupervisedLearningTaskT = TypeVar("SupervisedLearningTaskT", bound=SupervisedLearningTask)
 
 
-@register_trainer("vanilla_sl", SupervisedLearningTrainerConfig)
-class SupervisedLearningVanillaTrainer(
+@register_trainer("sl", SupervisedLearningTrainerConfig)
+class SupervisedLearningTrainer(
     VanillaTrainer[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
     Generic[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
 ):
     def train(
         self,
         model: ModelT,
         task: SupervisedLearningTaskT,
@@ -79,16 +83,14 @@
         optim, lr_sched = self._get_optim_and_lr_sched(model, optimizer, lr_scheduler)
         state = self._get_state(task, model, optim, lr_sched)
 
         def on_exit(signum: int, _: FrameType | None) -> None:
             sig = signal.Signals(signum)
             self.on_exit(sig, state, task, model, optim, lr_sched)
 
-        self.set_signal_handler(on_exit)
-
         def on_finish_training() -> None:
             self.save_checkpoint(state, task, model, optim, lr_sched)
             raise TrainingFinishedException
 
         # Handle user-defined interrupts.
         signal.signal(signal.SIGUSR1, on_exit)
 
@@ -130,32 +132,51 @@
                 while True:
                     with self.step_context("on_epoch_start"):
                         self.on_epoch_start(state, task, model, optim, lr_sched)
 
                     state.num_epoch_steps = 0
                     state.num_epoch_samples = 0
 
-                    for train_batch in train_pf:
+                    train_pf_iter = iter(train_pf)
+
+                    while True:
                         self._log_prefetcher_stats(train_pf)
 
                         if task.is_training_over(state):
                             on_finish_training()
 
                         with self.step_context("on_step_start"):
-                            self.on_step_start(state, train_batch, task, model, optim, lr_sched)
+                            self.on_step_start(state, task, model, optim, lr_sched)
+
+                        try:
+
+                            def batch_iterator() -> Iterator[Batch]:
+                                try:
+                                    yield next(train_pf_iter)
+                                except StopIteration:
+                                    raise EpochDoneException
+
+                                for _ in range(self.config.batches_per_step - 1):
+                                    try:
+                                        yield next(train_pf_iter)
+                                    except StopIteration:
+                                        pass
+
+                            loss_dict = self.train_step(
+                                task_model=task_model,
+                                batches=batch_iterator(),
+                                state=state,
+                                task=task,
+                                model=model,
+                                optim=optim,
+                                lr_sched=lr_sched,
+                            )
 
-                        loss_dict = self.train_step(
-                            task_model=task_model,
-                            batch=train_batch,
-                            state=state,
-                            task=task,
-                            model=model,
-                            optim=optim,
-                            lr_sched=lr_sched,
-                        )
+                        except EpochDoneException:
+                            break
 
                         valid_every_n_steps = self.config.validation.valid_every_n_steps
                         if valid_every_n_steps is not None and state.num_steps % valid_every_n_steps == 0:
                             self._log_prefetcher_stats(valid_pf)
 
                             self.val_step(
                                 task_model=task_model,
@@ -168,15 +189,15 @@
                         if self.should_checkpoint(state):
                             self.save_checkpoint(state, task, model, optim, lr_sched)
 
                         if profile is not None:
                             profile.step()
 
                         with self.step_context("on_step_end"):
-                            self.on_step_end(state, train_batch, loss_dict, task, model, optim, lr_sched)
+                            self.on_step_end(state, loss_dict, task, model, optim, lr_sched)
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
                     state.num_epochs += 1
 
         except TrainingFinishedException:
@@ -188,31 +209,7 @@
             )
 
         except Exception:
             logger.exception("Caught exception during training loop")
 
         finally:
             self.on_training_end(state, task, model, optim, lr_sched)
-
-
-@register_trainer("ddp_sl", SupervisedLearningTrainerConfig)
-class SupervisedLearningDDPTrainer(
-    SupervisedLearningVanillaTrainer[SupervisedLearningTrainerConfig, ModelT, SupervisedLearningTaskT],
-    DDPTrainer[SupervisedLearningTrainerConfig, ModelT, SupervisedLearningTaskT],
-):
-    pass
-
-
-@dataclass
-class SupervisedLearningSlurmTrainerConfig(
-    SupervisedLearningTrainerConfig,
-    SlurmTrainerConfig,
-):
-    pass
-
-
-@register_trainer("slurm_sl", SupervisedLearningSlurmTrainerConfig)
-class SupervisedLearningSlurmTrainer(
-    SupervisedLearningVanillaTrainer[SupervisedLearningSlurmTrainerConfig, ModelT, SupervisedLearningTaskT],
-    SlurmTrainer[SupervisedLearningSlurmTrainerConfig, ModelT, SupervisedLearningTaskT],
-):
-    pass
```

### Comparing `ml-starter-0.0.24/ml/trainers/slurm.py` & `ml-starter-0.0.25/ml/launchers/slurm.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,37 +16,29 @@
 
 import logging
 import os
 import re
 import signal
 import subprocess
 import sys
-from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
 from types import FrameType
-from typing import Callable, Generic, TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
-from torch import nn
-from torch.optim import Optimizer
 
 from ml.core.config import conf_field
 from ml.core.env import get_stage_dir
-from ml.core.registry import Objects, project_dirs
-from ml.core.state import State
-from ml.lr_schedulers.base import SchedulerAdapter
+from ml.core.registry import Objects, project_dirs, register_launcher
+from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.scripts.train import train_main
-from ml.trainers.base import ModelT, TaskT
-from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
-    get_world_size,
     is_master,
     set_init_method,
     set_master_addr,
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
@@ -120,71 +112,44 @@
     assert node_list is not None, "`SLURM_JOB_NODELIST` environment variable not set"
     hostnames = subprocess.check_output(["scontrol", "show", "hostnames", node_list])
     host = hostnames.split()[0].decode("utf-8")
     set_master_addr(host)
     return host
 
 
+def requeue_job() -> None:
+    if is_master():
+        if "SLURM_JOB_ID" in os.environ:
+            cmd = ["scontrol", "requeue", os.environ["SLURM_JOB_ID"]]
+            logger.info("Running %s", " ".join(cmd))
+            subprocess.check_call(cmd)
+        else:
+            logger.info("SLURM_JOB_ID environment variable not found; not requeueing")
+
+
 @dataclass
-class SlurmTrainerConfig(VanillaTrainerConfig):
+class SlurmLauncherConfig(BaseLauncherConfig):
     partition: str = conf_field(II("oc.env:SLURM_PARTITION,none"), help="Which partition to launch")
     time_limit: str = conf_field(II("oc.env:SLURM_TIME_LIMIT,3-00:00:00"), help="Time limit string")
     num_nodes: int = conf_field(MISSING, help="Total number of nodes to use")
     gpus_per_node: int = conf_field(II("oc.env:SLURM_GPUS_PER_NODE,8"), help="Number of GPUs per node")
     cpus_per_gpu: int = conf_field(II("oc.env:SLURM_CPUS_PER_GPU,1"), help="Number of CPUs per task")
     gpu_type: str | None = conf_field(None, help="Specific GPU type to pass to gres")
     num_jobs: int = conf_field(1, help="Number of redundant jobs to launch")
     comment: str | None = conf_field(None, help="An optional comment to add to the experiment")
     master_port: int = conf_field(get_random_port, help="The master port to use")
 
 
-SlurmTrainerConfigT = TypeVar("SlurmTrainerConfigT", bound=SlurmTrainerConfig)
-
-
 def ignore_signal(signum: int, _: FrameType | None) -> None:
     sig = signal.Signals(signum)
     logger.info("Ignoring signal %s", sig.name)
 
 
-class SlurmTrainer(
-    VanillaTrainer[SlurmTrainerConfigT, ModelT, TaskT],
-    Generic[SlurmTrainerConfigT, ModelT, TaskT],
-    ABC,
-):
-    def get_task_model(self, task: TaskT, model: ModelT) -> nn.Module:
-        task_model = super().get_task_model(task, model)
-        if get_world_size() > 1:
-            task_model = nn.parallel.DistributedDataParallel(task_model)
-        return task_model
-
-    def on_exit(
-        self,
-        sig: signal.Signals,
-        state: State,
-        task: TaskT,
-        model: ModelT,
-        optim: Optimizer,
-        lr_scheduler: SchedulerAdapter,
-    ) -> None:
-        super().on_exit(sig, state, task, model, optim, lr_scheduler)
-
-        if is_master():
-            if "SLURM_JOB_ID" in os.environ:
-                cmd = ["scontrol", "requeue", os.environ["SLURM_JOB_ID"]]
-                logger.info("Running %s", " ".join(cmd))
-                subprocess.check_call(cmd)
-            else:
-                logger.info("SLURM_JOB_ID environment variable not found; not requeueing")
-
-    def set_signal_handler(self, handler: Callable[[int, FrameType | None], None]) -> None:
-        super().set_signal_handler(handler)
-
-        signal.signal(signal.SIGUSR1, handler)
-        signal.signal(signal.SIGTERM, ignore_signal)
-
+@register_launcher("slurm", SlurmLauncherConfig)
+class SlurmLauncher(BaseLauncher[SlurmLauncherConfig]):
     def launch(self) -> None:
         # Gets some configuration options.
         gpus_per_node = self.config.gpus_per_node
         gpu_type = self.config.gpu_type
         tasks_per_node = gpus_per_node
         cpus_per_task = self.config.cpus_per_gpu
 
@@ -287,15 +252,20 @@
 
     # Sets the initialization method and configures per-rank logging.
     set_init_method(f"tcp://{get_master_addr()}:{get_master_port()}")
     configure_logging(rank=rank, world_size=world_size)
     init_process_group(backend=get_distributed_backend())
 
     objs = Objects.parse_raw_config(raw_config)  # type: ignore
+
     assert (trainer := objs.trainer) is not None
     trainer.add_lock_file("running", exists_ok=True)
     trainer.remove_lock_file("scheduled", missing_ok=True)
+
+    signal.signal(signal.SIGTERM, ignore_signal)
+    trainer.add_signal_handler(signal.SIGUSR1, requeue_job)
+
     train_main(objs)
 
 
 if __name__ == "__main__":
     slurm_main()
```

### Comparing `ml-starter-0.0.24/ml/trainers/vanilla.py` & `ml-starter-0.0.25/ml/trainers/vanilla.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Defines a vanilla trainer which doesn't do any device or data manipulation.
 
 This trainer expects the task to handle all the relevant movement of data and
 models to their associated devices.
 """
 
 import logging
-import signal
 from dataclasses import dataclass
-from types import FrameType
-from typing import Callable, Generic, TypeVar, cast
+from typing import Callable, Generic, Iterator, TypeVar, cast
 
 import torch
 from omegaconf import II
 from torch import Tensor, nn
 from torch.optim import Optimizer
 
 from ml.core.common_types import Batch, Loss
@@ -28,15 +26,15 @@
     GradientClippingTrainerMixin,
 )
 from ml.trainers.mixins.mixed_precision import (
     MixedPrecisionTrainerConfig,
     MixedPrecisionTrainerMixin,
 )
 from ml.trainers.mixins.profiler import ProfilerTrainerConfig, ProfilerTrainerMixin
-from ml.utils.device.base import Prefetcher
+from ml.utils.distributed import get_world_size
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TrainingFinishedException(Exception):
     pass
@@ -75,15 +73,14 @@
     GPUStatsConfig,
     CPUStatsConfig,
     BaseTrainerConfig,
 ):
     set_to_none: bool = conf_field(True, help="Mode for clearing optimizer gradients")
     deterministic: bool = conf_field(False, help="If set, use determinstic algorithms")
     use_tf32: bool = conf_field(True, help="If set, use TensorFloat32")
-    update_interval: int = conf_field(1, help="How often to update model parameters")
     torch_compile: TorchCompileConfig = conf_field(TorchCompileConfig(), help="Torch compile config")
     detect_anomaly: bool = conf_field(False, help="Whether to detect anomalies")
     detect_anomaly_check_nan: bool = conf_field(False, help="Whether to check for NaNs when detecting anomalies")
 
 
 VanillaTrainerConfigT = TypeVar("VanillaTrainerConfigT", bound=VanillaTrainerConfig)
 
@@ -93,66 +90,71 @@
     GradientClippingTrainerMixin[VanillaTrainerConfigT, ModelT, TaskT],
     MixedPrecisionTrainerMixin[VanillaTrainerConfigT, ModelT, TaskT],
     GPUStatsMixin[VanillaTrainerConfigT, ModelT, TaskT],
     CPUStatsMixin[VanillaTrainerConfigT, ModelT, TaskT],
     BaseTrainer[VanillaTrainerConfigT, ModelT, TaskT],
     Generic[VanillaTrainerConfigT, ModelT, TaskT],
 ):
-    def get_task_model_impl(self, task: TaskT, model: ModelT) -> nn.Module:
+    def get_task_model(self, task: TaskT, model: ModelT) -> nn.Module:
         device, dtype = self._device.get_device(), self._weight_precision
         model.init(device, dtype)
         task.to(device, dtype)
         task_model: nn.Module = TaskModel(task=task, model=model)
+        if get_world_size() > 1:
+            task_model = nn.parallel.DistributedDataParallel(task_model)
         return task_model
 
-    def get_task_model(self, task: TaskT, model: ModelT) -> nn.Module:
-        return self.get_task_model_impl(task, model)
-
     def train_step(
         self,
         *,
         task_model: nn.Module,
-        batch: Batch,
+        batches: Iterator[Batch],
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> dict[str, Tensor]:
         with self.step_context("change_mode"):
             task_model, state.phase = set_phase(task_model, "train")
-        with self.step_context("forward"), self.autocast_context():
-            loss = task_model(batch, state)
-        with self.step_context("get_single_loss"):
-            single_loss, loss_names = task.get_single_loss(loss)
-        with self.step_context("backward"):
-            self.scale_mixed_precision(single_loss.sum()).backward()
-        with self.step_context("log_losses"):
-            self.log_mp_scale()
-            single_loss_detached = single_loss.detach()
-            loss_dict = {name: single_loss_detached[i] for i, name in enumerate(loss_names)}
-            task.log_loss_dict(loss_dict, state)
-        if state.num_steps % self.config.update_interval == 0:
-            with self.step_context("clip_grads"):
-                self.clip_grads(model=task_model, optim=optim)
-            with self.step_context("step"):
-                self.step_optimizer(optim=optim)
-                lr_sched.step(state)
-                self.logger.log_scalar("lr_scale", lr_sched.lr_scale, namespace="optim")
-            with self.step_context("zero_grads"):
-                optim.zero_grad(set_to_none=self.config.set_to_none)
+        total_bsz: int | None = None
+        first_batch = True
+        for batch in batches:
+            bsz = task.get_batch_size(batch)
+            if bsz is not None:
+                total_bsz = bsz if total_bsz is None else total_bsz + bsz
+            with self.step_context("forward"), self.autocast_context():
+                loss = task_model(batch, state)
+            with self.step_context("get_single_loss"):
+                single_loss, loss_names = task.get_single_loss(loss)
+            with self.step_context("backward"):
+                self.scale_mixed_precision(single_loss.sum()).backward()
+            if first_batch:
+                with self.step_context("log_losses"):
+                    self.log_mp_scale()
+                    single_loss_detached = single_loss.detach()
+                    loss_dict = {name: single_loss_detached[i] for i, name in enumerate(loss_names)}
+                    task.log_loss_dict(loss_dict, state)
+                first_batch = False
+        with self.step_context("clip_grads"):
+            self.clip_grads(model=task_model, optim=optim)
+        with self.step_context("step"):
+            self.step_optimizer(optim=optim)
+            lr_sched.step(state)
+            self.logger.log_scalar("lr_scale", lr_sched.lr_scale, namespace="optim")
+        with self.step_context("zero_grads"):
+            optim.zero_grad(set_to_none=self.config.set_to_none)
         with self.step_context("write_logs"), self.autocast_context():
             self.write_logs(task, model, state)
         with self.step_context("update_state"):
             state.num_steps += 1
             state.num_epoch_steps += 1
-            bsz = task.get_batch_size(batch)
-            if bsz is not None:
-                state.num_samples += bsz
-                state.num_epoch_samples += bsz
+            if total_bsz is not None:
+                state.num_samples += total_bsz
+                state.num_epoch_samples += total_bsz
         return loss_dict
 
     def val_step(
         self,
         *,
         task_model: nn.Module,
         batch: Batch,
@@ -197,29 +199,14 @@
                 loss_dict = {name: single_loss_detached[i] for i, name in enumerate(loss_names)}
                 task.log_loss_dict(loss_dict, state)
             with self.step_context("write_logs"):
                 self.write_logs(task, model, state)
             with self.step_context("update_state"):
                 state.num_test_steps += 1
 
-    def on_exit(
-        self,
-        sig: signal.Signals,
-        state: State,
-        task: TaskT,
-        model: ModelT,
-        optim: Optimizer,
-        lr_scheduler: SchedulerAdapter,
-    ) -> None:
-        logger.info("Handling interrupt %s", sig.name)
-        self.save_checkpoint(state, task, model, optim, lr_scheduler)
-
-    def set_signal_handler(self, handler: Callable[[int, FrameType | None], None]) -> None:
-        pass
-
     def _init_environment(self) -> None:
         # Sets up environment.
         if self.config.deterministic:
             torch.use_deterministic_algorithms(True)
         if self.config.use_tf32 and torch.cuda.is_available():
             torch.backends.cuda.matmul.allow_tf32 = True
 
@@ -271,14 +258,7 @@
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> State:
         if (ckpt_path := self.get_ckpt_path()).exists():
             return self.load_checkpoint(ckpt_path, task, model, optim, lr_sched)
         return State.init_state()
-
-    def _log_prefetcher_stats(self, pf: Prefetcher) -> None:
-        self.logger.log_scalar("dt/get_batch", pf.get_batch_time, namespace="timers")
-        self.logger.log_scalar("dt/to_device", pf.to_device_time, namespace="timers")
-
-    def launch(self) -> None:
-        raise NotImplementedError(f"{self.__class__.__name__} doesn't support multiprocess training")
```

### Comparing `ml-starter-0.0.24/ml/utils/argparse.py` & `ml-starter-0.0.25/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/atomic.py` & `ml-starter-0.0.25/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/augmentation.py` & `ml-starter-0.0.25/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/caching.py` & `ml-starter-0.0.25/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/call_train.py` & `ml-starter-0.0.25/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/cli.py` & `ml-starter-0.0.25/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/colors.py` & `ml-starter-0.0.25/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/compiler.py` & `ml-starter-0.0.25/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/data.py` & `ml-starter-0.0.25/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/datetime.py` & `ml-starter-0.0.25/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/device/auto.py` & `ml-starter-0.0.25/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/device/base.py` & `ml-starter-0.0.25/ml/utils/device/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,7 +239,11 @@
     def autocast_context(cls, enabled: bool = True) -> ContextManager:
         device_type = cls.get_device().type
         if device_type == "mps":
             device_type = "cpu"
         if device_type not in ("cpu", "cuda"):
             return contextlib.nullcontext()
         return torch.autocast(device_type, enabled=enabled)
+
+    @classmethod
+    def supports_grad_scaler(cls) -> bool:
+        return False
```

### Comparing `ml-starter-0.0.24/ml/utils/device/cpu.py` & `ml-starter-0.0.25/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/device/gpu.py` & `ml-starter-0.0.25/ml/utils/device/gpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,32 @@
 
     @classmethod
     def get_device(cls) -> torch.device:
         return torch.device("cuda", 0)
 
     @classmethod
     def get_floating_point_type(cls) -> torch.dtype:
+        use_bf16 = get_env_bool("USE_BF16")
         use_fp32 = get_env_bool("USE_FP32")
         use_fp64 = get_env_bool("USE_FP64")
         if use_fp64:
             logger.info("Using FP64")
             return torch.float64
         elif use_fp32:
             logger.info("Using FP32")
             return torch.float32
+        elif use_bf16:
+            logger.info("Using BF16")
+            return torch.bfloat16
         else:
             return torch.float16
-            # return torch.bfloat16
 
     @classmethod
     def get_torch_compile_backend(cls) -> str | Callable:
         capability = torch.cuda.get_device_capability()
         if capability >= (7, 0):
             return "inductor"
         return "aot_ts_nvfuser"
+
+    @classmethod
+    def supports_grad_scaler(cls) -> bool:
+        return cls.get_floating_point_type() == torch.float16
```

### Comparing `ml-starter-0.0.24/ml/utils/device/metal.py` & `ml-starter-0.0.25/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/distributed.py` & `ml-starter-0.0.25/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/image.py` & `ml-starter-0.0.25/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/io.py` & `ml-starter-0.0.25/ml/utils/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 from omegaconf import DictConfig, OmegaConf
 
 from ml.core.registry import Objects, register_model, register_task
 from ml.models.base import BaseModel
 from ml.tasks.base import BaseTask
-from ml.trainers.base import DummyBaseTrainer
+from ml.trainers.base import BaseTrainer
 from ml.utils.device.auto import AutoDevice
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
@@ -32,19 +32,15 @@
         config = cast(DictConfig, OmegaConf.load(config))
     elif isinstance(config, dict):
         config = OmegaConf.create(config)
     Objects.resolve_config(config)
     return Objects.parse_raw_config(config)
 
 
-def get_checkpoint_path(
-    trainer: DummyBaseTrainer,
-    config_path: str | Path,
-    ckpt_path: str | Path | None,
-) -> Path:
+def get_checkpoint_path(trainer: BaseTrainer, config_path: str | Path, ckpt_path: str | Path | None) -> Path:
     if ckpt_path is not None:
         ckpt_path = Path(ckpt_path)
         if ckpt_path.exists():
             return ckpt_path
         logger.warning("Could not find the passed checkpoint at %s", ckpt_path)
 
     # Tries loading the checkpoint that the trainer thinks exists.
@@ -100,27 +96,29 @@
         RuntimeError: If the checkpoint is missing and `missing_ckpt_okay` is
             False.
     """
 
     with Timer("loading checkpoint"):
         ckpt: str | Path | dict | None = None
 
+        trainer: BaseTrainer
+
         if config_path is None:
             if ckpt_path is None:
                 raise ValueError("Must provide either a config path or a checkpoint path")
 
             ckpt = cast(dict, torch.load(ckpt_path, map_location="cpu"))
             if "config" not in ckpt:
                 raise ValueError("Could not find a config in the checkpoint")
             config = OmegaConf.create(ckpt["config"])
-            trainer = DummyBaseTrainer(config.trainer)
+            trainer = BaseTrainer(config.trainer)
 
         else:
             config = cast(DictConfig, OmegaConf.load(config_path))
-            trainer = DummyBaseTrainer(config.trainer)
+            trainer = BaseTrainer(config.trainer)
 
             # Uses the dummy trainer to load the checkpoint.
             try:
                 ckpt = get_checkpoint_path(trainer, config_path, ckpt_path)
             except RuntimeError:
                 if missing_ckpt_okay:
                     logger.exception("Could not load checkpoint")
```

### Comparing `ml-starter-0.0.24/ml/utils/large_models.py` & `ml-starter-0.0.25/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/logging.py` & `ml-starter-0.0.25/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/meter.py` & `ml-starter-0.0.25/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/staging.py` & `ml-starter-0.0.25/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/timer.py` & `ml-starter-0.0.25/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/torch_distributed.py` & `ml-starter-0.0.25/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml/utils/video.py` & `ml-starter-0.0.25/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.25/ml_starter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 ml/py.typed
 ml/core/__init__.py
 ml/core/common_types.py
 ml/core/config.py
 ml/core/env.py
 ml/core/registry.py
 ml/core/state.py
+ml/launchers/__init__.py
+ml/launchers/base.py
+ml/launchers/ddp.py
+ml/launchers/slurm.py
 ml/loggers/__init__.py
 ml/loggers/base.py
 ml/loggers/meter.py
 ml/loggers/multi.py
 ml/loggers/stdout.py
 ml/loggers/tensorboard.py
 ml/lr_schedulers/__init__.py
@@ -44,15 +48,15 @@
 ml/optimizers/base.py
 ml/optimizers/sgd.py
 ml/optimizers/shampoo.py
 ml/optimizers/types.py
 ml/scripts/__init__.py
 ml/scripts/cli.py
 ml/scripts/compiler.py
-ml/scripts/mp_train.py
+ml/scripts/launch.py
 ml/scripts/resolve.py
 ml/scripts/stage.py
 ml/scripts/train.py
 ml/tasks/__init__.py
 ml/tasks/base.py
 ml/tasks/datasets/__init__.py
 ml/tasks/datasets/async_iterable.py
@@ -74,18 +78,16 @@
 ml/tasks/rl/__init__.py
 ml/tasks/rl/base.py
 ml/tasks/rl/replay.py
 ml/tasks/sl/__init__.py
 ml/tasks/sl/base.py
 ml/trainers/__init__.py
 ml/trainers/base.py
-ml/trainers/ddp.py
 ml/trainers/rl.py
 ml/trainers/sl.py
-ml/trainers/slurm.py
 ml/trainers/vanilla.py
 ml/trainers/mixins/__init__.py
 ml/trainers/mixins/cpu_stats.py
 ml/trainers/mixins/gpu_stats.py
 ml/trainers/mixins/grad_clipping.py
 ml/trainers/mixins/heartbeat.py
 ml/trainers/mixins/mixed_precision.py
```

### Comparing `ml-starter-0.0.24/pyproject.toml` & `ml-starter-0.0.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.24/setup.py` & `ml-starter-0.0.25/setup.py`

 * *Files identical despite different names*

