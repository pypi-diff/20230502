# Comparing `tmp/ddapm-test-agent-1.8.0.tar.gz` & `tmp/ddapm-test-agent-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddapm-test-agent-1.8.0.tar", last modified: Thu Mar 23 21:07:30 2023, max compression
+gzip compressed data, was "ddapm-test-agent-1.9.0.tar", last modified: Tue May  2 14:34:18 2023, max compression
```

## Comparing `ddapm-test-agent-1.8.0.tar` & `ddapm-test-agent-1.9.0.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.438279 ddapm-test-agent-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.438279 ddapm-test-agent-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/LICENSE.apache2
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.442279 ddapm-test-agent-1.8.0/ddapm_test_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/apmtelemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/fmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/remoteconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/trace_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/trace_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/tracestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/ddapm_test_agent/tracestats_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.442279 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 21:07:30.000000 ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.442279 ddapm-test-agent-1.8.0/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/1.0-e192f5064e917083.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/Add-metrics.process_id-to-ignored-attributes-62b264f0ea591326.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/add-distributed-trace-c35a314698a3b966.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/add-fmt-command-cc31769942a5fec3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/add-rcm-endpoints-7e1f949e83e21039.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/add-support-telemetry-requests-10737cd3da802ca6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/args-88f664c83a96075d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/check-http-header-sensitivity-daaa9d9595ae86d6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/content_length-e1bab75580aa1dcb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/docker-arm64-images-a4b6b2cc527327d6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/fix-fmt-logging-6a323fd8d5d4eb28.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/fix-matching-319744b82d2514c1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/fix-partial-chunks-0db14ce3017e6173.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/fix-racecondition-9bd0ef15b7da60fa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/info-34dcd9cbcc382487.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/info-drop-p0s-c207889f590340fb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/new-process-id-tag-f0ab0daf652e05cc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/profiling-endpoint-0cd209e4e5b6cfc0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/proxy-37c94e2fb428c6fc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/python-support-1c447acc4607abc7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/python310-025fbc190363de98.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/python310-docker-image-d4e329cfecf6510e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/reuse-session-1670aa569907cf68.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/session-requests-b8057811f976220e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-cmds-de4a561911afee11.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-empty-maps-2cbe8cea3e7112fa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-error-messages-de41d9e3207fa30a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-filename-c068de1bc3e50c04.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-order-type-2d6424e380b2c88f.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/snapshot-parent-id-7abb860008702e70.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/span-ordering-1a7b383aa015bddc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/span-parent-id-a4d7d63fa623361c.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/throttling-590bf58ecb3cc4a5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/trace-stats-97da3a478dabfa99.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/trace-stats-snapshot-718ca37385c93e1e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/traces-endpoint-f4f9c1d94d6ceda2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/tracestats-fixes-07152c708e73ef96.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/tracestats-post-65ce788f81862532.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/tracestats-service-2a0a178cbd21b07d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/uds-64b11960931d8b77.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/uds-permissions-903266ac6445b873.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/v0.5-traces-cf469b0b71398d97.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/releasenotes/notes/version-0c32d2752f154eb9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/riotfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/scripts/check-releasenotes
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-23 21:07:30.450279 ddapm-test-agent-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/test_deps.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:07:30.446279 ddapm-test-agent-1.8.0/tests/integration_snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_multi_trace.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_single_trace.json
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_distributed_propagated.json
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_distributed_same_payload.json
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_missing_received.json
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_stats_tracestats.json
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_apmtelemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_remoteconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_snapshot_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/test_tracestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-23 21:07:25.000000 ddapm-test-agent-1.8.0/tests/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.598415 ddapm-test-agent-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.586415 ddapm-test-agent-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.586415 ddapm-test-agent-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/LICENSE.apache2
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-05-02 14:34:18.598415 ddapm-test-agent-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.590415 ddapm-test-agent-1.9.0/ddapm_test_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35163 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/apmtelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/remoteconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/trace_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/trace_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/tracestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/ddapm_test_agent/tracestats_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.590415 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 14:34:18.000000 ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.590415 ddapm-test-agent-1.9.0/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.594415 ddapm-test-agent-1.9.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/1.0-e192f5064e917083.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/Add-metrics.process_id-to-ignored-attributes-62b264f0ea591326.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-distributed-trace-c35a314698a3b966.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-fmt-command-cc31769942a5fec3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-optional-json-parser-10aac54bd1cbe322.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-rcm-endpoints-7e1f949e83e21039.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-session-to-rcm-endpoints-d97e925a04a99a65.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/add-support-telemetry-requests-10737cd3da802ca6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/args-88f664c83a96075d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/change-trace-proxy-headers-f9fcbb4efc4fcb95.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/check-http-header-sensitivity-daaa9d9595ae86d6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/content_length-e1bab75580aa1dcb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/docker-arm64-images-a4b6b2cc527327d6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/fix-fmt-logging-6a323fd8d5d4eb28.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/fix-matching-319744b82d2514c1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/fix-partial-chunks-0db14ce3017e6173.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/fix-racecondition-9bd0ef15b7da60fa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/improve-test-agent-debugging-5759413f1fc5f7fa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/improve-test-agent-proxying-a207f0fc81b3ab2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/info-34dcd9cbcc382487.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/info-drop-p0s-c207889f590340fb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/new-process-id-tag-f0ab0daf652e05cc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/profiling-endpoint-0cd209e4e5b6cfc0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/proxy-37c94e2fb428c6fc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/python-support-1c447acc4607abc7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/python310-025fbc190363de98.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/python310-docker-image-d4e329cfecf6510e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/reuse-session-1670aa569907cf68.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/session-requests-b8057811f976220e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-cmds-de4a561911afee11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-empty-maps-2cbe8cea3e7112fa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-error-messages-de41d9e3207fa30a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-filename-c068de1bc3e50c04.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-order-type-2d6424e380b2c88f.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/snapshot-parent-id-7abb860008702e70.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/span-ordering-1a7b383aa015bddc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/span-parent-id-a4d7d63fa623361c.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/throttling-590bf58ecb3cc4a5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/trace-stats-97da3a478dabfa99.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/trace-stats-snapshot-718ca37385c93e1e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/traces-endpoint-f4f9c1d94d6ceda2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/tracestats-fixes-07152c708e73ef96.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/tracestats-post-65ce788f81862532.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/tracestats-service-2a0a178cbd21b07d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/uds-64b11960931d8b77.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/uds-permissions-903266ac6445b873.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/v0.5-traces-cf469b0b71398d97.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/releasenotes/notes/version-0c32d2752f154eb9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/riotfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.594415 ddapm-test-agent-1.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/scripts/check-releasenotes
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 14:34:18.598415 ddapm-test-agent-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/test_deps.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.598415 ddapm-test-agent-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:34:18.598415 ddapm-test-agent-1.9.0/tests/integration_snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_multi_trace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_single_trace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_distributed_propagated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_distributed_same_payload.json
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_missing_received.json
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_stats_tracestats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_apmtelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_remoteconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_snapshot_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/test_tracestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-02 14:34:10.000000 ddapm-test-agent-1.9.0/tests/trace_utils.py
```

### Comparing `ddapm-test-agent-1.8.0/.github/workflows/changelog.yml` & `ddapm-test-agent-1.9.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/.github/workflows/docker.yml` & `ddapm-test-agent-1.9.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/.github/workflows/main.yml` & `ddapm-test-agent-1.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/.github/workflows/publish_pypi.yml` & `ddapm-test-agent-1.9.0/.github/workflows/publish_pypi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   release:
     types:
       - published
 
 jobs:
   build_wheel:
     name: Build wheels
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
         # Include all history and tags
         with:
           fetch-depth: 0
