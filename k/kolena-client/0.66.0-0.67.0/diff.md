# Comparing `tmp/kolena_client-0.66.0.tar.gz` & `tmp/kolena_client-0.67.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.66.0.tar", max compression
+gzip compressed data, was "kolena_client-0.67.0.tar", max compression
```

## Comparing `kolena_client-0.66.0.tar` & `kolena_client-0.67.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11346 2023-04-26 17:53:30.336171 kolena_client-0.66.0/LICENSE
--rw-r--r--   0        0        0      556 2023-04-26 17:53:30.336171 kolena_client-0.66.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1405 2023-04-26 17:53:30.336171 kolena_client-0.66.0/README.md
--rw-r--r--   0        0        0     1356 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1725 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     7578 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7480 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5507 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      690 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/samples.py
--rw-r--r--   0        0        0      833 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0      784 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_utils/_consts.py
--rw-r--r--   0        0        0     1604 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     6883 2023-04-26 17:53:30.336171 kolena_client-0.66.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      579 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     2774 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1260 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/futures.py
--rw-r--r--   0        0        0     1183 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2646 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4161 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/log.py
--rw-r--r--   0        0        0      997 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     4768 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     6672 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/stratification.py
--rw-r--r--   0        0        0     1942 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3005 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    14006 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3578 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     2541 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4138 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8415 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13650 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    12938 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     4707 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0      689 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/_consts.py
--rw-r--r--   0        0        0    20512 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9248 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14560 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12177 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    17008 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15219 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     4134 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/initialize.py
--rw-r--r--   0        0        0     4504 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     6423 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    14664 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0     9312 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      625 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2738 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7436 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13248 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22814 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    11379 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9293 2023-04-26 17:53:30.340170 kolena_client-0.66.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     1927 2023-04-26 17:53:47.627808 kolena_client-0.66.0/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 kolena_client-0.66.0/setup.py
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 kolena_client-0.66.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-02 18:26:43.464893 kolena_client-0.67.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-02 18:26:43.464893 kolena_client-0.67.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1405 2023-05-02 18:26:43.464893 kolena_client-0.67.0/README.md
+-rw-r--r--   0        0        0     1356 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1725 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     7578 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7480 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5507 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      690 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/samples.py
+-rw-r--r--   0        0        0      833 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/_consts.py
+-rw-r--r--   0        0        0     1604 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     7031 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      579 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1260 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/futures.py
+-rw-r--r--   0        0        0     1183 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2646 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4866 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0      997 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     4768 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     6672 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/stratification.py
+-rw-r--r--   0        0        0     1942 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3005 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    14006 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3578 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     2541 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4138 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8540 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13501 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    12954 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     4707 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0      689 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/_consts.py
+-rw-r--r--   0        0        0    20512 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9301 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14447 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12177 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    17008 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15282 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     4134 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     6423 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    15849 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0     9312 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      625 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2738 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7571 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13233 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22814 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9155 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    11542 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9293 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     1927 2023-05-02 18:26:59.568960 kolena_client-0.67.0/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 kolena_client-0.67.0/setup.py
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 kolena_client-0.67.0/PKG-INFO
```

### Comparing `kolena_client-0.66.0/LICENSE` & `kolena_client-0.67.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/LICENSE_HEADER` & `kolena_client-0.67.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/README.md` & `kolena_client-0.67.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/__init__.py` & `kolena_client-0.67.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/__init__.py` & `kolena_client-0.67.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/__init__.py` & `kolena_client-0.67.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.67.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/client_log.py` & `kolena_client-0.67.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/core.py` & `kolena_client-0.67.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/detection.py` & `kolena_client-0.67.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/fr.py` & `kolena_client-0.67.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/generic.py` & `kolena_client-0.67.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/repository.py` & `kolena_client-0.67.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/samples.py` & `kolena_client-0.67.0/kolena/_api/v1/samples.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/token.py` & `kolena_client-0.67.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_api/v1/workflow.py` & `kolena_client-0.67.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/__init__.py` & `kolena_client-0.67.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/_consts.py` & `kolena_client-0.67.0/kolena/_utils/_consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.67.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/batched_load.py` & `kolena_client-0.67.0/kolena/_utils/batched_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,18 @@
     return init_response
 
 
 def upload_data_frame(df: pd.DataFrame, batch_size: int, load_uuid: str) -> None:
     num_chunks = math.ceil(len(df) / batch_size)
     chunk_iter = np.array_split(df, num_chunks) if num_chunks > 0 else []
 
