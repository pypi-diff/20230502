# Comparing `tmp/aligned-0.0.9.tar.gz` & `tmp/aligned-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned-0.0.9.tar", max compression
+gzip compressed data, was "aligned-0.0.9a0.tar", max compression
```

## Comparing `aligned-0.0.9.tar` & `aligned-0.0.9a0.tar`

### file list

```diff
@@ -1,86 +1,73 @@
--rw-r--r--   0        0        0    11358 2023-04-28 09:13:53.038535 aligned-0.0.9/LICENSE
--rw-r--r--   0        0        0     8876 2023-04-28 09:13:53.038535 aligned-0.0.9/README.md
--rw-r--r--   0        0        0     1334 2023-04-28 09:13:53.038535 aligned-0.0.9/aligned/__init__.py
--rw-r--r--   0        0        0     1159 2023-04-28 09:13:53.038535 aligned-0.0.9/aligned/active_learning/job.py
--rw-r--r--   0        0        0     1421 2023-04-28 09:13:53.038535 aligned-0.0.9/aligned/active_learning/selection.py
--rw-r--r--   0        0        0     2204 2023-04-28 09:13:53.038535 aligned-0.0.9/aligned/active_learning/write_policy.py
--rw-r--r--   0        0        0    14732 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/cli.py
--rw-r--r--   0        0        0     8405 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/aggregation_factory.py
--rw-r--r--   0        0        0      441 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/constraint_factory.py
--rw-r--r--   0        0        0    34543 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/feature_factory.py
--rw-r--r--   0        0        0     7934 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/model.py
--rw-r--r--   0        0        0     5835 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/repo_reader.py
--rw-r--r--   0        0        0    19119 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/transformation_factory.py
--rw-r--r--   0        0        0      825 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/compiler/vector_index_factory.py
--rw-r--r--   0        0        0      667 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/data_file.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/data_source/__init__.py
--rw-r--r--   0        0        0     3954 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/data_source/batch_data_source.py
--rw-r--r--   0        0        0     2257 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/data_source/stream_data_source.py
--rw-r--r--   0        0        0     6382 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/enricher.py
--rw-r--r--   0        0        0      278 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/entity_data_source.py
--rw-r--r--   0        0        0      282 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/exceptions.py
--rw-r--r--   0        0        0     7477 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_source.py
--rw-r--r--   0        0        0    24785 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_store.py
--rw-r--r--   0        0        0      298 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/__init__.py
--rw-r--r--   0        0        0     2837 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/combined_view.py
--rw-r--r--   0        0        0     8523 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/feature_view.py
--rw-r--r--   0        0        0      799 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/tests/test_brest_cancer.py
--rw-r--r--   0        0        0     2782 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
--rw-r--r--   0        0        0     1239 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/tests/test_combined_view.py
--rw-r--r--   0        0        0     1079 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/feature_view/tests/test_hidden_variable.py
--rw-r--r--   0        0        0     1074 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/jobs/tests/test_combined_job.py
--rw-r--r--   0        0        0     1981 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/jobs/tests/test_derived_job.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/local/__init__.py
--rw-r--r--   0        0        0     9429 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/local/job.py
--rw-r--r--   0        0        0    10179 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/local/source.py
--rw-r--r--   0        0        0     1523 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/local/tests/test_jobs.py
--rw-r--r--   0        0        0     3089 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/online_source.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/psql/__init__.py
--rw-r--r--   0        0        0     4847 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/psql/data_source.py
--rw-r--r--   0        0        0    24425 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/psql/jobs.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redis/__init__.py
--rw-r--r--   0        0        0     9775 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redis/config.py
--rw-r--r--   0        0        0     3874 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redis/job.py
--rw-r--r--   0        0        0     2275 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redis/stream.py
--rw-r--r--   0        0        0     5241 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redis/tests/test_redis_job.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redshift/__init__.py
--rw-r--r--   0        0        0     3381 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redshift/data_source.py
--rw-r--r--   0        0        0     1163 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redshift/factory.py
--rw-r--r--   0        0        0    21924 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/redshift/jobs.py
--rw-r--r--   0        0        0    11566 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/request/retrival_request.py
--rw-r--r--   0        0        0     1805 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/request/tests/test_feature_request_generation.py
--rw-r--r--   0        0        0    38970 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/retrival_job.py
--rw-r--r--   0        0        0        0 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/s3/__init__.py
--rw-r--r--   0        0        0     6706 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/s3/config.py
--rw-r--r--   0        0        0     1447 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/s3/factory.py
--rw-r--r--   0        0        0     2017 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/s3/storage.py
--rw-r--r--   0        0        0      251 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/codable.py
--rw-r--r--   0        0        0     3226 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/constraints.py
--rw-r--r--   0        0        0     3555 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/derivied_feature.py
--rw-r--r--   0        0        0     2745 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/event_trigger.py
--rw-r--r--   0        0        0     5744 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/feature.py
--rw-r--r--   0        0        0    11915 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/feature_view.py
--rw-r--r--   0        0        0     1677 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/folder.py
--rw-r--r--   0        0        0     3197 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/literal_value.py
--rw-r--r--   0        0        0     3392 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/model.py
--rw-r--r--   0        0        0     7558 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/repo_definition.py
--rw-r--r--   0        0        0     1437 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/target.py
--rw-r--r--   0        0        0     8709 2023-04-28 09:13:53.042535 aligned-0.0.9/aligned/schemas/text_vectoriser.py
--rw-r--r--   0        0        0    55554 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/schemas/transformation.py
--rw-r--r--   0        0        0     2330 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/schemas/vector_storage.py
--rw-r--r--   0        0        0     9437 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/server.py
--rw-r--r--   0        0        0     9598 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/split_strategy.py
--rw-r--r--   0        0        0      196 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/storage.py
--rw-r--r--   0        0        0      682 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_cache_enricher.py
--rw-r--r--   0        0        0      549 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_cached_parquet.py
--rw-r--r--   0        0        0     1900 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_model_target.py
--rw-r--r--   0        0        0     1496 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_models_as_feature.py
--rw-r--r--   0        0        0     2056 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_statistic_enricher.py
--rw-r--r--   0        0        0     1759 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_train_test_validate_set.py
--rw-r--r--   0        0        0      905 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/tests/test_transformations.py
--rw-r--r--   0        0        0      323 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/validation/interface.py
--rw-r--r--   0        0        0     3382 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/validation/pandera.py
--rw-r--r--   0        0        0      848 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/validation/tests/test_pandera_validator.py
--rw-r--r--   0        0        0    10512 2023-04-28 09:13:53.046535 aligned-0.0.9/aligned/worker.py
--rw-r--r--   0        0        0     2847 2023-04-28 09:13:53.046535 aligned-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    11600 1970-01-01 00:00:00.000000 aligned-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-03 20:34:00.544967 aligned-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     8521 2023-01-03 20:34:00.544967 aligned-0.0.9a0/README.md
+-rw-r--r--   0        0        0     1189 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/__init__.py
+-rw-r--r--   0        0        0    14066 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/cli.py
+-rw-r--r--   0        0        0      441 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/constraint_factory.py
+-rw-r--r--   0        0        0    19110 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/feature_factory.py
+-rw-r--r--   0        0        0     5784 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/repo_reader.py
+-rw-r--r--   0        0        0    18324 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/transformation_factory.py
+-rw-r--r--   0        0        0      822 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_file.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/__init__.py
+-rw-r--r--   0        0        0     3467 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/batch_data_source.py
+-rw-r--r--   0        0        0     1973 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/stream_data_source.py
+-rw-r--r--   0        0        0     8108 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/enricher.py
+-rw-r--r--   0        0        0      278 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/entity_data_source.py
+-rw-r--r--   0        0        0      341 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/exceptions.py
+-rw-r--r--   0        0        0     7657 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_source.py
+-rw-r--r--   0        0        0    17949 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_store.py
+-rw-r--r--   0        0        0      298 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/__init__.py
+-rw-r--r--   0        0        0     4969 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/combined_view.py
+-rw-r--r--   0        0        0    10029 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/feature_view.py
+-rw-r--r--   0        0        0      944 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py
+-rw-r--r--   0        0        0     3135 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
+-rw-r--r--   0        0        0     1239 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py
+-rw-r--r--   0        0        0     1692 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_hidden_variable.py
+-rw-r--r--   0        0        0     1074 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py
+-rw-r--r--   0        0        0     1981 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_derived_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/__init__.py
+-rw-r--r--   0        0        0     6962 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/job.py
+-rw-r--r--   0        0        0     8899 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/source.py
+-rw-r--r--   0        0        0     1105 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/tests/test_jobs.py
+-rw-r--r--   0        0        0     3006 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/model.py
+-rw-r--r--   0        0        0     2967 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/online_source.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/__init__.py
+-rw-r--r--   0        0        0     4431 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/data_source.py
+-rw-r--r--   0        0        0    10601 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/jobs.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/__init__.py
+-rw-r--r--   0        0        0     4348 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/config.py
+-rw-r--r--   0        0        0     3288 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/job.py
+-rw-r--r--   0        0        0     2275 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/stream.py
+-rw-r--r--   0        0        0     4402 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/tests/test_redis_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/__init__.py
+-rw-r--r--   0        0        0     2660 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/data_source.py
+-rw-r--r--   0        0        0     1172 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/factory.py
+-rw-r--r--   0        0        0     8250 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/retrival_request.py
+-rw-r--r--   0        0        0     1817 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py
+-rw-r--r--   0        0        0    15322 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/retrival_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/__init__.py
+-rw-r--r--   0        0        0     5715 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/config.py
+-rw-r--r--   0        0        0     1447 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/factory.py
+-rw-r--r--   0        0        0     1846 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/storage.py
+-rw-r--r--   0        0        0      251 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/codable.py
+-rw-r--r--   0        0        0     2356 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/constraints.py
+-rw-r--r--   0        0        0     1379 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/derivied_feature.py
+-rw-r--r--   0        0        0     3663 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature.py
+-rw-r--r--   0        0        0     8217 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature_view.py
+-rw-r--r--   0        0        0      409 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/model.py
+-rw-r--r--   0        0        0     4478 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/repo_definition.py
+-rw-r--r--   0        0        0    37245 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/transformation.py
+-rw-r--r--   0        0        0     8663 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/server.py
+-rw-r--r--   0        0        0     5086 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/split_strategy.py
+-rw-r--r--   0        0        0      196 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/storage.py
+-rw-r--r--   0        0        0      682 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cache_enricher.py
+-rw-r--r--   0        0        0      549 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cached_parquet.py
+-rw-r--r--   0        0        0     2056 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py
+-rw-r--r--   0        0        0     2371 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_train_test_validate_set.py
+-rw-r--r--   0        0        0      905 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_transformations.py
+-rw-r--r--   0        0        0      193 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/interface.py
+-rw-r--r--   0        0        0     2392 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/pandera.py
+-rw-r--r--   0        0        0      848 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py
+-rw-r--r--   0        0        0     3846 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/worker.py
+-rw-r--r--   0        0        0     2553 2023-01-03 20:34:00.552967 aligned-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 aligned-0.0.9a0/setup.py
+-rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 aligned-0.0.9a0/PKG-INFO
```

### Comparing `aligned-0.0.9/LICENSE` & `aligned-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/README.md` & `aligned-0.0.9a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 # Aligned
 
 Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
 
-Main advantages:
-- Test new features faster
-- Adapt faster to new technical and business requirements.
-- Stop technology lock-in, like processing engines and infrastructure.
-- Stop vendor lock-in. Deploy to any provider that fits you
-
-As a result, loading model featurs can be done with the following code.
-
-```python
-await store.model("titanic").features_for(entities).as_pandas()
-```
-
 Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
 
 Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
 
-Aligned is still in actice development, so changes are likely.
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
 ## Feature Views
 
 Write features as the should be, as data models.
 Then get code completion and typesafety by referencing them in other features.
 
 This makes the features light weight, data source indipendent, and flexible.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aligned-0.0.9/aligned/__init__.py` & `aligned-0.0.9a0/aligned/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,29 +8,27 @@
     EventTimestamp,
     Float,
     Int32,
     Int64,
     String,
     Timestamp,
 )
-from aligned.compiler.model import Model
 from aligned.data_source.stream_data_source import HttpStreamSource
 from aligned.feature_store import FeatureStore
 from aligned.feature_view import (
     CombinedFeatureView,
     CombinedFeatureViewMetadata,
     FeatureView,
     FeatureViewMetadata,
 )
 from aligned.local.source import FileSource
 from aligned.psql.data_source import PostgreSQLConfig
 from aligned.redis.config import RedisConfig
 from aligned.redshift.data_source import RedshiftSQLConfig
 from aligned.s3.config import AwsS3Config
-from aligned.schemas.text_vectoriser import TextVectoriserModel
 
 __all__ = [
     'FeatureStore',
     'FeatureView',
     'FeatureViewMetadata',
     'CombinedFeatureView',
     'CombinedFeatureViewMetadata',
@@ -50,10 +48,8 @@
     'Entity',
     'UUID',
     'Int32',
     'Int64',
     'Float',
     'EventTimestamp',
     'Timestamp',
-    'Model',
-    'TextVectoriserModel',
 ]
```

### Comparing `aligned-0.0.9/aligned/cli.py` & `aligned-0.0.9a0/aligned/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,132 +1,92 @@
 import asyncio
 import logging
 import os
 import sys
-from collections.abc import Callable
-from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
-from functools import wraps
 from pathlib import Path
-from typing import Any
+from typing import Any, Coroutine
 
 import click
 from pytz import utc  # type: ignore
 
-from aligned.compiler.repo_reader import RepoReader, RepoReference
+from aligned.compiler.repo_reader import RepoReader
 from aligned.feature_source import WritableFeatureSource
 from aligned.schemas.codable import Codable
 from aligned.schemas.feature import Feature
 from aligned.schemas.repo_definition import RepoDefinition
-from aligned.worker import StreamWorker
 
 
-def coro(func: Callable) -> Callable:
-    @wraps(func)
-    def wrapper(*args, **kwargs: Any) -> Any:
-        return asyncio.run(func(*args, **kwargs))
-
-    return wrapper
+def sync(method: Coroutine) -> Any:
+    return asyncio.get_event_loop().run_until_complete(method)
 
 
 def make_tzaware(t: datetime) -> datetime:
     """We assume tz-naive datetimes are UTC"""
     if t.tzinfo is None:
         return t.replace(tzinfo=utc)
     else:
         return t
 
 
 def load_envs(path: Path) -> None:
-    from dotenv import load_dotenv
+    if path.is_file():
+        import os
 
-    if not load_dotenv(path):
+        with path.open() as file:
+            for line in file:
+                if len(line) < 3:
+                    continue
+                key, value = line.strip().split('=')
+                os.environ[key] = value
+    else:
         click.echo(f'No env file found at {path}')
 
 
-def setup_logger():
-    from logging.config import dictConfig
-
-    handler = 'console'
-    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
-    dictConfig(
-        {
-            'version': 1,
-            'disable_existing_loggers': False,
-            'filters': {
-                'correlation_id': {
-                    '()': 'asgi_correlation_id.CorrelationIdFilter',
-                    'uuid_length': 16,
-                },
-            },
-            'formatters': {
-                'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
-            },
-            'handlers': {
-                'console': {
-                    'class': 'logging.StreamHandler',
-                    'filters': ['correlation_id'],
-                    'formatter': 'console',
-                }
-            },
-            'loggers': {
-                # project
-                '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
-            },
-        }
-    )
-
-
 @click.group()
 def cli() -> None:
     pass
 
 
 @cli.command('apply')
-@coro
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--reference-file',
-    default='feature_store_location.py:source',
+    default='feature_store_location.py',
     help='The path to a feature store reference file. Defining where to read and write the feature store',
 )
 @click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-async def apply_command(repo_path: str, reference_file: str, env_file: str) -> None:
+def apply_command(repo_path: str, reference_file: str, env_file: str) -> None:
     """
     Create or update a feature store deployment
     """
-    from aligned import FileSource
-
-    setup_logger()
 
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    path, obj = reference_file.split(':')
-    reference_file_path = Path(path).absolute()
+    reference_file_path = Path(reference_file).absolute()
     load_envs(dir / env_file)
     sys.path.append(str(dir))
+    repo_ref = RepoReader.reference_from_path(dir, reference_file_path)
 
-    repo_ref = RepoReference('const', {'const': FileSource.json_at('./feature-store.json')})
-    with suppress(ValueError):
-        repo_ref = RepoReference.reference_object(dir, reference_file_path, obj)
+    click.echo(f'Updating file at: {repo_ref.selected}')
 
-    if file := repo_ref.selected_file:
-        click.echo(f'Updating file at: {file}')
+    # old_def = sync(repo_ref.selected_file.feature_store())
 
-        repo_def = await RepoReader.definition_from_path(dir)
+    repo_def = sync(RepoReader.definition_from_path(dir))
 
-        await file.write(repo_def.to_json(omit_none=True).encode('utf-8'))
+    if file := repo_ref.selected_file:
+        sync(file.write(repo_def.to_json(omit_none=True).encode('utf-8')))
     else:
         click.echo(f'No repo file found at {dir}')
 
 
 @cli.command('plan')
 @click.option(
     '--repo-path',
@@ -153,15 +113,15 @@
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--host',
-    default=None,
+    default='127.0.0.1',
     help='The host to serve on',
 )
 @click.option(
     '--port',
     '-p',
     default=8000,
     help='The port to serve on',
@@ -181,29 +141,55 @@
     '--reload',
     '-r',
     default=False,
     help='If the server should reload on dir changes',
 )
 @click.option(
     '--server-path',
-    default='server:server',
+    default='feature_store_location:feature_server',
     help='The path to the feature store server',
 )
 def serve_command(
-    repo_path: str, port: int, workers: int, env_file: str, reload: bool, server_path: str, host: str | None
+    repo_path: str, host: str, port: int, workers: int, env_file: str, reload: bool, server_path: str
 ) -> None:
     """
     Starts a API serving the feature store
     """
-    import uvicorn
-
-    setup_logger()
+    from logging.config import dictConfig
 
-    host = host or os.getenv('HOST', '127.0.0.1')
+    import uvicorn
 
+    handler = 'console'
+    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
+    dictConfig(
+        {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'filters': {
+                'correlation_id': {
+                    '()': 'asgi_correlation_id.CorrelationIdFilter',
+                    'uuid_length': 16,
+                },
+            },
+            'formatters': {
+                'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
+            },
+            'handlers': {
+                'console': {
+                    'class': 'logging.StreamHandler',
+                    'filters': ['correlation_id'],
+                    'formatter': 'console',
+                }
+            },
+            'loggers': {
+                # project
+                '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
+            },
+        }
+    )
     os.environ['ALADDIN_ENABLE_SERVER'] = 'True'
     # Needed in order to find the feature_store_location file
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
     uvicorn.run(
@@ -213,58 +199,92 @@
         workers=workers or workers,
         reload=reload,
         env_file=env_file_path,
     )
 
 
 @cli.command('serve-worker')