```

### Comparing `ddapm-test-agent-1.8.0/LICENSE.BSD3` & `ddapm-test-agent-1.9.0/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/LICENSE.apache2` & `ddapm-test-agent-1.9.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/PKG-INFO` & `ddapm-test-agent-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddapm-test-agent
-Version: 1.8.0
+Version: 1.9.0
 Summary: Test agent for Datadog APM client libraries
 Home-page: https://github.com/Datadog/dd-apm-test-agent
 Author: Kyle Verhoog
 Author-email: kyle@verhoog.ca
 License: BSD 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -101,14 +101,17 @@
 ### Proxy
 
 The test agent provides proxying to the Datadog agent. 
 This is enabled by passing the agent url to the test agent either via the `--agent-url` command-line argument or by the `DD_TRACE_AGENT_URL` or `DD_AGENT_URL` environment variables.
 
 When proxying is enabled, the response from the Datadog agent will be returned instead of one from the test agent.
 
+At the trace-level, proxying can also be disabled by including the `X-Datadog-Agent-Proxy-Disabled` header with a value of `true`. This will disable proxying after a trace 
+is handled, regardless of whether an agent URL is set.
+
 
 ### Snapshot testing
 
 The test agent provides a form of [characterization testing](https://en.wikipedia.org/wiki/Characterization_test) which
 we refer to as snapshotting. 
 This allows library maintainers to ensure that traces don't change unexpectedly when making unrelated changes.
 
@@ -185,14 +188,17 @@
 - `SNAPSHOT_IGNORED_ATTRS` [`"span_id,trace_id,parent_id,duration,start,metrics.system.pid,metrics.process_id,metrics.system.process_id,meta.runtime-id"`]: The
   attributes to ignore when comparing spans in snapshots.
 
 - `DD_AGENT_URL` [`""`]: URL to a Datadog agent. When provided requests will be proxied to the agent.
 
 - `DD_APM_RECEIVER_SOCKET` [`""`]: When provided, the test agent will listen for traces on a socket at the path provided (e.g., `/var/run/datadog/apm.socket`)
 
+- `DD_SUPPRESS_TRACE_PARSE_ERRORS` [`false`]: Set to `"True"` to disable span parse errors when decoding handled traces. When disabled, errors will not be thrown for
+metrics incorrectly placed within the meta field, or other type errors related to span tag formatting/types. Can also be set using the `--suppress-trace-parse-errors=True` option.
+
 
 
 ## API
 
 ### /test/traces
 
 Return traces that have been received by the agent. Traces matching specific trace ids can be requested with the options
@@ -301,24 +307,30 @@
 #### [optional] `X-Datadog-Test-Session-Token`
 
 Stats are returned as a JSON list of the stats payloads received.
 
 ## /test/session/responses/config (POST)
 Create a Remote Config payload to retrieve in endpoint `/v0.7/config`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"roots": ["eyJ....fX0="], "targets": "ey...19", "target_files": [{"path": "datadog/2/ASM_DATA/blocked_users/config", "raw": "eyJydWxlc19kYXRhIjogW119"}], "client_configs": ["datadog/2/ASM_DATA/blocked_users/config"]}'
 ```
 
 ## /test/session/responses/config/path (POST)
 Due to Remote Config payload being quite complicated, this endpoint works like `/test/session/responses/config (POST)` 
 but you should send a path and a message and this endpoint builds the Remote Config payload.
 
 The keys of the JSON body are `path` and `msg`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"path": "datadog/2/ASM_DATA/blocked_users/config", "msg": {"rules_data": []}}'
 ```
 
 ## Development
 
 ### Prerequisites
