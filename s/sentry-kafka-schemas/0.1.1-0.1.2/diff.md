# Comparing `tmp/sentry-kafka-schemas-0.1.1.tar.gz` & `tmp/sentry-kafka-schemas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.1.tar", last modified: Tue May  2 18:59:12 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.2.tar", last modified: Tue May  2 20:13:17 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.1.tar` & `sentry-kafka-schemas-0.1.2.tar`

### file list

```diff
@@ -1,119 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.748373 sentry-kafka-schemas-0.1.1/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.748373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.760373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.740373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.764373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.744373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.768373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.772373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:10.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    68329 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:10.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 18:59:06.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 18:59:09.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 18:59:08.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-02 18:59:07.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.772373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    90391 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    36710 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:59:12.752373 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 18:59:12.000000 sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:59:12.776373 sentry-kafka-schemas-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 18:58:57.000000 sentry-kafka-schemas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.437522 sentry-kafka-schemas-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:13:17.437522 sentry-kafka-schemas-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.421522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.421522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.425521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.429521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.429521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.417522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.429521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.429521 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:15.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 20:13:15.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68327 2023-05-02 20:13:14.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 20:13:13.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-02 20:13:14.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 20:13:15.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 20:13:12.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 20:13:14.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 20:13:14.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 20:13:13.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 20:13:13.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 20:13:12.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-02 20:13:12.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.433522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    90391 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36710 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.433522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.421522 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 20:13:17.000000 sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:17.437522 sentry-kafka-schemas-0.1.2/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:13:17.437522 sentry-kafka-schemas-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 20:13:03.000000 sentry-kafka-schemas-0.1.2/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.1/LICENSE` & `sentry-kafka-schemas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/README.md` & `sentry-kafka-schemas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, Dict, Literal, TypedDict
+from typing import Any, List, Dict, Literal, TypedDict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/events_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Tuple, Any, Literal, TypedDict, Union
+from typing import Literal, TypedDict, List, Tuple, Union, Any, Dict
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -98,15 +98,15 @@
     """Required property"""
 
     datetime: Required[str]
     """Required property"""
 
 
 
-EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen527235"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
+EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen88087"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
 """
 event_stream_message.
 
 The snuba eventstream message.
 """
 
 
@@ -582,15 +582,15 @@
 
 
 _BaseAnyof0 = Union[str]
 """ A "into-string" type that normalizes header names."""
 
 
 
-class _BaseGen527235(TypedDict, total=False):
+class _BaseGen88087(TypedDict, total=False):
     transaction_id: str
     project_id: Required[int]
     """Required property"""
 
     group_ids: Required[List[int]]
     """Required property"""
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, TypedDict, Literal, Any
+from typing import Dict, List, Any, TypedDict, Literal
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Literal, TypedDict, Union, List
+from typing import List, Union, TypedDict, Dict, Literal
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, TypedDict, Literal, Dict, List
+from typing import TypedDict, Literal, List, Dict, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, List, Literal, Any, Dict
+from typing import TypedDict, Dict, Any, Literal, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union, List, TypedDict, Any, Literal
+from typing import TypedDict, Any, Union, Literal, Dict, List
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Literal, TypedDict, Union
+from typing import TypedDict, Dict, Any, List, Literal, Union
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, TypedDict, Any, Dict, List
+from typing import Union, TypedDict, Dict, Any, List
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
     """clickhouse_query_profile."""
 
     time_range: Required[Union[int, None]]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, TypedDict, Literal, Dict, List
+from typing import Dict, TypedDict, Any, Literal, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union, Dict, TypedDict, Literal, Any, List
+from typing import TypedDict, List, Literal, Dict, Any, Tuple, Union
 from typing_extensions import Required
 
 
 class TransactionEvent(TypedDict, total=False):
     """transaction_event."""
 
     group_id: None
```

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.1/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.2/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 python/sentry_kafka_schemas/types.py
 python/sentry_kafka_schemas.egg-info/PKG-INFO
 python/sentry_kafka_schemas.egg-info/SOURCES.txt
 python/sentry_kafka_schemas.egg-info/dependency_links.txt
 python/sentry_kafka_schemas.egg-info/not-zip-safe
 python/sentry_kafka_schemas.egg-info/requires.txt
 python/sentry_kafka_schemas.egg-info/top_level.txt
+python/sentry_kafka_schemas/codecs/__init__.py
+python/sentry_kafka_schemas/codecs/json.py
+python/sentry_kafka_schemas/codecs/msgpack.py
 python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
 python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
 python/sentry_kafka_schemas/examples/events/1/end-merge.json
 python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
 python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
 python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
 python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
@@ -84,8 +87,15 @@
 python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
 python/sentry_kafka_schemas/topics/outcomes.yaml
 python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
 python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
 python/sentry_kafka_schemas/topics/snuba-metrics.yaml
 python/sentry_kafka_schemas/topics/snuba-queries.yaml
 python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
-python/sentry_kafka_schemas/topics/transactions.yaml
+python/sentry_kafka_schemas/topics/transactions.yaml
+python/tests/__init__.py
+python/tests/test_codecs.py
+python/tests/test_codeowner.py
+python/tests/test_examples.py
+python/tests/test_sentry_kafka_schemas.py
+python/tests/test_valid_schemas.py
+python/tests/test_valid_topic_data.py
```

