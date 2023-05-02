# Comparing `tmp/autosubmit-4.0.76.tar.gz` & `tmp/autosubmit-4.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit-4.0.76.tar", last modified: Mon Mar 27 07:23:56 2023, max compression
+gzip compressed data, was "autosubmit-4.0.77.tar", last modified: Tue May  2 08:29:58 2023, max compression
```

## Comparing `autosubmit-4.0.76.tar` & `autosubmit-4.0.77.tar`

### file list

```diff
@@ -1,402 +1,405 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.723681 autosubmit-4.0.76/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-02-21 14:36:36.000000 autosubmit-4.0.76/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-03-23 10:45:57.000000 autosubmit-4.0.76/.gitlab-ci.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      629 2023-03-16 14:55:14.000000 autosubmit-4.0.76/.readthedocs.yaml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.76/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-03-01 11:01:25.000000 autosubmit-4.0.76/CONTRIBUTING.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.76/LICENSE
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.76/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3099 2023-03-27 07:23:56.723681 autosubmit-4.0.76/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-02-10 15:39:53.000000 autosubmit-4.0.76/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-02-10 15:39:53.000000 autosubmit-4.0.76/README_PIP.md
--rw-rw-rw-   0 dbeltran  (1001) dbeltran  (1001)        7 2023-03-27 07:23:36.000000 autosubmit-4.0.76/VERSION
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/autosubmit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   318171 2023-03-27 07:17:11.000000 autosubmit-4.0.76/autosubmit/autosubmit.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/autosubmit/database/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/database/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/autosubmit/database/data/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/database/data/autosubmit.sql
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-03-01 11:01:25.000000 autosubmit-4.0.76/autosubmit/database/db_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/database/db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/database/db_structure.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/experiment/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/experiment/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-03-15 11:02:27.000000 autosubmit-4.0.76/autosubmit/experiment/experiment_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/experiment/statistics.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/git/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/git/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13736 2023-03-27 07:17:11.000000 autosubmit-4.0.76/autosubmit/git/autosubmit_git.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/helpers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.76/autosubmit/helpers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-03-15 11:02:27.000000 autosubmit-4.0.76/autosubmit/helpers/autosubmit_helper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/helpers/data_transfer.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/helpers/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/history/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/history/data_classes/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/data_classes/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/data_classes/experiment_run.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/data_classes/job_data.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.663681 autosubmit-4.0.76/autosubmit/history/database_managers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/database_managers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/database_managers/database_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/database_managers/database_models.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/database_managers/experiment_status_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/history/experiment_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/experiment_status.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/internal_logging.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.667681 autosubmit-4.0.76/autosubmit/history/platform_monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.667681 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-23 13:44:20.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/pending.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-03-23 13:44:20.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/platform_utils.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/slurm_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/platform_monitor/slurm_monitor_item.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/history/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.671681 autosubmit-4.0.76/autosubmit/job/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/job/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    91641 2023-03-27 07:17:11.000000 autosubmit-4.0.76/autosubmit/job/job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-03-01 11:01:25.000000 autosubmit-4.0.76/autosubmit/job/job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20160 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_dict.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      995 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_exceptions.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   120591 2023-03-15 11:02:27.000000 autosubmit-4.0.76/autosubmit/job/job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_list_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_package_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    60203 2023-03-01 11:01:25.000000 autosubmit-4.0.76/autosubmit/job/job_packager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    34059 2023-03-01 11:01:25.000000 autosubmit-4.0.76/autosubmit/job/job_packages.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/job/job_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.671681 autosubmit-4.0.76/autosubmit/monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/monitor/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/monitor/diagram.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-03-01 11:01:25.000000 autosubmit-4.0.76/autosubmit/monitor/monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/monitor/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.671681 autosubmit-4.0.76/autosubmit/notifications/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/notifications/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/notifications/mail_notifier.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/notifications/notifier.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.671681 autosubmit-4.0.76/autosubmit/platforms/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/platforms/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13384 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/ecplatform.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.675681 autosubmit-4.0.76/autosubmit/platforms/headers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/platforms/headers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/ec_cca_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/ec_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/local_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/lsf_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/pbs10_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/pbs11_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/pbs12_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/headers/pjm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/ps_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/sge_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6726 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/headers/slurm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/locplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5646 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/lsfplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53188 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10591 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/paramiko_submitter.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/pbsplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    21179 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/pjmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23630 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/psplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/sgeplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32719 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/slurmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/submitter.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.675681 autosubmit-4.0.76/autosubmit/platforms/wrappers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/autosubmit/platforms/wrappers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/platforms/wrappers/wrapper_builder.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7349 2023-03-23 10:45:57.000000 autosubmit-4.0.76/autosubmit/platforms/wrappers/wrapper_factory.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.675681 autosubmit-4.0.76/autosubmit/statistics/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.76/autosubmit/statistics/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/statistics/jobs_stat.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/statistics/statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-02-02 09:02:16.000000 autosubmit-4.0.76/autosubmit/statistics/stats_summary.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-02-10 15:39:53.000000 autosubmit-4.0.76/autosubmit/statistics/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/autosubmit.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3099 2023-03-27 07:23:56.000000 autosubmit-4.0.76/autosubmit.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12880 2023-03-27 07:23:56.000000 autosubmit-4.0.76/autosubmit.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-03-27 07:23:56.000000 autosubmit-4.0.76/autosubmit.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      419 2023-03-27 07:23:56.000000 autosubmit-4.0.76/autosubmit.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-03-27 07:23:56.000000 autosubmit-4.0.76/autosubmit.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.675681 autosubmit-4.0.76/bin/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-02-10 15:39:53.000000 autosubmit-4.0.76/bin/autosubmit
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.675681 autosubmit-4.0.76/docs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/Makefile
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.76/docs/autosubmit.pdf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.679681 autosubmit-4.0.76/docs/source/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.679681 autosubmit-4.0.76/docs/source/agui/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.679681 autosubmit-4.0.76/docs/source/agui/experiment/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.679681 autosubmit-4.0.76/docs/source/agui/experiment/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/experiment/fig/fig_experiment.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/agui/experiment/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig1_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig2_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig3_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig4_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig5_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig_ev_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig_tree_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/fig/fig_tree_2.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/graph/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/graph/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_3.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_4.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/agui/graph/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/agui/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/log/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/log/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/log/fig/fig_log_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/log/fig/fig_log_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/log/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.687681 autosubmit-4.0.76/docs/source/agui/performance/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/agui/performance/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/performance/fig/fig_performance_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/performance/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/agui/statistics/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/agui/statistics/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/statistics/fig/fig_stat_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/statistics/fig/fig_stat_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/statistics/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/agui/tree/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/agui/tree/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/agui/tree/fig/fig_tree_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/agui/tree/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10119 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/conf.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/devguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-02-10 15:39:53.000000 autosubmit-4.0.76/docs/source/devguide/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.691681 autosubmit-4.0.76/docs/source/installation/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/installation/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.695681 autosubmit-4.0.76/docs/source/introduction/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/introduction/fig1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/introduction/fig2.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/introduction/fig3.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-02-10 15:39:53.000000 autosubmit-4.0.76/docs/source/introduction/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.695681 autosubmit-4.0.76/docs/source/moduledoc/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/autosubmit.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/moduledoc/config.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/database.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/git.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/job.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/monitor.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/moduledoc/platforms.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.695681 autosubmit-4.0.76/docs/source/qstartguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/qstartguide/dummy.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-03-27 07:17:11.000000 autosubmit-4.0.76/docs/source/qstartguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.695681 autosubmit-4.0.76/docs/source/troubleshooting/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/troubleshooting/changelog.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/troubleshooting/error-codes.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/troubleshooting/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-02-10 15:39:53.000000 autosubmit-4.0.76/docs/source/troubleshooting/fig/monarch-da.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-02-10 15:39:53.000000 autosubmit-4.0.76/docs/source/troubleshooting/fig/new_dependencies_0.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-02-10 15:39:53.000000 autosubmit-4.0.76/docs/source/troubleshooting/fig/new_dependencies_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/troubleshooting/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/unused_figs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/unused_figs/group_chunk.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/unused_figs/horizontal-vertical.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/unused_figs/wrapper.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/unused_figs/wrapper_expression.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/unused_figs/wrapper_hybrid.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/configure/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30918 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/userguide/configure/develop_a_project.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/userguide/configure/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/create/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-03-15 11:02:27.000000 autosubmit-4.0.76/docs/source/userguide/create/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/userguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/manage/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/userguide/manage/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/run/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-03-15 11:02:27.000000 autosubmit-4.0.76/docs/source/userguide/run/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.699681 autosubmit-4.0.76/docs/source/userguide/wrappers/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.703681 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/dasim.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/horizontal_remote.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/multiple_wrappers.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/rerun.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/vertical-horizontal.png
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-02-02 09:02:16.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/fig/vertical-mixed.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-03-01 11:01:25.000000 autosubmit-4.0.76/docs/source/userguide/wrappers/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      710 2023-03-27 07:17:11.000000 autosubmit-4.0.76/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.703681 autosubmit-4.0.76/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.76/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-02-10 15:39:53.000000 autosubmit-4.0.76/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2023-02-10 15:39:53.000000 autosubmit-4.0.76/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      448 2023-03-27 07:17:11.000000 autosubmit-4.0.76/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-03-27 07:23:56.723681 autosubmit-4.0.76/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3051 2023-03-27 07:17:11.000000 autosubmit-4.0.76/setup.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.703681 autosubmit-4.0.76/test/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.703681 autosubmit-4.0.76/test/integration/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/integration/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/integration/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/integration/test_job.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/README
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/db/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/db/.gitignore
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/default_conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/default_conf/platforms.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.707681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.655681 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.711681 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.715681 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.719681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.719681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.659681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.719681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.719681 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.76/test/regression/tests.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/regression/tests_commands.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/tests_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/tests_runner.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/regression/tests_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-03-27 07:23:56.723681 autosubmit-4.0.76/test/unit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.76/test/unit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_basic_config.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-03-27 07:17:11.000000 autosubmit-4.0.76/test/unit/test_catlog.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.76/test/unit/test_chunk_date_lib.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-03-23 13:44:20.000000 autosubmit-4.0.76/test/unit/test_database_managers.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22517 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/unit/test_dic_jobs.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2729 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_expid.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-03-23 13:44:20.000000 autosubmit-4.0.76/test/unit/test_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12463 2023-03-27 07:17:11.000000 autosubmit-4.0.76/test/unit/test_job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/unit/test_job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47671 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_job_graph.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59180 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12489 2023-03-01 11:01:25.000000 autosubmit-4.0.76/test/unit/test_job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2374 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_job_package.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_machinefiles_wrapper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4963 2023-03-23 10:45:57.000000 autosubmit-4.0.76/test/unit/test_pjm.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-03-23 13:44:20.000000 autosubmit-4.0.76/test/unit/test_platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-03-15 11:02:27.000000 autosubmit-4.0.76/test/unit/test_setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-03-23 13:44:20.000000 autosubmit-4.0.76/test/unit/test_statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-03-23 13:44:20.000000 autosubmit-4.0.76/test/unit/test_strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    80575 2023-02-10 15:39:53.000000 autosubmit-4.0.76/test/unit/test_wrappers.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.gitlab-ci.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      629 2023-04-27 12:24:09.000000 autosubmit-4.0.77/.readthedocs.yaml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-04-27 12:24:09.000000 autosubmit-4.0.77/CONTRIBUTING.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.77/LICENSE
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.77/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 08:29:58.192849 autosubmit-4.0.77/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-04-27 12:24:09.000000 autosubmit-4.0.77/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-04-27 12:24:09.000000 autosubmit-4.0.77/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-05-02 08:29:32.000000 autosubmit-4.0.77/VERSION
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   318778 2023-05-02 07:56:09.000000 autosubmit-4.0.77/autosubmit/autosubmit.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/database/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/database/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/database/data/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/database/data/autosubmit.sql
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/database/db_structure.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/experiment/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/experiment/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/experiment/experiment_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/experiment/statistics.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/git/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/git/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-04-27 12:55:41.000000 autosubmit-4.0.77/autosubmit/git/autosubmit_git.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/helpers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/helpers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/autosubmit_helper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/data_transfer.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/helpers/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit/history/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/data_classes/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/data_classes/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/data_classes/experiment_run.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/data_classes/job_data.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/database_managers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/database_managers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/database_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/database_models.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/database_managers/experiment_status_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/experiment_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/experiment_status.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/internal_logging.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/platform_monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/pending.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_utils.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor_item.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/history/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/job/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/job/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93132 2023-04-28 13:09:09.000000 autosubmit-4.0.77/autosubmit/job/job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20050 2023-04-28 13:02:46.000000 autosubmit-4.0.77/autosubmit/job/job_dict.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      995 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_exceptions.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   120598 2023-05-02 07:38:24.000000 autosubmit-4.0.77/autosubmit/job/job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_list_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_package_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62106 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_packager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    36449 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_packages.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/job/job_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/monitor/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/diagram.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/monitor/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.160849 autosubmit-4.0.77/autosubmit/notifications/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/notifications/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/notifications/mail_notifier.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/notifications/notifier.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/ecplatform.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/headers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/headers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ec_cca_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ec_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/local_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/lsf_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs10_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs11_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pbs12_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/pjm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/ps_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/sge_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7122 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/headers/slurm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/locplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/lsfplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53639 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11360 2023-04-28 13:58:41.000000 autosubmit-4.0.77/autosubmit/platforms/paramiko_submitter.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/pbsplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    21092 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/pjmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    24934 2023-04-28 14:04:34.000000 autosubmit-4.0.77/autosubmit/platforms/platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/psplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/sgeplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32232 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/slurmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/submitter.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/platforms/wrappers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38627 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_builder.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7581 2023-04-28 10:58:24.000000 autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_factory.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/autosubmit/statistics/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/statistics/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/jobs_stat.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-02-02 09:02:16.000000 autosubmit-4.0.77/autosubmit/statistics/stats_summary.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-04-27 12:24:09.000000 autosubmit-4.0.77/autosubmit/statistics/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.156849 autosubmit-4.0.77/autosubmit.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12971 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      419 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-05-02 08:29:57.000000 autosubmit-4.0.77/autosubmit.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/bin/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-04-27 12:24:09.000000 autosubmit-4.0.77/bin/autosubmit
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/Makefile
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.77/docs/autosubmit.pdf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/experiment/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.164849 autosubmit-4.0.77/docs/source/agui/experiment/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/experiment/fig/fig_experiment.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/experiment/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig1_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig2_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig3_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig4_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig5_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_ev_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_tree_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/fig/fig_tree_2.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/graph/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/graph/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_3.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_4.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/graph/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/log/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/log/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/log/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/performance/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/performance/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/performance/fig/fig_performance_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/performance/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.168849 autosubmit-4.0.77/docs/source/agui/statistics/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/statistics/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/statistics/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/tree/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/agui/tree/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/agui/tree/fig/fig_tree_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/agui/tree/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10119 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/conf.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/devguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/devguide/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2124 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/installation/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/installation/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/introduction/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig2.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/introduction/fig3.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/introduction/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/moduledoc/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/autosubmit.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/moduledoc/config.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/database.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/git.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/job.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/monitor.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/moduledoc/platforms.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/qstartguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/qstartguide/dummy.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/qstartguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/troubleshooting/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/changelog.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/error-codes.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.172849 autosubmit-4.0.77/docs/source/troubleshooting/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/monarch-da.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_0.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/troubleshooting/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/unused_figs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/group_chunk.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/horizontal-vertical.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper_expression.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/unused_figs/wrapper_hybrid.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/configure/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-04-28 08:40:38.000000 autosubmit-4.0.77/docs/source/userguide/configure/develop_a_project.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20565 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/configure/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/create/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/create/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/manage/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/manage/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/run/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/run/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.176849 autosubmit-4.0.77/docs/source/userguide/wrappers/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/dasim.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/horizontal_remote.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/multiple_wrappers.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/rerun.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-horizontal.png
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-02-02 09:02:16.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-mixed.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-04-27 12:24:09.000000 autosubmit-4.0.77/docs/source/userguide/wrappers/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      710 2023-04-28 14:08:26.000000 autosubmit-4.0.77/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.77/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-04-27 12:24:09.000000 autosubmit-4.0.77/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-04-27 12:24:09.000000 autosubmit-4.0.77/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      448 2023-04-28 14:08:26.000000 autosubmit-4.0.77/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-05-02 08:29:58.192849 autosubmit-4.0.77/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3051 2023-04-27 12:24:09.000000 autosubmit-4.0.77/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/integration/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/integration/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/integration/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/integration/test_job.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/README
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/db/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/db/.gitignore
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/default_conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/default_conf/platforms.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.180849 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.184849 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.188849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.152849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.77/test/regression/tests.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/regression/tests_commands.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_runner.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/regression/tests_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-05-02 08:29:58.192849 autosubmit-4.0.77/test/unit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.77/test/unit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_basic_config.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_catlog.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.77/test/unit/test_chunk_date_lib.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_database_managers.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22797 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_dic_jobs.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2729 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_expid.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12868 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47670 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_graph.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59460 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2374 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_job_package.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3772 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_machinefiles_wrapper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_pjm.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2177 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_slurm_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81586 2023-04-27 12:24:09.000000 autosubmit-4.0.77/test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.76/.gitlab-ci.yml` & `autosubmit-4.0.77/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/.readthedocs.yaml` & `autosubmit-4.0.77/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/CONTRIBUTING.md` & `autosubmit-4.0.77/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/LICENSE` & `autosubmit-4.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/PKG-INFO` & `autosubmit-4.0.77/test/unit/README_PIP.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: autosubmit
-Version: 4.0.76
-Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
-Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
-Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
-Author: Daniel Beltran Mora
-Author-email: daniel.beltran@bsc.es
-License: GNU GPL v3
-Keywords: climate,weather,workflow,HPC
-Platform: GNU/Linux Debian
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: POSIX :: Linux
-License-File: LICENSE
-
 
 Autosubmit is a lightweight workflow manager designed to meet climate research necessities. Unlike other workflow solutions in the domain, it integrates the capabilities of an experiment manager, workflow orchestrator and monitor in a self-contained application. The experiment manager allows for defining and configuring experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts. These multi-scale workflows can involve from a few to thousands of steps and from one to multiple platforms.
 
 Autosubmit facilitates easy and fast integration and relocation on new platforms. On the one hand, users can rapidly execute general scripts and progressively parametrize them by reading Autosubmit variables. On the other hand, it is a self-contained desktop application capable of submitting jobs to remote platforms without any external deployment.
 
 Due to its robustness, it can handle different eventualities, such as networking or I/O errors. Finally, the monitoring capabilities extend beyond the desktop application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI. 
 
 Autosubmit is a Python package provided in PyPI. Conda recipes can also be found on the website. A containerized version for testing purposes is also available but not public yet.
 
 It has contributed to various European research projects and runs different operational systems. During the following years, it will support some of the Earth Digital Twins as the Digital Twin Ocean.
 
