# Comparing `tmp/sentry-kafka-schemas-0.1.0.tar.gz` & `tmp/sentry-kafka-schemas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.0.tar", last modified: Tue May  2 11:32:58 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.1.tar", last modified: Tue May  2 18:59:12 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.0.tar` & `sentry-kafka-schemas-0.1.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.593242 sentry-kafka-schemas-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.581242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:56.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 11:32:56.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    69878 2023-05-02 11:32:55.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 11:32:54.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-02 11:32:55.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 11:32:56.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 11:32:54.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 11:32:55.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 11:32:56.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 11:32:55.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 11:32:54.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 11:32:54.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    28388 2023-05-02 11:32:54.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    92767 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.589242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:32:58.585242 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 11:32:58.000000 sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:32:58.593242 sentry-kafka-schemas-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 11:32:46.000000 sentry-kafka-schemas-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.748373 sentry-kafka-schemas-0.1.1/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.748373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.760373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.772373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:10.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68329 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:10.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 18:59:06.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.772373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    90391 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36710 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.752373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.0/LICENSE` & `sentry-kafka-schemas-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/README.md` & `sentry-kafka-schemas-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Any, Dict, Literal, List
+from typing import List, Dict, TypedDict, Literal, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/events_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union, Literal, List, Dict, TypedDict, Any
+from typing import Dict, List, Tuple, Any, Literal, TypedDict, Union
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -98,15 +98,15 @@
     """Required property"""
 
     datetime: Required[str]
     """Required property"""
 
 
 
-EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen507476"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
+EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen527235"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
 """
 event_stream_message.
 
 The snuba eventstream message.
 """
 
 
@@ -562,15 +562,15 @@
 
     project_id: Required[int]
     """Required property"""
 
     event_ids: Required[List[str]]
     """Required property"""
 
-    old_primary_hash: str
+    old_primary_hash: Union[str, None]
     from_timestamp: str
     to_timestamp: str
     datetime: str
 
 
 class _Base(TypedDict, total=False):
     group_states: List["_BaseGroupStatesItem"]
@@ -582,15 +582,15 @@
 
 
 _BaseAnyof0 = Union[str]
 """ A "into-string" type that normalizes header names."""
 
 
 
-class _BaseGen507476(TypedDict, total=False):
+class _BaseGen527235(TypedDict, total=False):
     transaction_id: str
     project_id: Required[int]
     """Required property"""
 
     group_ids: Required[List[int]]
     """Required property"""
 
@@ -1483,71 +1483,24 @@
 
 _SentryEventTransactionInfoAnyof0 = Union["_SentryEventTransactionInfoAnyof0Anyof0"]
 """ Additional information about the name of the transaction."""
 
 
 
 class _SentryEventTransactionInfoAnyof0Anyof0(TypedDict, total=False):
-    changes: Union[List[Union[Union["_SentryEventTransactionInfoAnyof0Anyof0ChangesArrayItemAnyof0Anyof0"], None]], None]
-    """
-     A list of changes prior to the final transaction name.
-
-     This list must be empty if the transaction name is set at the beginning of the transaction
-     and never changed. There is no placeholder entry for the initial transaction name.
-    """
-
-    original: Union[str, None]
-    """
-     The unmodified transaction name as obtained by the source.
-
-     This value will only be set if the transaction name was modified during event processing.
-    """
-
-    propagations: Union[int, None]
-    """
-     The total number of propagations during the transaction.
-
-    minimum: 0
-    """
-
-    source: Union["_SentryEventTransactionInfoAnyof0Anyof0ChangesArrayItemAnyof0Anyof0SourceAnyof0", None]
+    source: Union[str, None]
     """
      Describes how the name of the transaction was determined.
 
      This will be used by the server to decide whether or not to scrub identifiers from the
      transaction name, or replace the entire name with a placeholder.
     """
 
 
 