-    for df_chunk in log.progress_bar(chunk_iter):
+    # only display progress bar if there are multiple chunks to upload
+    chunk_iter_logged = log.progress_bar(chunk_iter) if num_chunks > 1 else chunk_iter
+
+    for df_chunk in chunk_iter_logged:
         upload_data_frame_chunk(df_chunk, load_uuid)
 
 
 @retry(stop_max_attempt_number=3)
 def upload_data_frame_chunk(df_chunk: pd.DataFrame, load_uuid: str) -> None:
     # We use a file-like object here so that requests chunks the file upload
     # For reasons not entirely clear, this upload can fail with a broken connection if it is not chunked.
```

### Comparing `kolena_client-0.66.0/kolena/_utils/cli.py` & `kolena_client-0.67.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.67.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.67.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/datatypes.py` & `kolena_client-0.67.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/endpoints.py` & `kolena_client-0.67.0/kolena/_utils/endpoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,7 +65,25 @@
         path = "results/object-detection"
     elif workflow == WorkflowType.CLASSIFICATION.value:
         path = "results/classification"
     else:
         path = "results"
         params["workflow"] = workflow
     return f"{platform_url}/{path}?{urlencode(params)}"
+
+
+def get_test_suite_url(test_suite_id: int) -> str:
+    return _get_test_suite_url(get_client_state(), test_suite_id)
+
+
+def _get_test_suite_url(client_state: _ClientState, test_suite_id: int) -> str:
+    platform_url = _get_platform_url(client_state)
+    return f"{platform_url}/testing?{urlencode(dict(testSuiteId=test_suite_id))}"
+
+
+def get_model_url(model_id: int) -> str:
+    return _get_model_url(get_client_state(), model_id)
+
+
+def _get_model_url(client_state: _ClientState, model_id: int) -> str:
+    platform_url = _get_platform_url(client_state)
+    return f"{platform_url}/models?{urlencode(dict(modelIds=model_id))}"
```

### Comparing `kolena_client-0.66.0/kolena/_utils/frozen.py` & `kolena_client-0.67.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/futures.py` & `kolena_client-0.67.0/kolena/_utils/futures.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/geometry.py` & `kolena_client-0.67.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/inference_validators.py` & `kolena_client-0.67.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/instrumentation.py` & `kolena_client-0.67.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/krequests.py` & `kolena_client-0.67.0/kolena/_utils/krequests.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import uuid
 from typing import Any
 from typing import Dict
 
 import requests
 from requests import HTTPError
 from requests_toolbelt.adapters import socket_options
+from urllib3.util import Retry
 
 from kolena import __version__ as version
 from kolena._utils.endpoints import get_endpoint
 from kolena._utils.state import get_client_state
 from kolena._utils.state import kolena_initialized
 from kolena.errors import NameConflictError
 from kolena.errors import NotFoundError
@@ -42,14 +43,19 @@
 STATUS_CODE__CONFLICT = 409
 
 # Give the client 15 seconds to connect to kolena server
 # Slightly more than a multiple of 3, as per https://docs.python-requests.org/en/master/user/advanced/#timeouts
 CONNECTION_CONNECT_TIMEOUT = 15.05
 CONNECTION_READ_TIMEOUT = 60 * 60  # Give kolena server 1 hour to respond to client request
 
+# This only retries for failed DNS lookups, socket connections and connection timeouts.
+# HTTPAdapter sets this to 0 by default. https://requests.readthedocs.io/en/latest/_modules/requests/adapters/
+# Using the Retry object to configure a backoff which is not supported by using an int here.
+MAX_RETRIES = Retry(total=3, connect=3, read=0, redirect=0, status=0, backoff_factor=2)
+
 
 @kolena_initialized
 def _with_default_kwargs(**kwargs: Any) -> Dict[str, Any]:
     client_state = get_client_state()
     default_kwargs = {
         "timeout": (CONNECTION_CONNECT_TIMEOUT, CONNECTION_READ_TIMEOUT),
         "proxies": client_state.proxies,
@@ -66,37 +72,41 @@
         "headers": {**default_headers, **kwargs.get("headers", {})},
     }
 
 
 @kolena_initialized
 def get(endpoint_path: str, params: Any = None, **kwargs: Any) -> requests.Response:
     url = get_endpoint(endpoint_path=endpoint_path)
