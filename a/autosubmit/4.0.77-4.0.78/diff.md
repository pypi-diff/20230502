# Comparing `tmp/autosubmit-4.0.77.tar.gz` & `tmp/autosubmit-4.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit-4.0.77.tar", last modified: Tue May  2 08:29:58 2023, max compression
+gzip compressed data, was "autosubmit-4.0.78.tar", last modified: Tue May  2 09:03:56 2023, max compression
```

## Comparing `autosubmit-4.0.77.tar` & `autosubmit-4.0.78.tar`

### file list

```diff
@@ -1,405 +1,405 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.gitlab-ci.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      629 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.readthedocs.yaml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-04-27 12:24:09.000000 autosubmit-4.0.77/CONTRIBUTING.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.77/LICENSE
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.77/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 08:29:58.192849 autosubmit-4.0.77/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-04-27 12:24:09.000000 autosubmit-4.0.77/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-04-27 12:24:09.000000 autosubmit-4.0.77/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-05-02 08:29:32.000000 autosubmit-4.0.77/VERSION
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   318778 2023-05-02 07:56:09.000000 autosubmit-4.0.77/autosubmit/autosubmit.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/database/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/database/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/database/data/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/database/data/autosubmit.sql
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_structure.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/experiment/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/experiment/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/experiment/experiment_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/experiment/statistics.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/git/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/git/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-04-27 12:55:41.000000 autosubmit-4.0.77/autosubmit/git/autosubmit_git.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/helpers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/helpers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/autosubmit_helper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/data_transfer.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/history/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/data_classes/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/data_classes/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/data_classes/experiment_run.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/data_classes/job_data.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/database_managers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/database_managers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/database_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/database_models.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/experiment_status_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/experiment_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/experiment_status.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/internal_logging.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/platform_monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/pending.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_utils.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor_item.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/job/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/job/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93132 2023-04-28 13:09:09.000000 autosubmit-4.0.77/autosubmit/job/job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20050 2023-04-28 13:02:46.000000 autosubmit-4.0.77/autosubmit/job/job_dict.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      995 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_exceptions.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   120598 2023-05-02 07:38:24.000000 autosubmit-4.0.77/autosubmit/job/job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_list_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_package_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62106 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_packager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    36449 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_packages.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/monitor/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/diagram.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/notifications/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/notifications/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/notifications/mail_notifier.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/notifications/notifier.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/ecplatform.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/headers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/headers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ec_cca_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ec_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/local_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/lsf_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs10_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs11_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs12_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pjm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ps_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/sge_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7122 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/slurm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/locplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/lsfplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53639 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11360 2023-04-28 13:58:41.000000 autosubmit-4.0.77/autosubmit/platforms/paramiko_submitter.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/pbsplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    21092 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/pjmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    24934 2023-04-28 14:04:34.000000 autosubmit-4.0.77/autosubmit/platforms/platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/psplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/sgeplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32232 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/slurmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/submitter.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/wrappers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_builder.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7581 2023-04-28 10:58:24.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_factory.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/statistics/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/statistics/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/jobs_stat.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/statistics/stats_summary.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12971 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      419 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/bin/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-04-27 12:24:09.000000 autosubmit-4.0.77/bin/autosubmit
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/Makefile
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.77/docs/autosubmit.pdf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/experiment/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/experiment/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/experiment/fig/fig_experiment.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/experiment/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig1_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig2_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig3_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig4_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig5_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_ev_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_tree_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_tree_2.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/graph/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/graph/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_3.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_4.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/graph/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/log/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/log/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/performance/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/performance/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/performance/fig/fig_performance_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/performance/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/statistics/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/statistics/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/tree/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/tree/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/tree/fig/fig_tree_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/tree/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10119 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/conf.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/devguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/devguide/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/installation/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/installation/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/introduction/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig2.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig3.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/introduction/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/moduledoc/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/autosubmit.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/moduledoc/config.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/database.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/git.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/job.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/monitor.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/platforms.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/qstartguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/qstartguide/dummy.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/qstartguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/troubleshooting/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/changelog.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/error-codes.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/troubleshooting/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/monarch-da.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_0.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/unused_figs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/group_chunk.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/horizontal-vertical.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper_expression.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper_hybrid.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/configure/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-04-28 08:40:38.000000 autosubmit-4.0.77/docs/source/userguide/configure/develop_a_project.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/configure/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/create/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/create/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/manage/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/manage/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/run/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/run/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/wrappers/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/dasim.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/horizontal_remote.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/multiple_wrappers.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/rerun.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-horizontal.png
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-mixed.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      710 2023-04-28 14:08:26.000000 autosubmit-4.0.77/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-04-27 12:24:09.000000 autosubmit-4.0.77/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-04-27 12:24:09.000000 autosubmit-4.0.77/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      448 2023-04-28 14:08:26.000000 autosubmit-4.0.77/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-02 08:29:58.192849 autosubmit-4.0.77/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3051 2023-04-27 12:24:09.000000 autosubmit-4.0.77/setup.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/integration/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/integration/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/integration/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/integration/test_job.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/README
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/db/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/db/.gitignore
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/default_conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/default_conf/platforms.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.77/test/regression/tests.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/tests_commands.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_runner.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/unit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.77/test/unit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_basic_config.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_catlog.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/unit/test_chunk_date_lib.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_database_managers.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22797 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_dic_jobs.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2729 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_expid.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12868 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47670 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_graph.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59460 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2374 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_package.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_machinefiles_wrapper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_pjm.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2177 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_slurm_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81586 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_wrappers.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.927403 autosubmit-4.0.78/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-04-27 12:24:09.000000 autosubmit-4.0.78/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-04-27 12:24:09.000000 autosubmit-4.0.78/.gitlab-ci.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      629 2023-04-27 12:24:09.000000 autosubmit-4.0.78/.readthedocs.yaml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.78/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-04-27 12:24:09.000000 autosubmit-4.0.78/CONTRIBUTING.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.78/LICENSE
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.78/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 09:03:56.927403 autosubmit-4.0.78/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-04-27 12:24:09.000000 autosubmit-4.0.78/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-04-27 12:24:09.000000 autosubmit-4.0.78/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-05-02 09:03:39.000000 autosubmit-4.0.78/VERSION
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/autosubmit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   318778 2023-05-02 07:56:09.000000 autosubmit-4.0.78/autosubmit/autosubmit.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/database/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/database/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/database/data/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/database/data/autosubmit.sql
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/database/db_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/database/db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/database/db_structure.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/experiment/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/experiment/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/experiment/experiment_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/experiment/statistics.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/git/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/git/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-04-27 12:55:41.000000 autosubmit-4.0.78/autosubmit/git/autosubmit_git.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/helpers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.78/autosubmit/helpers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/helpers/autosubmit_helper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/helpers/data_transfer.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/helpers/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/history/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/history/data_classes/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/data_classes/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/data_classes/experiment_run.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/data_classes/job_data.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/history/database_managers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/database_managers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/database_managers/database_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/database_managers/database_models.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/database_managers/experiment_status_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/experiment_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/experiment_status.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/internal_logging.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/history/platform_monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/pending.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/platform_utils.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/slurm_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/platform_monitor/slurm_monitor_item.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/history/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/job/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/job/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93132 2023-04-28 13:09:09.000000 autosubmit-4.0.78/autosubmit/job/job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20050 2023-04-28 13:02:46.000000 autosubmit-4.0.78/autosubmit/job/job_dict.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      995 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_exceptions.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   120598 2023-05-02 07:38:24.000000 autosubmit-4.0.78/autosubmit/job/job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_list_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_package_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62106 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_packager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    36449 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_packages.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/job/job_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/monitor/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/monitor/diagram.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/monitor/monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/monitor/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/notifications/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/notifications/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/notifications/mail_notifier.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/notifications/notifier.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit/platforms/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/platforms/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/ecplatform.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/autosubmit/platforms/headers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/platforms/headers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/ec_cca_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/ec_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/local_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/lsf_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/pbs10_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/pbs11_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/pbs12_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/pjm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/ps_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/sge_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7122 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/headers/slurm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/locplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/lsfplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53639 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11360 2023-04-28 13:58:41.000000 autosubmit-4.0.78/autosubmit/platforms/paramiko_submitter.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/pbsplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    21092 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/pjmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    24934 2023-04-28 14:04:34.000000 autosubmit-4.0.78/autosubmit/platforms/platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/psplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/sgeplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32232 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/slurmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/submitter.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/autosubmit/platforms/wrappers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/autosubmit/platforms/wrappers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/platforms/wrappers/wrapper_builder.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7581 2023-04-28 10:58:24.000000 autosubmit-4.0.78/autosubmit/platforms/wrappers/wrapper_factory.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/autosubmit/statistics/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.78/autosubmit/statistics/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/statistics/jobs_stat.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/statistics/statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-02-02 09:02:16.000000 autosubmit-4.0.78/autosubmit/statistics/stats_summary.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-04-27 12:24:09.000000 autosubmit-4.0.78/autosubmit/statistics/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.903404 autosubmit-4.0.78/autosubmit.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 09:03:56.000000 autosubmit-4.0.78/autosubmit.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12971 2023-05-02 09:03:56.000000 autosubmit-4.0.78/autosubmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-02 09:03:56.000000 autosubmit-4.0.78/autosubmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      459 2023-05-02 09:03:56.000000 autosubmit-4.0.78/autosubmit.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-05-02 09:03:56.000000 autosubmit-4.0.78/autosubmit.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/bin/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-04-27 12:24:09.000000 autosubmit-4.0.78/bin/autosubmit
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/Makefile
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.78/docs/autosubmit.pdf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/agui/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/agui/experiment/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/agui/experiment/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/experiment/fig/fig_experiment.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/agui/experiment/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/agui/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig1_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig2_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig3_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig4_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig5_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig_ev_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig_tree_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/fig/fig_tree_2.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.907404 autosubmit-4.0.78/docs/source/agui/graph/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/graph/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_3.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_4.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/agui/graph/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/agui/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/log/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/log/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/log/fig/fig_log_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/log/fig/fig_log_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/log/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/performance/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/performance/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/performance/fig/fig_performance_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/performance/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/statistics/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/statistics/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/statistics/fig/fig_stat_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/statistics/fig/fig_stat_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/statistics/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/tree/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/agui/tree/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/agui/tree/fig/fig_tree_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/agui/tree/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10119 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/conf.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/devguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/devguide/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/installation/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/installation/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/introduction/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/introduction/fig1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/introduction/fig2.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/introduction/fig3.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/introduction/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/moduledoc/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/autosubmit.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/moduledoc/config.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/database.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/git.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/job.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/monitor.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/moduledoc/platforms.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/qstartguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/qstartguide/dummy.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/qstartguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.911404 autosubmit-4.0.78/docs/source/troubleshooting/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/changelog.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/error-codes.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/troubleshooting/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/fig/monarch-da.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/fig/new_dependencies_0.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/fig/new_dependencies_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/troubleshooting/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/unused_figs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/unused_figs/group_chunk.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/unused_figs/horizontal-vertical.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/unused_figs/wrapper.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/unused_figs/wrapper_expression.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/unused_figs/wrapper_hybrid.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/configure/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-04-28 08:40:38.000000 autosubmit-4.0.78/docs/source/userguide/configure/develop_a_project.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/configure/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/create/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/create/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/manage/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/manage/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/run/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/run/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/wrappers/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.915403 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/dasim.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/horizontal_remote.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/multiple_wrappers.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/rerun.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/vertical-horizontal.png
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-02-02 09:02:16.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/fig/vertical-mixed.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-04-27 12:24:09.000000 autosubmit-4.0.78/docs/source/userguide/wrappers/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      710 2023-04-28 14:08:26.000000 autosubmit-4.0.78/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.78/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-04-27 12:24:09.000000 autosubmit-4.0.78/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-04-27 12:24:09.000000 autosubmit-4.0.78/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      448 2023-04-28 14:08:26.000000 autosubmit-4.0.78/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-02 09:03:56.927403 autosubmit-4.0.78/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3098 2023-05-02 09:03:12.000000 autosubmit-4.0.78/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/integration/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/integration/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/integration/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/integration/test_job.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/README
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/db/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/db/.gitignore
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/default_conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/default_conf/platforms.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.919403 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.899404 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.923403 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.78/test/regression/tests.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/regression/tests_commands.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/tests_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/tests_runner.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/regression/tests_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 09:03:56.927403 autosubmit-4.0.78/test/unit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.78/test/unit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_basic_config.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_catlog.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.78/test/unit/test_chunk_date_lib.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_database_managers.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22797 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_dic_jobs.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2729 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_expid.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12868 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47670 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job_graph.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59460 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2374 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_job_package.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_machinefiles_wrapper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_pjm.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2177 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_slurm_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81586 2023-04-27 12:24:09.000000 autosubmit-4.0.78/test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.77/.gitlab-ci.yml` & `autosubmit-4.0.78/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/.readthedocs.yaml` & `autosubmit-4.0.78/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/CONTRIBUTING.md` & `autosubmit-4.0.78/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/LICENSE` & `autosubmit-4.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/PKG-INFO` & `autosubmit-4.0.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.77
+Version: 4.0.78
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.77/README.md` & `autosubmit-4.0.78/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/README_PIP.md` & `autosubmit-4.0.78/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/autosubmit.py` & `autosubmit-4.0.78/autosubmit/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/database/db_common.py` & `autosubmit-4.0.78/autosubmit/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/database/db_manager.py` & `autosubmit-4.0.78/autosubmit/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/database/db_structure.py` & `autosubmit-4.0.78/autosubmit/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/experiment/experiment_common.py` & `autosubmit-4.0.78/autosubmit/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/experiment/statistics.py` & `autosubmit-4.0.78/autosubmit/experiment/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/git/autosubmit_git.py` & `autosubmit-4.0.78/autosubmit/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/helpers/autosubmit_helper.py` & `autosubmit-4.0.78/autosubmit/helpers/autosubmit_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/helpers/utils.py` & `autosubmit-4.0.78/autosubmit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/data_classes/experiment_run.py` & `autosubmit-4.0.78/autosubmit/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/data_classes/job_data.py` & `autosubmit-4.0.78/autosubmit/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/database_managers/database_manager.py` & `autosubmit-4.0.78/autosubmit/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/database_managers/database_models.py` & `autosubmit-4.0.78/autosubmit/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/database_managers/experiment_history_db_manager.py` & `autosubmit-4.0.78/autosubmit/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/database_managers/experiment_status_db_manager.py` & `autosubmit-4.0.78/autosubmit/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/experiment_history.py` & `autosubmit-4.0.78/autosubmit/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/experiment_status.py` & `autosubmit-4.0.78/autosubmit/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/internal_logging.py` & `autosubmit-4.0.78/autosubmit/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper1.txt` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper1.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper2.txt` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper2.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_monitor.py` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_utils.py` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor.py` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor_item.py` & `autosubmit-4.0.78/autosubmit/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/strategies.py` & `autosubmit-4.0.78/autosubmit/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/history/utils.py` & `autosubmit-4.0.78/autosubmit/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job.py` & `autosubmit-4.0.78/autosubmit/job/job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_common.py` & `autosubmit-4.0.78/autosubmit/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_dict.py` & `autosubmit-4.0.78/autosubmit/job/job_dict.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_exceptions.py` & `autosubmit-4.0.78/autosubmit/job/job_exceptions.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_grouping.py` & `autosubmit-4.0.78/autosubmit/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_list.py` & `autosubmit-4.0.78/autosubmit/job/job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_list_persistence.py` & `autosubmit-4.0.78/autosubmit/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_package_persistence.py` & `autosubmit-4.0.78/autosubmit/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_packager.py` & `autosubmit-4.0.78/autosubmit/job/job_packager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_packages.py` & `autosubmit-4.0.78/autosubmit/job/job_packages.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/job/job_utils.py` & `autosubmit-4.0.78/autosubmit/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/monitor/diagram.py` & `autosubmit-4.0.78/autosubmit/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/monitor/monitor.py` & `autosubmit-4.0.78/autosubmit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/monitor/utils.py` & `autosubmit-4.0.78/autosubmit/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/notifications/mail_notifier.py` & `autosubmit-4.0.78/autosubmit/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/notifications/notifier.py` & `autosubmit-4.0.78/autosubmit/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/ecplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/ec_cca_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/ec_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/local_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/lsf_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/pbs10_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/pbs11_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/pbs12_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/pjm_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/pjm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/ps_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/sge_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/headers/slurm_header.py` & `autosubmit-4.0.78/autosubmit/platforms/headers/slurm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/locplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/lsfplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/paramiko_platform.py` & `autosubmit-4.0.78/autosubmit/platforms/paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/paramiko_submitter.py` & `autosubmit-4.0.78/autosubmit/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/pbsplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/pjmplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/pjmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/platform.py` & `autosubmit-4.0.78/autosubmit/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/psplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/sgeplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/slurmplatform.py` & `autosubmit-4.0.78/autosubmit/platforms/slurmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/submitter.py` & `autosubmit-4.0.78/autosubmit/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_builder.py` & `autosubmit-4.0.78/autosubmit/platforms/wrappers/wrapper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_factory.py` & `autosubmit-4.0.78/autosubmit/platforms/wrappers/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/statistics/jobs_stat.py` & `autosubmit-4.0.78/autosubmit/statistics/jobs_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/statistics/statistics.py` & `autosubmit-4.0.78/autosubmit/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/statistics/stats_summary.py` & `autosubmit-4.0.78/autosubmit/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit/statistics/utils.py` & `autosubmit-4.0.78/autosubmit/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/autosubmit.egg-info/PKG-INFO` & `autosubmit-4.0.78/autosubmit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.77
+Version: 4.0.78
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
```