```

### Comparing `ddapm-test-agent-1.8.0/README.md` & `ddapm-test-agent-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 ### Proxy
 
 The test agent provides proxying to the Datadog agent. 
 This is enabled by passing the agent url to the test agent either via the `--agent-url` command-line argument or by the `DD_TRACE_AGENT_URL` or `DD_AGENT_URL` environment variables.
 
 When proxying is enabled, the response from the Datadog agent will be returned instead of one from the test agent.
 
+At the trace-level, proxying can also be disabled by including the `X-Datadog-Agent-Proxy-Disabled` header with a value of `true`. This will disable proxying after a trace 
+is handled, regardless of whether an agent URL is set.
+
 
 ### Snapshot testing
 
 The test agent provides a form of [characterization testing](https://en.wikipedia.org/wiki/Characterization_test) which
 we refer to as snapshotting. 
 This allows library maintainers to ensure that traces don't change unexpectedly when making unrelated changes.
 
@@ -166,14 +169,17 @@
 - `SNAPSHOT_IGNORED_ATTRS` [`"span_id,trace_id,parent_id,duration,start,metrics.system.pid,metrics.process_id,metrics.system.process_id,meta.runtime-id"`]: The
   attributes to ignore when comparing spans in snapshots.
 
 - `DD_AGENT_URL` [`""`]: URL to a Datadog agent. When provided requests will be proxied to the agent.
 
 - `DD_APM_RECEIVER_SOCKET` [`""`]: When provided, the test agent will listen for traces on a socket at the path provided (e.g., `/var/run/datadog/apm.socket`)
 
+- `DD_SUPPRESS_TRACE_PARSE_ERRORS` [`false`]: Set to `"True"` to disable span parse errors when decoding handled traces. When disabled, errors will not be thrown for
+metrics incorrectly placed within the meta field, or other type errors related to span tag formatting/types. Can also be set using the `--suppress-trace-parse-errors=True` option.
+
 
 
 ## API
 
 ### /test/traces
 
 Return traces that have been received by the agent. Traces matching specific trace ids can be requested with the options
@@ -282,24 +288,30 @@
 #### [optional] `X-Datadog-Test-Session-Token`
 
 Stats are returned as a JSON list of the stats payloads received.
 
 ## /test/session/responses/config (POST)
 Create a Remote Config payload to retrieve in endpoint `/v0.7/config`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"roots": ["eyJ....fX0="], "targets": "ey...19", "target_files": [{"path": "datadog/2/ASM_DATA/blocked_users/config", "raw": "eyJydWxlc19kYXRhIjogW119"}], "client_configs": ["datadog/2/ASM_DATA/blocked_users/config"]}'
 ```
 
 ## /test/session/responses/config/path (POST)
 Due to Remote Config payload being quite complicated, this endpoint works like `/test/session/responses/config (POST)` 
 but you should send a path and a message and this endpoint builds the Remote Config payload.
 
 The keys of the JSON body are `path` and `msg`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"path": "datadog/2/ASM_DATA/blocked_users/config", "msg": {"rules_data": []}}'
 ```
 
 ## Development
 
 ### Prerequisites