-    return requests.get(url=url, params=params, **_with_default_kwargs(**kwargs))
+    with requests.Session() as s:
+        s.mount("https://", socket_options.TCPKeepAliveAdapter(max_retries=MAX_RETRIES))
+        return s.get(url=url, params=params, **_with_default_kwargs(**kwargs))
 
 
 @kolena_initialized
 def post(endpoint_path: str, data: Any = None, json: Any = None, **kwargs: Any) -> requests.Response:
     url = get_endpoint(endpoint_path=endpoint_path)
     with requests.Session() as s:
-        s.mount("https://", socket_options.TCPKeepAliveAdapter())
+        s.mount("https://", socket_options.TCPKeepAliveAdapter(max_retries=MAX_RETRIES))
         return s.post(url=url, data=data, json=json, **_with_default_kwargs(**kwargs))
 
 
 @kolena_initialized
 def put(endpoint_path: str, data: Any = None, json: Any = None, **kwargs: Any) -> requests.Response:
     url = get_endpoint(endpoint_path=endpoint_path)
     with requests.Session() as s:
-        s.mount("https://", socket_options.TCPKeepAliveAdapter())
+        s.mount("https://", socket_options.TCPKeepAliveAdapter(max_retries=MAX_RETRIES))
         return s.put(url=url, data=data, json=json, **_with_default_kwargs(**kwargs))
 
 
 @kolena_initialized
 def delete(endpoint_path: str, **kwargs: Any) -> requests.Response:
     url = get_endpoint(endpoint_path=endpoint_path)
-    return requests.delete(url=url, **_with_default_kwargs(**kwargs))
+    with requests.Session() as s:
+        s.mount("https://", socket_options.TCPKeepAliveAdapter(max_retries=MAX_RETRIES))
+        return requests.delete(url=url, **_with_default_kwargs(**kwargs))
 
 
 def raise_for_status(response: requests.Response) -> None:
     if response.status_code == STATUS_CODE__UNAUTHORIZED:
         # HTTP 401 is "unauthorized" but used as "unauthenticated"
         raise UnauthenticatedError(response.content)
     if response.status_code == STATUS_CODE__NOT_FOUND:
```

### Comparing `kolena_client-0.66.0/kolena/_utils/log.py` & `kolena_client-0.67.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/repository.py` & `kolena_client-0.67.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/serde.py` & `kolena_client-0.67.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/serializable.py` & `kolena_client-0.67.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/state.py` & `kolena_client-0.67.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/stratification.py` & `kolena_client-0.67.0/kolena/_utils/stratification.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.67.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/_utils/validators.py` & `kolena_client-0.67.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/__init__.py` & `kolena_client-0.67.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/metadata.py` & `kolena_client-0.67.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/model.py` & `kolena_client-0.67.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.67.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.67.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.67.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.67.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.67.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/test_case.py` & `kolena_client-0.67.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/test_config.py` & `kolena_client-0.67.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/test_image.py` & `kolena_client-0.67.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/test_run.py` & `kolena_client-0.67.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/classification/test_suite.py` & `kolena_client-0.67.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/__init__.py` & `kolena_client-0.67.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_datatypes.py` & `kolena_client-0.67.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.67.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.67.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.67.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/inference.py` & `kolena_client-0.67.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.67.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/model.py` & `kolena_client-0.67.0/kolena/detection/_internal/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from kolena._api.v1.detection import Model as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
+from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestCase
 from kolena.detection._internal import BaseTestImage
 from kolena.detection._internal import BaseTestSuite
@@ -87,28 +88,30 @@
         self._id = loaded.id
         self._workflow = WorkflowType(loaded.workflow)
         self._freeze()
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _create(cls, workflow: WorkflowType, name: str, metadata: Dict[str, Any]) -> CoreAPI.EntityData:
-        log.info(f"creating new model '{name}'")
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.success(f"created new model '{name}'")
-        return from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        obj = from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        log.info(f"created model '{name}' ({get_model_url(obj.id)})")
+        return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str) -> CoreAPI.EntityData:
         request = CoreAPI.LoadByNameRequest(name=name)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        return from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        obj = from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        log.info(f"loaded model '{name}' ({get_model_url(obj.id)})")