### Comparing `autosubmit-4.0.77/autosubmit.egg-info/SOURCES.txt` & `autosubmit-4.0.78/autosubmit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/bin/autosubmit` & `autosubmit-4.0.78/bin/autosubmit`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/Makefile` & `autosubmit-4.0.78/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/autosubmit.pdf` & `autosubmit-4.0.78/docs/autosubmit.pdf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/experiment/fig/fig_experiment.jpg` & `autosubmit-4.0.78/docs/source/agui/experiment/fig/fig_experiment.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/experiment/index.rst` & `autosubmit-4.0.78/docs/source/agui/experiment/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig1_gui.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig1_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig2_gui.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig2_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig3_gui.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig3_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig4_gui.jpg` & `autosubmit-4.0.78/docs/source/agui/fig/fig4_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig5_gui.jpg` & `autosubmit-4.0.78/docs/source/agui/fig/fig5_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig_ev_1.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig_ev_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig_tree_1.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig_tree_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/fig/fig_tree_2.png` & `autosubmit-4.0.78/docs/source/agui/fig/fig_tree_2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_1.jpg` & `autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_2.jpg` & `autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_3.jpg` & `autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_3.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_4.jpg` & `autosubmit-4.0.78/docs/source/agui/graph/fig/fig_graph_4.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/graph/index.rst` & `autosubmit-4.0.78/docs/source/agui/graph/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/index.rst` & `autosubmit-4.0.78/docs/source/agui/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_1.jpg` & `autosubmit-4.0.78/docs/source/agui/log/fig/fig_log_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_2.jpg` & `autosubmit-4.0.78/docs/source/agui/log/fig/fig_log_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/log/index.rst` & `autosubmit-4.0.78/docs/source/agui/log/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/performance/fig/fig_performance_1.jpg` & `autosubmit-4.0.78/docs/source/agui/performance/fig/fig_performance_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/performance/index.rst` & `autosubmit-4.0.78/docs/source/agui/performance/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_1.jpg` & `autosubmit-4.0.78/docs/source/agui/statistics/fig/fig_stat_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_2.jpg` & `autosubmit-4.0.78/docs/source/agui/statistics/fig/fig_stat_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/statistics/index.rst` & `autosubmit-4.0.78/docs/source/agui/statistics/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/tree/fig/fig_tree_2.jpg` & `autosubmit-4.0.78/docs/source/agui/tree/fig/fig_tree_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/agui/tree/index.rst` & `autosubmit-4.0.78/docs/source/agui/tree/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/conf.py` & `autosubmit-4.0.78/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/devguide/index.rst` & `autosubmit-4.0.78/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/index.rst` & `autosubmit-4.0.78/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/installation/index.rst` & `autosubmit-4.0.78/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/introduction/fig1.png` & `autosubmit-4.0.78/docs/source/introduction/fig1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/introduction/fig2.png` & `autosubmit-4.0.78/docs/source/introduction/fig2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/introduction/fig3.png` & `autosubmit-4.0.78/docs/source/introduction/fig3.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/introduction/index.rst` & `autosubmit-4.0.78/docs/source/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/moduledoc/platforms.rst` & `autosubmit-4.0.78/docs/source/moduledoc/platforms.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/qstartguide/dummy.png` & `autosubmit-4.0.78/docs/source/qstartguide/dummy.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/qstartguide/index.rst` & `autosubmit-4.0.78/docs/source/qstartguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/changelog.rst` & `autosubmit-4.0.78/docs/source/troubleshooting/changelog.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/error-codes.rst` & `autosubmit-4.0.78/docs/source/troubleshooting/error-codes.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/fig/monarch-da.png` & `autosubmit-4.0.78/docs/source/troubleshooting/fig/monarch-da.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_0.png` & `autosubmit-4.0.78/docs/source/troubleshooting/fig/new_dependencies_0.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_1.png` & `autosubmit-4.0.78/docs/source/troubleshooting/fig/new_dependencies_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/troubleshooting/index.rst` & `autosubmit-4.0.78/docs/source/troubleshooting/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/unused_figs/group_chunk.png` & `autosubmit-4.0.78/docs/source/unused_figs/group_chunk.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/unused_figs/horizontal-vertical.png` & `autosubmit-4.0.78/docs/source/unused_figs/horizontal-vertical.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/unused_figs/wrapper.png` & `autosubmit-4.0.78/docs/source/unused_figs/wrapper.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/unused_figs/wrapper_expression.png` & `autosubmit-4.0.78/docs/source/unused_figs/wrapper_expression.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/unused_figs/wrapper_hybrid.png` & `autosubmit-4.0.78/docs/source/unused_figs/wrapper_hybrid.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/configure/develop_a_project.rst` & `autosubmit-4.0.78/docs/source/userguide/configure/develop_a_project.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/configure/index.rst` & `autosubmit-4.0.78/docs/source/userguide/configure/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/create/index.rst` & `autosubmit-4.0.78/docs/source/userguide/create/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/index.rst` & `autosubmit-4.0.78/docs/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/manage/index.rst` & `autosubmit-4.0.78/docs/source/userguide/manage/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/run/index.rst` & `autosubmit-4.0.78/docs/source/userguide/run/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/dasim.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/dasim.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/horizontal_remote.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/horizontal_remote.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/multiple_wrappers.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/multiple_wrappers.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/rerun.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/rerun.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-horizontal.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/vertical-horizontal.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-mixed.png` & `autosubmit-4.0.78/docs/source/userguide/wrappers/fig/vertical-mixed.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/docs/source/userguide/wrappers/index.rst` & `autosubmit-4.0.78/docs/source/userguide/wrappers/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/environment.yml` & `autosubmit-4.0.78/environment.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/log/fd_show.py` & `autosubmit-4.0.78/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/log/log.py` & `autosubmit-4.0.78/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/setup.py` & `autosubmit-4.0.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description='Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.',
     long_description=open('README_PIP.md').read(),
     author='Daniel Beltran Mora',
     author_email='daniel.beltran@bsc.es',
     url='http://www.bsc.es/projects/earthscience/autosubmit/',
     download_url='https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit',
     keywords=['climate', 'weather', 'workflow', 'HPC'],