```

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/agent.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 from typing import Awaitable
 from typing import Callable
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Set
 from typing import cast
+from urllib.parse import urlparse
+from urllib.parse import urlunparse
 
 from aiohttp import ClientSession
 from aiohttp import web
 from aiohttp.web import Request
 from aiohttp.web import middleware
+from msgpack.exceptions import ExtraData as MsgPackExtraDataException
+from multidict import CIMultiDict
 
 from . import _get_version
 from . import trace_snapshot
 from . import tracestats_snapshot
 from .apmtelemetry import TelemetryEvent
 from .apmtelemetry import v2_decode as v2_apmtelemetry_decode
 from .checks import CheckTrace
@@ -104,14 +108,25 @@
     The token is retrieved from the headers or params of the request.
     """
     token = _session_token(request)
     request["session_token"] = token
     return await handler(request)
 
 
+def update_trace_agent_port(url, new_port):
+    # Updates the Agent URL with a new port number, returning the updated URL and old port
+    parsed_url = urlparse(url)
+    old_port = parsed_url.port
+    new_netloc = parsed_url.netloc.replace(f":{old_port}", f":{new_port}")
+    new_url = urlunparse(
+        (parsed_url.scheme, new_netloc, parsed_url.path, parsed_url.params, parsed_url.query, parsed_url.fragment)
+    )
+    return new_url
+
+
 class Agent:
     def __init__(self):
         """Only store the requests sent to the agent. There are many representations
         of data but typically information is lost while transforming the data.
 
         Storing exactly what is sent to the agent enables us to transform the data
         however we desire later on.
@@ -240,15 +255,15 @@
                 s = self._decode_v06_tracestats(req)
                 stats.append(s)
         return stats
 
     def _decode_v04_traces(self, request: Request) -> v04TracePayload:
         content_type = request.content_type
         raw_data = self._request_data(request)
-        return trace_decode_v04(content_type, raw_data)
+        return trace_decode_v04(content_type, raw_data, request.app["suppress_trace_parse_errors"])
 
     def _decode_v05_traces(self, request: Request) -> v04TracePayload:
         raw_data = self._request_data(request)
         return trace_decode_v05(raw_data)
 
     def _decode_v06_tracestats(self, request: Request) -> v06StatsPayload:
         raw_data = self._request_data(request)
@@ -270,39 +285,43 @@
             "s" if nstats else "",
         )
         return web.HTTPOk()
 
     async def handle_v07_remoteconfig(self, request: Request) -> web.Response:
         """Emulates Remote Config endpoint: /v0.7/config"""
         await self._store_request(request)
-        data = await self._rc_server.get_config_response()
+        token = _session_token(request)
+        data = await self._rc_server.get_config_response(token)
         return web.json_response(data)
 
     async def handle_v07_remoteconfig_create(self, request: Request) -> web.Response:
         """Configure the response payload of /v0.7/config."""
         raw_data = await request.read()
-        self._rc_server.create_config_response(json.loads(raw_data))
+        token = _session_token(request)
+        self._rc_server.create_config_response(token, json.loads(raw_data))
         return web.HTTPAccepted()
 
     async def handle_v07_remoteconfig_path_create(self, request: Request) -> web.Response:
         """
         Remote Config payloads are quite complex. This endpoints builds a remote config payload with a target
         file path and the content of it (msg)
         """
         raw_data = await request.read()
         content = json.loads(raw_data)
         path = content["path"]
         msg = content["msg"]
-        self._rc_server.create_config_path_response(path, msg)
+        token = _session_token(request)
+        self._rc_server.create_config_path_response(token, path, msg)
         return web.HTTPAccepted()
 
     async def handle_v07_remoteconfig_put(self, request: Request) -> web.Response:
         """Configure the response payload of /v0.7/config"""
         raw_data = await request.read()
-        self._rc_server.update_config_response(json.loads(raw_data))
+        token = _session_token(request)
+        self._rc_server.update_config_response(token, json.loads(raw_data))
         return web.HTTPAccepted()
 
     async def handle_v2_apmtelemetry(self, request: Request) -> web.Response:
         await self._store_request(request)
         v2_apmtelemetry_decode(self._request_data(request))
         # TODO: Validation
         # TODO: Snapshots
@@ -321,66 +340,113 @@
                 ],
                 "feature_flags": [],
                 "config": {},
                 "client_drop_p0s": True,
             }
         )
 
+    async def _proxy_request(self, request, headers, agent_url):
+        async with ClientSession() as session:
+            async with session.post(
+                f"{agent_url}/v0.4/traces",
+                headers=headers,
+                data=self._request_data(request),
+            ) as resp:
+                assert resp.status == 200, f"Request to agent unsuccessful, received [{resp.status}] response."
+
+                if "text/html" in resp.content_type:
+                    data = await resp.read()
+                    if len(data) == 0:
+                        log.info("Received empty response: %r from agent.", data)
+                        return web.HTTPOk()
+                    else:
+                        if isinstance(data, bytes):
+                            data = data.decode()
+                        try:
+                            response_data = json.loads(data)
+                        except json.JSONDecodeError as e:
+                            log.warning("Error decoding response data: %s, data=%r", str(e), data)
+                            log.warning("Original Request: %r", self._request_data(request))
+                            response_data = {}
+                        log.info("Response %r from agent:", data)
+                        return web.json_response(data=response_data)
+                else:
+                    data = await resp.json()
+                    log.info("Response %r from agent:", data)
+                    return web.json_response(data=data)
+
     async def _handle_traces(self, request: Request, version: Literal["v0.4", "v0.5"]) -> web.Response:
         await self._store_request(request)
         token = request["session_token"]
         checks: Checks = request.app["checks"]
+        headers = CIMultiDict(request.headers)
+
+        log.debug(f"New request: {request} with headers: {headers}")
+        log.debug(f"Request Data: {self._request_data(request)!r}")
+
+        agent_url = request.app["agent_url"]
+        response = None
+        proxy_to_agent = agent_url != ""
+
+        if "X-Datadog-Agent-Proxy-Disabled" in headers:
+            proxy_to_agent = headers.pop("X-Datadog-Agent-Proxy-Disabled").lower() != "true"
+
+        if "X-Datadog-Proxy-Port" in headers:
+            port = headers.pop("X-Datadog-Proxy-Port")
+            request.app["agent_url"] = update_trace_agent_port(request.app["agent_url"], new_port=port)
+            agent_url = request.app["agent_url"]
+            log.info("Found port in headers, new trace agent URL is: {}".format(request.app["agent_url"]))
+
+        if agent_url and proxy_to_agent:
+            headers = {
+                "Content-Type": headers.get("Content-Type", "application/msgpack"),
+                **{k: v for k, v in headers.items() if k.lower() not in ["content-type", "host", "transfer-encoding"]},
+            }
+            log.info("Forwarding request to agent at %r", agent_url)
+            log.debug(f"Using headers: {headers}")
+            response = await self._proxy_request(request, headers, agent_url)
 
-        await checks.check("trace_stall", headers=request.headers, request=request)
+        await checks.check("trace_stall", headers=headers, request=request)
 
         with CheckTrace.add_frame("headers") as f:
-            f.add_item(pprint.pformat(dict(request.headers)))
-            await checks.check("meta_tracer_version_header", headers=request.headers)
-            await checks.check("trace_content_length", headers=request.headers)
-
-            if version == "v0.4":
-                traces = self._decode_v04_traces(request)
-            elif version == "v0.5":
-                traces = self._decode_v05_traces(request)
-            log.info(
-                "received trace for token %r payload with %r trace chunks",
-                token,
-                len(traces),
-            )
-            for i, trace in enumerate(traces):
-                try:
-                    log.info(
-                        "Chunk %d\n%s",
-                        i,
-                        pprint_trace(trace, request.app["log_span_fmt"]),
-                    )
-                except ValueError:
-                    log.info("Chunk %d could not be displayed (might be incomplete).", i)
-            log.info("end of payload %s", "-" * 40)
-
-            with CheckTrace.add_frame(f"payload ({len(traces)} traces)"):
-                await checks.check(
-                    "trace_count_header",
-                    headers=request.headers,
-                    num_traces=len(traces),
+            f.add_item(pprint.pformat(dict(headers)))
+            await checks.check("meta_tracer_version_header", headers=headers)
+            await checks.check("trace_content_length", headers=headers)
+
+            try:
+                if version == "v0.4":
+                    traces = self._decode_v04_traces(request)
+                elif version == "v0.5":
+                    traces = self._decode_v05_traces(request)
+                log.info(
+                    "received trace for token %r payload with %r trace chunks",
+                    token,
+                    len(traces),
                 )
-
-        agent_url = request.app["agent_url"]
+                for i, trace in enumerate(traces):
+                    try:
+                        log.info(
+                            "Chunk %d\n%s",
+                            i,
+                            pprint_trace(trace, request.app["log_span_fmt"]),
+                        )
+                    except ValueError:
+                        log.info("Chunk %d could not be displayed (might be incomplete).", i)
+                log.info("end of payload %s", "-" * 40)
+
+                with CheckTrace.add_frame(f"payload ({len(traces)} traces)"):
+                    await checks.check(
+                        "trace_count_header",
+                        headers=headers,
+                        num_traces=len(traces),
+                    )
+            except MsgPackExtraDataException as e:
+                log.error(f"Error unpacking trace bytes with Msgpack: {str(e)}, error {e}")
         if agent_url:
-            log.info("Forwarding request to agent at %r", agent_url)
-            async with ClientSession() as session:
-                async with session.post(
-                    f"{agent_url}/v0.4/traces",
-                    headers=request.headers,
-                    data=self._request_data(request),
-                ) as resp:
-                    assert resp.status == 200
-                    data = await resp.json()
-                    log.info("Got response %r from agent", data)
-                    return web.json_response(data=data)
+            return response
 
         # TODO: implement sampling logic
         return web.json_response(data={"rate_by_service": {}})
 
     async def handle_session_start(self, request: Request) -> web.Response:
         self._requests.append(request)
         return web.HTTPOk()
@@ -591,14 +657,15 @@
     disabled_checks: List[str],
     log_span_fmt: str,
     snapshot_dir: str,
     snapshot_ci_mode: bool,
     snapshot_ignored_attrs: List[str],
     agent_url: str,
     trace_request_delay: float,
+    suppress_trace_parse_errors: bool,
 ) -> web.Application:
     agent = Agent()
     app = web.Application(
         client_max_size=int(100e6),  # 100MB - arbitrary
         middlewares=[
             check_failure_middleware,
             session_token_middleware,
@@ -644,14 +711,15 @@
     app["checks"] = checks
     app["snapshot_dir"] = snapshot_dir
     app["snapshot_ci_mode"] = snapshot_ci_mode
     app["log_span_fmt"] = log_span_fmt
     app["snapshot_ignored_attrs"] = snapshot_ignored_attrs
     app["agent_url"] = agent_url
     app["trace_request_delay"] = trace_request_delay
+    app["suppress_trace_parse_errors"] = suppress_trace_parse_errors
     return app
 
 
 def main(args: Optional[List[str]] = None) -> None:
     if args is None:
         args = sys.argv[1:]
     parser = argparse.ArgumentParser(
@@ -724,14 +792,22 @@
     )
     parser.add_argument(
         "--trace-request-delay",
         type=float,
         default=os.environ.get("DD_TEST_STALL_REQUEST_SECONDS", 0.0),
         help=("Will stall trace requests for specified amount of time"),
     )
+    parser.add_argument(
+        "--suppress-trace-parse-errors",
+        type=bool,
+        default=os.environ.get("DD_SUPPRESS_TRACE_PARSE_ERRORS", False),
+        help=(
+            "Will change the test agent trace decoder to use a more resilient parser to prevent decode and span verification errors"
+        ),
+    )
     parsed_args = parser.parse_args(args=args)
     logging.basicConfig(level=parsed_args.log_level)
 
     if parsed_args.version:
         print(_get_version())
         sys.exit(0)
 
@@ -756,14 +832,15 @@
         disabled_checks=parsed_args.disabled_checks,
         log_span_fmt=parsed_args.log_span_fmt,
         snapshot_dir=parsed_args.snapshot_dir,
         snapshot_ci_mode=parsed_args.snapshot_ci_mode,
         snapshot_ignored_attrs=parsed_args.snapshot_ignored_attrs,
         agent_url=parsed_args.agent_url,
         trace_request_delay=parsed_args.trace_request_delay,
+        suppress_trace_parse_errors=parsed_args.suppress_trace_parse_errors,
     )
 
     web.run_app(app, sock=apm_sock, port=parsed_args.port)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/checks.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/checks.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/cmd.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/cmd.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/fmt.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/fmt.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/remoteconfig.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/remoteconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from typing import Any
 from typing import Dict
 
 
 class RemoteConfigServer:
     _responses: Dict[str, Any] = {}
 
-    def _update_response(self, endpoint_key: str, data: Dict[str, Any]) -> None:
-        if self._responses.get(endpoint_key):
-            self._responses[endpoint_key].update(data)
+    def _update_response(self, token: str, data: Dict[str, Any]) -> None:
+        if self._responses.get(token):
+            self._responses[token].update(data)
         else:
-            self._create_response(endpoint_key, data)
+            self._create_response(token, data)
 
-    def _create_response(self, endpoint_key: str, data: Dict[str, Any]) -> None:
-        self._responses[endpoint_key] = data
+    def _create_response(self, token: str, data: Dict[str, Any]) -> None:
+        self._responses[token] = data
 
-    async def _get_response(self, endpoint_key: str) -> Dict[str, Any]:
-        return self._responses.get(endpoint_key, {})
+    async def _get_response(self, token: str) -> Dict[str, Any]:
+        return self._responses.get(token, {})
 
-    def update_config_response(self, data: Dict[str, Any]) -> None:
-        self._update_response("config", data)
+    def update_config_response(self, token: str, data: Dict[str, Any]) -> None:
+        self._update_response(token, data)
 
     @staticmethod
     def _build_config_path_response(path: str, msg: str) -> Dict[str, Any]:
         expires_date = datetime.datetime.strftime(
             datetime.datetime.now() + datetime.timedelta(days=1), "%Y-%m-%dT%H:%M:%SZ"
         )
         msg_enc = bytes(json.dumps(msg), encoding="utf-8")
@@ -79,16 +79,16 @@
                     "raw": str(base64.b64encode(msg_enc), encoding="utf-8"),
                 }
             ],
             "client_configs": [path],
         }
         return remote_config_payload
 
-    def create_config_path_response(self, path: str, msg: str) -> None:
+    def create_config_path_response(self, token: str, path: str, msg: str) -> None:
         remote_config_payload = self._build_config_path_response(path, msg)
-        self.create_config_response(remote_config_payload)
+        self.create_config_response(token, remote_config_payload)
 
-    def create_config_response(self, data: Dict[str, Any]) -> None:
-        self._create_response("config", data)
+    def create_config_response(self, token: str, data: Dict[str, Any]) -> None:
+        self._create_response(token, data)
 
-    async def get_config_response(self) -> Dict[str, Any]:
-        return await self._get_response("config")
+    async def get_config_response(self, token: str) -> Dict[str, Any]:
+        return await self._get_response(token)
```

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/trace_checks.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/trace_checks.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/trace_snapshot.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/trace_snapshot.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/tracestats.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/tracestats.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent/tracestats_snapshot.py` & `ddapm-test-agent-1.9.0/ddapm_test_agent/tracestats_snapshot.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/PKG-INFO` & `ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddapm-test-agent
-Version: 1.8.0
+Version: 1.9.0
 Summary: Test agent for Datadog APM client libraries
 Home-page: https://github.com/Datadog/dd-apm-test-agent
 Author: Kyle Verhoog
 Author-email: kyle@verhoog.ca
 License: BSD 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -101,14 +101,17 @@
 ### Proxy
 
 The test agent provides proxying to the Datadog agent. 
 This is enabled by passing the agent url to the test agent either via the `--agent-url` command-line argument or by the `DD_TRACE_AGENT_URL` or `DD_AGENT_URL` environment variables.
 
 When proxying is enabled, the response from the Datadog agent will be returned instead of one from the test agent.
 