+        return obj
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(
         self,
         test_object: Union[_TestCaseClass, _TestSuiteClass],
     ) -> List[Tuple[_TestImageClass, Optional[List[_InferenceClass]]]]:
         """
```

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.67.0/kolena/detection/_internal/test_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,46 +122,44 @@
         cls,
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
     ) -> "BaseTestCase":
         """Create a new test case with the provided name."""
-        log.info(f"creating new test case '{name}'")
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if images is not None:
             obj._hydrate(images)
-        log.success(f"created new test case '{name}'")
+        log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.EntityData:
         """Load an existing test case with the provided name."""
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
+        log.info(f"loaded test case '{name}'")
         return from_dict(data_class=CoreAPI.EntityData, data=res.json())
 
     @validate_arguments(config=ValidatorConfig)
     def _hydrate(self, images: List[_TestImageClass], description: Optional[str] = None) -> None:
         if len(images) == 0:
             log.warn("no images provided, unable to populate test case")
             return
         with self.edit(reset=True) as editor:
             if description is not None:
                 editor.description(description)
-            log.info(f"adding images to test case '{self.name}'")
             for image in log.progress_bar(images):
                 editor.add(image)
-            log.success(f"added images to test case '{self.name}'")
 
     @classmethod
     def _create_from_data(cls, data: CoreAPI.EntityData) -> "BaseTestCase":
         assert_workflows_match(cls._workflow, data.workflow)
         return cls._from(data)
 
     @validate_arguments(config=ValidatorConfig)
@@ -304,15 +302,15 @@
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited:
             return
 
-        log.info(f"updating test case '{self.name}'")
+        log.info(f"editing test case '{self.name}'")
         init_response = init_upload()
         df = self._to_data_frame(list(editor._images.values()))
         df_serialized = df.as_serializable()
         upload_data_frame(df=df_serialized, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
 
         request = CoreAPI.CompleteEditRequest(
             test_case_id=self._id,
@@ -324,8 +322,8 @@
         complete_res = krequests.put(
             endpoint_path=API.Path.COMPLETE_EDIT,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=CoreAPI.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"updated test case '{self.name}'")
+        log.success(f"edited test case '{self.name}'")
```

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.67.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.67.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.67.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.67.0/kolena/detection/_internal/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from pydantic import validate_arguments
 
 import kolena._api.v1.core as CoreAPI
 from kolena._api.v1.detection import TestSuite as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
+from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestCase
 from kolena.errors import NotFoundError
 from kolena.workflow._validators import assert_workflows_match
@@ -106,23 +107,22 @@
         cls,
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         test_cases: Optional[List[BaseTestCase]] = None,
     ) -> "BaseTestSuite":
         """Create a new test suite with the provided name."""
-        log.info(f"creating new test suite '{name}'")
         request = CoreAPI.TestSuite.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_cases is not None:
             obj._hydrate(test_cases)
-        log.success(f"created new test suite '{name}'")
+        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.TestSuite.EntityData:
         """Retrieve the existing test suite with the provided name."""
         request = CoreAPI.TestSuite.LoadByNameRequest(name=name, version=version)
@@ -134,18 +134,16 @@
     @validate_arguments(config=ValidatorConfig)
     def _hydrate(self, test_cases: List[BaseTestCase], description: Optional[str] = None) -> None:
         """Convenience method to hydrate an empty test suite with the provided test cases"""
         with self.edit(reset=True) as editor:
             if description is not None:
                 editor.description(description)
             if len(test_cases):
-                log.info(f"adding test cases to test suite '{self.name}'")
                 for test_case in log.progress_bar(test_cases):
                     editor.add(test_case)
-                log.info(f"added test cases to test suite '{self.name}'")
 
     @classmethod
     def _create_from_data(cls, data: CoreAPI.TestSuite.EntityData) -> "BaseTestSuite":
         assert_workflows_match(cls._workflow, data.workflow)
         obj = cls.__new__(cls)
         obj._id = data.id
         obj.name = data.name
@@ -179,15 +177,17 @@
 
         :param name: the name of the test suite to load.
         :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
         :return: the loaded test suite.
         """
         data = cls._load_by_name(name, version)
-        return cls._create_from_data(data)
+        obj = cls._create_from_data(data)
+        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        return obj
 
     class Editor:
         """
         Interface to edit a test suite. Create with :meth:`TestSuite.edit`.
         """
 
         _test_cases: List[BaseTestCase]
@@ -285,25 +285,25 @@
 
         yield editor
 
         if not editor._edited():
             log.info("no op: nothing edited")
             return
 
-        log.info(f"updating test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}'")
         request = CoreAPI.TestSuite.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             test_case_ids=list(editor._test_cases.values()),
         )
         data = json.dumps(dataclasses.asdict(request))
         res = krequests.post(endpoint_path=API.Path.EDIT, data=data)
         krequests.raise_for_status(res)
-        log.success(f"updated test suite '{self.name}'")
         test_suite_data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
