# Comparing `tmp/twigs-1.1.8.tar.gz` & `tmp/twigs-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twigs-1.1.8.tar", last modified: Tue Mar 22 09:02:35 2022, max compression
+gzip compressed data, was "dist/twigs-1.1.9.tar", last modified: Wed Mar 23 10:13:10 2022, max compression
```

## Comparing `twigs-1.1.8.tar` & `twigs-1.1.9.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/
--rw-r--r--   0 root         (0) root         (0)    32418 2022-03-14 07:03:39.000000 twigs-1.1.8/README.rst
--rw-r--r--   0 root         (0) root         (0)      408 2022-03-22 09:02:35.000000 twigs-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      164 2019-03-18 06:24:28.000000 twigs-1.1.8/AUTHORS.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)       60 2019-03-18 06:24:28.000000 twigs-1.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3513 2021-09-03 05:53:30.000000 twigs-1.1.8/tests/vmware.py
--rw-r--r--   0 root         (0) root         (0)      401 2019-03-18 06:24:28.000000 twigs-1.1.8/tests/test_twigs.py
--rw-r--r--   0 root         (0) root         (0)     3515 2019-03-18 06:24:28.000000 twigs-1.1.8/CONTRIBUTING.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/docs/
--rw-r--r--   0 root         (0) root         (0)      302 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)       33 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      767 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      606 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)       65 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/usage.rst
--rw-r--r--   0 root         (0) root         (0)     1118 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/installation.rst
--rwxr-xr-x   0 root         (0) root         (0)     4786 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       28 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/history.rst
--rw-r--r--   0 root         (0) root         (0)       28 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       27 2019-03-18 06:24:28.000000 twigs-1.1.8/docs/readme.rst
--rw-r--r--   0 root         (0) root         (0)      164 2022-01-23 06:49:20.000000 twigs-1.1.8/HISTORY.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/
--rw-r--r--   0 root         (0) root         (0)     8005 2021-08-10 13:01:39.000000 twigs-1.1.8/twigs/code_secrets_defaults.py
--rw-r--r--   0 root         (0) root         (0)    10905 2021-12-07 03:41:54.000000 twigs-1.1.8/twigs/aws.py
--rw-r--r--   0 root         (0) root         (0)     4575 2021-09-27 07:17:50.000000 twigs-1.1.8/twigs/acr.py
--rw-r--r--   0 root         (0) root         (0)     3433 2021-06-06 04:27:54.000000 twigs-1.1.8/twigs/docker_cis.py
--rwxr-xr-x   0 root         (0) root         (0)   127456 2020-05-10 10:56:25.000000 twigs-1.1.8/twigs/ssh-audit.py
--rw-r--r--   0 root         (0) root         (0)     3549 2021-09-27 07:17:50.000000 twigs-1.1.8/twigs/gcp.py
--rw-r--r--   0 root         (0) root         (0)     1597 2021-06-07 09:55:25.000000 twigs-1.1.8/twigs/azure_cis.py
--rw-r--r--   0 root         (0) root         (0)     6147 2022-01-28 14:09:06.000000 twigs-1.1.8/twigs/plugin_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/gcp_cis_tool/
--rw-r--r--   0 root         (0) root         (0)    11762 2021-09-03 07:11:08.000000 twigs-1.1.8/twigs/gcp_cis_tool/check3.py
--rw-r--r--   0 root         (0) root         (0)    17370 2021-09-30 06:58:44.000000 twigs-1.1.8/twigs/gcp_cis_tool/check1.py
--rw-r--r--   0 root         (0) root         (0)     8045 2021-10-21 05:17:06.000000 twigs-1.1.8/twigs/gcp_cis_tool/gcp_cis_utils.py
--rw-r--r--   0 root         (0) root         (0)    13088 2021-07-06 05:05:05.000000 twigs-1.1.8/twigs/gcp_cis_tool/check4.py
--rw-r--r--   0 root         (0) root         (0)     2543 2021-10-21 13:24:40.000000 twigs-1.1.8/twigs/gcp_cis_tool/gcp_cis.py
--rw-r--r--   0 root         (0) root         (0)    16823 2022-01-05 09:03:13.000000 twigs-1.1.8/twigs/gcp_cis_tool/check2.py
--rw-r--r--   0 root         (0) root         (0)     2057 2021-07-05 14:39:18.000000 twigs-1.1.8/twigs/gcp_cis_tool/check7.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-03-28 06:38:56.000000 twigs-1.1.8/twigs/gcp_cis_tool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2653 2021-06-30 10:28:31.000000 twigs-1.1.8/twigs/gcp_cis_tool/check5.py
--rw-r--r--   0 root         (0) root         (0)    14267 2021-07-05 12:41:41.000000 twigs-1.1.8/twigs/gcp_cis_tool/check6.py
--rwxr-xr-x   0 root         (0) root         (0)    14383 2021-09-27 07:17:50.000000 twigs-1.1.8/twigs/azure.py
--rw-r--r--   0 root         (0) root         (0)      711 2021-06-07 10:50:37.000000 twigs-1.1.8/twigs/gcp_cis.py
--rw-r--r--   0 root         (0) root         (0)     2550 2021-06-08 10:42:26.000000 twigs-1.1.8/twigs/iac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/dast_plugins/
--rw-r--r--   0 root         (0) root         (0)      160 2020-02-14 04:48:23.000000 twigs-1.1.8/twigs/dast_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7641 2022-01-13 10:23:13.000000 twigs-1.1.8/twigs/dast_plugins/skipfish.py
--rw-r--r--   0 root         (0) root         (0)     3225 2020-12-14 10:50:54.000000 twigs-1.1.8/twigs/dast_plugins/arachni.py
--rw-r--r--   0 root         (0) root         (0)    12047 2021-08-25 11:15:31.000000 twigs-1.1.8/twigs/code_secrets.py
--rw-r--r--   0 root         (0) root         (0)      159 2022-03-22 09:02:17.000000 twigs-1.1.8/twigs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2022-01-13 10:56:31.000000 twigs-1.1.8/twigs/plugin_registry.py
--rw-r--r--   0 root         (0) root         (0)     4154 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/k8s_cis.py
--rwxr-xr-x   0 root         (0) root         (0)    60625 2022-03-14 07:01:04.000000 twigs-1.1.8/twigs/twigs.py
--rw-r--r--   0 root         (0) root         (0)     2282 2020-08-11 12:46:59.000000 twigs-1.1.8/twigs/fingerprint.py
--rw-r--r--   0 root         (0) root         (0)     2876 2021-09-27 07:17:56.000000 twigs-1.1.8/twigs/vmware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/
--rw-r--r--   0 root         (0) root         (0)     3373 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_4_1.sh
--rwxr-xr-x   0 root         (0) root         (0)     1190 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/worker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/
--rw-r--r--   0 root         (0) root         (0)     1197 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/3_control_plane_configuration.sh
--rw-r--r--   0 root         (0) root         (0)     2891 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/2_etcd.sh
--rw-r--r--   0 root         (0) root         (0)    25381 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/1_control_plane_components.sh
--rw-r--r--   0 root         (0) root         (0)     4067 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/5_policies.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/worker/
--rw-r--r--   0 root         (0) root         (0)     9503 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/worker/4_worker_nodes.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/
--rwxr-xr-x   0 root         (0) root         (0)      569 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker.sh
--rwxr-xr-x   0 root         (0) root         (0)      825 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/
--rwxr-xr-x   0 root         (0) root         (0)     1763 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_3_contoller_manager.sh
--rwxr-xr-x   0 root         (0) root         (0)    12801 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_1_api_server.sh
--rwxr-xr-x   0 root         (0) root         (0)     9700 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_4_configuration_files.sh
--rwxr-xr-x   0 root         (0) root         (0)      236 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_2_scheduler.sh
--rwxr-xr-x   0 root         (0) root         (0)     1738 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_6_general_security_primitives.sh
--rwxr-xr-x   0 root         (0) root         (0)     2722 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_5_etcd.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation/
--rwxr-xr-x   0 root         (0) root         (0)      258 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_2_controller_manager.sh
--rwxr-xr-x   0 root         (0) root         (0)      201 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation/check_federation.sh
--rwxr-xr-x   0 root         (0) root         (0)     6577 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_1_api_server.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker/
--rwxr-xr-x   0 root         (0) root         (0)     3779 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_2_configure_files.sh
--rwxr-xr-x   0 root         (0) root         (0)     4312 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_1_kubelet.sh
--rwxr-xr-x   0 root         (0) root         (0)      568 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master.sh
--rwxr-xr-x   0 root         (0) root         (0)      703 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/federation.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/
--rwxr-xr-x   0 root         (0) root         (0)     1923 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_3_contoller_manager.sh
--rwxr-xr-x   0 root         (0) root         (0)    11779 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_1_api_server.sh
--rwxr-xr-x   0 root         (0) root         (0)     5111 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_4_configuration_files.sh
--rwxr-xr-x   0 root         (0) root         (0)      236 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_2_scheduler.sh
--rwxr-xr-x   0 root         (0) root         (0)     1609 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_6_general_security_primitives.sh
--rwxr-xr-x   0 root         (0) root         (0)     2722 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_5_etcd.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/federation/
--rwxr-xr-x   0 root         (0) root         (0)      258 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_2_controller_manager.sh
--rwxr-xr-x   0 root         (0) root         (0)      201 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/federation/check_federation.sh
--rwxr-xr-x   0 root         (0) root         (0)     6577 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_1_api_server.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/worker/
--rwxr-xr-x   0 root         (0) root         (0)     2277 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_2_configure_files.sh
--rwxr-xr-x   0 root         (0) root         (0)     4312 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_1_kubelet.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/
--rw-r--r--   0 root         (0) root         (0)     1189 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/3_control_plane_configuration.sh
--rw-r--r--   0 root         (0) root         (0)     2905 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/2_etcd.sh
--rw-r--r--   0 root         (0) root         (0)    25492 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/1_control_plane_components.sh
--rw-r--r--   0 root         (0) root         (0)     3983 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/5_policies.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/worker/
--rw-r--r--   0 root         (0) root         (0)     9521 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/worker/4_worker_nodes.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/
--rw-r--r--   0 root         (0) root         (0)      952 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/3_control_plane_configuration.sh
--rw-r--r--   0 root         (0) root         (0)      833 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/2_etcd.sh
--rw-r--r--   0 root         (0) root         (0)     8677 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/1_control_plane_components.sh
--rw-r--r--   0 root         (0) root         (0)     4488 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/6_managed_services.sh
--rw-r--r--   0 root         (0) root         (0)     3635 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/5_policies.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/worker/
--rw-r--r--   0 root         (0) root         (0)     7043 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/worker/4_worker_nodes.sh
--rw-r--r--   0 root         (0) root         (0)     3227 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_5_1.sh
--rw-r--r--   0 root         (0) root         (0)    11344 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3316 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper_gke.sh
--rw-r--r--   0 root         (0) root         (0)     4511 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_6_0.sh
--rwxr-xr-x   0 root         (0) root         (0)     1688 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/
--rwxr-xr-x   0 root         (0) root         (0)     2487 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_3_contoller_manager.sh
--rwxr-xr-x   0 root         (0) root         (0)    13972 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_1_api_server.sh
--rwxr-xr-x   0 root         (0) root         (0)    11028 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_4_configuration_files.sh
--rwxr-xr-x   0 root         (0) root         (0)      481 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_2_scheduler.sh
--rw-r--r--   0 root         (0) root         (0)     2400 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_7_podSecurityPolicies.sh
--rwxr-xr-x   0 root         (0) root         (0)     1488 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_6_general_security_primitives.sh
--rwxr-xr-x   0 root         (0) root         (0)     2918 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_5_etcd.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/worker/
--rwxr-xr-x   0 root         (0) root         (0)     5099 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_2_configure_files.sh
--rwxr-xr-x   0 root         (0) root         (0)     4955 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_1_kubelet.sh
--rwxr-xr-x   0 root         (0) root         (0)     1340 2022-02-16 07:05:57.000000 twigs-1.1.8/twigs/kubernetes-cis-benchmark/master.sh
--rw-r--r--   0 root         (0) root         (0)    14425 2022-01-13 08:43:26.000000 twigs-1.1.8/twigs/utils.py
--rw-r--r--   0 root         (0) root         (0)    26624 2022-01-14 05:52:13.000000 twigs-1.1.8/twigs/repo.py
--rw-r--r--   0 root         (0) root         (0)     8257 2022-03-22 08:58:51.000000 twigs-1.1.8/twigs/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     2823 2021-09-27 07:17:50.000000 twigs-1.1.8/twigs/gcr.py
--rw-r--r--   0 root         (0) root         (0)    29811 2022-03-10 09:37:48.000000 twigs-1.1.8/twigs/docker.py
--rw-r--r--   0 root         (0) root         (0)     2671 2021-02-27 04:48:56.000000 twigs-1.1.8/twigs/policy.py
--rw-r--r--   0 root         (0) root         (0)     7401 2021-09-27 07:17:50.000000 twigs-1.1.8/twigs/ecr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/plugins/
--rwxr-xr-x   0 root         (0) root         (0)      453 2022-01-11 13:53:04.000000 twigs-1.1.8/twigs/plugins/cve-2021-44832.sh
--rwxr-xr-x   0 root         (0) root         (0)      413 2022-01-11 13:47:01.000000 twigs-1.1.8/twigs/plugins/cve-2021-45105.sh
--rwxr-xr-x   0 root         (0) root         (0)      389 2022-01-11 13:40:30.000000 twigs-1.1.8/twigs/plugins/cve-2021-45046.sh
--rwxr-xr-x   0 root         (0) root         (0)      711 2021-12-30 09:57:54.000000 twigs-1.1.8/twigs/plugins/log4j_common.sh
--rwxr-xr-x   0 root         (0) root         (0)      386 2022-01-11 13:38:24.000000 twigs-1.1.8/twigs/plugins/cve-2021-44228.sh
--rw-r--r--   0 root         (0) root         (0)     1424 2021-06-07 10:07:33.000000 twigs-1.1.8/twigs/dast.py
--rw-r--r--   0 root         (0) root         (0)     5934 2022-03-03 05:43:31.000000 twigs-1.1.8/twigs/azure_functions.py
--rw-r--r--   0 root         (0) root         (0)     4279 2022-01-13 10:00:28.000000 twigs-1.1.8/twigs/aws_cis.py
--rwxr-xr-x   0 root         (0) root         (0)     3569 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/servicenow.py
--rw-r--r--   0 root         (0) root         (0)     3981 2022-01-03 09:55:06.000000 twigs-1.1.8/twigs/gcloud_functions.py
--rw-r--r--   0 root         (0) root         (0)     8503 2021-08-23 15:23:50.000000 twigs-1.1.8/twigs/inv_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs/azure_cis_tool/
--rw-r--r--   0 root         (0) root         (0)     8094 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check2.py
--rw-r--r--   0 root         (0) root         (0)    16397 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check6.py
--rw-r--r--   0 root         (0) root         (0)    53224 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/azure_cis.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-03-12 11:14:02.000000 twigs-1.1.8/twigs/azure_cis_tool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4808 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check7.py
--rw-r--r--   0 root         (0) root         (0)     3753 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check8.py
--rw-r--r--   0 root         (0) root         (0)     7508 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check1.py
--rw-r--r--   0 root         (0) root         (0)      988 2020-03-18 05:48:38.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_utils.py
--rw-r--r--   0 root         (0) root         (0)    10359 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check4.py
--rw-r--r--   0 root         (0) root         (0)     8637 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check5.py
--rw-r--r--   0 root         (0) root         (0)    11957 2020-08-04 06:51:42.000000 twigs-1.1.8/twigs/azure_cis_tool/az_cis_check3.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-01-13 08:03:30.000000 twigs-1.1.8/twigs/sast.py
--rw-r--r--   0 root         (0) root         (0)    22936 2022-03-16 09:23:03.000000 twigs-1.1.8/twigs/linux.py
--rw-r--r--   0 root         (0) root         (0)     7185 2020-05-22 09:50:31.000000 twigs-1.1.8/twigs/gd-ca-bundle.crt
--rw-r--r--   0 root         (0) root         (0)    38723 2022-03-22 09:02:35.000000 twigs-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1556 2019-03-18 06:24:28.000000 twigs-1.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2020-07-17 09:33:05.000000 twigs-1.1.8/twigs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      284 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)    38723 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5867 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-03-22 09:02:35.000000 twigs-1.1.8/twigs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      381 2022-02-16 07:08:37.000000 twigs-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2044 2022-03-22 09:01:53.000000 twigs-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)    32418 2022-03-23 08:16:36.000000 twigs-1.1.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2022-03-23 10:13:10.000000 twigs-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      164 2021-12-24 14:40:09.000000 twigs-1.1.9/AUTHORS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)       60 2021-12-24 14:40:09.000000 twigs-1.1.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2021-12-24 14:40:09.000000 twigs-1.1.9/tests/vmware.py
+-rw-r--r--   0 root         (0) root         (0)      401 2021-12-24 14:40:09.000000 twigs-1.1.9/tests/test_twigs.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2021-12-24 14:40:09.000000 twigs-1.1.9/CONTRIBUTING.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/docs/
+-rw-r--r--   0 root         (0) root         (0)      302 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      767 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      606 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)       65 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/usage.rst
+-rw-r--r--   0 root         (0) root         (0)     1118 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/installation.rst
+-rwxr-xr-x   0 root         (0) root         (0)     4786 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       28 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/history.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       27 2021-12-24 14:40:09.000000 twigs-1.1.9/docs/readme.rst
+-rw-r--r--   0 root         (0) root         (0)      164 2022-03-23 08:16:36.000000 twigs-1.1.9/HISTORY.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/
+-rw-r--r--   0 root         (0) root         (0)     8005 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/code_secrets_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/aws.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/acr.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/docker_cis.py
+-rwxr-xr-x   0 root         (0) root         (0)   127456 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/ssh-audit.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/plugin_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/gcp_cis_tool/
+-rw-r--r--   0 root         (0) root         (0)    11762 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check3.py
+-rw-r--r--   0 root         (0) root         (0)    17370 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check1.py
+-rw-r--r--   0 root         (0) root         (0)     8045 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/gcp_cis_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13088 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check4.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/gcp_cis.py
+-rw-r--r--   0 root         (0) root         (0)    16823 2022-01-12 09:32:24.000000 twigs-1.1.9/twigs/gcp_cis_tool/check2.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check7.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check5.py
+-rw-r--r--   0 root         (0) root         (0)    14267 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis_tool/check6.py
+-rwxr-xr-x   0 root         (0) root         (0)    14383 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure.py
+-rw-r--r--   0 root         (0) root         (0)      711 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcp_cis.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/iac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/dast_plugins/
+-rw-r--r--   0 root         (0) root         (0)      160 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/dast_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/dast_plugins/skipfish.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/dast_plugins/arachni.py
+-rw-r--r--   0 root         (0) root         (0)    12047 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/code_secrets.py
+-rw-r--r--   0 root         (0) root         (0)      159 2022-03-23 10:04:08.000000 twigs-1.1.9/twigs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/plugin_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/k8s_cis.py
+-rwxr-xr-x   0 root         (0) root         (0)    60625 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/twigs.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/fingerprint.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/vmware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/
+-rw-r--r--   0 root         (0) root         (0)     3373 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_4_1.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1190 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/worker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/
+-rw-r--r--   0 root         (0) root         (0)     1197 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/3_control_plane_configuration.sh
+-rw-r--r--   0 root         (0) root         (0)     2891 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/2_etcd.sh
+-rw-r--r--   0 root         (0) root         (0)    25381 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/1_control_plane_components.sh
+-rw-r--r--   0 root         (0) root         (0)     4067 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/5_policies.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/worker/
+-rw-r--r--   0 root         (0) root         (0)     9503 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/worker/4_worker_nodes.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)      569 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker.sh
+-rwxr-xr-x   0 root         (0) root         (0)      825 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/
+-rwxr-xr-x   0 root         (0) root         (0)     1763 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_3_contoller_manager.sh
+-rwxr-xr-x   0 root         (0) root         (0)    12801 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_1_api_server.sh
+-rwxr-xr-x   0 root         (0) root         (0)     9700 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_4_configuration_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)      236 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_2_scheduler.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1738 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_6_general_security_primitives.sh
+-rwxr-xr-x   0 root         (0) root         (0)     2722 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_5_etcd.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation/
+-rwxr-xr-x   0 root         (0) root         (0)      258 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_2_controller_manager.sh
+-rwxr-xr-x   0 root         (0) root         (0)      201 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation/check_federation.sh
+-rwxr-xr-x   0 root         (0) root         (0)     6577 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_1_api_server.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker/
+-rwxr-xr-x   0 root         (0) root         (0)     3779 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_2_configure_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4312 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_1_kubelet.sh
+-rwxr-xr-x   0 root         (0) root         (0)      568 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master.sh
+-rwxr-xr-x   0 root         (0) root         (0)      703 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/federation.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/
+-rwxr-xr-x   0 root         (0) root         (0)     1923 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_3_contoller_manager.sh
+-rwxr-xr-x   0 root         (0) root         (0)    11779 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_1_api_server.sh
+-rwxr-xr-x   0 root         (0) root         (0)     5111 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_4_configuration_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)      236 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_2_scheduler.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1609 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_6_general_security_primitives.sh
+-rwxr-xr-x   0 root         (0) root         (0)     2722 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_5_etcd.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/federation/
+-rwxr-xr-x   0 root         (0) root         (0)      258 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_2_controller_manager.sh
+-rwxr-xr-x   0 root         (0) root         (0)      201 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/federation/check_federation.sh
+-rwxr-xr-x   0 root         (0) root         (0)     6577 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_1_api_server.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/worker/
+-rwxr-xr-x   0 root         (0) root         (0)     2277 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_2_configure_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4312 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_1_kubelet.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/
+-rw-r--r--   0 root         (0) root         (0)     1189 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/3_control_plane_configuration.sh
+-rw-r--r--   0 root         (0) root         (0)     2905 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/2_etcd.sh
+-rw-r--r--   0 root         (0) root         (0)    25492 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/1_control_plane_components.sh
+-rw-r--r--   0 root         (0) root         (0)     3983 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/5_policies.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/worker/
+-rw-r--r--   0 root         (0) root         (0)     9521 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/worker/4_worker_nodes.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/
+-rw-r--r--   0 root         (0) root         (0)      952 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/3_control_plane_configuration.sh
+-rw-r--r--   0 root         (0) root         (0)      833 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/2_etcd.sh
+-rw-r--r--   0 root         (0) root         (0)     8677 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/1_control_plane_components.sh
+-rw-r--r--   0 root         (0) root         (0)     4488 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/6_managed_services.sh
+-rw-r--r--   0 root         (0) root         (0)     3635 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/5_policies.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/worker/
+-rw-r--r--   0 root         (0) root         (0)     7043 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/worker/4_worker_nodes.sh
+-rw-r--r--   0 root         (0) root         (0)     3227 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_5_1.sh
+-rw-r--r--   0 root         (0) root         (0)    11344 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3316 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper_gke.sh
+-rw-r--r--   0 root         (0) root         (0)     4511 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_6_0.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1688 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/
+-rwxr-xr-x   0 root         (0) root         (0)     2487 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_3_contoller_manager.sh
+-rwxr-xr-x   0 root         (0) root         (0)    13972 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_1_api_server.sh
+-rwxr-xr-x   0 root         (0) root         (0)    11028 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_4_configuration_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)      481 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_2_scheduler.sh
+-rw-r--r--   0 root         (0) root         (0)     2400 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_7_podSecurityPolicies.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1488 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_6_general_security_primitives.sh
+-rwxr-xr-x   0 root         (0) root         (0)     2918 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_5_etcd.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/worker/
+-rwxr-xr-x   0 root         (0) root         (0)     5099 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_2_configure_files.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4955 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_1_kubelet.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1340 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/kubernetes-cis-benchmark/master.sh
+-rw-r--r--   0 root         (0) root         (0)    14425 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/utils.py
+-rw-r--r--   0 root         (0) root         (0)    26624 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/repo.py
+-rw-r--r--   0 root         (0) root         (0)     8799 2022-03-23 10:02:31.000000 twigs-1.1.9/twigs/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gcr.py
+-rw-r--r--   0 root         (0) root         (0)    29811 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/policy.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/ecr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)      453 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/plugins/cve-2021-44832.sh
+-rwxr-xr-x   0 root         (0) root         (0)      413 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/plugins/cve-2021-45105.sh
+-rwxr-xr-x   0 root         (0) root         (0)      389 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/plugins/cve-2021-45046.sh
+-rwxr-xr-x   0 root         (0) root         (0)      711 2022-01-12 09:32:24.000000 twigs-1.1.9/twigs/plugins/log4j_common.sh
+-rwxr-xr-x   0 root         (0) root         (0)      386 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/plugins/cve-2021-44228.sh
+-rw-r--r--   0 root         (0) root         (0)     1424 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/dast.py
+-rw-r--r--   0 root         (0) root         (0)     5934 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/azure_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/aws_cis.py
+-rwxr-xr-x   0 root         (0) root         (0)     3569 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/servicenow.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2022-01-03 09:27:05.000000 twigs-1.1.9/twigs/gcloud_functions.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/inv_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs/azure_cis_tool/
+-rw-r--r--   0 root         (0) root         (0)     8094 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check2.py
+-rw-r--r--   0 root         (0) root         (0)    16397 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check6.py
+-rw-r--r--   0 root         (0) root         (0)    53224 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/azure_cis.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check7.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check8.py
+-rw-r--r--   0 root         (0) root         (0)     7508 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check1.py
+-rw-r--r--   0 root         (0) root         (0)      988 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10359 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check4.py
+-rw-r--r--   0 root         (0) root         (0)     8637 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check5.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/azure_cis_tool/az_cis_check3.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2022-01-14 09:48:22.000000 twigs-1.1.9/twigs/sast.py
+-rw-r--r--   0 root         (0) root         (0)    22936 2022-03-23 08:16:36.000000 twigs-1.1.9/twigs/linux.py
+-rw-r--r--   0 root         (0) root         (0)     7185 2021-12-24 14:40:09.000000 twigs-1.1.9/twigs/gd-ca-bundle.crt
+-rw-r--r--   0 root         (0) root         (0)    38723 2022-03-23 10:13:10.000000 twigs-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1556 2021-12-24 14:40:09.000000 twigs-1.1.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-24 14:44:12.000000 twigs-1.1.9/twigs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      284 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)    38723 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5867 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-03-23 10:13:10.000000 twigs-1.1.9/twigs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2022-03-23 08:16:36.000000 twigs-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-03-23 10:03:46.000000 twigs-1.1.9/setup.py
```

### Comparing `twigs-1.1.8/README.rst` & `twigs-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/tests/vmware.py` & `twigs-1.1.9/tests/vmware.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/CONTRIBUTING.rst` & `twigs-1.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/docs/make.bat` & `twigs-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/docs/Makefile` & `twigs-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/docs/installation.rst` & `twigs-1.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/docs/conf.py` & `twigs-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/code_secrets_defaults.py` & `twigs-1.1.9/twigs/code_secrets_defaults.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/aws.py` & `twigs-1.1.9/twigs/aws.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/acr.py` & `twigs-1.1.9/twigs/acr.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/docker_cis.py` & `twigs-1.1.9/twigs/docker_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/ssh-audit.py` & `twigs-1.1.9/twigs/ssh-audit.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp.py` & `twigs-1.1.9/twigs/gcp.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis.py` & `twigs-1.1.9/twigs/azure_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/plugin_processor.py` & `twigs-1.1.9/twigs/plugin_processor.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check3.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check3.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check1.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check1.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/gcp_cis_utils.py` & `twigs-1.1.9/twigs/gcp_cis_tool/gcp_cis_utils.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check4.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check4.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/gcp_cis.py` & `twigs-1.1.9/twigs/gcp_cis_tool/gcp_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check2.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check2.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check7.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check7.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check5.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check5.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis_tool/check6.py` & `twigs-1.1.9/twigs/gcp_cis_tool/check6.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure.py` & `twigs-1.1.9/twigs/azure.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcp_cis.py` & `twigs-1.1.9/twigs/gcp_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/iac.py` & `twigs-1.1.9/twigs/iac.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/dast_plugins/skipfish.py` & `twigs-1.1.9/twigs/dast_plugins/skipfish.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/dast_plugins/arachni.py` & `twigs-1.1.9/twigs/dast_plugins/arachni.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/code_secrets.py` & `twigs-1.1.9/twigs/code_secrets.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/plugin_registry.py` & `twigs-1.1.9/twigs/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/k8s_cis.py` & `twigs-1.1.9/twigs/k8s_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/twigs.py` & `twigs-1.1.9/twigs/twigs.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/fingerprint.py` & `twigs-1.1.9/twigs/fingerprint.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/vmware.py` & `twigs-1.1.9/twigs/vmware.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_4_1.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_4_1.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/worker.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/worker.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/3_control_plane_configuration.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/3_control_plane_configuration.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/2_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/2_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/1_control_plane_components.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/1_control_plane_components.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/master/5_policies.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/master/5_policies.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.5.1/worker/4_worker_nodes.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.5.1/worker/4_worker_nodes.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_3_contoller_manager.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_3_contoller_manager.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_1_api_server.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_1_api_server.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_4_configuration_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_4_configuration_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_6_general_security_primitives.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_6_general_security_primitives.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master/master_5_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master/master_5_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_1_api_server.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/federation/federation_1_api_server.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_2_configure_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_2_configure_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_1_kubelet.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/worker/worker_1_kubelet.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.2.0/master.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.2.0/master.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/federation.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/federation.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_3_contoller_manager.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_3_contoller_manager.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_1_api_server.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_1_api_server.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_4_configuration_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_4_configuration_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_6_general_security_primitives.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_6_general_security_primitives.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/master/master_5_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/master/master_5_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_1_api_server.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/federation/federation_1_api_server.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_2_configure_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_2_configure_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_1_kubelet.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.0.0/worker/worker_1_kubelet.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/3_control_plane_configuration.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/3_control_plane_configuration.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/2_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/2_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/1_control_plane_components.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/1_control_plane_components.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/master/5_policies.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/master/5_policies.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.6.0/worker/4_worker_nodes.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.6.0/worker/4_worker_nodes.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/3_control_plane_configuration.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/3_control_plane_configuration.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/2_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/2_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/1_control_plane_components.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/1_control_plane_components.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/6_managed_services.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/6_managed_services.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/master/5_policies.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/master/5_policies.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/gke/worker/4_worker_nodes.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/gke/worker/4_worker_nodes.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_5_1.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_5_1.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/LICENSE` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/LICENSE`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper_gke.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper_gke.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper1_6_0.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper1_6_0.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/helper.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/helper.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_3_contoller_manager.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_3_contoller_manager.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_1_api_server.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_1_api_server.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_4_configuration_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_4_configuration_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_7_podSecurityPolicies.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_7_podSecurityPolicies.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_6_general_security_primitives.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_6_general_security_primitives.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/master/master_5_etcd.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/master/master_5_etcd.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_2_configure_files.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_2_configure_files.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_1_kubelet.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/1.4.1/worker/worker_1_kubelet.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes-cis-benchmark/master.sh` & `twigs-1.1.9/twigs/kubernetes-cis-benchmark/master.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/utils.py` & `twigs-1.1.9/twigs/utils.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/repo.py` & `twigs-1.1.9/twigs/repo.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/kubernetes.py` & `twigs-1.1.9/twigs/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 import yaml
 import uuid
 import tempfile
 
 from . import utils as lib_utils
 from . import docker
 