+At the trace-level, proxying can also be disabled by including the `X-Datadog-Agent-Proxy-Disabled` header with a value of `true`. This will disable proxying after a trace 
+is handled, regardless of whether an agent URL is set.
+
 
 ### Snapshot testing
 
 The test agent provides a form of [characterization testing](https://en.wikipedia.org/wiki/Characterization_test) which
 we refer to as snapshotting. 
 This allows library maintainers to ensure that traces don't change unexpectedly when making unrelated changes.
 
@@ -185,14 +188,17 @@
 - `SNAPSHOT_IGNORED_ATTRS` [`"span_id,trace_id,parent_id,duration,start,metrics.system.pid,metrics.process_id,metrics.system.process_id,meta.runtime-id"`]: The
   attributes to ignore when comparing spans in snapshots.
 
 - `DD_AGENT_URL` [`""`]: URL to a Datadog agent. When provided requests will be proxied to the agent.
 
 - `DD_APM_RECEIVER_SOCKET` [`""`]: When provided, the test agent will listen for traces on a socket at the path provided (e.g., `/var/run/datadog/apm.socket`)
 
+- `DD_SUPPRESS_TRACE_PARSE_ERRORS` [`false`]: Set to `"True"` to disable span parse errors when decoding handled traces. When disabled, errors will not be thrown for
+metrics incorrectly placed within the meta field, or other type errors related to span tag formatting/types. Can also be set using the `--suppress-trace-parse-errors=True` option.
+
 
 
 ## API
 
 ### /test/traces
 
 Return traces that have been received by the agent. Traces matching specific trace ids can be requested with the options
@@ -301,24 +307,30 @@
 #### [optional] `X-Datadog-Test-Session-Token`
 
 Stats are returned as a JSON list of the stats payloads received.
 
 ## /test/session/responses/config (POST)
 Create a Remote Config payload to retrieve in endpoint `/v0.7/config`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"roots": ["eyJ....fX0="], "targets": "ey...19", "target_files": [{"path": "datadog/2/ASM_DATA/blocked_users/config", "raw": "eyJydWxlc19kYXRhIjogW119"}], "client_configs": ["datadog/2/ASM_DATA/blocked_users/config"]}'
 ```
 
 ## /test/session/responses/config/path (POST)
 Due to Remote Config payload being quite complicated, this endpoint works like `/test/session/responses/config (POST)` 
 but you should send a path and a message and this endpoint builds the Remote Config payload.
 
 The keys of the JSON body are `path` and `msg`
 
+#### [optional] `?test_session_token=`
+#### [optional] `X-Datadog-Test-Session-Token`
+
 ```
 curl -X POST 'http://0.0.0.0:8126/test/session/responses/config/path' -d '{"path": "datadog/2/ASM_DATA/blocked_users/config", "msg": {"rules_data": []}}'
 ```
 
 ## Development
 
 ### Prerequisites
```