-    install_requires=['autosubmitconfigparser==1.0.25','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','ruamel.yaml','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
+    install_requires=['ruamel.yaml>= 0.17','ruamel.yaml.clib >= 0.2','autosubmitconfigparser==1.0.26','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','ruamel.yaml','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux",
     ],
     packages=find_packages(),
```

### Comparing `autosubmit-4.0.77/test/integration/test_db_manager.py` & `autosubmit-4.0.78/test/integration/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/integration/test_job.py` & `autosubmit-4.0.78/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/README` & `autosubmit-4.0.78/test/regression/README`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/default_conf/platforms.conf` & `autosubmit-4.0.78/test/regression/default_conf/platforms.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.78/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mistral_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.78/test/regression/test_mn3_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.78/test/regression/test_mn4_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_moore_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_sedema_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.78/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/tests.conf` & `autosubmit-4.0.78/test/regression/tests.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/tests_commands.py` & `autosubmit-4.0.78/test/regression/tests_commands.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/tests_log.py` & `autosubmit-4.0.78/test/regression/tests_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/tests_runner.py` & `autosubmit-4.0.78/test/regression/tests_runner.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/regression/tests_utils.py` & `autosubmit-4.0.78/test/regression/tests_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/README_PIP.md` & `autosubmit-4.0.78/test/unit/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_basic_config.py` & `autosubmit-4.0.78/test/unit/test_basic_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_catlog.py` & `autosubmit-4.0.78/test/unit/test_catlog.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_chunk_date_lib.py` & `autosubmit-4.0.78/test/unit/test_chunk_date_lib.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_database_managers.py` & `autosubmit-4.0.78/test/unit/test_database_managers.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_db_manager.py` & `autosubmit-4.0.78/test/unit/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_dic_jobs.py` & `autosubmit-4.0.78/test/unit/test_dic_jobs.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_expid.py` & `autosubmit-4.0.78/test/unit/test_expid.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_history.py` & `autosubmit-4.0.78/test/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job.py` & `autosubmit-4.0.78/test/unit/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job_common.py` & `autosubmit-4.0.78/test/unit/test_job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job_graph.py` & `autosubmit-4.0.78/test/unit/test_job_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job_grouping.py` & `autosubmit-4.0.78/test/unit/test_job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job_list.py` & `autosubmit-4.0.78/test/unit/test_job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_job_package.py` & `autosubmit-4.0.78/test/unit/test_job_package.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_log.py` & `autosubmit-4.0.78/test/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_machinefiles_wrapper.py` & `autosubmit-4.0.78/test/unit/test_machinefiles_wrapper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_paramiko_platform.py` & `autosubmit-4.0.78/test/unit/test_paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_pjm.py` & `autosubmit-4.0.78/test/unit/test_pjm.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_platform_monitor.py` & `autosubmit-4.0.78/test/unit/test_platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_slurm_platform.py` & `autosubmit-4.0.78/test/unit/test_slurm_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_statistics.py` & `autosubmit-4.0.78/test/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_strategies.py` & `autosubmit-4.0.78/test/unit/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.77/test/unit/test_wrappers.py` & `autosubmit-4.0.78/test/unit/test_wrappers.py`

 * *Files identical despite different names*