+def get_helm_command_path():
+    HELM_CMD = os.environ.get('HELM_PATH')
+    if HELM_CMD is None:
+        HELM_CMD = "/usr/local/bin/helm"
+    else:
+        if os.path.isfile(HELM_CMD) == False:
+            logging.error("Helm command not found at specified HELM_PATH [%s]", HELM_CMD)
+            sys.exit(1)
+        elif os.access(HELM_CMD, os.X_OK) == False:
+            logging.error("Helm command file [%s] is not an executable", HELM_CMD)
+            sys.exit(1)
+    return HELM_CMD
+
 def get_deployment_name(yaml_json):
     if yaml_json.get('metadata') is None:
         return None
     namespace = yaml_json['metadata'].get('namespace')
     deployment_name = yaml_json['metadata'].get('name')
     return namespace, deployment_name
 
@@ -121,32 +134,33 @@
             extra_tags.append("InitContainer")
             allassets = allassets + discover_containers(args, init_container_list, asset_name, namespace, deployment_name, kind, extra_tags)
 
     return allassets
 
 def run_helm_command(cmdarr, encoding):
     try:
+        logging.debug("Running command %s", cmdarr)
         out = subprocess.check_output(cmdarr, shell=True)
         return out.decode(encoding)
     except subprocess.CalledProcessError as e:
         logging.error("Error running Helm command")
         logging.debug("[helm] command: %s", cmdarr[0])
         logging.debug("Output of [helm] command: %s", e.output)
         return None
 
 def discover_assets_from_helm_chart(args, helm_chart):
     allassets = []
     hc_name = None
     hc_version = None
     hc_type = None