### Comparing `ddapm-test-agent-1.8.0/ddapm_test_agent.egg-info/SOURCES.txt` & `ddapm-test-agent-1.9.0/ddapm_test_agent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,24 +34,29 @@
 ddapm_test_agent.egg-info/requires.txt
 ddapm_test_agent.egg-info/top_level.txt
 releasenotes/config.yaml
 releasenotes/notes/1.0-e192f5064e917083.yaml
 releasenotes/notes/Add-metrics.process_id-to-ignored-attributes-62b264f0ea591326.yaml
 releasenotes/notes/add-distributed-trace-c35a314698a3b966.yaml
 releasenotes/notes/add-fmt-command-cc31769942a5fec3.yaml
+releasenotes/notes/add-optional-json-parser-10aac54bd1cbe322.yaml
 releasenotes/notes/add-rcm-endpoints-7e1f949e83e21039.yaml
+releasenotes/notes/add-session-to-rcm-endpoints-d97e925a04a99a65.yaml
 releasenotes/notes/add-support-telemetry-requests-10737cd3da802ca6.yaml
 releasenotes/notes/args-88f664c83a96075d.yaml
+releasenotes/notes/change-trace-proxy-headers-f9fcbb4efc4fcb95.yaml
 releasenotes/notes/check-http-header-sensitivity-daaa9d9595ae86d6.yaml
 releasenotes/notes/content_length-e1bab75580aa1dcb.yaml
 releasenotes/notes/docker-arm64-images-a4b6b2cc527327d6.yaml
 releasenotes/notes/fix-fmt-logging-6a323fd8d5d4eb28.yaml
 releasenotes/notes/fix-matching-319744b82d2514c1.yaml
 releasenotes/notes/fix-partial-chunks-0db14ce3017e6173.yaml
 releasenotes/notes/fix-racecondition-9bd0ef15b7da60fa.yaml
