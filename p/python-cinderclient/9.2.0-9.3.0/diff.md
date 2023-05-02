# Comparing `tmp/python-cinderclient-9.2.0.tar.gz` & `tmp/python-cinderclient-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cinderclient-9.2.0.tar", last modified: Fri Dec 16 14:39:53 2022, max compression
+gzip compressed data, was "python-cinderclient-9.3.0.tar", last modified: Fri Feb 17 16:02:31 2023, max compression
```

## Comparing `python-cinderclient-9.2.0.tar` & `python-cinderclient-9.3.0.tar`

### file list

```diff
@@ -1,265 +1,266 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.236578 python-cinderclient-9.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1580 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13090 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46182 2022-12-16 14:39:52.000000 python-cinderclient-9.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21689 2022-12-16 14:39:53.236578 python-cinderclient-9.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17929 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.192575 python-cinderclient-9.2.0/cinderclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16016 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/api_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.192575 python-cinderclient-9.2.0/cinderclient/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18299 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11900 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16108 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32941 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.192575 python-cinderclient-9.2.0/cinderclient/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/contrib/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8829 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42459 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10139 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/shell_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.192575 python-cinderclient-9.2.0/cinderclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.196575 python-cinderclient-9.2.0/cinderclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6153 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6121 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3859 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/test_readonly_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/test_snapshot_create_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3913 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/test_volume_create_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/functional/test_volume_extend_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.196575 python-cinderclient-9.2.0/cinderclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1552 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fake_actions_module.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4384 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.200576 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10315 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/keystone_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11439 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1667 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_auth_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16887 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2478 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13559 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25694 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10452 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4490 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.204576 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.208576 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/contrib/test_list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27365 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45213 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/fakes_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_attachments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12624 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3727 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_cgsnapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7653 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_consistencygroups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_default_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3815 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8729 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6183 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2457 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3483 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_resource_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4485 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_services_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90087 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2399 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_snapshot_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4939 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6067 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_backups_30.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5558 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_encryption_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9891 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volumes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13165 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volumes_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9931 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.212576 python-cinderclient-9.2.0/cinderclient/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/attachments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3876 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/cgsnapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6478 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3359 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/consistencygroups.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.212576 python-cinderclient-9.2.0/cinderclient/v3/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/default_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9835 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2583 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2185 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5077 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/qos_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2158 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/resource_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108559 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88757 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/shell_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8924 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_backups_restore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_encryption_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11628 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5739 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volume_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13262 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volumes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20138 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/volumes_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/v3/workers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/cinderclient/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.212576 python-cinderclient-9.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7119 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/ext/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/cli/details.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/contributor/functional_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/contributor/unit_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15446 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/user/no_auth.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/doc/source/user/shell.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/functional_creds.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.216577 python-cinderclient-9.2.0/python_cinderclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21689 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9925 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-12-16 14:39:53.000000 python-cinderclient-9.2.0/python_cinderclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.184574 python-cinderclient-9.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.228577 python-cinderclient-9.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/add-generic-reset-state-command-d83v1f3accbf5807.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/adding-option-is-public-to-type-list-9a16bd9c2b8eb65a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/attachment-create-optional-server-id-9299d9da2b62b263.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/attachment-mode-8427aa6a2fa26e70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/backup-user-id-059ccea871893a0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1608166-ad91a7a9f50e658a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1675973-ad91a7a9f50e658a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1675974-34edd5g9870e65b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1675975-ad91a7a34e0esywc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1705093-9bc782d44018c27d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1713082-fb9276eed70f7e3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1826286-c9b68709a0d63d06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1867061-fix-py-raw-error-msg-ff3c6da0b01d5d6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1915996-3aaa5e2548eb7c93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/bug-1995883-force-flag-none-3a7bb87f655bcf42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cinder-poll-4f92694cc7eb657a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cinderclient-5-de0508ce5a221d21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cli-api-ver-negotiation-9f8fd8b77ae299fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cluster_commands-dca50e89c9d53cd2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cluster_list_manageable-40c02489b2c95d55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/cluster_migration_manage-31144d67bbfdb739.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/deprecate-allow-multiattach-2213a100c65a95c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/do-not-reset-volume-status-ae8e28132d7bfacd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/drop-python-3-6-and-3-7-fe2dc753e456b527.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/drop-python2-support-d3a1bedc75445edc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/drop-v2-support-e578ca21c7c6b532.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/enhance-backup-restore-shell-command-0cf55df6ca4b4c55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/feature-cross-az-backups-9d428ad4dfc552e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/list-with-count-78gtf45r66bf8912.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/log-request-id-148c74d308bcaa14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/messages-v3-api-3da81f4f66bf5903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/noauth-7d95e5af31a00e96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/profile-as-environment-variable-2a5c666ef759e486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/project-default-types-727156d1db10a24d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/reimage-volume-fea3a1178662e65a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/remove-cg-quota-9d4120b62f09cc5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/remove-credentials-e92b68e3bda80057.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/remove-deprecations-621919062f867015.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/remove-replv1-cabf2194edb9d963.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/remove-replv1-cli-61d5722438f888b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/replication-group-v3-api-022900ce6bf8feba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/return-request-id-to-caller-78d27f33f0048405.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/revert-to-snapshot-er4598df88aq5918.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/service_cleanup_cmd-cac85b697bc22af1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/service_dynamic_log-bd81d93c73fc1570.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/start-using-reno-18001103a6719c13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support---os-key-option-72ba2fd4880736ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-bs-mv-3.60-a65f1919b5068d17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-bs-mv-3.66-5214deb20d164056.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-create-volume-from-backup-c4e8aac89uy18uy2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-filter-type-7yt69ub7ccbf7419.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-filters-transfer-a1e7b728c7895a45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-generialized-resource-filter-8yf6w23f66bf5903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-keystone-v3-for-httpClient-d48ebb24880f5821.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-like-filter-7434w23f66bf5587.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-show-group-with-volume-ad820b8442e8a9e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/support-volume-summary-d6d5bb2acfef6ad5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/transfer-snapshots-555c61477835bcf7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/transfer-sort-ca622e9b8da605c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/ussuri-release-f0ebfc54cdac6680.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/victoria-release-0d9c2b43845c3d9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/volume-transfer-bug-23c760efb9f98a4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/wallaby-release-2535df50cc307fea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/xena-release-688918a69ada3a58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/notes/yoga-release-dcd35c98f6be478e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.232578 python-cinderclient-9.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.232578 python-cinderclient-9.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.232578 python-cinderclient-9.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9012 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-12-16 14:39:53.236578 python-cinderclient-9.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 14:39:53.236578 python-cinderclient-9.2.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/tools/cinder.bash_completion
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       41 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/tools/generate_authors.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7052 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/tools/lintstack.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/tools/lintstack.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3491 2022-12-16 14:39:26.000000 python-cinderclient-9.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1621 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13124 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46539 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21689 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17929 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.380381 python-cinderclient-9.3.0/cinderclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16016 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/api_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.380381 python-cinderclient-9.3.0/cinderclient/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18299 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11900 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16108 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32881 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.380381 python-cinderclient-9.3.0/cinderclient/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/contrib/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8829 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43186 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13044 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/shell_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.380381 python-cinderclient-9.3.0/cinderclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.384381 python-cinderclient-9.3.0/cinderclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6153 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6121 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3859 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/test_readonly_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/test_snapshot_create_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3913 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/test_volume_create_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/functional/test_volume_extend_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.384381 python-cinderclient-9.3.0/cinderclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1552 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fake_actions_module.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4384 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.384381 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2998 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10315 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/keystone_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11439 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1667 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_auth_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16887 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2478 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13559 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26295 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10506 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4490 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.392381 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.392381 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/contrib/test_list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27365 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45213 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/fakes_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_attachments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12624 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3727 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_cgsnapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7653 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_consistencygroups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_default_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3815 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8729 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6183 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2457 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3483 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_resource_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4485 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_services_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90794 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2399 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_snapshot_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4939 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6067 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_backups_30.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5558 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_encryption_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4054 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9891 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volumes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13165 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volumes_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.396381 python-cinderclient-9.3.0/cinderclient/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/attachments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3876 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/cgsnapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6478 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3359 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/consistencygroups.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.396381 python-cinderclient-9.3.0/cinderclient/v3/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/default_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5118 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9835 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2583 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2185 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5077 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/qos_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2158 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/resource_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108884 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    89051 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/shell_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8924 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_backups_restore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_encryption_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11628 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5739 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volume_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13262 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volumes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20138 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/volumes_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/v3/workers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/cinderclient/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.396381 python-cinderclient-9.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.396381 python-cinderclient-9.3.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7119 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/ext/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.400381 python-cinderclient-9.3.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.400381 python-cinderclient-9.3.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/cli/details.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4400 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.400381 python-cinderclient-9.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/contributor/functional_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/contributor/unit_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15446 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.400381 python-cinderclient-9.3.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/user/no_auth.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/doc/source/user/shell.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/functional_creds.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.400381 python-cinderclient-9.3.0/python_cinderclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21689 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9981 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 16:02:31.000000 python-cinderclient-9.3.0/python_cinderclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.376381 python-cinderclient-9.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.412381 python-cinderclient-9.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/add-generic-reset-state-command-d83v1f3accbf5807.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/adding-option-is-public-to-type-list-9a16bd9c2b8eb65a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/attachment-create-optional-server-id-9299d9da2b62b263.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/attachment-mode-8427aa6a2fa26e70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/backup-user-id-059ccea871893a0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1608166-ad91a7a9f50e658a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1675973-ad91a7a9f50e658a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1675974-34edd5g9870e65b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1675975-ad91a7a34e0esywc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1705093-9bc782d44018c27d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1713082-fb9276eed70f7e3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1826286-c9b68709a0d63d06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1867061-fix-py-raw-error-msg-ff3c6da0b01d5d6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1915996-3aaa5e2548eb7c93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/bug-1995883-force-flag-none-3a7bb87f655bcf42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cinder-poll-4f92694cc7eb657a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cinderclient-5-de0508ce5a221d21.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cli-api-ver-negotiation-9f8fd8b77ae299fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cluster_commands-dca50e89c9d53cd2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cluster_list_manageable-40c02489b2c95d55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/cluster_migration_manage-31144d67bbfdb739.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/collect-timing-ce6d521d40d422fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/deprecate-allow-multiattach-2213a100c65a95c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/do-not-reset-volume-status-ae8e28132d7bfacd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/drop-python-3-6-and-3-7-fe2dc753e456b527.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/drop-python2-support-d3a1bedc75445edc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/drop-v2-support-e578ca21c7c6b532.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/enhance-backup-restore-shell-command-0cf55df6ca4b4c55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/feature-cross-az-backups-9d428ad4dfc552e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/list-with-count-78gtf45r66bf8912.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/log-request-id-148c74d308bcaa14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/messages-v3-api-3da81f4f66bf5903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/noauth-7d95e5af31a00e96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/profile-as-environment-variable-2a5c666ef759e486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/project-default-types-727156d1db10a24d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/reimage-volume-fea3a1178662e65a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/remove-cg-quota-9d4120b62f09cc5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/remove-credentials-e92b68e3bda80057.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/remove-deprecations-621919062f867015.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/remove-replv1-cabf2194edb9d963.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/remove-replv1-cli-61d5722438f888b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/replication-group-v3-api-022900ce6bf8feba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/return-request-id-to-caller-78d27f33f0048405.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/revert-to-snapshot-er4598df88aq5918.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/service_cleanup_cmd-cac85b697bc22af1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/service_dynamic_log-bd81d93c73fc1570.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/start-using-reno-18001103a6719c13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support---os-key-option-72ba2fd4880736ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-bs-mv-3.60-a65f1919b5068d17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-bs-mv-3.66-5214deb20d164056.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-create-volume-from-backup-c4e8aac89uy18uy2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-filter-type-7yt69ub7ccbf7419.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-filters-transfer-a1e7b728c7895a45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-generialized-resource-filter-8yf6w23f66bf5903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-keystone-v3-for-httpClient-d48ebb24880f5821.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-like-filter-7434w23f66bf5587.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-show-group-with-volume-ad820b8442e8a9e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/support-volume-summary-d6d5bb2acfef6ad5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/transfer-snapshots-555c61477835bcf7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/transfer-sort-ca622e9b8da605c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/ussuri-release-f0ebfc54cdac6680.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/victoria-release-0d9c2b43845c3d9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/volume-transfer-bug-23c760efb9f98a4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/wallaby-release-2535df50cc307fea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/xena-release-688918a69ada3a58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/notes/yoga-release-dcd35c98f6be478e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9012 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 16:02:31.416381 python-cinderclient-9.3.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/tools/cinder.bash_completion
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       41 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/tools/generate_authors.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7052 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/tools/lintstack.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/tools/lintstack.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3508 2023-02-17 16:01:53.000000 python-cinderclient-9.3.0/tox.ini
```

### Comparing `python-cinderclient-9.2.0/.mailmap` & `python-cinderclient-9.3.0/.mailmap`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/.zuul.yaml` & `python-cinderclient-9.3.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     parent: python-cinderclient-functional-base
     nodeset: devstack-single-node-centos-9-stream
     vars:
       python_version: 3.9
       tox_envlist: functional-py39
 
 - project:
+    vars:
+      ensure_tox_version: '<4'
     templates:
       - check-requirements
       - lib-forward-testing-python3
       - openstack-cover-jobs
       - openstack-python3-antelope-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
```