-    HELM_CMD = "/usr/local/bin/helm"
     temp_template = uuid.uuid4().hex
     temp_template = tempfile.gettempdir() + os.path.sep + temp_template + ".yaml"
     if os.path.isfile(temp_template):
         os.remove(temp_template)
+    HELM_CMD = get_helm_command_path()
     cmdarr = [ HELM_CMD + " show chart " + helm_chart + " > " + temp_template ]
     cmd_output = run_helm_command(cmdarr, args.encoding)
     if cmd_output is None:
         logging.error("Unable to get Chart.yaml")
         return allassets
     with open(temp_template, 'r') as chart_yaml_fd:
         yaml_json = yaml.load(chart_yaml_fd, Loader=yaml.FullLoader)
```

### Comparing `twigs-1.1.8/twigs/gcr.py` & `twigs-1.1.9/twigs/gcr.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/docker.py` & `twigs-1.1.9/twigs/docker.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/policy.py` & `twigs-1.1.9/twigs/policy.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/ecr.py` & `twigs-1.1.9/twigs/ecr.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/plugins/log4j_common.sh` & `twigs-1.1.9/twigs/plugins/log4j_common.sh`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/dast.py` & `twigs-1.1.9/twigs/dast.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_functions.py` & `twigs-1.1.9/twigs/azure_functions.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/aws_cis.py` & `twigs-1.1.9/twigs/aws_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/servicenow.py` & `twigs-1.1.9/twigs/servicenow.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gcloud_functions.py` & `twigs-1.1.9/twigs/gcloud_functions.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/inv_file.py` & `twigs-1.1.9/twigs/inv_file.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check2.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check2.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check6.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check6.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/azure_cis.py` & `twigs-1.1.9/twigs/azure_cis_tool/azure_cis.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check7.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check7.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check8.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check8.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check1.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check1.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_utils.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_utils.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check4.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check4.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check5.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check5.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/azure_cis_tool/az_cis_check3.py` & `twigs-1.1.9/twigs/azure_cis_tool/az_cis_check3.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/sast.py` & `twigs-1.1.9/twigs/sast.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/linux.py` & `twigs-1.1.9/twigs/linux.py`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs/gd-ca-bundle.crt` & `twigs-1.1.9/twigs/gd-ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/PKG-INFO` & `twigs-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: twigs
-Version: 1.1.8
+Version: 1.1.9
 Summary: ThreatWatch Information Gathering Script
 Home-page: https://github.com/threatwatch/twigs
 Author: Paresh Borkar
 Author-email: opensource@threatwatch.io
 License: GNU General Public License v3
 Description: =====
         twigs
```

### Comparing `twigs-1.1.8/LICENSE` & `twigs-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/twigs.egg-info/PKG-INFO` & `twigs-1.1.9/twigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: twigs
-Version: 1.1.8
+Version: 1.1.9
 Summary: ThreatWatch Information Gathering Script
 Home-page: https://github.com/threatwatch/twigs
 Author: Paresh Borkar
 Author-email: opensource@threatwatch.io
 License: GNU General Public License v3
 Description: =====
         twigs
```

### Comparing `twigs-1.1.8/twigs.egg-info/SOURCES.txt` & `twigs-1.1.9/twigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twigs-1.1.8/setup.py` & `twigs-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     keywords='twigs',
     name='twigs',
     packages=find_packages(include=['twigs', 'twigs.dast_plugins', 'twigs.azure_cis_tool', 'twigs.gcp_cis_tool']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/threatwatch/twigs',
-    version='1.1.8',
+    version='1.1.9',
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'twigs=twigs.twigs:main',
         ],
     },
 )
```