+releasenotes/notes/improve-test-agent-debugging-5759413f1fc5f7fa.yaml
+releasenotes/notes/improve-test-agent-proxying-a207f0fc81b3ab2d.yaml
 releasenotes/notes/info-34dcd9cbcc382487.yaml
 releasenotes/notes/info-drop-p0s-c207889f590340fb.yaml
 releasenotes/notes/new-process-id-tag-f0ab0daf652e05cc.yaml
 releasenotes/notes/profiling-endpoint-0cd209e4e5b6cfc0.yaml
 releasenotes/notes/proxy-37c94e2fb428c6fc.yaml
 releasenotes/notes/python-support-1c447acc4607abc7.yaml
 releasenotes/notes/python310-025fbc190363de98.yaml
```

### Comparing `ddapm-test-agent-1.8.0/releasenotes/notes/1.0-e192f5064e917083.yaml` & `ddapm-test-agent-1.9.0/releasenotes/notes/1.0-e192f5064e917083.yaml`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/riotfile.py` & `ddapm-test-agent-1.9.0/riotfile.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/scripts/check-releasenotes` & `ddapm-test-agent-1.9.0/scripts/check-releasenotes`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/setup.cfg` & `ddapm-test-agent-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/setup.py` & `ddapm-test-agent-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/conftest.py` & `ddapm-test-agent-1.9.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,33 +59,40 @@
 
 @pytest.fixture
 def trace_request_delay() -> Generator[float, None, None]:
     yield 0.0
 
 
 @pytest.fixture