-Concretely, it is currently used at Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES...), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and many other. Autosubmit has run these workflows in different supercomputers in BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+Concretely, it is currently used at Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES...), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and many other. Autosubmit has run these workflows in different supercomputers in BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
```

### Comparing `autosubmit-4.0.76/README.md` & `autosubmit-4.0.77/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/README_PIP.md` & `autosubmit-4.0.77/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: autosubmit
+Version: 4.0.77
+Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
+Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
+Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
+Author: Daniel Beltran Mora
+Author-email: daniel.beltran@bsc.es
+License: GNU GPL v3
+Keywords: climate,weather,workflow,HPC
+Platform: GNU/Linux Debian
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE
+
+Autosubmit is a lightweight workflow manager and meta-scheduler. It was originally designed in 2011 for use in climate research for configuring and running experiments. In the last few years, it has been extended to cover additional use cases, and today it is used as a general orchestration tool. It supports scheduling jobs to remote batch servers (via SSH) such as PBS, LSF, SLURM, and SGE.
+
+Autosubmit is a Python package provided in PyPI, which facilitates easy and fast integration and relocation on new platforms. Conda recipes are available on the project website. A containerized version for testing purposes is also available but not public yet.
+
+The features found in Autosubmit characterize it as both an experiment manager and also as a workflow orchestrator. The experiment manager allows users to define and configure experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts.
 
-Autosubmit is a lightweight workflow manager designed to meet climate research necessities. Unlike other workflow solutions in the domain, it integrates the capabilities of an experiment manager, workflow orchestrator and monitor in a self-contained application. The experiment manager allows for defining and configuring experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts. These multi-scale workflows can involve from a few to thousands of steps and from one to multiple platforms.
+These multi-scale workflows can contain from a few steps to thousands of steps, and from a single platform to multiple platforms. Platform is a concept in Autosubmit to abstract servers. A workflow configuration can include one or multiple platforms, allowing the workflow to run on any number of servers via password-less SSH without any external deployment.
 
-Autosubmit facilitates easy and fast integration and relocation on new platforms. On the one hand, users can rapidly execute general scripts and progressively parametrize them by reading Autosubmit variables. On the other hand, it is a self-contained desktop application capable of submitting jobs to remote platforms without any external deployment.
+Due to its robustness it can handle different eventualities such as networking connectivity issues or I/O errors. The monitoring capabilities extend beyond the command-line application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI.
 
-Due to its robustness, it can handle different eventualities, such as networking or I/O errors. Finally, the monitoring capabilities extend beyond the desktop application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI. 
+It has contributed to various European research projects and runs different operational systems. It will support the Earth Digital Twins as the Digital Twin Ocean over the next years.
 
-Autosubmit is a Python package provided in PyPI. Conda recipes can also be found on the website. A containerized version for testing purposes is also available but not public yet.
-
-It has contributed to various European research projects and runs different operational systems. During the following years, it will support some of the Earth Digital Twins as the Digital Twin Ocean.
-
-Concretely, it is currently used at Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES...), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and many other. Autosubmit has run these workflows in different supercomputers in BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+It is currently used at the Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES, and others), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and for many other use cases. Autosubmit has been used to run workflows in different supercomputers at BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
```

### Comparing `autosubmit-4.0.76/autosubmit/autosubmit.py` & `autosubmit-4.0.77/autosubmit/autosubmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1174,14 +1174,15 @@
             os.chmod(os.path.join(exp_folder, "conf"), 0o755)
             os.chmod(os.path.join(exp_folder, "pkl"), 0o755)
             os.chmod(os.path.join(exp_folder, "tmp"), 0o755)
             os.chmod(os.path.join(exp_folder, "tmp", "ASLOGS"), 0o755)
             os.chmod(os.path.join(exp_folder, "tmp", "LOG_"+exp_id), 0o755)
             os.chmod(os.path.join(exp_folder, "plot"), 0o755)
             os.chmod(os.path.join(exp_folder, "status"), 0o755)
+            Log.info(f"Experiment folder: {exp_folder}")
         except OSError as e:
             try:
                 Autosubmit._delete_expid(exp_id, True)
             except:
                 pass
             raise AutosubmitCritical("Error while creating the experiment structure: {0}".format(str(e)), 7011)
 
@@ -1850,15 +1851,15 @@
             Log.debug("Processing job packages")
             try:
                 for (exp_id, package_name, job_name) in packages:
                     if package_name not in job_list.packages_dict:
                         job_list.packages_dict[package_name] = []
                     job_list.packages_dict[package_name].append(job_list.get_job_by_name(job_name))
                 # This function, checks the stored STATUS of jobs inside wrappers. Since "wrapper status" is a memory variable.
-                job_list = Autosubmit.check_wrapper_stored_status(job_list, as_conf)
+                job_list = Autosubmit.check_wrapper_stored_status(as_conf, job_list)
             except Exception as e:
                 raise AutosubmitCritical(
                     "Autosubmit failed while processing job packages. This might be due to a change in your experiment configuration files after 'autosubmit create' was performed.",
                     7014, str(e))
         if recover:
             Log.info("Recovering wrappers... Done")
 
@@ -2114,15 +2115,15 @@
                                 7051, e.message)
                     except AutosubmitCritical as e:  # Critical errors can't be recovered. Failed configuration or autosubmit error
                         raise AutosubmitCritical(e.message, e.code, e.trace)
                     except (portalocker.AlreadyLocked, portalocker.LockException) as e:
                         message = "We have detected that there is another Autosubmit instance using the experiment\n. Stop other Autosubmit instances that are using the experiment or delete autosubmit.lock file located on tmp folder"
                         raise AutosubmitCritical(message, 7000)
                     except BaseException as e:  # If this happens, there is a bug in the code or an exception not-well caught
-                        raise AutosubmitCritical("There is a bug in the code, please contact via git", 7070, str(e))
+                        raise AutosubmitCritical("There is a bug in the code, please contact via Gitlab", 7070, str(e))
 
 
                 Log.result("No more jobs to run.")
                 # Updating job data header with current information when experiment ends
                 try:
                     exp_history = ExperimentHistory(expid, jobdata_dir_path=BasicConfig.JOBDATA_DIR,
                                                     historiclog_dir_path=BasicConfig.HISTORICAL_LOG_DIR)
@@ -3400,23 +3401,23 @@
             try:
                 experiment_id = experiment_id.strip(" ")
                 exp_path = os.path.join(BasicConfig.LOCAL_ROOT_DIR, experiment_id)
 
                 as_conf = AutosubmitConfig(
                     experiment_id, BasicConfig, YAMLParserFactory())
                 as_conf.check_conf_files(False,no_log=True)
-                user = os.stat(as_conf.experiment_file).st_uid
+                user = os.stat(as_conf.conf_folder_yaml).st_uid
                 try:
                     user = pwd.getpwuid(user).pw_name
                 except Exception as e:
                     Log.warning(
                         "The user does not exist anymore in the system, using id instead")
 
                 created = datetime.datetime.fromtimestamp(
-                    os.path.getmtime(as_conf.experiment_file))
+                    os.path.getmtime(as_conf.conf_folder_yaml))
 
                 project_type = as_conf.get_project_type()
                 if as_conf.get_svn_project_url():
                     model = as_conf.get_svn_project_url()
                     branch = as_conf.get_svn_project_url()
                 else:
                     model = as_conf.get_git_project_origin()
@@ -3848,15 +3849,15 @@
         :param expid: experiment identifier
         :type expid: str
         """
         try:
             Autosubmit._check_ownership(expid, raise_error=True)
             as_conf = AutosubmitConfig(expid, BasicConfig, YAMLParserFactory())
             # as_conf.reload(force_load=True)
-            as_conf.check_conf_files(refresh=True)
+            as_conf.check_conf_files(False)
         except (AutosubmitError, AutosubmitCritical):
             raise
         except BaseException as e:
             raise AutosubmitCritical("Error while reading the configuration files", 7064, str(e))
         try:
             if "Expdef" in as_conf.wrong_config:
                 as_conf.show_messages()
@@ -4400,23 +4401,27 @@
             with portalocker.Lock(os.path.join(tmp_path, 'autosubmit.lock'), timeout=1) as fh:
                 try:
                     Log.info(
                         "Preparing .lock file to avoid multiple instances with same expid.")
 
                     as_conf = AutosubmitConfig(expid, BasicConfig, YAMLParserFactory())
                     # Get original configuration
-                    as_conf.check_conf_files(False, only_experiment_data=True, no_log=True)
+                    as_conf.check_conf_files(running_time=False, only_experiment_data=True, no_log=True)
                     # Getting output type provided by the user in config, 'pdf' as default
                     try:
                         if not Autosubmit._copy_code(as_conf, expid, as_conf.experiment_data.get("PROJECT",{}).get("PROJECT_TYPE","none"), False):
                             return False
-                    except:
-                        raise AutosubmitCritical("Error obtaining the project data, check the parameters related to PROJECT and GIT/SVN or LOCAL sections", code=7014)
+                    except AutosubmitCritical as e:
+                        raise
+                    except BaseException as e:
+                        raise AutosubmitCritical("Error obtaining the project data, check the parameters related to PROJECT and GIT/SVN or LOCAL sections", code=7014,trace=str(e))
                     # Update configuration with the new config in the dist ( if any )
-                    as_conf.check_conf_files(True,force_load=True, only_experiment_data=False, no_log=False)
+                    as_conf.check_conf_files(running_time=False,force_load=True, only_experiment_data=False, no_log=False)
+                    if len(as_conf.experiment_data.get("JOBS",{})) == 0 and "CUSTOM_CONFIG" in as_conf.experiment_data.get("DEFAULT",{}):
+                        raise AutosubmitCritical(f'Job list is empty\nCheck if there are YML files in {as_conf.experiment_data.get("DEFAULT","").get("CUSTOM_CONFIG","")}', code=7015)
                     output_type = as_conf.get_output_type()
 
                     if not os.path.exists(os.path.join(exp_path, "pkl")):
                         raise AutosubmitCritical(
                             "The pkl folder doesn't exists. Make sure that the 'pkl' folder exists in the following path: {}".format(
                                 exp_path), code=6013)
                     if not os.path.exists(os.path.join(exp_path, "plot")):
@@ -4584,18 +4589,20 @@
                     raise AutosubmitCritical("Stopped by user input", 7010)
                 except BaseException as e:
                     raise
         except (portalocker.AlreadyLocked, portalocker.LockException) as e:
             message = "We have detected that there is another Autosubmit instance using the experiment\n. Stop other Autosubmit instances that are using the experiment or delete autosubmit.lock file located on tmp folder"
             raise AutosubmitCritical(message, 7000)
         except AutosubmitError as e:
+            # TODO: == "" or is None?
             if e.trace == "":
                 e.trace = traceback.format_exc()
             raise AutosubmitError(e.message, e.code, e.trace)
         except AutosubmitCritical as e:
+            # TODO: == "" or is None?
             if e.trace == "":
                 e.trace = traceback.format_exc()
             raise AutosubmitCritical(e.message, e.code, e.trace)
         except BaseException as e:
             raise AutosubmitCritical(str(e), 7070)
 
     @staticmethod
@@ -5624,14 +5631,15 @@
         Autosubmit.create(testid, False, True)
         if not Autosubmit.run_experiment(testid):
             return False
         return True
 
     @staticmethod
     def _change_conf(testid, hpc, start_date, member, chunks, branch, random_select=False):
+        #TODO
         as_conf = AutosubmitConfig(testid, BasicConfig, YAMLParserFactory())
 
         if as_conf.experiment_data.get("RERUN", False):
             if str(as_conf.experiment_data["RERUN"].get("RERUN", "False")).lower() != "true":
                 raise AutosubmitCritical('Can not test a RERUN experiment', 7014)
 
         content = open(as_conf.experiment_file).read()
```

### Comparing `autosubmit-4.0.76/autosubmit/database/db_common.py` & `autosubmit-4.0.77/autosubmit/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/database/db_manager.py` & `autosubmit-4.0.77/autosubmit/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/database/db_structure.py` & `autosubmit-4.0.77/autosubmit/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/experiment/experiment_common.py` & `autosubmit-4.0.77/autosubmit/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/experiment/statistics.py` & `autosubmit-4.0.77/autosubmit/experiment/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/git/autosubmit_git.py` & `autosubmit-4.0.77/autosubmit/git/autosubmit_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,16 +278,15 @@
                 command_1 = "cd {0}; {1} ".format(project_path, command_1)
                 hpcarch.send_command(command_1)
         except subprocess.CalledProcessError as e:
             shutil.rmtree(project_path)
             if os.path.exists(project_backup_path):
                 Log.info("Restoring proj folder...")
                 shutil.move(project_backup_path, project_path)
-            raise AutosubmitCritical("Can not clone {0} into {1}".format(
-                git_project_branch + " " + git_project_origin, project_path), 7065)
+            raise AutosubmitCritical(f'Can not clone {git_project_branch+" "+git_project_origin} into {project_path}', 7065)
         if submodule_failure:
             Log.info("Some Submodule failures have been detected. Backup {0} will not be removed.".format(project_backup_path))
             return False
 
         if os.path.exists(project_backup_path):
             Log.info("Removing backup...")
             shutil.rmtree(project_backup_path)
```

### Comparing `autosubmit-4.0.76/autosubmit/helpers/autosubmit_helper.py` & `autosubmit-4.0.77/autosubmit/helpers/autosubmit_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/helpers/utils.py` & `autosubmit-4.0.77/autosubmit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/data_classes/experiment_run.py` & `autosubmit-4.0.77/autosubmit/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/data_classes/job_data.py` & `autosubmit-4.0.77/autosubmit/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/database_managers/database_manager.py` & `autosubmit-4.0.77/autosubmit/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/database_managers/database_models.py` & `autosubmit-4.0.77/autosubmit/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/database_managers/experiment_history_db_manager.py` & `autosubmit-4.0.77/autosubmit/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/database_managers/experiment_status_db_manager.py` & `autosubmit-4.0.77/autosubmit/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/experiment_history.py` & `autosubmit-4.0.77/autosubmit/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/experiment_status.py` & `autosubmit-4.0.77/autosubmit/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/internal_logging.py` & `autosubmit-4.0.77/autosubmit/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper1.txt` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper1.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper2.txt` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper2.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/platform_monitor.py` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/platform_utils.py` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/slurm_monitor.py` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/platform_monitor/slurm_monitor_item.py` & `autosubmit-4.0.77/autosubmit/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/strategies.py` & `autosubmit-4.0.77/autosubmit/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/history/utils.py` & `autosubmit-4.0.77/autosubmit/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job.py` & `autosubmit-4.0.77/autosubmit/job/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         self.script_name_wrapper = None
         self.delay_end = datetime.datetime.now()
         self.delay_retrials = "0"
         self.wrapper_type = None
         self._wrapper_queue = None
         self._platform = None
         self._queue = None
+        self._partition = None
+
         self.retry_delay = "0"
         self.platform_name = None # type: str
         self.section = None # type: str
         self.wallclock = None # type: str
         self.wchunkinc = None
         self.tasks = '1'
         self.nodes = ""
@@ -152,17 +154,17 @@
         self.distance_weight = 0
         self.level = 0
         self.export = "none"
         self.dependencies = []
         self.running = "once"
         self.start_time = None
         self.edge_info = dict()
-        self.partition = ""
-
-
+        self.total_jobs = None
+        self.max_waiting_jobs = None
+        self.exclusive = ""
     def __getstate__(self):
         odict = self.__dict__
         if '_platform' in odict:
             odict = odict.copy()  # copy the dict since we change it
             del odict['_platform']  # remove filehandle entry
         return odict
 
@@ -212,15 +214,15 @@
         """
         Comma separated list of children's names
         """
         return ",".join([str(child.name) for child in self._children])
 
     @property
     def is_serial(self):
-        return str(self.processors) == '1'
+        return str(self.processors) == '1' or str(self.processors) == ''
 
     @property
     def platform(self):
         """
         Returns the platform to be used by the job. Chooses between serial and parallel platforms
 
         :return HPCPlatform object for the job to use