-@coro
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
-    '--worker-path',
-    default='worker.py:worker',
-    help='The path to the `StreamWorker`',
+    '--reference-file',
+    default='feature_store_location.py',
+    help='The path to a feature store reference file. Defining where to read and write the feature store',
 )
 @click.option(
+    '--workers',
+    '-w',
+    default=1,
+    help='The number of workers',
+)
+@click.option('--views', '-v', help='The views to run in a worker', multiple=True)
+@click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-@click.option(
-    '--prune-unused-features',
-    default=False,
-    help='Will only process features that are used in a model if set to True',
-)
-async def serve_worker_command(
-    repo_path: str, worker_path: str, env_file: str, prune_unused_features: bool
+def serve_worker_command(
+    repo_path: str, reference_file: str, views: list[str], workers: int, env_file: str
 ) -> None:
     """
     Starts a API serving the feature store
     """
-    setup_logger()
+    from logging.config import dictConfig
 
+    from aligned.worker import start
+
+    handler = 'console'
+    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
+    dictConfig(
+        {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'filters': {
+                'correlation_id': {
+                    '()': 'asgi_correlation_id.CorrelationIdFilter',
+                    'uuid_length': 16,
+                },
+            },
+            'formatters': {
+                'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
+            },
+            'handlers': {
+                'console': {
+                    'class': 'logging.StreamHandler',
+                    'filters': ['correlation_id'],
+                    'formatter': 'console',
+                }
+            },
+            'loggers': {
+                # project
+                '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
+            },
+        }
+    )
     # Needed in order to find the feature_store_location file
-    path, obj = worker_path.split(':')
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    reference_file_path = Path(path).absolute()
+    reference_file_path = Path(reference_file).absolute()
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
 
-    worker = StreamWorker.from_object(dir, reference_file_path, obj)
+    repo_ref = RepoReader.reference_from_path(dir, reference_file_path)
+
+    if not repo_ref.selected_file:
+        raise ValueError('No selected feature store in the repo reference. Make sure the env var is set')
 
-    await worker.start(prune_unused_features)
+    feature_store = sync(repo_ref.selected_file.feature_store())
+
+    sync(start(store=feature_store, feature_views_to_process=set(views)))
 
 
 @cli.command('materialize')
-@coro
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--env-file',
@@ -275,40 +295,42 @@
     '--days',
     help='The number of days to materialize',
 )
 @click.option(
     '--view',
     help='The feature view to materialize',
 )
-async def materialize_command(repo_path: str, env_file: str, days: str, view: str) -> None:
+def materialize_command(repo_path: str, env_file: str, days: str, view: str) -> None:
     """
     Materializes the feature store
     """
     from aligned.feature_store import FeatureStore
 
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
     load_envs(dir / env_file)
 
     sys.path.append(str(dir))
-    repo_def = await RepoDefinition.from_path(repo_path)
+    repo_def = sync(RepoDefinition.from_path(repo_path))
     store = FeatureStore.from_definition(repo_def)
     batch_store = store.offline_store()
 
     if not isinstance(store.feature_source, WritableFeatureSource):
         raise ValueError('Batch feature sources are not supported for materialization')
 
     number_of_days = int(days)
     views = [view] if view else list(store.feature_views.keys())
 
     click.echo(f'Materializing the last {number_of_days} days')
     for feature_view in views:
         fv_store = batch_store.feature_view(feature_view)
         click.echo(f'Materializing {feature_view}')
-        await store.feature_source.write(
-            fv_store.previous(days=number_of_days), fv_store.view.request_all.needed_requests
+        sync(
+            store.feature_source.write(
+                fv_store.previous(days=number_of_days), fv_store.view.request_all.needed_requests
+            )
         )
 
 
 @dataclass
 class CategoricalFeatureSummary(Codable):
     missing_percentage: float
     unique_values: int
@@ -333,15 +355,14 @@
     numeric_features: dict[str, NumericFeatureSummary]
     categorical_features: dict[str, CategoricalFeatureSummary]
 
 
 # Should add some way of profiling models, not feature views.
 # Or maybe both
 @cli.command('profile')
-@coro
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--reference-file',
@@ -351,35 +372,35 @@
 @click.option('--output', default='profiling-result.json')
 @click.option('--dataset-size', default=10000)
 @click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-async def profile(repo_path: str, reference_file: str, env_file: str, output: str, dataset_size: int) -> None:
+def profile(repo_path: str, reference_file: str, env_file: str, output: str, dataset_size: int) -> None:
     import numpy as np
     from pandas import DataFrame
 
     from aligned import FeatureStore
 
     # Make sure modules can be read, and that the env is set
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
 
-    online_store: FeatureStore = await FeatureStore.from_reference_at_path(repo_path, reference_file)
+    online_store: FeatureStore = sync(FeatureStore.from_reference_at_path(repo_path, reference_file))
     feature_store = online_store.offline_store()
 
     results = ProfilingResult(numeric_features={}, categorical_features={})
 
     for feature_view_name in sorted(feature_store.feature_views.keys()):
         click.echo(f'Profiling: {feature_view_name}')
         feature_view = feature_store.feature_view(feature_view_name)
-        data_set: DataFrame = feature_view.all(limit=dataset_size).to_pandas()
+        data_set: DataFrame = sync(feature_view.all(limit=dataset_size).to_pandas())
 
         all_features: list[Feature] = list(feature_view.view.features) + list(
             feature_view.view.derived_features
         )
         for feature in all_features:
 
             data_slice = data_set[feature.name]
@@ -430,65 +451,10 @@
                     histogram_count=list(histogram),
                     histogram_splits=list(cuts),
                 )
 
     Path(output).write_bytes(results.to_json().encode('utf-8'))
 
 
-@cli.command('create_indexes')
-@coro
-@click.option(
-    '--repo-path',
-    default='.',
-    help='The path to the repo',
-)
-@click.option(
-    '--reference-file',
-    default='feature_store_location.py:source',
-    help='The path to a feature store reference file. Defining where to read and write the feature store',
-)
-@click.option(
-    '--env-file',
-    default='.env',
-    help='The path to env variables',
-)
-async def create_indexes(repo_path: str, reference_file: str, env_file: str) -> None:
-    from aligned import FeatureStore, FileSource
-
-    setup_logger()
-
-    # Make sure modules can be read, and that the env is set
-    path, obj = reference_file.split(':')
-    dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    reference_file_path = Path(path)
-
-    sys.path.append(str(dir))
-    env_file_path = dir / env_file
-    load_envs(env_file_path)
-
-    repo_ref = RepoReference('const', {'const': FileSource.json_at('./feature-store.json')})
-    with suppress(ValueError):
-        repo_ref = RepoReference.reference_object(dir, reference_file_path, obj)
-
-    if file := repo_ref.selected_file:
-        click.echo(f'Updating file at: {file}')
-
-        repo_def = await RepoReader.definition_from_path(dir)
-    else:
-        click.echo(f'No repo file found at {dir}. Returning without creating indexes')
-        return
-
-    feature_store = FeatureStore.from_definition(repo_def)
-
-    for feature_view_name in sorted(feature_store.feature_views.keys()):
-        view = feature_store.feature_views[feature_view_name]
-        if view.indexes is None:
-            continue
-
-        for index in view.indexes:
-            click.echo(f'Creating indexes for: {feature_view_name}, named {index.name}')
-            await index.storage.create_index(index)
-
-
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO, format='{asctime} {message}', style='{')
     cli()
```

### Comparing `aligned-0.0.9/aligned/compiler/repo_reader.py` & `aligned-0.0.9a0/aligned/compiler/repo_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
-from datetime import datetime
 from importlib import import_module
 from inspect import getmro, isclass
 from pathlib import Path
 from typing import Any
 
 from aligned.enricher import Enricher
+from aligned.model import Model
 from aligned.online_source import BatchOnlineSource, OnlineSource
-from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoMetadata, RepoReference
+from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoReference
 
 logger = logging.getLogger(__name__)
 
 
 def imports_for(file_path: Path) -> set[str]:
     try:
         with open(file_path) as file:
@@ -73,18 +73,15 @@
 class RepoReader:
     """
     A class reading a repo, and generates a repo config
     """
 
     @staticmethod
     async def definition_from_path(repo_path: Path) -> RepoDefinition:
-
-        metadata = RepoMetadata(created_at=datetime.now(), name=repo_path.name, github_url=None)
         repo = RepoDefinition(
-            metadata=metadata,
             feature_views=set(),
             combined_feature_views=set(),
             models=set(),
             online_source=BatchOnlineSource(),
             enrichers=[],
         )
 
@@ -107,37 +104,40 @@
 
             for attribute in dir(module):
                 if attribute in imports:
                     continue
 
                 obj = getattr(module, attribute)
 
-                if isinstance(obj, Enricher):
+                if isinstance(obj, Model):
+                    if not obj.name:
+                        obj.name = attribute
+                    repo.models.add(obj.schema())
+
+                elif isinstance(obj, Enricher):
                     repo.enrichers.append(
                         EnricherReference(module=module_path, attribute_name=attribute, enricher=obj)
                     )
                 elif isinstance(obj, OnlineSource):
                     repo.online_source = obj
                 else:
                     classes = super_classes_in(obj)
-                    if 'Model' in classes:
-                        repo.models.add(obj.compile())
-                    elif 'FeatureView' in classes:
-                        fv = obj.compile()
+                    if 'FeatureView' in classes:
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
                         feature_view_names[fv.name] = py_file.as_posix()
                         repo.feature_views.add(fv)
                     elif 'CombinedFeatureView' in classes:
-                        fv = obj.compile()
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
```

### Comparing `aligned-0.0.9/aligned/compiler/transformation_factory.py` & `aligned-0.0.9a0/aligned/compiler/transformation_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
+import asyncio
 from dataclasses import dataclass, field
 from datetime import timedelta
 from typing import Any, Callable
 
-import pandas as pd
-import polars as pl
+from pandas import DataFrame, Series
 
 from aligned.compiler.feature_factory import FeatureFactory, Transformation, TransformationFactory
-from aligned.schemas.transformation import LiteralValue, TextVectoriserModel
-
-logger = logging.getLogger(__name__)
+from aligned.enricher import StatisticEricher, TimespanSelector
+from aligned.exceptions import InvalidStandardScalerArtefact
+from aligned.schemas.feature_view import CompiledFeatureView
+from aligned.schemas.transformation import StandardScalingTransformation
 
 
 @dataclass
 class EqualsFactory(TransformationFactory):
 
     left: FeatureFactory
     right: FeatureFactory | Any
@@ -21,49 +21,34 @@
     @property
     def using_features(self) -> list[FeatureFactory]:
         if isinstance(self.right, FeatureFactory):
             return [self.left, self.right]
         else:
             return [self.left]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Equals
 
         if isinstance(self.right, FeatureFactory):
             raise NotImplementedError()
         else:
-            return Equals(self.left.name, LiteralValue.from_value(self.right))
-
-
-@dataclass
-class NotNullFactory(TransformationFactory):
-
-    value: FeatureFactory
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return [self.value]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import NotNull
-
-        return NotNull(self.value.name)
+            return Equals(self.left.name, self.right)
 
 
 @dataclass
 class RatioFactory(TransformationFactory):
 
     numerator: FeatureFactory
     denumerator: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.numerator, self.denumerator]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Ratio
 
         return Ratio(self.numerator.name, self.denumerator.name)
 
 
 @dataclass
 class OrdinalFactory(TransformationFactory):
@@ -71,15 +56,15 @@
     orders: list[str]
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Ordinal
 
         return Ordinal(self.feature.name, self.orders)
 
 
 @dataclass
 class ContainsFactory(TransformationFactory):
@@ -87,15 +72,15 @@
     text: str
     in_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.in_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Contains as ContainsTransformation
 
         return ContainsTransformation(self.in_feature.name, self.text)
 
 
 @dataclass
 class NotEqualsFactory(TransformationFactory):
@@ -103,18 +88,18 @@
     value: Any
     in_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.in_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import NotEquals as NotEqualsTransformation
 
-        return NotEqualsTransformation(self.in_feature.name, LiteralValue.from_value(self.value))
+        return NotEqualsTransformation(self.in_feature.name, self.value)
 
 
 @dataclass
 class GreaterThenFactory(TransformationFactory):
 
     left_feature: FeatureFactory
     right: Any
