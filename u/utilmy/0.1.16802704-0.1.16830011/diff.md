# Comparing `tmp/utilmy-0.1.16802704.tar.gz` & `tmp/utilmy-0.1.16830011.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilmy-0.1.16802704.tar", last modified: Fri Mar 31 13:47:33 2023, max compression
+gzip compressed data, was "utilmy-0.1.16830011.tar", last modified: Tue May  2 04:20:02 2023, max compression
```

## Comparing `utilmy-0.1.16802704.tar` & `utilmy-0.1.16830011.tar`

### file list

```diff
@@ -1,1874 +1,1874 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-31 13:47:18.000000 utilmy-0.1.16802704/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-31 13:47:32.000000 utilmy-0.1.16802704/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.587289 utilmy-0.1.16802704/utilmy/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/abash.py
--rw-r--r--   0 runner    (1001) docker     (123)    22843 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/adatasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/aws_spot_price.sh
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/ec2_spot_t3small.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/lambda/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/lambda/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32884 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_autoscale_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_launch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_monitor_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.595289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/main.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.547289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.547289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.595289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result10.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result11.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result4.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result5.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result6.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result7.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result8.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result9.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.595289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.595289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/mockscript1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/test_util_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/test_functionnal.sh
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/test_unit.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/test_util_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.547289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/test_aws_lambda_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/
--rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/00_AWS_BATCH_localpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/01_hyperparams_generator_localpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/05_batch_getresults_from_aws_locapc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_a_tasks_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_b_subprocess_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx10/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx10/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx11/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx11/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx12/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx12/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx13/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx13/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/params.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/subprocess_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.599289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/params.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/subprocess_pygmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.603289 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/aws_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_local_aws_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/util_cpu2.py
--rw-r--r--   0 runner    (1001) docker     (123)    66856 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/z_batch_lambda_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/util_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/cloud/aws/util_aws_daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.603289 utilmy-0.1.16802704/utilmy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/config_val.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.603289 utilmy-0.1.16802704/utilmy/configs/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/config_loguru.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/util_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/logs/util_log_std.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/pydantic_config_val.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/util_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25795 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/util_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/configs/util_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.603289 utilmy-0.1.16802704/utilmy/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/keyvalue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.607289 utilmy-0.1.16802704/utilmy/db/kvs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/couch_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)    30511 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/couch_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.607289 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.607289 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/kvdb/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb.go
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb_test.go
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/out
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.607289 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.607289 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_credis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker_macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker_v3.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/start_redis_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/util_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/kvs/util_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.611289 utilmy-0.1.16802704/utilmy/db/qdrant/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/dbvector.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/qdrant_example.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/qdrantinstall.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/startups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/qdrant/triplet.py
--rw-r--r--   0 runner    (1001) docker     (123)    84424 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/db/util_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.611289 utilmy-0.1.16802704/utilmy/deeplearning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.611289 utilmy-0.1.16802704/utilmy/deeplearning/autoencoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/autoencoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/autoencoder/keras_ae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.615289 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/
--rw-r--r--   0 runner    (1001) docker     (123)   106455 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/VAE.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/loss_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/loss_vq_vae2.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    88665 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_graph_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    93118 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_vqvae_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    23984 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_dataloader_img.py
--rw-r--r--   0 runner    (1001) docker     (123)    41275 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_dataloader_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_train.py
--rw-r--r--   0 runner    (1001) docker     (123)    23462 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/zkeras_torch_sentence.py
--rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/kkeras/zz_util_dataloader_img_old.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.615289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.619289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/i3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/x3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.619289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.623289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/affinity_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/amsoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/conv_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/dual_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/focal_loss_old.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/frelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/generalized_iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/group_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/info_nce_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/label_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/large_margin_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/lovasz_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/ohem_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/partial_fc_amsoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/pc_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/soft_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/taylor_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    93646 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/model_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.623289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30479 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/graphnlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38062 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/rule_encoder4.py
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/sentences_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/torch_lstm_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.623289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/layer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/model_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/torchinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/util_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52445 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/util_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.627289 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46285 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/model_ensemble_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    38058 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/rule_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    55129 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble2.py
--rw-r--r--   0 runner    (1001) docker     (123)    64675 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble4.py
--rw-r--r--   0 runner    (1001) docker     (123)    66230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    41242 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zrule_encoder2.py
--rw-r--r--   0 runner    (1001) docker     (123)   233273 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zsentence_tansformer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    70406 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zz_model_ensemble2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.627289 utilmy-0.1.16802704/utilmy/deeplearning/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/tutorial/transf.py
--rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/tutorial/zz_util_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34126 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    31983 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)    28915 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    38131 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/deeplearning/util_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.631290 utilmy-0.1.16802704/utilmy/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    56725 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    34839 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    19475 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/format2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/generate_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/generate_typehint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.631290 utilmy-0.1.16802704/utilmy/docs/test_script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.631290 utilmy-0.1.16802704/utilmy/docs/test_script/output/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.635290 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_normalize_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_normalize_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/test_script/test_script_normalize_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/util_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/util_template2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/zold_cli_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/zold_docstring2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/docs/zold_docstring3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.635290 utilmy-0.1.16802704/utilmy/excel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/excel/xl_pytthon.xlsm
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/excel/xlvba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.635290 utilmy-0.1.16802704/utilmy/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/graph/util_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/iio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.635290 utilmy-0.1.16802704/utilmy/images/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/images/TODO.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39561 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/images/util_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.639290 utilmy-0.1.16802704/utilmy/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.639290 utilmy-0.1.16802704/utilmy/nlp/kkeras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/kkeras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/kkeras/sentences.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ner_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.639290 utilmy-0.1.16802704/utilmy/nlp/ttorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.639290 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/kgDriverCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/knowledge_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.639290 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/kgDriverCode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/knowledge_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/mytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/pykeenTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38692 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/model_patent.py
--rw-r--r--   0 runner    (1001) docker     (123)    31070 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/ttorch/sentences.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_cocount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_gensim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    59668 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/util_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nlp/zzz_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/nnumpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/oos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.643290 utilmy-0.1.16802704/utilmy/optim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/expression_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/gp_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    89758 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/gp_searchformulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/res_ranking.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/util_hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/util_optim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.643290 utilmy-0.1.16802704/utilmy/optim/zold/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/gp_dcgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/gp_dcgp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/gp_formulae.py
--rw-r--r--   0 runner    (1001) docker     (123)    40314 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/optim/zold/gp_searchformulae_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    37954 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    30398 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/ppandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/ppolars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.643290 utilmy-0.1.16802704/utilmy/prepro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/prepro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/prepro_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/prepro_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/prepro_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/run_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    60684 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/prepro/util_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36899 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/bandits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/aabandit_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    29619 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/data_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/data_reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.647290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/bq.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/embed_dnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/preprocessing/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/serving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/serving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/serving/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/training/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/model_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/model_trainers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/configs/example_feature_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/configs/example_ml_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/scripts/create_bq_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/scripts/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/scripts/schemas/training_data.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.651290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/serving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/serving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24906 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/serving/test_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/training/test_train_bandit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/1 - Evaluating a new fraud policy with IPS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/2 - Evaluating a new fraud policy with the direct method.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/3 - Evaluating a new fraud policy with the doubly robust method.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.655290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/gbdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/direct_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/doubly_robust.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/inverse_propensity_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/training/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/epsilon_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/exp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.659290 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/create_movielens_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/eda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/visualize_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/ucb.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.559289 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/data/ml-20m/
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/data/ml-20m/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/contrib/placeholder
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.663290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/usage/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   109315 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/Bandit_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/DQN_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/deep_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/genetic_rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/genetic_rl_q_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.563289 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/known_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/known_parameters/placeholder
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/
--rw-r--r--   0 runner    (1001) docker     (123)    86016 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/A2C-CartPole-v0-ep100.db
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/a2c_cartpole-v0.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/td3_pendulum-v0.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/run_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.667290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/bootstrap_neural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/linpos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_linpos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_noise_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bernoulli_mab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/epsgreedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gaussian_mab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/ucb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/qlearning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/sarsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/valueiteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.671290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/offpolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/onpolicy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/ddpg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/dueling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/noisy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/prioritized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/ppo1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/sac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.675290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/vpg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.679290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/rollout_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.679290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/action_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/atari_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/gym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.679290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/vector_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.679290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/genetic_hyperparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/classical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/offpolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/onpolicy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/adult_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/census_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/covertype_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/magic_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/mushroom_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/statlog_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/discount.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.683290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_cb_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_data_bandits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_mab_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_multi_armed_bandits.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.687290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/test_agents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.687290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_a2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ddpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ppo1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_td3.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_vpg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.687290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.687290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_atari_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_vecenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.687290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_bandit_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_classical_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_deep_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.691290 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/offline_replayer_eval_amzon.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/bandits/recostep_offline_replayer_eval_movielens.py
--rw-r--r--   0 runner    (1001) docker     (123)    29315 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.691290 utilmy-0.1.16802704/utilmy/recsys/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/metrics/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/metrics/distance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.691290 utilmy-0.1.16802704/utilmy/recsys/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.691290 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessAmazonSportsOutdoors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessAmazonVideoGames.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessML20M.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessMSD.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessNetflix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessYahooMovies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/TrainModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    23417 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/CEASE/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.695290 utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/DynEASEr_Runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/ease.py
--rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/prepro1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57019 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/prepro_ae_identity.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/prod2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.695290 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/online_logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.695290 utilmy-0.1.16802704/utilmy/recsys/ranking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/optim_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/rank_fusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/rank_fusion_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/util_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/ranking/util_rankmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/util_ltr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/util_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/util_sequencepattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/util_tfranking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/GLOSSARY.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)    22918 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/SETUP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/conda.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/azureml_designer_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/azureml_designer_modules/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/azure-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/tuning.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.699290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.707291 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/als_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/dkn_MIND.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/fastai_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/geoimc_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/lightgbm_tinycriteo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19501 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/lstur_MIND.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19794 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/naml_MIND.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/ncf_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/npa_MIND.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19584 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/nrms_MIND.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42381 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/rbm_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/rlrmc_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens_with_azureml.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movieratings_with_azureml_designer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33721 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sequential_recsys_amazondataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    70802 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/tfidf_covid.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    86361 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/wide_deep_movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/xdeepfm_criteo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.707291 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/data_split.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    51720 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/data_transform.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/mind_utils.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   724899 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/wikidata_knowledge_graph.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.711290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/als_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/baseline_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   367918 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   379621 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/multi_vae_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   100142 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/rbm_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/sar_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   387601 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/standard_vae_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22587 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.711290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/dkn_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/mmlspark_lightgbm_criteo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54792 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.715290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   177486 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/fm_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   126498 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/lightfm_deep_dive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/ncf_deep_dive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.715290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/als_movielens_diversity_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    60296 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/evaluation.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.715290 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_surprise_svd.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    48854 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_wide_and_deep.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23910 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_ncf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    36598 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_surprise_svd.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   142486 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/tuning_spark_als.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.719291 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/aks_locust_load_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    40995 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/als_movie_o16n.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34217 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/lightgbm_criteo_o16n.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.719291 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17488 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40391 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/movielens.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/run_notebook_on_azureml.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.719291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.723291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/amazon_reviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/cosmos_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/covid_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15476 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/mind.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/movielens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/pandas_df_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/python_splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/spark_splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.723291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55477 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/python_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37392 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/spark_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.723291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.723291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/tuning/parameter_sweep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/notebook_memory_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/ads/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/ads/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/entertainment/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/food_and_restaurants/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/food_and_restaurants/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/news/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/news/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/retail/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/retail/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/travel/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/travel/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.727291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/azure_artifact_feed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/component_governance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/cpu_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/env-setup.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/gpu_unit_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/nightly_cpu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/nightly_gpu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/notebooks_gpu_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/notebooks_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/run_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/submit_azureml_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/smoke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/databricks_install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.731291 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/docker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/generate_conda_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/generate_requirements_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)   335949 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/recsys/zrecs/zprepro_recs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.735291 utilmy-0.1.16802704/utilmy/sspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/README_code.md
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/README_sparksubmit.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.735291 utilmy-0.1.16802704/utilmy/sspark/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/conda/config.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/conda/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.735291 utilmy-0.1.16802704/utilmy/sspark/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config_test_unit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.735291 utilmy-0.1.16802704/utilmy/sspark/config/config_yarn/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config_yarn/config_yarn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    95427 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/config_yarn/config_yarn_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.739291 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/Dockerfile-cluster
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/cluster.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.739291 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/bash
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/build
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/develop
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/compose/down
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/core-site.xml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/hdfs-site.xml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/mapred-site.xml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/ssh_config
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/start-all.sh
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/supervisord.conf
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/yarn-site.xml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.739291 utilmy-0.1.16802704/utilmy/sspark/script/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/script/hadoopVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/script/pysparkTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/script/server_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/script/sparkrunscript.sh
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/spark.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.739291 utilmy-0.1.16802704/utilmy/sspark/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.739291 utilmy-0.1.16802704/utilmy/sspark/src/afpgrowth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/afpgrowth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/afpgrowth/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.743291 utilmy-0.1.16802704/utilmy/sspark/src/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/GetFamiliesFromUserAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/dim_datetime_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.743291 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs_base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/fuzzy_match_udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.743291 utilmy-0.1.16802704/utilmy/sspark/src/functions/spark_udfs/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/functions/spark_udfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.571289 utilmy-0.1.16802704/utilmy/sspark/src/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.743291 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/0.test-pyspark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/1.text-classification-logistic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/10.fashion-mnist-inceptionv1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/2.text-classification-multinomial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/3.topic-modelling-tfidf-lda.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/4.word-vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/7.mnist-sparkflow-feedforward.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/8.mnist-sparkflow-cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/9.mnist-sparkflow-rnn-lstm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/all_book_titles.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/inception_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.747291 utilmy-0.1.16802704/utilmy/sspark/src/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_session_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_url_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_session_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_session_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    98545 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/util_hadoop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/util_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/util_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/util_sparkml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/util_trick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.747291 utilmy-0.1.16802704/utilmy/sspark/src/zvarious/
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/zvarious/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/zvarious/deploying-python-ml-in-pyspark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/src/zvarious/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.747291 utilmy-0.1.16802704/utilmy/sspark/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_session_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_session_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_table_volume_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/sspark/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.747291 utilmy-0.1.16802704/utilmy/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.751291 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    95223 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/bootstrap_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.751291 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    47092 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/tests/test_bootstrap_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.751291 utilmy-0.1.16802704/utilmy/stats/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    52671 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/aov.py
--rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/contingency.py
--rw-r--r--   0 runner    (1001) docker     (123)    51012 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/critical.py
--rw-r--r--   0 runner    (1001) docker     (123)    35359 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/descriptive.py
--rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/fa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/gof.py
--rw-r--r--   0 runner    (1001) docker     (123)    36202 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    83843 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/nonparametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/posthoc.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.755291 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_aov.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_contingency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_critical_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_descriptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_factor_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_gof.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_nonparametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_posthoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/stats/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/tabular/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/bayesian/abtest_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    26925 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/bayesian/model_bayesian_numpyro.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/bayesian/model_bayesian_pyro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/tabular/causal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/causal/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/tabular/causal/rscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/causal/rscripts/run_bnlearn.r
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/causal/util_bnlearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/causal/util_causal.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/tabular/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/sparse/prepro1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57019 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/sparse/prepro_ae_identity.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/sparse/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/sparse/test_model1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/sparse/test_model2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22066 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    55237 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    69006 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_lineartree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tabular/util_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.759291 utilmy-0.1.16802704/utilmy/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.571289 utilmy-0.1.16802704/utilmy/templates/templist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.763291 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/README_code.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.763291 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/config/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/config/config_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.763291 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/util_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/util_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/run_pipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.763291 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/scripts/run_example.sh
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/scripts/run_pipeline.bat
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.767291 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_util_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.767291 utilmy-0.1.16802704/utilmy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.767291 utilmy-0.1.16802704/utilmy/tools/cli_code/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.767291 utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.767291 utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/cli_doc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/cli_doc_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/cli_doc_auto/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_code/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_conda_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_convert_ipynb.py
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_env_autoinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_module_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cli_repo_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.771291 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.771291 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/project_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/project_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/project_graph/project_graph
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/test_script_argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.771291 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/goodnight.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/script_test_case_1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.771291 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/sub_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/sub_dir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/sub_dir/script_test_case_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/test_performance_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.771291 utilmy-0.1.16802704/utilmy/tools/cyberduck/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cyberduck/Google Drive.cyberduckprofile
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/cyberduck/cli_duck.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/globre.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.775291 utilmy-0.1.16802704/utilmy/tools/googledrive_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/googledrive_upload/Steps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/googledrive_upload/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/googledrive_upload/token.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.775291 utilmy-0.1.16802704/utilmy/tools/mybash/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.775291 utilmy-0.1.16802704/utilmy/tools/mybash/bashrc_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/bashrc_template/bashrc_base_1.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/bashrc_template/zshrc_macos.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.775291 utilmy-0.1.16802704/utilmy/tools/mybash/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    45536 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/docs/bash_history
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/docs/bashrc
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/docs/bashrc_base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/docs/homelist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/docs/pylint_jedi.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/init_mybash.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.775291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/__init/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/__init/alias_burak.sh
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/__init/alias_init.sh
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/__init/init_all.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/aws_spotprice
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/source_aws
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale_test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cconda/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cconda/conda_backup_all
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/croncheck
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/cronjob
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/cronjob.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cicd/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cicd/jwms-lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/files
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/findstr
--rwxr-xr-x   0 runner    (1001) docker     (123)     4789 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/folder
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggdrive/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggdrive/wget_googledrive
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.779291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggithub/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggithub/github_cloneall
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggithub/github_getallrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/gitlfs
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/gitpush
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/jupytercmd
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/nnetwork
--rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/nnode
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.787291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/__all.sh
--rw-r--r--   0 runner    (1001) docker     (123)   379670 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/allserver.sh
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/aws_endpoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/buildDocs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/check_iam.sh
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/check_redshift.sh
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/check_s3b.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/common_header.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-allenai-wmt16.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-allenai-wmt19.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-facebook-wmt19.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert_dataset.sh
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/distil_marian_enro_teacher.sh
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/distil_marian_no_teacher.sh
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/docker-entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/download_from_gcp.sh
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/dynamic_bs_example.sh
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/entropy_eval.sh
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/eval_deebert.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/hourly_data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run_ner.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run_pos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/scores_run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/set_env_docker.sh
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/start_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/start_generic_method.sh
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/start_redis_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/tests-to-run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/upload_models.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.787291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ss3/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ss3/dropbox
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ss3/mount_s3drive
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ss3/s3drive_rename
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.787291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/util_date.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/util_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/utils.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.787291 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/homecopy
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/homelist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/homepush
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/util_stable.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/utils.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/utils2.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2416 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/mybash/mybash/zzip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.787291 utilmy-0.1.16802704/utilmy/tools/test/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43077 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/Welcome_To_Colaboratory.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/cli_convert_ipynb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/file0.yml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/file1.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/py36.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/run_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.791291 utilmy-0.1.16802704/utilmy/tools/test/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/test/run_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/test_all.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.791291 utilmy-0.1.16802704/utilmy/tools/test/ztest/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ast_analyzer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/file_finder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.791291 utilmy-0.1.16802704/utilmy/tools/test/ztest/ok/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ok/ztest_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ok/ztest_log_all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/output_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/run_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_runall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tools/util_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.791291 utilmy-0.1.16802704/utilmy/tseries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.791291 utilmy-0.1.16802704/utilmy/tseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/models/model_bayesian_pyro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/models/model_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/prepro_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/torch_lstm (1).py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/torch_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39511 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/torch_outlier.py
--rw-r--r--   0 runner    (1001) docker     (123)    39511 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/torch_outlier_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/tseries/util_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    29159 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_conda.py
--rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/util_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)    43050 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/utilmy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.795292 utilmy-0.1.16802704/utilmy/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/css.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.795292 utilmy-0.1.16802704/utilmy/viz/ddash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.795292 utilmy-0.1.16802704/utilmy/viz/ddash/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.799291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.799291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/page1.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/page2.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/page2_1.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/page2_2.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/html/page2_3.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.799291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/img/
--rw-r--r--   0 runner    (1001) docker     (123)    31482 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/img/jsoneditor-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35432 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/jsoneditor.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   949767 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/jsoneditor.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/mixed_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.799291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/css_base1.css
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/dash_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/html_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/links_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/form_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/form_uploadjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/page1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/page2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/ca_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/chronos_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/framework_batches.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/hdfs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/home.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/main_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/nohit_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/yarn_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/util_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/mmm/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/mmm/contribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/multi-page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/pages/group-level-mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/dash_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.575289 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/ng_word.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/shop_limited_word.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.803291 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/src/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/note.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/ca_targeting_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/chronos_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/hdfs_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/nohit_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/yarn_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/start_app.sh
--rw-r--r--   0 runner    (1001) docker     (123)    25138 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/ddash/readme_help.md
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/model.vec
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/myembed.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/template1.py
--rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/test_vizhtml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    73258 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/testdata/viz_test3_all_graphs.html
--rw-r--r--   0 runner    (1001) docker     (123)    16263 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/util_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/video.py
--rw-r--r--   0 runner    (1001) docker     (123)    77295 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/vizhtml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.807292 utilmy-0.1.16802704/utilmy/viz/zarchive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/zarchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/viz/zarchive/toptoolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.811292 utilmy-0.1.16802704/utilmy/webscraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48265 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/batch_colab_scraper.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_github_gist_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_github_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_leetcode_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_openreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/cli_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/pdf_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/scrape_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.811292 utilmy-0.1.16802704/utilmy/webscraper/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/test/Scraper_INSTAGRAM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/test/scraper_img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/test/url_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/test/vc_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/util_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/webscraper/util_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/z_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zdocstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.815292 utilmy-0.1.16802704/utilmy/zml/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/core_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/core_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/datasketch_hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.815292 utilmy-0.1.16802704/utilmy/zml/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/example/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_adfraud.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_airline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_bankloan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_cardiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_income.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/classifier_mlflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/example/click/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/click/online_shopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/click/outlier_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/click/test_online_shopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/example/regress/
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/regress/regress_airbnb.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/regress/regress_boston.py
--rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/regress/regress_house.py
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/regress/regress_salary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/example/svd/
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/svd/benchmark_mf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/svd/benchmark_mf0.py
--rw-r--r--   0 runner    (1001) docker     (123)    56266 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_keras_vaemdn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_keras_vaemdn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_mkeras.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/test_mkeras_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/titanic_gefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/example/tseries/
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_m5sales.py
--rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_retail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_sales.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/zfraud.py
--rw-r--r--   0 runner    (1001) docker     (123)   389083 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/example/zmodel_new.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.819292 utilmy-0.1.16802704/utilmy/zml/install/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/py36.txt
--rw-r--r--   0 runner    (1001) docker     (123)   159294 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/pygraphviz-1.5-cp36-cp36m-win_amd64.whl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.823292 utilmy-0.1.16802704/utilmy/zml/install/zold/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/conda_list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/pip_deps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/py36_conda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/py36_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/py36b.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/py36c.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/zrequirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/zrequirements_option.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/install/zold/ztodo.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.823292 utilmy-0.1.16802704/utilmy/zml/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.827292 utilmy-0.1.16802704/utilmy/zml/source/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/bin/column_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)   587533 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/bin/feature_engineerng_RL.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.831292 utilmy-0.1.16802704/utilmy/zml/source/models/
--rw-r--r--   0 runner    (1001) docker     (123)    27302 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    38623 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/keras_deepctr.py
--rw-r--r--   0 runner    (1001) docker     (123)    50915 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/keras_widedeep.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/keras_widedeep_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_bayesian_numpyro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_bayesian_pyro.py
--rw-r--r--   0 runner    (1001) docker     (123)    23557 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39538 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_gefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23999 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_numpyro.py
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_outlier.py
--rw-r--r--   0 runner    (1001) docker     (123)    33048 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_vaem.py
--rw-r--r--   0 runner    (1001) docker     (123)    44421 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/model_vaemdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/optuna_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/torch_ease.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/torch_rectorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    51644 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/torch_rvae.py
--rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/torch_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/models/util_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    34413 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/prepro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/prepro_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/prepro_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/prepro_tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_feature_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_inpection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/run_train.py
--rw-r--r--   0 runner    (1001) docker     (123)    22705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    56979 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/util_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.835292 utilmy-0.1.16802704/utilmy/zml/source/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/stopwords_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_autofeature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21545 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    27782 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    40430 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/util_text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/source/utils/ztest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/titanic_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/toutlier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/tsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/tseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/zgitutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zml/ztemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.843292 utilmy-0.1.16802704/utilmy/zzarchive/
--rw-r--r--   0 runner    (1001) docker     (123)    24066 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/_HELP.py
--rw-r--r--   0 runner    (1001) docker     (123)    99167 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/alldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/allmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/allmodule_fin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/coke_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74438 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/datanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/fast_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/function_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/global01.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/kagglegym.py
--rw-r--r--   0 runner    (1001) docker     (123)    81841 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/multiprocessfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)   197340 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)   204262 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/portfolio_withdate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.847292 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/
--rw-r--r--   0 runner    (1001) docker     (123)    24066 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/_HELP.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99167 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/alldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/allmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/allmodule_fin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/coke_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    69794 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/datanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/fast_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/function_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/global01.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/kagglegym.py
--rw-r--r--   0 runner    (1001) docker     (123)    81841 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/multiprocessfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)   197340 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)   204262 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/portfolio_withdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/rstatpy.py
--rw-r--r--   0 runner    (1001) docker     (123)   152781 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util.py.bak
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util_min.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py2to3/utilgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.847292 utilmy-0.1.16802704/utilmy/zzarchive/py3/
--rw-r--r--   0 runner    (1001) docker     (123)   152672 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/py3/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/rstatpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.855292 utilmy-0.1.16802704/utilmy/zzarchive/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.855292 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/codeanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/global01.py
--rw-r--r--   0 runner    (1001) docker     (123)    44699 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.855292 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackagedev/
--rw-r--r--   0 runner    (1001) docker     (123)    25578 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackagedev/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    82945 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/alldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/allmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/benchmarktest.py
--rw-r--r--   0 runner    (1001) docker     (123)    62172 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/codeanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/dbcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/dl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/global01.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/installNewPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/java.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/multiprocessfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/panda_util.py
--rw-r--r--   0 runner    (1001) docker     (123)   154390 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/rec_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/rec_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/sobol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/stateprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/symbolicmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/technical_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/testmulti.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/theano_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22671 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/storage/theano_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)   112493 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   152905 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util.py.bak
--rw-r--r--   0 runner    (1001) docker     (123)    46315 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util_min.py
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/util_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/utilgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.855292 utilmy-0.1.16802704/utilmy/zzarchive/zzarchive/
--rw-r--r--   0 runner    (1001) docker     (123)    98384 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/zzarchive/zutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53361 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzarchive/zzarchive/zutil_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.859292 utilmy-0.1.16802704/utilmy/zzml/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README_HowTo.md
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README_addmodel.md
--rw-r--r--   0 runner    (1001) docker     (123)   188527 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README_research_papers.md
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README_testing.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/README_usage_CLI.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.579289 utilmy-0.1.16802704/utilmy/zzml/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.859292 utilmy-0.1.16802704/utilmy/zzml/docs/DEV_docs/
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/DEV_docs/dataloader.md
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/DEV_docs/json.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.859292 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_addmodel.md
--rw-r--r--   0 runner    (1001) docker     (123)   188527 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_research_papers.md
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_testing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_usage_CLI.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_usage_USECASE.md
--rw-r--r--   0 runner    (1001) docker     (123)    79235 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/deep_learning_models.md
--rw-r--r--   0 runner    (1001) docker     (123)    53059 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/reinforcement_learning_paperes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.863292 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    66081 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_line.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    39787 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_list.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_logs.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/mxnetf.png
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/pytorch.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    22774 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/tenserflow.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    91207 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/test_cli_error.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    34206 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/imgs/test_repo.PNG
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.863292 utilmy-0.1.16802704/utilmy/zzml/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/misc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/misc/details_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/misc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/misc/readdocs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.863292 utilmy-0.1.16802704/utilmy/zzml/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.863292 utilmy-0.1.16802704/utilmy/zzml/install/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/requirements_fake.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/run_doc.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/run_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/run_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/run_install2.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/run_pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.867292 utilmy-0.1.16802704/utilmy/zzml/install/zconda/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/zconda/centos_jupyter_docker
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/zconda/docker2.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/zconda/env_10_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/zconda/zconda_distri_py36tch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/install/zconda/zinstall.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.871292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.871292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/config/cli_test_list.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/config/install_horovod.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24941 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/dataloader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/distri_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/distri_torch_mpirun.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.879292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/README_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/arun_hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/arun_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/benchmark_timeseries_m4.py
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/benchmark_timeseries_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)   129982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/fashion_MNIST_mlmodels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    53700 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl.json
--rw-r--r--   0 runner    (1001) docker     (123)   292253 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl_titanic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras-textcnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.json
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.json
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_home_retail.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic.json
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic_hyper.json
--rw-r--r--   0 runner    (1001) docker     (123)    99230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/mnist_mlmodels_.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/randomforest_titanic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.json
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest_example2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.json
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.json
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow__lstm_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   400203 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/timeseries_m5_deepar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    99230 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vision_mnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vision_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)   129982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vison_fashion_MNIST.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.879292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/fb_prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_automl.json
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_prophet.json
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar.json
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar_dloader.json
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/util_autogluon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.883293 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/Autokeras.json
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/Autokeras.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/armdn.json
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/armdn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn.json
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.json
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/deep_ctr.json
--rw-r--r--   0 runner    (1001) docker     (123)    28714 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/deepctr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.json
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/textcnn.json
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/textcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.887292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/
--rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/matchZoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/textcnn.json
--rw-r--r--   0 runner    (1001) docker     (123)    23581 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/textcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    22075 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/torchhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/torchhub_cnn_dataloader.json
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/transformer_sentence.json
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/transformer_sentence.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/util_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/util_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.887292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/1_lstm.json
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/1_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.887292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/generic_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/tabular_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/template_data_pars.json
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/text_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/text_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42318 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    34572 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/ztemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/00_template_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/model_xxx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/models_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/optim_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/optim_config_prune.json
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/util_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/util_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    97802 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/model_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25761 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/ztest_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/mlmodels/ztest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/utilmy/zzml/pullrequest/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/pullrequest/aa_mycode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/pullrequest/pullrequest.json
--rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68705 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzml/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.891292 utilmy-0.1.16802704/utilmy/zzpiplist/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzpiplist/py36.txt
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-31 13:47:19.000000 utilmy-0.1.16802704/utilmy/zzpiplist/reqs_image.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:47:33.591289 utilmy-0.1.16802704/utilmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    72904 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 13:47:33.000000 utilmy-0.1.16802704/utilmy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-02 04:19:59.000000 utilmy-0.1.16830011/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.084167 utilmy-0.1.16830011/utilmy/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/abash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22843 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/adatasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/aws_spot_price.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/ec2_spot_t3small.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/lambda/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32884 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_autoscale_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_launch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_monitor_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.092167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/main.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.056167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.052167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.092167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demo_qstart/result9.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.092167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/out/task_demoxx1/result2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/mockscript1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/test_util_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/test_functionnal.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/test_unit.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/test_util_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.056167 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/test_aws_lambda_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/00_AWS_BATCH_localpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/01_hyperparams_generator_localpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/05_batch_getresults_from_aws_locapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_a_tasks_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_b_subprocess_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx10/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx10/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx11/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx11/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx12/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx12/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.096166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx13/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx13/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.100166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/params.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/subprocess_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.100166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/params.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/subprocess_pygmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.100166 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/aws_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_local_aws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/util_cpu2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66856 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/z_batch_lambda_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/util_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/cloud/aws/util_aws_daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.100166 utilmy-0.1.16830011/utilmy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/config_val.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.104167 utilmy-0.1.16830011/utilmy/configs/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/config_loguru.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/util_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/logs/util_log_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/pydantic_config_val.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/util_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25795 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/util_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/configs/util_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.104167 utilmy-0.1.16830011/utilmy/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/keyvalue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/kvs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/couch_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30511 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/couch_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/kvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb.go
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/out
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_credis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker_v3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/start_redis_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/util_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/kvs/util_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.108167 utilmy-0.1.16830011/utilmy/db/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/dbvector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/qdrant_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/qdrantinstall.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/startups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/qdrant/triplet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84424 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/db/util_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.112167 utilmy-0.1.16830011/utilmy/deeplearning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.112167 utilmy-0.1.16830011/utilmy/deeplearning/autoencoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/autoencoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/autoencoder/keras_ae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.116166 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/
+-rw-r--r--   0 runner    (1001) docker     (123)   106455 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/VAE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/loss_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/loss_vq_vae2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    88665 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_graph_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93118 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_vqvae_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23984 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_dataloader_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41275 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_dataloader_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23462 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/zkeras_torch_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/kkeras/zz_util_dataloader_img_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.120167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.120167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/i3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/x3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.120167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.124167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/affinity_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/amsoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/conv_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/dual_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/focal_loss_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/frelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/generalized_iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/group_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/info_nce_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/label_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/large_margin_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/lovasz_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/ohem_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/partial_fc_amsoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/pc_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/soft_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/taylor_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93646 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/model_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.128167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30479 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/graphnlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38062 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/rule_encoder4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/sentences_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/torch_lstm_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.128167 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/layer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/model_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/torchinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/util_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52445 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/util_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.132166 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46285 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/model_ensemble_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38058 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/rule_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55129 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64675 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41242 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zrule_encoder2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   233273 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zsentence_tansformer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    70406 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zz_model_ensemble2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.132166 utilmy-0.1.16830011/utilmy/deeplearning/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/tutorial/transf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/tutorial/zz_util_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34126 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31983 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28915 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38131 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/deeplearning/util_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.136166 utilmy-0.1.16830011/utilmy/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56725 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34839 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19475 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/format2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/generate_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/generate_typehint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.136166 utilmy-0.1.16830011/utilmy/docs/test_script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.136166 utilmy-0.1.16830011/utilmy/docs/test_script/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.136166 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_normalize_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_normalize_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/test_script/test_script_normalize_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/util_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/util_template2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/zold_cli_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/zold_docstring2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/docs/zold_docstring3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.140167 utilmy-0.1.16830011/utilmy/excel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/excel/xl_pytthon.xlsm
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/excel/xlvba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.140167 utilmy-0.1.16830011/utilmy/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/graph/util_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/iio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.140167 utilmy-0.1.16830011/utilmy/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/images/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39561 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/images/util_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.144167 utilmy-0.1.16830011/utilmy/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.144167 utilmy-0.1.16830011/utilmy/nlp/kkeras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/kkeras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/kkeras/sentences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ner_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.144167 utilmy-0.1.16830011/utilmy/nlp/ttorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.144167 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/kgDriverCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/knowledge_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.144167 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/kgDriverCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/knowledge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/mytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/pykeenTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38692 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/model_patent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31070 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/ttorch/sentences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_cocount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_gensim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59668 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/util_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nlp/zzz_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/nnumpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/oos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.148167 utilmy-0.1.16830011/utilmy/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/expression_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/gp_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89758 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/gp_searchformulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/res_ranking.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/util_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/util_optim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.148167 utilmy-0.1.16830011/utilmy/optim/zold/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/gp_dcgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/gp_dcgp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/gp_formulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40314 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/optim/zold/gp_searchformulae_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37954 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30398 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/ppandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/ppolars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.148167 utilmy-0.1.16830011/utilmy/prepro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/prepro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/prepro_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/prepro_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/prepro_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/run_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60684 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/prepro/util_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.152166 utilmy-0.1.16830011/utilmy/recsys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36899 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.152166 utilmy-0.1.16830011/utilmy/recsys/bandits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/aabandit_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/DOCS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    29619 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/data_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/data_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/embed_dnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/preprocessing/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/serving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/serving/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.156167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/training/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/model_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/model_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/configs/example_feature_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/configs/example_ml_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/scripts/create_bq_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/scripts/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/scripts/schemas/training_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/serving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24906 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/serving/test_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/training/test_train_bandit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.160167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/1 - Evaluating a new fraud policy with IPS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/2 - Evaluating a new fraud policy with the direct method.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/3 - Evaluating a new fraud policy with the doubly robust method.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/gbdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/direct_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/doubly_robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/inverse_propensity_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/training/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.164167 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/epsilon_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/exp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/create_movielens_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/eda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/visualize_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/ucb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.060166 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/data/ml-20m/
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/data/ml-20m/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/contrib/placeholder
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.168166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/usage/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   109315 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/Bandit_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/DQN_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/deep_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/genetic_rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/genetic_rl_q_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.060166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/known_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/known_parameters/placeholder
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/
+-rw-r--r--   0 runner    (1001) docker     (123)    86016 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/A2C-CartPole-v0-ep100.db
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/a2c_cartpole-v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/td3_pendulum-v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/run_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.172166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/bootstrap_neural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/linpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_linpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_noise_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bernoulli_mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/epsgreedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gaussian_mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/ucb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/qlearning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/sarsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/valueiteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.176167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/offpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/onpolicy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/ddpg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/dueling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/noisy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/prioritized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/ppo1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/sac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/vpg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.180167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/rollout_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.184167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/action_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/atari_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/gym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.184167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/vector_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.184167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/genetic_hyperparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.184167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/classical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/offpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/onpolicy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/adult_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/census_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/covertype_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/magic_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/mushroom_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/statlog_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_cb_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_data_bandits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_mab_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_multi_armed_bandits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.188166 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/test_agents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_a2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ppo1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_vpg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_atari_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_vecenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_bandit_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_classical_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_deep_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26664 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/offline_replayer_eval_amzon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/bandits/recostep_offline_replayer_eval_movielens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29315 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/metrics/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/metrics/distance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.192167 utilmy-0.1.16830011/utilmy/recsys/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.196167 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessAmazonSportsOutdoors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessAmazonVideoGames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessML20M.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessMSD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessNetflix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessYahooMovies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/TrainModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23417 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/CEASE/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.196167 utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/DynEASEr_Runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/ease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/prepro1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57019 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/prepro_ae_identity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/prod2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.196167 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/online_logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.196167 utilmy-0.1.16830011/utilmy/recsys/ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/optim_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/rank_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/rank_fusion_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/util_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/ranking/util_rankmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/util_ltr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/util_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/util_sequencepattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/util_tfranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/GLOSSARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22918 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/SETUP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/conda.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/azureml_designer_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/azureml_designer_modules/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/azure-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.200167 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.204167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.204167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/als_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/dkn_MIND.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/fastai_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/geoimc_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/lightgbm_tinycriteo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19501 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/lstur_MIND.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19794 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/naml_MIND.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/ncf_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/npa_MIND.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19584 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/nrms_MIND.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42381 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/rbm_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/rlrmc_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens_with_azureml.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movieratings_with_azureml_designer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33721 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sequential_recsys_amazondataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    70802 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/tfidf_covid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    86361 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/wide_deep_movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/xdeepfm_criteo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.208166 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/data_split.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    51720 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/data_transform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/mind_utils.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   724899 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/wikidata_knowledge_graph.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.212167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/als_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/baseline_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   367918 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   379621 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/multi_vae_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   100142 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/rbm_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/sar_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   387601 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/standard_vae_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22587 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.212167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/dkn_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/mmlspark_lightgbm_criteo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54792 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.212167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   177486 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/fm_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   126498 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/lightfm_deep_dive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/ncf_deep_dive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.216167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/als_movielens_diversity_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60296 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/evaluation.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.216167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_surprise_svd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    48854 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_wide_and_deep.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23910 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_ncf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36598 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_surprise_svd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   142486 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/tuning_spark_als.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.216167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/aks_locust_load_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    40995 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/als_movie_o16n.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34217 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/lightgbm_criteo_o16n.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.216167 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17488 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40391 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/movielens.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/run_notebook_on_azureml.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.220167 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.220167 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/amazon_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/cosmos_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/covid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/mind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/movielens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/pandas_df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/python_splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/spark_splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.220167 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55477 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/python_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37392 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/spark_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/tuning/parameter_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/notebook_memory_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/ads/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/ads/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/entertainment/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/food_and_restaurants/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/food_and_restaurants/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.224166 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/news/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/news/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.228167 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/retail/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/retail/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.228167 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/travel/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/travel/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.228167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.228167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/azure_artifact_feed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/component_governance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/cpu_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/env-setup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/gpu_unit_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/nightly_cpu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/nightly_gpu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/notebooks_gpu_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/notebooks_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/run_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/submit_azureml_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.228167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.232167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/smoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.232167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.232167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/databricks_install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.232167 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/generate_conda_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/generate_requirements_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   335949 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/recsys/zrecs/zprepro_recs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.236167 utilmy-0.1.16830011/utilmy/sspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/README_code.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/README_sparksubmit.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.236167 utilmy-0.1.16830011/utilmy/sspark/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/conda/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/conda/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.236167 utilmy-0.1.16830011/utilmy/sspark/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config_test_unit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.236167 utilmy-0.1.16830011/utilmy/sspark/config/config_yarn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config_yarn/config_yarn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    95427 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/config_yarn/config_yarn_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.240167 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/Dockerfile-cluster
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/cluster.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.240167 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/bash
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/build
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/develop
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/compose/down
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/core-site.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/hdfs-site.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/mapred-site.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/ssh_config
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/start-all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/supervisord.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/yarn-site.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.240167 utilmy-0.1.16830011/utilmy/sspark/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/script/hadoopVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/script/pysparkTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/script/server_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/script/sparkrunscript.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/spark.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.244166 utilmy-0.1.16830011/utilmy/sspark/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.244166 utilmy-0.1.16830011/utilmy/sspark/src/afpgrowth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/afpgrowth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/afpgrowth/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.244166 utilmy-0.1.16830011/utilmy/sspark/src/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/GetFamiliesFromUserAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/dim_datetime_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.244166 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs_base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/fuzzy_match_udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.244166 utilmy-0.1.16830011/utilmy/sspark/src/functions/spark_udfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/functions/spark_udfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.068167 utilmy-0.1.16830011/utilmy/sspark/src/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.248167 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/0.test-pyspark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/1.text-classification-logistic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/10.fashion-mnist-inceptionv1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/2.text-classification-multinomial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/3.topic-modelling-tfidf-lda.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/4.word-vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/7.mnist-sparkflow-feedforward.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/8.mnist-sparkflow-cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/9.mnist-sparkflow-rnn-lstm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/all_book_titles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/inception_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.248167 utilmy-0.1.16830011/utilmy/sspark/src/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_session_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_url_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_session_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_session_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98545 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/util_hadoop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/util_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42292 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/util_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/util_sparkml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/util_trick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.248167 utilmy-0.1.16830011/utilmy/sspark/src/zvarious/
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/zvarious/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/zvarious/deploying-python-ml-in-pyspark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/src/zvarious/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.252167 utilmy-0.1.16830011/utilmy/sspark/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_session_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_session_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_table_volume_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/sspark/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.252167 utilmy-0.1.16830011/utilmy/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.252167 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    95223 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/bootstrap_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.252167 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47092 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/tests/test_bootstrap_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.256167 utilmy-0.1.16830011/utilmy/stats/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52671 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/aov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34099 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/contingency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51012 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/critical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35359 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/descriptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/fa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/gof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36202 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83843 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/nonparametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/posthoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.260167 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_aov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_contingency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_critical_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_descriptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_factor_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_gof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_nonparametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_posthoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/stats/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.264167 utilmy-0.1.16830011/utilmy/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.264167 utilmy-0.1.16830011/utilmy/tabular/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/bayesian/abtest_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26925 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/bayesian/model_bayesian_numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/bayesian/model_bayesian_pyro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.264167 utilmy-0.1.16830011/utilmy/tabular/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/causal/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.264167 utilmy-0.1.16830011/utilmy/tabular/causal/rscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/causal/rscripts/run_bnlearn.r
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/causal/util_bnlearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/causal/util_causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.264167 utilmy-0.1.16830011/utilmy/tabular/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/sparse/prepro1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57019 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/sparse/prepro_ae_identity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/sparse/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/sparse/test_model1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/sparse/test_model2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22066 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55237 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69006 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_lineartree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tabular/util_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.268167 utilmy-0.1.16830011/utilmy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.068167 utilmy-0.1.16830011/utilmy/templates/templist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.268167 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/README_code.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.268167 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/config/config_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.272167 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/util_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/util_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/run_pipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.272167 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/scripts/run_example.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/scripts/run_pipeline.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.272167 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_util_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.276167 utilmy-0.1.16830011/utilmy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.276167 utilmy-0.1.16830011/utilmy/tools/cli_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.276167 utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.276167 utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/cli_doc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/cli_doc_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/cli_doc_auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_code/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_conda_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_convert_ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_env_autoinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cli_repo_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/project_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/project_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/project_graph/project_graph
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/test_script_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/goodnight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/script_test_case_1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/sub_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/sub_dir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/sub_dir/script_test_case_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/test_performance_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/cyberduck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cyberduck/Google Drive.cyberduckprofile
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/cyberduck/cli_duck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/globre.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/googledrive_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/googledrive_upload/Steps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/googledrive_upload/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/googledrive_upload/token.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/mybash/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.280166 utilmy-0.1.16830011/utilmy/tools/mybash/bashrc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/bashrc_template/bashrc_base_1.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/bashrc_template/zshrc_macos.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.284167 utilmy-0.1.16830011/utilmy/tools/mybash/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    45536 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/docs/bash_history
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/docs/bashrc
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/docs/bashrc_base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/docs/homelist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/docs/pylint_jedi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/init_mybash.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.284167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.284167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/__init/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/__init/alias_burak.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/__init/alias_init.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/__init/init_all.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.284167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/aws_spotprice
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/source_aws
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale_test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.288167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cconda/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cconda/conda_backup_all
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.288167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/croncheck
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/cronjob
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/cronjob.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.288167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cicd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cicd/jwms-lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/files
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/findstr
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4789 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/folder
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.288167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggdrive/wget_googledrive
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.288167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggithub/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggithub/github_cloneall
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggithub/github_getallrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/gitlfs
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/gitpush
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/jupytercmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/nnetwork
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/nnode
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.296167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/__all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   379670 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/allserver.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/aws_endpoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/buildDocs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/check_iam.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/check_redshift.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/check_s3b.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/common_header.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-allenai-wmt16.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-allenai-wmt19.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-facebook-wmt19.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert_dataset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/distil_marian_enro_teacher.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/distil_marian_no_teacher.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/docker-entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/download_from_gcp.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/dynamic_bs_example.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/entropy_eval.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/eval_deebert.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/hourly_data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run_ner.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run_pos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/scores_run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/set_env_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/start_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/start_generic_method.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/start_redis_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/tests-to-run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/upload_models.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.296167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ss3/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ss3/dropbox
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ss3/mount_s3drive
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ss3/s3drive_rename
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.296167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/util_date.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/util_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/utils.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.296167 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/homecopy
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/homelist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/homepush
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/util_stable.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/utils.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/utils2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2416 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/mybash/mybash/zzip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.300167 utilmy-0.1.16830011/utilmy/tools/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43077 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/Welcome_To_Colaboratory.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/cli_convert_ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/file0.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/file1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/py36.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/run_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.300167 utilmy-0.1.16830011/utilmy/tools/test/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/test/run_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/test_all.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.300167 utilmy-0.1.16830011/utilmy/tools/test/ztest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ast_analyzer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/file_finder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.300167 utilmy-0.1.16830011/utilmy/tools/test/ztest/ok/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ok/ztest_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ok/ztest_log_all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/output_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/run_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_runall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tools/util_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.304167 utilmy-0.1.16830011/utilmy/tseries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.304167 utilmy-0.1.16830011/utilmy/tseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/models/model_bayesian_pyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/models/model_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/prepro_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/torch_lstm (1).py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/torch_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39511 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/torch_outlier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39511 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/torch_outlier_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/tseries/util_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29159 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/util_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43707 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/utilmy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.304167 utilmy-0.1.16830011/utilmy/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/css.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.304167 utilmy-0.1.16830011/utilmy/viz/ddash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.308167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.308167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.308167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/page1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/page2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/page2_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/page2_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/html/page2_3.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.308167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    31482 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/img/jsoneditor-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35432 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/jsoneditor.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   949767 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/jsoneditor.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/mixed_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.308167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/css_base1.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/dash_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/html_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/links_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/form_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/form_uploadjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/page1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/page2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/ca_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/chronos_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/framework_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/hdfs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/main_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/nohit_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/yarn_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/util_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/mmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/mmm/contribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/multi-page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/pages/group-level-mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/dash_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.076166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.312167 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/ng_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/shop_limited_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/src/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.316166 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/layout/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/note.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.320167 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/ca_targeting_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/chronos_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/hdfs_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/nohit_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/yarn_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/start_app.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    25138 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/ddash/readme_help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/model.vec
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/myembed.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/template1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/test_vizhtml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.320167 utilmy-0.1.16830011/utilmy/viz/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    73258 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/testdata/viz_test3_all_graphs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16263 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/util_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77295 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/vizhtml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.320167 utilmy-0.1.16830011/utilmy/viz/zarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/zarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/viz/zarchive/toptoolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.320167 utilmy-0.1.16830011/utilmy/webscraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48265 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/batch_colab_scraper.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_github_gist_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_github_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_leetcode_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_openreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/cli_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/pdf_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/scrape_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.324167 utilmy-0.1.16830011/utilmy/webscraper/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/test/Scraper_INSTAGRAM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/test/scraper_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/test/url_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/test/vc_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/util_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/webscraper/util_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/z_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zdocstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.324167 utilmy-0.1.16830011/utilmy/zml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/core_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/core_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/datasketch_hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.328167 utilmy-0.1.16830011/utilmy/zml/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.328167 utilmy-0.1.16830011/utilmy/zml/example/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_adfraud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_airline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_bankloan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_cardiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/classifier_mlflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.332167 utilmy-0.1.16830011/utilmy/zml/example/click/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/click/online_shopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/click/outlier_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/click/test_online_shopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.332167 utilmy-0.1.16830011/utilmy/zml/example/regress/
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/regress/regress_airbnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/regress/regress_boston.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/regress/regress_house.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/regress/regress_salary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.332167 utilmy-0.1.16830011/utilmy/zml/example/svd/
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/svd/benchmark_mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/svd/benchmark_mf0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56266 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_keras_vaemdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_keras_vaemdn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_mkeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/test_mkeras_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/titanic_gefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.332167 utilmy-0.1.16830011/utilmy/zml/example/tseries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_m5sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_retail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/zfraud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   389083 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/example/zmodel_new.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.332167 utilmy-0.1.16830011/utilmy/zml/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/py36.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   159294 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/pygraphviz-1.5-cp36-cp36m-win_amd64.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.336167 utilmy-0.1.16830011/utilmy/zml/install/zold/
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/conda_list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/pip_deps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/py36_conda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/py36_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/py36b.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/py36c.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/zrequirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/zrequirements_option.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/install/zold/ztodo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.336167 utilmy-0.1.16830011/utilmy/zml/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.340167 utilmy-0.1.16830011/utilmy/zml/source/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/bin/column_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)   587533 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/bin/feature_engineerng_RL.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.344167 utilmy-0.1.16830011/utilmy/zml/source/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    27302 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38623 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/keras_deepctr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50915 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/keras_widedeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/keras_widedeep_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_bayesian_numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_bayesian_pyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23557 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39538 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_gefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23999 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_outlier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33048 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_vaem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44421 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/model_vaemdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/optuna_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/torch_ease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/torch_rectorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51644 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/torch_rvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/torch_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/models/util_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34413 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/prepro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/prepro_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/prepro_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/prepro_tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_feature_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_inpection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/run_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22705 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56979 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/util_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.348167 utilmy-0.1.16830011/utilmy/zml/source/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/stopwords_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_autofeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21545 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27782 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40430 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/util_text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/source/utils/ztest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/titanic_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/toutlier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/tsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/tseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/zgitutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zml/ztemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.356167 utilmy-0.1.16830011/utilmy/zzarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)    24066 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/_HELP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99167 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/alldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/allmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/allmodule_fin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/coke_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74438 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/datanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/fast_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/function_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/global01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/kagglegym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81841 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/multiprocessfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197340 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204262 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/portfolio_withdate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.360167 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)    24066 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/_HELP.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99167 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/alldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/allmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/allmodule_fin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/coke_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69794 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/datanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/fast_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/function_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/global01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/kagglegym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81841 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/multiprocessfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197340 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204262 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/portfolio_withdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/rstatpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152781 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util.py.bak
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py2to3/utilgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.360167 utilmy-0.1.16830011/utilmy/zzarchive/py3/
+-rw-r--r--   0 runner    (1001) docker     (123)   152672 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/py3/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/rstatpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.364167 utilmy-0.1.16830011/utilmy/zzarchive/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.368167 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/codeanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/global01.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44699 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.368167 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackagedev/
+-rw-r--r--   0 runner    (1001) docker     (123)    25578 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackagedev/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82945 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/alldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/allmodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/benchmarktest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62172 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/codeanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/dbcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/dl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/global01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/installNewPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/multiprocessfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/panda_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154390 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/rec_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/rec_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/sobol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/stateprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/symbolicmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/technical_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/testmulti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/theano_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22671 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/storage/theano_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112493 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152905 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util.py.bak
+-rw-r--r--   0 runner    (1001) docker     (123)    46315 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/util_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/utilgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.368167 utilmy-0.1.16830011/utilmy/zzarchive/zzarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)    98384 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/zzarchive/zutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53361 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzarchive/zzarchive/zutil_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.368167 utilmy-0.1.16830011/utilmy/zzml/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README_HowTo.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README_addmodel.md
+-rw-r--r--   0 runner    (1001) docker     (123)   188527 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README_research_papers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README_testing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/README_usage_CLI.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.076166 utilmy-0.1.16830011/utilmy/zzml/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.368167 utilmy-0.1.16830011/utilmy/zzml/docs/DEV_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/DEV_docs/dataloader.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/DEV_docs/json.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.372167 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_addmodel.md
+-rw-r--r--   0 runner    (1001) docker     (123)   188527 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_research_papers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_testing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_usage_CLI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_usage_USECASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    79235 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/deep_learning_models.md
+-rw-r--r--   0 runner    (1001) docker     (123)    53059 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/reinforcement_learning_paperes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.372167 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    66081 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_line.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    39787 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_list.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    30941 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_logs.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/mxnetf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/pytorch.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    22774 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/tenserflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    91207 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/test_cli_error.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    34206 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/imgs/test_repo.PNG
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.372167 utilmy-0.1.16830011/utilmy/zzml/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/misc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/misc/details_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/misc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/misc/readdocs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.372167 utilmy-0.1.16830011/utilmy/zzml/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.376167 utilmy-0.1.16830011/utilmy/zzml/install/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/requirements_fake.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/run_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/run_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/run_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/run_install2.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/run_pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.376167 utilmy-0.1.16830011/utilmy/zzml/install/zconda/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/zconda/centos_jupyter_docker
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/zconda/docker2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/zconda/env_10_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/zconda/zconda_distri_py36tch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/install/zconda/zinstall.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.380167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.380167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/config/cli_test_list.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/config/install_horovod.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24941 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/dataloader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/distri_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/distri_torch_mpirun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.388167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/README_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/arun_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/arun_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/benchmark_timeseries_m4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/benchmark_timeseries_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129982 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/fashion_MNIST_mlmodels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    53700 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl.json
+-rw-r--r--   0 runner    (1001) docker     (123)   292253 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl_titanic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras-textcnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_home_retail.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic_hyper.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/mnist_mlmodels_.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/randomforest_titanic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest_example2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow__lstm_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   400203 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/timeseries_m5_deepar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    99230 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vision_mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vision_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129982 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vison_fashion_MNIST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.388167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/fb_prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_automl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_prophet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar_dloader.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/util_autogluon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.392167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/Autokeras.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/Autokeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/armdn.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/armdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/deep_ctr.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28714 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/deepctr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/textcnn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-02 04:19:47.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/textcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.392167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/
+-rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/matchZoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/textcnn.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23581 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/textcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22075 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/torchhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/torchhub_cnn_dataloader.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/transformer_sentence.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/transformer_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/util_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/util_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.392167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/1_lstm.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/1_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.396167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/generic_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/tabular_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/template_data_pars.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/text_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/text_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42318 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34572 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/ztemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.396167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/00_template_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/model_xxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/models_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/optim_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/optim_config_prune.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/util_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/util_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    97802 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25761 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/ztest_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/mlmodels/ztest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/utilmy/zzml/pullrequest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/pullrequest/aa_mycode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/pullrequest/pullrequest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68705 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzml/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.400167 utilmy-0.1.16830011/utilmy/zzpiplist/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzpiplist/py36.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 04:19:48.000000 utilmy-0.1.16830011/utilmy/zzpiplist/reqs_image.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:20:02.088167 utilmy-0.1.16830011/utilmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 04:20:01.000000 utilmy-0.1.16830011/utilmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    72904 2023-05-02 04:20:02.000000 utilmy-0.1.16830011/utilmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:20:01.000000 utilmy-0.1.16830011/utilmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 04:20:01.000000 utilmy-0.1.16830011/utilmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 04:20:01.000000 utilmy-0.1.16830011/utilmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 04:20:01.000000 utilmy-0.1.16830011/utilmy.egg-info/top_level.txt
```

### Comparing `utilmy-0.1.16802704/PKG-INFO` & `utilmy-0.1.16830011/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilmy
-Version: 0.1.16802704
+Version: 0.1.16830011
 Summary: utils
 Author: Nono
 Keywords: utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -35,11 +35,11 @@
 
    https://groups.google.com/g/utilmy
 
 
 
 
 Hash:
-18e1c29368c22c166691762ccb195e5b88ee2378
+623885c267bb56b48921abbba325f4bb4a9cb13f
 
 
 ```
```

### Comparing `utilmy-0.1.16802704/README.md` & `utilmy-0.1.16830011/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/setup.py` & `utilmy-0.1.16830011/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ######################################################################################
 root = os.path.abspath(os.path.dirname(__file__))
 
 
 
 ##### Version  #######################################################################
-version ='0.1.16802704'
+version ='0.1.16830011'
 cmdclass= None
 print("version", version)
 
 
 
 ##### Requirements ###################################################################
 #with open('install/reqs_image.cmd') as fp:
```

### Comparing `utilmy-0.1.16802704/utilmy/__init__.py` & `utilmy-0.1.16830011/utilmy/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/abash.py` & `utilmy-0.1.16830011/utilmy/abash.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/adatasets.py` & `utilmy-0.1.16830011/utilmy/adatasets.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cli.py` & `utilmy-0.1.16830011/utilmy/cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/aws_spot_price.sh` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/aws_spot_price.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/aws/ec2_spot_t3small.json` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/aws/ec2_spot_t3small.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_autoscale_cli.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_autoscale_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_launch_cli.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_launch_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/batch_daemon_monitor_cli.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/batch_daemon_monitor_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/cli.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/config.toml` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/config.toml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/main.sh` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/main.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/main_run.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/main_run.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/task_template/task_config.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/task_template/task_config.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/test_util_batch.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/functional/test_util_batch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/test_unit.sh` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/test_unit.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/pytest/test_util_log.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/pytest/test_util_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/test_aws_lambda_run.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_lambda/test_aws_lambda_run.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/00_AWS_BATCH_localpc.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/00_AWS_BATCH_localpc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/01_hyperparams_generator_localpc.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/01_hyperparams_generator_localpc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/05_batch_getresults_from_aws_locapc.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/05_batch_getresults_from_aws_locapc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_a_tasks_launch.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_a_tasks_launch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_b_subprocess_launch.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/batch_b_subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_optim.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_optim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_script.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_aws_template/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/main.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/subprocess_optim.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/subprocess_optim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/utils.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx1_qstart/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/main.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/subprocess_pygmo.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/subprocess_pygmo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/utils.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/tasks/task_demoxx2_qstart/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/aws_methods.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/aws_methods.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_local_aws_cli.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_local_aws_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_sequencer.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/batch_sequencer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_main.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_subprocess.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/template_subprocess.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/test/zarchive/util_cpu2.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/test/zarchive/util_cpu2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_aws.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_aws.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_batch.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_batch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_cpu.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_cpu.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/autoscale_aws/util_log.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/autoscale_aws/util_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/util_aws.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/util_aws.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/cloud/aws/util_aws_daemon.py` & `utilmy-0.1.16830011/utilmy/cloud/aws/util_aws_daemon.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/logs/config_loguru.yaml` & `utilmy-0.1.16830011/utilmy/configs/logs/config_loguru.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/logs/test_log.py` & `utilmy-0.1.16830011/utilmy/configs/logs/test_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/logs/util_log.py` & `utilmy-0.1.16830011/utilmy/configs/logs/util_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/logs/util_log_std.py` & `utilmy-0.1.16830011/utilmy/configs/logs/util_log_std.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/pydantic_config_val.yaml` & `utilmy-0.1.16830011/utilmy/configs/pydantic_config_val.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/test.py` & `utilmy-0.1.16830011/utilmy/configs/test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/util_config.py` & `utilmy-0.1.16830011/utilmy/configs/util_config.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/util_dirs.py` & `utilmy-0.1.16830011/utilmy/configs/util_dirs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/configs/util_log.py` & `utilmy-0.1.16830011/utilmy/configs/util_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/data.py` & `utilmy-0.1.16830011/utilmy/data.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/dates.py` & `utilmy-0.1.16830011/utilmy/dates.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/keyvalue.py` & `utilmy-0.1.16830011/utilmy/db/keyvalue.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/couch_conn.py` & `utilmy-0.1.16830011/utilmy/db/kvs/couch_conn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/couch_queries.py` & `utilmy-0.1.16830011/utilmy/db/kvs/couch_queries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/docker-compose.yml` & `utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/go.sum` & `utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/go.sum`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb.go` & `utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb.go`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb_test.go` & `utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/kvdb/kvdb_test.go`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/kvs_bench_go/readme.md` & `utilmy-0.1.16830011/utilmy/db/kvs/kvs_bench_go/readme.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_credis.py` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_credis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_hiredis.py` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_hiredis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_bench_python/tests/test_redis.py` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_bench_python/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker.yml` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker_macos.yml` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker_macos.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/redis_cluster_docker_v3.yml` & `utilmy-0.1.16830011/utilmy/db/kvs/redis_cluster_docker_v3.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/util_cassandra.py` & `utilmy-0.1.16830011/utilmy/db/kvs/util_cassandra.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/kvs/util_redis.py` & `utilmy-0.1.16830011/utilmy/db/kvs/util_redis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/qdrant/dbvector.py` & `utilmy-0.1.16830011/utilmy/db/qdrant/dbvector.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/qdrant/qdrant_example.py` & `utilmy-0.1.16830011/utilmy/db/qdrant/qdrant_example.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/qdrant/startups.json` & `utilmy-0.1.16830011/utilmy/db/qdrant/startups.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/qdrant/test.py` & `utilmy-0.1.16830011/utilmy/db/qdrant/test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/qdrant/triplet.py` & `utilmy-0.1.16830011/utilmy/db/qdrant/triplet.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/db/util_sql.py` & `utilmy-0.1.16830011/utilmy/db/util_sql.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/debug.py` & `utilmy-0.1.16830011/utilmy/debug.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/decorators.py` & `utilmy-0.1.16830011/utilmy/decorators.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/VAE.ipynb` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/VAE.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/loss_graph.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/loss_graph.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/loss_vq_vae2.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/loss_vq_vae2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_graph_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_graph_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_template.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_template.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/train_vqvae_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/train_vqvae_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_dataloader_img.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_dataloader_img.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_dataloader_tab.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_dataloader_tab.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_debug.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_debug.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_layers.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_layers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_models.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_similarity.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_similarity.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/util_train.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/util_train.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/zkeras_torch_sentence.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/zkeras_torch_sentence.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/kkeras/zz_util_dataloader_img_old.py` & `utilmy-0.1.16830011/utilmy/deeplearning/kkeras/zz_util_dataloader_img_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/test.py` & `utilmy-0.1.16830011/utilmy/deeplearning/test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/__init__.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/base.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/i3d.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/i3d.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/images/x3d.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/images/x3d.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/layers/__init__.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/README.md` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/__init__.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/affinity_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/affinity_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/amsoftmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/amsoftmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/conv_ops.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/conv_ops.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/dice_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/dual_focal_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/dual_focal_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/ema.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/ema.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/focal_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/focal_loss_old.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/focal_loss_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/frelu.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/frelu.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/generalized_iou_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/generalized_iou_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/group_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/group_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/hswish.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/hswish.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/info_nce_dist.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/info_nce_dist.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/label_smooth.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/label_smooth.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/large_margin_softmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/large_margin_softmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/layer_norm.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/layer_norm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/lovasz_softmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/lovasz_softmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/mish.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/mish.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/ohem_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/ohem_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/one_hot.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/one_hot.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/partial_fc_amsoftmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/partial_fc_amsoftmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/pc_softmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/pc_softmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/soft_dice_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/soft_dice_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/swish.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/swish.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/taylor_softmax.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/taylor_softmax.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/test.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/losses/triplet_loss.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/model_ensemble.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/model_ensemble.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/graphnlp.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/graphnlp.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/rule_encoder4.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/rule_encoder4.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/sentences_model.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/sentences_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/models/torch_lstm_check.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/models/torch_lstm_check.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/README.md` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/enums.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/enums.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/formatting.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/formatting.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/layer_info.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/layer_info.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/model_statistics.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/model_statistics.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/torchinfo/torchinfo.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/torchinfo/torchinfo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/util_model.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/util_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/util_torch.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/util_torch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/model_ensemble_detail.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/model_ensemble_detail.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/rule_encoder.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/rule_encoder.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble2.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble4.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble4.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble_old.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zmodel_ensemble_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zrule_encoder2.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zrule_encoder2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zsentence_tansformer.ipynb` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zsentence_tansformer.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/ttorch/zsave/zz_model_ensemble2.py` & `utilmy-0.1.16830011/utilmy/deeplearning/ttorch/zsave/zz_model_ensemble2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/tutorial/transf.py` & `utilmy-0.1.16830011/utilmy/deeplearning/tutorial/transf.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/tutorial/zz_util_topk.py` & `utilmy-0.1.16830011/utilmy/deeplearning/tutorial/zz_util_topk.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_dl.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_dl.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_embedding.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_embedding.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_hash.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_hash.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_hyper.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_hyper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_onnx.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_onnx.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_topk.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_topk.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/deeplearning/util_yolo.py` & `utilmy-0.1.16830011/utilmy/deeplearning/util_yolo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/distributed.py` & `utilmy-0.1.16830011/utilmy/distributed.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/README.md` & `utilmy-0.1.16830011/utilmy/docs/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/cli.py` & `utilmy-0.1.16830011/utilmy/docs/cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/code_parser.py` & `utilmy-0.1.16830011/utilmy/docs/code_parser.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/docstring.py` & `utilmy-0.1.16830011/utilmy/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/format.py` & `utilmy-0.1.16830011/utilmy/docs/format.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/format2.py` & `utilmy-0.1.16830011/utilmy/docs/format2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/generate_doc.py` & `utilmy-0.1.16830011/utilmy/docs/generate_doc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/generate_typehint.py` & `utilmy-0.1.16830011/utilmy/docs/generate_typehint.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_core.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_core.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_header.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_header.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_no_logger.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_no_logger.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script/test_script_normalize_import.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script/test_script_normalize_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_core.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_core.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_header.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_header.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_no_logger.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_no_logger.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/output/test_script_normalize_import.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/output/test_script_normalize_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_core.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_core.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_header.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_header.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_help.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_help.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/test_script_no_logger.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/test_script_no_logger.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/test_script/test_script_normalize_import.py` & `utilmy-0.1.16830011/utilmy/docs/test_script/test_script_normalize_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/util_template.py` & `utilmy-0.1.16830011/utilmy/docs/util_template.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/util_template2.py` & `utilmy-0.1.16830011/utilmy/docs/util_template2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/zold_cli_format.py` & `utilmy-0.1.16830011/utilmy/docs/zold_cli_format.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/zold_docstring2.py` & `utilmy-0.1.16830011/utilmy/docs/zold_docstring2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/docs/zold_docstring3.py` & `utilmy-0.1.16830011/utilmy/docs/zold_docstring3.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/excel/xl_pytthon.xlsm` & `utilmy-0.1.16830011/utilmy/excel/xl_pytthon.xlsm`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/excel/xlvba.py` & `utilmy-0.1.16830011/utilmy/excel/xlvba.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/graph/__init__.py` & `utilmy-0.1.16830011/utilmy/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/graph/util_graph.py` & `utilmy-0.1.16830011/utilmy/graph/util_graph.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/iio.py` & `utilmy-0.1.16830011/utilmy/iio.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/images/util_image.py` & `utilmy-0.1.16830011/utilmy/images/util_image.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/kkeras/sentences.py` & `utilmy-0.1.16830011/utilmy/nlp/kkeras/sentences.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ner_extractor.py` & `utilmy-0.1.16830011/utilmy/nlp/ner_extractor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/kgDriverCode.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/kgDriverCode.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/knowledge_graph.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/knowledge_graph.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/kgraph/misc/pykeenTest.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/kgraph/misc/pykeenTest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/model_patent.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/model_patent.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/ttorch/sentences.py` & `utilmy-0.1.16830011/utilmy/nlp/ttorch/sentences.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_cluster.py` & `utilmy-0.1.16830011/utilmy/nlp/util_cluster.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_cocount.py` & `utilmy-0.1.16830011/utilmy/nlp/util_cocount.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_embedding.py` & `utilmy-0.1.16830011/utilmy/nlp/util_embedding.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_explain.py` & `utilmy-0.1.16830011/utilmy/nlp/util_explain.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_gensim.py` & `utilmy-0.1.16830011/utilmy/nlp/util_gensim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_ner.py` & `utilmy-0.1.16830011/utilmy/nlp/util_ner.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_nlp.py` & `utilmy-0.1.16830011/utilmy/nlp/util_nlp.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_topk.py` & `utilmy-0.1.16830011/utilmy/nlp/util_topk.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/util_transformers.py` & `utilmy-0.1.16830011/utilmy/nlp/util_transformers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nlp/zzz_text.py` & `utilmy-0.1.16830011/utilmy/nlp/zzz_text.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/nnumpy.py` & `utilmy-0.1.16830011/utilmy/nnumpy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/oos.py` & `utilmy-0.1.16830011/utilmy/oos.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/expression_check.py` & `utilmy-0.1.16830011/utilmy/optim/expression_check.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/gp_ranking.py` & `utilmy-0.1.16830011/utilmy/optim/gp_ranking.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/gp_searchformulae.py` & `utilmy-0.1.16830011/utilmy/optim/gp_searchformulae.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/res_ranking.txt` & `utilmy-0.1.16830011/utilmy/optim/res_ranking.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/util_hyper.py` & `utilmy-0.1.16830011/utilmy/optim/util_hyper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/util_optim.py` & `utilmy-0.1.16830011/utilmy/optim/util_optim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/zold/gp.py` & `utilmy-0.1.16830011/utilmy/optim/zold/gp.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/zold/gp_dcgp.py` & `utilmy-0.1.16830011/utilmy/optim/zold/gp_dcgp.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/zold/gp_dcgp2.py` & `utilmy-0.1.16830011/utilmy/optim/zold/gp_dcgp2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/zold/gp_formulae.py` & `utilmy-0.1.16830011/utilmy/optim/zold/gp_formulae.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/optim/zold/gp_searchformulae_old.py` & `utilmy-0.1.16830011/utilmy/optim/zold/gp_searchformulae_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/parallel.py` & `utilmy-0.1.16830011/utilmy/parallel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/ppandas.py` & `utilmy-0.1.16830011/utilmy/ppandas.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/ppolars.py` & `utilmy-0.1.16830011/utilmy/ppolars.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/prepro.py` & `utilmy-0.1.16830011/utilmy/prepro/prepro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/prepro_rec.py` & `utilmy-0.1.16830011/utilmy/prepro/prepro_rec.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/prepro_text.py` & `utilmy-0.1.16830011/utilmy/prepro/prepro_text.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/prepro_tseries.py` & `utilmy-0.1.16830011/utilmy/prepro/prepro_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/run_feature_profile.py` & `utilmy-0.1.16830011/utilmy/prepro/run_feature_profile.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/prepro/util_feature.py` & `utilmy-0.1.16830011/utilmy/prepro/util_feature.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ab.py` & `utilmy-0.1.16830011/utilmy/recsys/ab.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/aabandit_design.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/aabandit_design.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/CONTRIBUTING.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/DOCS.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/DOCS.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/Pipfile.lock` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/data_reader/reader.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/data_reader/reader.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/bq.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/bq.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/v1.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/v1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/db/v2.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/db/v2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/benchmarks.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/benchmarks.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/models/embed_dnn.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/models/embed_dnn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/preprocessing/preprocessor.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/serving/predictor.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/serving/predictor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/training/trainer.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/training/trainer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/feature_importance.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/feature_importance.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/model_constructors.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/model_constructors.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/model_trainers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/model_trainers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/banditml/utils/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/banditml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/configs/example_feature_config.json` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/configs/example_feature_config.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/configs/example_ml_config.json` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/configs/example_ml_config.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/scripts/create_bq_tables.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/scripts/create_bq_tables.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/setup.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/serving/test_predictor.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/serving/test_predictor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/banditml/training/test_train_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/banditml/training/test_train_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/fixtures.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml/tests/test_models.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/CONTRIBUTING.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/README.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/dev-requirements.txt` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/1 - Evaluating a new fraud policy with IPS.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/1 - Evaluating a new fraud policy with IPS.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/2 - Evaluating a new fraud policy with the direct method.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/2 - Evaluating a new fraud policy with the direct method.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/examples/3 - Evaluating a new fraud policy with the doubly robust method.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/examples/3 - Evaluating a new fraud policy with the doubly robust method.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/gbdt.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/gbdt.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/estimators/linear.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/estimators/linear.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/direct_method.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/direct_method.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/doubly_robust.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/methods/inverse_propensity_scoring.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/methods/inverse_propensity_scoring.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/ope/training/predictor.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/ope/training/predictor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/banditml_eval/setup.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/banditml_eval/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/LICENSE` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/LICENSE`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/README.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/epsilon_greedy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/exp3.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/exp3.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/run.sh` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/run.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/create_movielens_dataset.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/create_movielens_dataset.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/eda.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/eda.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/scripts/visualize_results.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/scripts/visualize_results.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/ucb.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/ucb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/bandits/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/bandits/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/eval_replay/data/ml-20m/README.txt` & `utilmy-0.1.16830011/utilmy/recsys/bandits/eval_replay/data/ml-20m/README.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/GETTING_STARTED.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/INSTALL.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/INSTALL.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/README.md` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/Makefile` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/Makefile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/make.bat` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/make.bat`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/requirements.txt` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/conf.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/docs/source/index.rst` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/environment.yml` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/environment.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/Bandit_demo.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/Bandit_demo.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/DQN_demo.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/DQN_demo.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/deep.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/deep.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/deep_cb.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/deep_cb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/genetic_rl.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/genetic_rl.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/genetic_rl_q_learning.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/genetic_rl_q_learning.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/A2C-CartPole-v0-ep100.db` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/A2C-CartPole-v0-ep100.db`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/a2c_cartpole-v0.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/a2c_cartpole-v0.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/td3_pendulum-v0.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/hyperparameters/optuna/td3_pendulum-v0.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/examples/run_cb.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/examples/run_cb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/__init__.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/bootstrap_neural.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/bootstrap_neural.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/base_model.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/base_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/bayesian.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/bayesian.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/neural.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/neural.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/transition.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/common/transition.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/fixed.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/fixed.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/linpos.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/linpos.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_greedy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_greedy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_linpos.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_linpos.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_noise_sampling.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/neural_noise_sampling.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/variational.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/contextual/variational.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bayesian.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bayesian.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bernoulli_mab.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/bernoulli_mab.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/epsgreedy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/epsgreedy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gaussian_mab.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gaussian_mab.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gradient.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/gradient.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/thompson.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/thompson.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/ucb.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/bandits/multiarmed/ucb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/qlearning.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/qlearning/qlearning.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/sarsa.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/sarsa/sarsa.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/valueiteration.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/classical/valueiteration/valueiteration.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/a2c.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/offpolicy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/offpolicy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/onpolicy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/base/onpolicy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/ddpg.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/categorical.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/categorical.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/double.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/double.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/dueling.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/dueling.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/noisy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/noisy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/prioritized.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/prioritized.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/dqn/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/ppo1.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/ppo1/ppo1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/sac.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/sac/sac.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/td3.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/td3/td3.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/vpg.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/agents/deep/vpg/vpg.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/__init__.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/actor_critic.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/actor_critic.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/buffers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/buffers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/noise.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/noise.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/policies.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/policies.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/rollout_storage.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/rollout_storage.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/core/values.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/core/values.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/__init__.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/action_wrappers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/action_wrappers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/atari_preprocessing.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/atari_preprocessing.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/atari_wrappers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/base_wrapper.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/frame_stack.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/frame_stack.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/gym_wrapper.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/suite.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/suite.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/time_limit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/time_limit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/torch.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/torch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/monitor.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/monitor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/normalize.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/normalize.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/vector_envs.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/vector_envs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/wrappers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/environments/vec_env/wrappers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/genetic_hyperparam.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/genetic_hyperparam.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/evolutionary/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/evolutionary/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/classical.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/classical.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/offpolicy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/offpolicy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/trainers/onpolicy.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/trainers/onpolicy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/__init__.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/adult_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/adult_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/base.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/base.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/census_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/census_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/covertype_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/covertype_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/magic_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/magic_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/mushroom_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/mushroom_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/statlog_bandit.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/statlog_bandit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/data_bandits/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/discount.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/discount.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/logger.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/models.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/genrl/utils/utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/genrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/setup.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_cb_agents.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_cb_agents.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_data_bandits.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_data_bandits.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_mab_agents.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_bandit/test_mab_agents.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/test_agents.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_classical/test_agents.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_a2c.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_a2c.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_custom.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_custom.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ddpg.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ddpg.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn_cnn.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_dqn_cnn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ppo1.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_ppo1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_sac.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_sac.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_td3.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_td3.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_vpg.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_agents/test_deep/test_vpg.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_atari_wrappers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_vecenv.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_vecenv.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_environments/test_wrappers.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_environments/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_bandit_trainer.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_bandit_trainer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_classical_trainer.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_classical_trainer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_trainers/test_deep_trainer.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_trainers/test_deep_trainer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/test_models.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/test_models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/genrl/tests/test_utils/test_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/genrl/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/offline_replayer_eval_amzon.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/offline_replayer_eval_amzon.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/bandits/recostep_offline_replayer_eval_movielens.py` & `utilmy-0.1.16830011/utilmy/recsys/bandits/recostep_offline_replayer_eval_movielens.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/metric.py` & `utilmy-0.1.16830011/utilmy/recsys/metric.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/metrics/distance_metrics.py` & `utilmy-0.1.16830011/utilmy/recsys/metrics/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessAmazonSportsOutdoors.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessAmazonSportsOutdoors.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessAmazonVideoGames.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessAmazonVideoGames.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessML20M.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessML20M.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessMSD.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessMSD.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessNetflix.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessNetflix.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/PreprocessYahooMovies.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/PreprocessYahooMovies.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/README.md` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/TrainModel.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/TrainModel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/models.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/CEASE/util.py` & `utilmy-0.1.16830011/utilmy/recsys/models/CEASE/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/DynEASEr_Runtime.py` & `utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/DynEASEr_Runtime.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/README.md` & `utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/dynaEASE/util.py` & `utilmy-0.1.16830011/utilmy/recsys/models/dynaEASE/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/ease.py` & `utilmy-0.1.16830011/utilmy/recsys/models/ease.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/prepro1.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/models/prepro1.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/prepro_ae_identity.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/models/prepro_ae_identity.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/prod2vec.py` & `utilmy-0.1.16830011/utilmy/recsys/models/prod2vec.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/README.md` & `utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/environment.py` & `utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/environment.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/main.py` & `utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/online_logistic_regression.py` & `utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/online_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/models/topk_bandit/policies.py` & `utilmy-0.1.16830011/utilmy/recsys/models/topk_bandit/policies.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ranking/optim_rank.py` & `utilmy-0.1.16830011/utilmy/recsys/ranking/optim_rank.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ranking/rank_fusion.py` & `utilmy-0.1.16830011/utilmy/recsys/ranking/rank_fusion.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ranking/rank_fusion_functions.py` & `utilmy-0.1.16830011/utilmy/recsys/ranking/rank_fusion_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ranking/util_rank.py` & `utilmy-0.1.16830011/utilmy/recsys/ranking/util_rank.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/ranking/util_rankmerge.py` & `utilmy-0.1.16830011/utilmy/recsys/ranking/util_rankmerge.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/util_ltr.py` & `utilmy-0.1.16830011/utilmy/recsys/util_ltr.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/util_rec.py` & `utilmy-0.1.16830011/utilmy/recsys/util_rec.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/util_sequencepattern.py` & `utilmy-0.1.16830011/utilmy/recsys/util_sequencepattern.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/util_tfranking.py` & `utilmy-0.1.16830011/utilmy/recsys/util_tfranking.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/vectors.py` & `utilmy-0.1.16830011/utilmy/recsys/vectors.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/AUTHORS.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/CONTRIBUTING.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/GLOSSARY.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/GLOSSARY.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/NEWS.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/NEWS.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/SECURITY.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/SETUP.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/SETUP.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/conda.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/conda.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/DEVELOPMENT.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/contrib/sarplus/azure-pipelines.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/contrib/sarplus/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/Makefile` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/Makefile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/conf.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/datasets.rst` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/datasets.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/index.rst` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/models.rst` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/docs/source/utils.rst` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/als_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/als_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/dkn_MIND.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/dkn_MIND.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/fastai_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/fastai_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/geoimc_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/geoimc_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/lightgbm_tinycriteo.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/lightgbm_tinycriteo.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/lstur_MIND.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/lstur_MIND.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/naml_MIND.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/naml_MIND.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/ncf_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/ncf_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/npa_MIND.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/npa_MIND.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/nrms_MIND.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/nrms_MIND.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/rbm_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/rbm_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/rlrmc_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/rlrmc_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens_with_azureml.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movielens_with_azureml.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sar_movieratings_with_azureml_designer.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sar_movieratings_with_azureml_designer.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/sequential_recsys_amazondataset.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/sequential_recsys_amazondataset.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/tfidf_covid.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/tfidf_covid.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/wide_deep_movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/wide_deep_movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/00_quick_start/xdeepfm_criteo.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/00_quick_start/xdeepfm_criteo.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/data_split.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/data_split.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/data_transform.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/data_transform.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/mind_utils.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/mind_utils.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/01_prepare_data/wikidata_knowledge_graph.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/01_prepare_data/wikidata_knowledge_graph.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/als_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/als_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/baseline_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/baseline_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/multi_vae_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/multi_vae_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/rbm_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/rbm_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/sar_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/sar_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/standard_vae_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/standard_vae_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/dkn_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/dkn_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/mmlspark_lightgbm_criteo.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/mmlspark_lightgbm_criteo.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/fm_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/fm_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/lightfm_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/lightfm_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/02_model_hybrid/ncf_deep_dive.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/02_model_hybrid/ncf_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/als_movielens_diversity_metrics.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/als_movielens_diversity_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/03_evaluate/evaluation.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/03_evaluate/evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_surprise_svd.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_surprise_svd.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_wide_and_deep.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/azureml_hyperdrive_wide_and_deep.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_ncf.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_ncf.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_surprise_svd.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/nni_surprise_svd.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/tuning_spark_als.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/04_model_select_and_optimize/tuning_spark_als.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/aks_locust_load_test.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/aks_locust_load_test.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/als_movie_o16n.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/als_movie_o16n.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/05_operationalize/lightgbm_criteo_o16n.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/05_operationalize/lightgbm_criteo_o16n.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/benchmark_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/06_benchmarks/movielens.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/06_benchmarks/movielens.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/run_notebook_on_azureml.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/run_notebook_on_azureml.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/examples/template.ipynb` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/examples/template.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/amazon_reviews.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/amazon_reviews.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/cosmos_cli.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/cosmos_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/covid_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/covid_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/criteo.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/download_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/download_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/mind.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/mind.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/movielens.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/pandas_df_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/pandas_df_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/python_splitters.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/python_splitters.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/spark_splitters.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/spark_splitters.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/sparse.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/sparse.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/split_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/split_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/datasets/wikidata.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/datasets/wikidata.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/python_evaluation.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/python_evaluation.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/evaluation/spark_evaluation.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/evaluation/spark_evaluation.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/tuning/parameter_sweep.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/tuning/parameter_sweep.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/constants.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/constants.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/general_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/gpu_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/k8s_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/notebook_memory_management.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/notebook_memory_management.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/notebook_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/plot.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/plot.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/python_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/spark_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/tf_utils.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/recommenders/utils/timer.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/recommenders/utils/timer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/news/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/news/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/scenarios/retail/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/scenarios/retail/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/setup.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/azure_artifact_feed.yaml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/azure_artifact_feed.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/component_governance.yaml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/component_governance.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/cpu_unit_tests.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/cpu_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/gpu_unit_test.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/gpu_unit_test.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/nightly_cpu.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/nightly_cpu.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/nightly_gpu.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/nightly_gpu.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/notebooks_gpu_unit_tests.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/notebooks_gpu_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/notebooks_unit_tests.yml` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/notebooks_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/run_pytest.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/run_pytest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/ci/submit_azureml_pytest.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/ci/submit_azureml_pytest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tests/conftest.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/databricks_install.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/databricks_install.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/docker/Dockerfile` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/docker/README.md` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/docker/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/generate_conda_file.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/generate_conda_file.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tools/generate_requirements_txt.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tools/generate_requirements_txt.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/tox.ini` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/tox.ini`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/recsys/zrecs/zprepro_recs.py` & `utilmy-0.1.16830011/utilmy/recsys/zrecs/zprepro_recs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/Dockerfile` & `utilmy-0.1.16830011/utilmy/sspark/Dockerfile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/README.md` & `utilmy-0.1.16830011/utilmy/sspark/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/README_code.md` & `utilmy-0.1.16830011/utilmy/sspark/README_code.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/README_sparksubmit.md` & `utilmy-0.1.16830011/utilmy/sspark/README_sparksubmit.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/conda/README.md` & `utilmy-0.1.16830011/utilmy/sspark/conda/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config_local.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config_local.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config_test.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config_test.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config_test_unit.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config_test_unit.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config_yarn/config_yarn.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config_yarn/config_yarn.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/config_yarn/config_yarn_template.yaml` & `utilmy-0.1.16830011/utilmy/sspark/config/config_yarn/config_yarn_template.yaml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/Dockerfile` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/Dockerfile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/Dockerfile-cluster` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/Dockerfile-cluster`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/LICENSE` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/LICENSE`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/README.md` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/docker-compose-cluster.yml` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/config/hadoop_spark_hive/mapred-site.xml` & `utilmy-0.1.16830011/utilmy/sspark/config/hadoop_spark_hive/mapred-site.xml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/docker-compose.yml` & `utilmy-0.1.16830011/utilmy/sspark/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/main.py` & `utilmy-0.1.16830011/utilmy/sspark/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/script/pysparkTest.py` & `utilmy-0.1.16830011/utilmy/sspark/script/pysparkTest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/script/server_start.sh` & `utilmy-0.1.16830011/utilmy/sspark/script/server_start.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/script/sparkrunscript.sh` & `utilmy-0.1.16830011/utilmy/sspark/script/sparkrunscript.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/GetFamiliesFromUserAgent.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/GetFamiliesFromUserAgent.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/dim_datetime_utilities.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/dim_datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/__init__.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs_base_functions.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/datetime_udfs_base_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/fuzzy_match_udfs.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/fuzzy_match_udfs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions_test.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/general_udfs_base_functions_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/functions/pandas_udfs/timeseries.py` & `utilmy-0.1.16830011/utilmy/sspark/src/functions/pandas_udfs/timeseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/0.test-pyspark.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/0.test-pyspark.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/1.text-classification-logistic.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/1.text-classification-logistic.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/10.fashion-mnist-inceptionv1.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/10.fashion-mnist-inceptionv1.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/2.text-classification-multinomial.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/2.text-classification-multinomial.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/3.topic-modelling-tfidf-lda.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/3.topic-modelling-tfidf-lda.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/4.word-vector.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/4.word-vector.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/7.mnist-sparkflow-feedforward.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/7.mnist-sparkflow-feedforward.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/8.mnist-sparkflow-cnn.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/8.mnist-sparkflow-cnn.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/9.mnist-sparkflow-rnn-lstm.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/9.mnist-sparkflow-rnn-lstm.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/ml/notebooks/inception_utils.py` & `utilmy-0.1.16830011/utilmy/sspark/src/ml/notebooks/inception_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_session_length.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_session_length.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_url_unique.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_url_unique.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_predict_volume.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_predict_volume.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_log.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_session_log.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_session_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/tables/table_user_session_stats.py` & `utilmy-0.1.16830011/utilmy/sspark/src/tables/table_user_session_stats.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/util_hadoop.py` & `utilmy-0.1.16830011/utilmy/sspark/src/util_hadoop.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/util_models.py` & `utilmy-0.1.16830011/utilmy/sspark/src/util_models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/util_spark.py` & `utilmy-0.1.16830011/utilmy/sspark/src/util_spark.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/util_sparkml.py` & `utilmy-0.1.16830011/utilmy/sspark/src/util_sparkml.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/util_trick.py` & `utilmy-0.1.16830011/utilmy/sspark/src/util_trick.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/utils.py` & `utilmy-0.1.16830011/utilmy/sspark/src/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/zvarious/README.md` & `utilmy-0.1.16830011/utilmy/sspark/src/zvarious/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/src/zvarious/deploying-python-ml-in-pyspark.ipynb` & `utilmy-0.1.16830011/utilmy/sspark/src/zvarious/deploying-python-ml-in-pyspark.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/conftest.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_common.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_functions.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_log.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_session_log.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_session_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_table_user_session_stats.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_table_user_session_stats.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_table_volume_predict.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_table_volume_predict.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/sspark/tests/test_utils.py` & `utilmy-0.1.16830011/utilmy/sspark/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/README.md` & `utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/bootstrap_stat.py` & `utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/bootstrap_stat.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/datasets.py` & `utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/datasets.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/pyproject.toml` & `utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/pyproject.toml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/bootstrap_stat/tests/test_bootstrap_stat.py` & `utilmy-0.1.16830011/utilmy/stats/bootstrap_stat/tests/test_bootstrap_stat.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/example.py` & `utilmy-0.1.16830011/utilmy/stats/example.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/README.md` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/_lib.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/_lib.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/aov.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/aov.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/contingency.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/contingency.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/critical.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/critical.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/descriptive.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/descriptive.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/fa.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/fa.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/gof.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/gof.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/hypothesis.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/hypothesis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/nonparametric.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/nonparametric.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/posthoc.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/posthoc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_aov.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_aov.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_contingency.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_contingency.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_critical_values.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_critical_values.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_descriptive.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_descriptive.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_gof.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_gof.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_hypothesis.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_internal.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_nonparametric.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_nonparametric.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/hypothesis/tests/test_posthoc.py` & `utilmy-0.1.16830011/utilmy/stats/hypothesis/tests/test_posthoc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/stats/statistics.py` & `utilmy-0.1.16830011/utilmy/stats/statistics.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/bayesian/abtest_inference.py` & `utilmy-0.1.16830011/utilmy/tabular/bayesian/abtest_inference.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/bayesian/model_bayesian_numpyro.py` & `utilmy-0.1.16830011/utilmy/tabular/bayesian/model_bayesian_numpyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/bayesian/model_bayesian_pyro.py` & `utilmy-0.1.16830011/utilmy/tabular/bayesian/model_bayesian_pyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/causal/readme.md` & `utilmy-0.1.16830011/utilmy/tabular/causal/readme.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/causal/rscripts/run_bnlearn.r` & `utilmy-0.1.16830011/utilmy/tabular/causal/rscripts/run_bnlearn.r`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/causal/util_bnlearn.py` & `utilmy-0.1.16830011/utilmy/tabular/causal/util_bnlearn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/sparse/prepro1.ipynb` & `utilmy-0.1.16830011/utilmy/tabular/sparse/prepro1.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/sparse/prepro_ae_identity.ipynb` & `utilmy-0.1.16830011/utilmy/tabular/sparse/prepro_ae_identity.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/sparse/test_data.py` & `utilmy-0.1.16830011/utilmy/tabular/sparse/test_data.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/sparse/test_model1.py` & `utilmy-0.1.16830011/utilmy/tabular/sparse/test_model1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/sparse/test_model2.py` & `utilmy-0.1.16830011/utilmy/tabular/sparse/test_model2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/tabular.py` & `utilmy-0.1.16830011/utilmy/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_activelearning.py` & `utilmy-0.1.16830011/utilmy/tabular/util_activelearning.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_drift.py` & `utilmy-0.1.16830011/utilmy/tabular/util_drift.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_ensemble.py` & `utilmy-0.1.16830011/utilmy/tabular/util_ensemble.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_explain.py` & `utilmy-0.1.16830011/utilmy/tabular/util_explain.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_generator.py` & `utilmy-0.1.16830011/utilmy/tabular/util_generator.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_lightgbm.py` & `utilmy-0.1.16830011/utilmy/tabular/util_lightgbm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_lineartree.py` & `utilmy-0.1.16830011/utilmy/tabular/util_lineartree.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_regression.py` & `utilmy-0.1.16830011/utilmy/tabular/util_regression.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_sampling.py` & `utilmy-0.1.16830011/utilmy/tabular/util_sampling.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_sparse.py` & `utilmy-0.1.16830011/utilmy/tabular/util_sparse.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tabular/util_uncertainty.py` & `utilmy-0.1.16830011/utilmy/tabular/util_uncertainty.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/cli.py` & `utilmy-0.1.16830011/utilmy/templates/cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/Dockerfile` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/Dockerfile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/README.md` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/README_code.md` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/README_code.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/__init__.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/dataset.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/dataset.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/pipeline.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/pipeline.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/transform.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/transform.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/util_exceptions.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/util_exceptions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/util_image.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/util_image.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/utils.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/mygenerator/validate.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/mygenerator/validate.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/run_pipy.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/run_pipy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/setup.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/__init__.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_dataset.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_import.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_pipeline.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_transform.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_util_image.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_util_image.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/templates/templist/pypi_package/tests/test_validate.py` & `utilmy-0.1.16830011/utilmy/templates/templist/pypi_package/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/README.md` & `utilmy-0.1.16830011/utilmy/tools/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_code/README.md` & `utilmy-0.1.16830011/utilmy/tools/cli_code/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_code/cli_code/cli_doc_auto/main.py` & `utilmy-0.1.16830011/utilmy/tools/cli_code/cli_code/cli_doc_auto/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_code/setup.py` & `utilmy-0.1.16830011/utilmy/tools/cli_code/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_conda_merge.py` & `utilmy-0.1.16830011/utilmy/tools/cli_conda_merge.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_convert_ipynb.py` & `utilmy-0.1.16830011/utilmy/tools/cli_convert_ipynb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_docs.py` & `utilmy-0.1.16830011/utilmy/tools/cli_docs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_download.py` & `utilmy-0.1.16830011/utilmy/tools/cli_download.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_env_autoinstall.py` & `utilmy-0.1.16830011/utilmy/tools/cli_env_autoinstall.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_json.py` & `utilmy-0.1.16830011/utilmy/tools/cli_json.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_module_parser.py` & `utilmy-0.1.16830011/utilmy/tools/cli_module_parser.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cli_repo_check.py` & `utilmy-0.1.16830011/utilmy/tools/cli_repo_check.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/Pipfile.lock` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/README.md` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/project_graph/project_graph` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/project_graph/project_graph`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/setup.py` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/test_script_argparse.py` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/test_script_argparse.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/codeparser_project_graph/tests/test_performance_graph.py` & `utilmy-0.1.16830011/utilmy/tools/codeparser_project_graph/tests/test_performance_graph.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cyberduck/Google Drive.cyberduckprofile` & `utilmy-0.1.16830011/utilmy/tools/cyberduck/Google Drive.cyberduckprofile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/cyberduck/cli_duck.py` & `utilmy-0.1.16830011/utilmy/tools/cyberduck/cli_duck.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/globre.py` & `utilmy-0.1.16830011/utilmy/tools/globre.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/googledrive_upload/Steps.txt` & `utilmy-0.1.16830011/utilmy/tools/googledrive_upload/Steps.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/googledrive_upload/apps.py` & `utilmy-0.1.16830011/utilmy/tools/googledrive_upload/apps.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/googledrive_upload/token.json` & `utilmy-0.1.16830011/utilmy/tools/googledrive_upload/token.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/README.md` & `utilmy-0.1.16830011/utilmy/tools/mybash/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/bashrc_template/bashrc_base_1.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/bashrc_template/bashrc_base_1.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/bashrc_template/zshrc_macos.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/bashrc_template/zshrc_macos.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/docs/bash_history` & `utilmy-0.1.16830011/utilmy/tools/mybash/docs/bash_history`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/docs/bashrc` & `utilmy-0.1.16830011/utilmy/tools/mybash/docs/bashrc`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/docs/bashrc_base.txt` & `utilmy-0.1.16830011/utilmy/tools/mybash/docs/bashrc_base.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/docs/pylint_jedi.txt` & `utilmy-0.1.16830011/utilmy/tools/mybash/docs/pylint_jedi.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale_test` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/aaws/zbatch_autoscale_test`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cconda/conda_backup_all` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cconda/conda_backup_all`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/croncheck` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/croncheck`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/cronjob` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/cronjob`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ccron/cronjob.txt` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ccron/cronjob.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/cicd/jwms-lib.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/cicd/jwms-lib.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/files` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/files`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/findstr` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/findstr`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/folder` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/folder`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggdrive/wget_googledrive` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggdrive/wget_googledrive`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggithub/github_cloneall` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggithub/github_cloneall`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ggithub/github_getallrepo.py` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ggithub/github_getallrepo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/gitpush` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/gitpush`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/jupytercmd` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/jupytercmd`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/nnode` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/nnode`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/__all.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/__all.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/allserver.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/allserver.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/aws_endpoint.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/aws_endpoint.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/buildDocs.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/buildDocs.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/check_iam.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/check_iam.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/check_redshift.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/check_redshift.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/common_header.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/common_header.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-allenai-wmt16.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-allenai-wmt16.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-allenai-wmt19.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-allenai-wmt19.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert-facebook-wmt19.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert-facebook-wmt19.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/convert_dataset.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/convert_dataset.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/distil_marian_enro_teacher.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/distil_marian_enro_teacher.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/distil_marian_no_teacher.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/distil_marian_no_teacher.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/download_from_gcp.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/download_from_gcp.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/dynamic_bs_example.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/dynamic_bs_example.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/entropy_eval.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/entropy_eval.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/eval_deebert.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/eval_deebert.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/hourly_data.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/hourly_data.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run_ner.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run_ner.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/run_pos.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/run_pos.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/scores_run.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/scores_run.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/start_generic_method.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/start_generic_method.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/others/tests-to-run.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/others/tests-to-run.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ss3/mount_s3drive` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ss3/mount_s3drive`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/util_date.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/util_date.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/util_macos.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/util_macos.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/ssource/utils.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/ssource/utils.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/homecopy` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/homecopy`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/util_stable.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/util_stable.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/utils.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/utils.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/utils/utils2.sh` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/utils/utils2.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/mybash/mybash/zzip` & `utilmy-0.1.16830011/utilmy/tools/mybash/mybash/zzip`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/Welcome_To_Colaboratory.ipynb` & `utilmy-0.1.16830011/utilmy/tools/test/Welcome_To_Colaboratory.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/cli_convert_ipynb.py` & `utilmy-0.1.16830011/utilmy/tools/test/cli_convert_ipynb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/file0.yml` & `utilmy-0.1.16830011/utilmy/tools/test/file0.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/file1.yml` & `utilmy-0.1.16830011/utilmy/tools/test/file1.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/run_train.py` & `utilmy-0.1.16830011/utilmy/tools/test/run_train.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/test/run_train.py` & `utilmy-0.1.16830011/utilmy/tools/test/test/run_train.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/test_all.sh` & `utilmy-0.1.16830011/utilmy/tools/test/test_all.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ast_analyzer_test.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ast_analyzer_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/file_finder_test.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/file_finder_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ok/ztest_import.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ok/ztest_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ok/ztest_log_all.txt` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ok/ztest_log_all.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/output_test.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/output_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_import.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_runall.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_runall.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/test/ztest/ztest_util.py` & `utilmy-0.1.16830011/utilmy/tools/test/ztest/ztest_util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tools/util_cli.py` & `utilmy-0.1.16830011/utilmy/tools/util_cli.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/models/model_bayesian_pyro.py` & `utilmy-0.1.16830011/utilmy/tseries/models/model_bayesian_pyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/models/model_tseries.py` & `utilmy-0.1.16830011/utilmy/tseries/models/model_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/prepro_tseries.py` & `utilmy-0.1.16830011/utilmy/tseries/prepro_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/torch_lstm (1).py` & `utilmy-0.1.16830011/utilmy/tseries/torch_lstm (1).py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/torch_lstm.py` & `utilmy-0.1.16830011/utilmy/tseries/torch_lstm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/torch_outlier.py` & `utilmy-0.1.16830011/utilmy/tseries/torch_outlier.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/torch_outlier_comment.py` & `utilmy-0.1.16830011/utilmy/tseries/torch_outlier_comment.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/tseries/util_tseries.py` & `utilmy-0.1.16830011/utilmy/tseries/util_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_batch.py` & `utilmy-0.1.16830011/utilmy/util_batch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_colab.py` & `utilmy-0.1.16830011/utilmy/util_colab.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_conda.py` & `utilmy-0.1.16830011/utilmy/util_conda.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_cpu.py` & `utilmy-0.1.16830011/utilmy/util_cpu.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_download.py` & `utilmy-0.1.16830011/utilmy/util_download.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_numba.py` & `utilmy-0.1.16830011/utilmy/util_numba.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/util_zip.py` & `utilmy-0.1.16830011/utilmy/util_zip.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/utilmy_base.py` & `utilmy-0.1.16830011/utilmy/utilmy_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,14 +759,47 @@
         with open(self.findex, mode='a') as fp:
             fp.write(ss )
         return True   
 
 
 
 ###################################################################################################
+def json_load(path) :
+  """function json_load.
+  Doc::
+          
+  """
+  try :
+    return json.load(open( path, mode='r'))
+  except Exception as e :
+    log(e)
+    return {}
+
+
+def json_save(dd:dict, path:str) :
+  """function json_save
+  Doc::
+          
+  """
+  os_makedirs(path)
+  try :
+    json.dump(dd, open( path, mode='w'))
+    return path
+  except Exception as e :
+    log(e)
+
+
+def pprint(dd,indent=3):
+    if isinstance(dd, dict):
+        log(json.dumps(cc, sort_keys=True, indent=indent,separators=(',', ': ') ))  
+    else :
+        log(dd)
+
+    
+###################################################################################################
 ###### Pandas #####################################################################################
 from utilmy.parallel import (
     pd_read_file,    ### parallel reading
     pd_read_file2,
     pd_groupby_parallel,
 )
```