@@ -261,15 +263,38 @@
         """
         Sets the queue to be used by the job.
 
         :param value: queue to set
         :type value: HPCPlatform
         """
         self._queue = value
+    @property
+    def partition(self):
+        """
+        Returns the queue to be used by the job. Chooses between serial and parallel platforms
 
+        :return HPCPlatform object for the job to use
+        :rtype: HPCPlatform
+        """
+        if self._partition is not None and len(str(self._partition)) > 0:
+            return self._partition
+        if self.is_serial:
+            return self._platform.serial_platform.serial_partition
+        else:
+            return self._platform.partition
+
+    @partition.setter
+    def partition(self, value):
+        """
+        Sets the partion to be used by the job.
+
+        :param value: partion to set
+        :type value: HPCPlatform
+        """
+        self._partition = value
     @property
     def children(self):
         """
         Returns a list containing all children of the job
 
         :return: child jobs
         :rtype: set
@@ -991,24 +1016,31 @@
         parameters['CURRENT_SCRATCH_DIR'] = job_platform.scratch
         parameters['CURRENT_PROJ_DIR'] = job_platform.project_dir
         parameters['CURRENT_ROOTDIR'] = job_platform.root_dir
         parameters['CURRENT_LOGDIR'] = job_platform.get_files_path()
 
         return parameters
     def update_platform_associated_parameters(self,as_conf, parameters, job_platform, chunk):
-        self.queue = self.queue
+        self.executable = str(as_conf.jobs_data[self.section].get("EXECUTABLE", as_conf.platforms_data.get(job_platform.name,{}).get("EXECUTABLE","")))
+        self.total_jobs = int(as_conf.jobs_data[self.section].get("TOTALJOBS", job_platform.total_jobs))
+        self.max_waiting_jobs = int(as_conf.jobs_data[self.section].get("MAXWAITINGJOBS", job_platform.max_waiting_jobs))
+
         self.processors = str(as_conf.jobs_data[self.section].get("PROCESSORS",as_conf.platforms_data.get(job_platform.name,{}).get("PROCESSORS","1")))
+        self.exclusive = str(as_conf.jobs_data[self.section].get("EXCLUSIVE",as_conf.platforms_data.get(job_platform.name,{}).get("EXCLUSIVE",False)))
         self.threads = str(as_conf.jobs_data[self.section].get("THREADS",as_conf.platforms_data.get(job_platform.name,{}).get("THREADS","1")))
         self.tasks = str(as_conf.jobs_data[self.section].get("TASKS",as_conf.platforms_data.get(job_platform.name,{}).get("TASKS","1")))
         self.nodes = str(as_conf.jobs_data[self.section].get("NODES",as_conf.platforms_data.get(job_platform.name,{}).get("NODES","")))
         self.hyperthreading = str(as_conf.jobs_data[self.section].get("HYPERTHREADING",as_conf.platforms_data.get(job_platform.name,{}).get("HYPERTHREADING","none")))
         if int(self.tasks) <= 1 and int(job_platform.processors_per_node) > 1 and int(self.processors) > int(job_platform.processors_per_node):
             self.tasks = job_platform.processors_per_node
         self.memory = str(as_conf.jobs_data[self.section].get("MEMORY",as_conf.platforms_data.get(job_platform.name,{}).get("MEMORY","")))
         self.memory_per_task = str(as_conf.jobs_data[self.section].get("MEMORY_PER_TASK",as_conf.platforms_data.get(job_platform.name,{}).get("MEMORY_PER_TASK","")))
+        # These are to activate serial platform if neccesary
+        self.queue = self.queue
+        self.partition = self.partition
         self.wallclock = as_conf.jobs_data[self.section].get("WALLCLOCK",as_conf.platforms_data.get(self.platform_name,{}).get("MAX_WALLCLOCK",None))
         if self.wallclock is None and job_platform.type not in ['ps',"local","PS","LOCAL"]:
             self.wallclock = "01:59"
         elif self.wallclock is None and job_platform.type in ['ps','local',"PS","LOCAL"]:
             self.wallclock = "00:00"
         # Increasing according to chunk
         self.wallclock = increase_wallclock_by_chunk(
```

### Comparing `autosubmit-4.0.76/autosubmit/job/job_common.py` & `autosubmit-4.0.77/autosubmit/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job_dict.py` & `autosubmit-4.0.77/autosubmit/job/job_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,31 +374,30 @@
             job.type = Type.BASH
         elif job_type == 'python' or job_type == 'python3':
             job.type = Type.PYTHON3
         elif job_type == 'python2':
             job.type = Type.PYTHON2
         elif job_type == 'r':
             job.type = Type.R
-        job.executable = str(parameters[section].get( "EXECUTABLE", ""))
         hpcarch = self.experiment_data.get("DEFAULT",{})
         hpcarch = hpcarch.get("HPCARCH","")
         job.platform_name = str(parameters[section].get("PLATFORM", hpcarch)).upper()
         if self.experiment_data["PLATFORMS"].get(job.platform_name, "") == "" and job.platform_name.upper() != "LOCAL":
             raise AutosubmitCritical("Platform does not exists, check the value of %JOBS.{0}.PLATFORM% = {1} parameter".format(job.section,job.platform_name),7000,"List of platforms: {0} ".format(self.experiment_data["PLATFORMS"].keys()) )
         job.file = str(parameters[section].get( "FILE", ""))
         job.additional_files = parameters[section].get( "ADDITIONAL_FILES", [])
 
+        job.executable = str(parameters[section].get("EXECUTABLE", self.experiment_data["PLATFORMS"].get(job.platform_name,{}).get("EXECUTABLE","")))
         job.queue = str(parameters[section].get( "QUEUE", ""))
+
         job.ec_queue = str(parameters[section].get("EC_QUEUE", ""))
         if job.ec_queue == "" and job.platform_name != "LOCAL":
             job.ec_queue = str(self.experiment_data["PLATFORMS"][job.platform_name].get("EC_QUEUE","hpc"))
 
         job.partition = str(parameters[section].get( "PARTITION", ""))
-        if job.partition == "" and job.platform_name.upper() not in ["LOCAL",""]:
-            job.partition = str(self.experiment_data["PLATFORMS"][job.platform_name].get("PARTITION",""))
         job.check = str(parameters[section].get( "CHECK", "true")).lower()
         job.export = str(parameters[section].get( "EXPORT", ""))
         job.processors = str(parameters[section].get( "PROCESSORS", ""))
         job.threads = str(parameters[section].get( "THREADS", ""))
         job.tasks = str(parameters[section].get( "TASKS", ""))
         job.memory = str(parameters[section].get("MEMORY", ""))
         job.memory_per_task = str(parameters[section].get("MEMORY_PER_TASK", ""))
```

### Comparing `autosubmit-4.0.76/autosubmit/job/job_exceptions.py` & `autosubmit-4.0.77/autosubmit/job/job_exceptions.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job_grouping.py` & `autosubmit-4.0.77/autosubmit/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job_list.py` & `autosubmit-4.0.77/autosubmit/job/job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
                     self._ordered_jobs_by_date_member[wrapper_section] = {}
             except BaseException as e:
                 raise AutosubmitCritical("Some section jobs of the wrapper:{0} are not in the current job_list defined in jobs.conf".format(wrapper_section),7014,str(e))
 
 
     @staticmethod
     def _add_dependencies(date_list, member_list, chunk_list, dic_jobs, graph, option="DEPENDENCIES"):
-        jobs_data = dic_jobs._jobs_data["JOBS"]
+        jobs_data = dic_jobs._jobs_data.get("JOBS",{})
         for job_section in jobs_data.keys():
             Log.debug("Adding dependencies for {0} jobs".format(job_section))
             # If it does not have dependencies, do nothing
             if not (job_section, option):
                 continue
 
             dependencies_keys = jobs_data[job_section].get(option,{})
```

### Comparing `autosubmit-4.0.76/autosubmit/job/job_list_persistence.py` & `autosubmit-4.0.77/autosubmit/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job_package_persistence.py` & `autosubmit-4.0.77/autosubmit/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/job/job_packager.py` & `autosubmit-4.0.77/autosubmit/job/job_packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,27 +38,16 @@
     :type as_config: AutosubmitConfig object.\n
     :param platform: A particular platform we are dealing with, e.g. Lsf Platform.\n
     :type platform: Specific Platform Object, e.g. LsfPlatform(), EcPlatform(), ...\n
     :param jobs_list: Contains the list of the jobs, along other properties.\n
     :type jobs_list: JobList object.
     """
 
-    def __init__(self, as_config, platform, jobs_list, hold=False):
-        self.current_wrapper_section = "WRAPPERS"
-        self._as_config = as_config
-        self._platform = platform
-        self._jobs_list = jobs_list
-        self.hold = hold
-        # These are defined in the [wrapper] section of autosubmit_,conf
-        self.wrapper_type = dict()
-        self.wrapper_policy = dict()
-        self.wrapper_method = dict()
-        self.jobs_in_wrapper = dict()
-        self.extensible_wallclock = dict()
-        self.wrapper_info = list()
+    def calculate_job_limits(self,platform,job=None):
+        jobs_list = self._jobs_list
         # Submitted + Queuing Jobs for specific Platform
         queuing_jobs = jobs_list.get_queuing(platform)
         # We now consider the running jobs count
         running_jobs = jobs_list.get_running(platform)
         running_by_id = dict()
         for running_job in running_jobs:
             running_by_id[running_job.id] = running_job
@@ -73,23 +62,46 @@
         submitted_by_id = dict()
         for submitted_job in submitted_jobs:
             submitted_by_id[submitted_job.id] = submitted_job
         submitted_jobs_len = len(list(submitted_by_id.keys()))
 
         waiting_jobs = submitted_jobs_len + queuing_jobs_len
         # Calculate available space in Platform Queue
-        self._max_wait_jobs_to_submit = platform.max_waiting_jobs - waiting_jobs
+        if job is not None and job.max_waiting_jobs != platform.max_waiting_jobs is not None:
+            self._max_wait_jobs_to_submit = job.max_waiting_jobs - waiting_jobs
+        else:
+            self._max_wait_jobs_to_submit = platform.max_waiting_jobs - waiting_jobs
         # .total_jobs is defined in each section of platforms_.yml, if not from there, it comes form autosubmit_.yml
         # .total_jobs Maximum number of jobs at the same time
-        self._max_jobs_to_submit = platform.total_jobs - queuing_jobs_len
+        if job is not None and job.total_jobs != platform.total_jobs:
+            self._max_jobs_to_submit = job.total_jobs - queuing_jobs_len
+        else:
+            self._max_jobs_to_submit = platform.total_jobs - queuing_jobs_len
         # Subtracting running jobs
         self._max_jobs_to_submit = self._max_jobs_to_submit - running_jobs_len
         self._max_jobs_to_submit = self._max_jobs_to_submit if self._max_jobs_to_submit > 0 else 0
         self.max_jobs = min(self._max_wait_jobs_to_submit,self._max_jobs_to_submit)
 
+    def __init__(self, as_config, platform, jobs_list, hold=False):
+        self.current_wrapper_section = "WRAPPERS"
+        self._as_config = as_config
+        self._platform = platform
+        self._jobs_list = jobs_list
+        self.hold = hold
+        # These are defined in the [wrapper] section of autosubmit_,conf
+        self.wrapper_type = dict()
+        self.wrapper_policy = dict()
+        self.wrapper_method = dict()
+        self.jobs_in_wrapper = dict()
+        self.extensible_wallclock = dict()
+        self.wrapper_info = list()
+        self.calculate_job_limits(platform)
+        self.special_variables = dict()
+
+
 
         #todo add default values
         #Wrapper building starts here
         for wrapper_section,wrapper_data in self._as_config.experiment_data.get("WRAPPERS",{}).items():
             if isinstance(wrapper_data,collections.abc.Mapping ):
                 self.wrapper_type[wrapper_section] = self._as_config.get_wrapper_type(wrapper_data)
                 self.wrapper_policy[wrapper_section] = self._as_config.get_wrapper_policy(wrapper_data)