@@ -122,15 +107,15 @@
     @property
     def using_features(self) -> list[FeatureFactory]:
         if isinstance(self.right, FeatureFactory):
             return [self.left_feature, self.right]
         else:
             return [self.left_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import GreaterThen, GreaterThenValue
 
         if isinstance(self.right, FeatureFactory):
             return GreaterThen(self.left_feature.name, self.right.name)
         else:
             return GreaterThenValue(self.left_feature.name, self.right)
 
@@ -141,15 +126,15 @@
     value: Any
     in_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.in_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import GreaterThenOrEqual as GTETransformation
 
         return GTETransformation(self.in_feature.name, self.value)
 
 
 @dataclass
 class LowerThenFactory(TransformationFactory):
@@ -157,15 +142,15 @@
     value: float
     in_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.in_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import LowerThen as LTTransformation
 
         return LTTransformation(self.in_feature.name, self.value)
 
 
 @dataclass
 class LowerThenOrEqualFactory(TransformationFactory):
@@ -173,30 +158,30 @@
     value: float
     in_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.in_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import LowerThenOrEqual as LTETransformation
 
         return LTETransformation(self.in_feature.name, self.value)
 
 
 # @dataclass
 # class Split(TransformationFactory):
 
 #     pattern: str
 #     from_feature: FeatureFactory
 #     max_splits: int | None
 
 #     @property
-#     def method(self) -> Callable[[pd.DataFrame], pd.Series]:
-#         async def met(df: pd.DataFrame) -> pd.Series:
+#     def method(self) -> Callable[[DataFrame], Series]:
+#         async def met(df: DataFrame) -> Series:
 #             return df[self.from_feature.name].str.split(pat=self.pattern, n=self.max_splits)
 
 #         return met
 
 #     def index(self, index: int) -> 'ArrayIndex':
 #         return ArrayIndex(index, self)
 
@@ -209,16 +194,16 @@
 #     def __init__(self, index: int, feature: FeatureFactory) -> None:
 #         self.using_features = [feature]
 #         self.feature = Bool()
 #         self.index = index
 #         self.from_feature = feature
 
 #     @property
-#     def method(self) -> Callable[[pd.DataFrame], pd.Series]:
-#         async def met(df: pd.DataFrame) -> pd.Series:
+#     def method(self) -> Callable[[DataFrame], Series]:
+#         async def met(df: DataFrame) -> Series:
 #             return df[self.from_feature.name].str[self.index]
 
 #         return met
 
 
 @dataclass
 class DateComponentFactory(TransformationFactory):
@@ -226,15 +211,15 @@
     component: str
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import DateComponent as DCTransformation
 
         return DCTransformation(self.feature.name, self.component)
 
 
 @dataclass
 class DifferanceBetweenFactory(TransformationFactory):
@@ -242,90 +227,62 @@
     first_feature: FeatureFactory
     second_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.first_feature, self.second_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Subtraction
 
         return Subtraction(self.first_feature.name, self.second_feature.name)
 
 
 @dataclass
 class AdditionBetweenFactory(TransformationFactory):
 
     first_feature: FeatureFactory
-    second_feature: FeatureFactory | Any
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        if isinstance(self.second_feature, FeatureFactory):
-            return [self.first_feature, self.second_feature]
-        else:
-            return [self.first_feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import Addition, AdditionValue
-
-        if isinstance(self.second_feature, FeatureFactory):
-            return Addition(self.first_feature.name, self.second_feature.name)
-        else:
-            return AdditionValue(self.first_feature.name, LiteralValue.from_value(self.second_feature))
-
-
-@dataclass
-class PowerFactory(TransformationFactory):
-
-    first: FeatureFactory
-    second: FeatureFactory | Any
+    second_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
-        if isinstance(self.second, FeatureFactory):
-            return [self.first, self.second]
-        return [self.first]
+        return [self.first_feature, self.second_feature]
 
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import Power, PowerFeature
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
+        from aligned.schemas.transformation import Addition
 
-        if isinstance(self.second, FeatureFactory):
-            return PowerFeature(self.first.name, self.second.name)
-        else:
-            value = LiteralValue.from_value(self.second)
-            return Power(self.first.name, value)
+        return Addition(self.first_feature.name, self.second_feature.name)
 
 
 @dataclass
 class TimeDifferanceFactory(TransformationFactory):
 
     first_feature: FeatureFactory
     second_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.first_feature, self.second_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import TimeDifference as TDTransformation
 
         return TDTransformation(self.first_feature.name, self.second_feature.name)
 
 
 @dataclass
 class LogTransformFactory(TransformationFactory):
 
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import LogarithmOnePluss
 
         return LogarithmOnePluss(self.feature.name)
 
 
 @dataclass
 class ReplaceFactory(TransformationFactory):
@@ -333,46 +290,106 @@
     values: dict[str, str]
     source_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.source_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import ReplaceStrings
 
         return ReplaceStrings(self.source_feature.name, self.values)
 
 
 @dataclass
 class ToNumericalFactory(TransformationFactory):
 
     from_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.from_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import ToNumerical as ToNumericalTransformation
 
         return ToNumericalTransformation(self.from_feature.name)
 
 
 @dataclass
+class StandardScalingFactory(TransformationFactory):
+
+    feature: FeatureFactory
+
+    limit: int | None = field(default=None)
+    timespan: timedelta | None = field(default=None)
+
+    @property
+    def using_features(self) -> list[FeatureFactory]:
+        return [self.feature]
+
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
+        from aligned.enricher import StatisticEricher
+
+        if self.feature.transformation:
+            raise ValueError('Standard scaling is not supported for derived features yet')
+
+        if len(source_views) != 1:
+            raise ValueError('Expected one source')
+
+        feature_view = source_views[0]
+
+        if not isinstance(feature_view.batch_data_source, StatisticEricher):
+            raise ValueError('The data source needs to conform to StatisticEricher')
+
+        timespan: TimespanSelector | None = None
+
+        feature_name = self.feature.name
+
+        if self.timespan:
+            if not feature_view.event_timestamp:
+                raise InvalidStandardScalerArtefact(
+                    'Unable to find a event_timestamp, this is needed'
+                    ' when using `timespan` for artefact generation.\n',
+                    'Make sure the event_timestamp is above the'
+                    ' transformation in the feature view decleration',
+                )
+            timespan = TimespanSelector(self.timespan, time_column=feature_view.event_timestamp.name)
+
+        std_enricher = feature_view.batch_data_source.std(
+            columns={feature_name}, time=timespan, limit=self.limit
+        )
+        mean_enricher = feature_view.batch_data_source.mean(
+            columns={feature_name}, time=timespan, limit=self.limit
+        )
+
+        std, mean = await asyncio.gather(std_enricher.as_df(), mean_enricher.as_df())
+
+        if std.isna().any() or (std == 0).any():
+            raise InvalidStandardScalerArtefact(
+                f'The standard deviation for {feature_name} is 0.'
+                'Therefore convaying no meaningful information.\n'
+                'This could be because the used dataset has no values,'
+                'so maybe consider changing `limit`,`timspan` or change the datasource'
+            )
+
+        return StandardScalingTransformation(mean[feature_name], std[feature_name], feature_name)
+
+
+@dataclass
 class IsInFactory(TransformationFactory):
 
     feature: FeatureFactory
     values: list
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import IsIn as IsInTransformation
 
         return IsInTransformation(self.values, self.feature.name)
 
 
 @dataclass
 class AndFactory(TransformationFactory):
@@ -380,15 +397,15 @@
     first_feature: FeatureFactory
     second_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.first_feature, self.second_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import And as AndTransformation
 
         return AndTransformation(self.first_feature.name, self.second_feature.name)
 
 
 @dataclass
 class OrFactory(TransformationFactory):
@@ -396,196 +413,163 @@
     first_feature: FeatureFactory
     second_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.first_feature, self.second_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Or as OrTransformation
 
         return OrTransformation(self.first_feature.name, self.second_feature.name)
 
 
 @dataclass
 class InverseFactory(TransformationFactory):
 
     from_feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.from_feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Inverse as InverseTransformation
 
         return InverseTransformation(self.from_feature.name)
 
 
 class FillNaStrategy:
-    def compile(self) -> Any:
+    async def compile(self, feature: FeatureFactory, source_views: list[CompiledFeatureView]) -> Any:
         pass
 
+    @staticmethod
+    def mean(limit: int | None = None) -> 'FillNaStrategy':
+        return MeanFillNaStrategy(limit)
+
 
 @dataclass
 class ConstantFillNaStrategy(FillNaStrategy):
     value: Any
 
-    def compile(self) -> Any:
+    async def compile(self, feature: FeatureFactory, source_views: list[CompiledFeatureView]) -> Any:
         return self.value
 
 
 @dataclass
+class MeanFillNaStrategy(FillNaStrategy):
+
+    limit: int | None = field(default=None)
+
+    async def compile(self, feature: FeatureFactory, source_views: list[CompiledFeatureView]) -> Any:
+        if len(source_views) != 1:
+            raise ValueError('Need exactly one source in order to compute mean fill value')
+
+        source = source_views[0]
+        if not isinstance(source.batch_data_source, StatisticEricher):
+            raise ValueError('The data source needs to be a StatisticEnricher')
+
+        mean = await source.batch_data_source.mean(columns={feature.name}, limit=self.limit).as_df()
+        return mean[feature.name]
+
+
+@dataclass
 class FillMissingFactory(TransformationFactory):
 
     feature: FeatureFactory
     strategy: FillNaStrategy
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import FillNaValues
 
-        fill_value = self.strategy.compile()
-
-        return FillNaValues(
-            key=self.feature.name, value=LiteralValue.from_value(fill_value), dtype=self.feature.dtype
-        )
+        fill_value = await self.strategy.compile(self.feature, source_views)
+        return FillNaValues(key=self.feature.name, value=fill_value, dtype=self.feature.dtype)
 
 
 @dataclass
 class FloorFactory(TransformationFactory):
 
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Floor
 
         return Floor(self.feature.name)
 
 
 @dataclass
 class CeilFactory(TransformationFactory):
 
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Ceil
 
         return Ceil(self.feature.name)
 
 
 @dataclass
 class RoundFactory(TransformationFactory):
 
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Round
 
         return Round(self.feature.name)
 
 
 @dataclass
 class AbsoluteFactory(TransformationFactory):
 
     feature: FeatureFactory
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Absolute
 
         return Absolute(self.feature.name)
 
 
 @dataclass
-class PandasTransformationFactory(TransformationFactory):
+class DillTransformationFactory(TransformationFactory):
 
     dtype: FeatureFactory
-    method: Callable[[pd.DataFrame], pd.Series]
+    method: Callable[[DataFrame], Series]
     _using_features: list[FeatureFactory]
 
     @property
     def using_features(self) -> list[FeatureFactory]:
         return self._using_features
 
-    def compile(self) -> Transformation:
-        import inspect
-        import types
-
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         import dill
 
-        from aligned.schemas.transformation import PandasFunctionTransformation, PandasLambdaTransformation
+        from aligned.schemas.transformation import DillTransformation
 
-        if isinstance(self.method, types.LambdaType) and self.method.__name__ == '<lambda>':
-            return PandasLambdaTransformation(
-                method=dill.dumps(self.method),
-                code=inspect.getsource(self.method).strip(),
-                dtype=self.dtype.dtype,
-            )
-        else:
-            return PandasFunctionTransformation(
-                code=inspect.getsource(self.method),
-                function_name=dill.source.getname(self.method),
-                dtype=self.dtype.dtype,
-            )
-
-
-@dataclass
-class PolarsTransformationFactory(TransformationFactory):
-
-    dtype: FeatureFactory
-    method: pl.Expr | Callable[[pl.LazyFrame, pl.Expr], pl.LazyFrame]
-    _using_features: list[FeatureFactory]
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return self._using_features
-
-    def compile(self) -> Transformation:
-        import inspect
-        import types
-
-        import dill
-
-        from aligned.schemas.transformation import PolarsFunctionTransformation, PolarsLambdaTransformation
-
-        if isinstance(self.method, pl.Expr):
-            code = str(self.method)
-            self.method = lambda df, alias: df.with_column(self.method.alias(alias))
-        else:
-            code = inspect.getsource(self.method)
-
-        if isinstance(self.method, types.LambdaType) and self.method.__name__ == '<lambda>':
-            return PolarsLambdaTransformation(
-                method=dill.dumps(self.method), code=code.strip(), dtype=self.dtype.dtype
-            )
-        else:
-            return PolarsFunctionTransformation(
-                code=code,
-                function_name=dill.source.getname(self.method),
-                dtype=self.dtype.dtype,
-            )
+        return DillTransformation(method=dill.dumps(self.method, recurse=True), dtype=self.dtype.dtype)
 
 
 class AggregatableTransformation:
 
     group_by: list[FeatureFactory] | None = field(default=None)
 
     def copy(self) -> 'AggregatableTransformation':
@@ -602,106 +586,19 @@
     @property
     def using_features(self) -> list[FeatureFactory]:
         if self.group_by:
             return [self.feature] + self.group_by
         else:
             return [self.feature]
 
-    def compile(self) -> Transformation:
+    async def compile(self, source_views: list[CompiledFeatureView]) -> Transformation:
         from aligned.schemas.transformation import Mean
 
+        if len(source_views) != 1:
+            raise ValueError('Unable to compute mean for CombinedView')
+
         return Mean(
             key=self.feature.name, group_keys=[feat.name for feat in self.group_by] if self.group_by else None
         )
 
     def copy(self) -> 'MeanTransfomrationFactory':
         return MeanTransfomrationFactory(self.feature, self.over, self.group_by)
-
-
-@dataclass
-class WordVectoriserFactory(TransformationFactory):
-
-    feature: FeatureFactory
-    model: TextVectoriserModel
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return [self.feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import WordVectoriser
-
-        return WordVectoriser(self.feature.name, self.model)
-
-
-@dataclass
-class LoadImageFactory(TransformationFactory):
-
-    url_feature: FeatureFactory
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return [self.url_feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import LoadImageUrl
-
-        return LoadImageUrl(self.url_feature.name)
-
-
-@dataclass
-class GrayscaleImageFactory(TransformationFactory):
-
-    image_feature: FeatureFactory
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return [self.image_feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import GrayscaleImage
-
-        return GrayscaleImage(self.image_feature.name)
-
-
-@dataclass
-class AppendStrings(TransformationFactory):
-
-    first_feature: FeatureFactory
-    second_feature: FeatureFactory | LiteralValue
-    separator: str = field(default='')
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        if isinstance(self.second_feature, LiteralValue):
-            return [self.first_feature]
-        else:
-            return [self.first_feature, self.second_feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import AppendConstString, AppendStrings
-
-        if isinstance(self.second_feature, LiteralValue):
-            return AppendConstString(self.first_feature.name, self.second_feature.value)
-        else:
-            return AppendStrings(self.first_feature.name, self.second_feature.name, self.separator)
-
-
-@dataclass
-class ClipFactory(TransformationFactory):
-
-    feature: FeatureFactory
-    lower_bound: int | float
-    upper_bound: int | float
-
-    @property
-    def using_features(self) -> list[FeatureFactory]:
-        return [self.feature]
-
-    def compile(self) -> Transformation:
-        from aligned.schemas.transformation import Clip
-
-        return Clip(
-            self.feature.name,
-            LiteralValue.from_value(self.lower_bound),
-            LiteralValue.from_value(self.upper_bound),
-        )
```

### Comparing `aligned-0.0.9/aligned/data_file.py` & `aligned-0.0.9a0/aligned/data_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,24 @@
     It can therefore be loaded in and writen to.
     Either as a pandas data frame, or a dask data frame.
     """
 
     async def read_pandas(self) -> pd.DataFrame:
         raise NotImplementedError()
 
-    async def to_pandas(self) -> pd.DataFrame:
+    async def read_dask(self) -> pd.DataFrame:
+        raise NotImplementedError()
+
+    async def to_df(self) -> pd.DataFrame:
         await self.read_pandas()
 
+    async def to_dask(self) -> pd.DataFrame:
+        await self.read_dask()
+
     async def to_polars(self) -> pl.LazyFrame:
         raise NotImplementedError()
 
-    async def write_polars(self, df: pl.LazyFrame) -> None:
+    async def write_pandas(self, df: pd.DataFrame) -> None:
         raise NotImplementedError()
 
-    async def write_pandas(self, df: pd.DataFrame) -> None:
+    async def write_dask(self, df: pd.DataFrame) -> None:
         raise NotImplementedError()
```

### Comparing `aligned-0.0.9/aligned/data_source/batch_data_source.py` & `aligned-0.0.9a0/aligned/data_source/batch_data_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from __future__ import annotations
-
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import TYPE_CHECKING, TypeVar
+from typing import Optional, TypeVar
 
 from mashumaro.types import SerializableType
 
+from aligned.request.retrival_request import RetrivalRequest
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalJob
 from aligned.schemas.codable import Codable
 from aligned.schemas.feature import Feature
 
-if TYPE_CHECKING:
-    from aligned.request.retrival_request import RetrivalRequest
-    from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalJob
-
 
 class BatchDataSourceFactory:
 
-    supported_data_sources: dict[str, type[BatchDataSource]]
+    supported_data_sources: dict[str, type['BatchDataSource']]
 
-    _shared: BatchDataSourceFactory | None = None
+    _shared: Optional['BatchDataSourceFactory'] = None
 
     def __init__(self) -> None:
-        from aligned.local.source import CsvFileSource, ParquetFileSource
+        from aligned.local.source import CsvFileSource
         from aligned.psql.data_source import PostgreSQLDataSource
         from aligned.redshift.data_source import RedshiftSQLDataSource
         from aligned.s3.config import AwsS3CsvDataSource, AwsS3ParquetDataSource
 
         self.supported_data_sources = {
             PostgreSQLDataSource.type_name: PostgreSQLDataSource,
-            ParquetFileSource.type_name: ParquetFileSource,
             CsvFileSource.type_name: CsvFileSource,
             AwsS3CsvDataSource.type_name: AwsS3CsvDataSource,
             AwsS3ParquetDataSource.type_name: AwsS3ParquetDataSource,
             RedshiftSQLDataSource.type_name: RedshiftSQLDataSource,
         }
 
     @classmethod
-    def shared(cls) -> BatchDataSourceFactory:
+    def shared(cls) -> 'BatchDataSourceFactory':
         if cls._shared:
             return cls._shared
         cls._shared = BatchDataSourceFactory()
         return cls._shared
 
 
 T = TypeVar('T')
@@ -57,24 +52,21 @@
     type_name: str
 
     @abstractmethod
     def job_group_key(self) -> str:
         pass
 
     def _serialize(self) -> dict:
-        assert (
-            self.type_name in BatchDataSourceFactory.shared().supported_data_sources
-        ), f'Unknown type_name: {self.type_name}'
         return self.to_dict()
 
     def __hash__(self) -> int:
         return hash(self.job_group_key())
 
     @classmethod
-    def _deserialize(cls, value: dict) -> BatchDataSource:
+    def _deserialize(cls, value: dict) -> 'BatchDataSource':
         name_type = value['type_name']
         if name_type not in BatchDataSourceFactory.shared().supported_data_sources:
             raise ValueError(
                 f"Unknown batch data source id: '{name_type}'.\nRemember to add the"
                 ' data source to the BatchDataSourceFactory.supported_data_sources if'
                 ' it is a custom type.'
             )
@@ -90,22 +82,17 @@
         request: RetrivalRequest,
         start_date: datetime,
         end_date: datetime,
     ) -> DateRangeJob:
         raise NotImplementedError()
 
     @classmethod
-    def multi_source_features_for(
-        cls: type[T], facts: RetrivalJob, requests: list[tuple[T, RetrivalRequest]]
-    ) -> RetrivalJob:
+    def feature_for(cls: type[T], facts: dict[str, list], requests: dict[T, RetrivalRequest]) -> RetrivalJob:
         raise NotImplementedError()
 
-    def features_for(self, facts: RetrivalJob, request: RetrivalRequest) -> RetrivalJob:
-        return type(self).multi_source_features_for(facts, [(self, request)])
-
 
 class ColumnFeatureMappable:
     mapping_keys: dict[str, str]
 
     def columns_for(self, features: list[Feature]) -> list[str]:
         return [self.mapping_keys.get(feature.name, feature.name) for feature in features]
```

### Comparing `aligned-0.0.9/aligned/data_source/stream_data_source.py` & `aligned-0.0.9a0/aligned/data_source/stream_data_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-from __future__ import annotations
-
 from abc import ABC
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import Optional
 
 from mashumaro.types import SerializableType
 
 from aligned.schemas.codable import Codable
 
-if TYPE_CHECKING:
-    from aligned.retrival_job import RetrivalJob
-
 
 class StreamDataSourceFactory:
 
-    supported_data_sources: dict[str, type[StreamDataSource]]
+    supported_data_sources: dict[str, type['StreamDataSource']]
 
-    _shared: StreamDataSourceFactory | None = None
+    _shared: Optional['StreamDataSourceFactory'] = None
 
     def __init__(self) -> None:
         from aligned.redis.config import RedisStreamSource
 
         self.supported_data_sources = {
             HttpStreamSource.name: HttpStreamSource,
             RedisStreamSource.name: RedisStreamSource,
         }
 
     @classmethod
-    def shared(cls) -> StreamDataSourceFactory:
+    def shared(cls) -> 'StreamDataSourceFactory':
         if cls._shared:
             return cls._shared
         cls._shared = StreamDataSourceFactory()
         return cls._shared
 
 
 class StreamDataSource(ABC, Codable, SerializableType):
@@ -39,19 +34,18 @@
     Used to determend if an API call should be created, or if we should listen to a stream.
     """
 
     name: str
     topic_name: str
 
     def _serialize(self) -> dict:
-        assert self.name in StreamDataSourceFactory.shared().supported_data_sources
         return self.to_dict()
 
     @classmethod
-    def _deserialize(cls, value: dict) -> StreamDataSource:
+    def _deserialize(cls, value: dict) -> 'StreamDataSource':
         name = value['name']
         if name not in StreamDataSourceFactory.shared().supported_data_sources:
             raise ValueError(
                 f"Unknown stream data source id: '{name}'.\nRemember to add the"
                 ' data source to the StreamDataSourceFactory.supported_data_sources if'
                 ' it is a custom type.'
             )
@@ -64,14 +58,9 @@
 class HttpStreamSource(StreamDataSource):
 
     topic_name: str
     mappings: dict[str, str] = field(default_factory=dict)
 
     name: str = 'http'
 
-    def map_values(self, mappings: dict[str, str]) -> HttpStreamSource:
+    def map_values(self, mappings: dict[str, str]) -> 'HttpStreamSource':
         return HttpStreamSource(topic_name=self.topic_name, mappings=self.mappings | mappings)
-
-
-class SinkableDataSource:
-    async def write_to_stream(self, job: RetrivalJob) -> None:
-        pass
```

### Comparing `aligned-0.0.9/aligned/enricher.py` & `aligned-0.0.9a0/aligned/enricher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
+from contextlib import suppress
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import pandas as pd
 from mashumaro.types import SerializableType
 
 from aligned.redis.config import RedisConfig
 from aligned.schemas.codable import Codable
 
+with suppress(ModuleNotFoundError):
+    import dask.dataframe as dd
+
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TimespanSelector(Codable):
     timespand: timedelta
     time_column: str
@@ -53,14 +57,18 @@
     def cache(self, ttl: timedelta, cache_key: str) -> Enricher:
         return FileCacheEnricher(ttl, cache_key, self)
 
     @abstractmethod
     async def as_df(self) -> pd.DataFrame:
         pass
 
+    @abstractmethod
+    async def as_dask(self) -> dd.DataFrame:
+        pass
+
 
 class SupportedEnrichers:
 
     types: dict[str, type[Enricher]]
 
     _shared: SupportedEnrichers | None = None
 
@@ -98,14 +106,19 @@
         self.timeout = timeout
 
     async def as_df(self) -> pd.DataFrame:
         redis = self.config.redis()
         async with redis.lock(self.lock_name, timeout=self.timeout) as _:
             return await self.enricher.as_df()
 
+    async def as_dask(self) -> dd.DataFrame:
+        redis = self.config.redis()
+        async with redis.lock(self.lock_name, timeout=self.timeout) as _:
+            return await self.enricher.as_dask()
+
 
 @dataclass
 class CsvFileSelectedEnricher(Enricher):
     file: str
     time: TimespanSelector | None = field(default=None)
     limit: int | None = field(default=None)
     name: str = 'selective_file'
@@ -128,14 +141,17 @@
         if not self.time:
             return file
 
         date = datetime.now() - self.time.timespand
         selector = file[self.time.time_column] >= date
         return file.loc[selector]
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class CsvFileEnricher(Enricher):
 
     file: str
     name: str = 'file'
 
@@ -143,14 +159,17 @@
         self, time: TimespanSelector | None = None, limit: int | None = None
     ) -> CsvFileSelectedEnricher:
         return CsvFileSelectedEnricher(self.file, time=time, limit=limit)
 
     async def as_df(self) -> pd.DataFrame:
         return pd.read_csv(self.file)
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class LoadedStatEnricher(Enricher):
 
     stat: str
     columns: list[str]
     enricher: Enricher
@@ -162,14 +181,24 @@
         if self.stat == 'mean':
             return renamed[self.columns].mean()
         elif self.stat == 'std':
             return renamed[self.columns].std()
         else:
             raise ValueError(f'Not supporting stat: {self.stat}')
 
+    async def as_dask(self) -> dd.DataFrame:
+        data = await self.enricher.as_dask()
+        renamed = data.rename(columns=self.mapping_keys)
+        if self.stat == 'mean':
+            return renamed[self.columns].mean()
+        elif self.stat == 'std':
+            return renamed[self.columns].std()
+        else:
+            raise ValueError(f'Not supporting stat: {self.stat}')
+
 
 @dataclass
 class FileCacheEnricher(Enricher):
 
     ttl: timedelta
     file_path: str
     enricher: Enricher
@@ -195,14 +224,28 @@
             logger.info(f'Storing cache at file {file_uri.as_uri()}')
             data.to_parquet(file_uri)
         else:
             logger.info('Loading cache')
             data = pd.read_parquet(file_uri)
         return data
 
+    async def as_dask(self) -> dd.DataFrame:
+        file_uri = Path(self.file_path).absolute()
+
+        if self.is_out_of_date_cache():
+            logger.info('Fetching from source')
+            data: dd.DataFrame = await self.enricher.as_dask()
+            file_uri.parent.mkdir(exist_ok=True, parents=True)
+            logger.info(f'Storing cache at file {file_uri.as_uri()}')
+            data.to_parquet(file_uri)
+        else:
+            logger.info('Loading cache')
+            data = dd.read_parquet(file_uri)
+        return data
+
 
 @dataclass
 class SqlDatabaseEnricher(Enricher):
 
     query: str
     values: dict | None
     url_env: str
@@ -212,16 +255,20 @@
         self.query = query
         self.values = values
         self.url_env = url_env
 
     async def as_df(self) -> pd.DataFrame:
         import os
 
-        import connectorx as cx
-
-        df = cx.read_sql(os.environ[self.url_env], self.query, return_type='pandas')
+        from databases import Database
 
+        async with Database(os.environ[self.url_env]) as db:
+            records = await db.fetch_all(self.query, values=self.values)
+        df = pd.DataFrame.from_records([dict(record) for record in records])
         for name, dtype in df.dtypes.iteritems():
             if dtype == 'object':  # Need to convert the databases UUID type
                 df[name] = df[name].astype('str')
-
         return df
+
+    async def as_dask(self) -> dd.DataFrame:
+        pdf = await self.as_df()
+        return dd.from_pandas(pdf)
```

### Comparing `aligned-0.0.9/aligned/feature_source.py` & `aligned-0.0.9a0/aligned/feature_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 import polars as pl
 
 from aligned.data_source.batch_data_source import BatchDataSource
 from aligned.request.retrival_request import FeatureRequest, RequestResult, RetrivalRequest
-from aligned.retrival_job import RetrivalJob
+from aligned.retrival_job import FactualRetrivalJob
+
+if TYPE_CHECKING:
+    from aligned.retrival_job import RetrivalJob
 
 
 class FeatureSource:
-    def features_for(self, facts: RetrivalJob, request: FeatureRequest) -> RetrivalJob:
+    def features_for(self, facts: dict[str, list], request: FeatureRequest) -> RetrivalJob:
         raise NotImplementedError()
 
 
 class WritableFeatureSource:
     async def write(self, job: RetrivalJob, requests: list[RetrivalRequest]) -> None:
         raise NotImplementedError()
 
@@ -41,86 +44,89 @@
 
     sources: dict[str, BatchDataSource]
 
     @property
     def source_types(self) -> dict[str, type[BatchDataSource]]:
         return {source.job_group_key(): type(source) for source in self.sources.values()}
 
-    def features_for(self, facts: RetrivalJob, request: FeatureRequest) -> RetrivalJob:
+    def features_for(self, facts: dict[str, list], request: FeatureRequest) -> RetrivalJob:
         from aligned.retrival_job import CombineFactualJob
 
-        core_requests = [
-            (self.sources[request.location.identifier], request)
+        core_requests = {
+            self.sources[request.feature_view_name]: request
             for request in request.needed_requests
-            if request.location.identifier in self.sources
-        ]
+            if request.feature_view_name in self.sources
+        }
         source_groupes = {
-            self.sources[request.location.identifier].job_group_key()
+            self.sources[request.feature_view_name].job_group_key()
             for request in request.needed_requests
-            if request.location.identifier in self.sources
+            if request.feature_view_name in self.sources
         }
-
         # The combined views basicly, as they have no direct
         combined_requests = [
-            request for request in request.needed_requests if request.location.identifier not in self.sources
+            request for request in request.needed_requests if request.feature_view_name not in self.sources
         ]
         jobs = [
-            self.source_types[source_group].multi_source_features_for(
+            self.source_types[source_group]
+            .feature_for(
                 facts=facts,
+                requests={
+                    source: req
+                    for source, req in core_requests.items()
+                    if source.job_group_key() == source_group
+                },
+            )
+            .derive_features(
                 requests=[
-                    (source, req) for source, req in core_requests if source.job_group_key() == source_group
-                ],
+                    req for source, req in core_requests.items() if source.job_group_key() == source_group
+                ]
             )
             for source_group in source_groupes
         ]
-        return (
-            CombineFactualJob(
-                jobs=jobs,
-                combined_requests=combined_requests,
-            )
-            .ensure_types(request.needed_requests)
-            .derive_features(request.needed_requests)
-        )
+        return CombineFactualJob(
+            jobs=jobs,
+            combined_requests=combined_requests,
+        ).ensure_types(request.needed_requests)
 
     def all_for(self, request: FeatureRequest, limit: int | None = None) -> RetrivalJob:
         if len(request.needed_requests) != 1:
             raise ValueError("Can't use all_for with a request that has subrequests")
-        if request.location.identifier not in self.sources:
+        if request.name not in self.sources:
             raise ValueError(
                 (
-                    f"Unable to find feature view named '{request.location.identifier}'.",
+                    f"Unable to find feature view named '{request.name}'.",
                     'Make sure it is added to the featuer store',
                 )
             )
         return (
-            self.sources[request.location.identifier]
+            self.sources[request.name]
             .all_data(request.needed_requests[0], limit)
-            .ensure_types(request.needed_requests)
             .derive_features(request.needed_requests)
+            .ensure_types(request.needed_requests)
         )
 
     def all_between(self, start_date: datetime, end_date: datetime, request: FeatureRequest) -> RetrivalJob:
         if len(request.needed_requests) != 1:
             raise ValueError("Can't use all_for with a request that has subrequests")
-        if request.location.identifier not in self.sources:
+        if request.name not in self.sources:
             raise ValueError(
                 (
-                    f"Unable to find feature view named '{request.location.identifier}'.",
+                    f"Unable to find feature view named '{request.name}'.",
                     'Make sure it is added to the featuer store',
                 )
             )
         return (
-            self.sources[request.location.identifier]
+            self.sources[request.name]
             .all_between_dates(request.needed_requests[0], start_date, end_date)
-            .ensure_types(request.needed_requests)
             .derive_features(requests=request.needed_requests)
+            .ensure_types(request.needed_requests)
         )
 
 
-class FactualInMemoryJob(RetrivalJob):
+class FactualInMemoryJob(FactualRetrivalJob):
     """
     A job using a in mem storage, aka a dict.
 
     This will store the features in the following format:
 
     values = {
         "feature_view:entity-id:feature-name": value,
@@ -132,36 +138,38 @@
         "titanic_passenger:20:class": "Eco",
         "titanic_passenger:21:class": "VIP",
     }
     """
 
     values: dict[str, Any]
     requests: list[RetrivalRequest]
-    facts: RetrivalJob
+    facts: dict[str, list]
 
     @property
     def request_result(self) -> RequestResult:
         return RequestResult.from_request_list(self.requests)
 
-    def __init__(self, values: dict[str, Any], requests: list[RetrivalRequest], facts: RetrivalJob) -> None:
+    def __init__(
+        self, values: dict[str, Any], requests: list[RetrivalRequest], facts: dict[str, list]
+    ) -> None:
         self.values = values
         self.requests = requests
         self.facts = facts
 
     def key(self, request: RetrivalRequest, entity: str, feature_name: str) -> str:
-        return f'{request.location}:{entity}:{feature_name}'
+        return f'{request.feature_view_name}:{entity}:{feature_name}'
 
     async def to_pandas(self) -> pd.DataFrame:
 
         columns = set()
         for request in self.requests:
             for feature in request.all_feature_names:
                 columns.add(feature)
 
-        result_df = await self.facts.to_pandas()
+        result_df = pd.DataFrame(self.facts)
 
         for request in self.requests:
             entity_ids = result_df[list(request.entity_names)]
             entities = entity_ids.sum(axis=1)
 
             for feature in request.all_feature_names:
                 # if feature.name in request.entity_names:
@@ -178,19 +186,19 @@
 
 
 @dataclass
 class InMemoryFeatureSource(FeatureSource, WritableFeatureSource):
 
     values: dict[str, Any]
 
-    def features_for(self, facts: RetrivalJob, request: FeatureRequest) -> RetrivalJob:
+    def features_for(self, facts: dict[str, list], request: FeatureRequest) -> RetrivalJob:
         return FactualInMemoryJob(self.values, request.needed_requests, facts)
 
     def key(self, request: RetrivalRequest, entity: str, feature_name: str) -> str:
-        return f'{request.location}:{entity}:{feature_name}'
+        return f'{request.feature_view_name}:{entity}:{feature_name}'
 
     async def write(self, job: RetrivalJob, requests: list[RetrivalRequest]) -> None:
         data = await job.to_pandas()
 
         for _, row in data.iterrows():
             # Run one query per row
             for request in requests:
```

### Comparing `aligned-0.0.9/aligned/feature_store.py` & `aligned-0.0.9a0/aligned/feature_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,93 @@
 import logging
 from collections import defaultdict
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from importlib import import_module
 from typing import Any
 
-from aligned.compiler.model import Model
 from aligned.data_file import DataFileReference
 from aligned.enricher import Enricher
 from aligned.exceptions import CombinedFeatureViewQuerying
 from aligned.feature_source import (
     BatchFeatureSource,
     FeatureSource,
     RangeFeatureSource,
     WritableFeatureSource,
 )
 from aligned.feature_view.combined_view import CombinedFeatureView, CompiledCombinedFeatureView
 from aligned.feature_view.feature_view import FeatureView
-from aligned.online_source import BatchOnlineSource, OnlineSource
+from aligned.model import Model
+from aligned.online_source import BatchOnlineSource
 from aligned.request.retrival_request import FeatureRequest, RetrivalRequest
-from aligned.retrival_job import FilterJob, RetrivalJob, StreamAggregationJob, SupervisedJob
-from aligned.schemas.feature import FeatureLocation
+from aligned.retrival_job import DerivedFeatureJob, FilterJob, RetrivalJob
 from aligned.schemas.feature_view import CompiledFeatureView
-from aligned.schemas.model import EventTrigger
 from aligned.schemas.model import Model as ModelSchema
-from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoMetadata
+from aligned.schemas.repo_definition import EnricherReference, RepoDefinition
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class RawStringFeatureRequest:
     features: set[str]
 
     @property
-    def locations(self) -> set[FeatureLocation]:
+    def feature_view_names(self) -> set[str]:
         return {RawStringFeatureRequest.unpack_feature(feature)[0] for feature in self.features}
 
     @property
-    def grouped_features(self) -> dict[FeatureLocation, set[str]]:
+    def grouped_features(self) -> dict[str, set[str]]:
         unpacked_features = [RawStringFeatureRequest.unpack_feature(feature) for feature in self.features]
         grouped = defaultdict(set)
         for feature_view, feature in unpacked_features:
             grouped[feature_view].add(feature)
         return grouped
 
     @property
     def feature_names(self) -> set[str]:
         return {RawStringFeatureRequest.unpack_feature(feature)[1] for feature in self.features}
 
     @staticmethod
-    def unpack_feature(feature: str) -> tuple[FeatureLocation, str]:
+    def unpack_feature(feature: str) -> tuple[str, str]:
         splits = feature.split(':')
-        if len(splits) == 3:
-            return (FeatureLocation(splits[1], splits[0]), splits[2])
-        if len(splits) == 2:
-            return (FeatureLocation(splits[0], 'feature_view'), splits[1])
-        else:
-            raise ValueError(f'Unable to decode {splits}')
+        if len(splits) != 2:
+            raise ValueError(f'Invalid feature name: {feature}')
+        return (splits[0], splits[1])
 
 
 class FeatureStore:
 
     feature_source: FeatureSource
     feature_views: dict[str, CompiledFeatureView]
     combined_feature_views: dict[str, CompiledCombinedFeatureView]
     models: dict[str, ModelSchema]
     event_timestamp_column = 'event_timestamp'
 
     @property
     def all_models(self) -> list[str]:
-        return list(self.models.keys())
+        return list(self.model_requests.keys())
 
     def __init__(
         self,
         feature_views: dict[str, CompiledFeatureView],
         combined_feature_views: dict[str, CompiledCombinedFeatureView],
         models: dict[str, ModelSchema],
         feature_source: FeatureSource,
     ) -> None:
         self.feature_source = feature_source
         self.combined_feature_views = combined_feature_views
         self.feature_views = feature_views
-        self.models = models
+        self.model_requests = models
 
     @staticmethod
     def experimental() -> 'FeatureStore':
         from aligned.online_source import BatchOnlineSource
 
-        return FeatureStore.from_definition(
-            RepoDefinition(
-                metadata=RepoMetadata(created_at=datetime.utcnow(), name='experimental'),
-                online_source=BatchOnlineSource(),
-            )
-        )
+        return FeatureStore.from_definition(RepoDefinition(online_source=BatchOnlineSource()))
 
     @staticmethod
     def register_enrichers(enrichers: list[EnricherReference]) -> None:
         from types import ModuleType
 
         class DynamicEnricher(ModuleType):
             def __init__(self, values: dict[str, Enricher]) -> None:
@@ -158,24 +148,14 @@
         return FeatureStore(
             feature_views=feature_views,
             combined_feature_views=combined_feature_views,
             models={model.name: model for model in repo.models},
             feature_source=source,
         )
 
-    def repo_definition(self) -> RepoDefinition:
-        return RepoDefinition(
-            metadata=RepoMetadata(datetime.utcnow(), 'feature_store_location.py'),
-            feature_views=set(self.feature_views.values()),
-            combined_feature_views=set(self.combined_feature_views.values()),
-            models=set(self.models.values()),
-            online_source=BatchOnlineSource(),
-            enrichers=[],
-        )
-
     @staticmethod
     async def from_reference_at_path(
         path: str = '.', reference_file: str = 'feature_store_location.py'
     ) -> 'FeatureStore':
         """Looks for a file reference struct, and loads the associated repo.
 
         This can be used for changing which feature store definitions
@@ -209,305 +189,179 @@
 
         Returns:
             FeatureStore: The generated feature store
         """
         definition = await RepoDefinition.from_path(path)
         return FeatureStore.from_definition(definition)
 
-    def features_for_request(
-        self, requests: FeatureRequest, entities: dict[str, list] | RetrivalJob, feature_names: set[str]
-    ) -> RetrivalJob:
-        entity_request: RetrivalJob
-
-        if isinstance(entities, dict):
-            if requests.needs_event_timestamp and self.event_timestamp_column not in entities:
-                raise ValueError(f'Missing {self.event_timestamp_column} in entities')
-
-            entity_request = RetrivalJob.from_dict(entities, requests)
-        else:
-            entity_request = entities
-
-        return FilterJob(
-            feature_names,
-            self.feature_source.features_for(entity_request, requests),
-        )
-
-    def features_for(self, entities: dict[str, list] | RetrivalJob, features: list[str]) -> RetrivalJob:
+    def features_for(self, entities: dict[str, list], features: list[str]) -> RetrivalJob:
 
         feature_request = RawStringFeatureRequest(features=set(features))
+        entities_names: set[str] = set(entities.keys())
         requests = self.requests_for(feature_request)
-
         feature_names = set()
 
+        if requests.needs_event_timestamp and self.event_timestamp_column not in entities:
+            raise ValueError(f'Missing {self.event_timestamp_column} in entities')
+
         if requests.needs_event_timestamp:
             feature_names.add(self.event_timestamp_column)
 
         for view, feature_set in feature_request.grouped_features.items():
             if feature_set != {'*'}:
                 feature_names.update(feature_set)
             else:
                 for request in requests.needed_requests:
-                    if view.name == request.location.name:
+                    if request.feature_view_name == view:
                         feature_names.update(request.all_feature_names)
         for request in requests.needed_requests:
             feature_names.update(request.entity_names)
+            entities_names.update(request.entity_names)
 
-        return self.features_for_request(requests, entities, feature_names)
+        return FilterJob(
+            feature_names,
+            self.feature_source.features_for(entities, requests),
+        )
 
     def model(self, name: str) -> 'ModelFeatureStore':
-        model = self.models[name]
-        return ModelFeatureStore(model, self)
-
-    def event_triggers_for(self, feature_view: str) -> set[EventTrigger]:
-        triggers = self.feature_views[feature_view].event_triggers or set()
-        for model in self.models.values():
-            for target in model.predictions_view.classification_targets:
-                if target.event_trigger and target.estimating.location.location == feature_view:
-                    triggers.add(target.event_trigger)
-        return triggers
+        model = self.model_requests[name]
+        request = self.requests_for_model(model)
+        return ModelFeatureStore(self.feature_source, request)
+
+    def requests_for_model(self, model: ModelSchema) -> FeatureRequest:
+        feature_referances = {f'{feature.feature_view}:{feature.name}' for feature in model.features}.union(
+            {f'{feature.feature_view}:{feature.name}' for feature in model.targets or set()}
+        )
+        return FeatureStore._requests_for(
+            RawStringFeatureRequest(feature_referances), self.feature_views, self.combined_feature_views
+        )
 
     @staticmethod
     def _requests_for(
         feature_request: RawStringFeatureRequest,
         feature_views: dict[str, CompiledFeatureView],
         combined_feature_views: dict[str, CompiledCombinedFeatureView],
     ) -> FeatureRequest:
         features = feature_request.grouped_features
         requests: list[RetrivalRequest] = []
         entity_names = set()
         needs_event_timestamp = False
 
-        for location in feature_request.locations:
-            feature_view_name = location.name
+        for feature_view_name in feature_request.feature_view_names:
             if feature_view_name in combined_feature_views:
                 cfv = combined_feature_views[feature_view_name]
-                if len(features[location]) == 1 and list(features[location])[0] == '*':
+                if len(features[feature_view_name]) == 1 and list(features[feature_view_name])[0] == '*':
                     sub_requests = cfv.request_all
                 else:
-                    sub_requests = cfv.requests_for(features[location])
+                    sub_requests = cfv.requests_for(features[feature_view_name])
                 requests.extend(sub_requests.needed_requests)
                 for request in sub_requests.needed_requests:
                     entity_names.update(request.entity_names)
                     if request.event_timestamp:
                         needs_event_timestamp = True
 
-            elif feature_view_name in feature_views:
+            else:
                 feature_view = feature_views[feature_view_name]
-                if len(features[location]) == 1 and list(features[location])[0] == '*':
+                if len(features[feature_view_name]) == 1 and list(features[feature_view_name])[0] == '*':
                     sub_requests = feature_view.request_all
                 else:
-                    sub_requests = feature_view.request_for(features[location])
+                    sub_requests = feature_view.request_for(features[feature_view_name])
                 requests.extend(sub_requests.needed_requests)
                 for request in sub_requests.needed_requests:
                     entity_names.update(request.entity_names)
                     if request.event_timestamp:
                         needs_event_timestamp = True
-            else:
-                raise ValueError(
-                    f'Unable to find: {feature_view_name}, '
-                    f'availible views are: {combined_feature_views.keys()}, and: {feature_views.keys()}'
-                )
 
         if needs_event_timestamp:
             entity_names.add('event_timestamp')
 
         return FeatureRequest(
-            FeatureLocation.model('custom features'),
+            'some_name',
             feature_request.feature_names.union(entity_names),
             RetrivalRequest.combine(requests),
         )
 
     def requests_for(self, feature_request: RawStringFeatureRequest) -> FeatureRequest:
         return FeatureStore._requests_for(feature_request, self.feature_views, self.combined_feature_views)
 
     def feature_view(self, view: str) -> 'FeatureViewStore':
         if view in self.combined_feature_views:
             raise CombinedFeatureViewQuerying(
                 'You are trying to get a combined feature view. ',
                 'This is only possible through store.features_for(...), as of now.\n',
             )
-        feature_view = self.feature_views[view]
-        return FeatureViewStore(self, feature_view, self.event_triggers_for(view))
+        view = self.feature_views[view]
+        return FeatureViewStore(self.feature_source, view)
 
-    def add_feature_view(self, feature_view: FeatureView) -> None:
-        compiled_view = type(feature_view).compile()
+    async def add_feature_view(self, feature_view: FeatureView) -> None:
+        compiled_view = await type(feature_view).compile()
         self.feature_views[compiled_view.name] = compiled_view
         if isinstance(self.feature_source, BatchFeatureSource):
-            self.feature_source.sources[
-                FeatureLocation.feature_view(compiled_view.name).identifier
-            ] = compiled_view.batch_data_source
+            self.feature_source.sources[compiled_view.name] = compiled_view.batch_data_source
 
-    def add_combined_feature_view(self, feature_view: CombinedFeatureView) -> None:
-        compiled_view = type(feature_view).compile()
+    async def add_combined_feature_view(self, feature_view: CombinedFeatureView) -> None:
+        compiled_view = await type(feature_view).compile()
         self.combined_feature_views[compiled_view.name] = compiled_view
 
     def add_model(self, model: Model) -> None:
-        compiled_model = type(model).compile()
-        self.models[compiled_model.name] = compiled_model
-
-    def with_source(self, source: OnlineSource | None = None) -> 'FeatureStore':
-        """
-        Creates a new instance of a feature store, but changes where to fetch the features from
-
-        ```
-        store = # Load the store
-        redis_store = store.with_source(redis.online_source())
-        batch_source = redis_store.with_source()
-        ```
-
-        Args:
-            source (OnlineSource): The source to fetch from, None will lead to using the batch source
+        self.models[model.name] = model.schema()
 
-        Returns:
-            FeatureStore: A new feature store instance
-        """
-        online_source = source or BatchOnlineSource()
+    def offline_store(self) -> 'FeatureStore':
         return FeatureStore(
             feature_views=self.feature_views,
             combined_feature_views=self.combined_feature_views,
-            models=self.models,
-            feature_source=online_source.feature_source(set(self.feature_views.values())),
+            models=self.model_requests,
+            feature_source=BatchOnlineSource().feature_source(set(self.feature_views.values())),
         )
 
-    def offline_store(self) -> 'FeatureStore':
-        return self.with_source()
-
-    def model_features_for(self, view_name: str) -> set[str]:
-        all_model_features: set[str] = set()
-        for model in self.models.values():
-            all_model_features.update(
-                {feature.name for feature in model.features if feature.location.name == view_name}
-            )
-        return all_model_features
-
 
 @dataclass
 class ModelFeatureStore:
 
-    model: ModelSchema
-    store: FeatureStore
+    source: FeatureSource
+    request: FeatureRequest
 
-    @property
-    def raw_string_features(self) -> set[str]:
-        return {f'{feature.location.identifier}:{feature.name}' for feature in self.model.features}
-
-    @property
-    def request(self) -> FeatureRequest:
-        return self.store.requests_for(RawStringFeatureRequest(self.raw_string_features))
+    def features_for(self, entities: dict[str, list]) -> FilterJob:
 
-    def features_for(self, entities: dict[str, list] | RetrivalJob) -> RetrivalJob:
-        request = self.request
-        features = self.raw_string_features
-        return self.store.features_for(entities, list(features)).filter(request.features_to_include)
-
-    def with_target(self) -> 'SupervisedModelFeatureStore':
-        return SupervisedModelFeatureStore(self.model, self.store)
-
-    def cached_at(self, location: DataFileReference) -> RetrivalJob:
-        from aligned.local.job import FileFullJob
+        if self.request.needs_event_timestamp and 'event_timestamp' not in entities:
+            raise ValueError('Missing event_timestamp in entities')
 
-        features = {f'{feature.location.identifier}:{feature.name}' for feature in self.model.features}
-        request = self.store.requests_for(RawStringFeatureRequest(features))
-
-        return FileFullJob(location, RetrivalRequest.unsafe_combine(request.needed_requests)).filter(
-            request.features_to_include
-        )
-
-    def process_features(self, input: RetrivalJob | dict[str, list]) -> RetrivalJob:
-        request = self.request
-
-        if isinstance(input, RetrivalJob):
-            job = input.filter(request.features_to_include)
-        elif isinstance(input, dict):
-            job = RetrivalJob.from_dict(input, request=request.needed_requests)
-        else:
-            raise ValueError(f'features must be a dict or a RetrivalJob, was {type(input)}')
-
-        return (
-            job.ensure_types(request.needed_requests)
-            .derive_features(request.needed_requests)
-            .filter(request.features_to_include)
+        return FilterJob(
+            self.request.features_to_include,
+            self.source.features_for(entities, self.request),
         )
 
+    def cached_at(self, location: DataFileReference) -> FilterJob:
+        from aligned.local.job import FileFullJob
 
-@dataclass
-class SupervisedModelFeatureStore:
-
-    model: ModelSchema
-    store: FeatureStore
-
-    def features_for(self, entities: dict[str, list] | RetrivalJob) -> SupervisedJob:
-        feature_refs = self.model.features
-        features = {f'{feature.location.identifier}:{feature.name}' for feature in feature_refs}
-        target_features = {
-            f'{feature.estimating.location.identifier}:{feature.estimating.name}'
-            for feature in self.model.predictions_view.classification_targets
-        }
-        targets = {feature.estimating.name for feature in self.model.predictions_view.classification_targets}
-        request = self.store.requests_for(RawStringFeatureRequest(features))
-        target_request = self.store.requests_for(
-            RawStringFeatureRequest(target_features)
-        ).without_event_timestamp(name_sufix='target')
-
-        total_request = FeatureRequest(
-            FeatureLocation.model(self.model.name),
-            request.features_to_include.union(target_request.features_to_include),
-            request.needed_requests + target_request.needed_requests,
-        )
-        job = self.store.features_for_request(total_request, entities, total_request.features_to_include)
-        return SupervisedJob(
-            job,
-            target_columns=targets,
+        return FilterJob(
+            self.request.features_to_include,
+            FileFullJob(location, RetrivalRequest.unsafe_combine(self.request.needed_requests)),
         )
 
 
 @dataclass
 class FeatureViewStore:
 
-    store: FeatureStore
+    source: FeatureSource
     view: CompiledFeatureView
-    event_triggers: set[EventTrigger] = field(default_factory=set)
     feature_filter: set[str] | None = field(default=None)
-    only_write_model_features: bool = field(default=False)
-
-    @property
-    def request(self) -> RetrivalRequest:
-        if self.only_write_model_features:
-            features_in_models = self.store.model_features_for(self.view.name)
-            return self.view.request_for(features_in_models).needed_requests[0]
-        else:
-            return self.view.request_all.needed_requests[0]
-
-    @property
-    def source(self) -> FeatureSource:
-        return self.store.feature_source
-
-    def with_optimised_write(self) -> 'FeatureViewStore':
-        features_in_models = self.store.model_features_for(self.view.name)
-        return self.select(features_in_models)
 
     def all(self, limit: int | None = None) -> RetrivalJob:
         if not isinstance(self.source, RangeFeatureSource):
             raise ValueError(f'The source ({self.source}) needs to conform to RangeFeatureSource')
 
-        request = self.view.request_all
         if self.feature_filter:
             request = self.view.request_for(self.feature_filter)
+            return FilterJob(include_features=self.feature_filter, job=self.source.all_for(request, limit))
 
-        job = (
-            self.source.all_for(request, limit)
-            .ensure_types(request.needed_requests)
-            .derive_features(request.needed_requests)
-        )
-        if self.feature_filter:
-            return FilterJob(include_features=self.feature_filter, job=job)
-        else:
-            return job
+        request = self.view.request_all
+        return self.source.all_for(request, limit)
 
-    def between_dates(self, start_date: datetime, end_date: datetime) -> RetrivalJob:
+    def between(self, start_date: datetime, end_date: datetime) -> RetrivalJob:
         if not isinstance(self.source, RangeFeatureSource):
             raise ValueError(
                 f'The source needs to conform to RangeFeatureSource, you got a {type(self.source)}'
             )
 
         if self.feature_filter:
             request = self.view.request_for(self.feature_filter)
@@ -515,110 +369,78 @@
 
         request = self.view.request_all
         return self.source.all_between(start_date, end_date, request)
 
     def previous(self, days: int = 0, minutes: int = 0, seconds: int = 0) -> RetrivalJob:
         end_date = datetime.utcnow()
         start_date = end_date - timedelta(days=days, minutes=minutes, seconds=seconds)
-        return self.between_dates(start_date, end_date)
-
-    def features_for(self, entities: dict[str, list] | RetrivalJob) -> RetrivalJob:
-
-        request = self.view.request_all
-        if self.feature_filter:
-            request = self.view.request_for(self.feature_filter)
-
-        if isinstance(entities, dict):
-            entity_job = RetrivalJob.from_dict(entities, request)
-        elif isinstance(entities, RetrivalJob):
-            entity_job = entities
-        else:
-            raise ValueError(f'entities must be a dict or a RetrivalJob, was {type(entities)}')
-
-        job = self.source.features_for(entity_job, request)
-        if self.feature_filter:
-            return job.filter(self.feature_filter)
-        else:
-            return job
+        return self.between(start_date, end_date)
 
     def select(self, features: set[str]) -> 'FeatureViewStore':
-        return FeatureViewStore(self.store, self.view, self.event_triggers, features)
+        return FeatureViewStore(self.source, self.view, features)
 
     @property
     def write_input(self) -> set[str]:
         features = set()
         for request in self.view.request_all.needed_requests:
             features.update(request.all_required_feature_names)
             features.update(request.entity_names)
             if event_timestamp := request.event_timestamp:
                 features.add(event_timestamp.name)
         return features
 
     async def write(self, values: dict[str, list[Any]]) -> None:
-        from aligned import FileSource
-        from aligned.data_file import DataFileReference
-        from aligned.schemas.derivied_feature import AggregateOver
-
-        request = self.view.request_all.needed_requests[0]
-        job = (
-            RetrivalJob.from_dict(values, request)
-            .validate_entites()
-            .fill_missing_columns()
-            .ensure_types([request])
-        )
-
-        aggregations = request.aggregate_over()
-        if aggregations:
-            checkpoints: dict[AggregateOver, DataFileReference] = {}
-
-            for aggregation in aggregations.keys():
-                name = f'{self.view.name}_agg'
+        await self.batch_write(values)
 
-                if aggregation.window:
-                    name += f'_{aggregation.window.time_window.total_seconds()}'
+    async def process_input(self, values: dict[str, list[Any]]) -> dict[str, list[Any]]:
+        from pandas import DataFrame
 
-                if aggregation.condition:
-                    name += f'_{aggregation.condition.name}'
-
-                checkpoints[aggregation] = FileSource.parquet_at(name)
-
-            job = StreamAggregationJob(job, checkpoints)
-
-        await self.batch_write(job)
-
-    def process_input(self, values: dict[str, list[Any]]) -> RetrivalJob:
+        from aligned.local.job import FileFullJob
+        from aligned.local.source import LiteralReference
 
         request = self.view.request_all.needed_requests[0]
+        df = DataFrame.from_records(values)
 
-        job = RetrivalJob.from_dict(values, request)
-
-        return job.fill_missing_columns().ensure_types([request]).derive_features([request])
-
-    async def batch_write(self, values: dict[str, list[Any]] | RetrivalJob) -> None:
+        if request.entity_names - set(df.columns):
+            missing = request.entity_names - set(df.columns)
+            raise ValueError(f'Missing entities: {missing}')
+
+        if request.all_required_feature_names - set(df.columns):
+            missing = request.all_required_feature_names - set(df.columns)
+            df[list(missing)] = None
+        output = await DerivedFeatureJob(
+            FileFullJob(LiteralReference(df), request), requests=[request]
+        ).to_pandas()
+        return output.to_dict('list')
 
+    async def batch_write(self, values: dict[str, list[Any]]) -> None:
         if not isinstance(self.source, WritableFeatureSource):
             logger.info('Feature Source is not writable')
             return
 
-        # As it is a feature view, should it only contain one request
-        request = self.request
+        from pandas import DataFrame
 
-        core_job: RetrivalJob
+        from aligned.local.job import FileFullJob
+        from aligned.local.source import LiteralReference
 
-        if isinstance(values, RetrivalJob):
-            core_job = values
-        elif isinstance(values, dict):
-            core_job = RetrivalJob.from_dict(values, request)
-        else:
-            raise ValueError(f'values must be a dict or a RetrivalJob, was {type(values)}')
-
-        job = (
-            core_job.derive_features([request])
-            .listen_to_events(self.event_triggers)
-            .update_vector_index(self.view.indexes)
-        )
+        # As it is a feature view, should it only contain one request
+        request = self.view.request_all.needed_requests[0]
+        df = DataFrame.from_records(values)
 
-        if self.feature_filter:
-            logger.info(f'Only writing features used by models: {self.feature_filter}')
-            job = job.filter(self.feature_filter)
+        if request.entity_names - set(df.columns):
+            missing = request.entity_names - set(df.columns)
+            raise ValueError(f'Missing entities: {missing}')
+
+        if request.all_required_feature_names - set(df.columns):
+            missing = request.all_required_feature_names - set(df.columns)
+            logger.info(
+                f"""
+Some features is missing.
+Will fill values with None, but it could be a potential problem: {missing}
+"""
+            )
+            df[list(missing)] = None
 
-        await self.source.write(job, [request])
+        await self.source.write(
+            DerivedFeatureJob(FileFullJob(LiteralReference(df), request, limit=None), requests=[request]),
+            [request],
+        )
```

### Comparing `aligned-0.0.9/aligned/feature_view/feature_view.py` & `aligned-0.0.9a0/aligned/feature_view/feature_view.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,76 @@
-from __future__ import annotations
-
 from abc import ABC, abstractproperty
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, TypeVar
+from typing import Callable, TypeVar
 
-from aligned.compiler.feature_factory import (
-    AggregationTransformationFactory,
-    Embedding,
-    Entity,
-    EventTimestamp,
-)
+from aligned.compiler.feature_factory import Entity, EventTimestamp, FeatureFactory
 from aligned.data_source.batch_data_source import BatchDataSource
 from aligned.data_source.stream_data_source import StreamDataSource
-from aligned.schemas.derivied_feature import AggregatedFeature, AggregateOver, AggregationTimeWindow
-from aligned.schemas.feature import FeatureLocation, FeatureReferance
+from aligned.request.retrival_request import FeatureRequest, RetrivalRequest
+from aligned.schemas.feature import Feature
 from aligned.schemas.feature_view import CompiledFeatureView
 
-if TYPE_CHECKING:
-    from aligned.feature_store import FeatureViewStore
-
 # Enables code compleation in the select method
 FVType = TypeVar('FVType')
 
 
+class FeatureSelectable:
+    @classmethod
+    def select(
+        cls: type[FVType], features: Callable[[type[FVType]], list[FeatureFactory]]
+    ) -> RetrivalRequest:
+        pass
+
+    @classmethod
+    def select_all(cls: type[FVType]) -> RetrivalRequest:
+        pass
+
+
 @dataclass
 class FeatureViewMetadata:
     name: str
     description: str
     batch_source: BatchDataSource
-    stream_source: StreamDataSource | None = field(default=None)
-    contacts: list[str] | None = field(default=None)
+    stream_source: StreamDataSource | None = None
     tags: dict[str, str] = field(default_factory=dict)
 
     @staticmethod
-    def from_compiled(view: CompiledFeatureView) -> FeatureViewMetadata:
+    def from_compiled(view: CompiledFeatureView) -> 'FeatureViewMetadata':
         return FeatureViewMetadata(
             name=view.name,
             description=view.description,
             tags=view.tags,
             batch_source=view.batch_data_source,
-            stream_source=view.stream_data_source,
+            stream_source=None,
         )
 
 
-class FeatureView(ABC):
+class FeatureView(ABC, FeatureSelectable):
     """
     A collection of features, and a way to combine them.
 
     This should contain the core features, and might contain derived features (aka. transformations).
     """
 
     @abstractproperty
     def metadata(self) -> FeatureViewMetadata:
         pass
 
-    @staticmethod
-    def metadata_with(
-        name: str,
-        description: str,
-        batch_source: BatchDataSource,
-        stream_source: StreamDataSource | None = None,
-        contacts: list[str] | None = None,
-        tags: dict[str, str] | None = None,
-    ) -> FeatureViewMetadata:
-        from aligned import HttpStreamSource
+    @classmethod
+    def select(cls: type[FVType], features: Callable[[type[FVType]], list[FeatureFactory]]) -> FeatureRequest:
+        view: CompiledFeatureView = cls.compile_graph_only()  # type: ignore
+        names = features(cls)
+        return view.request_for({feature.name for feature in names if feature.name})
 
-        return FeatureViewMetadata(
-            name,
-            description,
-            batch_source,
-            stream_source or HttpStreamSource(name),
-            contacts=contacts,
-            tags=tags or {},
-        )
+    @classmethod
+    def select_all(cls: type[FVType]) -> FeatureRequest:
+        return cls.compile_graph_only().request_all  # type: ignore
 
     @classmethod
-    def compile(cls) -> CompiledFeatureView:
+    async def compile(cls) -> CompiledFeatureView:
         from aligned.compiler.feature_factory import FeatureFactory
 
         # Used to deterministicly init names for hidden features
         hidden_features = 0
 
         metadata = cls().metadata
         var_names = [name for name in cls().__dir__() if not name.startswith('_')]
@@ -88,38 +79,27 @@
             name=metadata.name,
             description=metadata.description,
             tags=metadata.tags,
             batch_data_source=metadata.batch_source,
             entities=set(),
             features=set(),
             derived_features=set(),
-            aggregated_features=set(),
             event_timestamp=None,
             stream_data_source=metadata.stream_source,
-            indexes=[],
         )
-        aggregations: list[FeatureFactory] = []
 
         for var_name in var_names:
             feature = getattr(cls, var_name)
 
             if not isinstance(feature, FeatureFactory):
                 continue
 
             feature._name = var_name
-            feature._location = FeatureLocation.feature_view(metadata.name)
-            compiled_feature = feature.feature()
-
-            if isinstance(feature, Embedding) and feature.indexes:
-                view.indexes.extend(
-                    [
-                        index.compile(feature._location, compiled_feature, view.entities)
-                        for index in feature.indexes
-                    ]
-                )
+            feature._feature_view = metadata.name
+            compiled_feature = await feature.feature()
 
             if feature.transformation:
                 # Adding features that is not stored in the view
                 # e.g:
                 # class SomeView(FeatureView):
                 #     ...
                 #     x, y = Bool(), Bool()
@@ -131,46 +111,41 @@
                 # Sorting by key in order to instanciate the "core" features first
                 # And then making it possible for other features to reference them
                 def sort_key(x: tuple[int, FeatureFactory]) -> int:
                     return x[0]
 
                 for depth, feature_dep in sorted(feature_deps, key=sort_key):
 
-                    if not feature_dep._location:
-                        feature_dep._location = FeatureLocation.feature_view(metadata.name)
+                    if not feature_dep._feature_view:
+                        feature_dep._feature_view = metadata.name
 
                     if feature_dep._name:
-                        feat_dep = feature_dep.feature()
+                        feat_dep = await feature_dep.feature()
                         if feat_dep in view.features or feat_dep in view.entities:
                             continue
 
                     if depth == 0:
-                        # The raw value and the transformed have the same name
                         feature_dep._name = var_name
-                        feat_dep = feature_dep.feature()
+                        feat_dep = await feature_dep.feature()
                         view.features.add(feat_dep)
                         continue
 
                     if not feature_dep._name:
                         feature_dep._name = str(hidden_features)
                         hidden_features += 1
 
-                    if isinstance(feature_dep.transformation, AggregationTransformationFactory):
-                        aggregations.append(feature_dep)
-                    else:
-                        feature_graph = feature_dep.compile()  # Should decide on which payload to send
-                        if feature_graph in view.derived_features:
-                            continue
+                    feature_graph = feature_dep.compile_graph_only()  # Should decide on which payload to send
+                    if feature_graph in view.derived_features:
+                        continue
 
-                        view.derived_features.add(feature_dep.compile())
+                    view.derived_features.add(await feature_dep.compile([view]))
 
-                if isinstance(feature.transformation, AggregationTransformationFactory):
-                    aggregations.append(feature)
-                else:
-                    view.derived_features.add(feature.compile())  # Should decide on which payload to send
+                view.derived_features.add(
+                    await feature.compile([view])  # Should decide on which payload to send
+                )
 
             elif isinstance(feature, Entity):
                 view.entities.add(compiled_feature)
             elif isinstance(feature, EventTimestamp):
                 if view.event_timestamp is not None:
                     raise Exception(
                         'Can only have one EventTimestamp for each'
@@ -181,49 +156,104 @@
                 view.event_timestamp = feature.event_timestamp()
             else:
                 view.features.add(compiled_feature)
 
         if not view.entities:
             raise ValueError(f'FeatureView {metadata.name} must contain at least one Entity')
 
-        aggregation_group_by = [
-            FeatureReferance(entity.name, FeatureLocation.feature_view(view.name), entity.dtype)
-            for entity in view.entities
-        ]
-
-        for aggr in aggregations:
-            agg_trans = aggr.transformation
-            if not isinstance(agg_trans, AggregationTransformationFactory):
+        return view
+
+    @classmethod
+    def compile_graph_only(cls) -> CompiledFeatureView:
+        """Compiles a view with all its metadata,
+        However it is not containing the correct compiled transofmrations in all cases
+        As it will nto compute the different artefacts.
+
+        This is a flaw in the current system and should potentially be fixed by creating artefacts
+        based on data models and not views. As that is more data set spesifics.
+        It would therefore not need two different compile methods
+        """
+        from aligned.compiler.feature_factory import FeatureFactory
+
+        # Used to deterministicly init names for hidden features
+        hidden_features = 0
+
+        metadata = cls().metadata
+        var_names = [name for name in cls().__dir__() if not name.startswith('_')]
+
+        view = CompiledFeatureView(
+            name=metadata.name,
+            description=metadata.description,
+            tags=metadata.tags,
+            batch_data_source=metadata.batch_source,
+            entities=set(),
+            features=set(),
+            derived_features=set(),
+            event_timestamp=None,
+            stream_data_source=metadata.stream_source,
+        )
+
+        for var_name in var_names:
+            feature = getattr(cls, var_name)
+
+            if not isinstance(feature, FeatureFactory):
                 continue
 
-            if view.event_timestamp is None and agg_trans.time_window:
-                raise ValueError(f'FeatureView {metadata.name} must contain an EventTimestamp')
+            feature._name = var_name
+            feature._feature_view = metadata.name
+            compiled_feature = Feature(name=feature._name, dtype=feature.dtype)
 
-            time_window: AggregationTimeWindow | None = None
-            if agg_trans.time_window:
+            if feature.transformation:
+                feature_deps = [(feat.depth(), feat) for feat in feature.feature_dependencies()]
 
-                timestamp_ref = FeatureReferance(
-                    view.event_timestamp.name,
-                    FeatureLocation.feature_view(view.name),
-                    dtype=view.event_timestamp.dtype,
-                )
-                time_window = AggregationTimeWindow(agg_trans.time_window, timestamp_ref)
+                # Sorting by key in order to instanciate the "core" features first
+                # And then making it possible for other features to reference them
+                def sort_key(x: tuple[int, FeatureFactory]) -> int:
+                    return x[0]
 
-            aggr.transformation = agg_trans.with_group_by(aggregation_group_by)
-            config = AggregateOver(aggregation_group_by, window=time_window, condition=None)
-            feature = aggr.compile()
-            feat = AggregatedFeature(
-                derived_feature=feature,
-                aggregate_over=config,
-            )
-            view.aggregated_features.add(feat)
+                for depth, feature_dep in sorted(feature_deps, key=sort_key):
 
-        return view
+                    if not feature_dep._feature_view:
+                        feature_dep._feature_view = metadata.name
 
-    @classmethod
-    def query(cls) -> FeatureViewStore:
-        from aligned import FeatureStore
+                    if feature_dep._name:
+                        feat_dep = Feature(feature_dep._name, dtype=feature_dep.dtype)
+                        if feat_dep in view.features or feat_dep in view.entities:
+                            continue
+
+                    if depth == 0:
+                        feature_dep._name = var_name
+                        feat_dep = Feature(var_name, dtype=feature_dep.dtype)
+                        view.features.add(feat_dep)
+                        continue
+
+                    if not feature_dep._name:
+                        feature_dep._name = str(hidden_features)
+                        hidden_features += 1
 
-        self = cls()
-        store = FeatureStore.experimental()
-        store.add_feature_view(self)
-        return store.feature_view(self.metadata.name)
+                    feature_graph = feature_dep.compile_graph_only()  # Should decide on which payload to send
+                    if feature_graph in view.derived_features:
+                        continue
+
+                    view.derived_features.add(
+                        feature_dep.compile_graph_only()  # Should decide on which payload to send
+                    )
+                view.derived_features.add(feature.compile_graph_only())
+            elif isinstance(feature, Entity):
+                view.entities.add(compiled_feature)
+
+            elif isinstance(feature, EventTimestamp):
+                if view.event_timestamp is not None:
+                    raise Exception(
+                        'Can only have one EventTimestamp for each'
+                        ' FeatureViewDefinition. Check that this is the case for'
+                        f' {cls.__name__}'
+                    )
+                view.features.add(compiled_feature)
+                view.event_timestamp = feature.event_timestamp()
+            else:
+                view.features.add(compiled_feature)
+
+        if not view.entities:
+            raise ValueError(f'FeatureView {metadata.name} must contain at least one Entity')
+
+        return view
```

### Comparing `aligned-0.0.9/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,22 +10,25 @@
     breast_scan_feature_view_with_datetime: FeatureView,
     breast_scan_with_timestamp_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime
     store = breast_scan_with_timestamp_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
     assert limit_features.shape[0] == 6
 
@@ -35,49 +38,56 @@
     breast_scan_feature_view_with_datetime_and_aggregation: FeatureView,
     breast_scan_with_timestamp_and_aggregation_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime_and_aggregation
     store = breast_scan_with_timestamp_and_aggregation_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
 
     assert limit_features.shape[0] == 6
+    assert features['mean_fd_worst_for_group'].isna().count() != 0
 
 
-# @pytest.mark.asyncio
-# async def test_between_datetime_features_polars(
-#     breast_scan_feature_view_with_datetime: FeatureView,
-#     breast_scan_with_timestamp_feature_store: FeatureStore,
-# ) -> None:
-#     feature_view = breast_scan_feature_view_with_datetime
-#     store = breast_scan_with_timestamp_feature_store
-#     job = store.feature_view(feature_view.metadata.name).all()
-#     features = (await job.to_polars()).collect()
-
-#     assert 'created_at' in features.columns
-#     assert 'is_malignant' in features.columns
-#     assert 'diagnosis' in features.columns
-#     assert 'scan_id' in features.columns
-
-#     limit_features = (
-#         await store.feature_view(feature_view.metadata.name)
-#         .between_dates(
-#             start_date=datetime(2020, 1, 5),
-#             end_date=datetime(2020, 1, 11),
-#         )
-#         .to_polars()
-#     ).collect()
+@pytest.mark.asyncio
+async def test_between_datetime_features_polars(
+    breast_scan_feature_view_with_datetime: FeatureView,
+    breast_scan_with_timestamp_feature_store: FeatureStore,
+) -> None:
+    feature_view = breast_scan_feature_view_with_datetime
+    store = breast_scan_with_timestamp_feature_store
+    job = store.feature_view(feature_view.metadata.name).all()
+    features = (await job.to_polars()).collect()
+
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
 
-#     assert limit_features.shape[0] == 6
+    assert 'created_at' in features.columns
+    assert 'is_malignant' in features.columns
+    assert 'diagnosis' in features.columns
+    assert 'scan_id' in features.columns
+
+    limit_features = (
+        await store.feature_view(feature_view.metadata.name)
+        .between(
+            start_date=datetime(2020, 1, 5),
+            end_date=datetime(2020, 1, 11),
+        )
+        .to_polars()
+    ).collect()
+
+    assert limit_features.shape[0] == 6
```

### Comparing `aligned-0.0.9/aligned/feature_view/tests/test_combined_view.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/jobs/tests/test_combined_job.py` & `aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/jobs/tests/test_derived_job.py` & `aligned-0.0.9a0/aligned/jobs/tests/test_derived_job.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/local/job.py` & `aligned-0.0.9a0/aligned/local/job.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,41 +2,18 @@
 from datetime import datetime
 
 import pandas as pd
 import polars as pl
 
 from aligned.local.source import DataFileReference
 from aligned.request.retrival_request import RetrivalRequest
-from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RequestResult, RetrivalJob
+from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RequestResult
 from aligned.schemas.feature import Feature
 
 
-class LiteralRetrivalJob(RetrivalJob):
-
-    df: pl.LazyFrame
-    result: RequestResult
-
-    def __init__(self, df: pl.LazyFrame | pd.DataFrame, result: RequestResult) -> None:
-        self.result = result
-        if isinstance(df, pd.DataFrame):
-            self.df = pl.from_pandas(df).lazy()
-        else:
-            self.df = df
-
-    @property
-    def request_result(self) -> RequestResult:
-        return self.result
-
-    async def to_pandas(self) -> pd.DataFrame:
-        return self.df.collect().to_pandas()
-
-    async def to_polars(self) -> pl.LazyFrame:
-        return self.df
-
-
 @dataclass
 class FileFullJob(FullExtractJob):
 
     source: DataFileReference
     request: RetrivalRequest
     limit: int | None = field(default=None)
 
@@ -157,98 +134,55 @@
 
 
 @dataclass
 class FileFactualJob(FactualRetrivalJob):
 
     source: DataFileReference
     requests: list[RetrivalRequest]
-    facts: RetrivalJob
+    facts: dict[str, list]
 
     @property
     def request_result(self) -> RequestResult:
         return RequestResult.from_request_list(self.requests)
 
-    async def file_transformations(self, df: pl.LazyFrame) -> pl.LazyFrame:
-        """Selects only the wanted subset from the loaded source
-
-        ```python
-        await self.file_transformations(await self.source.to_polars())
-        ```
-
-        Args:
-            df (pl.LazyFrame): The loaded file source which contains all features
-
-        Returns:
-            pl.LazyFrame: The subset of the source which is needed for the request
-        """
+    def file_transformations(self, df: pd.DataFrame) -> pd.DataFrame:
         from aligned.data_source.batch_data_source import ColumnFeatureMappable
 
         all_features: set[Feature] = set()
         for request in self.requests:
             all_features.update(request.all_required_features)
 
-        result = await self.facts.to_polars()
-        event_timestamp_col = 'event_timestamp'
-        row_id_name = 'row_id'
-        result = result.with_row_count(row_id_name)
+        result = pd.DataFrame(self.facts)
 
         for request in self.requests:
             entity_names = request.entity_names
             all_names = request.all_required_feature_names.union(entity_names)
 
-            if request.event_timestamp:
-                all_names.add(request.event_timestamp.name)
-
             request_features = all_names
             if isinstance(self.source, ColumnFeatureMappable):
                 request_features = self.source.feature_identifier_for(all_names)
 
-            feature_df = df.select(request_features)
-
-            renames = {org_name: wanted_name for org_name, wanted_name in zip(request_features, all_names)}
-            feature_df = feature_df.rename(renames)
-
-            for entity in request.entities:
-                feature_df = feature_df.with_column(pl.col(entity.name).cast(entity.dtype.polars_type))
-                result = result.with_column(pl.col(entity.name).cast(entity.dtype.polars_type))
-
-            column_selects = list(entity_names.union({'row_id'}))
-            if request.event_timestamp:
-                column_selects.append('event_timestamp')
-
-            # Need to only select the relevent entities and row_id
-            # Otherwise will we get a duplicate column error
-            # We also need to remove the entities after the row_id is joined
-            new_result: pl.LazyFrame = result.select(column_selects).join(
-                feature_df, on=list(entity_names), how='left'
+            mask = pd.Series.repeat(pd.Series([True]), df.shape[0]).reset_index(drop=True)
+            set_mask = pd.Series.repeat(pd.Series([True]), result.shape[0]).reset_index(drop=True)
+            for entity in entity_names:
+                entity
+                if isinstance(self.source, ColumnFeatureMappable):
+                    entity_source_name = self.source.feature_identifier_for([entity])[0]
+
+                mask = mask & (df[entity_source_name].isin(self.facts[entity]))
+
+                set_mask = set_mask & (pd.Series(self.facts[entity]).isin(df[entity_source_name]))
+
+            feature_df = df.loc[mask, request_features]
+            feature_df = feature_df.rename(
+                columns={org_name: wanted_name for org_name, wanted_name in zip(request_features, all_names)},
             )
-            new_result = new_result.select(pl.exclude(list(entity_names)))
-
-            if request.event_timestamp:
-                new_result = new_result.with_columns(
-                    pl.col(request.event_timestamp.name)
-                    .str.strptime(pl.Datetime, '%+')
-                    .alias(request.event_timestamp.name)
-                )
-                field = request.event_timestamp.name
-                ttl = request.event_timestamp.ttl
-                if ttl:
-                    ttl_request = (pl.col(field) <= pl.col(event_timestamp_col)) & (
-                        pl.col(field) >= pl.col(event_timestamp_col) - ttl
-                    )
-                    new_result = new_result.filter(pl.col(field).is_null() | ttl_request)
-                else:
-                    new_result = new_result.filter(
-                        pl.col(field).is_null() | (pl.col(field) <= pl.col(event_timestamp_col))
-                    )
-
-            unique = new_result.unique(subset=row_id_name, keep='first')
-            result = result.join(unique, on=row_id_name, how='left')
-            result = result.select(pl.exclude('.*_right$'))
+            result.loc[set_mask, list(all_names)] = feature_df.reset_index(drop=True)
 
-        return result.select([pl.exclude('row_id')])
+        return result
 
     async def to_pandas(self) -> pd.DataFrame:
-        return (await self.to_polars()).collect().to_pandas()
+        file = await self.source.read_pandas()
+        return self.file_transformations(file)
 
     async def to_polars(self) -> pl.LazyFrame:
-        return await self.file_transformations(await self.source.to_polars())
+        return pl.from_pandas(await self.to_pandas())
```

### Comparing `aligned-0.0.9/aligned/local/source.py` & `aligned-0.0.9a0/aligned/local/source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
-from pathlib import Path
-from typing import TYPE_CHECKING, Literal
+from typing import Literal
 from uuid import uuid4
 
 import pandas as pd
 import polars as pl
 from httpx import HTTPStatusError
 
 from aligned.data_file import DataFileReference
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.enricher import CsvFileEnricher, Enricher, LoadedStatEnricher, StatisticEricher, TimespanSelector
 from aligned.exceptions import UnableToFindFileException
+from aligned.feature_store import FeatureStore
 from aligned.local.job import FileDateJob, FileFactualJob, FileFullJob
 from aligned.request.retrival_request import RetrivalRequest
-from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RetrivalJob
+from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob
 from aligned.s3.storage import FileStorage, HttpStorage
 from aligned.schemas.codable import Codable
-from aligned.schemas.folder import Folder
+from aligned.schemas.repo_definition import RepoDefinition
 from aligned.storage import Storage
 
-if TYPE_CHECKING:
-    from aligned.feature_store import FeatureStore
-
-
 logger = logging.getLogger(__name__)
 
 
 class StorageFileReference:
     """
     A reference to a file that can be loaded as bytes.
 
@@ -40,17 +36,14 @@
     async def read(self) -> bytes:
         raise NotImplementedError()
 
     async def write(self, content: bytes) -> None:
         raise NotImplementedError()
 
     async def feature_store(self) -> FeatureStore:
-        from aligned import FeatureStore
-        from aligned.schemas.repo_definition import RepoDefinition
-
         file = await self.read()
         return FeatureStore.from_definition(RepoDefinition.from_json(file))
 
 
 @dataclass
 class CsvConfig(Codable):
     """
@@ -87,23 +80,14 @@
             )
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
     async def to_polars(self) -> pl.LazyFrame:
-
-        if self.path.startswith('http'):
-            from io import BytesIO
-
-            buffer = await HttpStorage().read(self.path)
-            io_buffer = BytesIO(buffer)
-            io_buffer.seek(0)
-            return pl.read_csv(io_buffer, sep=self.csv_config.seperator).lazy()
-
         return pl.scan_csv(self.path, sep=self.csv_config.seperator)
 
     async def write_pandas(self, df: pd.DataFrame) -> None:
         df.to_csv(
             self.path,
             sep=self.csv_config.seperator,
             compression=self.csv_config.compression,
@@ -138,29 +122,28 @@
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
     ) -> DateRangeJob:
         return FileDateJob(source=self, request=request, start_date=start_date, end_date=end_date)
 
     @classmethod
-    def multi_source_features_for(
-        cls, facts: RetrivalJob, requests: list[tuple[CsvFileSource, RetrivalRequest]]
+    def feature_for(
+        cls, facts: dict[str, list], requests: dict[CsvFileSource, RetrivalRequest]
     ) -> FactualRetrivalJob:
-        sources = {source for source, _ in requests}
-        if len(sources) != 1:
+        if len(requests.keys()) != 1:
             raise ValueError(f'Only able to load one {requests} at a time')
 
-        source = list(sources)[0]
+        source = list(requests.keys())[0]
         if not isinstance(source, cls):
             raise ValueError(f'Only {cls} is supported, recived: {source}')
 
         # Group based on config
         return FileFactualJob(
             source=source,
-            requests=[request for _, request in requests],
+            requests=list(requests.values()),
             facts=facts,
         )
 
 
 @dataclass
 class ParquetConfig(Codable):
     """
@@ -169,15 +152,15 @@
 
     engine: Literal['auto', 'pyarrow', 'fastparquet'] = field(default='auto')
     compression: Literal['snappy', 'gzip', 'brotli', None] = field(default='snappy')
     should_write_index: bool = field(default=False)
 
 
 @dataclass
-class ParquetFileSource(BatchDataSource, ColumnFeatureMappable, DataFileReference):
+class ParquetFileSource(BatchDataSource, ColumnFeatureMappable):
     """
     A source pointing to a Parquet file
     """
 
     path: str
     mapping_keys: dict[str, str] = field(default_factory=dict)
     config: ParquetConfig = field(default_factory=ParquetConfig)
@@ -202,43 +185,37 @@
         df.to_parquet(
             self.path,
             engine=self.config.engine,
             compression=self.config.compression,
             index=self.config.should_write_index,
         )
 
-    async def to_polars(self) -> pl.LazyFrame:
-        return pl.scan_parquet(self.path)
-
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        df.sink_parquet(self.path, compression=self.config.compression)
-
     def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         return FileFullJob(self, request, limit)
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
     ) -> DateRangeJob:
         return FileDateJob(source=self, request=request, start_date=start_date, end_date=end_date)
 
     @classmethod
-    def multi_source_features_for(
-        cls, facts: RetrivalJob, requests: list[tuple[ParquetFileSource, RetrivalRequest]]
+    def feature_for(
+        cls, facts: dict[str, list], requests: dict[ParquetFileSource, RetrivalRequest]
     ) -> FactualRetrivalJob:
-        if len(requests) != 1:
+        if len(requests.keys()) != 1:
             raise ValueError(f'Only able to load one {requests} at a time')
 
-        source = requests[0][0]
+        source = list(requests.keys())[0]
         if not isinstance(source, cls):
             raise ValueError(f'Only {cls} is supported, recived: {source}')
 
         # Group based on config
         return FileFactualJob(
             source=source,
-            requests=[request for _, request in requests],
+            requests=list(requests.values()),
             facts=facts,
         )
 
 
 @dataclass
 class StorageFileSource(StorageFileReference):
 
@@ -254,72 +231,53 @@
     def __hash__(self) -> int:
         return hash(self.path)
 
     async def read(self) -> bytes:
         return await self.storage.read(self.path)
 
     async def write(self, content: bytes) -> None:
-        await self.storage.write(self.path, content)
+        return await self.storage.write(self.path, content)
 
 
 class FileSource:
     """
     A factory class, creating references to files.
 
     This therefore abstracts away the concrete classes the users wants.
     Therefore making them easier to discover.
     """
 
     @staticmethod
-    def json_at(path: str) -> StorageFileSource:
+    def from_path(path: str) -> StorageFileSource:
         return StorageFileSource(path=path)
 
     @staticmethod
     def csv_at(
         path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
     ) -> CsvFileSource:
         return CsvFileSource(path, mapping_keys=mapping_keys or {}, csv_config=csv_config or CsvConfig())
 
     @staticmethod
     def parquet_at(
         path: str, mapping_keys: dict[str, str] | None = None, config: ParquetConfig | None = None
     ) -> ParquetFileSource:
         return ParquetFileSource(path=path, mapping_keys=mapping_keys or {}, config=config or ParquetConfig())
 
-    @staticmethod
-    def folder(path: str) -> Folder:
-        return LocalFolder(base_path=Path(path))
-
 
 @dataclass
-class LocalFolder(Folder):
-
-    base_path: Path
-    name = 'local_folder'
-
-    def file_at(self, path: Path) -> StorageFileReference:
-        return StorageFileSource(path=str(self.base_path / path))
-
-
 class LiteralReference(DataFileReference):
     """
     A class containing a in mem pandas frame.
 
     This makes it easier standardise the interface when writing data.
     """
 
-    file: pl.LazyFrame
-
-    def __init__(self, file: pl.LazyFrame | pd.DataFrame) -> None:
-        if isinstance(file, pd.DataFrame):
-            self.file = pl.from_pandas(file).lazy()
-        else:
-            self.file = file
+    file: pd.DataFrame
 
     def job_group_key(self) -> str:
         return str(uuid4())
 
     async def read_pandas(self) -> pd.DataFrame:
-        return self.file.collect().to_pandas()
+        return self.file
 
     async def to_polars(self) -> pl.LazyFrame:
-        return self.file
+        return pl.from_pandas(self.file).lazy()
```

### Comparing `aligned-0.0.9/aligned/online_source.py` & `aligned-0.0.9a0/aligned/online_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from dataclasses import dataclass
 from typing import Any, Optional
 
 from mashumaro.types import SerializableType
 
 from aligned.feature_source import FeatureSource, InMemoryFeatureSource
 from aligned.schemas.codable import Codable
-from aligned.schemas.feature import FeatureLocation
 from aligned.schemas.feature_view import CompiledFeatureView
 
 logger = logging.getLogger(__name__)
 
 
 class OnlineSourceFactory:
 
@@ -85,17 +84,15 @@
 
     source_type = 'batch'
 
     def feature_source(self, feature_views: set[CompiledFeatureView]) -> FeatureSource:
         from aligned.feature_source import BatchFeatureSource
 
         return BatchFeatureSource(
-            sources={
-                FeatureLocation.feature_view(fv.name).identifier: fv.batch_data_source for fv in feature_views
-            }
+            sources={fv.name: fv.batch_data_source for fv in feature_views},
         )
 
 
 @dataclass
 class InMemoryOnlineSource(OnlineSource):
 
     source_type: str = 'in-mem'
```

### Comparing `aligned-0.0.9/aligned/psql/data_source.py` & `aligned-0.0.9a0/aligned/psql/data_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING, Callable
 
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.enricher import SqlDatabaseEnricher, StatisticEricher
 from aligned.request.retrival_request import RetrivalRequest
-from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob, RetrivalJob
+from aligned.retrival_job import DateRangeJob, FactualRetrivalJob, FullExtractJob
 from aligned.schemas.codable import Codable
 
 if TYPE_CHECKING:
     from aligned.enricher import Enricher, TimespanSelector
     from aligned.entity_data_source import EntityDataSource
 
 
@@ -26,42 +26,34 @@
 
         return os.environ[self.env_var]
 
     @staticmethod
     def from_url(url: str) -> PostgreSQLConfig:
         import os
 
-        if 'PSQL_DATABASE' not in os.environ:
-            os.environ['PSQL_DATABASE'] = url
+        os.environ['PSQL_DATABASE'] = url
         return PostgreSQLConfig(env_var='PSQL_DATABASE')
 
     @staticmethod
-    def localhost(db: str, credentials: tuple[str, str] | None = None) -> PostgreSQLConfig:
-        if credentials:
-            return PostgreSQLConfig.from_url(f'postgresql://{credentials[0]}:{credentials[1]}@localhost/{db}')
+    def localhost(db: str) -> PostgreSQLConfig:
         return PostgreSQLConfig.from_url(f'postgresql://localhost/{db}')
 
     def table(self, table: str, mapping_keys: dict[str, str] | None = None) -> PostgreSQLDataSource:
         return PostgreSQLDataSource(config=self, table=table, mapping_keys=mapping_keys or {})
 
     def data_enricher(self, sql: str, values: dict | None = None) -> Enricher:
         from aligned.enricher import SqlDatabaseEnricher
 
         return SqlDatabaseEnricher(self.env_var, sql, values)
 
     def entity_source(self, timestamp_column: str, sql: Callable[[str], str]) -> EntityDataSource:
-        from aligned.compiler.model import SqlEntityDataSource
+        from aligned.model import SqlEntityDataSource
 
         return SqlEntityDataSource(sql, self.env_var, timestamp_column)
 
-    def fetch(self, query: str) -> RetrivalJob:
-        from aligned.psql.jobs import PostgreSqlJob
-
-        return PostgreSqlJob(self, query)
-
 
 @dataclass
 class PostgreSQLDataSource(BatchDataSource, ColumnFeatureMappable, StatisticEricher):
 
     config: PostgreSQLConfig
     table: str
     mapping_keys: dict[str, str]
@@ -83,15 +75,15 @@
         query = f'SELECT {sql_columns} FROM {self.table}'
         if time:
             seconds = time.timespand.total_seconds()
             query += f' WHERE {time.time_column} >= NOW() - interval \'{seconds} seconds\''
         if limit and isinstance(limit, int):
             query += f' LIMIT {limit}'
 
-        return SqlDatabaseEnricher(self.config.env_var, query)
+        return SqlDatabaseEnricher(self.config.url, query)
 
     def std(
         self, columns: set[str], time: TimespanSelector | None = None, limit: int | None = None
     ) -> Enricher:
         reverse_map = {value: key for key, value in self.mapping_keys.items()}
         sql_columns = ', '.join(
             [f'STDDEV({reverse_map.get(column, column)}) AS {column}' for column in columns]
@@ -100,15 +92,15 @@
         query = f'SELECT {sql_columns} FROM {self.table}'
         if time:
             seconds = time.timespand.total_seconds()
             query += f' WHERE {time.time_column} >= NOW() - interval \'{seconds} seconds\''
         if limit and isinstance(limit, int):
             query += f' LIMIT {limit}'
 
-        return SqlDatabaseEnricher(self.config.env_var, query)
+        return SqlDatabaseEnricher(self.config.url, query)
 
     def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         from aligned.psql.jobs import FullExtractPsqlJob
 
         return FullExtractPsqlJob(self, request, limit)
 
     def all_between_dates(
@@ -118,18 +110,18 @@
         end_date: datetime,
     ) -> DateRangeJob:
         from aligned.psql.jobs import DateRangePsqlJob
 
         return DateRangePsqlJob(self, start_date, end_date, request)
 
     @classmethod
-    def multi_source_features_for(
-        cls, facts: RetrivalJob, requests: list[tuple[PostgreSQLDataSource, RetrivalRequest]]
+    def feature_for(
+        cls, facts: dict[str, list], requests: dict[PostgreSQLDataSource, RetrivalRequest]
     ) -> FactualRetrivalJob:
         # Group based on config
         from aligned.psql.jobs import FactPsqlJob
 
         return FactPsqlJob(
-            sources={request.location: source for source, request in requests},
-            requests=[request for _, request in requests],
+            sources={request.feature_view_name: source for source, request in requests.items()},
+            requests=list(requests.values()),
             facts=facts,
         )
```

### Comparing `aligned-0.0.9/aligned/redis/stream.py` & `aligned-0.0.9a0/aligned/redis/stream.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/redshift/data_source.py` & `aligned-0.0.9a0/aligned/redshift/data_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Callable
 
 from aligned import RedisConfig
-from aligned.compiler.model import EntityDataSource, SqlEntityDataSource
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.enricher import Enricher
-from aligned.psql.data_source import PostgreSQLConfig, PostgreSQLDataSource
-from aligned.retrival_job import DateRangeJob, RetrivalJob, RetrivalRequest
+from aligned.model import EntityDataSource, SqlEntityDataSource
+from aligned.psql.data_source import PostgreSQLConfig
+from aligned.retrival_job import DateRangeJob, RetrivalRequest
 from aligned.schemas.codable import Codable
 
 
 @dataclass
 class RedshiftSQLConfig(Codable):
     env_var: str
     schema: str | None = None
@@ -26,21 +24,21 @@
 
     @property
     def psql_config(self) -> PostgreSQLConfig:
 
         return PostgreSQLConfig(self.env_var, self.schema)
 
     @staticmethod
-    def from_url(url: str) -> RedshiftSQLConfig:
+    def from_url(url: str) -> 'RedshiftSQLConfig':
         import os
 
         os.environ['REDSHIFT_DATABASE'] = url.replace('redshift:', 'postgresql:')
         return RedshiftSQLConfig(env_var='REDSHIFT_DATABASE')
 
-    def table(self, table: str, mapping_keys: dict[str, str] | None = None) -> RedshiftSQLDataSource:
+    def table(self, table: str, mapping_keys: dict[str, str] | None = None) -> 'RedshiftSQLDataSource':
         return RedshiftSQLDataSource(config=self, table=table, mapping_keys=mapping_keys or {})
 
     def data_enricher(
         self, name: str, sql: str, redis: RedisConfig, values: dict | None = None, lock_timeout: int = 60
     ) -> Enricher:
         from pathlib import Path
 
@@ -63,38 +61,21 @@
 
     config: RedshiftSQLConfig
     table: str
     mapping_keys: dict[str, str]
 
     type_name = 'redshift'
 
-    def to_psql_source(self) -> PostgreSQLDataSource:
-        return PostgreSQLDataSource(self.config.psql_config, self.table, self.mapping_keys)
-
     def job_group_key(self) -> str:
         return self.config.env_var
 
     def __hash__(self) -> int:
         return hash(self.table)
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
     ) -> DateRangeJob:
         from aligned.psql.jobs import DateRangePsqlJob, PostgreSQLDataSource
 
         source = PostgreSQLDataSource(self.config.psql_config, self.table, self.mapping_keys)
 
         return DateRangePsqlJob(source, start_date, end_date, request)
-
-    @classmethod
-    def multi_source_features_for(
-        cls: type[RedshiftSQLDataSource],
-        facts: RetrivalJob,
-        requests: list[tuple[RedshiftSQLDataSource, RetrivalRequest]],
-    ) -> RetrivalJob:
-        from aligned.redshift.jobs import FactRedshiftJob
-
-        return FactRedshiftJob(
-            sources={request.location: source.to_psql_source() for source, request in requests},
-            requests=[request for _, request in requests],
-            facts=facts,
-        )
```

### Comparing `aligned-0.0.9/aligned/redshift/factory.py` & `aligned-0.0.9a0/aligned/redshift/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         self,
         facts: dict[str, list],
         requests: dict[RedshiftSQLDataSource, RetrivalRequest],
     ) -> FactPsqlJob:
         # Group based on config
         return FactPsqlJob(
             facts=facts,
-            sources={request.location: source for source, request in requests.items()},
+            sources={request.feature_view_name: source for source, request in requests.items()},
             requests=list(requests.values()),
         )
```

### Comparing `aligned-0.0.9/aligned/request/retrival_request.py` & `aligned-0.0.9a0/aligned/request/retrival_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,51 @@
-from collections import defaultdict
 from dataclasses import dataclass, field
 
 from aligned.schemas.codable import Codable
-from aligned.schemas.derivied_feature import AggregatedFeature, AggregateOver, DerivedFeature
-from aligned.schemas.feature import EventTimestamp, Feature, FeatureLocation
+from aligned.schemas.derivied_feature import DerivedFeature
+from aligned.schemas.feature import EventTimestamp, Feature
 
 
 @dataclass
 class RetrivalRequest(Codable):
     """
     Describes all the information needed for a request to be successful.
 
     This do not mean all the data is shown to the end user,
     as there may be some features that depend on other features.
     """
 
-    name: str
-    location: FeatureLocation
+    feature_view_name: str
     entities: set[Feature]
     features: set[Feature]
     derived_features: set[DerivedFeature]
-    aggregated_features: set[AggregatedFeature] = field(default_factory=set)
     event_timestamp: EventTimestamp | None = field(default=None)
 
-    features_to_exclude: set[str] = field(default_factory=set)
-
-    def filter_features(self, feature_names: set[str]) -> 'RetrivalRequest':
-        return RetrivalRequest(
-            name=self.name,
-            location=self.location,
-            entities=self.entities,
-            features=self.features,
-            derived_features=self.derived_features,
-            aggregated_features=self.aggregated_features,
-            event_timestamp=self.event_timestamp,
-            features_to_exclude=self.features_to_exclude.union(self.all_feature_names - feature_names),
-        )
-
-    @property
-    def returned_features(self) -> set[Feature]:
-        return {feature for feature in self.all_features if feature.name not in self.features_to_exclude}
-
     @property
     def feature_names(self) -> list[str]:
         return [feature.name for feature in self.features]
 
     @property
     def request_result(self) -> 'RequestResult':
         return RequestResult.from_request(self)
 
     def derived_feature_map(self) -> dict[str, DerivedFeature]:
-        return {
-            feature.name: feature for feature in self.derived_features.union(self.derived_aggregated_features)
-        }
-
-    @property
-    def derived_aggregated_features(self) -> set[DerivedFeature]:
-        return {feature.derived_feature for feature in self.aggregated_features}
+        return {feature.name: feature for feature in self.derived_features}
 
     @property
     def all_required_features(self) -> set[Feature]:
         return self.features - self.entities
 
     @property
     def all_required_feature_names(self) -> set[str]:
         return {feature.name for feature in self.all_required_features}
 
     @property
     def all_features(self) -> set[Feature]:
-        return self.features.union(self.derived_features).union(
-            {feature.derived_feature for feature in self.aggregated_features}
-        )
+        return self.features.union(self.derived_features)
 
     @property
     def all_feature_names(self) -> set[str]:
         return {feature.name for feature in self.all_features}
 
     @property
     def entity_names(self) -> set[str]:
@@ -105,102 +76,64 @@
             depth = feature.depth
             while depth >= len(feature_orders):
                 feature_orders.append(set())
             feature_orders[depth].add(feature_map[feature.name])
 
         return feature_orders
 
-    def aggregate_over(self) -> dict[AggregateOver, set[AggregatedFeature]]:
-        features = defaultdict(set)
-        for feature in self.aggregated_features:
-            features[feature.aggregate_over].add(feature)
-        return features
-
-    def without_event_timestamp(self, name_sufix: str | None = None) -> 'RetrivalRequest':
-        return RetrivalRequest(
-            name=f'{self.name}{name_sufix or ""}',
-            location=self.location,
-            entities=self.entities,
-            features=self.features,
-            derived_features=self.derived_features,
-            aggregated_features=self.aggregated_features,
-        )
-
     @staticmethod
     def combine(requests: list['RetrivalRequest']) -> list['RetrivalRequest']:
-        grouped_requests: dict[FeatureLocation, RetrivalRequest] = {}
-        returned_features: dict[FeatureLocation, set[Feature]] = {}
+        grouped_requests: dict[str, RetrivalRequest] = {}
         entities = set()
         for request in requests:
             entities.update(request.entities)
-            fv_name = request.location
+            fv_name = request.feature_view_name
             if fv_name not in grouped_requests:
                 grouped_requests[fv_name] = RetrivalRequest(
-                    name=request.name,
-                    location=fv_name,
+                    feature_view_name=fv_name,
                     entities=request.entities,
                     features=request.features,
                     derived_features=request.derived_features,
-                    aggregated_features=request.aggregated_features,
                     event_timestamp=request.event_timestamp,
                 )
-                returned_features[fv_name] = request.returned_features
             else:
                 grouped_requests[fv_name].derived_features.update(request.derived_features)
                 grouped_requests[fv_name].features.update(request.features)
-                grouped_requests[fv_name].aggregated_features.update(request.aggregated_features)
                 grouped_requests[fv_name].entities.update(request.entities)
-                returned_features[fv_name].update(request.returned_features)
-
-        for request in grouped_requests.values():
-            request.features_to_exclude = request.features_to_exclude.union(
-                request.all_feature_names - {feature.name for feature in returned_features[request.location]}
-            )
 
         return list(grouped_requests.values())
 
     @staticmethod
     def unsafe_combine(requests: list['RetrivalRequest']) -> list['RetrivalRequest']:
 
         result_request = RetrivalRequest(
-            name=requests[0].name,
-            location=requests[0].location,
+            feature_view_name='random',
             entities=set(),
             features=set(),
             derived_features=set(),
-            aggregated_features=set(),
             event_timestamp=None,
         )
         for request in requests:
             result_request.derived_features.update(request.derived_features)
             result_request.features.update(request.features)
             result_request.entities.update(request.entities)
-            result_request.aggregated_features.update(request.aggregated_features)
 
         return result_request
 
 
 @dataclass
 class RequestResult(Codable):
     """
     Describes the returend response of a request
     """
 
     entities: set[Feature]
     features: set[Feature]
     event_timestamp: str | None
 
-    @property
-    def feature_columns(self) -> list[str]:
-        return [feature.name for feature in self.features]
-
-    @property
-    def entity_columns(self) -> list[str]:
-        return [entity.name for entity in self.entities]
-
     def __add__(self, obj: 'RequestResult') -> 'RequestResult':
         return RequestResult(
             entities=self.entities.union(obj.entities),
             features=self.features.union(obj.features),
             event_timestamp='event_timestamp' if self.event_timestamp or obj.event_timestamp else None,
         )
 
@@ -279,25 +212,18 @@
     features_to_include = {'is_male'}
     needed_requests = [
         features={'sex'}, # would fetch only the sex feature, as `is_male` relies on it
         derived_features={'is_male'} # The feature to be computed
     ]
     """
 
-    location: FeatureLocation
+    name: str
     features_to_include: set[str]
     needed_requests: list[RetrivalRequest]
 
     @property
     def needs_event_timestamp(self) -> bool:
         return any(request.event_timestamp for request in self.needed_requests)
 
     @property
     def request_result(self) -> RequestResult:
         return RequestResult.from_request_list(self.needed_requests)
-
-    def without_event_timestamp(self, name_sufix: str | None = None) -> 'FeatureRequest':
-        return FeatureRequest(
-            location=self.location,
-            features_to_include=self.features_to_include,
-            needed_requests=[request.without_event_timestamp(name_sufix) for request in self.needed_requests],
-        )
```

### Comparing `aligned-0.0.9/aligned/request/tests/test_feature_request_generation.py` & `aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from aligned import FeatureView
 
 
 @pytest.mark.asyncio
 async def test_fetch_all_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     request = compiled_view.request_all
 
     expected_features = {
         'age',
         'name',
         'sex',
         'survived',
@@ -33,15 +33,15 @@
     assert len(request.request_result.entities) == 1
     assert len(request.request_result.features) == len(expected_features)
 
 
 @pytest.mark.asyncio
 async def test_fetch_features_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     wanted_features = {'cabin', 'is_male'}
     request = compiled_view.request_for(wanted_features)
     expected_features = {'sex', 'cabin', 'is_male'}
     assert not request.needs_event_timestamp
     assert len(request.needed_requests) == 1
 
     retrival_request = request.needed_requests[0]
```

### Comparing `aligned-0.0.9/aligned/s3/config.py` & `aligned-0.0.9a0/aligned/s3/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
 
 import pandas as pd
-import polars as pl
 from httpx import HTTPStatusError
 
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.exceptions import UnableToFindFileException
 from aligned.local.job import FileDateJob, FileFullJob
 from aligned.local.source import CsvConfig, DataFileReference, ParquetConfig, StorageFileReference
 from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalRequest
@@ -46,15 +45,15 @@
     def url(self) -> str:
         import os
 
         region = os.environ[self.bucket_env]
         bucket = os.environ[self.bucket_env]
         return f'https://{region}.amazoneaws.com/{bucket}/'
 
-    def json_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
+    def file_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
         return AwsS3DataSource(config=self, path=path)
 
     def csv_at(
         self, path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
     ) -> 'AwsS3CsvDataSource':
         return AwsS3CsvDataSource(
             config=self, path=path, mapping_keys=mapping_keys or {}, csv_config=csv_config or CsvConfig()
@@ -136,23 +135,14 @@
             sep=self.csv_config.seperator,
             index=self.csv_config.should_write_index,
             compression=self.csv_config.compression,
         )
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
 
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_csv(
-            buffer,
-            sep=self.csv_config.seperator,
-        )
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
     def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         return FileFullJob(self, request=request, limit=limit)
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
     ) -> DateRangeJob:
         return FileDateJob(self, request, start_date, end_date)
@@ -185,28 +175,12 @@
             buffer = BytesIO(data)
             return pd.read_parquet(buffer)
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
-    async def to_polars(self) -> pl.LazyFrame:
-        try:
-            data = await self.storage.read(self.path)
-            buffer = BytesIO(data)
-            return pl.read_parquet(buffer).lazy()
-        except FileNotFoundError:
-            raise UnableToFindFileException()
-        except HTTPStatusError:
-            raise UnableToFindFileException()
-
     async def write_pandas(self, df: pd.DataFrame) -> None:
         buffer = BytesIO()
-        df.to_parquet(buffer, compression=self.parquet_config.compression, engine=self.parquet_config.engine)
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_parquet(buffer, compression=self.parquet_config.compression)
+        df.to_parquet(buffer)
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
```

### Comparing `aligned-0.0.9/aligned/s3/factory.py` & `aligned-0.0.9a0/aligned/s3/factory.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/s3/storage.py` & `aligned-0.0.9a0/aligned/s3/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 try:
     from aioaws.s3 import S3Client
 except ModuleNotFoundError:
 
@@ -18,43 +18,40 @@
     from aligned.s3.config import AwsS3Config
 
 
 @dataclass
 class AwsS3Storage(Storage):
 
     config: AwsS3Config
-    timeout: int = field(default=60)
 
     async def read(self, path: str) -> bytes:
         from httpx import AsyncClient
 
-        async with AsyncClient(timeout=self.timeout) as client:
+        async with AsyncClient() as client:
             s3_client = S3Client(client, self.config.s3_config)
             url = s3_client.signed_download_url(path)
             response = await client.get(url)
             response.raise_for_status()
             return response.content
 
     async def write(self, path: str, content: bytes) -> None:
         from httpx import AsyncClient
 
-        async with AsyncClient(timeout=self.timeout) as client:
+        async with AsyncClient() as client:
             s3_client = S3Client(client, self.config.s3_config)
             await s3_client.upload(path, content)
 
 
 @dataclass
 class FileStorage(Storage):
     async def read(self, path: str) -> bytes:
         return Path(path).read_bytes()
 
     async def write(self, path: str, content: bytes) -> None:
-        lib_path = Path(path)
-        lib_path.parent.mkdir(parents=True, exist_ok=True)
-        lib_path.write_bytes(content)
+        Path(path).write_bytes(content)
 
 
 @dataclass
 class HttpStorage(Storage):
     async def read(self, path: str) -> bytes:
         if not (path.startswith('http://') or path.startswith('https://')):
             raise ValueError('Invalid url')
```

### Comparing `aligned-0.0.9/aligned/schemas/constraints.py` & `aligned-0.0.9a0/aligned/schemas/constraints.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class Constraint(Codable, SerializableType):
     name: str
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def _serialize(self) -> dict:
-        assert self.name in SupportedConstraints.shared().types, f'Constraint {self.name} is not supported'
         return self.to_dict()
 
     @classmethod
     def _deserialize(cls, value: dict) -> 'Constraint':
         name_type = value['name']
         del value['name']
         data_class = SupportedConstraints.shared().types[name_type]
@@ -37,16 +36,14 @@
         for tran_type in [
             LowerBound,
             LowerBoundInclusive,
             UpperBound,
             UpperBoundInclusive,
             Required,
             InDomain,
-            MaxLength,
-            MinLength,
         ]:
             self.add(tran_type)
 
     def add(self, constraint: type[Constraint]) -> None:
         self.types[constraint.name] = constraint
 
     @classmethod
@@ -94,64 +91,14 @@
     name = 'upper_bound_inc'
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 @dataclass
-class MinLength(Constraint):
-    value: int
-
-    name = 'min_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class Regex(Constraint):
-    value: str
-
-    name = 'regex'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class EndsWith(Constraint):
-    value: str
-
-    name = 'ends_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class StartsWith(Constraint):
-    value: str
-
-    name = 'starts_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class MaxLength(Constraint):
-    value: int
-
-    name = 'max_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
 class And(Constraint):
 
     left: Constraint
     right: Constraint
     name = 'and'
 
     def __hash__(self) -> int:
```

### Comparing `aligned-0.0.9/aligned/server.py` & `aligned-0.0.9a0/aligned/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 from fastapi import FastAPI, HTTPException, Response
-from fastapi.responses import RedirectResponse
 from numpy import nan
 from pydantic import BaseModel
 
 from aligned.data_source.stream_data_source import HttpStreamSource
 from aligned.feature_source import WritableFeatureSource
 from aligned.feature_store import FeatureStore
 from aligned.schemas.feature import Feature
@@ -97,19 +96,16 @@
         async def all(limit: int | None = None) -> dict:
             df = await feature_store.feature_view(name).all(limit=limit).to_pandas()
             df.replace(nan, value=None, inplace=True)
             return df.to_dict('list')
 
     @staticmethod
     def model_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
-        from aligned.feature_store import RawStringFeatureRequest
-
-        model = feature_store.models[name]
-        features = {f'{feature.location.identifier}:{feature.name}' for feature in model.features}
-        feature_request = feature_store.requests_for(RawStringFeatureRequest(features))
+        model = feature_store.model_requests[name]
+        feature_request = feature_store.requests_for_model(model)
 
         entities: set[Feature] = set()
         for request in feature_request.needed_requests:
             entities.update(request.entities)
 
         required_features = entities.copy()
         for request in feature_request.needed_requests:
@@ -152,41 +148,28 @@
                 entity_values['event_timestamp'] = [
                     datetime.fromtimestamp(value)
                     if isinstance(value, (float, int))
                     else datetime.fromisoformat(value)
                     for value in entity_values['event_timestamp']
                 ]
 
-            df = await feature_store.model(name).features_for(entity_values).to_polars()
-            pandas_df = df.collect().to_pandas()
+            df = await feature_store.model(name).features_for(entity_values).to_pandas()
             orient = 'values'
-            body = ','.join(
-                [f'"{column}":{pandas_df[column].to_json(orient=orient)}' for column in pandas_df.columns]
-            )
+            body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
             return Response(content=f'{{{body}}}', media_type='application/json')
 
     @staticmethod
     def app(feature_store: FeatureStore) -> FastAPI:
         from asgi_correlation_id import CorrelationIdMiddleware
         from fastapi import FastAPI
         from fastapi.middleware import Middleware
-        from prometheus_fastapi_instrumentator import Instrumentator
-        from starlette.status import HTTP_200_OK
 
         app = FastAPI(middleware=[Middleware(CorrelationIdMiddleware)])
         app.docs_url = '/docs'
 
-        @app.on_event('startup')
-        async def startup():
-            Instrumentator().instrument(app).expose(app)
-
-        @app.get('health', status_code=HTTP_200_OK)
-        def health() -> None:
-            return
-
         for model in feature_store.all_models:
             FastAPIServer.model_path(model, feature_store, app)
 
         can_write_to_store = isinstance(feature_store.feature_source, WritableFeatureSource)
 
         topics: dict[str, TopicInfo] = {}
 
@@ -216,18 +199,14 @@
             logger.info(
                 (
                     'Warning! The server is not using a WritableFeatureSource, ',
                     'and can therefore not setup stream sources',
                 )
             )
 
-        @app.get('/')
-        async def root() -> RedirectResponse:
-            return RedirectResponse('/docs')
-
         @app.post('/features')
         async def features(payload: APIFeatureRequest) -> dict:
             df = await feature_store.features_for(
                 payload.entities,
                 features=payload.features,
             ).to_pandas()
             orient = 'values'
```

### Comparing `aligned-0.0.9/aligned/tests/test_cache_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_cache_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/tests/test_cached_parquet.py` & `aligned-0.0.9a0/aligned/tests/test_cached_parquet.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/tests/test_statistic_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/tests/test_transformations.py` & `aligned-0.0.9a0/aligned/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/aligned/validation/pandera.py` & `aligned-0.0.9a0/aligned/validation/pandera.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,43 @@
 import logging
 from typing import Callable
 
 import pandas as pd
-import polars as pl
 from pandera import Check, Column, DataFrameSchema  # type: ignore[attr-defined]
 
 from aligned.schemas.constraints import Constraint, Required
-from aligned.schemas.feature import Feature, FeatureType
+from aligned.schemas.feature import Feature
 from aligned.validation.interface import Validator
 
 logger = logging.getLogger(__name__)
 
 
 class PanderaValidator(Validator):
 
     check_map: dict[str, Callable[[Constraint], Check]] = {
         'lower_bound': lambda constraint: Check.greater_than(constraint.value),
         'lower_bound_inc': lambda constraint: Check.greater_than_or_equal_to(constraint.value),
         'upper_bound': lambda constraint: Check.less_than(constraint.value),
         'upper_bound_inc': lambda constraint: Check.less_than_or_equal_to(constraint.value),
         'in_domain': lambda domain: Check.isin(domain.values),
-        'min_length': lambda constraint: Check.str_length(min_value=constraint.value),
-        'max_length': lambda constraint: Check.str_length(max_value=constraint.value),
-        'regex': lambda constraint: Check.str_matches(constraint.value),
-        'ends_with': lambda constraint: Check.str_endswith(constraint.value),
-        'starts_with': lambda constraint: Check.str_startswith(constraint.value),
-    }
-
-    datatype_check = {
-        FeatureType('').bool,
-        FeatureType('').string,
-        FeatureType('').uuid,
-        FeatureType('').date,
     }
 
     def _column_for(self, feature: Feature) -> Column:
-        Check.str_matches
-
         if feature.constraints is None:
-            return Column(
-                feature.dtype.pandas_type if feature.dtype in self.datatype_check else None, nullable=True
-            )
+            return Column(feature.dtype.pandas_type, nullable=True)
 
         is_nullable = Required() not in feature.constraints
 
-        checks = [
-            self.check_map[constraint.name](constraint)
-            for constraint in feature.constraints
-            if constraint.name in self.check_map
-        ]
-
         return Column(
-            dtype=feature.dtype.pandas_type if feature.dtype in self.datatype_check else None,
-            checks=checks,
+            feature.dtype.pandas_type,
+            checks=[
+                self.check_map[constraint.name](constraint)
+                for constraint in feature.constraints
+                if constraint.name in self.check_map
+            ],
             nullable=is_nullable,
             required=not is_nullable,
         )
 
     def _build_schema(self, features: list[Feature]) -> DataFrameSchema:
         return DataFrameSchema(columns={feature.name: self._column_for(feature) for feature in features})
 
@@ -75,11 +56,7 @@
 
             if error.failure_cases['index'].iloc[0] is None:
                 raise ValueError(error)
 
             return await self.validate_pandas(
                 features, df.loc[df.index.delete(error.failure_cases['index'])].reset_index()
             )
-
-    async def validate_polars(self, features: list[Feature], df: pl.LazyFrame) -> pl.LazyFrame:
-        input_df = df.collect().to_pandas()
-        return pl.from_pandas(await self.validate_pandas(features, input_df)).lazy()
```

### Comparing `aligned-0.0.9/aligned/validation/tests/test_pandera_validator.py` & `aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.9/pyproject.toml` & `aligned-0.0.9a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligned"
-version = "0.0.9"
+version = "0.0.9a"
 description = "A scalable feature store that makes it easy to align offline and online ML systems"
 authors = ["Mats E. Mollestad <mats@mollestad.no>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/otovo/aladdin"
 repository = "https://github.com/otovo/aladdin"
 keywords = [
@@ -36,52 +36,46 @@
 ]
 packages = [
     { include = "aligned" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-dotenv = "^0.21.0"
 click = "^8.1.3"
 pandas = "^1.3.1"
 fastapi = { version = "^0.77.1", optional = true }
 uvicorn = { version = "^0.17.6", optional = true }
 redis = { version = "^4.3.1", optional = true }
 mashumaro = "^3.0.1"
 dill = "^0.3.4"
 aioaws = { version = "^0.12", optional = true }
+databases = { version = "^0.5.5", optional = true }
+asyncpg = { version = "^0.25.0", optional = true }
 pyarrow = "^8.0.0"
 Jinja2 = "^3.1.2"
 nest-asyncio = "^1.5.5"
 asgi-correlation-id = { version = "^3.0.0", optional = true }
+dask = {version = "^2022.7.0", extras = ["dataframe"], optional = true}
 pandera = {version = "^0.13.3", optional = true}
 httpx = "^0.23.0"
 polars = { version = "^0.15.6", extras = ["all"] }
-connectorx = { version = "^0.3.1", optional = true }
-pillow = { version = "^9.4.0", optional = true }
-prometheus-fastapi-instrumentator = { version="^5.9.1", optional = true }
-gensim = { version = "4.3.0", optional = true }
-openai = { version = "^0.27.2", optional = true }
-sentence-transformers = { version = "^2.2.2", optional = true }
 
 [tool.poetry.extras]
-aws = ["aioaws", "connectorx"]
-psql = ["connectorx"]
+aws = ["aioaws", "databases"]
+psql = ["databases", "asyncpg"]
 redis = ["redis"]
-server = ["asgi-correlation-id", "fastapi", "uvicorn", "prometheus-fastapi-instrumentator"]
+server = ["asgi-correlation-id", "fastapi", "uvicorn"]
+dask = ["dask"]
 pandera = ["pandera"]
-image = ["pillow"]
-text = ["gensim", "openai", "sentence-transformers"]
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.2.6"
 pytest-mock = "^3.8.1"
 freezegun = "^1.2.2"
 pytest-asyncio = "^0.20.1"
-fakeredis = "^2.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aligned = 'aligned.cli:cli'
```

### Comparing `aligned-0.0.9/PKG-INFO` & `aligned-0.0.9a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned
-Version: 0.0.9
+Version: 0.0.9a0
 Summary: A scalable feature store that makes it easy to align offline and online ML systems
 Home-page: https://github.com/otovo/aladdin
 License: Apache-2.0
 Keywords: python,typed,ml,prediction,feature,store,feature-store,feast,tecton
 Author: Mats E. Mollestad
 Author-email: mats@mollestad.no
 Requires-Python: >=3.10,<4.0
@@ -22,66 +22,49 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aws
-Provides-Extra: image
+Provides-Extra: dask
 Provides-Extra: pandera
 Provides-Extra: psql
 Provides-Extra: redis
 Provides-Extra: server
-Provides-Extra: text
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aioaws (>=0.12,<0.13) ; extra == "aws"
 Requires-Dist: asgi-correlation-id (>=3.0.0,<4.0.0) ; extra == "server"
+Requires-Dist: asyncpg (>=0.25.0,<0.26.0) ; extra == "psql"
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: connectorx (>=0.3.1,<0.4.0) ; extra == "aws" or extra == "psql"
+Requires-Dist: dask[dataframe] (>=2022.7.0,<2023.0.0) ; extra == "dask"
+Requires-Dist: databases (>=0.5.5,<0.6.0) ; extra == "aws" or extra == "psql"
 Requires-Dist: dill (>=0.3.4,<0.4.0)
 Requires-Dist: fastapi (>=0.77.1,<0.78.0) ; extra == "server"
-Requires-Dist: gensim (==4.3.0) ; extra == "text"
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: mashumaro (>=3.0.1,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0) ; extra == "text"
 Requires-Dist: pandas (>=1.3.1,<2.0.0)
 Requires-Dist: pandera (>=0.13.3,<0.14.0) ; extra == "pandera"
-Requires-Dist: pillow (>=9.4.0,<10.0.0) ; extra == "image"
 Requires-Dist: polars[all] (>=0.15.6,<0.16.0)
-Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<6.0.0) ; extra == "server"
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0) ; extra == "redis"
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "text"
 Requires-Dist: uvicorn (>=0.17.6,<0.18.0) ; extra == "server"
 Project-URL: Repository, https://github.com/otovo/aladdin
 Description-Content-Type: text/markdown
 
 # Aligned
 
 Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
 
-Main advantages:
-- Test new features faster
-- Adapt faster to new technical and business requirements.
-- Stop technology lock-in, like processing engines and infrastructure.
-- Stop vendor lock-in. Deploy to any provider that fits you
-
-As a result, loading model featurs can be done with the following code.
-
-```python
-await store.model("titanic").features_for(entities).as_pandas()
-```
-
 Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
 
 Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
 
-Aligned is still in actice development, so changes are likely.
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
 ## Feature Views
 
 Write features as the should be, as data models.
 Then get code completion and typesafety by referencing them in other features.
 
 This makes the features light weight, data source indipendent, and flexible.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