+        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(test_suite_data.id)})")
         with self._unfrozen():
             self.version = test_suite_data.version
             self.description = test_suite_data.description
             self.test_cases = [self._test_case_from(tc) for tc in test_suite_data.test_cases]
             self._id = test_suite_data.id
```

### Comparing `kolena_client-0.66.0/kolena/detection/ground_truth.py` & `kolena_client-0.67.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/inference.py` & `kolena_client-0.67.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/metadata.py` & `kolena_client-0.67.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/model.py` & `kolena_client-0.67.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/test_case.py` & `kolena_client-0.67.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/test_config.py` & `kolena_client-0.67.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/test_image.py` & `kolena_client-0.67.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/test_run.py` & `kolena_client-0.67.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/detection/test_suite.py` & `kolena_client-0.67.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/errors.py` & `kolena_client-0.67.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/__init__.py` & `kolena_client-0.67.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/_consts.py` & `kolena_client-0.67.0/kolena/fr/_consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/datatypes.py` & `kolena_client-0.67.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/model.py` & `kolena_client-0.67.0/kolena/fr/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import numpy as np
 from pydantic.dataclasses import dataclass
 
 from kolena._api.v1.fr import Model as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.endpoints import get_model_url
 from kolena._utils.serde import from_dict
 from kolena._utils.uninstantiable import Uninstantiable
 from kolena._utils.validators import ValidatorConfig
 from kolena.fr import TestCase
 from kolena.fr import TestSuite
 from kolena.fr.datatypes import LoadedPairResultDataFrame
 
@@ -52,36 +53,36 @@
         Create a new model with the provided name and metadata.
 
         :param name: unique name of the new model to create
         :param metadata: unstructured metadata to associate with the model
         :return: the created model
         :raises ValueError: if a model by the provided name already exists
         """
-        log.info(f"creating model '{name}'")
         request = API.CreateRequest(name=name, metadata=metadata)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.success(f"created model '{name}'")
-        return Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
+        obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
+        log.info(f"created model '{name}' ({get_model_url(obj.data.id)})")
+        return obj
 
     @classmethod
     def load_by_name(cls, name: str) -> "Model":
         """
         Retrieve the existing model with the provided name.
 
         :param name: name of the model to retrieve
         :return: the retrieved model
         :raises KeyError: if no model with the provided name exists
         """
-        log.info(f"loading model '{name}'")
         request = API.LoadByNameRequest(name=name)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.success(f"loaded model '{name}'")
-        return Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
+        obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
+        log.info(f"loaded model '{name}' ({get_model_url(obj.data.id)})")
+        return obj
 
     def _get_load_pair_results_request(
         self,
         test_object: Union[TestSuite, TestSuite.Data, TestCase, TestCase.Data],
     ) -> API.LoadPairResultsRequest:
         if isinstance(test_object, TestSuite):
             return API.LoadPairResultsRequest(model_id=self.data.id, test_suite_id=test_object.data.id)
```

### Comparing `kolena_client-0.66.0/kolena/fr/test_case.py` & `kolena_client-0.67.0/kolena/fr/test_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,23 +120,22 @@
         Create a new test case with the provided name.
 
         :param name: the name of the new test case to create.
         :param description: optional free-form description of the test case to create.
         :param test_samples: optionally specify a set of test samples to populate the test case.
         :return: the newly created test case.
         """
-        log.info(f"creating new test case '{name}'")
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_samples is not None:
             obj._hydrate(test_samples)
-        log.success(f"created new test case '{name}'")
+        log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
@@ -158,20 +157,19 @@
             of the test case with the provided name is returned
         :return: the loaded test case
         """
         return cls.load(name, version)
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestCase":
-        log.info(f"loading test case '{name}'")
         request = API.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
-        log.success(f"loaded test case '{name}'")
+        log.info(f"loaded test case '{name}'")
         return cls._create_from_data(data)
 
     def load_data(self) -> TestCaseDataFrame:
         """
         Load all pairs data for a test case.
 
         :return: a DataFrame containing all pairs defined in this test case
@@ -310,15 +308,15 @@
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited():
             return
 