@@ -140,15 +152,21 @@
                     if len(tmp) > completed_jobs:
                         completed_jobs = len(tmp)
                         highest_completed = [job]
                     else:
                         highest_completed.append(job)
             for job in highest_completed:
                 job.distance_weight = job.distance_weight - 1
-
+    def _special_variables(self,job):
+        special_variables = dict()
+        if job.section not in self.special_variables:
+            special_variables[job.section] = dict()
+            if job.total_jobs != self._platform.total_jobs:
+                special_variables[job.section]["TOTAL_JOBS"] = job
+                self.special_variables.update(special_variables)
     def build_packages(self):
         # type: () -> List[JobPackageBase]
         """
         Returns the list of the built packages to be submitted
 
         :return: List of packages depending on type of package, JobPackageVertical Object for 'vertical'.
         :rtype: List() of JobPackageVertical
@@ -190,18 +208,35 @@
                 jobs_ready = sorted_jobs
                 pass
             except IndexError:
                 pass
         if len(jobs_ready) == 0:
             # If there are no jobs ready, result is tuple of empty
             return packages_to_submit
-        if not (self._max_wait_jobs_to_submit > 0 and self._max_jobs_to_submit > 0):
-            # If there is no more space in platform, result is tuple of empty
-            Log.debug("No more space in platform {0} for jobs {1}".format(self._platform.name, [job.name for job in jobs_ready]))
-            return packages_to_submit
+        #check if there are jobs listed on calculate_job_limits
+        for job in jobs_ready:
+            self._special_variables(job)
+        if len(self.special_variables) > 0:
+            for section in self.special_variables:
+                if "TOTAL_JOBS" in self.special_variables[section]:
+                    self.calculate_job_limits(self._platform,self.special_variables[section]["TOTAL_JOBS"])
+                if not (self._max_wait_jobs_to_submit > 0 and self._max_jobs_to_submit > 0):
+                    # If there is no more space in platform, result is tuple of empty
+                    Log.debug("No more space in platform {0} for jobs {1}".format(self._platform.name,
+                                                                                  [job.name for job in jobs_ready]))
+                    return packages_to_submit
+                self.calculate_job_limits(self._platform)
+
+        else:
+            self.calculate_job_limits(self._platform)
+            if not (self._max_wait_jobs_to_submit > 0 and self._max_jobs_to_submit > 0):
+                # If there is no more space in platform, result is tuple of empty
+                Log.debug("No more space in platform {0} for jobs {1}".format(self._platform.name, [job.name for job in jobs_ready]))
+                return packages_to_submit
+
 
         # Sort by 6 first digits of date
         available_sorted = sorted(
             jobs_ready, key=lambda k: k.long_name.split('_')[1][:6])
         # Sort by Priority, the highest first
         list_of_available = sorted(
             available_sorted, key=lambda k: k.priority, reverse=True)
@@ -503,15 +538,15 @@
                                                 if job.status == Status.READY:
                                                     if job.type == Type.PYTHON and not self._platform.allow_python_jobs:
                                                         package = JobPackageSimpleWrapped(
                                                             [job])
                                                     else:
                                                         package = JobPackageSimple([job])
                                                     packages_to_submit.append(package)
-                                            Log.info("Wrapper policy is set to flexible and there is a deadlock, As will submit the jobs sequentially")
+                                            Log.info("Wrapper policy is set to flexible and there is a deadlock, Autosubmit will submit the jobs sequentially")
                     else:
                         for job in jobs:
                             job.packed = False
                             if job.type == Type.PYTHON and not self._platform.allow_python_jobs:
                                 package = JobPackageSimpleWrapped([job])
                             else:
                                 package = JobPackageSimple([job])
```

### Comparing `autosubmit-4.0.76/autosubmit/job/job_packages.py` & `autosubmit-4.0.77/autosubmit/job/job_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     def _create_scripts_threaded(self,jobs,configuration):
         for i in range(0, len(jobs)):
             self._job_scripts[jobs[i].name] = jobs[i].create_script(configuration)
 
     def _create_common_script(self,filename=""):
         pass
 
+
     def submit(self, configuration, parameters,only_generate=False,hold=False):
         """
         :param hold:
         :para configuration: Autosubmit basic configuration \n
         :type configuration: AutosubmitConfig object \n
         :param parameters; Parameters from joblist \n
         :type parameters: JobList,parameters \n
@@ -157,14 +158,16 @@
                                 raise AutosubmitCritical("Template [ {0} ] using CHECK=On_submission has some empty variable {0}".format(job.name),7014)
                         if not job.check_script(configuration, parameters,show_logs=job.check_warnings):
                             Log.warning("Script {0} check failed",job.name)
                             Log.warning("On submission script has some empty variables")
                         else:
                             Log.result("Script {0} OK",job.name)
                     job.update_parameters(configuration, parameters)
+                    # Looking for special variables
+
                     # looking for directives on jobs
                     self._custom_directives = self._custom_directives | set(job.custom_directives)
             else:
                 Lhandle = list()
                 for i in range(0, len(self.jobs), chunksize):
                     Lhandle.append(self.check_scripts(self.jobs[i:i + chunksize], configuration, parameters, only_generate, hold))
                 for dataThread in Lhandle:
@@ -345,27 +348,27 @@
     :param dependency: Name of potential dependency
     :type dependency: String
     """
     FILE_PREFIX = 'ASThread'
 
     def __init__(self, jobs, dependency=None, jobs_resources=dict(),method='ASThread',configuration=None,wrapper_section="WRAPPERS", wrapper_info= {}):
         super(JobPackageThread, self).__init__(jobs)
+        # to be pass as "configuration"
         if len(wrapper_info) > 0 :
             self.wrapper_type = wrapper_info[0]
             self.wrapper_policy = wrapper_info[1]
             self.wrapper_method = wrapper_info[2]
             self.jobs_in_wrapper = wrapper_info[3]
             self.extensible_wallclock = wrapper_info[4]
         else:
             self.wrapper_type = None
             self.wrapper_policy = None
             self.wrapper_method = None
             self.jobs_in_wrapper = None
             self.extensible_wallclock = 0
-
         self._job_scripts = {}
         # Seems like this one is not used at all in the class
         self._job_dependency = dependency
         self._common_script = None
         self._wallclock = '00:00'
         self._num_processors = '0'
         self._jobs_resources = jobs_resources
@@ -386,18 +389,54 @@
             else:
                 self.queue = jobs[0].queue
             wr_partition = configuration.get_wrapper_partition(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
             if wr_partition is not None and len(str(wr_partition)) > 0:
                 self.partition = wr_partition
             else:
                 self.partition = jobs[0].partition
+            wr_exclusive = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXCLUSIVE",False)
+            if  wr_exclusive:
+                self.exclusive = wr_exclusive
+            else:
+                self.exclusive = jobs[0].exclusive
+            wr_custom_directives = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("CUSTOM_DIRECTIVES",[])
+            if len(str(wr_custom_directives)) > 0:
+                self.custom_directives = wr_custom_directives
+            else:
+                self.custom_directives = jobs[0].custom_directives
+            wr_executable = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXECUTABLE",None)
+            if wr_executable is None:
+                self.executable = wr_executable
+            else:
+                self.executable = jobs[0].executable
         else:
             self.queue = jobs[0].queue
             self.partition = jobs[0].partition
         self.method = method
+        self._wrapper_factory.as_conf = configuration
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"] = configuration.experiment_data["WRAPPERS"][self.current_wrapper_section]
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["TYPE"] = self.wrapper_type
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["WRAPPER_POLICY"] = self.wrapper_policy
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["INNER_RETRIALS"] = self.inner_retrials
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXTEND_WALLCLOCK"] = self.extensible_wallclock
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["METHOD"] = self.wrapper_method
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXPORT"] = self.export
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["QUEUE"] = self.queue
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["PARTITION"] = self.partition
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXCLUSIVE"] = self.exclusive
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["EXECUTABLE"] = self.executable
+        self._wrapper_factory.as_conf.experiment_data["CURRENT_WRAPPER"]["CUSTOM_DIRECTIVES"] = self.custom_directives
+
+        pass
+
+
+
+
+
+
 #pipeline
     @property
     def name(self):
         return self._name
     @property
     def _jobs_scripts(self):
         self._jobs_resources['PROCESSORS_PER_NODE'] = self.platform.processors_per_node
```

### Comparing `autosubmit-4.0.76/autosubmit/job/job_utils.py` & `autosubmit-4.0.77/autosubmit/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/monitor/diagram.py` & `autosubmit-4.0.77/autosubmit/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/monitor/monitor.py` & `autosubmit-4.0.77/autosubmit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/monitor/utils.py` & `autosubmit-4.0.77/autosubmit/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/notifications/mail_notifier.py` & `autosubmit-4.0.77/autosubmit/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/notifications/notifier.py` & `autosubmit-4.0.77/autosubmit/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/ecplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/ecplatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,16 +304,15 @@
             return False
         return True
 
     def get_ssh_output(self):
         return self._ssh_output
     def get_ssh_output_err(self):
         return self._ssh_output_err
-    @staticmethod
-    def wrapper_header(filename, queue, project, wallclock, num_procs, expid, dependency, rootdir, directives, partition=""):
+    def wrapper_header(self,**kwargs):
         return """\
         #!/bin/bash
         ###############################################################################
         #              {0}
         ###############################################################################
         #
         #PBS -N {0}
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/ec_cca_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/ec_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/local_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/lsf_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/pbs10_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/pbs11_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/pbs12_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/pjm_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/pjm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/ps_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/sge_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/headers/slurm_header.py` & `autosubmit-4.0.77/autosubmit/platforms/headers/slurm_header.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,27 @@
         :return: account directive
         :rtype: str
         """
         # There is no account, so directive is empty
         if job.parameters['CURRENT_PROJ'] != '':
             return "SBATCH -A {0}".format(job.parameters['CURRENT_PROJ'])
         return ""
+    def get_exclusive_directive(self, job):
+        """
+        Returns account directive for the specified job
+
+        :param job: job to create account directive for
+        :type job: Job
+        :return: account directive
+        :rtype: str
+        """
+        # There is no account, so directive is empty
+        if job.exclusive:
+            return "SBATCH --exclusive"
+        return ""
 
     def get_nodes_directive(self, job):
         """
         Returns nodes directive for the specified job
         :param job: job to create nodes directive for
         :type job: Job
         :return: nodes directive
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/locplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/lsfplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/lsfplatform.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,16 +114,15 @@
     def get_submit_cmd(self, job_script, job, hold=False, export=""):
         if (export is None or export.lower() == "none") or len(export) == 0:
             export = ""
         else:
             export += " ; "
         return export + self._submit_cmd + job_script
 
-    @staticmethod
-    def wrapper_header(filename, queue, project, wallclock, num_procs, dependency, directives, partition=""):
+    def wrapper_header(self,**kwargs):
         return """\
         #!/usr/bin/env python3
         ###############################################################################
         #              {0}
         ###############################################################################
         #
         #BSUB -J {0}
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/paramiko_platform.py` & `autosubmit-4.0.77/autosubmit/platforms/paramiko_platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -640,22 +640,22 @@
         sleep_time = 5
         sleep(sleep_time)
         slurm_error = False
         e_msg = ""
         try:
             self.send_command(cmd)
         except AutosubmitError as e:
-            e_msg = str(e.trace)+" "+str(e.message)
+            e_msg = e.error_message
             slurm_error = True
         if not slurm_error:
             while not self._check_jobid_in_queue(self.get_ssh_output(), job_list_cmd) and retries > 0:
                 try:
                     self.send_command(cmd)
                 except AutosubmitError as e:
-                    e_msg = str(e.trace) + " " + str(e.message)
+                    e_msg = e.error_message
                     slurm_error = True
                     break
                 Log.debug('Retrying check job command: {0}', cmd)
                 Log.debug('retries left {0}', retries)
                 Log.debug('Will be retrying in {0} seconds', sleep_time)
                 retries -= 1
                 sleep(sleep_time)
@@ -723,15 +723,15 @@
                 else:
                     job_status = Status.UNKNOWN
                     Log.error(
                         'check_job() The job id ({0}) status is {1}.', job.id, job_status)
                 job.new_status = job_status
             self.get_queue_status(in_queue_jobs,list_queue_jobid,as_conf)
         else:
-            for job in job_list:
+            for job, job_prev_status in job_list:
                 job_status = Status.UNKNOWN
                 Log.warning(
                     'check_job() The job id ({0}) from platform {1} has an status of {2}.', job.id, self.name, job_status)
             raise AutosubmitError("Some Jobs are in Unknown status", 6008)
             # job.new_status=job_status
         if slurm_error:
             raise AutosubmitError(e_msg,6000)
@@ -756,14 +756,26 @@
         if retries >= 0:
             #get id last line
             job_ids_names = job_id_name.split('\n')[1:-1]
             #get all ids by job-name
             job_ids = [job_id.split(',')[0] for job_id in job_ids_names]
         return job_ids
 
+    def get_queue_status(self, in_queue_jobs, list_queue_jobid, as_conf):
+        """Get queue status for a list of jobs.
+
+        The job statuses are normally found via a command sent to the remote platform.
+
+        Each ``job`` in ``in_queue_jobs`` must be updated. Implementations may check
+        for the reason for queueing cancellation, or if the job is held, and update
+        the ``job`` status appropriately.
+        """
+        raise NotImplementedError
+
+
     def get_checkjob_cmd(self, job_id):
         """
         Returns command to check job status on remote platforms
 
         :param job_id: id of job to check
         :param job_id: int
         :return: command to check job status
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/paramiko_submitter.py` & `autosubmit-4.0.77/autosubmit/platforms/paramiko_submitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http: www.gnu.org / licenses / >.
 
 
 import os
+from collections import defaultdict
 
 from log.log import Log,AutosubmitCritical,AutosubmitError
 from autosubmitconfigparser.config.basicconfig import BasicConfig
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 from .submitter import Submitter
 from autosubmit.platforms.psplatform import PsPlatform
 from autosubmit.platforms.lsfplatform import LsfPlatform
@@ -62,43 +63,53 @@
             BasicConfig.LOCAL_ROOT_DIR, local_platform.expid)
         local_platform.host = 'localhost'
         # Add object to entry in dictionary
         platforms['local'] = local_platform
         platforms['LOCAL'] = local_platform
         self.platforms = platforms
 
+
     def load_platforms(self, asconf, retries=5):
         """
         Create all the platforms object that will be used by the experiment
 
         :param retries: retries in case creation of service fails
         :param asconf: autosubmit config to use
         :type asconf: AutosubmitConfig
         :return: platforms used by the experiment
         :rtype: dict
         """
         exp_data = asconf.experiment_data
+        config = BasicConfig().props()
+        config.update(exp_data)
         raise_message=""
         platforms_used = list()
         hpcarch = asconf.get_platform()
         platforms_used.append(hpcarch)
-
+        platforms_serial_in_paralell = defaultdict(list)
         # Traverse jobs defined in jobs_.conf and add platforms found if not already included
         jobs_data = exp_data.get('JOBS', {})
         for job in jobs_data:
             hpc = jobs_data[job].get('PLATFORM', hpcarch).upper()
             if hpc not in platforms_used:
                 platforms_used.append(hpc)
