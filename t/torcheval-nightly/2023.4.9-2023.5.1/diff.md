# Comparing `tmp/torcheval-nightly-2023.4.9.tar.gz` & `tmp/torcheval-nightly-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torcheval-nightly-2023.4.9.tar", last modified: Sun Apr  9 11:55:37 2023, max compression
+gzip compressed data, was "dist/torcheval-nightly-2023.5.1.tar", last modified: Mon May  1 12:03:17 2023, max compression
```

## Comparing `torcheval-nightly-2023.4.9.tar` & `torcheval-nightly-2023.5.1.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/min.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18405 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/image/psnr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/num_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_information_preserved.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/image/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/text/word_information_preserved.py
--rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/auroc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/metrics/window/weighted_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/tools/flops.py
--rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/tools/module_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/utils/random_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval/utils/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/utils/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/utils/test_utils/dummy_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/utils/test_utils/metric_class_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 11:52:31.000000 torcheval-nightly-2023.4.9/torcheval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:55:37.000000 torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18405 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/image/psnr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/num_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_information_preserved.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/text/word_information_preserved.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/metrics/window/weighted_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/tools/flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/tools/module_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/utils/random_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval/utils/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/utils/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/utils/test_utils/dummy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/utils/test_utils/metric_class_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-01 12:00:22.000000 torcheval-nightly-2023.5.1/torcheval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:03:17.000000 torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/zip-safe
```

### Comparing `torcheval-nightly-2023.4.9/LICENSE` & `torcheval-nightly-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/PKG-INFO` & `torcheval-nightly-2023.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2023.4.9
+Version: 2023.5.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: image
 License-File: LICENSE
 
 # TorchEval
 
 <p align="center">
 <a href="https://github.com/pytorch/torcheval/actions?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/pytorch/torcheval/.github/workflows/unit_test.yaml?branch=main" alt="build status"></a>
 <a href="https://pypi.org/project/torcheval"><img src="https://img.shields.io/pypi/v/torcheval" alt="pypi version"></a>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2023.4.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2023.5.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE # TorchEval
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+image License-File: LICENSE # TorchEval
       [build_status] [pypi_version] [pypi_nightly_version] [bsd_license]
 [docs]
 **This library is currently in Alpha and currently does not have a stable
 release. The API may change and may not be backward compatible. If you have
 suggestions for improvements, please open a GitHub issue. We'd love to hear
 your feedback.** A library that contains a rich collection of performant
 PyTorch model metrics, a simple interface to create new metrics, a toolkit to
```

### Comparing `torcheval-nightly-2023.4.9/README.md` & `torcheval-nightly-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/setup.py` & `torcheval-nightly-2023.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,9 +73,12 @@
             "Intended Audience :: Developers",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: BSD License",
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.7",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
         ],
-        extras_require={"dev": read_requirements("dev-requirements.txt")},
+        extras_require={
+            "dev": read_requirements("dev-requirements.txt"),
+            "image": read_requirements("image-requirements.txt"),
+        },
     )
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     MulticlassRecall,
     MultilabelAccuracy,
     MultilabelAUPRC,
     MultilabelPrecisionRecallCurve,
     MultilabelRecallAtFixedPrecision,
     TopKMultilabelAccuracy,
 )
