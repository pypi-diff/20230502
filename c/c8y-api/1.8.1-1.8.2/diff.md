# Comparing `tmp/c8y_api-1.8.1.tar.gz` & `tmp/c8y_api-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c8y_api-1.8.1.tar", last modified: Tue Apr 18 07:05:46 2023, max compression
+gzip compressed data, was "c8y_api-1.8.2.tar", last modified: Tue May  2 10:34:10 2023, max compression
```

## Comparing `c8y_api-1.8.1.tar` & `c8y_api-1.8.2.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.853045 c8y_api-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-18 07:05:33.000000 c8y_api-1.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 07:05:33.000000 c8y_api-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-18 07:05:46.873045 c8y_api-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-18 07:05:33.000000 c8y_api-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_main_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/administration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/managedobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/notification2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/tenant_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_tk/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_tk/notification2/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/notification2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/notification2/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_devicegroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_global_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_inventoryroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-04-18 07:05:33.000000 c8y_api-1.8.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:05:33.000000 c8y_api-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 07:05:33.000000 c8y_api-1.8.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/cumulocity-tenant_options.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/cumulocity.json
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/dealing_with_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/handling_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/multi_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/notification2_asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/notification2_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/simple_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/simple_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/user_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 07:05:46.873045 c8y_api-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.869045 c8y_api-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/alarm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/application.json
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/audit_records.json
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/bulk_operations.json
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/event.json
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/global_role.json
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/inventoryrole.json
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/managed_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/operation.json
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/series.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/tenant_option.json
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_bulk_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_inventoryrole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_managedobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_tenant_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/user.json
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/util/
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-18 07:05:33.000000 c8y_api-1.8.1/util/microservice_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-18 07:05:33.000000 c8y_api-1.8.1/util/testing_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.828902 c8y_api-1.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.816902 c8y_api-1.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.816902 c8y_api-1.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-02 10:33:59.000000 c8y_api-1.8.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-02 10:33:59.000000 c8y_api-1.8.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-02 10:33:59.000000 c8y_api-1.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 10:33:59.000000 c8y_api-1.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-02 10:33:59.000000 c8y_api-1.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 10:33:59.000000 c8y_api-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-02 10:34:10.828902 c8y_api-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-02 10:33:59.000000 c8y_api-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.816902 c8y_api-1.8.2/c8y_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17106 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_main_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.820902 c8y_api-1.8.2/c8y_api/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.820902 c8y_api-1.8.2/c8y_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/administration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/managedobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/notification2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_api/model/tenant_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.816902 c8y_api-1.8.2/c8y_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-02 10:34:10.000000 c8y_api-1.8.2/c8y_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-02 10:34:10.000000 c8y_api-1.8.2/c8y_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:34:10.000000 c8y_api-1.8.2/c8y_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 10:34:10.000000 c8y_api-1.8.2/c8y_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 10:34:10.000000 c8y_api-1.8.2/c8y_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.820902 c8y_api-1.8.2/c8y_tk/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_tk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.820902 c8y_api-1.8.2/c8y_tk/notification2/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_tk/notification2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 10:33:59.000000 c8y_api-1.8.2/c8y_tk/notification2/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.824902 c8y_api-1.8.2/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_devicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_global_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_inventoryroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-02 10:33:59.000000 c8y_api-1.8.2/integration_tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-05-02 10:33:59.000000 c8y_api-1.8.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 10:33:59.000000 c8y_api-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 10:33:59.000000 c8y_api-1.8.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.824902 c8y_api-1.8.2/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/cumulocity-notification2_synchronous.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/cumulocity-tenant_options.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/cumulocity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/dealing_with_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/handling_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/multi_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/notification2_asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/notification2_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/simple_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/simple_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/user_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-02 10:33:59.000000 c8y_api-1.8.2/samples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 10:34:10.828902 c8y_api-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.824902 c8y_api-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.828902 c8y_api-1.8.2/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/alarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/audit_records.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/bulk_operations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/global_role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/inventoryrole.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/managed_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/operation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/tenant_option.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_bulk_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_inventoryrole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_managedobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_tenant_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/model/user.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/test_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-02 10:33:59.000000 c8y_api-1.8.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:34:10.828902 c8y_api-1.8.2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-02 10:33:59.000000 c8y_api-1.8.2/util/microservice_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-02 10:33:59.000000 c8y_api-1.8.2/util/testing_util.py
```

### Comparing `c8y_api-1.8.1/.github/workflows/codeql-analysis.yml` & `c8y_api-1.8.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/.github/workflows/python-publish.yml` & `c8y_api-1.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/CHANGELOG.md` & `c8y_api-1.8.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog
 