### Comparing `python-cinderclient-9.2.0/AUTHORS` & `python-cinderclient-9.3.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 Christine Wang <ijuwang@us.ibm.com>
 Chuck Short <chuck.short@canonical.com>
 Cian O'Driscoll <cian@hp.com>
 Clark Boylan <clark.boylan@gmail.com>
 Clay Gerrard <clay.gerrard@gmail.com>
 Corey Bryant <corey.bryant@canonical.com>
 Cory Stone <corystone@gmail.com>
+Cyril Roelandt <cyril@redhat.com>
 Dan Prince <dprince@redhat.com>
 Davanum Srinivas <dims@linux.vnet.ibm.com>
 Dave Chen <wei.d.chen@intel.com>
 Dean Troyer <dtroyer@gmail.com>
 Deepti Ramakrishna <deepti.ramakrishna@intel.com>
 Derrick J. Wippler <thrawn01@gmail.com>
 Diane Fleming <diane.fleming@rackspace.com>
```

### Comparing `python-cinderclient-9.2.0/CONTRIBUTING.rst` & `python-cinderclient-9.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/ChangeLog` & `python-cinderclient-9.3.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 CHANGES
 =======
 
+9.3.0
+-----
+
+* Update minimum requirements
+* remove simplejson requirement
+* Continue using tox 3
+* Python3.11: fix crashes in ShellTest
+* Add test coverage for shell snapshot-create w/ metadata
+* Move print operations to shell\_utils
+
 9.2.0
 -----
 
 * Handle downgraded client for snapshot-create
+* Remove python-dev from bindep
 * Add Python3 antelope unit tests
 * Update bindep for ubuntu jammy
 * Update master for stable/zed
 
 9.1.0
 -----
 
 * Bump API max version to 3.70
+* Python3.11: Fix argparse-related test failures
 * Fix extension loading from python path
 
 9.0.0
 -----
 
 * Update python testing as per zed cycle testing runtime
 * Update master for stable/yoga
 
 8.3.0
 -----
 
 * Prepare for Yoga cinderclient release
 * Add volume reimage command
 * Move tempest requirement to functional env
+* Add support for collect-timing option
 * Add Python 3 only classifier
 * Updating python testing as per Yoga testing runtime
 
 8.2.0
 -----
 
 * Improve help text of volume create command
```

### Comparing `python-cinderclient-9.2.0/HACKING.rst` & `python-cinderclient-9.3.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/LICENSE` & `python-cinderclient-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/PKG-INFO` & `python-cinderclient-9.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cinderclient
-Version: 9.2.0
+Version: 9.3.0
 Summary: OpenStack Block Storage API Client Library
 Home-page: https://docs.openstack.org/python-cinderclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-cinderclient-9.2.0/README.rst` & `python-cinderclient-9.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/__init__.py` & `python-cinderclient-9.3.0/cinderclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/_i18n.py` & `python-cinderclient-9.3.0/cinderclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/api_versions.py` & `python-cinderclient-9.3.0/cinderclient/api_versions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/apiclient/base.py` & `python-cinderclient-9.3.0/cinderclient/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/apiclient/exceptions.py` & `python-cinderclient-9.3.0/cinderclient/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/base.py` & `python-cinderclient-9.3.0/cinderclient/base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/client.py` & `python-cinderclient-9.3.0/cinderclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #    under the License.
 """OpenStack Client interface. Handles the REST calls and responses."""
 
 import glob
 import hashlib
 import importlib.util
 import itertools
+import json
 import logging
 import os
 import pkgutil
 import re
 import urllib
 from urllib import parse as urlparse
 
@@ -43,19 +44,14 @@
 
 try:
     from eventlet import sleep
 except ImportError:
     from time import sleep
 
 try:
-    import json
-except ImportError:
-    import simplejson as json
-
-try:
     osprofiler_web = importutils.try_import("osprofiler.web")
 except Exception:
     pass
 
 
 _VALID_VERSIONS = ['v3']
 V3_SERVICE_TYPE = 'volumev3'
```

### Comparing `python-cinderclient-9.2.0/cinderclient/contrib/noauth.py` & `python-cinderclient-9.3.0/cinderclient/contrib/noauth.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/exceptions.py` & `python-cinderclient-9.3.0/cinderclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/extension.py` & `python-cinderclient-9.3.0/cinderclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/shell.py` & `python-cinderclient-9.3.0/cinderclient/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,14 +701,20 @@
             raise exc.CommandError(
                 "You must provide an authentication URL "
                 "through --os-auth-url or env[OS_AUTH_URL].")
 
         if not auth_session:
             auth_session = self._get_keystone_session()
 