+        # Traverse used platforms and look for serial_platforms and add them if not already included
+        for platform in platforms_used:
+            hpc = asconf.experiment_data.get("PLATFORMS",{}).get(platform,{}).get("SERIAL_PLATFORM", None)
+            if hpc is not None:
+                platforms_serial_in_paralell[hpc].append(platform)
+                if hpc not in platforms_used:
+                    platforms_used.append(hpc)
 
         platform_data = exp_data.get('PLATFORMS', {})
         # Declare platforms dictionary, key: Platform Name, Value: Platform Object
         platforms = dict()
 
         # Build Local Platform Object
-        local_platform = LocalPlatform(asconf.expid, 'local', BasicConfig)
+        local_platform = LocalPlatform(asconf.expid, 'local', config)
         local_platform.max_wallclock = asconf.get_max_wallclock()
         local_platform.max_processors = asconf.get_max_processors()
         local_platform.max_waiting_jobs = asconf.get_max_waiting_jobs()
         local_platform.total_jobs = asconf.get_total_jobs()
         local_platform.scratch = os.path.join(
             BasicConfig.LOCAL_ROOT_DIR, asconf.expid, BasicConfig.LOCAL_TMP_DIR)
         local_platform.temp_dir = os.path.join(
@@ -114,36 +125,37 @@
         for section in platform_data:
             # Consider only those included in the list of jobs
             if section not in platforms_used:
                 continue
 
             platform_type = platform_data[section].get('TYPE', '').lower()
             platform_version = platform_data[section].get('VERSION', '')
+
             try:
                 if platform_type == 'pbs':
                     remote_platform = PBSPlatform(
-                        asconf.expid, section, BasicConfig, platform_version)
+                        asconf.expid, section, config, platform_version)
                 elif platform_type == 'sge':
                     remote_platform = SgePlatform(
-                        asconf.expid, section, BasicConfig)
+                        asconf.expid, section, config)
                 elif platform_type == 'ps':
                     remote_platform = PsPlatform(
-                        asconf.expid, section, BasicConfig)
+                        asconf.expid, section, config)
                 elif platform_type == 'lsf':
                     remote_platform = LsfPlatform(
-                        asconf.expid, section, BasicConfig)
+                        asconf.expid, section, config)
                 elif platform_type == 'ecaccess':
                     remote_platform = EcPlatform(
-                        asconf.expid, section, BasicConfig, platform_version)
+                        asconf.expid, section, config, platform_version)
                 elif platform_type == 'slurm':
                     remote_platform = SlurmPlatform(
-                        asconf.expid, section, BasicConfig)
+                        asconf.expid, section, config)
                 elif platform_type == 'pjm':
                     remote_platform = PJMPlatform(
-                        asconf.expid, section, BasicConfig)
+                        asconf.expid, section, config)
                 else:
                     raise Exception(
                         "Queue type not specified on platform {0}".format(section))
 
             except ParamikoPlatformException as e:
                 Log.error("Queue exception: {0}".format(str(e)))
                 return None
@@ -179,15 +191,18 @@
             remote_platform.reservation = platform_data[section].get('RESERVATION', "")
             remote_platform.exclusivity = platform_data[section].get('EXCLUSIVITY', "")
             remote_platform.user = platform_data[section].get('USER', "")
             remote_platform.scratch = platform_data[section].get('SCRATCH_DIR', "")
             remote_platform.project_dir = platform_data[section].get('SCRATCH_PROJECT_DIR', remote_platform.project)
             remote_platform.temp_dir = platform_data[section].get('TEMP_DIR', "")
             remote_platform._default_queue = platform_data[section].get('QUEUE', "")
+            remote_platform._partition = platform_data[section].get('PARTITION', "")
             remote_platform._serial_queue = platform_data[section].get('SERIAL_QUEUE', "")
+            remote_platform._serial_partition = platform_data[section].get('SERIAL_PARTITION', "")
+
             remote_platform.ec_queue = platform_data[section].get('EC_QUEUE', "hpc")
 
             remote_platform.ec_queue = platform_data[section].get('EC_QUEUE', "hpc")
 
             remote_platform.processors_per_node = platform_data[section].get('PROCESSORS_PER_NODE',"1")
             remote_platform.custom_directives = platform_data[section].get('CUSTOM_DIRECTIVES',"")
             if len(remote_platform.custom_directives) > 0:
@@ -200,15 +215,15 @@
 
                 platforms[section] = remote_platform
             except Exception as e:
                 raise_message = "Error in platform.conf: SCRATCH_DIR, PROJECT, USER, EXPID must be defined for platform {0}".format(section)
             # Executes update_cmds() from corresponding Platform Object
             # Save platform into result dictionary
 
-            serial = platform_data[section].get('SERIAL_PLATFORM',None)
-            if serial is not None and len(str(serial)) > 0:
-                platforms[section].serial_platform = serial.upper()
+        for serial,platforms_with_serial_options in platforms_serial_in_paralell.items():
+            for section in platforms_with_serial_options:
+                platforms[section].serial_platform = platforms[serial]
 
 
         self.platforms = platforms
         if raise_message != "":
             raise AutosubmitError(raise_message)
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/pbsplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/pjmplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/pjmplatform.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         self.job_status['QUEUING'] = ['ACC','QUE', 'RNA', 'RNP','HLD'] # TODO NOT SURE ABOUT HOLD HLD
         self.job_status['FAILED'] = ['ERR','CCL','RJT']
         self._pathdir = "\$HOME/LOG_" + self.expid
         self._allow_arrays = False
         self._allow_wrappers = True # NOT SURE IF WE NEED WRAPPERS
         self.update_cmds()
         self.config = config
-        exp_id_path = os.path.join(config.LOCAL_ROOT_DIR, self.expid)
+        exp_id_path = os.path.join(self.config.get("LOCAL_ROOT_DIR"), self.expid)
         tmp_path = os.path.join(exp_id_path, "tmp")
         self._submit_script_path = os.path.join(
-            tmp_path, config.LOCAL_ASLOG_DIR, "submit_" + self.name + ".sh")
+            tmp_path, self.config.get("LOCAL_ASLOG_DIR"), "submit_" + self.name + ".sh")
         self._submit_script_file = open(self._submit_script_path, 'wb').close()
 
     def submit_error(self,output):
         """
         Check if the output of the submit command contains an error message.
         :param output: output of the submit cmd
         :return: boolean
@@ -160,15 +160,15 @@
     def open_submit_script(self):
         self._submit_script_file = open(self._submit_script_path, 'wb').close()
         self._submit_script_file = open(self._submit_script_path, 'ab')
 
     def get_submit_script(self):
         self._submit_script_file.close()
         os.chmod(self._submit_script_path, 0o750)
-        return os.path.join(self.config.LOCAL_ASLOG_DIR, os.path.basename(self._submit_script_path))
+        return os.path.join(self.config.get("LOCAL_ASLOG_DIR"), os.path.basename(self._submit_script_path))
 
     def submit_job(self, job, script_name, hold=False, export="none"):
         """
         Submit a job from a given job object.
 
         :param export:
         :param job: job object
@@ -408,16 +408,15 @@
         reason = [x.split()[2] for x in output.splitlines()
                   if x.split()[0] == str(job_id)]
         # In case of duplicates.. we take the first one
         if len(reason) > 0:
             return reason[0]
         return reason
 
-    @staticmethod
-    def wrapper_header(filename, queue, project, wallclock, num_procs, dependency, directives, threads, method="asthreads", partition=""):
+    def wrapper_header(self,**kwargs):
         if method == 'srun':
             language = "#!/bin/bash"
             return \
                 language + """
 ###############################################################################
 #              {0}
 ###############################################################################
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/platform.py` & `autosubmit-4.0.77/autosubmit/platforms/platform.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,20 @@
         :param name:
         """
         self.connected = False
         self.expid = expid # type: str
         self.name = name # type: str
         self.config = config
         self.tmp_path = os.path.join(
-            self.config.LOCAL_ROOT_DIR, self.expid, self.config.LOCAL_TMP_DIR)
+            self.config.get("LOCAL_ROOT_DIR"), self.expid, self.config.get("LOCAL_TMP_DIR"))
         self._serial_platform = None
         self._serial_queue = None
+        self._serial_partition = None
         self._default_queue = None
+        self._partition = None
         self.ec_queue = "hpc"
         self.processors_per_node = "1"
         self.scratch_free_space = None
         self.custom_directives = None
         self.host = ''
         self.user = ''
         self.project = ''
@@ -57,15 +59,24 @@
         self.get_cmd = None
         self.put_cmd = None
         self._submit_hold_cmd = None
         self._submit_command_name = None
         self._submit_cmd = None
         self._checkhost_cmd = None
         self.cancel_cmd = None
-
+    def get_exclusive_directive(self, job):
+        """
+        Returns exclusive directive for the specified job
+        :param job: job to create exclusive directive for
+        :type job: Job
+        :return: exclusive directive
+        :rtype: str
+        """
+        # only implemented for slurm
+        return ""
     def get_multiple_jobids(self,job_list,valid_packages_to_submit,failed_packages,error_message="",hold=False):
         return False,valid_packages_to_submit
         #raise NotImplementedError
 
     def process_batch_ready_jobs(self, valid_packages_to_submit, failed_packages, error_message="", hold=False):
         return True, valid_packages_to_submit
 
@@ -190,38 +201,66 @@
         if self._serial_platform is None:
             return self
         return self._serial_platform
 
     @serial_platform.setter
     def serial_platform(self, value):
         self._serial_platform = value
+    @property
+    def partition(self):
+        """
+        Partition to use for jobs
+        :return: queue's name
+        :rtype: str
+        """
+        if self._partition is None:
+            return ''
+        return self._partition
 
+    @partition.setter
+    def partition(self, value):
+        self._partition = value
     @property
     def queue(self):
         """
         Queue to use for jobs
         :return: queue's name
         :rtype: str
         """
-        if self._default_queue is None:
+        if self._default_queue is None or self._default_queue == "":
             return ''
         return self._default_queue
 
     @queue.setter
     def queue(self, value):
         self._default_queue = value
 
     @property
+    def serial_partition(self):
+        """
+        Partition to use for serial jobs
+        :return: partition's name
+        :rtype: str
+        """
+        if self._serial_partition is None or self._serial_partition == "":
+            return self.partition
+        return self._serial_partition
+
+    @serial_partition.setter
+    def serial_partition(self, value):
+        self._serial_partition = value
+
+    @property
     def serial_queue(self):
         """
         Queue to use for serial jobs
         :return: queue's name
         :rtype: str
         """
-        if self._serial_queue is None:
+        if self._serial_queue is None or self._serial_queue == "":
             return self.queue
         return self._serial_queue
 
     @serial_queue.setter
     def serial_queue(self, value):
         self._serial_queue = value
 
@@ -258,14 +297,16 @@
         else:
             prefix = self.name + '_'
 
         parameters['{0}ARCH'.format(prefix)] = self.name
         parameters['{0}HOST'.format(prefix)] = self.host
         parameters['{0}QUEUE'.format(prefix)] = self.queue
         parameters['{0}EC_QUEUE'.format(prefix)] = self.ec_queue
+        parameters['{0}PARTITION'.format(prefix)] = self.partition
+
 
         parameters['{0}USER'.format(prefix)] = self.user
         parameters['{0}PROJ'.format(prefix)] = self.project
         parameters['{0}BUDG'.format(prefix)] = self.budget
         parameters['{0}RESERVATION'.format(prefix)] = self.reservation
         parameters['{0}EXCLUSIVITY'.format(prefix)] = self.exclusivity
         parameters['{0}TYPE'.format(prefix)] = self.type
@@ -436,15 +477,15 @@
         :param job_name: name of job to check
         :type job_name: str
         :return: True if successful, False otherwise
         :rtype: bool
         """
         filename = job_name + '_STAT'
         stat_local_path = os.path.join(
-            self.config.LOCAL_ROOT_DIR, self.expid, self.config.LOCAL_TMP_DIR, filename)
+            self.config.get("LOCAL_ROOT_DIR"), self.expid, self.config.get("LOCAL_TMP_DIR"), filename)
         if os.path.exists(stat_local_path):
             os.remove(stat_local_path)
         if self.check_file_exists(filename):
             if self.get_file(filename, True):
                 Log.debug('{0}_STAT file have been transferred', job_name)
                 return True
         Log.debug('{0}_STAT file not found', job_name)
@@ -476,15 +517,15 @@
         :param job_name: name of job to check
         :type job_name: str
         :return: True if successful, False otherwise
         :rtype: bool
         """
         filename = job_name
         stat_local_path = os.path.join(
-            self.config.LOCAL_ROOT_DIR, self.expid, self.config.LOCAL_TMP_DIR, filename)
+            self.config.get("LOCAL_ROOT_DIR"), self.expid, self.config.get("LOCAL_TMP_DIR"), filename)
         if os.path.exists(stat_local_path):
             os.remove(stat_local_path)
         if self.check_file_exists(filename):
             if self.get_file(filename, True):
                 return True
             else:
                 return False
@@ -496,15 +537,15 @@
         Get the path to the platform's LOG directory
 
         :return: platform's LOG directory
         :rtype: str
         """
         if self.type == "local":
             path = os.path.join(
-                self.root_dir, self.config.LOCAL_TMP_DIR, 'LOG_{0}'.format(self.expid))
+                self.root_dir, self.config.get("LOCAL_TMP_DIR"), 'LOG_{0}'.format(self.expid))
         else:
             path = os.path.join(self.root_dir, 'LOG_{0}'.format(self.expid))
         return path
 
     def submit_job(self, job, script_name, hold=False, export="none"):
         """
         Submit a job from a given job object.
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/psplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/sgeplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/slurmplatform.py` & `autosubmit-4.0.77/autosubmit/platforms/slurmplatform.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         self.job_status['FAILED'] = ['FAILED', 'CANCELLED', 'CANCELLED+', 'NODE_FAIL',
                                      'PREEMPTED', 'SUSPENDED', 'TIMEOUT', 'OUT_OF_MEMORY', 'OUT_OF_ME+', 'OUT_OF_ME']
         self._pathdir = "\$HOME/LOG_" + self.expid
         self._allow_arrays = False
         self._allow_wrappers = True
         self.update_cmds()
         self.config = config
-        exp_id_path = os.path.join(config.LOCAL_ROOT_DIR, self.expid)
+        exp_id_path = os.path.join(self.config.get("LOCAL_ROOT_DIR"), self.expid)
         tmp_path = os.path.join(exp_id_path, "tmp")
         self._submit_script_path = os.path.join(
-            tmp_path, config.LOCAL_ASLOG_DIR, "submit_" + self.name + ".sh")
+            tmp_path, self.config.get("LOCAL_ASLOG_DIR"), "submit_" + self.name + ".sh")
         self._submit_script_file = open(self._submit_script_path, 'wb').close()
 
     def process_batch_ready_jobs(self,valid_packages_to_submit,failed_packages,error_message="",hold=False):
         """
         Retrieve multiple jobs identifiers.
         :param valid_packages_to_submit:
         :param failed_packages:
@@ -109,17 +109,15 @@
                                     error_msg += job_tmp.section + "&"
                         if has_trace_bad_parameters:
                             error_message+="Check job and queue specified in jobs.conf. Sections that could be affected: {0}".format(error_msg[:-1])
                         else:
                             error_message+="\ncheck that {1} platform has set the correct scheduler. Sections that could be affected: {0}".format(
                                     error_msg[:-1], self.name)
 
-                        if e.trace is None:
-                            e.trace = ""
-                        raise AutosubmitCritical(error_message,7014,e.message+"\n"+str(e.trace))
+                        raise AutosubmitCritical(error_message, 7014, e.error_message)
                 except IOError as e:
                     raise AutosubmitError(
                         "IO issues ", 6016, str(e))
                 except BaseException as e:
                     if str(e).find("scheduler") != -1:
                         raise AutosubmitCritical("Are you sure that [{0}] scheduler is the correct type for platform [{1}]?.\n Please, double check that {0} is loaded for {1} before autosubmit launch any job.".format(self.type.upper(),self.name.upper()),7070)
                     raise AutosubmitError(
@@ -186,15 +184,15 @@
     def open_submit_script(self):
         self._submit_script_file = open(self._submit_script_path, 'wb').close()
         self._submit_script_file = open(self._submit_script_path, 'ab')
 
     def get_submit_script(self):
         self._submit_script_file.close()
         os.chmod(self._submit_script_path, 0o750)
-        return os.path.join(self.config.LOCAL_ASLOG_DIR, os.path.basename(self._submit_script_path))
+        return os.path.join(self.config.get("LOCAL_ASLOG_DIR"), os.path.basename(self._submit_script_path))
 
     def submit_job(self, job, script_name, hold=False, export="none"):
         """
         Submit a job from a given job object.
 
         :param export:
         :param job: job object