-from torcheval.metrics.image.psnr import PeakSignalNoiseRatio
+
+from torcheval.metrics.image import FrechetInceptionDistance, PeakSignalNoiseRatio
 from torcheval.metrics.metric import Metric
 
 from torcheval.metrics.ranking import (
     ClickThroughRate,
     HitRate,
     ReciprocalRank,
     WeightedCalibration,
@@ -68,26 +69,28 @@
     # functional metrics
     "functional",
     # class metrics
     "AUC",
     "BinaryAccuracy",
     "BinaryAUPRC",
     "BinaryAUROC",
+    "BinaryBinnedAUPRC",
     "BinaryBinnedAUROC",
     "BinaryBinnedPrecisionRecallCurve",
     "BinaryConfusionMatrix",
     "BinaryF1Score",
     "BinaryNormalizedEntropy",
     "BinaryPrecision",
     "BinaryPrecisionRecallCurve",
     "BinaryRecall",
     "BinaryRecallAtFixedPrecision",
     "BLEUScore",
     "Cat",
     "ClickThroughRate",
+    "FrechetInceptionDistance",
     "HitRate",
     "Max",
     "Mean",
     "MeanSquaredError",
     "Min",
     "MulticlassAccuracy",
     "MulticlassAUPRC",
@@ -99,20 +102,20 @@
     "MulticlassPrecision",
     "MulticlassPrecisionRecallCurve",
     "MulticlassRecall",
     "MultilabelAccuracy",
     "MultilabelAUPRC",
     "MultilabelPrecisionRecallCurve",
     "MultilabelRecallAtFixedPrecision",
+    "PeakSignalNoiseRatio",
     "Perplexity",
     "TopKMultilabelAccuracy",
     "R2Score",
     "ReciprocalRank",
     "Sum",
-    "PeakSignalNoiseRatio",
     "Throughput",
     "WeightedCalibration",
     "WindowedBinaryAUROC",
     "WindowedBinaryNormalizedEntropy",
     "WindowedClickThroughRate",
     "WindowedMeanSquaredError",
     "WindowedWeightedCalibration",
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/auc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/cat.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/cat.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/max.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/max.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/mean.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/min.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/min.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/sum.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/aggregation/throughput.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/accuracy.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/auprc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/auroc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/binary_normalized_entropy.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_auprc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_auroc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_auroc.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Compute AUROC, which is the area under the ROC Curve, for binary classification.
     Its functional version is :func:`torcheval.metrics.functional.binary_binned_auroc`.
 
     Args:
         num_tasks (int):  Number of tasks that need binary_binned_auroc calculation. Default value
                     is 1. binary_binned_auroc for each task will be calculated independently.
-        threshold: A integeter representing number of bins, a list of thresholds, or a tensor of thresholds.
+        threshold: A integer representing number of bins, a list of thresholds, or a tensor of thresholds.
     See also :class:`MulticlassBinnedAUROC <MulticlassBinnedAUROC>`
 
 
     Examples::
 
         >>> import torch
         >>> from torcheval.metrics import BinaryBinnedAUROC
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/confusion_matrix.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/f1_score.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/precision.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/precision_recall_curve.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/recall.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,27 @@
     multiclass_confusion_matrix,
     multiclass_f1_score,
     multiclass_precision,
     multiclass_precision_recall_curve,
     multiclass_recall,
     multilabel_accuracy,
     multilabel_auprc,
+    multilabel_binned_precision_recall_curve,
     multilabel_precision_recall_curve,
     multilabel_recall_at_fixed_precision,
     topk_multilabel_accuracy,
 )
 from torcheval.metrics.functional.image import peak_signal_noise_ratio
 from torcheval.metrics.functional.ranking import (
     click_through_rate,
     frequency_at_k,
     hit_rate,
     num_collisions,
     reciprocal_rank,
+    retrieval_precision,
     weighted_calibration,
 )
 from torcheval.metrics.functional.regression import mean_squared_error, r2_score
 from torcheval.metrics.functional.text import (
     bleu_score,
     perplexity,
     word_error_rate,
@@ -80,21 +82,23 @@
     "multiclass_confusion_matrix",
     "multiclass_f1_score",
     "multiclass_precision",
     "multiclass_precision_recall_curve",
     "multiclass_recall",
     "multilabel_accuracy",
     "multilabel_auprc",
+    "multilabel_binned_precision_recall_curve",
     "multilabel_precision_recall_curve",
     "multilabel_recall_at_fixed_precision",
     "num_collisions",
     "peak_signal_noise_ratio",
     "perplexity",
     "r2_score",
     "reciprocal_rank",
+    "retrieval_precision",
     "sum",
     "throughput",
     "topk_multilabel_accuracy",
     "weighted_calibration",
     "word_error_rate",
     "word_information_preserved",
     "word_information_lost",
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/auc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/mean.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/sum.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/aggregation/throughput.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from torcheval.metrics.functional.classification.binned_auroc import (
     binary_binned_auroc,
     multiclass_binned_auroc,
 )
 from torcheval.metrics.functional.classification.binned_precision_recall_curve import (
     binary_binned_precision_recall_curve,
     multiclass_binned_precision_recall_curve,
+    multilabel_binned_precision_recall_curve,
 )
 from torcheval.metrics.functional.classification.confusion_matrix import (
     binary_confusion_matrix,
     multiclass_confusion_matrix,
 )
 from torcheval.metrics.functional.classification.f1_score import (
     binary_f1_score,
@@ -78,12 +79,13 @@
     "multiclass_confusion_matrix",
     "multiclass_f1_score",
     "multiclass_precision",
     "multiclass_precision_recall_curve",
     "multiclass_recall",
     "multilabel_accuracy",
     "multilabel_auprc",
+    "multilabel_binned_precision_recall_curve",
     "multilabel_precision_recall_curve",
     "multilabel_recall_at_fixed_precision",
     "topk_multilabel_accuracy",
 ]
 __doc_name__ = "Classification Metrics"
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/accuracy.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/auprc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/auroc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_auprc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/precision_recall_curve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,299 +1,333 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import List, Optional, Tuple, Union
+
+from typing import List, Optional, Tuple
 
 import torch
-from torcheval.metrics.functional.classification.binned_precision_recall_curve import (
-    _binary_binned_precision_recall_curve_compute,
-    _binary_binned_precision_recall_curve_update,
-    _multiclass_binned_precision_recall_curve_compute,
-    _multiclass_binned_precision_recall_curve_update,
-)
-from torcheval.metrics.functional.tensor_utils import (
-    _create_threshold_tensor,
-    _riemann_integral,
-)
+import torch.nn.functional as F
 
-DEFAULT_NUM_THRESHOLD = 100
+"""
+This file contains binary_precision_recall_curve, multiclass_precision_recall_curve and multilabel_precision_recall_curve functions.
+"""
 
 
 @torch.inference_mode()
-def binary_binned_auprc(
+def binary_precision_recall_curve(
     input: torch.Tensor,
     target: torch.Tensor,
-    *,
-    num_tasks: int = 1,
-    threshold: Union[int, List[float], torch.Tensor] = DEFAULT_NUM_THRESHOLD,
-) -> Tuple[torch.Tensor, torch.Tensor]:
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
     """
-    Binned Version of AUPRC, which is the area under the AUPRC Curve, for binary classification.
-    Its class version is ``torcheval.metrics.BinaryBinnedAUPRC``.
+    Returns precision-recall pairs and their corresponding thresholds for
+    binary classification tasks. If a class is missing from the target tensor,
+    its recall values are set to 1.0.
 
-    Computation is done by computing the area under the precision/recall curve; precision and recall
-    are computed for the buckets defined by `threshold`.
+    Its class version is ``torcheval.metrics.BinaryPrecisionRecallCurve``.
+    See also :func:`multiclass_precision_recall_curve <torcheval.metrics.functional.multiclass_precision_recall_curve>`, :func:`multilabel_precision_recall_curve <torcheval.metrics.functional.multilabel_precision_recall_curve>`
 
     Args:
         input (Tensor): Tensor of label predictions
-            It should be predicted label, probabilities or logits with shape of (num_tasks, n_sample) or (n_sample, ).
-
-        target (Tensor): Tensor of ground truth labels with shape of (num_tasks, n_sample) or (n_sample, ).
-
-        num_tasks (int):  Number of tasks that need binary_binned_auprc calculation. Default value
-                    is 1. binary_binned_auprc for each task will be calculated independently.
+            It should be probabilities or logits with shape of (n_sample, ).
+        target (Tensor): Tensor of ground truth labels with shape of (n_samples, ).
 
-        threshold (Tensor, int, List[float]): Either an integer representing the number of bins, a list of thresholds, or a tensor of thresholds.
-                    The same thresholds will be used for all tasks.
-                    If `threshold` is a tensor, it must be 1D.
-                    If list or tensor is given, the first element must be 0 and the last must be 1.
+    Returns:
+        Tuple:
+            - precision (Tensor): Tensor of precision result. Its shape is (n_thresholds + 1, )
+            - recall (Tensor): Tensor of recall result. Its shape is (n_thresholds + 1, )
+            - thresholds (Tensor): Tensor of threshold. Its shape is (n_thresholds, )
 
-    Examples:
+    Examples::
 
         >>> import torch
-        >>> from torcheval.metrics.functional import binary_binned_auprc
-        >>> input = torch.tensor([0.2, 0.3, 0.4, 0.5])
+        >>> from torcheval.metrics.functional import binary_precision_recall_curve
+        >>> input = torch.tensor([0.1, 0.5, 0.7, 0.8])
         >>> target = torch.tensor([0, 0, 1, 1])
-        >>> binary_binned_auprc(input, target, threshold=5)
-        (tensor(1.0),
-        tensor([0.0000, 0.2500, 0.5000, 0.7500, 1.0000]))
-
-        >>> input = torch.tensor([0.2, 0.3, 0.4, 0.5])
-        >>> target = torch.tensor([0, 0, 1, 1])
-        >>> threshold = torch.tensor([0.0000, 0.2500, 0.7500, 1.0000])
-        >>> binary_binned_auprc(input, target, threshold=threshold)
-        (tensor(0.6667),
-        tensor([0.0000, 0.2500, 0.7500, 1.0000]))
-
-        >>> input = torch.tensor([[0.2, 0.3, 0.4, 0.5], [0, 1, 2, 3]])
-        >>> target = torch.tensor([[0, 0, 1, 1], [0, 1, 1, 1]])
-        >>> threshold = torch.tensor([0.0000, 0.2500, 0.7500, 1.0000])
-        >>> binary_binned_auprc(input, target, num_tasks=2, threshold=threshold)
-        (tensor([0.6667, 1.0000],
-        tensor([0.0000, 0.2500, 0.7500, 1.0000]))
+        >>> binary_precision_recall_curve(input, target)
+        (tensor([0.5000, 0.6667, 1.0000, 1.0000, 1.0000]),
+        tensor([1.0000, 1.0000, 1.0000, 0.5000, 0.0000]),
+        tensor([0.1000, 0.5000, 0.7000, 0.8000]))
     """
-    threshold = _create_threshold_tensor(threshold, target.device)
-    _binary_binned_auprc_param_check(num_tasks, threshold)
-    _binary_binned_auprc_update_input_check(input, target, num_tasks, threshold)
-    return _binary_binned_auprc_compute(input, target, num_tasks, threshold)
-
-
-def _binary_binned_auprc_compute(
-    input: torch.Tensor,
-    target: torch.Tensor,
-    num_tasks: int,
-    threshold: torch.Tensor,
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    if num_tasks == 1 and input.ndim == 1:
-        num_tp, num_fp, num_fn = _binary_binned_precision_recall_curve_update(
-            input, target, threshold
-        )
-        precision, recall, _ = _binary_binned_precision_recall_curve_compute(
-            num_tp, num_fp, num_fn, threshold
-        )
-        auprc_result = _riemann_integral(recall, precision)
-    else:
-        auprcs = []
-        for i in range(num_tasks):
-            num_tp, num_fp, num_fn = _binary_binned_precision_recall_curve_update(
-                input[i, :], target[i, :], threshold
-            )
-            precision, recall, _ = _binary_binned_precision_recall_curve_compute(
-                num_tp, num_fp, num_fn, threshold
-            )
-            auprcs.append(_riemann_integral(recall, precision))
-        auprc_result = torch.tensor(auprcs, device=input.device)
-    auprc_result = torch.nan_to_num(auprc_result, nan=0.0)
-    return auprc_result, threshold
-
-
-def _binary_binned_auprc_param_check(
-    num_tasks: int,
-    threshold: torch.Tensor,
-) -> None:
-    if num_tasks < 1:
-        raise ValueError("`num_tasks` has to be at least 1.")
+    _binary_precision_recall_curve_update(input, target)
+    return _binary_precision_recall_curve_compute(input, target)
 
-    if threshold.ndim != 1:
-        raise ValueError(
-            f"`threshold` should be 1-dimensional, but got {threshold.ndim}D tensor."
-        )
 
-    if (torch.diff(threshold) < 0.0).any():
-        raise ValueError("The `threshold` should be a sorted tensor.")
+def _binary_precision_recall_curve_update(
+    input: torch.Tensor,
+    target: torch.Tensor,
+) -> None:
+    _binary_precision_recall_curve_update_input_check(input, target)
 
-    if (threshold < 0.0).any() or (threshold > 1.0).any():
-        raise ValueError("The values in `threshold` should be in the range of [0, 1].")
 
-    if threshold[0] != 0:
-        raise ValueError("First value in `threshold` should be 0.")
+def _binary_precision_recall_curve_compute(
+    input: torch.Tensor,
+    target: torch.Tensor,
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    precision, recall, threshold = _compute_for_each_class(input, target, 1)
 
-    if threshold[-1] != 1:
-        raise ValueError("Last value in `threshold` should be 1.")
+    return precision, recall, threshold
 
 
-def _binary_binned_auprc_update_input_check(
+def _binary_precision_recall_curve_update_input_check(
     input: torch.Tensor,
     target: torch.Tensor,
-    num_tasks: int,
-    threshold: torch.Tensor,
 ) -> None:
+    if input.ndim != 1:
+        raise ValueError(
+            "input should be a one-dimensional tensor, " f"got shape {input.shape}."
+        )
+
+    if target.ndim != 1:
+        raise ValueError(
+            "target should be a one-dimensional tensor, " f"got shape {target.shape}."
+        )
+
     if input.shape != target.shape:
         raise ValueError(
             "The `input` and `target` should have the same shape, "
             f"got shapes {input.shape} and {target.shape}."
         )
-    elif num_tasks == 1:
-        # for num_tasks = 1, accept 1D or 2D tensor
-        if input.ndim not in (1, 2):
-            raise ValueError(
-                f"`num_tasks = 1`, `input` is expected to be 1D or 2D tensor, but got shape {input.shape}."
-            )
-    else:
-        # for num_tasks > 1, accept 2D tensor only, and the shape should be (num_tasks, num_samples)
-        if input.ndim != 2:
-            raise ValueError(
-                f"`num_tasks = {num_tasks}`, `input` is expected to be 2D tensor, but got shape {input.shape}."
-            )
-        elif input.shape[0] != num_tasks:
-            raise ValueError(
-                f"`num_tasks = {num_tasks}`, `input`'s shape is expected to be ({num_tasks}, num_samples), but got shape {input.shape}."
-            )
 
 
 @torch.inference_mode()
-def multiclass_binned_auprc(
+def multiclass_precision_recall_curve(
     input: torch.Tensor,
     target: torch.Tensor,
     *,
-    num_classes: int,
-    threshold: Union[int, List[float], torch.Tensor] = DEFAULT_NUM_THRESHOLD,
-    average: Optional[str] = "macro",
-) -> Tuple[torch.Tensor, torch.Tensor]:
+    num_classes: Optional[int] = None,
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], List[torch.Tensor]]:
     """
-    Binned Version of AUPRC, which is the area under the AUPRC Curve, for multiclass classification.
-    Its class version is ``torcheval.metrics.MulticlassBinnedAUPRC``.
+    Returns precision-recall pairs and their corresponding thresholds for
+    multi-class classification tasks. If a class is missing from the target
+    tensor, its recall values are set to 1.0.
 
-    Computation is done by computing the area under the precision/recall curve; precision and recall
-    are computed for the buckets defined by `threshold`.
+    Its class version is ``torcheval.metrics.MulticlassPrecisionRecallCurve``.
+    See also :func:`binary_precision_recall_curve <torcheval.metrics.functional.binary_precision_recall_curve>`, :func:`multilabel_precision_recall_curve <torcheval.metrics.functional.multilabel_precision_recall_curve>`
 
     Args:
         input (Tensor): Tensor of label predictions
-            It should be probabilities or logits with shape of (n_samples, n_classes).
+            It should be probabilities or logits with shape of (n_sample, n_class).
         target (Tensor): Tensor of ground truth labels with shape of (n_samples, ).
-        num_classes (int): Number of classes.
-        threshold (Tensor, int, List[float]): Either an integer representing the number of bins, a list of thresholds, or a tensor of thresholds.
-                    The same thresholds will be used for all tasks.
-                    If `threshold` is a tensor, it must be 1D.
-                    If list or tensor is given, the first element must be 0 and the last must be 1.
-        average (str, optional):
-            - ``'macro'`` [default]:
-                Calculate metrics for each class separately, and return their unweighted mean.
-            - ``None``:
-                Calculate the metric for each class separately, and return
-                the metric for every class.
+        num_classes (Optional):
+            Number of classes. Set to the second dimension of the input if num_classes is None.
+
+    Return:
+        a tuple of (precision: List[torch.Tensor], recall: List[torch.Tensor], thresholds: List[torch.Tensor])
+            precision: List of precision result. Each index indicates the result of a class.
+            recall: List of recall result. Each index indicates the result of a class.
+            thresholds: List of threshold. Each index indicates the result of a class.
 
     Examples::
 
         >>> import torch
-        >>> from torcheval.metrics.functional import multiclass_binned_auroc
-        >>> input = torch.tensor([[0.1, 0.2, 0.1], [0.4, 0.2, 0.1], [0.6, 0.1, 0.2], [0.4, 0.2, 0.3], [0.6, 0.2, 0.4]])
-        >>> target = torch.tensor([0, 1, 2, 1, 0])
-        >>> multiclass_binned_auprc(input, target, num_classes=3, threshold=5, average='macro')
-        tensor(0.35)
-        >>> multiclass_binned_auprc(input, target, num_classes=3, threshold=5, average=None)
-        tensor([0.4500, 0.4000, 0.2000])
-        >>> input = torch.tensor([[0.1, 0.2, 0.1, 0.4], [0.4, 0.2, 0.1, 0.7], [0.6, 0.1, 0.2, 0.4], [0.4, 0.2, 0.3, 0.2], [0.6, 0.2, 0.4, 0.5]])
-        >>> target = torch.tensor([0, 1, 2, 1, 0])
-        >>> threshold = torch.tensor([0.0, 0.1, 0.4, 0.7, 0.8, 1.0])
-        >>> multiclass_binned_auprc(input, target, num_classes=4, threshold=threshold, average='macro')
-        tensor(0.24375)
-        >>> multiclass_binned_auprc(input, target, num_classes=4, threshold=threshold, average=None)
-        tensor([0.3250, 0.2000, 0.2000, 0.2500])
+        >>> from torcheval.metrics.functional import multiclass_precision_recall_curve
+        >>> input = torch.tensor([[0.1, 0.1, 0.1, 0.1], [0.5, 0.5, 0.5, 0.5], [0.7, 0.7, 0.7, 0.7], [0.8, 0.8, 0.8, 0.8]])
+        >>> target = torch.tensor([0, 1, 2, 3])
+        >>> multiclass_precision_recall_curve(input, target, num_classes=4)
+        ([tensor([0.2500, 0.0000, 0.0000, 0.0000, 1.0000]),
+        tensor([0.2500, 0.3333, 0.0000, 0.0000, 1.0000]),
+        tensor([0.2500, 0.3333, 0.5000, 0.0000, 1.0000]),
+        tensor([0.2500, 0.3333, 0.5000, 1.0000, 1.0000])],
+        [tensor([1., 0., 0., 0., 0.]),
+        tensor([1., 1., 0., 0., 0.]),
+        tensor([1., 1., 1., 0., 0.]),
+        tensor([1., 1., 1., 1., 0.])],
+        [tensor([0.1000, 0.5000, 0.7000, 0.8000]),
+        tensor([0.1000, 0.5000, 0.7000, 0.8000]),
+        tensor([0.1000, 0.5000, 0.7000, 0.8000]),
+        tensor([0.1000, 0.5000, 0.7000, 0.8000])])
     """
-    threshold = _create_threshold_tensor(threshold, target.device)
-    _multiclass_binned_auprc_param_check(num_classes, threshold, average)
-    _multiclass_binned_auprc_update_input_check(input, target, num_classes)
-    return _multiclass_binned_auprc_compute(
-        input, target, num_classes, threshold, average
-    )
-
-
-def _multiclass_binned_auprc_compute(
-    input: torch.Tensor,
-    target: torch.Tensor,
-    num_classes: int,
-    threshold: torch.Tensor,
-    average: Optional[str] = "macro",
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    num_tp, num_fp, num_fn = _multiclass_binned_precision_recall_curve_update(
-        input, target, num_classes, threshold
-    )
-    prec, recall, thresh = _multiclass_binned_precision_recall_curve_compute(
-        num_tp, num_fp, num_fn, num_classes, threshold
-    )
-    auprcs = []
-    for p, r in zip(prec, recall):
-        auprcs.append(_riemann_integral(r, p))
-    auprcs = torch.tensor(auprcs).to(input.device).nan_to_num(nan=0.0)
-
-    if average == "macro":
-        return torch.mean(auprcs), threshold
-    else:
-        return auprcs, threshold
-
-
-def _multiclass_binned_auprc_param_check(
-    num_classes: int,
-    threshold: torch.Tensor,
-    average: Optional[str],
-) -> None:
-    average_options = ("macro", "none", None)
-    if average not in average_options:
-        raise ValueError(
-            f"`average` was not in the allowed value of {average_options}, got {average}."
-        )
-    if num_classes < 2:
-        raise ValueError("`num_classes` has to be at least 2.")
+    if num_classes is None and input.ndim == 2:
+        num_classes = input.shape[1]
+    _multiclass_precision_recall_curve_update(input, target, num_classes)
+    return _multiclass_precision_recall_curve_compute(input, target, num_classes)
 
-    if threshold.ndim != 1:
-        raise ValueError(
-            f"`threshold` should be 1-dimensional, but got {threshold.ndim}D tensor."
-        )
 
-    if (torch.diff(threshold) < 0.0).any():
-        raise ValueError("The `threshold` should be a sorted tensor.")
-
-    if (threshold < 0.0).any() or (threshold > 1.0).any():
-        raise ValueError("The values in `threshold` should be in the range of [0, 1].")
+def _multiclass_precision_recall_curve_update(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_classes: Optional[int],
+) -> None:
+    _multiclass_precision_recall_curve_update_input_check(input, target, num_classes)
 
-    if threshold[0] != 0:
-        raise ValueError("First value in `threshold` should be 0.")
 
-    if threshold[-1] != 1:
-        raise ValueError("Last value in `threshold` should be 1.")
+@torch.jit.script
+def _multiclass_precision_recall_curve_compute(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_classes: Optional[int],
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], List[torch.Tensor]]:
+    if num_classes is None:
+        num_classes = input.shape[1]
+    thresholds, indices = input.T.sort(dim=1, descending=True)
+    mask = F.pad(thresholds.diff(dim=1) != 0, [0, 1], value=1.0).flip(1)
+    sizes: List[int] = mask.sum(1).tolist()
+    thresholds = thresholds.flip(1)[mask].split(sizes)
+
+    arange = torch.arange(num_classes, device=target.device)
+    cmp = target[indices] == arange[:, None]
+    num_tp = cmp.cumsum(1).flip(1)
+    num_fp = (~cmp).cumsum(1).flip(1)
+
+    # The last precision and recall values are 1.0 and 0.0, respectively
+    precision = F.pad(num_tp / (num_tp + num_fp), [0, 1], value=1.0)
+    recall = F.pad((num_tp / num_tp[:, :1]).nan_to_num_(1.0), [0, 1], value=0.0)
+    mask = F.pad(mask, [0, 1], value=1.0)
+    sizes: List[int] = mask.sum(1).tolist()
+
+    precision = precision[mask].split(sizes)
+    recall = recall[mask].split(sizes)
+    return list(precision), list(recall), list(thresholds)
 
 
-def _multiclass_binned_auprc_update_input_check(
+def _multiclass_precision_recall_curve_update_input_check(
     input: torch.Tensor,
     target: torch.Tensor,
-    num_classes: int,
+    num_classes: Optional[int],
 ) -> None:
     if input.size(0) != target.size(0):
         raise ValueError(
             "The `input` and `target` should have the same first dimension, "
             f"got shapes {input.shape} and {target.shape}."
         )
 
     if target.ndim != 1:
         raise ValueError(
             "target should be a one-dimensional tensor, " f"got shape {target.shape}."
         )
 
-    if not (input.ndim == 2 and input.shape[1] == num_classes):
+    if not (input.ndim == 2 and (num_classes is None or input.shape[1] == num_classes)):
         raise ValueError(
             f"input should have shape of (num_sample, num_classes), "
             f"got {input.shape} and num_classes={num_classes}."
         )
+
+
+@torch.jit.script
+def _compute_for_each_class(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    pos_label: int,
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    threshold, indices = input.sort(descending=True)
+    mask = F.pad(threshold.diff(dim=0) != 0, [0, 1], value=1.0)
+    num_tp = (target[indices] == pos_label).cumsum(0)[mask]
+    num_fp = (1 - (target[indices] == pos_label).long()).cumsum(0)[mask]
+    precision = (num_tp / (num_tp + num_fp)).flip(0)
+    recall = (num_tp / num_tp[-1]).flip(0)
+    threshold = threshold[mask].flip(0)
+
+    # The last precision and recall values are 1.0 and 0.0 without a corresponding threshold.
+    # This ensures that the graph starts on the y-axis.
+    precision = torch.cat([precision, precision.new_ones(1)])
+    recall = torch.cat([recall, recall.new_zeros(1)])
+
+    # If recalls are NaNs, set NaNs to 1.0s.
+    if torch.isnan(recall[0]):
+        recall = torch.nan_to_num(recall, 1.0)
+
+    return precision, recall, threshold
+
+
+@torch.inference_mode()
+def multilabel_precision_recall_curve(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    *,
+    num_labels: Optional[int] = None,
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], List[torch.Tensor]]:
+    """
+    Returns precision-recall pairs and their corresponding thresholds for
+    multi-label classification tasks. If there are no samples for a label
+    in the target tensor, its recall values are set to 1.0.
+
+    Its class version is ``torcheval.metrics.MultilabelPrecisionRecallCurve``.
+    See also :func:`binary_precision_recall_curve <torcheval.metrics.functional.binary_precision_recall_curve>`, :func:`multiclass_precision_recall_curve <torcheval.metrics.functional.multiclass_precision_recall_curve>`
+
+    Args:
+        input (Tensor): Tensor of label predictions
+            It should be probabilities or logits with shape of (n_sample, n_label).
+        target (Tensor): Tensor of ground truth labels with shape of (n_samples, n_label).
+        num_labels (Optional): Number of labels.
+
+    Return:
+        a tuple of (precision: List[torch.Tensor], recall: List[torch.Tensor], thresholds: List[torch.Tensor])
+            precision: List of precision result. Each index indicates the result of a label.
+            recall: List of recall result. Each index indicates the result of a label.
+            thresholds: List of threshold. Each index indicates the result of a label.
+
+    Examples::
+
+        >>> import torch
+        >>> from torcheval.metrics.functional import multilabel_precision_recall_curve
+        >>> input = torch.tensor([[0.75, 0.05, 0.35], [0.45, 0.75, 0.05], [0.05, 0.55, 0.75], [0.05, 0.65, 0.05]])
+        >>> target = torch.tensor([[1, 0, 1], [0, 0, 0], [0, 1, 1], [1, 1, 1]])
+        >>> multilabel_precision_recall_curve(input, target, num_labels=3)
+        ([tensor([0.5, 0.5, 1.0, 1.0]),
+        tensor([0.5, 0.66666667, 0.5, 0.0, 1.0]),
+        tensor([0.75, 1.0, 1.0, 1.0])],
+        [tensor([1.0, 0.5, 0.5, 0.0]),
+        tensor([1.0, 1.0, 0.5, 0.0, 0.0]),
+        tensor([1.0, 0.66666667, 0.33333333, 0.0])],
+        [tensor([0.05, 0.45, 0.75]),
+        tensor([0.05, 0.55, 0.65, 0.75]),
+        tensor([0.05, 0.35, 0.75])])
+    """
+    if input.ndim != 2:
+        raise ValueError(
+            f"input should be a two-dimensional tensor, got shape {input.shape}."
+        )
+    if num_labels is None:
+        num_labels = input.shape[1]
+    _multilabel_precision_recall_curve_update(input, target, num_labels)
+    return _multilabel_precision_recall_curve_compute(input, target, num_labels)
+
+
+def _multilabel_precision_recall_curve_update(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_labels: int,
+) -> None:
+    _multilabel_precision_recall_curve_update_input_check(input, target, num_labels)
+
+
+@torch.jit.script
+def _multilabel_precision_recall_curve_compute(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_labels: int,
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], List[torch.Tensor]]:
+    precisions, recalls, thresholds = [], [], []
+    for i in range(num_labels):
+        precision, recall, threshold = _compute_for_each_class(
+            input[:, i], target[:, i], 1
+        )
+        precisions.append(precision)
+        recalls.append(recall)
+        thresholds.append(threshold)
+    return precisions, recalls, thresholds
+
+
+def _multilabel_precision_recall_curve_update_input_check(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_labels: int,
+) -> None:
+    if input.shape != target.shape:
+        raise ValueError(
+            "Expected both input.shape and target.shape to have the same shape"
+            f" but got {input.shape} and {target.shape}."
+        )
+
+    if input.ndim != 2:
+        raise ValueError(
+            f"input should be a two-dimensional tensor, got shape {input.shape}."
+        )
+
+    if input.shape[1] != num_labels:
+        raise ValueError(
+            f"input should have shape of (num_sample, num_labels), "
+            f"got {input.shape} and num_labels={num_labels}."
+        )
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_auroc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List, Optional, Tuple, Union
 
 import torch
 from torch.nn import functional as F
 from torcheval.metrics.functional.classification.precision_recall_curve import (
     _binary_precision_recall_curve_update_input_check,
     _multiclass_precision_recall_curve_update_input_check,
+    _multilabel_precision_recall_curve_update_input_check,
 )
 from torcheval.metrics.functional.tensor_utils import _create_threshold_tensor
 
 
 @torch.inference_mode()
 def binary_binned_precision_recall_curve(
     input: torch.Tensor,
@@ -82,18 +83,34 @@
 
 @torch.jit.script
 def _update(
     input: torch.Tensor,
     target: torch.Tensor,
     threshold: torch.Tensor,
 ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-    pred_label = input >= threshold[:, None]
-    num_tp = (pred_label & target).sum(dim=1)
-    num_fp = pred_label.sum(dim=1) - num_tp
-    num_fn = target.sum() - num_tp
+    num_thresholds = len(threshold)
+
+    # (index, target) values, stored as 2 * index + target
+    index_target = (
+        2 * (torch.searchsorted(threshold, input, right=True) - 1) + target
+    ).type(torch.float64)
+    hist = torch.histc(
+        index_target, bins=2 * num_thresholds, min=0, max=2 * num_thresholds
+    )
+    # For each index j, Find the last index i such that input[j] >= threshold[i]
+
+    # false positives are positives_idx[0], true positives are positives_idx[1]
+    target_sum = target.sum()
+    positives_idx = hist.reshape((num_thresholds, 2)).T.type(target_sum.dtype)
+
+    # suffix sum: For each threshold index/("true/false" positives) combination,
+    # find how many indices j such that input[j] >= threshold[i]
+    suffix_total = positives_idx.flip(dims=(1,)).cumsum(dim=1).flip(dims=(1,))
+    num_fp, num_tp = suffix_total[0], suffix_total[1]
+    num_fn = target_sum - num_tp
     return num_tp, num_fp, num_fn
 
 
 @torch.jit.script
 def _binary_binned_precision_recall_curve_compute(
     num_tp: torch.Tensor,
     num_fp: torch.Tensor,
@@ -219,14 +236,146 @@
 
     return (
         list(precision.T),
         list(recall.T),
         threshold,
     )
 
+
+@torch.inference_mode()
+def multilabel_binned_precision_recall_curve(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_labels: Optional[int] = None,
+    threshold: Union[int, List[float], torch.Tensor] = 100,
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], torch.Tensor]:
+    """
+    Compute precision recall curve with given thresholds.
+    Its class version is ``torcheval.metrics.MultilabelBinnedPrecisionRecallCurve``.
+    See also :func:`binary_binned_precision_recall_curve <torcheval.metrics.functional.binary_binned_precision_recall_curve>`,
+    :func:`multiclass_precision_recall_curve <torcheval.metrics.functional.multiclass_precision_recall_curve>`
+
+    Args:
+        input (Tensor): Tensor of label predictions
+            It should be probabilities or logits with shape of (n_sample, n_label).
+        target (Tensor): Tensor of ground truth labels with shape of (n_samples, n_label).
+        num_labels (Optional): Number of labels.
+        threshold:
+            a integer representing number of bins, a list of thresholds,
+            or a tensor of thresholds.
+
+    Return:
+        a tuple of (precision: List[torch.Tensor], recall: List[torch.Tensor], thresholds: List[torch.Tensor])
+            precision: List of precision result. Each index indicates the result of a label.
+            recall: List of recall result. Each index indicates the result of a label.
+            thresholds: List of threshold. Each index indicates the result of a label.
+
+    Examples::
+
+        >>> import torch
+        >>> from torcheval.metrics.functional import multilabel_binned_precision_recall_curve
+        >>> input = torch.tensor([[0.75, 0.05, 0.35], [0.45, 0.75, 0.05], [0.05, 0.55, 0.75], [0.05, 0.65, 0.05]])
+        >>> target = torch.tensor([[1, 0, 1], [0, 0, 0], [0, 1, 1], [1, 1, 1]])
+        >>> multilabel_binned_precision_recall_curve(input, target, num_labels=3, thresholds=5)
+        (tensor([[0.5000, 0.5000, 1.0000, 1.0000, 0.0000, 1.0000],
+                 [0.5000, 0.6667, 0.6667, 0.0000, 0.0000, 1.0000],
+                 [0.7500, 1.0000, 1.0000, 1.0000, 0.0000, 1.0000]]),
+         tensor([[1.0000, 0.5000, 0.5000, 0.5000, 0.0000, 0.0000],
+                 [1.0000, 1.0000, 1.0000, 0.0000, 0.0000, 0.0000],
+                 [1.0000, 0.6667, 0.3333, 0.3333, 0.0000, 0.0000]]),
+         tensor([0.0000, 0.2500, 0.5000, 0.7500, 1.0000]))
+    """
+    threshold = _create_threshold_tensor(threshold, target.device)
+    _binned_precision_recall_curve_param_check(threshold)
+
+    if input.ndim != 2:
+        raise ValueError(
+            f"input should be a two-dimensional tensor, got shape {input.shape}."
+        )
+    if num_labels is None:
+        num_labels = input.shape[1]
+    num_tp, num_fp, num_fn = _multilabel_binned_precision_recall_curve_update(
+        input, target, num_labels, threshold
+    )
+    return _multilabel_binned_precision_recall_curve_compute(
+        num_tp, num_fp, num_fn, num_labels, threshold
+    )
+
+
+def _multilabel_binned_precision_recall_curve_update(
+    input: torch.Tensor,
+    target: torch.Tensor,
+    num_labels: int,
+    threshold: torch.Tensor,
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    _multilabel_precision_recall_curve_update_input_check(input, target, num_labels)
+
+    num_samples, num_labels = tuple(input.shape)
+    num_thresholds = len(threshold)
+
+    # For each sample index j and label k, we need:
+    # (largest_threshold_index, k, target[j, k])
+    # where largest_threshold_index is largest i such that input[j,k] >= threshold[i].
+    # We flatten this tuple into a single value.
+    largest_index = (
+        2
+        * (
+            num_labels * (torch.searchsorted(threshold, input, right=True) - 1)
+            + torch.arange(num_labels, device=input.device, dtype=torch.int64)
+        )
+        + target
+    )
+
+    hist = torch.histc(
+        largest_index.type(torch.float64),
+        bins=2 * num_thresholds * num_labels,
+        min=0,
+        max=2 * num_thresholds * num_labels,
+    )
+    class_counts = target.sum(dim=0)
+
+    # false positives are positives_idx[0], true positives are positives_idx[1]
+    positives_idx = (
+        hist.reshape((num_thresholds, num_labels, 2))
+        .transpose(0, 2)
+        .type(class_counts.dtype)
+    )
+
+    # suffix sum: For each threshold index/("true/false" positives) combination,
+    # find how many indices j such that input[j] >= threshold[i].
+    suffix_total = positives_idx.flip(dims=(-1,)).cumsum(dim=-1).flip(dims=(-1,))
+    num_fp, num_tp = suffix_total[0].T, suffix_total[1].T
+    num_fn = class_counts[None, :] - num_tp
+    return num_tp, num_fp, num_fn
+
+
+@torch.jit.script
+def _multilabel_binned_precision_recall_curve_compute(
+    num_tp: torch.Tensor,
+    num_fp: torch.Tensor,
+    num_fn: torch.Tensor,
+    num_labels: int,
+    threshold: torch.Tensor,
+) -> Tuple[List[torch.Tensor], List[torch.Tensor], torch.Tensor]:
+    # Set precision to 1.0 if all predictions are zeros.
+    precision = torch.nan_to_num(num_tp / (num_tp + num_fp), 1.0)
+    recall = num_tp / (num_tp + num_fn)
+
+    # The last precision and recall values are 1.0 and 0.0 without a corresponding threshold.
+    # This ensures that the graph starts on the y-axis.
+    assert isinstance(num_labels, int)
+    precision = torch.cat([precision, precision.new_ones(1, num_labels)], dim=0)
+    recall = torch.cat([recall, recall.new_zeros(1, num_labels)], dim=0)
+
+    return (
+        list(precision.T),
+        list(recall.T),
+        threshold,
+    )
+
 
 def _binned_precision_recall_curve_param_check(
     threshold: torch.Tensor,
 ) -> None:
     if (torch.diff(threshold) < 0.0).any():
         raise ValueError("The `threshold` should be a sorted tensor.")
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/confusion_matrix.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/f1_score.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/f1_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,15 @@
     f1 = torch.nan_to_num(f1)
 
     if average == "micro":
         return f1
     elif average == "macro":
         return f1.mean()
     elif average == "weighted":
-        # pyre-fixme[61]: `mask` is undefined, or not always defined.
-        return (f1 * (num_label[mask] / num_label.sum())).sum()
+        return (f1 * (num_label / num_label.sum())).sum()
     else:  # average is None
         return f1
 
 
 def _f1_score_param_check(
     num_classes: Optional[int],
     average: Optional[str],
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/precision.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,16 @@
     target: torch.Tensor,
     threshold: float = 0.5,
 ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
 
     _binary_precision_update_input_check(input, target)
 
     input = torch.where(input < threshold, 0, 1)
-    num_tp = (input & target).sum()
-    num_fp = (input & (~target)).sum()
+    num_tp = (input * target).sum(dim=-1)
+    num_fp = input.sum(dim=-1) - num_tp
 
     num_label = torch.tensor(0.0)
 
     return num_tp, num_fp, num_label
 
 
 def _binary_precision_update_input_check(
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/recall.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/image/psnr.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 # LICENSE file in the root directory of this source tree.
 
 from torcheval.metrics.functional.ranking.click_through_rate import click_through_rate
 from torcheval.metrics.functional.ranking.frequency import frequency_at_k
 from torcheval.metrics.functional.ranking.hit_rate import hit_rate
 from torcheval.metrics.functional.ranking.num_collisions import num_collisions
 from torcheval.metrics.functional.ranking.reciprocal_rank import reciprocal_rank
+from torcheval.metrics.functional.ranking.retrieval_precision import retrieval_precision
 from torcheval.metrics.functional.ranking.weighted_calibration import (
     weighted_calibration,
 )
 
 __all__ = [
     "click_through_rate",
     "frequency_at_k",
     "hit_rate",
     "num_collisions",
     "reciprocal_rank",
     "weighted_calibration",
+    "retrieval_precision",
 ]
 __doc_name__ = "Ranking Metrics"
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/click_through_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/frequency.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/frequency.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/hit_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/num_collisions.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/num_collisions.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/reciprocal_rank.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/ranking/weighted_calibration.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/mean_squared_error.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/regression/r2_score.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/tensor_utils.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/bleu.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/helper.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/perplexity.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_error_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_information_lost.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/functional/text/word_information_preserved.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/functional/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/image/psnr.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/metric.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/ranking/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/ranking/click_through_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/ranking/hit_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/ranking/reciprocal_rank.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/ranking/weighted_calibration.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/regression/mean_squared_error.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/regression/r2_score.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/bleu.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/perplexity.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/word_error_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/word_information_lost.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/text/word_information_preserved.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/toolkit.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/toolkit.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/__init__.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/auroc.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/click_through_rate.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/mean_squared_error.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/normalized_entropy.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/metrics/window/weighted_calibration.py` & `torcheval-nightly-2023.5.1/torcheval/metrics/window/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/tools/flops.py` & `torcheval-nightly-2023.5.1/torcheval/tools/flops.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
         >>> import copy
         >>> import torch
         >>> import torchvision.models as models
         >>> from torcheval.tools.flops import FlopTensorDispatchMode
 
         >>> module = models.resnet18()
-        >>> inp = torch.randn(1, 3, 224, 224)
+        >>> module_input = torch.randn(1, 3, 224, 224)
         >>> with FlopTensorDispatchMode(module) as ftdm:
         >>>     # count forward flops
         >>>     res = module(module_input).mean()
         >>>     flops_forward = copy.deepcopy(ftdm.flop_counts)
 
         >>>     # reset count before counting backward flops
         >>>     ftdm.reset()
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/tools/module_summary.py` & `torcheval-nightly-2023.5.1/torcheval/tools/module_summary.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/utils/test_utils/dummy_metric.py` & `torcheval-nightly-2023.5.1/torcheval/utils/test_utils/dummy_metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval/utils/test_utils/metric_class_tester.py` & `torcheval-nightly-2023.5.1/torcheval/utils/test_utils/metric_class_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     compute_result: Any
     # pyre-ignore[4]: There's no restrictions on return types of a specific metric computation
     merge_and_compute_result: Any
     num_total_updates: int = NUM_TOTAL_UPDATES
     num_processes: int = NUM_PROCESSES
     atol: float = 1e-8
     rtol: float = 1e-5
+    min_updates_before_compute: int = 0
     device: Literal["cuda", "cpu"] = "cpu"
 
 
 class MetricClassTester(unittest.TestCase):
     def setUp(self) -> None:
         self._test_case_spec = None
 
@@ -60,14 +61,15 @@
         # pyre-ignore[2]: There's no restrictions on return types of a specific metric computation
         compute_result: Any,
         # pyre-ignore[2]: There's no restrictions on return types of a specific metric computation
         merge_and_compute_result: Any = None,
         num_total_updates: int = NUM_TOTAL_UPDATES,
         num_processes: int = NUM_PROCESSES,
         test_merge_with_one_update: bool = True,
+        min_updates_before_compute: int = 0,
         atol: float = 1e-8,
         rtol: float = 1e-5,
         test_devices: Optional[List[str]] = None,
     ) -> None:
         """
         Run a test case to verify metric class implementations.
 
@@ -87,14 +89,15 @@
                 in update_kwargs.
             num_total_updates: Number of updates in the update_kwargs.
             num_processes: Number of processes for metric computation distributed
                 training. ``num_total_updates`` should be divisible by
                 ``num_processes``.
             test_merge_with_one_update: Whether to test merge_state when there's only
                 one update call applied to all metric instances.
+            min_updates_before_compute: Minimum number of updates before testing compute.
             atol: Absolute tolerance used in ``torch.testing.assert_close``
             rtol: Relative tolerance used in ``torch.testing.assert_close``
             test_devices: List of test devices. If None, will be determined
                 automatically.
         """
         # update args and state names should not be empty
         self.assertTrue(update_kwargs)
@@ -120,14 +123,15 @@
             update_kwargs,
             compute_result,
             merge_and_compute_result,
             num_total_updates,
             num_processes,
             atol,
             rtol,
+            min_updates_before_compute,
         )
 
         if test_devices is None:
             test_devices = ("cpu", "cuda") if torch.cuda.is_available() else ("cpu",)
 
         for device in test_devices:
             self._test_case_spec.device = device
@@ -168,15 +172,18 @@
         result = None
         test_metric = deepcopy(self._test_case_spec.metric)
         for i in range(self._test_case_spec.num_total_updates):
             # test chainable call
             current_batch_update_kwargs = {
                 k: v[i] for k, v in self._test_case_spec.update_kwargs.items()
             }
-            result = test_metric.update(**current_batch_update_kwargs).compute()
+            if i >= self._test_case_spec.min_updates_before_compute:
+                result = test_metric.update(**current_batch_update_kwargs).compute()
+            else:
+                test_metric.update(**current_batch_update_kwargs)
 
         final_computation_result = test_metric.compute()
         # compute result from single process should be same as one merged from multiple processes
         assert_result_close(
             final_computation_result,
             self._test_case_spec.compute_result,
             atol=self._test_case_spec.atol,
@@ -230,15 +237,17 @@
         # update, merge, compute
         for i in range(num_processes):
             for j in range(num_total_updates // num_processes):
                 metric_i_current_batch_update_kwargs = {
                     k: v[i * num_total_updates // num_processes + j]
                     for k, v in self._test_case_spec.update_kwargs.items()
                 }
-                test_metrics[i].update(**metric_i_current_batch_update_kwargs).compute()
+                test_metrics[i].update(**metric_i_current_batch_update_kwargs)
+                if j >= self._test_case_spec.min_updates_before_compute:
+                    test_metrics[i].compute()
         test_metrics_unmerged = [deepcopy(metric) for metric in test_metrics]
         final_computation_result = (
             test_metrics[0].merge_state(test_metrics[1:]).compute()
         )
         assert_result_close(
             final_computation_result,
             self._test_case_spec.merge_and_compute_result,
@@ -315,15 +324,17 @@
         num_processes = test_spec.num_processes
 
         for i in range(num_total_updates // num_processes):
             metric_current_batch_update_kwargs = {
                 k: v[rank * num_total_updates // num_processes + i]
                 for k, v in test_spec.update_kwargs.items()
             }
-            metric.update(**metric_current_batch_update_kwargs).compute()
+            metric.update(**metric_current_batch_update_kwargs)
+            if i >= test_spec.min_updates_before_compute:
+                metric.compute()
         final_computation_result = sync_and_compute(metric)
         if rank == 0:
             assert_result_close(
                 final_computation_result,
                 test_spec.merge_and_compute_result,
                 atol=test_spec.atol,
                 rtol=test_spec.rtol,
```

### Comparing `torcheval-nightly-2023.4.9/torcheval/version.py` & `torcheval-nightly-2023.5.1/torcheval/version.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/PKG-INFO` & `torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2023.4.9
+Version: 2023.5.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: image
 License-File: LICENSE
 
 # TorchEval
 
 <p align="center">
 <a href="https://github.com/pytorch/torcheval/actions?query=branch%3Amain"><img src="https://img.shields.io/github/actions/workflow/status/pytorch/torcheval/.github/workflows/unit_test.yaml?branch=main" alt="build status"></a>
 <a href="https://pypi.org/project/torcheval"><img src="https://img.shields.io/pypi/v/torcheval" alt="pypi version"></a>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2023.4.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2023.5.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE # TorchEval
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+image License-File: LICENSE # TorchEval
       [build_status] [pypi_version] [pypi_nightly_version] [bsd_license]
 [docs]
 **This library is currently in Alpha and currently does not have a stable
 release. The API may change and may not be backward compatible. If you have
 suggestions for improvements, please open a GitHub issue. We'd love to hear
 your feedback.** A library that contains a rich collection of performant
 PyTorch model metrics, a simple interface to create new metrics, a toolkit to
```

### Comparing `torcheval-nightly-2023.4.9/torcheval_nightly.egg-info/SOURCES.txt` & `torcheval-nightly-2023.5.1/torcheval_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,26 +55,28 @@
 torcheval/metrics/functional/image/psnr.py
 torcheval/metrics/functional/ranking/__init__.py
 torcheval/metrics/functional/ranking/click_through_rate.py
 torcheval/metrics/functional/ranking/frequency.py
 torcheval/metrics/functional/ranking/hit_rate.py
 torcheval/metrics/functional/ranking/num_collisions.py
 torcheval/metrics/functional/ranking/reciprocal_rank.py
+torcheval/metrics/functional/ranking/retrieval_precision.py
 torcheval/metrics/functional/ranking/weighted_calibration.py
 torcheval/metrics/functional/regression/__init__.py
 torcheval/metrics/functional/regression/mean_squared_error.py
 torcheval/metrics/functional/regression/r2_score.py
 torcheval/metrics/functional/text/__init__.py
 torcheval/metrics/functional/text/bleu.py
 torcheval/metrics/functional/text/helper.py
 torcheval/metrics/functional/text/perplexity.py
 torcheval/metrics/functional/text/word_error_rate.py
 torcheval/metrics/functional/text/word_information_lost.py
 torcheval/metrics/functional/text/word_information_preserved.py
 torcheval/metrics/image/__init__.py
+torcheval/metrics/image/fid.py
 torcheval/metrics/image/psnr.py
 torcheval/metrics/ranking/__init__.py
 torcheval/metrics/ranking/click_through_rate.py
 torcheval/metrics/ranking/hit_rate.py
 torcheval/metrics/ranking/reciprocal_rank.py
 torcheval/metrics/ranking/weighted_calibration.py
 torcheval/metrics/regression/__init__.py
```