-        log.info(f"updating test case '{self.name}'")
+        log.info(f"editing test case '{self.name}'")
         init_response = init_upload()
         df = pd.DataFrame(editor._samples.values(), columns=TEST_CASE_COLUMNS)
         df_validated = validate_df_schema(df, TestCaseDataFrameSchema)
 
         upload_data_frame(df=df_validated, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
         request = API.CompleteEditRequest(
             test_case_id=self._id,
@@ -330,15 +328,15 @@
         complete_res = krequests.post(
             endpoint_path=API.Path.COMPLETE_EDIT,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=API.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"updated test case '{self.name}'")
+        log.success(f"edited test case '{self.name}'")
 
     @validate_arguments
     def iter_data(self, batch_size: int = 10_000_000) -> Iterator[TestCaseDataFrame]:
         """
         Iterator of DataFrames describing all pairs data for a test case.
 
         :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
```

### Comparing `kolena_client-0.66.0/kolena/fr/test_images.py` & `kolena_client-0.67.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/test_run.py` & `kolena_client-0.67.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/fr/test_suite.py` & `kolena_client-0.67.0/kolena/fr/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from deprecation import deprecated
 from pydantic import validate_arguments
 
 from kolena._api.v1.fr import TestSuite as API
 from kolena._utils import krequests
 from kolena._utils import log
+from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.fr.test_case import TestCase
 
@@ -118,22 +119,21 @@
         Create a new test suite with the provided name.
 
         :param name: the name of the new test suite to create.
         :param description: optional free-form description of the test suite to create.
         :param test_cases: optionally specify a set of test cases to populate the test suite.
         :return: the newly created test suite.
         """
-        log.info(f"creating test suite '{name}'")
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         obj._hydrate(baseline_test_cases, non_baseline_test_cases)
-        log.success(f"created test suite '{name}'")
+        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
 
@@ -156,20 +156,20 @@
         :return: the retrieved test suite.
         :raises NotFoundError: if the test suite with the provided name doesn't exist.
         """
         return cls.load(name, version)
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestSuite":
-        log.info(f"loading test suite '{name}'")
         request = API.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.success(f"loaded test suite '{name}'")
-        return cls._create_from_data(from_dict(data_class=API.EntityData, data=res.json()))
+        obj = cls._create_from_data(from_dict(data_class=API.EntityData, data=res.json()))
+        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        return obj
 
     def _populate_from_other(self, other: "TestSuite") -> None:
         with self._unfrozen():
             self._id = other._id
             self.name = other.name
             self.version = other.version
             self.description = other.description
@@ -323,21 +323,21 @@
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited:
             return
 
-        log.info(f"updating test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}'")
         request = API.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             baseline_test_case_ids=list(editor._baseline_test_cases.values()),
             non_baseline_test_case_ids=list(editor._non_baseline_test_cases.values()),
         )
         res = krequests.post(endpoint_path=API.Path.EDIT, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=API.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
-        log.success(f"updated test suite '{self.name}'")
+        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(self._id)})")
```

### Comparing `kolena_client-0.66.0/kolena/initialize.py` & `kolena_client-0.67.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/__init__.py` & `kolena_client-0.67.0/kolena/workflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .model import Model
 from .evaluator import AxisConfig
 from .evaluator import Plot
 from .evaluator import Curve
 from .evaluator import CurvePlot
 from .evaluator import ConfusionMatrix
 from .evaluator import Histogram
+from .evaluator import BarPlot
 from .evaluator import MetricsTestCase
 from .evaluator import MetricsTestSample
 from .evaluator import MetricsTestSuite
 from .evaluator import Evaluator
 from .evaluator import EvaluatorConfiguration
 from .evaluator_function import BasicEvaluatorFunction as _BasicEvaluatorFunction
 from .evaluator_function import TestCases
@@ -68,14 +69,15 @@
     "Model",
     "AxisConfig",
     "Plot",
     "Curve",
     "CurvePlot",
     "ConfusionMatrix",
     "Histogram",
+    "BarPlot",
     "MetricsTestCase",
     "MetricsTestSample",
     "MetricsTestSuite",
     "Evaluator",
     "EvaluatorConfiguration",
     "BasicEvaluatorFunction",
     "TestCases",
```

### Comparing `kolena_client-0.66.0/kolena/workflow/_datatypes.py` & `kolena_client-0.67.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/_helpers.py` & `kolena_client-0.67.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/_validators.py` & `kolena_client-0.67.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/annotation.py` & `kolena_client-0.67.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/asset.py` & `kolena_client-0.67.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/evaluator.py` & `kolena_client-0.67.0/kolena/workflow/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 NullableNumberSeries = Sequence[Union[float, int, None]]
 
 
 class _PlotType(DataType):
     CURVE = "CURVE"
     CONFUSION_MATRIX = "CONFUSION_MATRIX"
     HISTOGRAM = "HISTOGRAM"
+    BAR = "BAR"
 
     @staticmethod
     def _data_category() -> str:
         return "PLOT"
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
@@ -195,14 +196,48 @@
 
     @staticmethod
     def _data_type() -> _PlotType:
         return _PlotType.HISTOGRAM
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
+class BarPlot(Plot):
+    """A plot visualizing a set of bars per test case."""
+
+    title: str
+
+    #: Axis label for the axis along which the bars are laid out (``labels``).
+    x_label: str
+
+    #: Axis label for the axis corresponding to bar height (``values``).
+    y_label: str
+
+    #: Labels for each bar with corresponding height specified in ``values``.
+    labels: Sequence[Union[str, int, float]]
+
+    #: Values for each bar with corresponding label specified in ``labels``.
+    values: NullableNumberSeries
+
+    #: Custom format options to allow for control over the display of the numerical plot axis (``values``).
+    config: Optional[AxisConfig] = None
+
+    def __post_init_post_parse__(self) -> None:
+        n_labels, n_values = len(self.labels), len(self.values)
+        if n_labels == 0 or n_values == 0 or n_labels != n_values:
+            raise ValueError(
+                f"Series 'labels' (length: {n_labels}) and 'values' (length: {n_values}) "
+                "must be equal length and non-empty",
+            )
+
+    @staticmethod
+    def _data_type() -> _PlotType:
+        return _PlotType.BAR
+
+
+@dataclass(frozen=True, config=ValidatorConfig)
 class ConfusionMatrix(Plot):
     """
     A confusion matrix. Example:
 
     .. code-block:: python
 
         ConfusionMatrix(
```

### Comparing `kolena_client-0.66.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.67.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/ground_truth.py` & `kolena_client-0.67.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/inference.py` & `kolena_client-0.67.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.67.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.67.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/model.py` & `kolena_client-0.67.0/kolena/workflow/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from kolena._api.v1.core import Model as CoreAPI
 from kolena._api.v1.generic import Model as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.workflow import GroundTruth
@@ -107,34 +108,36 @@
         Create a new model.
 
         :param name: the unique name of the new model to create.
         :param infer: optional inference function for this model.
         :param metadata: optional unstructured metadata to store with this model.
         :return: the newly created model.
         """
-        log.info(f"creating model '{name}'")
         metadata = metadata or {}
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.success(f"created model '{name}'")
-        return cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
+        obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
+        log.info(f"created model '{name}' ({get_model_url(obj._id)})")
+        return obj
 
     @classmethod
     def load(cls, name: str, infer: Optional[Callable[[TestSample], Inference]] = None) -> "Model":
         """
         Load an existing model.
 
         :param name: the name of the model to load.
         :param infer: optional inference function for this model.
         """
         request = CoreAPI.LoadByNameRequest(name=name)
         res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        return cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
+        obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
+        log.info(f"loaded model '{name}' ({get_model_url(obj._id)})")
+        return obj
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(self, test_case: TestCase) -> List[Tuple[TestSample, GroundTruth, Inference]]:
         """
         Load all inferences stored for this model on the provided test case.
 
         :param test_case: the test case for which to load inferences.
```

### Comparing `kolena_client-0.66.0/kolena/workflow/test_case.py` & `kolena_client-0.67.0/kolena/workflow/test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,24 +151,23 @@
         Create a new test case with the provided name.
 
         :param name: the name of the new test case to create.
         :param description: optional free-form description of the test case to create.
         :param test_samples: optionally specify a set of test samples and ground truths to populate the test case.
         :return: the newly created test case.
         """
-        log.info(f"creating new test case '{name}'")
         cls._validate_test_samples(test_samples)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_samples is not None:
             obj._hydrate(test_samples)
-        log.success(f"created new test case '{name}'")
+        log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
@@ -177,14 +176,15 @@
             when unset.
         :return: the loaded test case.
         """
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        log.info(f"loaded test case '{name}'")
         return cls._create_from_data(data)
 
     def load_test_samples(self) -> List[Tuple[TestSample, GroundTruth]]:
         """Load all test samples and ground truths in this test case."""
         return list(self.iter_test_samples())
 
     def iter_test_samples(self) -> Iterator[Tuple[TestSample, GroundTruth]]:
@@ -287,15 +287,15 @@
         editor = self.Editor(self.description, reset)
 
         yield editor
 
         if not editor._edited():
             return
 
-        log.info(f"updating test case '{self.name}'")
+        log.info(f"editing test case '{self.name}'")
         init_response = init_upload()
         df_serialized = editor._to_data_frame().as_serializable()
         upload_data_frame(df=df_serialized, batch_size=_BatchSize.UPLOAD_RECORDS, load_uuid=init_response.uuid)
 
         request = CoreAPI.CompleteEditRequest(
             test_case_id=self._id,
             current_version=self.version,
@@ -306,8 +306,8 @@
         complete_res = krequests.put(
             endpoint_path=API.Path.COMPLETE_EDIT,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=CoreAPI.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"updated test case '{self.name}'")
+        log.success(f"edited test case '{self.name}'")
```

### Comparing `kolena_client-0.66.0/kolena/workflow/test_run.py` & `kolena_client-0.67.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/test_sample.py` & `kolena_client-0.67.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/kolena/workflow/test_suite.py` & `kolena_client-0.67.0/kolena/workflow/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from kolena._api.v1.core import TestSuite as CoreAPI
 from kolena._api.v1.generic import TestSuite as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils._consts import _BatchSize
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.workflow import TestSample
@@ -147,24 +148,23 @@
         Create a new test suite with the provided name.
 
         :param name: the name of the new test suite to create.
         :param description: optional free-form description of the test suite to create.
         :param test_cases: optionally specify a set of test cases to populate the test suite.
         :return: the newly created test suite.
         """
-        log.info(f"creating test suite '{name}'")
         cls._validate_test_cases(test_cases)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         if test_cases is not None:
             obj._hydrate(test_cases)
-        log.success(f"created test suite '{name}'")
+        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
 
@@ -173,15 +173,17 @@
             version when unset.
         :return: the loaded test suite.
         """
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
-        return cls._create_from_data(data)
+        obj = cls._create_from_data(data)
+        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        return obj
 
     class Editor:
         _test_cases: List[TestCase]
         _reset: bool
         _description: str
         _initial_test_case_ids: List[int]
         _initial_description: str
@@ -241,27 +243,27 @@
         editor = self.Editor(self.test_cases, self.description, reset)
 
         yield editor
 
         if not editor._edited():
             return
 
-        log.info(f"updating test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}'")
         request = CoreAPI.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             test_case_ids=[tc._id for tc in editor._test_cases],
         )
         res = krequests.post(endpoint_path=API.Path.EDIT, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
-        log.success(f"updated test suite '{self.name}'")
+        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(self._id)})")
 
     def load_test_samples(self) -> List[Tuple[TestCase, List[TestSample]]]:
         test_case_id_to_samples: Dict[int, List[TestSample]] = defaultdict(list)
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadTestSamplesRequest(
                 test_suite_id=self._id,
                 batch_size=_BatchSize.LOAD_SAMPLES,
```

### Comparing `kolena_client-0.66.0/kolena/workflow/workflow.py` & `kolena_client-0.67.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.66.0/pyproject.toml` & `kolena_client-0.67.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.66.0"
+version = "0.67.0"
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.66.0/setup.py` & `kolena_client-0.67.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                              'typing-extensions>=4.5.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena-client',
-    'version': '0.66.0',
+    'version': '0.67.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
     'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>\n  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\n`kolena-client` is the Python client library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 'click>=8.1.3,<9.0.0', 'dacite>=1.6', 'deprecation>=2.1.0,<3.0.0',
 'numpy>=1.19', 'pandas>=1.1,<1.6', 'pandera>=0.9.0', 'pyarrow>=8',
 'pydantic>=1.8', 'requests-toolbelt>=0.9.1,<0.10.0', 'requests>=2.20',
 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0', 'tqdm>=4,<5']
 extras_require = \ {':python_version < "3.8"': ['importlib-metadata<5.0',
 'typing-extensions>=4.5.0,<5.0.0']} entry_points = \ {'console_scripts':
 ['kolena = kolena._utils.cli:run']} setup_kwargs = { 'name': 'kolena-client',
-'version': '0.66.0', 'description': "Client for Kolena's machine learning (ML)
+'version': '0.67.0', 'description': "Client for Kolena's machine learning (ML)
 testing and debugging platform.", 'long_description': '
                                  \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena-client]\n [https://img.shields.io/
 pypi/l/kolena-client]\n [https://img.shields.io/badge/docs-
 Tutorial%20%26%20Usage-6434c1]\n [https://img.shields.io/badge/docs-
 API%20Reference-6434c1]\n
```

### Comparing `kolena_client-0.66.0/PKG-INFO` & `kolena_client-0.67.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.66.0
+Version: 0.67.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.66.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.67.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.11
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