@@ -602,63 +600,46 @@
             elif reason == '(JobHeldUser)':
                 if not job.hold:
                     # should be self.release_cmd or something like that but it is not implemented
                     self.send_command("scontrol release {0}".format(job.id))
                     job.new_status = Status.QUEUING  # If it was HELD and was released, it should be QUEUING next.
                 else:
                     job.new_status = Status.HELD
-    @staticmethod
-    def wrapper_header(filename, queue, project, wallclock, num_procs, dependency, directives, threads, method="asthreads", partition=""):
-        if method == 'srun':
-            language = "#!/bin/bash"
-            return \
-                language + """
+    def wrapper_header(self,**kwargs):
+        wr_header = f"""
 ###############################################################################
-#              {0}
+#              {kwargs["name"].split("_")[0]+"_Wrapper"}
 ###############################################################################
 #
-#SBATCH -J {0}
-{1}
-{8}
-#SBATCH -A {2}
-#SBATCH --output={0}.out
-#SBATCH --error={0}.err
-#SBATCH -t {3}:00
-#SBATCH -n {4}
-#SBATCH --cpus-per-task={7}
-{5}
-{6}
+#SBATCH -J {kwargs["name"]}
+{kwargs["queue"]}
+{kwargs["partition"]}
+{kwargs["dependency"]}
+#SBATCH -A {kwargs["project"]}
+#SBATCH --output={kwargs["name"]}.out
+#SBATCH --error={kwargs["name"]}.err
+#SBATCH -t {kwargs["wallclock"]}:00
+#SBATCH -n {kwargs["num_processors"]}
+#SBATCH --cpus-per-task={kwargs["threads"]}
+{kwargs["exclusive"]}
+{kwargs["custom_directives"]}
 
 #
 ###############################################################################
-                """.format(filename, queue, project, wallclock, num_procs, dependency,
-                           '\n'.ljust(13).join(str(s) for s in directives), threads,partition)
+"""
+        if kwargs["method"] == 'srun':
+            language = kwargs["executable"]
+            if language is None or len(language) == 0:
+                language = "#!/bin/bash"
+            return language + wr_header
         else:
-            language = "#!/usr/bin/env python3"
-            return \
-                language + """
-###############################################################################
-#              {0}
-###############################################################################
-#
-#SBATCH -J {0}
-{1}
-{8}
-#SBATCH -A {2}
-#SBATCH --output={0}.out
-#SBATCH --error={0}.err
-#SBATCH -t {3}:00
-#SBATCH --cpus-per-task={7}
-#SBATCH -n {4}
-{5}
-{6}
-#
-###############################################################################
-            """.format(filename, queue, project, wallclock, num_procs, dependency,
-                       '\n'.ljust(13).join(str(s) for s in directives), threads,partition)
+            language = kwargs["executable"]
+            if language is None or len(language) == 0:
+                language = "#!/usr/bin/env python3"
+            return language + wr_header
 
     @staticmethod
     def allocated_nodes():
         return """os.system("scontrol show hostnames $SLURM_JOB_NODELIST > node_list_{0}".format(node_id))"""
 
     def check_file_exists(self, filename,wrapper_failed=False):
         file_exist = False
```

### Comparing `autosubmit-4.0.76/autosubmit/platforms/submitter.py` & `autosubmit-4.0.77/autosubmit/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/wrappers/wrapper_builder.py` & `autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/platforms/wrappers/wrapper_factory.py` & `autosubmit-4.0.77/autosubmit/platforms/wrappers/wrapper_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,23 +22,28 @@
     BashHorizontalWrapperBuilder, BashVerticalWrapperBuilder, SrunHorizontalWrapperBuilder,SrunVerticalHorizontalWrapperBuilder
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 
 
 class WrapperFactory(object):
 
     def __init__(self, platform):
+        self.as_conf = None
         self.platform = platform
         self.wrapper_director = WrapperDirector()
         self.exception = "This type of wrapper is not supported for this platform"
 
     def get_wrapper(self, wrapper_builder, **kwargs):
+        wrapper_data = self.as_conf.experiment_data["CURRENT_WRAPPER"]
         kwargs['allocated_nodes'] = self.allocated_nodes()
         kwargs['dependency'] = self.dependency(kwargs['dependency'])
         kwargs['queue'] = self.queue(kwargs['queue'])
-        kwargs['partition'] = self.partition(kwargs['partition'])
+        kwargs['partition'] = self.partition(wrapper_data['PARTITION'])
+        kwargs["exclusive"] = self.exclusive(wrapper_data['EXCLUSIVE'])
+        kwargs["custom_directives"] = self.custom_directives(wrapper_data["CUSTOM_DIRECTIVES"])
+        kwargs["executable"] = wrapper_data["EXECUTABLE"]
         kwargs['header_directive'] = self.header_directives(**kwargs)
         builder = wrapper_builder(**kwargs)
         return self.wrapper_director.construct(builder)
 
     def vertical_wrapper(self, **kwargs):
         raise NotImplemented(self.exception)
 
@@ -55,26 +60,43 @@
         pass
 
     def allocated_nodes(self):
         return ''
 
     def dependency(self, dependency):
         return '#' if dependency is None else self.dependency_directive(dependency)
-
     def queue(self, queue):
         return '#' if not queue else self.queue_directive(queue)
     def partition(self, partition):
         return '#' if not partition else self.partition_directive(partition)
+    def exclusive(self, exclusive):
+        return '#' if not exclusive or str(exclusive).lower() == "false" else self.exclusive_directive(exclusive)
+    def custom_directives(self, custom_directives):
+        return '#' if not custom_directives else self.get_custom_directives(custom_directives)
+    def get_custom_directives(self, custom_directives):
+        """
+        Returns custom directives for the specified job
+        :param job: Job object
+        :return: String with custom directives
+        """
+        # There is no custom directives, so directive is empty
+        if custom_directives != '':
+            return '\n'.join(str(s) for s in custom_directives)
+        return ""
+
     def dependency_directive(self, dependency):
         pass
-
     def queue_directive(self, queue):
         pass
     def partition_directive(self, partition):
         pass
+    def exclusive_directive(self, exclusive):
+        pass
+
+
 
 
 class SlurmWrapperFactory(WrapperFactory):
 
     def vertical_wrapper(self, **kwargs):
         return PythonVerticalWrapperBuilder(**kwargs)
 
@@ -91,41 +113,41 @@
     def hybrid_wrapper_vertical_horizontal(self, **kwargs):
         if kwargs["method"] == 'srun':
             return SrunVerticalHorizontalWrapperBuilder(**kwargs)
         else:
             return PythonVerticalHorizontalWrapperBuilder(**kwargs)
 
     def header_directives(self, **kwargs):
-        return self.platform.wrapper_header(kwargs['name'], kwargs['queue'], kwargs['project'], kwargs['wallclock'],
-                                            kwargs['num_processors'], kwargs['dependency'], kwargs['directives'],kwargs['threads'],kwargs['method'],kwargs['partition'])
+        return self.platform.wrapper_header(**kwargs)
 
     def allocated_nodes(self):
         return self.platform.allocated_nodes()
 
     def dependency_directive(self, dependency):
         return '#SBATCH --dependency=afterok:{0}'.format(dependency)
 
     def queue_directive(self, queue):
         return '#SBATCH --qos={0}'.format(queue)
 
     def partition_directive(self, partition):
         return '#SBATCH --partition={0}'.format(partition)
+    def exclusive_directive(self, exclusive):
+        return '#SBATCH --exclusive'
 
 
 class LSFWrapperFactory(WrapperFactory):
 
     def vertical_wrapper(self, **kwargs):
         return PythonVerticalWrapperBuilder(**kwargs)
 
     def horizontal_wrapper(self, **kwargs):
         return PythonHorizontalWrapperBuilder(**kwargs)
 
     def header_directives(self, **kwargs):
-        return self.platform.wrapper_header(kwargs['name'], kwargs['queue'], kwargs['project'], kwargs['wallclock'],
-                                            kwargs['num_processors'], kwargs['dependency'], kwargs['directives'],kwargs['threads'])
+        return self.platform.wrapper_header(**kwargs)
 
     def queue_directive(self, queue):
         return queue
 
     def dependency_directive(self, dependency):
         return '#BSUB -w \'done({0})\' [-ti]'.format(dependency)
 
@@ -135,17 +157,15 @@
     def vertical_wrapper(self, **kwargs):
         return BashVerticalWrapperBuilder(**kwargs)
 
     def horizontal_wrapper(self, **kwargs):
         return BashHorizontalWrapperBuilder(**kwargs)
 
     def header_directives(self, **kwargs):
-        return self.platform.wrapper_header(kwargs['name'], kwargs['queue'], kwargs['project'], kwargs['wallclock'],
-                                            kwargs['num_processors'], kwargs['expid'], kwargs['dependency'],
-                                            kwargs['rootdir'], kwargs['directives'],kwargs['threads'])
+        return self.platform.wrapper_header(**kwargs)
 
     def queue_directive(self, queue):
         return queue
 
     def dependency_directive(self, dependency):
         return '#PBS -v depend=afterok:{0}'.format(dependency)
 
@@ -167,16 +187,15 @@
     def hybrid_wrapper_vertical_horizontal(self, **kwargs):
         if kwargs["method"] == 'srun':
             return SrunVerticalHorizontalWrapperBuilder(**kwargs)
         else:
             return PythonVerticalHorizontalWrapperBuilder(**kwargs)
 
     def header_directives(self, **kwargs):
-        return self.platform.wrapper_header(kwargs['name'], kwargs['queue'], kwargs['project'], kwargs['wallclock'],
-                                            kwargs['num_processors'], kwargs['dependency'], kwargs['directives'],kwargs['threads'],kwargs['method'],kwargs['partition'])
+        return self.platform.wrapper_header(**kwargs)
 
     def allocated_nodes(self):
         return self.platform.allocated_nodes()
 
     #def dependency_directive(self, dependency):
     #    # There is no option for afterok in the PJM scheduler, but I think it is not needed.
     #    return '#PJM --dependency=afterok:{0}'.format(dependency)
```

### Comparing `autosubmit-4.0.76/autosubmit/statistics/jobs_stat.py` & `autosubmit-4.0.77/autosubmit/statistics/jobs_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/statistics/statistics.py` & `autosubmit-4.0.77/autosubmit/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/statistics/stats_summary.py` & `autosubmit-4.0.77/autosubmit/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit/statistics/utils.py` & `autosubmit-4.0.77/autosubmit/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/autosubmit.egg-info/PKG-INFO` & `autosubmit-4.0.77/autosubmit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.76
+Version: 4.0.77
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
 Platform: GNU/Linux Debian
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
+Autosubmit is a lightweight workflow manager and meta-scheduler. It was originally designed in 2011 for use in climate research for configuring and running experiments. In the last few years, it has been extended to cover additional use cases, and today it is used as a general orchestration tool. It supports scheduling jobs to remote batch servers (via SSH) such as PBS, LSF, SLURM, and SGE.
 
-Autosubmit is a lightweight workflow manager designed to meet climate research necessities. Unlike other workflow solutions in the domain, it integrates the capabilities of an experiment manager, workflow orchestrator and monitor in a self-contained application. The experiment manager allows for defining and configuring experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts. These multi-scale workflows can involve from a few to thousands of steps and from one to multiple platforms.
+Autosubmit is a Python package provided in PyPI, which facilitates easy and fast integration and relocation on new platforms. Conda recipes are available on the project website. A containerized version for testing purposes is also available but not public yet.
 
-Autosubmit facilitates easy and fast integration and relocation on new platforms. On the one hand, users can rapidly execute general scripts and progressively parametrize them by reading Autosubmit variables. On the other hand, it is a self-contained desktop application capable of submitting jobs to remote platforms without any external deployment.
+The features found in Autosubmit characterize it as both an experiment manager and also as a workflow orchestrator. The experiment manager allows users to define and configure experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts.
 
-Due to its robustness, it can handle different eventualities, such as networking or I/O errors. Finally, the monitoring capabilities extend beyond the desktop application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI. 
+These multi-scale workflows can contain from a few steps to thousands of steps, and from a single platform to multiple platforms. Platform is a concept in Autosubmit to abstract servers. A workflow configuration can include one or multiple platforms, allowing the workflow to run on any number of servers via password-less SSH without any external deployment.
 
-Autosubmit is a Python package provided in PyPI. Conda recipes can also be found on the website. A containerized version for testing purposes is also available but not public yet.
+Due to its robustness it can handle different eventualities such as networking connectivity issues or I/O errors. The monitoring capabilities extend beyond the command-line application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI.
 
-It has contributed to various European research projects and runs different operational systems. During the following years, it will support some of the Earth Digital Twins as the Digital Twin Ocean.
+It has contributed to various European research projects and runs different operational systems. It will support the Earth Digital Twins as the Digital Twin Ocean over the next years.
 
-Concretely, it is currently used at Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES...), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and many other. Autosubmit has run these workflows in different supercomputers in BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+It is currently used at the Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES, and others), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and for many other use cases. Autosubmit has been used to run workflows in different supercomputers at BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
```

### Comparing `autosubmit-4.0.76/autosubmit.egg-info/SOURCES.txt` & `autosubmit-4.0.77/autosubmit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,17 @@
 test/unit/test_history.py
 test/unit/test_job.py
 test/unit/test_job_common.py
 test/unit/test_job_graph.py
 test/unit/test_job_grouping.py
 test/unit/test_job_list.py
 test/unit/test_job_package.py
+test/unit/test_log.py
 test/unit/test_machinefiles_wrapper.py
+test/unit/test_paramiko_platform.py
 test/unit/test_pjm.py
 test/unit/test_platform_monitor.py
 test/unit/test_setup.py