### Comparing `utilmy-0.1.16802704/utilmy/utils.py` & `utilmy-0.1.16830011/utilmy/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/css.py` & `utilmy-0.1.16830011/utilmy/viz/css.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/app.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/app.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/img/jsoneditor-icons.svg` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/img/jsoneditor-icons.svg`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/jsoneditor.min.css` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/jsoneditor.min.css`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/jsoneditor.min.js` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/mixed_layout.json` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/mixed_layout.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/scripts.js` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/scripts.js`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/css_base1.css` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/css_base1.css`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/dash_layout.json` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/dash_layout.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/html_layout.json` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/html_layout.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/assets/template/links_layout.json` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/assets/template/links_layout.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/form_calc.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/form_calc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/form_uploadjson.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/form_uploadjson.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/page1.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/page1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/page2.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/page2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/ca_target.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/ca_target.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/chronos_viewer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/chronos_viewer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/framework_batches.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/framework_batches.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/hdfs_viewer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/hdfs_viewer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/main_page.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/main_page.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/nohit_explorer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/nohit_explorer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/templates/yarn_apps.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/templates/yarn_apps.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/util_dash.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/util_dash.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app1/pages/utils.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app1/pages/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/main.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/main.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/mmm/contribution.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/mmm/contribution.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/multi-page.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/multi-page.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/app2_example/pages/group-level-mmm.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/app2_example/pages/group-level-mmm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/dash_help.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/dash_help.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/app.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/app.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/ng_word.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/ng_word.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dash-poc/basic/shop_limited_word.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dash-poc/basic/shop_limited_word.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/Makefile` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/Makefile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/README.md` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/docker/Dockerfile` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/src/config.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/src/config.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/dashboard1/src/run.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/dashboard1/src/run.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/app.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/app.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/helpers/utils.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/layout/layout.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/layout/layout.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/ca_targeting_qa.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/ca_targeting_qa.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/chronos_viewer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/chronos_viewer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/hdfs_viewer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/hdfs_viewer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/nohit_explorer.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/nohit_explorer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/pages/yarn_apps.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/pages/yarn_apps.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/requirements.txt` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/requirements.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/ddash/simple-dash/routes.py` & `utilmy-0.1.16830011/utilmy/viz/ddash/ddash/simple-dash/routes.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/ddash/readme_help.md` & `utilmy-0.1.16830011/utilmy/viz/ddash/readme_help.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/embedding.py` & `utilmy-0.1.16830011/utilmy/viz/embedding.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/model.vec` & `utilmy-0.1.16830011/utilmy/viz/model.vec`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/template1.py` & `utilmy-0.1.16830011/utilmy/viz/template1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/test_vizhtml.py` & `utilmy-0.1.16830011/utilmy/viz/test_vizhtml.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/testdata/viz_test3_all_graphs.html` & `utilmy-0.1.16830011/utilmy/viz/testdata/viz_test3_all_graphs.html`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/util_map.py` & `utilmy-0.1.16830011/utilmy/viz/util_map.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/video.py` & `utilmy-0.1.16830011/utilmy/viz/video.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/vizhtml.py` & `utilmy-0.1.16830011/utilmy/viz/vizhtml.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/viz/zarchive/toptoolbar.py` & `utilmy-0.1.16830011/utilmy/viz/zarchive/toptoolbar.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/batch_colab_scraper.ipynb` & `utilmy-0.1.16830011/utilmy/webscraper/batch_colab_scraper.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_arxiv.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_arxiv.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_github_gist_search.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_github_gist_search.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_github_search.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_github_search.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_leetcode_extract.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_leetcode_extract.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_openreview.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_openreview.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/cli_reddit.py` & `utilmy-0.1.16830011/utilmy/webscraper/cli_reddit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/pdf_scraper.py` & `utilmy-0.1.16830011/utilmy/webscraper/pdf_scraper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/scrape_batch.py` & `utilmy-0.1.16830011/utilmy/webscraper/scrape_batch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/test/Scraper_INSTAGRAM.py` & `utilmy-0.1.16830011/utilmy/webscraper/test/Scraper_INSTAGRAM.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/test/scraper_img.py` & `utilmy-0.1.16830011/utilmy/webscraper/test/scraper_img.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/test/url_scraper.py` & `utilmy-0.1.16830011/utilmy/webscraper/test/url_scraper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/test/vc_scraper.py` & `utilmy-0.1.16830011/utilmy/webscraper/test/vc_scraper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/util_search.py` & `utilmy-0.1.16830011/utilmy/webscraper/util_search.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/webscraper/util_web.py` & `utilmy-0.1.16830011/utilmy/webscraper/util_web.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zdocstring.py` & `utilmy-0.1.16830011/utilmy/zdocstring.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/README.md` & `utilmy-0.1.16830011/utilmy/zml/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/core_deploy.py` & `utilmy-0.1.16830011/utilmy/zml/core_deploy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/core_run.py` & `utilmy-0.1.16830011/utilmy/zml/core_run.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/core_test.py` & `utilmy-0.1.16830011/utilmy/zml/core_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/datasketch_hashing.py` & `utilmy-0.1.16830011/utilmy/zml/datasketch_hashing.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_adfraud.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_adfraud.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_airline.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_airline.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_bankloan.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_bankloan.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_cardiff.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_cardiff.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_income.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_income.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_multi.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_multi.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_optuna.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_optuna.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier/classifier_sentiment.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier/classifier_sentiment.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/classifier_mlflow.py` & `utilmy-0.1.16830011/utilmy/zml/example/classifier_mlflow.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/click/online_shopping.py` & `utilmy-0.1.16830011/utilmy/zml/example/click/online_shopping.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/click/outlier_predict.py` & `utilmy-0.1.16830011/utilmy/zml/example/click/outlier_predict.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/click/test_online_shopping.py` & `utilmy-0.1.16830011/utilmy/zml/example/click/test_online_shopping.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/regress/regress_airbnb.py` & `utilmy-0.1.16830011/utilmy/zml/example/regress/regress_airbnb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/regress/regress_boston.py` & `utilmy-0.1.16830011/utilmy/zml/example/regress/regress_boston.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/regress/regress_house.py` & `utilmy-0.1.16830011/utilmy/zml/example/regress/regress_house.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/regress/regress_salary.py` & `utilmy-0.1.16830011/utilmy/zml/example/regress/regress_salary.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/svd/benchmark_mf.py` & `utilmy-0.1.16830011/utilmy/zml/example/svd/benchmark_mf.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/svd/benchmark_mf0.py` & `utilmy-0.1.16830011/utilmy/zml/example/svd/benchmark_mf0.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test.ipynb` & `utilmy-0.1.16830011/utilmy/zml/example/test.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test.py` & `utilmy-0.1.16830011/utilmy/zml/example/test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_automl.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_automl.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_features.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_features.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_hyperopt.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_keras_vaemdn.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_keras_vaemdn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_keras_vaemdn2.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_keras_vaemdn2.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_mkeras.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_mkeras.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/test_mkeras_dense.py` & `utilmy-0.1.16830011/utilmy/zml/example/test_mkeras_dense.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/titanic_gefs.py` & `utilmy-0.1.16830011/utilmy/zml/example/titanic_gefs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_m5sales.py` & `utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_m5sales.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_retail.py` & `utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_retail.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/tseries/tseries_sales.py` & `utilmy-0.1.16830011/utilmy/zml/example/tseries/tseries_sales.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/zfraud.py` & `utilmy-0.1.16830011/utilmy/zml/example/zfraud.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/example/zmodel_new.txt` & `utilmy-0.1.16830011/utilmy/zml/example/zmodel_new.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/py36.txt` & `utilmy-0.1.16830011/utilmy/zml/install/py36.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/pygraphviz-1.5-cp36-cp36m-win_amd64.whl` & `utilmy-0.1.16830011/utilmy/zml/install/pygraphviz-1.5-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/conda_list.yml` & `utilmy-0.1.16830011/utilmy/zml/install/zold/conda_list.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/py36_conda.txt` & `utilmy-0.1.16830011/utilmy/zml/install/zold/py36_conda.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/py36_full.txt` & `utilmy-0.1.16830011/utilmy/zml/install/zold/py36_full.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/py36b.txt` & `utilmy-0.1.16830011/utilmy/zml/install/zold/py36b.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/py36c.txt` & `utilmy-0.1.16830011/utilmy/zml/install/zold/py36c.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/install/zold/ztodo.txt` & `utilmy-0.1.16830011/utilmy/zml/install/zold/ztodo.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/bin/column_encoder.py` & `utilmy-0.1.16830011/utilmy/zml/source/bin/column_encoder.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/bin/feature_engineerng_RL.pdf` & `utilmy-0.1.16830011/utilmy/zml/source/bin/feature_engineerng_RL.pdf`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/dataset.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/dataset.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/keras_deepctr.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/keras_deepctr.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/keras_widedeep.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/keras_widedeep.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/keras_widedeep_dense.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/keras_widedeep_dense.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_bayesian_numpyro.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_bayesian_numpyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_bayesian_pyro.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_bayesian_pyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_encoder.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_encoder.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_gefs.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_gefs.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_numpyro.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_numpyro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_outlier.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_outlier.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_sampler.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_sampler.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_sklearn.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_sklearn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_tseries.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_vaem.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_vaem.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/model_vaemdn.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/model_vaemdn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/optuna_lightgbm.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/optuna_lightgbm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/torch_ease.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/torch_ease.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/torch_rectorch.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/torch_rectorch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/torch_rvae.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/torch_rvae.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/torch_tabular.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/torch_tabular.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/models/util_models.py` & `utilmy-0.1.16830011/utilmy/zml/source/models/util_models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/prepro.py` & `utilmy-0.1.16830011/utilmy/zml/source/prepro.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/prepro_rec.py` & `utilmy-0.1.16830011/utilmy/zml/source/prepro_rec.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/prepro_text.py` & `utilmy-0.1.16830011/utilmy/zml/source/prepro_text.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/prepro_tseries.py` & `utilmy-0.1.16830011/utilmy/zml/source/prepro_tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_feature_profile.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_feature_profile.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_hyperopt.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_hyperopt.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_inference.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_inference.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_inpection.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_inpection.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_mlflow.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_mlflow.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_preprocess.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_preprocess.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_sampler.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_sampler.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/run_train.py` & `utilmy-0.1.16830011/utilmy/zml/source/run_train.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/util.py` & `utilmy-0.1.16830011/utilmy/zml/source/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/util_feature.py` & `utilmy-0.1.16830011/utilmy/zml/source/util_feature.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/stopwords_en.json` & `utilmy-0.1.16830011/utilmy/zml/source/utils/stopwords_en.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_autofeature.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_autofeature.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_automl.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_automl.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_credit.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_credit.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_csv.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_csv.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_date.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_date.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_import.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_import.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_metric.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_metric.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_model.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_optim.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_optim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_pipeline.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_pipeline.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_plot.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_plot.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_sql.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_sql.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_stat.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_stat.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_text.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_text.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/util_text_embedding.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/util_text_embedding.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/source/utils/ztest.py` & `utilmy-0.1.16830011/utilmy/zml/source/utils/ztest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/titanic_classifier.py` & `utilmy-0.1.16830011/utilmy/zml/titanic_classifier.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/toutlier.py` & `utilmy-0.1.16830011/utilmy/zml/toutlier.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/tsampler.py` & `utilmy-0.1.16830011/utilmy/zml/tsampler.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/tseries.py` & `utilmy-0.1.16830011/utilmy/zml/tseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/zgitutil.py` & `utilmy-0.1.16830011/utilmy/zml/zgitutil.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zml/ztemplate.py` & `utilmy-0.1.16830011/utilmy/zml/ztemplate.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/_HELP.py` & `utilmy-0.1.16830011/utilmy/zzarchive/_HELP.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/alldata.py` & `utilmy-0.1.16830011/utilmy/zzarchive/alldata.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/allmodule.py` & `utilmy-0.1.16830011/utilmy/zzarchive/allmodule.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/allmodule_fin.py` & `utilmy-0.1.16830011/utilmy/zzarchive/allmodule_fin.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/coke_functions.py` & `utilmy-0.1.16830011/utilmy/zzarchive/coke_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/datanalysis.py` & `utilmy-0.1.16830011/utilmy/zzarchive/datanalysis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/excel.py` & `utilmy-0.1.16830011/utilmy/zzarchive/excel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/fast.py` & `utilmy-0.1.16830011/utilmy/zzarchive/fast.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/fast_parallel.py` & `utilmy-0.1.16830011/utilmy/zzarchive/fast_parallel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/filelock.py` & `utilmy-0.1.16830011/utilmy/zzarchive/filelock.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/function_custom.py` & `utilmy-0.1.16830011/utilmy/zzarchive/function_custom.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/geospatial.py` & `utilmy-0.1.16830011/utilmy/zzarchive/geospatial.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/global01.py` & `utilmy-0.1.16830011/utilmy/zzarchive/global01.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/kagglegym.py` & `utilmy-0.1.16830011/utilmy/zzarchive/kagglegym.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/linux.py` & `utilmy-0.1.16830011/utilmy/zzarchive/linux.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/multiprocessfunc.py` & `utilmy-0.1.16830011/utilmy/zzarchive/multiprocessfunc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/multithread.py` & `utilmy-0.1.16830011/utilmy/zzarchive/multithread.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/portfolio.py` & `utilmy-0.1.16830011/utilmy/zzarchive/portfolio.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/portfolio_withdate.py` & `utilmy-0.1.16830011/utilmy/zzarchive/portfolio_withdate.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/_HELP.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/_HELP.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/alldata.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/alldata.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/allmodule.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/allmodule.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/allmodule_fin.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/allmodule_fin.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/coke_functions.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/coke_functions.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/datanalysis.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/datanalysis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/excel.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/excel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/fast.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/fast.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/fast_parallel.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/fast_parallel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/filelock.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/filelock.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/function_custom.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/function_custom.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/geospatial.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/geospatial.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/global01.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/global01.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/kagglegym.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/kagglegym.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/linux.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/linux.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/multiprocessfunc.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/multiprocessfunc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/portfolio.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/portfolio.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/portfolio_withdate.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/portfolio_withdate.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/report.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/report.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/rstatpy.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/rstatpy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util.py.bak` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util.py.bak`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util_min.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util_min.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/util_ml.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/util_ml.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py2to3/utilgeo.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py2to3/utilgeo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/py3/util.py` & `utilmy-0.1.16830011/utilmy/zzarchive/py3/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/report.py` & `utilmy-0.1.16830011/utilmy/zzarchive/report.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/rstatpy.py` & `utilmy-0.1.16830011/utilmy/zzarchive/rstatpy.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/codeanalysis.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/codeanalysis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/global01.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/global01.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackage_gen/util.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackage_gen/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/aapackagedev/random.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/aapackagedev/random.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/alldata.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/alldata.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/allmodule.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/allmodule.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/benchmarktest.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/benchmarktest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/codeanalysis.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/codeanalysis.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/dbcheck.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/dbcheck.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/derivatives.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/derivatives.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/dl_utils.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/dl_utils.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/excel.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/excel.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/global01.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/global01.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/installNewPackage.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/installNewPackage.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/java.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/java.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/multiprocessfunc.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/multiprocessfunc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/panda_util.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/panda_util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/portfolio.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/portfolio.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/rec_data.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/rec_data.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/rec_metrics.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/rec_metrics.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/sobol.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/sobol.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/stateprocessor.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/stateprocessor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/symbolicmath.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/symbolicmath.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/technical_indicator.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/technical_indicator.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/testmulti.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/testmulti.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/theano_imdb.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/theano_imdb.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/storage/theano_lstm.py` & `utilmy-0.1.16830011/utilmy/zzarchive/storage/theano_lstm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util.py.bak` & `utilmy-0.1.16830011/utilmy/zzarchive/util.py.bak`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util_aws.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util_aws.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util_min.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util_min.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util_ml.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util_ml.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util_sql.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util_sql.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/util_web.py` & `utilmy-0.1.16830011/utilmy/zzarchive/util_web.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/utilgeo.py` & `utilmy-0.1.16830011/utilmy/zzarchive/utilgeo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/zzarchive/zutil.py` & `utilmy-0.1.16830011/utilmy/zzarchive/zzarchive/zutil.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzarchive/zzarchive/zutil_features.py` & `utilmy-0.1.16830011/utilmy/zzarchive/zzarchive/zutil_features.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/LICENSE` & `utilmy-0.1.16830011/utilmy/zzml/LICENSE`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README.md` & `utilmy-0.1.16830011/utilmy/zzml/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README_HowTo.md` & `utilmy-0.1.16830011/utilmy/zzml/README_HowTo.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README_addmodel.md` & `utilmy-0.1.16830011/utilmy/zzml/README_addmodel.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README_research_papers.md` & `utilmy-0.1.16830011/utilmy/zzml/README_research_papers.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README_testing.md` & `utilmy-0.1.16830011/utilmy/zzml/README_testing.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/README_usage_CLI.md` & `utilmy-0.1.16830011/utilmy/zzml/README_usage_CLI.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/DEV_docs/dataloader.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/DEV_docs/dataloader.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/DEV_docs/json.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/DEV_docs/json.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_addmodel.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_addmodel.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_research_papers.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_research_papers.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_testing.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_testing.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_usage_CLI.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_usage_CLI.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/README_usage_USECASE.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/README_usage_USECASE.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/deep_learning_models.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/deep_learning_models.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/README_docs/reinforcement_learning_paperes.md` & `utilmy-0.1.16830011/utilmy/zzml/docs/README_docs/reinforcement_learning_paperes.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_line.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_line.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_list.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_list.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/error_logs.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/error_logs.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/mxnetf.png` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/mxnetf.png`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/pytorch.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/pytorch.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/tenserflow.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/tenserflow.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/test_cli_error.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/test_cli_error.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/imgs/test_repo.PNG` & `utilmy-0.1.16830011/utilmy/zzml/docs/imgs/test_repo.PNG`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/misc/Makefile` & `utilmy-0.1.16830011/utilmy/zzml/docs/misc/Makefile`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/misc/details_list.txt` & `utilmy-0.1.16830011/utilmy/zzml/docs/misc/details_list.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/misc/make.bat` & `utilmy-0.1.16830011/utilmy/zzml/docs/misc/make.bat`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/misc/readdocs.txt` & `utilmy-0.1.16830011/utilmy/zzml/docs/misc/readdocs.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/source/conf.py` & `utilmy-0.1.16830011/utilmy/zzml/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/docs/source/index.rst` & `utilmy-0.1.16830011/utilmy/zzml/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/requirements_fake.txt` & `utilmy-0.1.16830011/utilmy/zzml/install/requirements_fake.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/run_doc.bat` & `utilmy-0.1.16830011/utilmy/zzml/install/run_doc.bat`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/run_doc.py` & `utilmy-0.1.16830011/utilmy/zzml/install/run_doc.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/run_install.sh` & `utilmy-0.1.16830011/utilmy/zzml/install/run_install.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/run_install2.sh` & `utilmy-0.1.16830011/utilmy/zzml/install/run_install2.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/run_pypi.py` & `utilmy-0.1.16830011/utilmy/zzml/install/run_pypi.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/zconda/centos_jupyter_docker` & `utilmy-0.1.16830011/utilmy/zzml/install/zconda/centos_jupyter_docker`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/zconda/docker2.yml` & `utilmy-0.1.16830011/utilmy/zzml/install/zconda/docker2.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/zconda/env_10_list.txt` & `utilmy-0.1.16830011/utilmy/zzml/install/zconda/env_10_list.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/zconda/zconda_distri_py36tch.yml` & `utilmy-0.1.16830011/utilmy/zzml/install/zconda/zconda_distri_py36tch.yml`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/install/zconda/zinstall.txt` & `utilmy-0.1.16830011/utilmy/zzml/install/zconda/zinstall.txt`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/_version.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/_version.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/benchmark.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/benchmark.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/config/cli_test_list.md` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/config/cli_test_list.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/data.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/data.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/dataloader.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/dataloader.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/dataloader_test.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/dataloader_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/distri_torch.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/distri_torch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/distri_torch_mpirun.sh` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/distri_torch_mpirun.sh`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/distributed.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/distributed.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/README_usage.md` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/README_usage.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/arun_hyper.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/arun_hyper.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/arun_model.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/arun_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/benchmark_timeseries_m4.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/benchmark_timeseries_m4.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/benchmark_timeseries_m5.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/benchmark_timeseries_m5.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/fashion_MNIST_mlmodels.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/fashion_MNIST_mlmodels.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/gluon_automl_titanic.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/gluon_automl_titanic.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras-textcnn.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras-textcnn.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/keras_charcnn_reuters.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_glass.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_glass.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_home_retail.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_home_retail.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/lightgbm_titanic_hyper.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/lightgbm_titanic_hyper.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/mnist_mlmodels_.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/mnist_mlmodels_.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/randomforest_titanic.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/randomforest_titanic.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest_example2.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_randomForest_example2.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/sklearn_titanic_svm.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow_1_lstm.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/tensorflow__lstm_json.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/tensorflow__lstm_json.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/timeseries_m5_deepar.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/timeseries_m5_deepar.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vision_mnist.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vision_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vision_mnist.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vision_mnist.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/example/vison_fashion_MNIST.ipynb` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/example/vison_fashion_MNIST.ipynb`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/metrics.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/metrics.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/README.md` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/README.md`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/fb_prophet.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/fb_prophet.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_automl.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_automl.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_automl.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_automl.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluon_prophet.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluon_prophet.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar_dloader.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_deepar_dloader.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/gluonts_model_old.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/gluonts_model_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/util.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_gluon/util_autogluon.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_gluon/util_autogluon.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/Autokeras.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/Autokeras.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/Autokeras.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/Autokeras.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/armdn.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/armdn.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/armdn.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/armdn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/charcnn_zhang.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/deep_ctr.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/deep_ctr.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/deepctr.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/deepctr.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/namentity_crm_bilstm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/preprocess.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/preprocess.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/textcnn.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/textcnn.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/textcnn.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/textcnn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_keras/util.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_keras/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/matchZoo.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/matchZoo.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/textcnn.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/textcnn.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/textcnn.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/textcnn.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/torchhub.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/torchhub.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/torchhub_cnn_dataloader.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/torchhub_cnn_dataloader.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/transformer_sentence.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/transformer_sentence.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/transformer_sentence.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/transformer_sentence.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/util_data.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/util_data.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tch/util_transformer.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tch/util_transformer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/1_lstm.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/1_lstm.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/1_lstm.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/1_lstm.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/model_tf/util.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/model_tf/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/models.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/models.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/optim.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/optim.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/pipeline.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/pipeline.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/generic.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/generic.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/generic_old.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/generic_old.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/image.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/image.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/tabular_keras.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/tabular_keras.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/template_data_pars.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/template_data_pars.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/text_keras.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/text_keras.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/text_torch.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/text_torch.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/timeseries.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/timeseries.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocess/ztemp.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocess/ztemp.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/preprocessor.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/preprocessor.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/00_template_keras.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/00_template_keras.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/model_xxx.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/model_xxx.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/models_config.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/models_config.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/optim_config.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/optim_config.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/template/optim_config_prune.json` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/template/optim_config_prune.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/util.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/util.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/util_json.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/util_json.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/util_log.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/util_log.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/bayesian.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/bayesian.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/model_v1.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/model_v1.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/parse.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/parse.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/predict.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/predict.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/test_dataloader.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/train.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/train.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/utils/ztest_structure.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/utils/ztest_structure.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/mlmodels/ztest.py` & `utilmy-0.1.16830011/utilmy/zzml/mlmodels/ztest.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/pullrequest/aa_mycode_test.py` & `utilmy-0.1.16830011/utilmy/zzml/pullrequest/aa_mycode_test.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/pullrequest/pullrequest.json` & `utilmy-0.1.16830011/utilmy/zzml/pullrequest/pullrequest.json`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/pylintrc` & `utilmy-0.1.16830011/utilmy/zzml/pylintrc`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/setup.cfg` & `utilmy-0.1.16830011/utilmy/zzml/setup.cfg`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/setup.py` & `utilmy-0.1.16830011/utilmy/zzml/setup.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy/zzml/versioneer.py` & `utilmy-0.1.16830011/utilmy/zzml/versioneer.py`

 * *Files identical despite different names*

### Comparing `utilmy-0.1.16802704/utilmy.egg-info/PKG-INFO` & `utilmy-0.1.16830011/utilmy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilmy
-Version: 0.1.16802704
+Version: 0.1.16830011
 Summary: utils
 Author: Nono
 Keywords: utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -35,11 +35,11 @@
 
    https://groups.google.com/g/utilmy
 
 
 
 
 Hash:
-18e1c29368c22c166691762ccb195e5b88ee2378
+623885c267bb56b48921abbba325f4bb4a9cb13f
 
 
 ```
```

### Comparing `utilmy-0.1.16802704/utilmy.egg-info/SOURCES.txt` & `utilmy-0.1.16830011/utilmy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