-class _SentryEventTransactionInfoAnyof0Anyof0ChangesArrayItemAnyof0Anyof0(TypedDict, total=False):
-    propagations: Union[int, None]
-    """
-     The number of propagations from the start of the transaction to this change.
-
-    minimum: 0
-    """
-
-    source: Union["_SentryEventTransactionInfoAnyof0Anyof0ChangesArrayItemAnyof0Anyof0SourceAnyof0", None]
-    """ Describes how the previous transaction name was determined."""
-
-    timestamp: Union["_SentryEventReceived", None]
-    """
-     Timestamp when the transaction name was changed.
-
-     This adheres to the event timestamp specification.
-    """
-
-
-
-_SentryEventTransactionInfoAnyof0Anyof0ChangesArrayItemAnyof0Anyof0SourceAnyof0 = str
-"""Describes how the name of the transaction was determined."""
-
-
-
 _SentryEventTypeAnyof0 = Union[Literal["error"], Literal["csp"], Literal["hpkp"], Literal["expectct"], Literal["expectstaple"], Literal["transaction"], Literal["default"]]
 """
 The type of an event.
 
 The event type determines how Sentry handles the event and has an impact on processing, rate limiting, and quotas. There are three fundamental classes of event types:
 
 - **Error monitoring events** (`default`, `error`): Processed and grouped into unique issues based on their exception stack traces and error messages. - **Security events** (`csp`, `hpkp`, `expectct`, `expectstaple`): Derived from Browser security violation reports and grouped into unique issues based on the endpoint and violation. SDKs do not send such events. - **Transaction events** (`transaction`): Contain operation spans and collected into traces for performance monitoring.
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Literal, Any, TypedDict
+from typing import TypedDict, List, Literal, Any, Dict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, TypedDict, List, Dict, Literal
+from typing import Dict, Literal, TypedDict, Union, List
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Dict, List, TypedDict, Any
+from typing import Any, TypedDict, Literal, Dict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, TypedDict, Dict, Any, Literal
+from typing import Any, TypedDict, Literal, Dict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Union, List, Dict, TypedDict, Any
+from typing import Dict, Union, List, TypedDict, Any, Literal
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Any, Union, Literal, TypedDict
+from typing import Any, Dict, List, Literal, TypedDict, Union
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, TypedDict, Any, Union, List
+from typing import Union, TypedDict, Any, Dict, List
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
     """clickhouse_query_profile."""
 
     time_range: Required[Union[int, None]]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Literal, Dict, List, Any
+from typing import List, Any, Dict, Literal, TypedDict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Tuple, Union, Any, Dict, Literal, List
+from typing import Tuple, Union, Dict, TypedDict, Literal, Any, List
 from typing_extensions import Required
 
 
 class TransactionEvent(TypedDict, total=False):
     """transaction_event."""
 
     group_id: None
@@ -33,25 +33,47 @@
 
 
 
 class _TransactionEventData(TypedDict, total=False):
     type: Required[str]
     """Required property"""
 
-    transaction: str
-    transaction_info: Union["_TransactionEventDataTransactionInfoAnyof0", None]
+    transaction: Union[str, None]
+    """
+     Transaction name of the event.
+
+     For example, in a web app, this might be the route name (`"/users/<username>/"` or
+     `UserView`), in a task queue it might be the function + module name.
+    """
+
+    transaction_info: "_TransactionEventDataTransactionInfo"
     timestamp: Required[Union[int, float]]
     """Required property"""
 
     start_timestamp: Required[Union[int, float]]
     """Required property"""
 
     received: Union[int, float]
-    release: str
-    environment: str
+    release: Union[str, None]
+    """
+     The release version of the application.
+
+     **Release versions must be unique across all projects in your organization.** This value
+     can be the git SHA for the given project, or a product identifier with a semantic version.
+    """
+
+    environment: Union[str, None]
+    """
+     The environment name, such as `production` or `staging`.
+
+     ```json
+     { "environment": "production" }
+     ```
+    """
+
     contexts: Required["_TransactionEventDataContexts"]
     """Required property"""
 
     tags: List[List[Union[None, str]]]
     extra: "_TransactionEventDataExtra"
     sdk: "_TransactionEventDataSdk"
     project: int
@@ -855,9 +877,21 @@
     """Required property"""
 
     hash: Required[str]
     """Required property"""
 
 
 
+_TransactionEventDataTransactionInfo = Union["_TransactionEventDataTransactionInfoAnyof0"]
+""" Additional information about the name of the transaction."""
+
+
+
 class _TransactionEventDataTransactionInfoAnyof0(TypedDict, total=False):
-    source: str
+    source: Union[str, None]
+    """
+    Describes how the name of the transaction was determined.
+
+     This will be used by the server to decide whether or not to scrub identifiers from the
+     transaction name, or replace the entire name with a placeholder.
+    """
+
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998624953078078%*

 * *Differences: {"'definitions'": "{'TombstoneEventsMessage': {'items': {2: {'properties': {'old_primary_hash': "*

 * *                  "{'type': ['string', 'null']}}}}}, 'TransactionInfo': {'anyOf': {0: "*

 * *                  "{'properties': {'source': {'type': ['string', 'null'], delete: ['anyOf']}, "*

 * *                  "delete: ['changes', 'original', 'propagations']}}}}, delete: "*

 * *                  "['TransactionNameChange']}"}*

```diff
@@ -2777,15 +2777,18 @@
                             },
                             "type": "array"
                         },
                         "from_timestamp": {
                             "type": "string"
                         },
                         "old_primary_hash": {
-                            "type": "string"
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         },
                         "project_id": {
                             "type": "integer"
                         },
                         "to_timestamp": {
                             "type": "string"
                         }
@@ -2889,103 +2892,27 @@
             "description": " A 32-character hex string as described in the W3C trace context spec."
         },
         "TransactionInfo": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
-                        "changes": {
-                            "description": " A list of changes prior to the final transaction name.\n\n This list must be empty if the transaction name is set at the beginning of the transaction\n and never changed. There is no placeholder entry for the initial transaction name.",
-                            "items": {
-                                "anyOf": [
-                                    {
-                                        "$ref": "#/definitions/TransactionNameChange"
-                                    },
-                                    {
-                                        "type": "null"
-                                    }
-                                ]
-                            },
-                            "type": [
-                                "array",
-                                "null"
-                            ]
-                        },
-                        "original": {
-                            "description": " The unmodified transaction name as obtained by the source.\n\n This value will only be set if the transaction name was modified during event processing.",
+                        "source": {
+                            "description": " Describes how the name of the transaction was determined.\n\n This will be used by the server to decide whether or not to scrub identifiers from the\n transaction name, or replace the entire name with a placeholder.",
                             "type": [
                                 "string",
                                 "null"
                             ]
-                        },
-                        "propagations": {
-                            "description": " The total number of propagations during the transaction.",
-                            "minimum": 0,
-                            "type": [
-                                "integer",
-                                "null"
-                            ]
-                        },
-                        "source": {
-                            "anyOf": [
-                                {
-                                    "$ref": "#/definitions/TransactionSource"
-                                },
-                                {
-                                    "type": "null"
-                                }
-                            ],
-                            "description": " Describes how the name of the transaction was determined.\n\n This will be used by the server to decide whether or not to scrub identifiers from the\n transaction name, or replace the entire name with a placeholder."
                         }
                     },
                     "type": "object"
                 }
             ],
             "description": " Additional information about the name of the transaction."
         },
-        "TransactionNameChange": {
-            "anyOf": [
-                {
-                    "additionalProperties": true,
-                    "properties": {
-                        "propagations": {
-                            "description": " The number of propagations from the start of the transaction to this change.",
-                            "minimum": 0,
-                            "type": [
-                                "integer",
-                                "null"
-                            ]
-                        },
-                        "source": {
-                            "anyOf": [
-                                {
-                                    "$ref": "#/definitions/TransactionSource"
-                                },
-                                {
-                                    "type": "null"
-                                }
-                            ],
-                            "description": " Describes how the previous transaction name was determined."
-                        },
-                        "timestamp": {
-                            "anyOf": [
-                                {
-                                    "$ref": "#/definitions/Timestamp"
-                                },
-                                {
-                                    "type": "null"
-                                }
-                            ],
-                            "description": " Timestamp when the transaction name was changed.\n\n This adheres to the event timestamp specification."
-                        }
-                    },
-                    "type": "object"
-                }
-            ]
-        },
         "TransactionSource": {
             "description": "Describes how the name of the transaction was determined.",
             "type": "string"
         },
         "User": {
             "anyOf": [
                 {
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998708559692318%*

 * *Differences: {"'definitions'": "{'Data': {'properties': {'transaction': {'type': ['string', 'null'], "*

 * *                  "'description': ' Transaction name of the event.\\n\\n For example, in a web "*

 * *                  'app, this might be the route name (`"/users/<username>/"` or\\n `UserView`), in '*

 * *                  "a task queue it might be the function + module name.'}, 'release': {'type': "*

 * *                  "['string', 'null'], 'description': ' The release version of the "*

 * *                  'application.\\n\\n **Re […]*

```diff
@@ -291,15 +291,19 @@
                 "contexts": {
                     "$ref": "#/definitions/Contexts"
                 },
                 "culprit": {
                     "type": "string"
                 },
                 "environment": {
-                    "type": "string"
+                    "description": " The environment name, such as `production` or `staging`.\n\n ```json\n { \"environment\": \"production\" }\n ```",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "extra": {
                     "$ref": "#/definitions/Extra"
                 },
                 "location": {
                     "type": "string"
                 },
@@ -309,15 +313,19 @@
                 "project": {
                     "type": "integer"
                 },
                 "received": {
                     "type": "number"
                 },
                 "release": {
-                    "type": "string"
+                    "description": " The release version of the application.\n\n **Release versions must be unique across all projects in your organization.** This value\n can be the git SHA for the given project, or a product identifier with a semantic version.",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "sdk": {
                     "$ref": "#/definitions/SDK"
                 },
                 "spans": {
                     "items": {
                         "$ref": "#/definitions/Span"
@@ -346,15 +354,19 @@
                 "timestamp": {
                     "type": "number"
                 },
                 "title": {
                     "type": "string"
                 },
                 "transaction": {
-                    "type": "string"
+                    "description": " Transaction name of the event.\n\n For example, in a web app, this might be the route name (`\"/users/<username>/\"` or\n `UserView`), in a task queue it might be the function + module name.",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "transaction_info": {
                     "$ref": "#/definitions/TransactionInfo"
                 },
                 "type": {
                     "type": "string"
                 }
@@ -1366,25 +1378,28 @@
             "required": [],
             "title": "transaction_event",
             "type": "object"
         },
         "TransactionInfo": {
             "anyOf": [
                 {
+                    "additionalProperties": true,
                     "properties": {
                         "source": {
-                            "type": "string"
+                            "description": "Describes how the name of the transaction was determined.\n\n This will be used by the server to decide whether or not to scrub identifiers from the\n transaction name, or replace the entire name with a placeholder.",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
                         }
                     },
                     "type": "object"
-                },
-                {
-                    "type": "null"
                 }
-            ]
+            ],
+            "description": " Additional information about the name of the transaction."
         }
     },
     "items": [
         {
             "const": 2
         },
         {
```

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.0/setup.py` & `sentry-kafka-schemas-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.0",
+    version="0.1.1",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=["sentry_kafka_schemas", "sentry_kafka_schemas.schema_types"],
```