+test/unit/test_slurm_platform.py
 test/unit/test_statistics.py
 test/unit/test_strategies.py
 test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.76/bin/autosubmit` & `autosubmit-4.0.77/bin/autosubmit`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/Makefile` & `autosubmit-4.0.77/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/autosubmit.pdf` & `autosubmit-4.0.77/docs/autosubmit.pdf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/experiment/fig/fig_experiment.jpg` & `autosubmit-4.0.77/docs/source/agui/experiment/fig/fig_experiment.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/experiment/index.rst` & `autosubmit-4.0.77/docs/source/agui/experiment/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig1_gui.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig1_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig2_gui.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig2_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig3_gui.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig3_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig4_gui.jpg` & `autosubmit-4.0.77/docs/source/agui/fig/fig4_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig5_gui.jpg` & `autosubmit-4.0.77/docs/source/agui/fig/fig5_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig_ev_1.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig_ev_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig_tree_1.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig_tree_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/fig/fig_tree_2.png` & `autosubmit-4.0.77/docs/source/agui/fig/fig_tree_2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_1.jpg` & `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_2.jpg` & `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_3.jpg` & `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_3.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/graph/fig/fig_graph_4.jpg` & `autosubmit-4.0.77/docs/source/agui/graph/fig/fig_graph_4.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/graph/index.rst` & `autosubmit-4.0.77/docs/source/agui/graph/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/index.rst` & `autosubmit-4.0.77/docs/source/agui/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/log/fig/fig_log_1.jpg` & `autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/log/fig/fig_log_2.jpg` & `autosubmit-4.0.77/docs/source/agui/log/fig/fig_log_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/log/index.rst` & `autosubmit-4.0.77/docs/source/agui/log/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/performance/fig/fig_performance_1.jpg` & `autosubmit-4.0.77/docs/source/agui/performance/fig/fig_performance_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/performance/index.rst` & `autosubmit-4.0.77/docs/source/agui/performance/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/statistics/fig/fig_stat_1.jpg` & `autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/statistics/fig/fig_stat_2.jpg` & `autosubmit-4.0.77/docs/source/agui/statistics/fig/fig_stat_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/statistics/index.rst` & `autosubmit-4.0.77/docs/source/agui/statistics/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/tree/fig/fig_tree_2.jpg` & `autosubmit-4.0.77/docs/source/agui/tree/fig/fig_tree_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/agui/tree/index.rst` & `autosubmit-4.0.77/docs/source/agui/tree/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/conf.py` & `autosubmit-4.0.77/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/devguide/index.rst` & `autosubmit-4.0.77/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/index.rst` & `autosubmit-4.0.77/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/installation/index.rst` & `autosubmit-4.0.77/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/introduction/fig1.png` & `autosubmit-4.0.77/docs/source/introduction/fig1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/introduction/fig2.png` & `autosubmit-4.0.77/docs/source/introduction/fig2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/introduction/fig3.png` & `autosubmit-4.0.77/docs/source/introduction/fig3.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/introduction/index.rst` & `autosubmit-4.0.77/docs/source/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/moduledoc/platforms.rst` & `autosubmit-4.0.77/docs/source/moduledoc/platforms.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/qstartguide/dummy.png` & `autosubmit-4.0.77/docs/source/qstartguide/dummy.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/qstartguide/index.rst` & `autosubmit-4.0.77/docs/source/qstartguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/changelog.rst` & `autosubmit-4.0.77/docs/source/troubleshooting/changelog.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/error-codes.rst` & `autosubmit-4.0.77/docs/source/troubleshooting/error-codes.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/fig/monarch-da.png` & `autosubmit-4.0.77/docs/source/troubleshooting/fig/monarch-da.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/fig/new_dependencies_0.png` & `autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_0.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/fig/new_dependencies_1.png` & `autosubmit-4.0.77/docs/source/troubleshooting/fig/new_dependencies_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/troubleshooting/index.rst` & `autosubmit-4.0.77/docs/source/troubleshooting/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/unused_figs/group_chunk.png` & `autosubmit-4.0.77/docs/source/unused_figs/group_chunk.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/unused_figs/horizontal-vertical.png` & `autosubmit-4.0.77/docs/source/unused_figs/horizontal-vertical.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/unused_figs/wrapper.png` & `autosubmit-4.0.77/docs/source/unused_figs/wrapper.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/unused_figs/wrapper_expression.png` & `autosubmit-4.0.77/docs/source/unused_figs/wrapper_expression.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/unused_figs/wrapper_hybrid.png` & `autosubmit-4.0.77/docs/source/unused_figs/wrapper_hybrid.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/configure/develop_a_project.rst` & `autosubmit-4.0.77/docs/source/userguide/configure/develop_a_project.rst`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
     The ``MAX_WALLCLOCK`` field is optional.
     The ``MAX_PROCESSORS`` field is optional.
     The ``PROCESSORS_PER_NODE`` field is optional.
 
 .. warning::
 
     The ``SERIAL_QUEUE`` and ``QUEUE`` field are used for specify a -QOS.
-    For specify a partition, you must use ``CUSTOM_DIRECTIVES``.
+    For specify a partition, you must use ``PARTITION``.
     For specify the memory usage you must use ``MEMORY`` but only in jobs.yml.
 
 The custom directives can be used for multiple parameters at the same time using the follow syntax.
 
     vi <expid>/conf/platform_cxxx.yml
 
 .. code-block:: yaml
```

### Comparing `autosubmit-4.0.76/docs/source/userguide/configure/index.rst` & `autosubmit-4.0.77/docs/source/userguide/configure/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/create/index.rst` & `autosubmit-4.0.77/docs/source/userguide/create/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/index.rst` & `autosubmit-4.0.77/docs/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/manage/index.rst` & `autosubmit-4.0.77/docs/source/userguide/manage/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/run/index.rst` & `autosubmit-4.0.77/docs/source/userguide/run/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/dasim.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/dasim.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/horizontal_remote.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/horizontal_remote.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/multiple_wrappers.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/multiple_wrappers.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/rerun.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/rerun.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/vertical-horizontal.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-horizontal.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/fig/vertical-mixed.png` & `autosubmit-4.0.77/docs/source/userguide/wrappers/fig/vertical-mixed.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/docs/source/userguide/wrappers/index.rst` & `autosubmit-4.0.77/docs/source/userguide/wrappers/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/environment.yml` & `autosubmit-4.0.77/environment.yml`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - bcrypt
 - pip
 - mock
 - portalocker
 - networkx
 - sqlite
 - pip:
-  - autosubmitconfigparser==1.0.24
+  - autosubmitconfigparser==1.0.26
   - argparse>=1.4.0
   - bcrypt>=3.2.0
   - python-dateutil>=2.8.2
   - matplotlib>=3.5.1
   - numpy<1.22
   - py3dotplus>=1.1.0
   - pyparsing>=3.0.7
```

### Comparing `autosubmit-4.0.76/log/fd_show.py` & `autosubmit-4.0.77/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/log/log.py` & `autosubmit-4.0.77/log/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import logging
 import os
 import sys
 from time import sleep
 from datetime import datetime
+from typing import Union
 
 
 class AutosubmitError(Exception):
-    """Exception raised for Autosubmit critical errors .
+    """Exception raised for Autosubmit errors.
+
     Attributes:
-        errorcode -- Classified code
-        message -- explanation of the error
+        message (str): explanation of the error
+        code (int): classified code
+        trace (str): extra information about the error
     """
 
-    def __init__(self, message="Unhandled Error", code=6000, trace=None):
+    def __init__(self, message="Unhandled Error", code=6000, trace: Union[None, str]=None):
         self.code = code
         self.message = message
         self.trace = trace
 
+    @property
+    def error_message(self) -> str:
+        """
+        Return the error message ready to be logged, with both trace
+        (when present) and the message separated by a space. Or just
+        the message if no trace is available.
+
+        :return: ``trace`` and ``message`` separated by a space, or just the
+                 ``message`` if no ``trace`` is available.
+        :rtype: str
+        """
+        return self.message if not self.trace else f'{self.trace} {self.message}'
+
     def __str__(self):
         return " "
 
 
 class AutosubmitCritical(Exception):
     """Exception raised for Autosubmit critical errors .
     Attributes:
```

### Comparing `autosubmit-4.0.76/setup.py` & `autosubmit-4.0.77/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description='Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.',
     long_description=open('README_PIP.md').read(),
     author='Daniel Beltran Mora',
     author_email='daniel.beltran@bsc.es',
     url='http://www.bsc.es/projects/earthscience/autosubmit/',
     download_url='https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit',
     keywords=['climate', 'weather', 'workflow', 'HPC'],
-    install_requires=['autosubmitconfigparser==1.0.24','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','ruamel.yaml','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
+    install_requires=['autosubmitconfigparser==1.0.25','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','ruamel.yaml','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux",
     ],
     packages=find_packages(),
```

### Comparing `autosubmit-4.0.76/test/integration/test_db_manager.py` & `autosubmit-4.0.77/test/integration/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/integration/test_job.py` & `autosubmit-4.0.77/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/README` & `autosubmit-4.0.77/test/regression/README`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/default_conf/platforms.conf` & `autosubmit-4.0.77/test/regression/default_conf/platforms.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.77/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mistral_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mistral_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn3_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_moore_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_moore_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_sedema_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.77/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/tests.conf` & `autosubmit-4.0.77/test/regression/tests.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/tests_commands.py` & `autosubmit-4.0.77/test/regression/tests_commands.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/tests_log.py` & `autosubmit-4.0.77/test/regression/tests_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/tests_runner.py` & `autosubmit-4.0.77/test/regression/tests_runner.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/regression/tests_utils.py` & `autosubmit-4.0.77/test/regression/tests_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/README_PIP.md` & `autosubmit-4.0.77/README_PIP.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+Autosubmit is a lightweight workflow manager and meta-scheduler. It was originally designed in 2011 for use in climate research for configuring and running experiments. In the last few years, it has been extended to cover additional use cases, and today it is used as a general orchestration tool. It supports scheduling jobs to remote batch servers (via SSH) such as PBS, LSF, SLURM, and SGE.
 
-Autosubmit is a lightweight workflow manager designed to meet climate research necessities. Unlike other workflow solutions in the domain, it integrates the capabilities of an experiment manager, workflow orchestrator and monitor in a self-contained application. The experiment manager allows for defining and configuring experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts. These multi-scale workflows can involve from a few to thousands of steps and from one to multiple platforms.
+Autosubmit is a Python package provided in PyPI, which facilitates easy and fast integration and relocation on new platforms. Conda recipes are available on the project website. A containerized version for testing purposes is also available but not public yet.
 
-Autosubmit facilitates easy and fast integration and relocation on new platforms. On the one hand, users can rapidly execute general scripts and progressively parametrize them by reading Autosubmit variables. On the other hand, it is a self-contained desktop application capable of submitting jobs to remote platforms without any external deployment.
+The features found in Autosubmit characterize it as both an experiment manager and also as a workflow orchestrator. The experiment manager allows users to define and configure experiments, supported by a hierarchical database that ensures reproducibility and traceability. The orchestrator is designed to run complex workflows in research and operational mode by managing their dependencies and interfacing with local and remote hosts.
 
-Due to its robustness, it can handle different eventualities, such as networking or I/O errors. Finally, the monitoring capabilities extend beyond the desktop application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI. 
+These multi-scale workflows can contain from a few steps to thousands of steps, and from a single platform to multiple platforms. Platform is a concept in Autosubmit to abstract servers. A workflow configuration can include one or multiple platforms, allowing the workflow to run on any number of servers via password-less SSH without any external deployment.
 
-Autosubmit is a Python package provided in PyPI. Conda recipes can also be found on the website. A containerized version for testing purposes is also available but not public yet.
+Due to its robustness it can handle different eventualities such as networking connectivity issues or I/O errors. The monitoring capabilities extend beyond the command-line application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI.
 
-It has contributed to various European research projects and runs different operational systems. During the following years, it will support some of the Earth Digital Twins as the Digital Twin Ocean.
+It has contributed to various European research projects and runs different operational systems. It will support the Earth Digital Twins as the Digital Twin Ocean over the next years.
 
-Concretely, it is currently used at Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES...), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and many other. Autosubmit has run these workflows in different supercomputers in BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+It is currently used at the Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES, and others), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and for many other use cases. Autosubmit has been used to run workflows in different supercomputers at BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
```

### Comparing `autosubmit-4.0.76/test/unit/test_basic_config.py` & `autosubmit-4.0.77/test/unit/test_basic_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_catlog.py` & `autosubmit-4.0.77/test/unit/test_catlog.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_chunk_date_lib.py` & `autosubmit-4.0.77/test/unit/test_chunk_date_lib.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_database_managers.py` & `autosubmit-4.0.77/test/unit/test_database_managers.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_db_manager.py` & `autosubmit-4.0.77/test/unit/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_dic_jobs.py` & `autosubmit-4.0.77/test/unit/test_dic_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,19 +549,25 @@
 
         self.dictionary._create_jobs_once(mock_section.name, priority, Type.BASH, dict(),splits)
 
         self.assertEqual(mock_section, self.dictionary._dic[mock_section.name])
         self.dictionary.build_job.assert_called_once_with(mock_section.name, priority, None, None, None, Type.BASH, {},splits)
         self.job_list.graph.add_node.assert_called_once_with(mock_section.name)
 
-
+import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
-
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     DEFAULT_PLATFORMS_CONF = ''
```

### Comparing `autosubmit-4.0.76/test/unit/test_expid.py` & `autosubmit-4.0.77/test/unit/test_expid.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_history.py` & `autosubmit-4.0.77/test/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_job.py` & `autosubmit-4.0.77/test/unit/test_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,37 +30,37 @@
         self.as_conf.experiment_data["PLATFORMS"] = dict()
         self.job = Job(self.job_name, self.job_id, Status.WAITING, self.job_priority)
         self.job.processors = 2
         self.as_conf.load_project_parameters = Mock(return_value=dict())
 
 
     def test_when_the_job_has_more_than_one_processor_returns_the_parallel_platform(self):
-        platform = Platform(self.experiment_id, 'parallel-platform', FakeBasicConfig)
+        platform = Platform(self.experiment_id, 'parallel-platform', FakeBasicConfig().props())
         platform.serial_platform = 'serial-platform'
 
         self.job._platform = platform
         self.job.processors = 999
 
         returned_platform = self.job.platform
 
         self.assertEqual(platform, returned_platform)
 
     def test_when_the_job_has_only_one_processor_returns_the_serial_platform(self):
-        platform = Platform(self.experiment_id, 'parallel-platform', FakeBasicConfig)
+        platform = Platform(self.experiment_id, 'parallel-platform', FakeBasicConfig().props())
         platform.serial_platform = 'serial-platform'
 
         self.job._platform = platform
         self.job.processors = 1
 
         returned_platform = self.job.platform
 
         self.assertEqual('serial-platform', returned_platform)
 
     def test_set_platform(self):
-        dummy_platform = Platform('whatever', 'rand-name', FakeBasicConfig)
+        dummy_platform = Platform('whatever', 'rand-name', FakeBasicConfig().props())
         self.assertNotEqual(dummy_platform, self.job.platform)
 
         self.job.platform = dummy_platform
 
         self.assertEqual(dummy_platform, self.job.platform)
 
     def test_when_the_job_has_a_queue_returns_that_queue(self):
@@ -69,33 +69,33 @@
 
         returned_queue = self.job.queue
 
         self.assertEqual(dummy_queue, returned_queue)
 
     def test_when_the_job_has_not_a_queue_and_some_processors_returns_the_queue_of_the_platform(self):
         dummy_queue = 'whatever-parallel'
-        dummy_platform = Platform('whatever', 'rand-name', FakeBasicConfig)
+        dummy_platform = Platform('whatever', 'rand-name', FakeBasicConfig().props())
         dummy_platform.queue = dummy_queue
         self.job.platform = dummy_platform
 
         self.assertIsNone(self.job._queue)
 
         returned_queue = self.job.queue
 
         self.assertIsNotNone(returned_queue)
         self.assertEqual(dummy_queue, returned_queue)
 
     def test_when_the_job_has_not_a_queue_and_one_processor_returns_the_queue_of_the_serial_platform(self):
         serial_queue = 'whatever-serial'
         parallel_queue = 'whatever-parallel'
 
-        dummy_serial_platform = Platform('whatever', 'serial', FakeBasicConfig)
+        dummy_serial_platform = Platform('whatever', 'serial', FakeBasicConfig().props())
         dummy_serial_platform.serial_queue = serial_queue
 
-        dummy_platform = Platform('whatever', 'parallel', FakeBasicConfig)
+        dummy_platform = Platform('whatever', 'parallel', FakeBasicConfig().props())
         dummy_platform.serial_platform = dummy_serial_platform
         dummy_platform.queue = parallel_queue
         dummy_platform.processors_per_node = "1"
         #dummy_platform.hyperthreading = "false"
 
         self.job._platform = dummy_platform
         self.job.processors = '1'
@@ -308,20 +308,31 @@
         self.assertTrue('Y' in parameters)
         self.assertTrue('Y_' in parameters)
         self.assertEqual('%d%', parameters['d'])
         self.assertEqual('%d_%', parameters['d_'])
         self.assertEqual('%Y%', parameters['Y'])
         self.assertEqual('%Y_%', parameters['Y_'])
 
-
+import inspect
 class FakeBasicConfig:
+    def __init__(self):
+        pass
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
+    #convert this to dict
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     DEFAULT_PLATFORMS_CONF = ''
     DEFAULT_JOBS_CONF = ''
 
 
 
+
```

### Comparing `autosubmit-4.0.76/test/unit/test_job_common.py` & `autosubmit-4.0.77/test/unit/test_job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_job_graph.py` & `autosubmit-4.0.77/test/unit/test_job_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,15 +914,14 @@
 
         job.date = date
         job.member = member
         job.chunk = chunk
         job.split = split
 
         return job
-
 class FakeBasicConfig:
     def __init__(self):
         pass
 
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
```

### Comparing `autosubmit-4.0.76/test/unit/test_job_grouping.py` & `autosubmit-4.0.77/test/unit/test_job_grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,19 +979,25 @@
 
         job.date = parse_date(date)
         job.member = member
         job.chunk = chunk
         job.split = split
 
         return job
-
+import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
-
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     DEFAULT_PLATFORMS_CONF = ''
```

### Comparing `autosubmit-4.0.76/test/unit/test_job_list.py` & `autosubmit-4.0.77/test/unit/test_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,19 +271,25 @@
     def _createDummyJobWithStatus(self, status):
         job_name = str(randrange(999999, 999999999))
         job_id = randrange(1, 999)
         job = Job(job_name, job_id, status, 0)
         job.type = randrange(0, 2)
         return job
 
-
+import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
-
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     DEFAULT_PLATFORMS_CONF = ''
```

### Comparing `autosubmit-4.0.76/test/unit/test_job_package.py` & `autosubmit-4.0.77/test/unit/test_job_package.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_machinefiles_wrapper.py` & `autosubmit-4.0.77/test/unit/test_machinefiles_wrapper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_pjm.py` & `autosubmit-4.0.77/test/unit/test_pjm.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,23 @@
 from pathlib import Path
 from autosubmit.platforms.platform import Platform
 from autosubmit.platforms.pjmplatform import PJMPlatform
 import autosubmit.platforms.headers.pjm_header
 from tempfile import TemporaryDirectory
 from datetime import datetime
 from autosubmit.job.job import Job, Status
-
+import inspect
 class FakeBasicConfig:
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     LOCAL_ASLOG_DIR = '/dummy/local/aslog/dir'
```

### Comparing `autosubmit-4.0.76/test/unit/test_platform_monitor.py` & `autosubmit-4.0.77/test/unit/test_platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_statistics.py` & `autosubmit-4.0.77/test/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_strategies.py` & `autosubmit-4.0.77/test/unit/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.76/test/unit/test_wrappers.py` & `autosubmit-4.0.77/test/unit/test_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,26 @@
         cls.workflows['running_once']['sections']["s5"] = dict()
         cls.workflows['running_once']['sections']["s5"]["RUNNING"] = "once"
         cls.workflows['running_once']['sections']["s5"]["WALLCLOCK"] = '00:30'
         cls.workflows['running_once']['sections']["s5"]["DEPENDENCIES"] = "s2"
 
     def setUp(self):
         self.experiment_id = 'random-id'
+        self._wrapper_factory = MagicMock()
+
         self.config = FakeBasicConfig
         self._platform = MagicMock()
         self.as_conf = MagicMock()
         self.as_conf.experiment_data = dict()
         self.as_conf.experiment_data["JOBS"] = dict()
         self.as_conf.jobs_data = self.as_conf.experiment_data["JOBS"]
 
         self.as_conf.experiment_data["PLATFORMS"] = dict()
         self.as_conf.experiment_data["WRAPPERS"] = dict()
+
         self.job_list = JobList(self.experiment_id, self.config, YAMLParserFactory(),
                                 JobListPersistenceDb('.', '.'),self.as_conf)
         self.parser_mock = MagicMock(spec='SafeConfigParser')
 
         self._platform.max_waiting_jobs = 100
         self._platform.total_jobs = 100
         self.config.get_wrapper_type = MagicMock(return_value='vertical')
@@ -181,14 +184,16 @@
             'METHOD': "ASThread",
             'QUEUE': "debug",
             'POLICY': "flexible",
             'RETRIALS': 0,
             'EXTEND_WALLCLOCK': 0
         }
         self.as_conf.experiment_data["WRAPPERS"]["WRAPPERS"] = options