+        # collect_timing is a keystone session option
+        if (not isinstance(auth_session, session.Session)
+                and getattr(args, 'collect_timing', False) is True):
+            raise exc.AuthorizationFailure("Provided auth plugin doesn't "
+                                           "support collect_timing option")
+
         insecure = self.options.insecure
 
         client_args = dict(
             region_name=os_region_name,
             tenant_id=os_project_id,
             endpoint_type=endpoint_type,
             extensions=self.extensions,
@@ -801,14 +807,25 @@
         finally:
             if profile:
                 trace_id = osprofiler_profiler.get().get_base_id()
                 print("Trace ID: %s" % trace_id)
                 print("To display trace use next command:\n"
                       "osprofiler trace show --html %s " % trace_id)
 
+            if getattr(args, 'collect_timing', False) is True:
+                self._print_timings(auth_session)
+
+    def _print_timings(self, session):
+        timings = session.get_timings()
+        utils.print_list(
+            timings,
+            fields=('method', 'url', 'seconds'),
+            sortby_index=None,
+            formatters={'seconds': lambda r: r.elapsed.total_seconds()})
+
     def _discover_client(self,
                          current_client,
                          os_api_version,
                          os_endpoint_type,
                          os_service_type,
                          os_username,
                          os_password,
```

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/base.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/test_cli.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/test_readonly_cli.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/test_readonly_cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/test_snapshot_create_cli.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/test_snapshot_create_cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/test_volume_create_cli.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/test_volume_create_cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/functional/test_volume_extend_cli.py` & `python-cinderclient-9.3.0/cinderclient/tests/functional/test_volume_extend_cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fake_actions_module.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fake_actions_module.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fakes.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/availability_zones.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/base.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/client.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/client.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/keystone_client.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/keystone_client.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/fixture_data/snapshots.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/fixture_data/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_api_versions.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_auth_plugins.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_auth_plugins.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_base.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_client.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_exceptions.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_http.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_shell.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,49 +116,49 @@
     def test_help_unknown_command(self):
         self.assertRaises(exceptions.CommandError, self.shell, 'help foofoo')
 
     def test_help(self):
         # Some expected help output, including microversioned commands
         required = [
             r'.*?^usage: ',
-            r'.*?(?m)^\s+create\s+Creates a volume.',
-            r'.*?(?m)^\s+summary\s+Get volumes summary.',
-            r'.*?(?m)^Run "cinder help SUBCOMMAND" for help on a subcommand.',
+            r'.*?^\s+create\s+Creates a volume.',
+            r'.*?^\s+summary\s+Get volumes summary.',
+            r'.*?^Run "cinder help SUBCOMMAND" for help on a subcommand.',
         ]
         help_text = self.shell('help')
         for r in required:
             self.assertThat(help_text,
                             matchers.MatchesRegex(r, re.DOTALL | re.MULTILINE))
 
     def test_help_on_subcommand(self):
         required = [
             r'.*?^usage: cinder list',
-            r'.*?(?m)^Lists all volumes.',
+            r'.*?^Lists all volumes.',
         ]
         help_text = self.shell('help list')
         for r in required:
             self.assertThat(help_text,
                             matchers.MatchesRegex(r, re.DOTALL | re.MULTILINE))
 
     def test_help_on_subcommand_mv(self):
         required = [
             r'.*?^usage: cinder summary',
-            r'.*?(?m)^Get volumes summary.',
+            r'.*?^Get volumes summary.',
         ]
         help_text = self.shell('help summary')
         for r in required:
             self.assertThat(help_text,
                             matchers.MatchesRegex(r, re.DOTALL | re.MULTILINE))
 
     def test_help_arg_no_subcommand(self):
         required = [
             r'.*?^usage: ',
-            r'.*?(?m)^\s+create\s+Creates a volume.',
-            r'.*?(?m)^\s+summary\s+Get volumes summary.',
-            r'.*?(?m)^Run "cinder help SUBCOMMAND" for help on a subcommand.',
+            r'.*?^\s+create\s+Creates a volume.',
+            r'.*?^\s+summary\s+Get volumes summary.',
+            r'.*?^Run "cinder help SUBCOMMAND" for help on a subcommand.',
         ]
         help_text = self.shell('--os-volume-api-version 3.40')
         for r in required:
             self.assertThat(help_text,
                             matchers.MatchesRegex(r, re.DOTALL | re.MULTILINE))
 
     @ddt.data('backup-create --help', '--help backup-create')
@@ -372,26 +372,30 @@
 
 class TestLoadVersionedActions(utils.TestCase):
     def setUp(self):
         super(TestLoadVersionedActions, self).setUp()
 
         self.mock_completion()
 
-    def test_load_versioned_actions(self):
+    def test_load_versioned_actions_v3_0(self):
         parser = cinderclient.shell.CinderClientArgumentParser()
         subparsers = parser.add_subparsers(metavar='<subcommand>')
         shell = cinderclient.shell.OpenStackCinderShell()
         shell.subcommands = {}
         shell._find_actions(subparsers, fake_actions_module,
                             api_versions.APIVersion("3.0"), False, [])
         self.assertIn('fake-action', shell.subcommands.keys())
         self.assertEqual(
             "fake_action 3.0 to 3.1",
             shell.subcommands['fake-action'].get_default('func')())
 
+    def test_load_versioned_actions_v3_2(self):
+        parser = cinderclient.shell.CinderClientArgumentParser()
+        subparsers = parser.add_subparsers(metavar='<subcommand>')
+        shell = cinderclient.shell.OpenStackCinderShell()
         shell.subcommands = {}
         shell._find_actions(subparsers, fake_actions_module,
                             api_versions.APIVersion("3.2"), False, [])
         self.assertIn('fake-action', shell.subcommands.keys())
         self.assertEqual(
             "fake_action 3.2 to 3.3",
             shell.subcommands['fake-action'].get_default('func')())
@@ -517,39 +521,44 @@
             mock.call('-h', '--help', action='help', help='==SUPPRESS=='),
             mock.call('--bar',
                       help="bar help (Supported by API versions"
                            " 3.3 - 3.4)")])
 
     @mock.patch.object(cinderclient.shell.CinderClientArgumentParser,
                        'add_argument')
-    def test_load_actions_with_versioned_args(self, mock_add_arg):
+    def test_load_actions_with_versioned_args_v36(self, mock_add_arg):
         parser = cinderclient.shell.CinderClientArgumentParser(add_help=False)
         subparsers = parser.add_subparsers(metavar='<subcommand>')
         shell = cinderclient.shell.OpenStackCinderShell()
         shell.subcommands = {}
         shell._find_actions(subparsers, fake_actions_module,
                             api_versions.APIVersion("3.6"), False, [])
         self.assertIn(mock.call('--foo', help="first foo"),
                       mock_add_arg.call_args_list)
         self.assertNotIn(mock.call('--foo', help="second foo"),
                          mock_add_arg.call_args_list)
 
-        mock_add_arg.reset_mock()
-
+    @mock.patch.object(cinderclient.shell.CinderClientArgumentParser,
+                       'add_argument')
+    def test_load_actions_with_versioned_args_v39(self, mock_add_arg):
+        parser = cinderclient.shell.CinderClientArgumentParser(add_help=False)
+        subparsers = parser.add_subparsers(metavar='<subcommand>')
+        shell = cinderclient.shell.OpenStackCinderShell()
+        shell.subcommands = {}
         shell._find_actions(subparsers, fake_actions_module,
                             api_versions.APIVersion("3.9"), False, [])
         self.assertNotIn(mock.call('--foo', help="first foo"),
                          mock_add_arg.call_args_list)
         self.assertIn(mock.call('--foo', help="second foo"),
                       mock_add_arg.call_args_list)
 
 
 class ShellUtilsTest(utils.TestCase):
 
-    @mock.patch.object(cinderclient.utils, 'print_dict')
+    @mock.patch.object(cinderclient.shell_utils, 'print_dict')
     def test_print_volume_image(self, mock_print_dict):
         response = {'os-volume_upload_image': {'name': 'myimg1'}}
         image_resp_tuple = (202, response)
         cinderclient.shell_utils.print_volume_image(image_resp_tuple)
 
         response = {'os-volume_upload_image':
                     {'name': 'myimg2',
```

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/test_utils.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,60 +216,60 @@
 
 class PrintListTestCase(test_utils.TestCase):
 
     def test_print_list_with_list(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
         to_print = [Row(a=3, b=4), Row(a=1, b=2)]
         with CaptureStdout() as cso:
-            utils.print_list(to_print, ['a', 'b'])
+            shell_utils.print_list(to_print, ['a', 'b'])
         # Output should be sorted by the first key (a)
         self.assertEqual("""\
 +---+---+
 | a | b |
 +---+---+
 | 1 | 2 |
 | 3 | 4 |
 +---+---+
 """, cso.read())
 
     def test_print_list_with_None_data(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
         to_print = [Row(a=3, b=None), Row(a=1, b=2)]
         with CaptureStdout() as cso:
-            utils.print_list(to_print, ['a', 'b'])
+            shell_utils.print_list(to_print, ['a', 'b'])
         # Output should be sorted by the first key (a)
         self.assertEqual("""\
 +---+---+
 | a | b |
 +---+---+
 | 1 | 2 |
 | 3 | - |
 +---+---+
 """, cso.read())
 
     def test_print_list_with_list_sortby(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
         to_print = [Row(a=4, b=3), Row(a=2, b=1)]
         with CaptureStdout() as cso:
-            utils.print_list(to_print, ['a', 'b'], sortby_index=1)
+            shell_utils.print_list(to_print, ['a', 'b'], sortby_index=1)
         # Output should be sorted by the second key (b)
         self.assertEqual("""\
 +---+---+
 | a | b |
 +---+---+
 | 2 | 1 |
 | 4 | 3 |
 +---+---+
 """, cso.read())
 
     def test_print_list_with_list_no_sort(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
         to_print = [Row(a=3, b=4), Row(a=1, b=2)]
         with CaptureStdout() as cso:
-            utils.print_list(to_print, ['a', 'b'], sortby_index=None)
+            shell_utils.print_list(to_print, ['a', 'b'], sortby_index=None)
         # Output should be in the order given
         self.assertEqual("""\
 +---+---+
 | a | b |
 +---+---+
 | 3 | 4 |
 | 1 | 2 |
@@ -279,29 +279,29 @@
     def test_print_list_with_generator(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
 
         def gen_rows():
             for row in [Row(a=1, b=2), Row(a=3, b=4)]:
                 yield row
         with CaptureStdout() as cso:
-            utils.print_list(gen_rows(), ['a', 'b'])
+            shell_utils.print_list(gen_rows(), ['a', 'b'])
         self.assertEqual("""\
 +---+---+
 | a | b |
 +---+---+
 | 1 | 2 |
 | 3 | 4 |
 +---+---+
 """, cso.read())
 
     def test_print_list_with_return(self):
         Row = collections.namedtuple('Row', ['a', 'b'])
         to_print = [Row(a=3, b='a\r'), Row(a=1, b='c\rd')]
         with CaptureStdout() as cso:
-            utils.print_list(to_print, ['a', 'b'])
+            shell_utils.print_list(to_print, ['a', 'b'])
         # Output should be sorted by the first key (a)
         self.assertEqual("""\
 +---+-----+
 | a | b   |
 +---+-----+
 | 1 | c d |
 | 3 | a   |
@@ -310,21 +310,21 @@
 
 
 class PrintDictTestCase(test_utils.TestCase):
 
     def test__pretty_format_dict(self):
         content = {'key1': 'value1', 'key2': 'value2'}
         expected = "key1 : value1\nkey2 : value2"
-        result = utils._pretty_format_dict(content)
+        result = shell_utils._pretty_format_dict(content)
         self.assertEqual(expected, result)
 
     def test_print_dict_with_return(self):
         d = {'a': 'A', 'b': 'B', 'c': 'C', 'd': 'test\rcarriage\n\rreturn'}
         with CaptureStdout() as cso:
-            utils.print_dict(d)
+            shell_utils.print_dict(d)
         self.assertEqual("""\
 +----------+---------------+
 | Property | Value         |
 +----------+---------------+
 | a        | A             |
 | b        | B             |
 | c        | C             |
@@ -333,15 +333,15 @@
 +----------+---------------+
 """, cso.read())
 
     def test_print_dict_with_dict_inside(self):
         content = {'a': 'A', 'b': 'B', 'f_key':
                    {'key1': 'value1', 'key2': 'value2'}}
         with CaptureStdout() as cso:
-            utils.print_dict(content, formatters='f_key')
+            shell_utils.print_dict(content, formatters='f_key')
         self.assertEqual("""\
 +----------+---------------+
 | Property | Value         |
 +----------+---------------+
 | a        | A             |
 | b        | B             |
 | f_key    | key1 : value1 |
```

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/utils.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/contrib/test_list_extensions.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/contrib/test_list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/fakes.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/fakes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/fakes_base.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/fakes_base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_attachments.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_attachments.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_auth.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_auth.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_availability_zone.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_capabilities.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_cgsnapshots.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_cgsnapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_clusters.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_clusters.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_consistencygroups.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_consistencygroups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_default_types.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_default_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_group_snapshots.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_group_types.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_group_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_groups.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_limits.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_messages.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_pools.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_pools.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_qos.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_qos.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_quota_classes.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_quotas.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_resource_filters.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_resource_filters.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_services.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_services.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_services_base.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_services_base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_shell.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
     @ddt.data("3.10", "3.11")
     def test_list_with_group_id_after_3_10(self, version):
         command = ('--os-volume-api-version %s list --group_id fake_id' %
                    version)
         self.run_command(command)
         self.assert_called('GET', '/volumes/detail?group_id=fake_id')
 
-    @mock.patch("cinderclient.utils.print_list")
+    @mock.patch("cinderclient.shell_utils.print_list")
     def test_list_duplicate_fields(self, mock_print):
         self.run_command('list --field Status,id,Size,status')
         self.assert_called('GET', '/volumes/detail')
         key_list = ['ID', 'Status', 'Size']
         mock_print.assert_called_once_with(mock.ANY, key_list,
             exclude_unavailable=True, sortby_index=0)
 
@@ -524,15 +524,15 @@
     @ddt.unpack
     def test_attachment_list(self, cmd, expected):
         command = '--os-volume-api-version 3.27 attachment-list '
         command += cmd
         self.run_command(command)
         self.assert_called('GET', '/attachments%s' % expected)
 
-    @mock.patch('cinderclient.utils.print_list')
+    @mock.patch('cinderclient.shell_utils.print_list')
     @mock.patch.object(cinderclient.v3.attachments.VolumeAttachmentManager,
             'list')
     def test_attachment_list_setattr(self, mock_list, mock_print):
         command = '--os-volume-api-version 3.27 attachment-list '
         fake_attachment = [attachments.VolumeAttachment(mock.ANY, attachment)
                 for attachment in fakes.fake_attachment_list['attachments']]
         mock_list.return_value = fake_attachment
@@ -966,14 +966,23 @@
             'volume_id': '123456',
             'name': None,
             'description': None,
             'metadata': {}
         }
     }
 
+    SNAP_BODY_3_66_W_METADATA = {
+        'snapshot': {
+            'volume_id': '123456',
+            'name': None,
+            'description': None,
+            'metadata': {'a': 'b'}
+        }
+    }
+
     @ddt.data(True, 'true', 'on', '1')
     @mock.patch('cinderclient.utils.find_resource')
     def test_snapshot_create_3_66_with_force_true(self, f_val, mock_find_vol):
         mock_find_vol.return_value = volumes.Volume(
             self, {'id': '123456'}, loaded=True)
         mock_find_vol.return_value = volumes.Volume(self,
                                                     {'id': '123456'},
@@ -1033,14 +1042,23 @@
                 'description': None,
                 'metadata': {}
             }
         }
         self.assert_called_anytime('POST', '/snapshots',
                                    body=pre_3_66_request_body)
 
+    @mock.patch('cinderclient.utils.find_resource')
+    def test_snapshot_create_w_metadata(self, mock_find_vol):
+        mock_find_vol.return_value = volumes.Volume(
+            self, {'id': '123456'}, loaded=True)
+        self.run_command('--os-volume-api-version 3.66 '
+                         'snapshot-create 123456 --metadata a=b')
+        self.assert_called_anytime('POST', '/snapshots',
+                                   body=self.SNAP_BODY_3_66_W_METADATA)
+
     def test_snapshot_manageable_list(self):
         self.run_command('--os-volume-api-version 3.8 '
                          'snapshot-manageable-list fakehost')
         self.assert_called('GET', '/manageable_snapshots/detail?host=fakehost')
 
     def test_snapshot_manageable_list_details(self):
         self.run_command('--os-volume-api-version 3.8 '
@@ -1281,26 +1299,26 @@
     def test_service_get_log_before_3_32(self, get_levels_mock):
         self.assertRaises(SystemExit,
                           self.run_command, '--os-volume-api-version 3.28 '
                          'service-get-log')
         get_levels_mock.assert_not_called()
 
     @mock.patch('cinderclient.v3.services.ServiceManager.get_log_levels')
-    @mock.patch('cinderclient.utils.print_list')
+    @mock.patch('cinderclient.shell_utils.print_list')
     def test_service_get_log_no_params(self, print_mock, get_levels_mock):
         self.run_command('--os-volume-api-version 3.32 service-get-log')
         get_levels_mock.assert_called_once_with('', '', '')
         print_mock.assert_called_once_with(get_levels_mock.return_value,
                                            ('Binary', 'Host', 'Prefix',
                                             'Level'))
 
     @ddt.data('*', 'cinder-api', 'cinder-volume', 'cinder-scheduler',
               'cinder-backup')
     @mock.patch('cinderclient.v3.services.ServiceManager.get_log_levels')
-    @mock.patch('cinderclient.utils.print_list')
+    @mock.patch('cinderclient.shell_utils.print_list')
     def test_service_get_log(self, binary, print_mock, get_levels_mock):
         server = 'host1'
         prefix = 'sqlalchemy'
 
         self.run_command('--os-volume-api-version 3.32 service-get-log '
                          '--binary %s --server %s --prefix %s' % (
                              binary, server, prefix))
@@ -1450,15 +1468,15 @@
                                'description': None,
                                'incremental': False,
                                'force': False,
                                'snapshot_id': None,
                                'availability_zone': 'AZ2'}}
         self.assert_called('POST', '/backups', body=expected)
 
-    @mock.patch("cinderclient.utils.print_list")
+    @mock.patch("cinderclient.shell_utils.print_list")
     def test_snapshot_list(self, mock_print_list):
         """Ensure we always present all existing fields when listing snaps."""
         self.run_command('--os-volume-api-version 3.65 snapshot-list')
         self.assert_called('GET', '/snapshots/detail')
         columns = ['ID', 'Volume ID', 'Status', 'Name', 'Size',
                    'Consumes Quota', 'User ID']
         mock_print_list.assert_called_once_with(mock.ANY, columns,
@@ -1919,15 +1937,15 @@
             'volume': None,
             'name': None,
             'volume_type': None,
             'availability_zone': 'different-az',
         },
     )
     @ddt.unpack
-    @mock.patch('cinderclient.utils.print_dict')
+    @mock.patch('cinderclient.shell_utils.print_dict')
     @mock.patch('cinderclient.tests.unit.v3.fakes_base._stub_restore')
     def test_do_backup_restore(self,
                                mock_stub_restore,
                                mock_print_dict,
                                volume,
                                name,
                                volume_type,
```

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_snapshot_actions.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_snapshot_actions.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_type_access.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_type_access.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_types.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_backups.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_backups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_backups_30.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_backups_30.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_encryption_types.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_encryption_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volume_transfers.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volume_transfers.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volumes.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volumes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/tests/unit/v3/test_volumes_base.py` & `python-cinderclient-9.3.0/cinderclient/tests/unit/v3/test_volumes_base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/__init__.py` & `python-cinderclient-9.3.0/cinderclient/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/attachments.py` & `python-cinderclient-9.3.0/cinderclient/v3/attachments.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/availability_zones.py` & `python-cinderclient-9.3.0/cinderclient/v3/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/capabilities.py` & `python-cinderclient-9.3.0/cinderclient/v3/capabilities.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/cgsnapshots.py` & `python-cinderclient-9.3.0/cinderclient/v3/cgsnapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/client.py` & `python-cinderclient-9.3.0/cinderclient/v3/client.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/clusters.py` & `python-cinderclient-9.3.0/cinderclient/v3/clusters.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/consistencygroups.py` & `python-cinderclient-9.3.0/cinderclient/v3/consistencygroups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/contrib/list_extensions.py` & `python-cinderclient-9.3.0/cinderclient/v3/contrib/list_extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from cinderclient import base
-from cinderclient import utils
+from cinderclient import shell_utils
 
 
 class ListExtResource(base.Resource):
     @property
     def summary(self):
         descr = self.description.strip()
         if not descr:
@@ -37,8 +37,8 @@
         return self._list("/extensions", 'extensions')
 
 
 def do_list_extensions(client, _args):
     """Lists all available os-api extensions."""
     extensions = client.list_extensions.show_all()
     fields = ["Name", "Summary", "Alias", "Updated"]
-    utils.print_list(extensions, fields)
+    shell_utils.print_list(extensions, fields)
```

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/default_types.py` & `python-cinderclient-9.3.0/cinderclient/v3/default_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/group_snapshots.py` & `python-cinderclient-9.3.0/cinderclient/v3/group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/group_types.py` & `python-cinderclient-9.3.0/cinderclient/v3/group_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/groups.py` & `python-cinderclient-9.3.0/cinderclient/v3/groups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/limits.py` & `python-cinderclient-9.3.0/cinderclient/v3/limits.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/messages.py` & `python-cinderclient-9.3.0/cinderclient/v3/messages.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/pools.py` & `python-cinderclient-9.3.0/cinderclient/v3/pools.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/qos_specs.py` & `python-cinderclient-9.3.0/cinderclient/v3/qos_specs.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/quota_classes.py` & `python-cinderclient-9.3.0/cinderclient/v3/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/quotas.py` & `python-cinderclient-9.3.0/cinderclient/v3/quotas.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/resource_filters.py` & `python-cinderclient-9.3.0/cinderclient/v3/resource_filters.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/services.py` & `python-cinderclient-9.3.0/cinderclient/v3/services.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/shell.py` & `python-cinderclient-9.3.0/cinderclient/v3/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     if cs.api_version >= api_versions.APIVersion('3.56'):
         columns.append('User ID')
 
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(backups, columns, sortby_index=sortby_index)
+    shell_utils.print_list(backups, columns, sortby_index=sortby_index)
     if show_count:
         print("Backup in total: %s" % total_count)
 
     with cs.backups.completion_cache(
             'uuid',
             cinderclient.v3.volume_backups.VolumeBackup,
             mode="w"):
@@ -278,15 +278,15 @@
         info['volume_id'] = volume._info['id']
         info['volume_name'] = volume_name
     else:
         restore = cs.restores.restore(backup.id, volume_id, args.name)
         info.update(restore._info)
         info.pop('links', None)
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--detail',
            action='store_true',
            help='Show detailed information about pools.')
 @utils.arg('--filters',
            action=AppendFilters,
@@ -312,15 +312,15 @@
     infos.update(pools._info)
 
     for info in infos['pools']:
         backend = dict()
         backend['name'] = info['name']
         if args.detail:
             backend.update(info['capabilities'])
-        utils.print_dict(backend)
+        shell_utils.print_dict(backend)
     AppendFilters.filters = []
 
 
 RESET_STATE_RESOURCES = {'volume': utils.find_volume,
                          'backup': shell_utils.find_backup,
                          'snapshot': shell_utils.find_volume_snapshot,
                          'group': shell_utils.find_group,
@@ -514,15 +514,15 @@
         if search_opts['all_tenants']:
             key_list.insert(1, 'Tenant ID')
 
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(volumes, key_list, exclude_unavailable=True,
+    shell_utils.print_list(volumes, key_list, exclude_unavailable=True,
                      sortby_index=sortby_index)
     if show_count:
         print("Volume in total: %s" % total_count)
     AppendFilters.filters = []
 
 
 @utils.arg('entity', metavar='<entity>', nargs='+',
@@ -743,15 +743,15 @@
         timeout_period = os.environ.get("POLL_TIMEOUT_PERIOD", 3600)
         shell_utils._poll_for_status(
             cs.volumes.get, volume.id, info, 'creating', ['available'],
             timeout_period, cs.client.global_request_id, cs.messages)
         volume = cs.volumes.get(volume.id)
         info.update(volume._info)
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
     with cs.volumes.completion_cache('uuid',
                                      cinderclient.v3.volumes.Volume,
                                      mode="a"):
         cs.volumes.write_to_completion_cache('uuid', volume.id)
     if volume.name is not None:
         with cs.volumes.completion_cache('name',
@@ -808,15 +808,15 @@
     all_tenants = args.all_tenants
     info = cs.volumes.summary(all_tenants)
 
     formatters = ['total_size', 'total_count']
     if cs.api_version >= api_versions.APIVersion("3.36"):
         formatters.append('metadata')
 
-    utils.print_dict(info['volume-summary'], formatters=formatters)
+    shell_utils.print_dict(info['volume-summary'], formatters=formatters)
 
 
 @api_versions.wraps('3.11')
 @utils.arg('--filters',
            action=AppendFilters,
            type=str,
            nargs='*',
@@ -849,15 +849,15 @@
 def do_group_type_show(cs, args):
     """Show group type details."""
     gtype = shell_utils.find_gtype(cs, args.group_type)
     info = dict()
     info.update(gtype._info)
 
     info.pop('links', None)
-    utils.print_dict(info, formatters=['group_specs'])
+    shell_utils.print_dict(info, formatters=['group_specs'])
 
 
 @api_versions.wraps('3.11')
 @utils.arg('id',
            metavar='<id>',
            help='ID of the group type.')
 @utils.arg('--name',
@@ -877,15 +877,15 @@
     shell_utils.print_group_type_list([gtype])
 
 
 @api_versions.wraps('3.11')
 def do_group_specs_list(cs, args):
     """Lists current group types and specs."""
     gtypes = cs.group_types.list()
-    utils.print_list(gtypes, ['ID', 'Name', 'group_specs'])
+    shell_utils.print_list(gtypes, ['ID', 'Name', 'group_specs'])
 
 
 @api_versions.wraps('3.11')
 @utils.arg('name',
            metavar='<name>',
            help='Name of new group type.')
 @utils.arg('--description',
@@ -1166,51 +1166,51 @@
                                 num_down_hosts=args.num_down_hosts,
                                 detailed=args.detailed)
 
     columns = ['Name', 'Binary', 'State', 'Status']
     if args.detailed:
         columns.extend(('Num Hosts', 'Num Down Hosts', 'Last Heartbeat',
                         'Disabled Reason', 'Created At', 'Updated at'))
-    utils.print_list(clusters, columns)
+    shell_utils.print_list(clusters, columns)
 
 
 @api_versions.wraps('3.7')
 @utils.arg('binary', metavar='<binary>', nargs='?', default='cinder-volume',
            help='Binary to filter by.  Default: cinder-volume.')
 @utils.arg('name', metavar='<cluster-name>',
            help='Name of the clustered service to show.')
 def do_cluster_show(cs, args):
     """Show detailed information on a clustered service."""
     cluster = cs.clusters.show(args.name, args.binary)
-    utils.print_dict(cluster.to_dict())
+    shell_utils.print_dict(cluster.to_dict())
 
 
 @api_versions.wraps('3.7')
 @utils.arg('binary', metavar='<binary>', nargs='?', default='cinder-volume',
            help='Binary to filter by.  Default: cinder-volume.')
 @utils.arg('name', metavar='<cluster-name>',
            help='Name of the clustered services to update.')
 def do_cluster_enable(cs, args):
     """Enables clustered services."""
     cluster = cs.clusters.update(args.name, args.binary, disabled=False)
-    utils.print_dict(cluster.to_dict())
+    shell_utils.print_dict(cluster.to_dict())
 
 
 @api_versions.wraps('3.7')
 @utils.arg('binary', metavar='<binary>', nargs='?', default='cinder-volume',
            help='Binary to filter by.  Default: cinder-volume.')
 @utils.arg('name', metavar='<cluster-name>',
            help='Name of the clustered services to update.')
 @utils.arg('--reason', metavar='<reason>', default=None,
            help='Reason for disabling clustered service.')
 def do_cluster_disable(cs, args):
     """Disables clustered services."""
     cluster = cs.clusters.update(args.name, args.binary, disabled=True,
                                  disabled_reason=args.reason)
-    utils.print_dict(cluster.to_dict())
+    shell_utils.print_dict(cluster.to_dict())
 
 
 @api_versions.wraps('3.24')
 @utils.arg('--cluster', metavar='<cluster-name>', default=None,
            help='Cluster name. Default=None.')
 @utils.arg('--host', metavar='<hostname>', default=None,
            help='Service host name. Default=None.')
@@ -1247,20 +1247,20 @@
 
     cleaning, unavailable = cs.workers.clean(**filters)
 
     columns = ('ID', 'Cluster Name', 'Host', 'Binary')
 
     if cleaning:
         print('Following services will be cleaned:')
-        utils.print_list(cleaning, columns)
+        shell_utils.print_list(cleaning, columns)
 
     if unavailable:
         print('There are no alternative nodes to do cleanup for the following '
               'services:')
-        utils.print_list(unavailable, columns)
+        shell_utils.print_list(unavailable, columns)
 
     if not (cleaning or unavailable):
         print('No cleanable services matched cleanup criteria.')
 
 
 @utils.arg('host',
            metavar='<host>',
@@ -1333,15 +1333,15 @@
                                bootable=args.bootable,
                                cluster=getattr(args, 'cluster', None))
 
     info = {}
     volume = cs.volumes.get(volume.id)
     info.update(volume._info)
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps('3.8')
 # NOTE(geguileo): host is positional but optional in order to maintain backward
 # compatibility even with mutually exclusive arguments.  If version is < 3.16
 # then only host positional argument will be possible, and since the
 # exclusive_arg group has required=True it will be required even if it's
@@ -1390,15 +1390,15 @@
     volumes = cs.volumes.list_manageable(host=args.host, detailed=detailed,
                                          marker=args.marker, limit=args.limit,
                                          offset=args.offset, sort=args.sort,
                                          cluster=cluster)
     columns = ['reference', 'size', 'safe_to_manage']
     if detailed:
         columns.extend(['reason_not_safe', 'cinder_id', 'extra_info'])
-    utils.print_list(volumes, columns, sortby_index=None)
+    shell_utils.print_list(volumes, columns, sortby_index=None)
 
 
 @api_versions.wraps('3.13')
 @utils.arg('--all-tenants',
            dest='all_tenants',
            metavar='<0|1>',
            nargs='?',
@@ -1423,15 +1423,15 @@
     # Update search option with `filters`
     if AppendFilters.filters:
         search_opts.update(shell_utils.extract_filters(AppendFilters.filters))
 
     groups = cs.groups.list(search_opts=search_opts)
 
     columns = ['ID', 'Status', 'Name']
-    utils.print_list(groups, columns)
+    shell_utils.print_list(groups, columns)
 
     with cs.groups.completion_cache(
             'uuid',
             cinderclient.v3.groups.Group,
             mode='w'):
         for group in groups:
             cs.groups.write_to_completion_cache('uuid', group.id)
@@ -1465,15 +1465,15 @@
         group = shell_utils.find_group(cs, args.group,
                                        list_volume=args.list_volume)
     else:
         group = shell_utils.find_group(cs, args.group)
     info.update(group._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps('3.13')
 @utils.arg('grouptype',
            metavar='<group-type>',
            help='Group type.')
 @utils.arg('volumetypes',
@@ -1501,15 +1501,15 @@
         availability_zone=args.availability_zone)
 
     info = dict()
     group = cs.groups.get(group.id)
     info.update(group._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
     with cs.groups.completion_cache('uuid',
                                     cinderclient.v3.groups.Group,
                                     mode='a'):
         cs.groups.write_to_completion_cache('uuid', group.id)
 
     if group.name is not None:
@@ -1552,15 +1552,15 @@
     info = cs.groups.create_from_src(
         group_snapshot.id if group_snapshot else None,
         source_group.id if source_group else None,
         args.name,
         args.description)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps('3.13')
 @utils.arg('group',
            metavar='<group>', nargs='+',
            help='Name or ID of one or more groups '
                 'to be deleted.')
@@ -1692,15 +1692,16 @@
         }
     """
 
     rc, replication_targets = shell_utils.find_group(
         cs, args.group).list_replication_targets()
     rep_targets = replication_targets.get('replication_targets')
     if rep_targets and len(rep_targets) > 0:
-        utils.print_list(rep_targets, [key for key in rep_targets[0].keys()])
+        shell_utils.print_list(rep_targets,
+                               [key for key in rep_targets[0].keys()])
 
 
 @api_versions.wraps('3.14')
 @utils.arg('--all-tenants',
            dest='all_tenants',
            metavar='<0|1>',
            nargs='?',
@@ -1739,30 +1740,30 @@
     # Update search option with `filters`
     if AppendFilters.filters:
         search_opts.update(shell_utils.extract_filters(AppendFilters.filters))
 
     group_snapshots = cs.group_snapshots.list(search_opts=search_opts)
 
     columns = ['ID', 'Status', 'Name']
-    utils.print_list(group_snapshots, columns)
+    shell_utils.print_list(group_snapshots, columns)
     AppendFilters.filters = []
 
 
 @api_versions.wraps('3.14')
 @utils.arg('group_snapshot',
            metavar='<group_snapshot>',
            help='Name or ID of group snapshot.')
 def do_group_snapshot_show(cs, args):
     """Shows group snapshot details."""
     info = dict()
     group_snapshot = shell_utils.find_group_snapshot(cs, args.group_snapshot)
     info.update(group_snapshot._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps('3.14')
 @utils.arg('group',
            metavar='<group>',
            help='Name or ID of a group.')
 @utils.arg('--name',
@@ -1782,15 +1783,15 @@
         args.description)
 
     info = dict()
     group_snapshot = cs.group_snapshots.get(group_snapshot.id)
     info.update(group_snapshot._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps('3.14')
 @utils.arg('group_snapshot',
            metavar='<group_snapshot>', nargs='+',
            help='Name or ID of one or more group snapshots to be deleted.')
 def do_group_snapshot_delete(cs, args):
@@ -1837,15 +1838,15 @@
         columns.extend(["Replication Status", "Active Backend ID", "Frozen"])
     # NOTE(jay-lau-513): we check if the response has disabled_reason
     # so as not to add the column when the extended ext is not enabled.
     if result and hasattr(result[0], 'disabled_reason'):
         columns.append("Disabled Reason")
     if cs.api_version.matches('3.49'):
         columns.extend(["Backend State"])
-    utils.print_list(result, columns)
+    shell_utils.print_list(result, columns)
 
 
 @api_versions.wraps('3.8')
 # NOTE(geguileo): host is positional but optional in order to maintain backward
 # compatibility even with mutually exclusive arguments.  If version is < 3.16
 # then only host positional argument will be possible, and since the
 # exclusive_arg group has required=True it will be required even if it's
@@ -1896,23 +1897,23 @@
                                                     limit=args.limit,
                                                     offset=args.offset,
                                                     sort=args.sort,
                                                     cluster=cluster)
     columns = ['reference', 'size', 'safe_to_manage', 'source_reference']
     if detailed:
         columns.extend(['reason_not_safe', 'cinder_id', 'extra_info'])
-    utils.print_list(snapshots, columns, sortby_index=None)
+    shell_utils.print_list(snapshots, columns, sortby_index=None)
 
 
 @api_versions.wraps("3.0")
 def do_api_version(cs, args):
     """Display the server API version information."""
     columns = ['ID', 'Status', 'Version', 'Min_version']
     response = cs.services.server_api_version()
-    utils.print_list(response, columns)
+    shell_utils.print_list(response, columns)
 
 
 @api_versions.wraps("3.40")
 @utils.arg(
     'snapshot',
     metavar='<snapshot>',
     help='Name or ID of the snapshot to restore. The snapshot must be the '
@@ -2006,29 +2007,29 @@
 
     columns = ['ID', 'Resource Type', 'Resource UUID', 'Event ID',
                'User Message']
     if sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(messages, columns, sortby_index=sortby_index)
+    shell_utils.print_list(messages, columns, sortby_index=sortby_index)
     AppendFilters.filters = []
 
 
 @api_versions.wraps("3.3")
 @utils.arg('message',
            metavar='<message>',
            help='ID of message.')
 def do_message_show(cs, args):
     """Shows message details."""
     info = dict()
     message = shell_utils.find_message(cs, args.message)
     info.update(message._info)
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @api_versions.wraps("3.3")
 @utils.arg('message',
            metavar='<message>', nargs='+',
            help='ID of one or more message to be deleted.')
 def do_message_delete(cs, args):
@@ -2175,19 +2176,19 @@
                                              sort=args.sort)
 
     shell_utils.translate_volume_snapshot_keys(snapshots)
     sortby_index = None if args.sort else 0
     # It's the server's responsibility to return the appropriate fields for the
     # requested microversion, we present all known fields and skip those that
     # are missing.
-    utils.print_list(snapshots,
-                     ['ID', 'Volume ID', 'Status', 'Name', 'Size',
-                      'Consumes Quota', 'User ID'],
-                     exclude_unavailable=True,
-                     sortby_index=sortby_index)
+    shell_utils.print_list(snapshots,
+                           ['ID', 'Volume ID', 'Status', 'Name', 'Size',
+                            'Consumes Quota', 'User ID'],
+                           exclude_unavailable=True,
+                           sortby_index=sortby_index)
     if show_count:
         print("Snapshot in total: %s" % total_count)
 
     with cs.volume_snapshots.completion_cache(
             'uuid',
             cinderclient.v3.volume_snapshots.Snapshot,
             mode='w'):
@@ -2407,34 +2408,34 @@
     for attachment in attachments:
         setattr(attachment, 'server_id', getattr(attachment, 'instance', None))
     columns = ['ID', 'Volume ID', 'Status', 'Server ID']
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(attachments, columns, sortby_index=sortby_index)
+    shell_utils.print_list(attachments, columns, sortby_index=sortby_index)
     AppendFilters.filters = []
 
 
 @api_versions.wraps('3.27')
 @utils.arg('attachment',
            metavar='<attachment>',
            help='ID of attachment.')
 def do_attachment_show(cs, args):
     """Show detailed information for attachment."""
     attachment = cs.attachments.show(args.attachment)
     attachment_dict = attachment.to_dict()
     connection_dict = attachment_dict.pop('connection_info', {})
-    utils.print_dict(attachment_dict)
+    shell_utils.print_dict(attachment_dict)
 
     # TODO(jdg): Need to add checks here like admin/policy for displaying the
     # connection_info, this is still experimental so we'll leave it enabled for
     # now
     if connection_dict:
-        utils.print_dict(connection_dict)
+        shell_utils.print_dict(connection_dict)
 
 
 @api_versions.wraps('3.27')
 @utils.arg('volume',
            metavar='<volume>',
            help='Name or ID of volume or volumes to attach.')
 @utils.arg('server_id',
@@ -2499,17 +2500,17 @@
     mode = getattr(args, 'mode', 'null')
     attachment = cs.attachments.create(volume.id,
                                        connector,
                                        args.server_id,
                                        mode)
 
     connector_dict = attachment.pop('connection_info', None)
-    utils.print_dict(attachment)
+    shell_utils.print_dict(attachment)
     if connector_dict:
-        utils.print_dict(connector_dict)
+        shell_utils.print_dict(connector_dict)
 
 
 @api_versions.wraps('3.27')
 @utils.arg('attachment',
            metavar='<attachment>',
            help='ID of attachment.')
 @utils.arg('--initiator',
@@ -2553,17 +2554,17 @@
                  'os_type': args.ostype,
                  'multipath': args.multipath,
                  'mountpoint': args.mountpoint}
     attachment = cs.attachments.update(args.attachment,
                                        connector)
     attachment_dict = attachment.to_dict()
     connector_dict = attachment_dict.pop('connection_info', None)
-    utils.print_dict(attachment_dict)
+    shell_utils.print_dict(attachment_dict)
     if connector_dict:
-        utils.print_dict(connector_dict)
+        shell_utils.print_dict(connector_dict)
 
 
 @api_versions.wraps('3.27')
 @utils.arg('attachment',
            metavar='<attachment>', nargs='+',
            help='ID of attachment or attachments to delete.')
 def do_attachment_delete(cs, args):
@@ -2594,15 +2595,15 @@
     print("Client supported API versions:")
     print("Minimum version %(v)s" %
           {'v': api_versions.MIN_VERSION})
     print("Maximum version %(v)s" %
           {'v': api_versions.MAX_VERSION})
 
     print("\nServer supported API versions:")
-    utils.print_list(result, columns)
+    shell_utils.print_list(result, columns)
 
 
 @api_versions.wraps('3.32')
 @utils.arg('level',
            metavar='<log-level>',
            choices=('INFO', 'WARNING', 'ERROR', 'DEBUG',
                     'info', 'warning', 'error', 'debug'),
@@ -2637,15 +2638,15 @@
            default='',
            help='Prefix for the log. ie: "sqlalchemy.".')
 def do_service_get_log(cs, args):
     """Gets the service log level."""
     log_levels = cs.services.get_log_levels(args.binary, args.server,
                                             args.prefix)
     columns = ('Binary', 'Host', 'Prefix', 'Level')
-    utils.print_list(log_levels, columns)
+    shell_utils.print_list(log_levels, columns)
 
 
 @utils.arg('volume', metavar='<volume>',
            help='Name or ID of volume to backup.')
 @utils.arg('--container', metavar='<container>',
            default=None,
            help='Backup container name. Default=None.')
@@ -2714,15 +2715,15 @@
                                **kwargs)
     info = {"volume_id": volume.id}
     info.update(backup._info)
 
     if 'links' in info:
         info.pop('links')
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
     with cs.backups.completion_cache(
             'uuid',
             cinderclient.v3.volume_backups.VolumeBackup,
             mode="a"):
         cs.backups.write_to_completion_cache('uuid', backup.id)
 
@@ -2755,15 +2756,15 @@
     transfer = cs.transfers.create(volume.id,
                                    args.name,
                                    **kwargs)
     info = dict()
     info.update(transfer._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--all-tenants',
            dest='all_tenants',
            metavar='<0|1>',
            nargs='?',
            type=int,
@@ -2803,15 +2804,15 @@
         if len(sort_args) > 2:
             raise exceptions.CommandError(
                 'Invalid sort parameter provided. Argument must be in the '
                 'form "key[:<asc|desc>]".')
 
     transfers = cs.transfers.list(search_opts=search_opts, sort=sort)
     columns = ['ID', 'Volume ID', 'Name']
-    utils.print_list(transfers, columns)
+    shell_utils.print_list(transfers, columns)
     AppendFilters.filters = []
 
 
 @api_versions.wraps('3.62')
 @utils.arg('volume_type',
            metavar='<volume_type>',
            help='Name or ID of the volume type.')
@@ -2820,32 +2821,32 @@
            help='ID of project for which to set default type.')
 def do_default_type_set(cs, args):
     """Sets a default volume type for a project."""
     volume_type = args.volume_type
     project = args.project
 
     default_type = cs.default_types.create(volume_type, project)
-    utils.print_dict(default_type._info)
+    shell_utils.print_dict(default_type._info)
 
 
 @api_versions.wraps('3.62')
 @utils.arg('--project-id',
            metavar='<project_id>',
            default=None,
            help='ID of project for which to show the default type.')
 def do_default_type_list(cs, args):
     """Lists all default volume types."""
 
     project_id = args.project_id
     default_types = cs.default_types.list(project_id)
     columns = ['Volume Type ID', 'Project ID']
     if project_id:
-        utils.print_dict(default_types._info)
+        shell_utils.print_dict(default_types._info)
     else:
-        utils.print_list(default_types, columns)
+        shell_utils.print_list(default_types, columns)
 
 
 @api_versions.wraps('3.62')
 @utils.arg('project_id',
            metavar='<project_id>',
            nargs='+',
            help='ID of project for which to unset default type.')
```

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/shell_base.py` & `python-cinderclient-9.3.0/cinderclient/v3/shell_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         if search_opts['all_tenants']:
             key_list.insert(1, 'Tenant ID')
 
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(volumes, key_list, exclude_unavailable=True,
+    shell_utils.print_list(volumes, key_list, exclude_unavailable=True,
                      sortby_index=sortby_index)
 
 
 @utils.arg('volume',
            metavar='<volume>',
            help='Name or ID of volume.')
 def do_show(cs, args):
@@ -177,17 +177,17 @@
     info.update(volume._info)
 
     if 'readonly' in info['metadata']:
         info['readonly'] = info['metadata']['readonly']
 
     info.pop('links', None)
     info = _translate_attachments(info)
-    utils.print_dict(info,
-                     formatters=['metadata', 'volume_image_metadata',
-                                 'attachment_ids', 'attached_servers'])
+    shell_utils.print_dict(info,
+                           formatters=['metadata', 'volume_image_metadata',
+                                       'attachment_ids', 'attached_servers'])
 
 
 class CheckSizeArgForCreate(argparse.Action):
     def __call__(self, parser, args, values, option_string=None):
         if ((args.snapshot_id or args.source_volid)
                 is None and values is None):
             if not hasattr(args, 'backup_id') or args.backup_id is None:
@@ -321,15 +321,15 @@
     info.update(volume._info)
 
     if 'readonly' in info['metadata']:
         info['readonly'] = info['metadata']['readonly']
 
     info.pop('links', None)
     info = _translate_attachments(info)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--cascade',
            action='store_true',
            default=False,
            help='Remove any snapshots along with volume. Default=False.')
 @utils.arg('volume',
@@ -577,17 +577,17 @@
                                          sort=args.sort)
     shell_utils.translate_volume_snapshot_keys(snapshots)
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
 
-    utils.print_list(snapshots,
-                     ['ID', 'Volume ID', 'Status', 'Name', 'Size'],
-                     sortby_index=sortby_index)
+    shell_utils.print_list(snapshots,
+                           ['ID', 'Volume ID', 'Status', 'Name', 'Size'],
+                           sortby_index=sortby_index)
 
 
 @utils.arg('snapshot',
            metavar='<snapshot>',
            help='Name or ID of snapshot.')
 def do_snapshot_show(cs, args):
     """Shows snapshot details."""
@@ -710,15 +710,15 @@
 def do_type_show(cs, args):
     """Show volume type details."""
     vtype = shell_utils.find_vtype(cs, args.volume_type)
     info = dict()
     info.update(vtype._info)
 
     info.pop('links', None)
-    utils.print_dict(info, formatters=['extra_specs'])
+    shell_utils.print_dict(info, formatters=['extra_specs'])
 
 
 @utils.arg('id',
            metavar='<id>',
            help='ID of the volume type.')
 @utils.arg('--name',
            metavar='<name>',
@@ -742,15 +742,15 @@
                                    is_public)
     shell_utils.print_volume_type_list([vtype])
 
 
 def do_extra_specs_list(cs, args):
     """Lists current volume types and extra specs."""
     vtypes = cs.volume_types.list()
-    utils.print_list(vtypes, ['ID', 'Name', 'extra_specs'])
+    shell_utils.print_list(vtypes, ['ID', 'Name', 'extra_specs'])
 
 
 @utils.arg('name',
            metavar='<name>',
            help='Name of new volume type.')
 @utils.arg('--description',
            metavar='<description>',
@@ -817,15 +817,15 @@
     volume_type = shell_utils.find_volume_type(cs, args.volume_type)
     if volume_type.is_public:
         raise exceptions.CommandError("Failed to get access list "
                                       "for public volume type.")
     access_list = cs.volume_type_access.list(volume_type)
 
     columns = ['Volume_type_ID', 'Project_ID']
-    utils.print_list(access_list, columns)
+    shell_utils.print_list(access_list, columns)
 
 
 @utils.arg('--volume-type', metavar='<volume_type>', required=True,
            help='Volume type name or ID to add access for the given project.')
 @utils.arg('--project-id', metavar='<project_id>', required=True,
            help='Project ID to add volume type access for.')
 def do_type_access_add(cs, args):
@@ -968,27 +968,27 @@
            nargs='?',
            default=None,
            help='Display information for a single tenant (Admin only).')
 def do_absolute_limits(cs, args):
     """Lists absolute limits for a user."""
     limits = cs.limits.get(args.tenant).absolute
     columns = ['Name', 'Value']
-    utils.print_list(limits, columns)
+    shell_utils.print_list(limits, columns)
 
 
 @utils.arg('tenant',
            metavar='<tenant_id>',
            nargs='?',
            default=None,
            help='Display information for a single tenant (Admin only).')
 def do_rate_limits(cs, args):
     """Lists rate limits for a user."""
     limits = cs.limits.get(args.tenant).rate
     columns = ['Verb', 'URI', 'Value', 'Remain', 'Unit', 'Next_Available']
-    utils.print_list(limits, columns)
+    shell_utils.print_list(limits, columns)
 
 
 @utils.arg('volume',
            metavar='<volume>',
            help='Name or ID of volume to snapshot.')
 @utils.arg('--force',
            metavar='<True|False>',
@@ -1129,26 +1129,26 @@
 
     info = {"volume_id": volume.id}
     info.update(backup._info)
 
     if 'links' in info:
         info.pop('links')
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('backup', metavar='<backup>', help='Name or ID of backup.')
 def do_backup_show(cs, args):
     """Shows backup details."""
     backup = shell_utils.find_backup(cs, args.backup)
     info = dict()
     info.update(backup._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--all-tenants',
            metavar='<all_tenants>',
            nargs='?',
            type=int,
            const=1,
@@ -1207,15 +1207,15 @@
     shell_utils.translate_volume_snapshot_keys(backups)
     columns = ['ID', 'Volume ID', 'Status', 'Name', 'Size', 'Object Count',
                'Container']
     if args.sort:
         sortby_index = None
     else:
         sortby_index = 0
-    utils.print_list(backups, columns, sortby_index=sortby_index)
+    shell_utils.print_list(backups, columns, sortby_index=sortby_index)
 
 
 @utils.arg('--force',
            action="store_true",
            help='Allows deleting backup of a volume '
            'when its status is other than "available" or "error". '
            'Default=False.')
@@ -1269,35 +1269,35 @@
     restore = cs.restores.restore(backup.id, volume_id, args.name)
 
     info = {"backup_id": backup.id}
     info.update(restore._info)
 
     info.pop('links', None)
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('backup', metavar='<backup>',
            help='ID of the backup to export.')
 def do_backup_export(cs, args):
     """Export backup metadata record."""
     info = cs.backups.export_record(args.backup)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('backup_service', metavar='<backup_service>',
            help='Backup service to use for importing the backup.')
 @utils.arg('backup_url', metavar='<backup_url>',
            help='Backup URL for importing the backup metadata.')
 def do_backup_import(cs, args):
     """Import backup metadata record."""
     info = cs.backups.import_record(args.backup_service, args.backup_url)
     info.pop('links', None)
 
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('backup', metavar='<backup>', nargs='+',
            help='Name or ID of the backup to modify.')
 @utils.arg('--state', metavar='<state>',
            default='available',
            help='The state to assign to the backup. Valid values are '
@@ -1341,15 +1341,15 @@
     volume = utils.find_volume(cs, args.volume)
     transfer = cs.transfers.create(volume.id,
                                    args.name)
     info = dict()
     info.update(transfer._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('transfer', metavar='<transfer>',
            help='Name or ID of transfer to delete.')
 def do_transfer_delete(cs, args):
     """Undoes a transfer."""
     transfer = shell_utils.find_transfer(cs, args.transfer)
@@ -1363,15 +1363,15 @@
 def do_transfer_accept(cs, args):
     """Accepts a volume transfer."""
     transfer = cs.transfers.accept(args.transfer, args.auth_key)
     info = dict()
     info.update(transfer._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--all-tenants',
            dest='all_tenants',
            metavar='<0|1>',
            nargs='?',
            type=int,
@@ -1387,27 +1387,27 @@
     """Lists all transfers."""
     all_tenants = int(os.environ.get("ALL_TENANTS", args.all_tenants))
     search_opts = {
         'all_tenants': all_tenants,
     }
     transfers = cs.transfers.list(search_opts=search_opts)
     columns = ['ID', 'Volume ID', 'Name']
-    utils.print_list(transfers, columns)
+    shell_utils.print_list(transfers, columns)
 
 
 @utils.arg('transfer', metavar='<transfer>',
            help='Name or ID of transfer to accept.')
 def do_transfer_show(cs, args):
     """Shows transfer details."""
     transfer = shell_utils.find_transfer(cs, args.transfer)
     info = dict()
     info.update(transfer._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('volume', metavar='<volume>',
            help='Name or ID of volume to extend.')
 @utils.arg('new_size',
            metavar='<new_size>',
            type=int,
@@ -1437,24 +1437,24 @@
     columns = ["Binary", "Host", "Zone", "Status", "State", "Updated_at"]
     if replication:
         columns.extend(["Replication Status", "Active Backend ID", "Frozen"])
     # NOTE(jay-lau-513): we check if the response has disabled_reason
     # so as not to add the column when the extended ext is not enabled.
     if result and hasattr(result[0], 'disabled_reason'):
         columns.append("Disabled Reason")
-    utils.print_list(result, columns)
+    shell_utils.print_list(result, columns)
 
 
 @utils.arg('host', metavar='<hostname>', help='Host name.')
 @utils.arg('binary', metavar='<binary>', help='Service binary.')
 def do_service_enable(cs, args):
     """Enables the service."""
     result = cs.services.enable(args.host, args.binary)
     columns = ["Host", "Binary", "Status"]
-    utils.print_list([result], columns)
+    shell_utils.print_list([result], columns)
 
 
 @utils.arg('host', metavar='<hostname>', help='Host name.')
 @utils.arg('binary', metavar='<binary>', help='Service binary.')
 @utils.arg('--reason', metavar='<reason>',
            help='Reason for disabling service.')
 def do_service_disable(cs, args):
@@ -1462,15 +1462,15 @@
     columns = ["Host", "Binary", "Status"]
     if args.reason:
         columns.append('Disabled Reason')
         result = cs.services.disable_log_reason(args.host, args.binary,
                                                 args.reason)
     else:
         result = cs.services.disable(args.host, args.binary)
-    utils.print_list([result], columns)
+    shell_utils.print_list([result], columns)
 
 
 def treeizeAvailabilityZone(zone):
     """Builds a tree view for availability zones."""
     AvailabilityZone = availability_zones.AvailabilityZone
 
     az = AvailabilityZone(zone.manager,
@@ -1521,21 +1521,21 @@
         except Exception:
             raise
 
     result = []
     for zone in availability_zones:
         result += treeizeAvailabilityZone(zone)
     shell_utils.translate_availability_zone_keys(result)
-    utils.print_list(result, ['Name', 'Status'])
+    shell_utils.print_list(result, ['Name', 'Status'])
 
 
 def do_encryption_type_list(cs, args):
     """Shows encryption type details for volume types. Admin only."""
     result = cs.volume_encryption_types.list()
-    utils.print_list(result, ['Volume Type ID', 'Provider', 'Cipher',
+    shell_utils.print_list(result, ['Volume Type ID', 'Provider', 'Cipher',
                               'Key Size', 'Control Location'])
 
 
 @utils.arg('volume_type',
            metavar='<volume_type>',
            type=str,
            help='Name or ID of volume type.')
@@ -1792,42 +1792,42 @@
 def do_snapshot_metadata(cs, args):
     """Sets or deletes snapshot metadata."""
     snapshot = shell_utils.find_volume_snapshot(cs, args.snapshot)
     metadata = shell_utils.extract_metadata(args)
 
     if args.action == 'set':
         metadata = snapshot.set_metadata(metadata)
-        utils.print_dict(metadata._info)
+        shell_utils.print_dict(metadata._info)
     elif args.action == 'unset':
         snapshot.delete_metadata(list(metadata.keys()))
 
 
 @utils.arg('snapshot', metavar='<snapshot>',
            help='ID of snapshot.')
 def do_snapshot_metadata_show(cs, args):
     """Shows snapshot metadata."""
     snapshot = shell_utils.find_volume_snapshot(cs, args.snapshot)
-    utils.print_dict(snapshot._info['metadata'], 'Metadata-property')
+    shell_utils.print_dict(snapshot._info['metadata'], 'Metadata-property')
 
 
 @utils.arg('volume', metavar='<volume>',
            help='ID of volume.')
 def do_metadata_show(cs, args):
     """Shows volume metadata."""
     volume = utils.find_volume(cs, args.volume)
-    utils.print_dict(volume._info['metadata'], 'Metadata-property')
+    shell_utils.print_dict(volume._info['metadata'], 'Metadata-property')
 
 
 @utils.arg('volume', metavar='<volume>',
            help='ID of volume.')
 def do_image_metadata_show(cs, args):
     """Shows volume image metadata."""
     volume = utils.find_volume(cs, args.volume)
     resp, body = volume.show_image_metadata(volume)
-    utils.print_dict(body['metadata'], 'Metadata-property')
+    shell_utils.print_dict(body['metadata'], 'Metadata-property')
 
 
 @utils.arg('volume',
            metavar='<volume>',
            help='ID of volume for which to update metadata.')
 @utils.arg('metadata',
            metavar='<key=value>',
@@ -1835,15 +1835,15 @@
            default=[],
            help='Metadata key and value pair or pairs to update.')
 def do_metadata_update_all(cs, args):
     """Updates volume metadata."""
     volume = utils.find_volume(cs, args.volume)
     metadata = shell_utils.extract_metadata(args)
     metadata = volume.update_all_metadata(metadata)
-    utils.print_dict(metadata['metadata'], 'Metadata-property')
+    shell_utils.print_dict(metadata['metadata'], 'Metadata-property')
 
 
 @utils.arg('snapshot',
            metavar='<snapshot>',
            help='ID of snapshot for which to update metadata.')
 @utils.arg('metadata',
            metavar='<key=value>',
@@ -1851,15 +1851,15 @@
            default=[],
            help='Metadata key and value pair to update.')
 def do_snapshot_metadata_update_all(cs, args):
     """Updates snapshot metadata."""
     snapshot = shell_utils.find_volume_snapshot(cs, args.snapshot)
     metadata = shell_utils.extract_metadata(args)
     metadata = snapshot.update_all_metadata(metadata)
-    utils.print_dict(metadata)
+    shell_utils.print_dict(metadata)
 
 
 @utils.arg('volume', metavar='<volume>', help='ID of volume to update.')
 @utils.arg('read_only',
            metavar='<True|true|False|false>',
            choices=['True', 'true', 'False', 'false'],
            help='Enables or disables update of volume to '
@@ -1950,15 +1950,15 @@
                                metadata=volume_metadata,
                                bootable=args.bootable)
 
     info = {}
     volume = cs.volumes.get(volume.id)
     info.update(volume._info)
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('volume', metavar='<volume>',
            help='Name or ID of the volume to unmanage.')
 def do_unmanage(cs, args):
     """Stop managing a volume."""
     volume = utils.find_volume(cs, args.volume)
@@ -1974,29 +1974,29 @@
            default=0,
            help='Shows details for all tenants. Admin only.')
 def do_consisgroup_list(cs, args):
     """Lists all consistency groups."""
     consistencygroups = cs.consistencygroups.list()
 
     columns = ['ID', 'Status', 'Name']
-    utils.print_list(consistencygroups, columns)
+    shell_utils.print_list(consistencygroups, columns)
 
 
 @utils.arg('consistencygroup',
            metavar='<consistencygroup>',
            help='Name or ID of a consistency group.')
 def do_consisgroup_show(cs, args):
     """Shows details of a consistency group."""
     info = dict()
     consistencygroup = shell_utils.find_consistencygroup(cs,
                                                          args.consistencygroup)
     info.update(consistencygroup._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('volumetypes',
            metavar='<volume-types>',
            help='Volume types.')
 @utils.arg('--name',
            metavar='<name>',
@@ -2019,15 +2019,15 @@
         availability_zone=args.availability_zone)
 
     info = dict()
     consistencygroup = cs.consistencygroups.get(consistencygroup.id)
     info.update(consistencygroup._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('--cgsnapshot',
            metavar='<cgsnapshot>',
            help='Name or ID of a cgsnapshot. Default=None.')
 @utils.arg('--source-cg',
            metavar='<source-cg>',
@@ -2057,15 +2057,15 @@
     info = cs.consistencygroups.create_from_src(
         cgsnapshot.id if cgsnapshot else None,
         source_cg.id if source_cg else None,
         args.name,
         args.description)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('consistencygroup',
            metavar='<consistencygroup>', nargs='+',
            help='Name or ID of one or more consistency groups '
                 'to be deleted.')
 @utils.arg('--force',
@@ -2162,28 +2162,28 @@
         'status': args.status,
         'consistencygroup_id': args.consistencygroup_id,
     }
 
     cgsnapshots = cs.cgsnapshots.list(search_opts=search_opts)
 
     columns = ['ID', 'Status', 'Name']
-    utils.print_list(cgsnapshots, columns)
+    shell_utils.print_list(cgsnapshots, columns)
 
 
 @utils.arg('cgsnapshot',
            metavar='<cgsnapshot>',
            help='Name or ID of cgsnapshot.')
 def do_cgsnapshot_show(cs, args):
     """Shows cgsnapshot details."""
     info = dict()
     cgsnapshot = shell_utils.find_cgsnapshot(cs, args.cgsnapshot)
     info.update(cgsnapshot._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('consistencygroup',
            metavar='<consistencygroup>',
            help='Name or ID of a consistency group.')
 @utils.arg('--name',
            metavar='<name>',
@@ -2203,15 +2203,15 @@
         args.description)
 
     info = dict()
     cgsnapshot = cs.cgsnapshots.get(cgsnapshot.id)
     info.update(cgsnapshot._info)
 
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('cgsnapshot',
            metavar='<cgsnapshot>', nargs='+',
            help='Name or ID of one or more cgsnapshots to be deleted.')
 def do_cgsnapshot_delete(cs, args):
     """Removes one or more cgsnapshots."""
@@ -2237,32 +2237,32 @@
     infos.update(pools._info)
 
     for info in infos['pools']:
         backend = dict()
         backend['name'] = info['name']
         if args.detail:
             backend.update(info['capabilities'])
-        utils.print_dict(backend)
+        shell_utils.print_dict(backend)
 
 
 @utils.arg('host',
            metavar='<host>',
            help='Cinder host to show backend volume stats and properties; '
                 'takes the form: host@backend-name')
 def do_get_capabilities(cs, args):
     """Show backend volume stats and properties. Admin only."""
 
     capabilities = cs.capabilities.get(args.host)
     infos = dict()
     infos.update(capabilities._info)
 
     prop = infos.pop('properties', None)
-    utils.print_dict(infos, "Volume stats")
-    utils.print_dict(prop, "Backend properties",
-                     formatters=sorted(prop.keys()))
+    shell_utils.print_dict(infos, "Volume stats")
+    shell_utils.print_dict(prop, "Backend properties",
+                           formatters=sorted(prop.keys()))
 
 
 @utils.arg('volume',
            metavar='<volume>',
            help='Cinder volume that already exists in the volume backend.')
 @utils.arg('identifier',
            metavar='<identifier>',
@@ -2304,15 +2304,15 @@
                                           description=args.description,
                                           metadata=snapshot_metadata)
 
     info = {}
     snapshot = cs.volume_snapshots.get(snapshot.id)
     info.update(snapshot._info)
     info.pop('links', None)
-    utils.print_dict(info)
+    shell_utils.print_dict(info)
 
 
 @utils.arg('snapshot', metavar='<snapshot>',
            help='Name or ID of the snapshot to unmanage.')
 def do_snapshot_unmanage(cs, args):
     """Stop managing a snapshot."""
     snapshot = shell_utils.find_volume_snapshot(cs, args.snapshot)
@@ -2374,15 +2374,15 @@
     detailed = strutils.bool_from_string(args.detailed)
     volumes = cs.volumes.list_manageable(host=args.host, detailed=detailed,
                                          marker=args.marker, limit=args.limit,
                                          offset=args.offset, sort=args.sort)
     columns = ['reference', 'size', 'safe_to_manage']
     if detailed:
         columns.extend(['reason_not_safe', 'cinder_id', 'extra_info'])
-    utils.print_list(volumes, columns, sortby_index=None)
+    shell_utils.print_list(volumes, columns, sortby_index=None)
 
 
 @utils.arg('host',
            metavar='<host>',
            help='Cinder host on which to list manageable snapshots; '
                 'takes the form: host@backend-name#pool')
 @utils.arg('--detailed',
@@ -2418,8 +2418,8 @@
                                                     marker=args.marker,
                                                     limit=args.limit,
                                                     offset=args.offset,
                                                     sort=args.sort)
     columns = ['reference', 'size', 'safe_to_manage', 'source_reference']
     if detailed:
         columns.extend(['reason_not_safe', 'cinder_id', 'extra_info'])
-    utils.print_list(snapshots, columns, sortby_index=None)
+    shell_utils.print_list(snapshots, columns, sortby_index=None)
```

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_backups.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_backups.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_backups_restore.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_backups_restore.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_encryption_types.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_encryption_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_snapshots.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_transfers.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_transfers.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_type_access.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_type_access.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volume_types.py` & `python-cinderclient-9.3.0/cinderclient/v3/volume_types.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volumes.py` & `python-cinderclient-9.3.0/cinderclient/v3/volumes.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/volumes_base.py` & `python-cinderclient-9.3.0/cinderclient/v3/volumes_base.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/v3/workers.py` & `python-cinderclient-9.3.0/cinderclient/v3/workers.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/cinderclient/version.py` & `python-cinderclient-9.3.0/cinderclient/version.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/Makefile` & `python-cinderclient-9.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/ext/cli.py` & `python-cinderclient-9.3.0/doc/ext/cli.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/cli/index.rst` & `python-cinderclient-9.3.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/conf.py` & `python-cinderclient-9.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/contributor/contributing.rst` & `python-cinderclient-9.3.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/contributor/functional_tests.rst` & `python-cinderclient-9.3.0/doc/source/contributor/functional_tests.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/contributor/unit_tests.rst` & `python-cinderclient-9.3.0/doc/source/contributor/unit_tests.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/index.rst` & `python-cinderclient-9.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/user/no_auth.rst` & `python-cinderclient-9.3.0/doc/source/user/no_auth.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/doc/source/user/shell.rst` & `python-cinderclient-9.3.0/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/pylintrc` & `python-cinderclient-9.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/python_cinderclient.egg-info/PKG-INFO` & `python-cinderclient-9.3.0/python_cinderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-cinderclient
-Version: 9.2.0
+Version: 9.3.0
 Summary: OpenStack Block Storage API Client Library
 Home-page: https://docs.openstack.org/python-cinderclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-cinderclient-9.2.0/python_cinderclient.egg-info/SOURCES.txt` & `python-cinderclient-9.3.0/python_cinderclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 releasenotes/notes/bug-1995883-force-flag-none-3a7bb87f655bcf42.yaml
 releasenotes/notes/cinder-poll-4f92694cc7eb657a.yaml
 releasenotes/notes/cinderclient-5-de0508ce5a221d21.yaml
 releasenotes/notes/cli-api-ver-negotiation-9f8fd8b77ae299fd.yaml
 releasenotes/notes/cluster_commands-dca50e89c9d53cd2.yaml
 releasenotes/notes/cluster_list_manageable-40c02489b2c95d55.yaml
 releasenotes/notes/cluster_migration_manage-31144d67bbfdb739.yaml
+releasenotes/notes/collect-timing-ce6d521d40d422fb.yaml
 releasenotes/notes/deprecate-allow-multiattach-2213a100c65a95c1.yaml
 releasenotes/notes/do-not-reset-volume-status-ae8e28132d7bfacd.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-fe2dc753e456b527.yaml
 releasenotes/notes/drop-python2-support-d3a1bedc75445edc.yaml
 releasenotes/notes/drop-v2-support-e578ca21c7c6b532.yaml
 releasenotes/notes/enhance-backup-restore-shell-command-0cf55df6ca4b4c55.yaml
 releasenotes/notes/feature-cross-az-backups-9d428ad4dfc552e1.yaml
```

### Comparing `python-cinderclient-9.2.0/releasenotes/notes/cinderclient-5-de0508ce5a221d21.yaml` & `python-cinderclient-9.3.0/releasenotes/notes/cinderclient-5-de0508ce5a221d21.yaml`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/releasenotes/notes/support-bs-mv-3.60-a65f1919b5068d17.yaml` & `python-cinderclient-9.3.0/releasenotes/notes/support-bs-mv-3.60-a65f1919b5068d17.yaml`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/releasenotes/notes/ussuri-release-f0ebfc54cdac6680.yaml` & `python-cinderclient-9.3.0/releasenotes/notes/ussuri-release-f0ebfc54cdac6680.yaml`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/releasenotes/notes/wallaby-release-2535df50cc307fea.yaml` & `python-cinderclient-9.3.0/releasenotes/notes/wallaby-release-2535df50cc307fea.yaml`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/releasenotes/notes/xena-release-688918a69ada3a58.yaml` & `python-cinderclient-9.3.0/releasenotes/notes/xena-release-688918a69ada3a58.yaml`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/releasenotes/source/conf.py` & `python-cinderclient-9.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/setup.cfg` & `python-cinderclient-9.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/setup.py` & `python-cinderclient-9.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/test-requirements.txt` & `python-cinderclient-9.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/tools/cinder.bash_completion` & `python-cinderclient-9.3.0/tools/cinder.bash_completion`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/tools/lintstack.py` & `python-cinderclient-9.3.0/tools/lintstack.py`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/tools/lintstack.sh` & `python-cinderclient-9.3.0/tools/lintstack.sh`

 * *Files identical despite different names*

### Comparing `python-cinderclient-9.2.0/tox.ini` & `python-cinderclient-9.3.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tox]
 distribute = False
 envlist = py3,pep8
 minversion = 3.18.0
+requires = tox<4
 skipsdist = True
 # this allows tox to infer the base python from the environment name
 # and override any basepython configured in this file
 ignore_basepython_conflict=true
 
 [testenv]
 basepython = python3
```