+
+## Version 1.8.2
+
+* Bumped flask from 2.2.2 to 2.3.2 (vulnerability)
+
+  Bumped python-dateutil from 2.8.1 to 2.8.2 (pandas requirement)
+
+* Added `is_tls` property to `CumulocityRestApi` class;
+
+  fixed secure protocol handling for Notification2 websocket connections.
+
+* Microservice build support improvements.
+
+
+## Version 1.8.1
+
+* Fixed series value collection for incomplete series.
+
+
 ## Version 1.8
 
 * Adding support for measurement series queries.
 
 ## Version 1.7
 
 * Adding support for the Audit API.
```

### Comparing `c8y_api-1.8.1/LICENSE` & `c8y_api-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/PKG-INFO` & `c8y_api-1.8.2/c8y_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: c8y_api
-Version: 1.8.1
+Name: c8y-api
+Version: 1.8.2
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.8.1/README.md` & `c8y_api-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/_auth.py` & `c8y_api-1.8.2/c8y_api/_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/_base_api.py` & `c8y_api-1.8.2/c8y_api/_base_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             auth (AuthBase):  Authentication details
             application_key (str):  Application ID to include in requests
                 (for billing/metering purposes).
         """
         self.base_url = base_url.rstrip('/')
         self.tenant_id = tenant_id
         self.application_key = application_key
+        self.is_tls = self.base_url.startswith('https')
 
         if auth:
             self.auth = auth
             self.username = self._resolve_username_from_auth(auth)
         elif username and password:
             self.auth = HTTPBasicAuth(f'{tenant_id}/{username}', password)
             self.username = username
```

### Comparing `c8y_api-1.8.1/c8y_api/_jwt.py` & `c8y_api-1.8.2/c8y_api/_jwt.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/_main_api.py` & `c8y_api-1.8.2/c8y_api/_main_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/_registry_api.py` & `c8y_api-1.8.2/c8y_api/_registry_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/_util.py` & `c8y_api-1.8.2/c8y_api/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/app/__init__.py` & `c8y_api-1.8.2/c8y_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/__init__.py` & `c8y_api-1.8.2/c8y_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/_base.py` & `c8y_api-1.8.2/c8y_api/model/_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/_parser.py` & `c8y_api-1.8.2/c8y_api/model/_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/_util.py` & `c8y_api-1.8.2/c8y_api/model/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/administration.py` & `c8y_api-1.8.2/c8y_api/model/administration.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/alarms.py` & `c8y_api-1.8.2/c8y_api/model/alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/applications.py` & `c8y_api-1.8.2/c8y_api/model/applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/audit.py` & `c8y_api-1.8.2/c8y_api/model/audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/binaries.py` & `c8y_api-1.8.2/c8y_api/model/binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/events.py` & `c8y_api-1.8.2/c8y_api/model/events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/identity.py` & `c8y_api-1.8.2/c8y_api/model/identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/inventory.py` & `c8y_api-1.8.2/c8y_api/model/inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/managedobjects.py` & `c8y_api-1.8.2/c8y_api/model/managedobjects.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/measurements.py` & `c8y_api-1.8.2/c8y_api/model/measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/notification2.py` & `c8y_api-1.8.2/c8y_api/model/notification2.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,17 +254,18 @@
     def build_websocket_uri(self, token: str):
         """Build websocket access URL.
 
         Args:
             token (str):  Subscriber access token
 
         Returns:
-             A websocket (wss://) URL to access the subscriber channel.
+             A websocket (ws(s)://) URL to access the subscriber channel.
         """
-        return f'wss://{self.host}/notification2/consumer/?token={token}'
+        protocol = 'wss' if self.c8y.is_tls else 'ws'
+        return f'{protocol}://{self.host}/notification2/consumer/?token={token}'
 
     def _build_token_definition(self, subscription: str, expires: int, subscriber: str = None):
         return {
             'subscriber': subscriber or self._default_subscriber,
             'subscription' : subscription,
             'expiresInMinutes' : expires
         }
```

### Comparing `c8y_api-1.8.1/c8y_api/model/operations.py` & `c8y_api-1.8.2/c8y_api/model/operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api/model/tenant_options.py` & `c8y_api-1.8.2/c8y_api/model/tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/c8y_api.egg-info/PKG-INFO` & `c8y_api-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: c8y-api
-Version: 1.8.1
+Name: c8y_api
+Version: 1.8.2
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.8.1/c8y_api.egg-info/SOURCES.txt` & `c8y_api-1.8.2/c8y_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 integration_tests/test_inventoryroles.py
 integration_tests/test_measurements.py
 integration_tests/test_operations.py
 integration_tests/test_tenant_options.py
 integration_tests/test_users.py
 samples/Dockerfile
 samples/build.sh
+samples/cumulocity-notification2_synchronous.json
 samples/cumulocity-tenant_options.json
 samples/cumulocity.json
 samples/dealing_with_measurements.py
 samples/handling_events.py
 samples/multi_tenant_app.py
 samples/notification2_asynchronous.py
 samples/notification2_synchronous.py
```

### Comparing `c8y_api-1.8.1/c8y_tk/notification2/listener.py` & `c8y_api-1.8.2/c8y_tk/notification2/listener.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/conftest.py` & `c8y_api-1.8.2/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_alarms.py` & `c8y_api-1.8.2/integration_tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_applications.py` & `c8y_api-1.8.2/integration_tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_audits.py` & `c8y_api-1.8.2/integration_tests/test_audits.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_binaries.py` & `c8y_api-1.8.2/integration_tests/test_binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_bulk_operations.py` & `c8y_api-1.8.2/integration_tests/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_device_registry.py` & `c8y_api-1.8.2/integration_tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_devicegroups.py` & `c8y_api-1.8.2/integration_tests/test_devicegroups.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_events.py` & `c8y_api-1.8.2/integration_tests/test_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_global_roles.py` & `c8y_api-1.8.2/integration_tests/test_global_roles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_identity.py` & `c8y_api-1.8.2/integration_tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_inventory.py` & `c8y_api-1.8.2/integration_tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_inventoryroles.py` & `c8y_api-1.8.2/integration_tests/test_inventoryroles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_measurements.py` & `c8y_api-1.8.2/integration_tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_operations.py` & `c8y_api-1.8.2/integration_tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_tenant_options.py` & `c8y_api-1.8.2/integration_tests/test_tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/integration_tests/test_users.py` & `c8y_api-1.8.2/integration_tests/test_users.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/pylintrc` & `c8y_api-1.8.2/pylintrc`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/build.sh` & `c8y_api-1.8.2/samples/build.sh`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # Darmstadt, Germany and/or Software AG USA Inc., Reston, VA, USA,
 # and/or its subsidiaries and/or its affiliates and/or their licensors.
 # Use, reproduction, transfer, publication or disclosure is prohibited except
 # as specifically provided for in your License Agreement with Software AG.
 
 NAME="$1"
 VERSION="$2"
-IMG_NAME=`echo "$NAME" | tr '[:upper:]' '[:lower:]' | tr '[:punct:]' '-'`
+IMG_NAME="$3"
+if ! [[ $IMG_NAME ]]; then
+  IMG_NAME=`echo "$NAME" | tr '[:upper:]' '[:lower:]' | tr '[:punct:]' '-'`
+fi
 BUILD_DIR="./build/samples/$NAME"
 DIST_DIR="./dist/samples/$NAME"
 TARGET="$DIST_DIR/$IMG_NAME.zip"
 
 echo "Name: $NAME, Image Name: $IMG_NAME, Version: $VERSION"
 echo "Build directory: $BUILD_DIR"
 echo "Dist directory:  $DIST_DIR"
@@ -41,15 +44,15 @@
 cp -r "./c8y_api" "$BUILD_DIR"
 cp -r "./c8y_tk" "$BUILD_DIR"
 sed -e "s/{VERSION}/$VERSION/g" ./samples/cumulocity.json > "$BUILD_DIR/cumulocity.json"
 sed -e "s/{SAMPLE}/$NAME/g" ./samples/Dockerfile > "$BUILD_DIR/Dockerfile"
 # extend cumulocity.json is defined
 if [[ -r ./samples/cumulocity-$NAME.json ]]; then
   echo -n "Found custom extension at './samples/cumulocity-$NAME.json'. Applying ..."
-  tmp=`tempfile`
+  tmp=`mktemp`
   jq -s '.[0] + .[1]' "$BUILD_DIR/cumulocity.json" ./samples/cumulocity-$NAME.json > $tmp
   mv $tmp "$BUILD_DIR/cumulocity.json"
   echo "  Done."
 fi
 
 # build image
 echo "Building image ..."
```

### Comparing `c8y_api-1.8.1/samples/dealing_with_measurements.py` & `c8y_api-1.8.2/samples/dealing_with_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/handling_events.py` & `c8y_api-1.8.2/samples/handling_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/multi_tenant_app.py` & `c8y_api-1.8.2/samples/multi_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/notification2_asynchronous.py` & `c8y_api-1.8.2/samples/notification2_asynchronous.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/notification2_synchronous.py` & `c8y_api-1.8.2/samples/notification2_synchronous.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/simple_agent.py` & `c8y_api-1.8.2/samples/simple_agent.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/simple_tenant_app.py` & `c8y_api-1.8.2/samples/simple_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/tenant_options.py` & `c8y_api-1.8.2/samples/tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/user_sessions.py` & `c8y_api-1.8.2/samples/user_sessions.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/samples/util.py` & `c8y_api-1.8.2/samples/util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/setup.cfg` & `c8y_api-1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tasks.py` & `c8y_api-1.8.2/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,28 +38,29 @@
     This will create a distributable wheel (.whl) file.
     """
     c.run('python -m build')
 
 
 @task(help={
     'sample': "Which sample to build.",
+    'name': "Microservice name. Defaults to sample name.",
     "version": "Microservice version. Defaults to '1.0.0'.",
 })
-def build_ms(c, sample, version='1.0.0'):
+def build_ms(c, sample, name=None, version='1.0.0'):
     """Build a Cumulocity microservice binary for upload.
 
     This will build a ready to deploy Cumulocity microservice from a sample
     file within the `samples` folder. Any sample Python script can be used
     (if it implements microservice logic).
 
-    Use the file name without .py extension as name. The build microservice
-    will use a similar name, following Cumulocity naming guidelines.
+    By default, uses the file name without .py extension as name. The built
+    microservice will use a similar name, following Cumulocity guidelines.
     """
     sample_name = ms_util.format_sample_name(sample)
-    c.run(f'samples/build.sh {sample_name} {version}')
+    c.run(f'samples/build.sh {sample_name} {version} {name if name else ""}')
 
 
 @task(help={
     'sample': "Which sample to register."
 })
 def register_ms(_, sample):
     """Register a sample as microservice at Cumulocity."""
```

### Comparing `c8y_api-1.8.1/tests/model/alarm.json` & `c8y_api-1.8.2/tests/model/alarm.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/application.json` & `c8y_api-1.8.2/tests/model/application.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/audit_records.json` & `c8y_api-1.8.2/tests/model/audit_records.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/bulk_operations.json` & `c8y_api-1.8.2/tests/model/bulk_operations.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/device.json` & `c8y_api-1.8.2/tests/model/device.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/event.json` & `c8y_api-1.8.2/tests/model/event.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/global_role.json` & `c8y_api-1.8.2/tests/model/global_role.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/inventoryrole.json` & `c8y_api-1.8.2/tests/model/inventoryrole.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/managed_object.json` & `c8y_api-1.8.2/tests/model/managed_object.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/series.json` & `c8y_api-1.8.2/tests/model/series.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/subscriptions.json` & `c8y_api-1.8.2/tests/model/subscriptions.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/tenant_option.json` & `c8y_api-1.8.2/tests/model/tenant_option.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_alarm.py` & `c8y_api-1.8.2/tests/model/test_alarm.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_application.py` & `c8y_api-1.8.2/tests/model/test_application.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_audit.py` & `c8y_api-1.8.2/tests/model/test_audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_base.py` & `c8y_api-1.8.2/tests/model/test_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_bulk_operation.py` & `c8y_api-1.8.2/tests/model/test_bulk_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_device.py` & `c8y_api-1.8.2/tests/model/test_device.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_event.py` & `c8y_api-1.8.2/tests/model/test_event.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_global_role.py` & `c8y_api-1.8.2/tests/model/test_global_role.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_inventory.py` & `c8y_api-1.8.2/tests/model/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_inventoryrole.py` & `c8y_api-1.8.2/tests/model/test_inventoryrole.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_managedobject.py` & `c8y_api-1.8.2/tests/model/test_managedobject.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_measurements.py` & `c8y_api-1.8.2/tests/model/test_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_operation.py` & `c8y_api-1.8.2/tests/model/test_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_parser.py` & `c8y_api-1.8.2/tests/model/test_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_resource.py` & `c8y_api-1.8.2/tests/model/test_resource.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_subscription.py` & `c8y_api-1.8.2/tests/model/test_subscription.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_tenant_option.py` & `c8y_api-1.8.2/tests/model/test_tenant_option.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/test_user.py` & `c8y_api-1.8.2/tests/model/test_user.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/model/user.json` & `c8y_api-1.8.2/tests/model/user.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/test_app.py` & `c8y_api-1.8.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/test_auth.py` & `c8y_api-1.8.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/test_base_api.py` & `c8y_api-1.8.2/tests/test_base_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/test_device_registry.py` & `c8y_api-1.8.2/tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/test_util.py` & `c8y_api-1.8.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/tests/utils.py` & `c8y_api-1.8.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/util/microservice_util.py` & `c8y_api-1.8.2/util/microservice_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8.1/util/testing_util.py` & `c8y_api-1.8.2/util/testing_util.py`

 * *Files identical despite different names*