+        self.as_conf.experiment_data["WRAPPERS"]["CURRENT_WRAPPER"] = options
+        self._wrapper_factory.as_conf = self.as_conf
         self.job_packager = JobPackager(
             self.as_conf, self._platform, self.job_list)
         self.job_list._ordered_jobs_by_date_member["WRAPPERS"] = dict()
 
     ### ONE SECTION WRAPPER ###
     def test_returned_packages(self):
         self.current_wrapper_section = {}
@@ -261,16 +266,15 @@
             section_list, wrapper_limits)
 
         package_m1_s2 = [d1_m1_1_s2, d1_m1_2_s2, d1_m1_3_s2, d1_m1_4_s2, d1_m1_5_s2, d1_m1_6_s2, d1_m1_7_s2, d1_m1_8_s2,
                          d1_m1_9_s2, d1_m1_10_s2]
         package_m2_s2 = [d1_m2_1_s2, d1_m2_2_s2, d1_m2_3_s2, d1_m2_4_s2, d1_m2_5_s2, d1_m2_6_s2, d1_m2_7_s2, d1_m2_8_s2,
                          d1_m2_9_s2, d1_m2_10_s2]
 
-        packages = [JobPackageVertical(
-            package_m1_s2), JobPackageVertical(package_m2_s2)]
+        packages = [JobPackageVertical(package_m1_s2,configuration=self.as_conf), JobPackageVertical(package_m2_s2,configuration=self.as_conf)]
 
         # returned_packages = returned_packages[]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_max_jobs(self):
         date_list = ["d1", "d2"]
@@ -344,15 +348,15 @@
 
         package_m1_s2 = [d1_m1_1_s2, d1_m1_2_s2, d1_m1_3_s2, d1_m1_4_s2, d1_m1_5_s2, d1_m1_6_s2, d1_m1_7_s2, d1_m1_8_s2,
                          d1_m1_9_s2, d1_m1_10_s2]
         package_m2_s2 = [d1_m2_1_s2, d1_m2_2_s2, d1_m2_3_s2, d1_m2_4_s2, d1_m2_5_s2, d1_m2_6_s2, d1_m2_7_s2, d1_m2_8_s2,
                          d1_m2_9_s2, d1_m2_10_s2]
 
         packages = [JobPackageVertical(
-            package_m1_s2), JobPackageVertical(package_m2_s2)]
+            package_m1_s2,configuration=self.as_conf), JobPackageVertical(package_m2_s2,configuration=self.as_conf)]
 
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_max_wrapped_jobs(self):
         date_list = ["d1", "d2"]
         member_list = ["m1", "m2"]
@@ -414,15 +418,15 @@
 
         package_m1_s2 = [d1_m1_1_s2, d1_m1_2_s2,
                          d1_m1_3_s2, d1_m1_4_s2, d1_m1_5_s2]
         package_m2_s2 = [d1_m2_1_s2, d1_m2_2_s2,
                          d1_m2_3_s2, d1_m2_4_s2, d1_m2_5_s2]
 
         packages = [JobPackageVertical(
-            package_m1_s2), JobPackageVertical(package_m2_s2)]
+            package_m1_s2,configuration=self.as_conf), JobPackageVertical(package_m2_s2,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_max_wallclock(self):
         date_list = ["d1", "d2"]
@@ -485,15 +489,15 @@
 
         package_m1_s2 = [d1_m1_1_s2, d1_m1_2_s2,
                          d1_m1_3_s2, d1_m1_4_s2, d1_m1_5_s2]
         package_m2_s2 = [d1_m2_1_s2, d1_m2_2_s2,
                          d1_m2_3_s2, d1_m2_4_s2, d1_m2_5_s2]
 
         packages = [JobPackageVertical(
-            package_m1_s2), JobPackageVertical(package_m2_s2)]
+            package_m1_s2,configuration=self.as_conf), JobPackageVertical(package_m2_s2,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_section_not_self_dependent(self):
         date_list = ["d1", "d2"]
@@ -553,15 +557,15 @@
 
         self.job_list._ordered_jobs_by_date_member["WRAPPERS"]["d1"]["m2"] = [d1_m2_1_s3]
 
         package_m1_s2 = [d1_m1_1_s3]
         package_m2_s2 = [d1_m2_1_s3]
 
         packages = [JobPackageVertical(
-            package_m1_s2), JobPackageVertical(package_m2_s2)]
+            package_m1_s2,configuration=self.as_conf), JobPackageVertical(package_m2_s2,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     ### MIXED WRAPPER ###
     def test_returned_packages_mixed_wrapper(self):
@@ -636,15 +640,15 @@
 
         package_m1_s2_s3 = [d1_m1_1_s2, d1_m1_1_s3, d1_m1_2_s2, d1_m1_2_s3, d1_m1_3_s2, d1_m1_3_s3, d1_m1_4_s2,
                             d1_m1_4_s3]
         package_m2_s2_s3 = [d1_m2_1_s2, d1_m2_1_s3, d1_m2_2_s2, d1_m2_2_s3, d1_m2_3_s2, d1_m2_3_s3, d1_m2_4_s2,
                             d1_m2_4_s3]
 
         packages = [JobPackageVertical(
-            package_m1_s2_s3), JobPackageVertical(package_m2_s2_s3)]
+            package_m1_s2_s3,configuration=self.as_conf), JobPackageVertical(package_m2_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_parent_failed_mixed_wrapper(self):
         date_list = ["d1"]
@@ -713,15 +717,15 @@
         wrapper_limits["max_by_section"] = max_wrapper_job_by_section
         returned_packages = self.job_packager._build_vertical_packages(
             section_list, wrapper_limits)
 
         package_m1_s2_s3 = [d1_m1_1_s2, d1_m1_1_s3, d1_m1_2_s2, d1_m1_2_s3, d1_m1_3_s2, d1_m1_3_s3, d1_m1_4_s2,
                             d1_m1_4_s3]
 
-        packages = [JobPackageVertical(package_m1_s2_s3)]
+        packages = [JobPackageVertical(package_m1_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_max_jobs_mixed_wrapper(self):
         wrapper_expression = "s2 s3"
@@ -795,15 +799,15 @@
 
         package_m1_s2_s3 = [d1_m1_1_s2, d1_m1_1_s3, d1_m1_2_s2, d1_m1_2_s3, d1_m1_3_s2, d1_m1_3_s3, d1_m1_4_s2,
                             d1_m1_4_s3]
         package_m2_s2_s3 = [d1_m2_1_s2, d1_m2_1_s3, d1_m2_2_s2, d1_m2_2_s3, d1_m2_3_s2, d1_m2_3_s3, d1_m2_4_s2,
                             d1_m2_4_s3]
 
         packages = [JobPackageVertical(
-            package_m1_s2_s3), JobPackageVertical(package_m2_s2_s3)]
+            package_m1_s2_s3,configuration=self.as_conf), JobPackageVertical(package_m2_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         # print("test_returned_packages_max_jobs_mixed_wrapper")
         for i in range(0, len(returned_packages)):
             # print("Element " + str(i))
             # print("Returned from packager")
             # for job in returned_packages[i]._jobs:
@@ -885,15 +889,15 @@
 
         package_m1_s2_s3 = [d1_m1_1_s2, d1_m1_1_s3,
                             d1_m1_2_s2, d1_m1_2_s3, d1_m1_3_s2]
         package_m2_s2_s3 = [d1_m2_1_s2, d1_m2_1_s3,
                             d1_m2_2_s2, d1_m2_2_s3, d1_m2_3_s2]
 
         packages = [JobPackageVertical(
-            package_m1_s2_s3), JobPackageVertical(package_m2_s2_s3)]
+            package_m1_s2_s3,configuration=self.as_conf), JobPackageVertical(package_m2_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_max_wallclock_mixed_wrapper(self):
         date_list = ["d1"]
@@ -965,15 +969,15 @@
         returned_packages = self.job_packager._build_vertical_packages(
             section_list, wrapper_limits)
 
         package_m1_s2_s3 = [d1_m1_1_s2, d1_m1_1_s3, d1_m1_2_s2, d1_m1_2_s3]
         package_m2_s2_s3 = [d1_m2_1_s2, d1_m2_1_s3, d1_m2_2_s2, d1_m2_2_s3]
 
         packages = [JobPackageVertical(
-            package_m1_s2_s3), JobPackageVertical(package_m2_s2_s3)]
+            package_m1_s2_s3,configuration=self.as_conf), JobPackageVertical(package_m2_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_returned_packages_first_chunks_completed_mixed_wrapper(self):
         date_list = ["d1"]
@@ -1063,15 +1067,15 @@
         returned_packages = self.job_packager._build_vertical_packages(
             section_list, wrapper_limits)
 
         package_m1_s2_s3 = [d1_m1_2_s3, d1_m1_3_s3, d1_m1_4_s2, d1_m1_4_s3]
         package_m2_s2_s3 = [d1_m2_3_s2, d1_m2_3_s3, d1_m2_4_s2, d1_m2_4_s3]
 
         packages = [JobPackageVertical(
-            package_m1_s2_s3), JobPackageVertical(package_m2_s2_s3)]
+            package_m1_s2_s3,configuration=self.as_conf), JobPackageVertical(package_m2_s2_s3,configuration=self.as_conf)]
 
         #returned_packages = returned_packages[0]
         for i in range(0, len(returned_packages)):
             self.assertListEqual(returned_packages[i]._jobs, packages[i]._jobs)
 
     def test_ordered_dict_jobs_simple_workflow_mixed_wrapper(self):
         date_list = ["d1"]
@@ -1511,19 +1515,25 @@
         job.date = date
         job.member = member
         job.chunk = chunk
         job.section = section
 
         return job
 
-
+import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
-
+    def props(self):
+        pr = {}
+        for name in dir(self):
+            value = getattr(self, name)
+            if not name.startswith('__') and not inspect.ismethod(value) and not inspect.isfunction(value):
+                pr[name] = value
+        return pr
     DB_DIR = '/dummy/db/dir'
     DB_FILE = '/dummy/db/file'
     DB_PATH = '/dummy/db/path'
     LOCAL_ROOT_DIR = '/dummy/local/root/dir'
     LOCAL_TMP_DIR = '/dummy/local/temp/dir'
     LOCAL_PROJ_DIR = '/dummy/local/proj/dir'
     DEFAULT_PLATFORMS_CONF = ''
```