+def suppress_trace_parse_errors() -> Generator[bool, None, None]:
+    yield False
+
+
+@pytest.fixture
 async def agent_app(
     aiohttp_server,
     agent_disabled_checks,
     log_span_fmt,
     snapshot_dir,
     snapshot_ci_mode,
     snapshot_ignored_attrs,
     agent_url,
     trace_request_delay,
+    suppress_trace_parse_errors,
 ):
     app = await aiohttp_server(
         make_app(
             agent_disabled_checks,
             log_span_fmt,
             str(snapshot_dir),
             snapshot_ci_mode,
             snapshot_ignored_attrs,
             agent_url,
             trace_request_delay,
+            suppress_trace_parse_errors,
         )
     )
     yield app
 
 
 @pytest.fixture
 async def agent(agent_app, aiohttp_client, loop):
@@ -104,21 +111,26 @@
                     "trace_id": random.randint(0, 2**64),
                     "span_id": random.randint(0, 2**64),
                     "parent_id": None,
                     "resource": "/users/",
                     "type": "http",
                     "start": 1342343123,
                     "duration": 123214,
+                    "error": 0,
                     "meta": {
+                        "component": "",
                         "http.url": "http://localhost:8080/users",
                         "http.method": "GET",
                         "http.status_code": "200",
                         "http.status_msg": "OK",
+                        "language": "python",
+                        "runtime-id": "2d377516ca12429aaf072f037ed2e4cc",
                     },
                     "metrics": {
+                        "process_id": 111,
                         "sampling_priority_v1": 1.0,
                     },
                 }
             ),
         ]
     ]
     return data
```

### Comparing `ddapm-test-agent-1.8.0/tests/integration_snapshots/test_multi_trace.json` & `ddapm-test-agent-1.9.0/tests/integration_snapshots/test_multi_trace.json`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/integration_snapshots/test_single_trace.json` & `ddapm-test-agent-1.9.0/tests/integration_snapshots/test_single_trace.json`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_distributed_propagated.json` & `ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_distributed_propagated.json`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_distributed_same_payload.json` & `ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_distributed_same_payload.json`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/integration_snapshots/test_trace_missing_received.json` & `ddapm-test-agent-1.9.0/tests/integration_snapshots/test_trace_missing_received.json`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_agent.py` & `ddapm-test-agent-1.9.0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_checks.py` & `ddapm-test-agent-1.9.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_session.py` & `ddapm-test-agent-1.9.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_snapshot.py` & `ddapm-test-agent-1.9.0/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_snapshot_integration.py` & `ddapm-test-agent-1.9.0/tests/test_snapshot_integration.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/test_trace.py` & `ddapm-test-agent-1.9.0/tests/test_trace.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,27 +48,39 @@
                     ]
                 ]
             ),
         ),
     ],
 )
 def test_decode_v04(content_type, payload):
-    assert decode_v04(content_type, payload) is not None
+    assert decode_v04(content_type, payload, False) is not None
 
 
 @pytest.mark.parametrize(
     "content_type, payload",
     [
         ("application/msgpack", msgpack.packb([{"name": "test"}])),
         ("application/json", json.dumps([{"name": "test"}])),
     ],
 )
 def test_decode_v04_bad(content_type, payload):
     with pytest.raises(TypeError):
-        decode_v04(content_type, payload)
+        decode_v04(content_type, payload, False)
+
+
+@pytest.mark.parametrize(
+    "content_type, payload",
+    [
+        ("application/msgpack", msgpack.packb([{"name": "test"}])),
+        ("application/json", json.dumps([{"name": "test"}])),
+    ],
+)
+def test_decode_v04_bad_doesnt_raise_with_supress(content_type, payload):
+    with pytest.raises(TypeError):
+        decode_v04(content_type, payload, True)
 
 
 @pytest.mark.parametrize(
     "trace",
     [
         [{"name": "root"}],
         [{"name": "root", "parent_id": 0}],
```

### Comparing `ddapm-test-agent-1.8.0/tests/test_tracestats.py` & `ddapm-test-agent-1.9.0/tests/test_tracestats.py`

 * *Files identical despite different names*

### Comparing `ddapm-test-agent-1.8.0/tests/trace_utils.py` & `ddapm-test-agent-1.9.0/tests/trace_utils.py`

 * *Files identical despite different names*

