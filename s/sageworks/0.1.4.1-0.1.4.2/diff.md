# Comparing `tmp/sageworks-0.1.4.1.tar.gz` & `tmp/sageworks-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.4.1.tar", last modified: Sun Apr 23 23:38:24 2023, max compression
+gzip compressed data, was "sageworks-0.1.4.2.tar", last modified: Tue May  2 13:24:45 2023, max compression
```

## Comparing `sageworks-0.1.4.1.tar` & `sageworks-0.1.4.2.tar`

### file list

```diff
@@ -1,266 +1,270 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.186098 sageworks-0.1.4.1/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.125592 sageworks-0.1.4.1/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.4.1/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.4.1/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.4.1/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.4.1/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1385 2023-04-20 18:56:17.000000 sageworks-0.1.4.1/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     5902 2023-04-23 23:38:24.186185 sageworks-0.1.4.1/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     5163 2023-04-15 19:49:43.000000 sageworks-0.1.4.1/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.4.1/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.119883 sageworks-0.1.4.1/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.125777 sageworks-0.1.4.1/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.126453 sageworks-0.1.4.1/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12208 2023-04-07 02:17:27.000000 sageworks-0.1.4.1/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.4.1/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1066 2023-04-07 21:10:26.000000 sageworks-0.1.4.1/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.127837 sageworks-0.1.4.1/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.128955 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)      928 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      904 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      928 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1776 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4717 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.129430 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     1620 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1413 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     1510 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.130513 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     1288 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2023-04-09 22:27:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2517 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.131082 sageworks-0.1.4.1/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2140 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.131818 sageworks-0.1.4.1/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.132317 sageworks-0.1.4.1/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.4.1/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.4.1/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2500 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133090 sageworks-0.1.4.1/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.4.1/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.4.1/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.4.1/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133322 sageworks-0.1.4.1/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.4.1/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133865 sageworks-0.1.4.1/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3926 2023-04-22 20:31:36.000000 sageworks-0.1.4.1/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-22 20:11:28.000000 sageworks-0.1.4.1/aws_setup/aws_account_check_deep.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.135629 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      960 2023-04-20 18:09:55.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/README.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2023-04-20 17:46:12.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.135957 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      503 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/sageworks_sandbox_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136237 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136418 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      549 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136726 sageworks-0.1.4.1/config/
--rw-r--r--   0 briford    (501) staff       (20)      148 2023-04-13 17:23:15.000000 sageworks-0.1.4.1/config/sageworks_config.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.138328 sageworks-0.1.4.1/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.4.1/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      613 2023-04-18 16:23:14.000000 sageworks-0.1.4.1/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.4.1/data/test_data.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.139164 sageworks-0.1.4.1/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.4.1/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.145110 sageworks-0.1.4.1/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.4.1/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.4.1/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.4.1/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.4.1/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.4.1/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.4.1/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.4.1/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.4.1/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.4.1/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.4.1/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.4.1/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.4.1/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.4.1/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.145901 sageworks-0.1.4.1/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/examples/data_to_data_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.146230 sageworks-0.1.4.1/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   236764 2023-04-20 18:57:28.000000 sageworks-0.1.4.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.152342 sageworks-0.1.4.1/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.4.1/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.4.1/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.4.1/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.4.1/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.4.1/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.4.1/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      173 2023-04-17 20:59:36.000000 sageworks-0.1.4.1/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.153321 sageworks-0.1.4.1/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1533 2023-04-23 22:12:54.000000 sageworks-0.1.4.1/scripts/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-04-23 23:38:24.186503 sageworks-0.1.4.1/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1772 2023-04-23 23:38:12.000000 sageworks-0.1.4.1/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.120819 sageworks-0.1.4.1/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.153493 sageworks-0.1.4.1/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.4.1/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154218 sageworks-0.1.4.1/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121028 sageworks-0.1.4.1/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154302 sageworks-0.1.4.1/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.4.1/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154521 sageworks-0.1.4.1/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.4.1/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121187 sageworks-0.1.4.1/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154743 sageworks-0.1.4.1/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.155642 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.156284 sageworks-0.1.4.1/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.4.1/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.4.1/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4542 2023-04-19 17:15:47.000000 sageworks-0.1.4.1/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157134 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7447 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2000 2023-04-19 17:23:07.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     1625 2023-04-19 17:34:03.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/data_source_abstract.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157450 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9826 2023-04-19 16:14:58.000000 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157781 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    11500 2023-04-19 16:37:35.000000 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.158138 sageworks-0.1.4.1/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4288 2023-04-19 16:37:35.000000 sageworks-0.1.4.1/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.158631 sageworks-0.1.4.1/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     6953 2023-04-14 22:13:26.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     7200 2023-04-17 17:05:59.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.168627 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-14 17:50:25.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
--rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2574 2023-04-22 20:48:49.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.171275 sageworks-0.1.4.1/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.4.1/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121799 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.171573 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     3841 2023-04-23 23:15:11.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172302 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4140 2023-04-18 20:16:32.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172682 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172778 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172867 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173132 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173677 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173939 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174057 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174172 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174459 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175161 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2585 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175448 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.122746 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175571 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175817 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.176111 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.176643 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.177002 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.178346 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     7073 2023-04-19 22:49:17.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)     9472 2023-04-19 16:44:04.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5439 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.180455 sageworks-0.1.4.1/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.4.1/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3961 2023-04-04 03:03:27.000000 sageworks-0.1.4.1/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.4.1/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     6168 2023-04-11 20:47:59.000000 sageworks-0.1.4.1/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_config.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_sqs.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.180894 sageworks-0.1.4.1/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)    12080 2023-04-19 17:03:51.000000 sageworks-0.1.4.1/src/sageworks/views/artifacts_summary.py
--rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.182980 sageworks-0.1.4.1/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      731 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.4.1/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.4.1/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1808 2023-04-07 15:59:10.000000 sageworks-0.1.4.1/src/sageworks/web_components/table.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154122 sageworks-0.1.4.1/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     5902 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     8651 2023-04-23 23:38:24.000000 sageworks-0.1.4.1/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)      124 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.183230 sageworks-0.1.4.1/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.184282 sageworks-0.1.4.1/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1169 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.4.1/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1095 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.184713 sageworks-0.1.4.1/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      347 2023-04-12 21:35:42.000000 sageworks-0.1.4.1/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      682 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.4.1/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.185813 sageworks-0.1.4.1/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.4.1/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      729 2023-04-13 21:22:54.000000 sageworks-0.1.4.1/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.853603 sageworks-0.1.4.2/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.803236 sageworks-0.1.4.2/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.4.2/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.4.2/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.4.2/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.4.2/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     5684 2023-05-02 13:24:45.853702 sageworks-0.1.4.2/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     4951 2023-05-01 19:54:07.000000 sageworks-0.1.4.2/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.4.2/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.797248 sageworks-0.1.4.2/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.803407 sageworks-0.1.4.2/applications/aws_dashboard/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.803785 sageworks-0.1.4.2/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.4.2/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     1066 2023-04-29 19:22:53.000000 sageworks-0.1.4.2/applications/aws_dashboard/aws_dashboard.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.804444 sageworks-0.1.4.2/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.805039 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/
+-rw-r--r--   0 briford    (501) staff       (20)     4046 2023-05-01 19:42:38.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      914 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      938 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1786 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/main_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4722 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.805262 sageworks-0.1.4.2/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     2350 2023-05-02 13:17:43.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)     1423 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     1520 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/feature_sets.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.805919 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/
+-rw-r--r--   0 briford    (501) staff       (20)     1366 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/data_sources_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/endpoints_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/feature_sets_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/main_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2341 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/models_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2111 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/main.py
+-rw-r--r--   0 briford    (501) staff       (20)     2535 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/aws_dashboard/pages/models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.806622 sageworks-0.1.4.2/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2158 2023-05-01 19:48:59.000000 sageworks-0.1.4.2/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.807343 sageworks-0.1.4.2/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.807848 sageworks-0.1.4.2/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.4.2/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.4.2/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2500 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.808536 sageworks-0.1.4.2/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.4.2/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.4.2/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.4.2/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.808750 sageworks-0.1.4.2/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.4.2/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.809147 sageworks-0.1.4.2/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3315 2023-04-30 02:51:12.000000 sageworks-0.1.4.2/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     4010 2023-04-30 03:07:40.000000 sageworks-0.1.4.2/aws_setup/aws_account_check_deep.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.810854 sageworks-0.1.4.2/aws_setup/sageworks_cdk/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.811164 sageworks-0.1.4.2/aws_setup/sageworks_cdk/stacks/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/stacks/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2402 2023-04-30 18:00:46.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.811390 sageworks-0.1.4.2/aws_setup/sageworks_cdk/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.811565 sageworks-0.1.4.2/aws_setup/sageworks_cdk/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.4.2/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.811811 sageworks-0.1.4.2/config/
+-rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.4.2/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.813140 sageworks-0.1.4.2/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.4.2/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)      613 2023-04-18 16:23:14.000000 sageworks-0.1.4.2/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.4.2/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.814076 sageworks-0.1.4.2/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.4.2/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.819680 sageworks-0.1.4.2/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.4.2/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.4.2/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.4.2/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.4.2/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.4.2/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.4.2/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.4.2/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.4.2/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.4.2/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.4.2/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.4.2/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.4.2/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.4.2/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.820477 sageworks-0.1.4.2/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.820814 sageworks-0.1.4.2/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236764 2023-04-20 18:57:28.000000 sageworks-0.1.4.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.825394 sageworks-0.1.4.2/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.4.2/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.4.2/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.4.2/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.4.2/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.4.2/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.4.2/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.4.2/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.829290 sageworks-0.1.4.2/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)     1716 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-02 13:24:45.854022 sageworks-0.1.4.2/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1766 2023-05-02 13:24:38.000000 sageworks-0.1.4.2/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.798453 sageworks-0.1.4.2/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.829600 sageworks-0.1.4.2/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.4.2/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.830592 sageworks-0.1.4.2/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.798702 sageworks-0.1.4.2/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.830688 sageworks-0.1.4.2/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.4.2/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.830913 sageworks-0.1.4.2/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.4.2/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.798873 sageworks-0.1.4.2/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.831142 sageworks-0.1.4.2/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.4.2/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.832181 sageworks-0.1.4.2/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.4.2/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.4.2/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.832718 sageworks-0.1.4.2/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.4.2/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.4.2/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4567 2023-04-30 15:25:18.000000 sageworks-0.1.4.2/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.833617 sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8473 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2534 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     1783 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.833837 sageworks-0.1.4.2/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9826 2023-04-19 16:14:58.000000 sageworks-0.1.4.2/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.834186 sageworks-0.1.4.2/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    11500 2023-04-19 16:37:35.000000 sageworks-0.1.4.2/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.834630 sageworks-0.1.4.2/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4288 2023-04-19 16:37:35.000000 sageworks-0.1.4.2/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.835366 sageworks-0.1.4.2/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     7591 2023-04-30 17:35:38.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     7426 2023-04-30 02:50:10.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.837611 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4187 2023-04-30 18:15:05.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     2589 2023-04-30 02:50:10.000000 sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.838240 sageworks-0.1.4.2/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.4.2/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.799511 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.838578 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     5597 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.839230 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.839526 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.839618 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.839702 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.839973 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.840502 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.840783 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.840949 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5918 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.841079 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.841299 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.842004 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2585 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.842234 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.800295 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.842329 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.842568 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.842837 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.843449 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.843800 sageworks-0.1.4.2/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.2/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.845124 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7073 2023-04-19 22:49:17.000000 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     9472 2023-04-19 16:44:04.000000 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5464 2023-04-30 02:50:10.000000 sageworks-0.1.4.2/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.847095 sageworks-0.1.4.2/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.4.2/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.4.2/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6563 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.4.2/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.4.2/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.4.2/src/sageworks/utils/sageworks_sqs.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.848053 sageworks-0.1.4.2/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     9429 2023-05-02 13:13:09.000000 sageworks-0.1.4.2/src/sageworks/views/artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.4.2/src/sageworks/views/view.py
+-rw-r--r--   0 briford    (501) staff       (20)    12557 2023-05-02 13:17:43.000000 sageworks-0.1.4.2/src/sageworks/views/web_artifacts_summary.py
+-rw-r--r--   0 briford    (501) staff       (20)     5649 2023-05-01 19:53:31.000000 sageworks-0.1.4.2/src/sageworks/views/web_data_source_view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.850405 sageworks-0.1.4.2/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1335 2023-04-30 15:51:43.000000 sageworks-0.1.4.2/src/sageworks/web_components/box_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.4.2/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/web_components/feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.4.2/src/sageworks/web_components/feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.4.2/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.4.2/src/sageworks/web_components/model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.4.2/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.4.2/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2116 2023-04-30 02:31:13.000000 sageworks-0.1.4.2/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1920 2023-04-30 00:05:24.000000 sageworks-0.1.4.2/src/sageworks/web_components/violin_plot.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.830484 sageworks-0.1.4.2/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     5684 2023-05-02 13:24:45.000000 sageworks-0.1.4.2/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     8772 2023-05-02 13:24:45.000000 sageworks-0.1.4.2/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-02 13:24:45.000000 sageworks-0.1.4.2/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)      124 2023-05-02 13:24:45.000000 sageworks-0.1.4.2/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-02 13:24:45.000000 sageworks-0.1.4.2/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.850744 sageworks-0.1.4.2/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.851849 sageworks-0.1.4.2/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1169 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.4.2/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1095 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.852316 sageworks-0.1.4.2/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      347 2023-04-12 21:35:42.000000 sageworks-0.1.4.2/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      682 2023-04-02 18:05:33.000000 sageworks-0.1.4.2/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.4.2/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-02 13:24:45.853288 sageworks-0.1.4.2/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.4.2/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.4.2/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-04-13 21:22:54.000000 sageworks-0.1.4.2/tox.ini
```

### Comparing `sageworks-0.1.4.1/.gitignore` & `sageworks-0.1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/LICENSE` & `sageworks-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/Makefile` & `sageworks-0.1.4.2/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 clean: clean-build clean-pyc clean-misc
 
 clean-build:
 	find . -name 'build' -exec rm -rf {} +
 	find . -name '_build' -exec rm -rf {} +
 	find . -name 'dist' -exec rm -rf {} +
 	find . -name '*.egg-info' -exec rm -rf {} +
+	find . -name '*.eggs' -exec rm -rf {} +
 	find . -name '*.tar.gz' -exec rm -rf {} +
 	find . -name '.tox' -exec rm -rf {} +
 	find . -name '.coverage' -exec rm -rf {} +
 	find . -name '.cache' -exec rm -rf {} +
 	find . -name '__pycache__' -exec rm -rf {} +
 
 clean-pyc:
```

### Comparing `sageworks-0.1.4.1/PKG-INFO` & `sageworks-0.1.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.4.1
-Summary: SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models
+Version: 0.1.4.2
+Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -48,22 +48,19 @@
 <img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
-- [Initial Setup and Installation](https://github.com/SuperCowPowers/sageworks/wiki/Initial-Setup-and-Installation) for initial AWS/config/repository set up. 
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
-- [Coding with SageWorks Video](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
+- [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-### SageWorks Analysis Notebooks
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from Start to Finish
-
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
 - SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
 - **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
 - **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
 - Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
 - **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
@@ -76,10 +73,10 @@
 
 
 ### SageWorks Alpha Testers Wanted
 Our experienced team can provide development and consulting services to help you effectively use Amazon’s Machine Learning services within your organization.
 
 The popularity of cloud based Machine Learning services is booming. The problem many companies face is how that capability gets effectively used and harnessed to drive real business decisions and provide concrete value for their organization.
 
-Using SageWorks will minimizize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
```

### Comparing `sageworks-0.1.4.1/Readme.md` & `sageworks-0.1.4.2/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,22 +30,19 @@
 <img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
-- [Initial Setup and Installation](https://github.com/SuperCowPowers/sageworks/wiki/Initial-Setup-and-Installation) for initial AWS/config/repository set up. 
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
-- [Coding with SageWorks Video](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
+- [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-### SageWorks Analysis Notebooks
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from Start to Finish
-
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
 - SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
 - **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
 - **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
 - Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
 - **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
@@ -58,10 +55,10 @@
 
 
 ### SageWorks Alpha Testers Wanted
 Our experienced team can provide development and consulting services to help you effectively use Amazon’s Machine Learning services within your organization.
 
 The popularity of cloud based Machine Learning services is booming. The problem many companies face is how that capability gets effectively used and harnessed to drive real business decisions and provide concrete value for their organization.
 
-Using SageWorks will minimizize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.4.2/applications/aws_dashboard/assets/custom.css`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,17 @@
 
 /* Typography
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 h1, h2, h3, h4, h5, h6 {
   margin-top: 0;
   margin-bottom: 0;
   font-weight: 300; }
-h1 { font-size: 4.5rem; line-height: 1.2;  letter-spacing: -.1rem; margin-bottom: 0rem; }
-h2 { font-size: 3.6rem; line-height: 1.25; letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.8rem;}
-h3 { font-size: 3.0rem; line-height: 1.3;  letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.5rem;}
+h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem; margin-bottom: 0rem; }
+h2 { font-size: 3.3rem; line-height: 1.25; letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.8rem;}
+h3 { font-size: 2.7rem; line-height: 1.3;  letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.5rem;}
 h4 { font-size: 2.6rem; line-height: 1.35; letter-spacing: -.08rem; margin-bottom: 0rem; margin-top: 1.2rem;}
 h5 { font-size: 2.2rem; line-height: 1.5;  letter-spacing: -.05rem; margin-bottom: 0rem; margin-top: 0.6rem;}
 h6 { font-size: 2.0rem; line-height: 1.6;  letter-spacing: 0; margin-bottom: 0.75rem; margin-top: 0.75rem;}
 
 p {
   margin-top: 0; }
 
@@ -320,17 +320,20 @@
 li {
   margin-bottom: 1rem; }
 
 
 /* Tables
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 table {
-  border: 3px solid #222222;
+  border: 4px solid #222222;
   border-collapse: collapse;
 }
+tr {
+  border: 1px solid #666666;
+}
 th:not(.CalendarDay),
 td:not(.CalendarDay) {
   padding: 12px 15px;
   text-align: left;
   border-bottom: 1px solid #E1E1E1; }
 th:first-child:not(.CalendarDay),
 td:first-child:not(.CalendarDay) {
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.4.2/applications/aws_dashboard/aws_dashboard.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """FeatureSets Callbacks: Callback within the FeatureSets Web User Interface"""
 from datetime import datetime
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
     @app.callback(Output("last-updated-endpoints", "children"), Input("endpoints-updater", "n_intervals"))
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_endpoints_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
+def update_endpoints_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("ENDPOINTS_DETAILS", "data"), Input("endpoints-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
         sageworks_artifacts.refresh()
         endpoints = sageworks_artifacts.endpoints_summary()
         return endpoints.to_dict("records")
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """FeatureSets Callbacks: Callback within the FeatureSets Web User Interface"""
 from datetime import datetime
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
     @app.callback(Output("last-updated-feature-sets", "children"), Input("feature-sets-updater", "n_intervals"))
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_feature_sets_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
+def update_feature_sets_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("FEATURE_SETS_DETAILS", "data"), Input("feature-sets-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
         sageworks_artifacts.refresh()
         feature_sets = sageworks_artifacts.feature_sets_summary()
         return feature_sets.to_dict("records")
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/main_callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Callbacks/Connections in the Web User Interface"""
 from datetime import datetime
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 # Cheese Sauce
 all_data = None
 
 
-def update_last_updated(app: Dash, sageworks_artifacts: ArtifactsSummary):
+def update_last_updated(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("last-updated", "children"), Input("main-updater", "n_intervals"))
     def time_updated(n):
         global all_data
         print("Calling ALL Artifact Refresh...")
         sageworks_artifacts.refresh()
         all_data = sageworks_artifacts.view_data()
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from dash import Dash
 from dash.dependencies import Input, Output
 from datetime import datetime
 
 # SageWorks Imports
 from sageworks.web_components.model_data import ModelData
 from sageworks.web_components import feature_importance, confusion_matrix, model_details, feature_details
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 
 def update_last_updated(app: Dash):
     @app.callback(Output("last-updated-models", "children"), Input("models-updater", "n_intervals"))
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_models_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
+def update_models_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
     @app.callback(Output("models_table", "data"), Input("models-updater", "n_intervals"))
     def data_sources_update(n):
-        print("Calling DataSources Refresh...")
+        print("Calling Models Refresh...")
         sageworks_artifacts.refresh()
         models = sageworks_artifacts.models_summary()
         return models.to_dict("records")
 
 
 # Highlights the selected row in the table
 def table_row_select(app: Dash, table_name: str):
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Endpoints:  A SageWorks Web Interface to view, interact, and manage Endpoints"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
 from sageworks.web_components import line_chart
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.endpoints_layout import endpoints_layout
 import pages.callbacks.endpoints_callbacks as callbacks
 
 register_page(__name__, path="/endpoints")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-sageworks_artifacts = ArtifactsSummary()
+sageworks_artifacts = WebArtifactsSummary()
 endpoints_summary = sageworks_artifacts.endpoints_summary()
 
 # Create a table to display the feature sets
 endpoints_table = table.create(
     "ENDPOINTS_DETAILS",
     endpoints_summary,
     header_color="rgb(100, 60, 100)",
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/feature_sets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """DataSources:  A SageWorks Web Interface to view, interact, and manage Data Sources"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
 from sageworks.web_components import scatter_plot
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.feature_sets_layout import feature_sets_layout
 import pages.callbacks.feature_sets_callbacks as callbacks
 
 register_page(__name__, path="/feature_sets")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-sageworks_artifacts = ArtifactsSummary()
+sageworks_artifacts = WebArtifactsSummary()
 feature_sets_summary = sageworks_artifacts.feature_sets_summary()
 
 # Create a table to display the feature sets
 feature_sets_table = table.create(
     "FEATURE_SETS_DETAILS",
     feature_sets_summary,
     header_color="rgb(100, 100, 60)",
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/feature_sets_layout.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""DataSources Layout: Layout for the DataSources page in the Artifact Viewer"""
+"""FeatureSets Layout: Layout for the FeatureSets page in the Artifact Viewer"""
 from dash import html, dcc
 import dash_bootstrap_components as dbc
 
 
-def data_sources_layout(components: dict) -> html.Div:
+def feature_sets_layout(components: dict) -> html.Div:
     # Just put all the tables in as Rows for Now (do something fancy later)
     layout = html.Div(
         children=[
             dbc.Row(
                 [
-                    html.H2("SageWorks: DataSources (Alpha)"),
+                    html.H2("SageWorks: FeatureSets (Alpha)"),
                     html.Div(
                         "Last Updated: ",
-                        id="last-updated-data-sources",
+                        id="last-updated-feature-sets",
                         style={
                             "color": "rgb(140, 200, 140)",
                             "fontSize": 15,
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
-            dbc.Row(components["data_sources_details"]),
+            dbc.Row(components["feature_sets_details"]),
             dbc.Row(
                 [
-                    dbc.Col(components["histo_plot"]),
-                    dbc.Col(components["box_plot"]),
+                    dbc.Col(components["scatter1"]),
+                    dbc.Col(components["scatter2"]),
                 ]
             ),
-            dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
+            dcc.Interval(id="feature-sets-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/endpoints_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/data_sources_layout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-"""FeatureSets Layout: Layout for the FeatureSets page in the Artifact Viewer"""
+"""DataSources Layout: Layout for the DataSources page in the Artifact Viewer"""
 from dash import html, dcc
 import dash_bootstrap_components as dbc
 
 
-def feature_sets_layout(components: dict) -> html.Div:
+def data_sources_layout(components: dict) -> html.Div:
     # Just put all the tables in as Rows for Now (do something fancy later)
     layout = html.Div(
         children=[
             dbc.Row(
                 [
-                    html.H2("SageWorks: FeatureSets (Alpha)"),
+                    html.H2("SageWorks: DataSources (Alpha)"),
                     html.Div(
                         "Last Updated: ",
-                        id="last-updated-feature-sets",
+                        id="last-updated-data-sources",
                         style={
                             "color": "rgb(140, 200, 140)",
                             "fontSize": 15,
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
-            dbc.Row(components["feature_sets_details"]),
-            dbc.Row(
-                [
-                    dbc.Col(components["scatter1"]),
-                    dbc.Col(components["scatter2"]),
-                ]
-            ),
-            dcc.Interval(id="feature-sets-updater", interval=5000, n_intervals=0),
+            dbc.Row(components["data_sources_summary"]),
+            dbc.Row(html.H3("Sampled Rows", id="sample_rows_header"), style={"padding": "30px 0px 10px 0px"}),
+            dbc.Row(components["data_source_sample_rows"], style={"padding": "0px 0px 30px 0px"}),
+            dbc.Row(components["violin_plot"]),
+            dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/main_layout.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/main_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/layout/models_layout.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
                 id="last-updated-models",
                 style={
                     "color": "rgb(140, 200, 140)",
                     "fontSize": 15,
                     "padding": "0px 0px 0px 160px",
                 },
             ),
-            dcc.Interval(id="models-updater", interval=5000, n_intervals=0),
             dbc.Row(style={"padding": "30px 0px 0px 0px"}),
             dbc.Row(
                 [
                     # Model Table and Model Details
                     dbc.Col(
                         [
                             dbc.Row(components["models_table"]),
@@ -51,11 +50,12 @@
                             ),
                             dbc.Row(components["feature_details"], style={"padding": "0px 0px 0px 20px"}),
                         ],
                         width=4,
                     ),
                 ]
             ),
+            dcc.Interval(id="models-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/main.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Main: The main SageWorks Web Interface to view, interact, and manage SageWorks Artifacts"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.main_layout import main_layout
 import pages.callbacks.main_callbacks as callbacks
 
 register_page(__name__, path="/")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-artifacts_summary = ArtifactsSummary()
-sageworks_artifacts = artifacts_summary.view_data()
+web_artifacts_summary = WebArtifactsSummary()
+sageworks_artifacts = web_artifacts_summary.view_data()
 
 # Grab the Artifact Information DataFrame for each AWS Service and pass it to the table creation
 tables = dict()
 tables["INCOMING_DATA"] = table.create(
     "INCOMING_DATA",
     sageworks_artifacts["INCOMING_DATA"],
     header_color="rgb(60, 60, 100)",
@@ -55,12 +55,12 @@
     "feature_sets": tables["FEATURE_SETS"],
     "models": tables["MODELS"],
     "endpoints": tables["ENDPOINTS"],
 }
 
 # Setup our callbacks/connections
 app = dash.get_app()
-callbacks.update_last_updated(app, artifacts_summary)
+callbacks.update_last_updated(app, web_artifacts_summary)
 callbacks.update_artifact_tables(app)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = main_layout(components)
```

### Comparing `sageworks-0.1.4.1/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.4.2/applications/aws_dashboard/pages/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from dash_bootstrap_templates import load_figure_template
 
 
 # SageWorks Imports
 
 from sageworks.web_components import confusion_matrix, table, scatter_plot
 from sageworks.web_components import feature_importance, model_data, model_details, feature_details
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 
 # Local Imports
 from pages.layout.models_layout import models_layout
 import pages.callbacks.models_callbacks as callbacks
 
 register_page(__name__, path="/models")
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-artifacts_summary = ArtifactsSummary()
-models_summary = artifacts_summary.models_summary(concise=True)
+web_artifacts_summary = WebArtifactsSummary()
+models_summary = web_artifacts_summary.models_summary(concise=True)
 
 # Read in our fake model data
 data_path = os.path.join(os.path.dirname(__file__), "data/toy_data.csv")
 fake_model_info = model_data.ModelData(data_path)
 
 # Create a table to display the models
 models_table = table.create(
```

### Comparing `sageworks-0.1.4.1/applications/hello_world/callbacks.py` & `sageworks-0.1.4.2/applications/hello_world/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/hello_world/hello_world.py` & `sageworks-0.1.4.2/applications/hello_world/hello_world.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """HelloWorld: A SageWorks HelloWorld Application"""
 from dash import Dash
 import dash_bootstrap_components as dbc
 
 
 # SageWorks Imports
-from sageworks.views.artifacts_summary import ArtifactsSummary
+from sageworks.views.web_artifacts_summary import WebArtifactsSummary
 from sageworks.web_components import table
 
 
 # Local Imports
 import layout
 
 
@@ -22,20 +22,20 @@
 
 
 def setup_artifact_viewer():
     # Set Default Template for figures
     # load_figure_template('darkly')
 
     # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-    sageworks_artifacts = ArtifactsSummary()
-    artifacts_summary = sageworks_artifacts.view_data()
+    sageworks_artifacts = WebArtifactsSummary()
+    web_artifacts_summary = sageworks_artifacts.view_data()
 
     # Just a bunch of tables for now :)
     tables = {}
-    for service_category, artifact_info_df in artifacts_summary.items():
+    for service_category, artifact_info_df in web_artifacts_summary.items():
         # Grab the Artifact Information DataFrame for each AWS Service
         tables[service_category] = table.create(service_category, artifact_info_df)
 
     # Create our components
     components = {
         "incoming_data": tables["INCOMING_DATA"],
         "data_sources": tables["DATA_SOURCES"],
```

### Comparing `sageworks-0.1.4.1/applications/hello_world/layout.py` & `sageworks-0.1.4.2/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/model_viewer/callbacks.py` & `sageworks-0.1.4.2/applications/model_viewer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.4.2/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.4.2/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/model_viewer/layout.py` & `sageworks-0.1.4.2/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/applications/model_viewer/model_viewer.py` & `sageworks-0.1.4.2/applications/model_viewer/model_viewer.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/aws_setup/aws_account_check_deep.py` & `sageworks-0.1.4.2/tests/create_sageworks_objs_for_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/aws_setup/sageworks_sandbox/README.md` & `sageworks-0.1.4.2/aws_setup/sageworks_cdk/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SageWorks Sandbox AWS Deployment
 
 To run/deploy the SageWorks AWS Sandbox you'll need install a couple of Python packages
-either in a Python VirtualENV of your choice (PyENV is good) or any Python3 will do
+either in a Python VirtualENV of your choice (PyENV is good) or any Python3 will do. You'll also need to use a newer version of node such as node v19.6
 
 ```
 $ pip install -r requirements.txt
 ```
 
 At this point you can now synthesize the CloudFormation template and deploy the SageWorks Sandbox AWS Components.
```

### Comparing `sageworks-0.1.4.1/aws_setup/sageworks_sandbox/cdk.json` & `sageworks-0.1.4.2/aws_setup/sageworks_cdk/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/data/abalone.csv` & `sageworks-0.1.4.2/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/data/test_data.csv` & `sageworks-0.1.4.2/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/data/test_data.json` & `sageworks-0.1.4.2/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/admin_notes.md` & `sageworks-0.1.4.2/docs/admin_notes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/big_spider.png` & `sageworks-0.1.4.2/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/graph_representation.png` & `sageworks-0.1.4.2/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.4.2/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/powered_aws_transparent.png` & `sageworks-0.1.4.2/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/powered_aws_white.png` & `sageworks-0.1.4.2/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.4.2/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/sageworks.png` & `sageworks-0.1.4.2/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/sageworks_concepts.png` & `sageworks-0.1.4.2/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/scp.png` & `sageworks-0.1.4.2/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/scp_labs.png` & `sageworks-0.1.4.2/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/images/small_spider.png` & `sageworks-0.1.4.2/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/sageworks_classes_concepts.md` & `sageworks-0.1.4.2/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/docs/scp_consulting.md` & `sageworks-0.1.4.2/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/examples/data_to_data_example.py` & `sageworks-0.1.4.2/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.1.4.2/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/athena_query_aqsol.png` & `sageworks-0.1.4.2/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.1.4.2/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.1.4.2/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/model_screenshot.png` & `sageworks-0.1.4.2/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/sageworks_concepts.png` & `sageworks-0.1.4.2/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/notebooks/images/scp_labs.png` & `sageworks-0.1.4.2/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/scripts/data_source_tags.py` & `sageworks-0.1.4.2/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/scripts/generate_jsonl_data.py` & `sageworks-0.1.4.2/scripts/generate_jsonl_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import json
 import boto3
 import random
 import string
 import gzip
 import os
+from datetime import datetime, timezone
+
+# SageWorks Imports
+from sageworks.utils.iso_8601 import datetime_to_iso8601
 
 # Set up S3 client
-s3 = boto3.client('s3')
+s3 = boto3.client("s3")
 
 # Set up some variables
 num_files = 10  # Number of files to create
 num_records_per_file = 1000  # Number of records to create in each file
 
 
 # Define a function to generate random data
 def generate_data():
     return {
-        'id': ''.join(random.choices(string.ascii_letters + string.digits, k=8)),
-        'name': ''.join(random.choices(string.ascii_letters, k=10)),
-        'age': random.randint(18, 65),
-        'address': ''.join(random.choices(string.ascii_letters + string.digits + ', .', k=20))
+        "id": "".join(random.choices(string.ascii_letters + string.digits, k=8)),
+        "name": "".join(random.choices(string.ascii_letters, k=10)),
+        "age": random.randint(18, 65),
+        "address": "".join(random.choices(string.ascii_letters + string.digits + ", .", k=20)),
+        "date": datetime_to_iso8601(datetime.now(timezone.utc))
     }
 
 
 # Loop through and generate the files
 for i in range(num_files):
     # Set up the file name
-    filename = f'data_{i}.jsonl'
+    filename = f"data_{i}.jsonl"
     print(filename)
 
     # Generate the records
     records = []
     for j in range(num_records_per_file):
         records.append(generate_data())
 
     # Write the records to the file in JSONL format
-    with open(filename, 'w') as f:
+    with open(filename, "w") as f:
         for record in records:
-            f.write(json.dumps(record) + '\n')
+            f.write(json.dumps(record) + "\n")
 
     # Compress the file and save as gzipped file
-    with open(filename, 'rb') as f_in:
-        with gzip.open(f'{filename}.gz', 'wb') as f_out:
+    with open(filename, "rb") as f_in:
+        with gzip.open(f"{filename}.gz", "wb") as f_out:
             f_out.writelines(f_in)
 
     # Upload the file to S3
     s3_file_path = f"incoming-data/jsonl-data/{filename}.gz"
-    s3.upload_file(f'{filename}.gz', 'scp-sageworks-artifacts', s3_file_path)
+    s3.upload_file(f"{filename}.gz", "scp-sageworks-artifacts", s3_file_path)
 
     # Delete the local copy of the file
     os.remove(filename)
-    os.remove(f'{filename}.gz')
+    os.remove(f"{filename}.gz")
 
-print('Done!')
+print("Done!")
```

### Comparing `sageworks-0.1.4.1/scripts/list_data_sources.py` & `sageworks-0.1.4.2/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/setup.cfg` & `sageworks-0.1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/setup.py` & `sageworks-0.1.4.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.4.1",
-    description="SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models",
+    version="0.1.4.2",
+    description="SageWorks: A Python WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `sageworks-0.1.4.1/src/sageworks/__init__.py` & `sageworks-0.1.4.2/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.4.2/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.4.2/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.4.2/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.4.2/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     # AWSServiceBroker pulls and collects metadata from a bunch of AWS Services
     aws_broker = AWSServiceBroker()
 
     # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
     sageworks_config = SageWorksConfig()
     data_catalog_db = "sageworks"
-    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
-    data_source_s3_path = sageworks_bucket + "/data-sources"
-    feature_sets_s3_path = sageworks_bucket + "/feature-sets"
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+    data_source_s3_path = "s3://" + sageworks_bucket + "/data-sources"
+    feature_sets_s3_path = "s3://" + sageworks_bucket + "/feature-sets"
 
     def __init__(self, uuid):
         """Artifact Initialization"""
         self.uuid = uuid
         self.log = logging.getLogger(__name__)
 
     @abstractmethod
```

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/athena_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,14 +126,32 @@
     def athena_test_query(self):
         """Validate that Athena Queries are working"""
         query = f"select count(*) as count from {self.table_name}"
         df = wr.athena.read_sql_query(sql=query, database=self.data_catalog_db, boto3_session=self.boto_session)
         scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
         self.log.info(f"Athena TEST Query successful (scanned bytes: {scanned_bytes})")
 
+    def sample_df(self, max_rows: int = 1000) -> pd.DataFrame:
+        """Pull a sample of rows from the DataSource
+        Args:
+            max_rows (int): Maximum number of rows to pull
+        """
+        num_rows = self.num_rows()
+        if num_rows > max_rows:
+            # With Bernoulli Sampling it can give you 0 rows on small samples
+            # so we need to make sure we have at least 100 rows for the sample
+            # and then we can limit the output to max_rows
+            sample_rows = max(max_rows, 100)
+            percentage = min(100, round(sample_rows * 100.0 / num_rows))
+            self.log.warning(f"DataSource has {num_rows} rows.. sampling down to {max_rows}...")
+            query = f"SELECT * FROM {self.table_name} TABLESAMPLE BERNOULLI({percentage})"
+        else:
+            query = f"SELECT * FROM {self.table_name}"
+        return self.query(query).head(max_rows)
+
     def details(self) -> dict:
         """Additional Details about this AthenaSource Artifact"""
         details = super().details()
         details["s3_storage_location"] = self.s3_storage_location()
         return details
 
     def delete(self):
@@ -152,15 +170,15 @@
         wr.s3.delete_objects(self.s3_storage_location(), boto3_session=self.boto_session)
 
 
 if __name__ == "__main__":
     """Exercise the AthenaSource Class"""
 
     # Retrieve a Data Source
-    my_data = AthenaSource("test_data")
+    my_data = AthenaSource("abalone_data")
 
     # Verify that the Athena Data Source exists
     assert my_data.check()
 
     # What's my SageWorks UUID
     print(f"UUID: {my_data.uuid}")
 
@@ -182,10 +200,15 @@
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
     # Get Metadata and tags associated with this Artifact
     print(f"Meta: {my_data.sageworks_meta()}")
     print(f"Tags: {my_data.sageworks_tags()}")
 
+    # Get a sample of the data
+    df = my_data.sample_df(10)
+    print(f"Sample Data: {df.shape}")
+    print(df)
+
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
```

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/data_source_abstract.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/data_sources/data_source_abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         return {name: type_ for name, type_ in zip(self.column_names(), self.column_types())}
 
     @abstractmethod
     def query(self, query: str) -> pd.DataFrame:
         """Query the DataSourceAbstract"""
         pass
 
+    @abstractmethod
+    def sample_df(self, max_rows: int = 1000) -> pd.DataFrame:
+        """Return a sample DataFrame from this DataSource"""
+        pass
+
     def details(self) -> dict:
         """Additional Details about this DataSourceAbstract Artifact"""
         details = self.summary()
         details["num_rows"] = self.num_rows()
         details["num_columns"] = self.num_columns()
         details["column_details"] = self.column_details()
         return details
```

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/feature_set.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.4.2/src/sageworks/artifacts/models/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class AWSAccountClamp:
     def __init__(self):
         """AWSAccountClamp provides logic/functionality over a set of AWS IAM Services"""
         self.log = logging.getLogger(__file__)
 
         # Grab the AWS Role Name from the SageWorks Config
         config = SageWorksConfig()
-        role_name = config.get_config_value("SAGEWORKS_AWS", "SAGEWORKS_ROLE")
+        role_name = config.get_config_value("SAGEWORKS_AWS", "SAGEWORKS_ROLE_NAME")
         self.role_name = role_name
 
         # The default AWS Assume Role TTL is 1 hour, so we'll set our TTL to 50 minutes
         self.session_time_delta = timedelta(minutes=50)
 
     def check_aws_identity(self) -> bool:
         """Check the AWS Identity currently active"""
@@ -151,15 +151,31 @@
         """Get the AWS AccountID"""
         return self.boto_session().region_name
 
 
 if __name__ == "__main__":
     """Exercise the AWS Account Clamp Class"""
 
-    # Import the Check Class to test this class :)
-    from sageworks.aws_service_broker.aws_account_check import AWSAccountCheck
-
     # Create the class
-    aws_account_check = AWSAccountCheck()
+    aws_account_clamp = AWSAccountClamp()
 
-    # Check that out AWS Account Clamp is working AOK
-    aws_account_check.check()
+    # Check out that AWS Account Clamp is working AOK
+    """Check if the AWS Account is Setup Correctly"""
+    print("*** AWS Identity Check ***")
+    aws_account_clamp.check_aws_identity()
+    print("Identity Check Success...")
+
+    print("*** AWS Assume SageWorks ExecutionRole Check ***")
+    check_boto_session = aws_account_clamp.boto_session()
+    print("Assume Role Success...")
+
+    print("*** AWS App Config Check ***")
+    aws_account_clamp.check_app_config(check_boto_session)
+    print("App Config Check Success...")
+
+    print("*** AWS S3 Access Check ***")
+    aws_account_clamp.check_s3_access(check_boto_session)
+    print("S3 Access Check Success...")
+
+    print("*** AWS Sagemaker Session/Client Check ***")
+    sm_client = aws_account_clamp.sagemaker_client()
+    print(sm_client.list_feature_groups()["FeatureGroupSummaries"])
```

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import argparse
 from enum import Enum, auto
 import logging
 from threading import Thread
 
 # SageWorks Imports
+from sageworks.utils.cache import Cache
 from sageworks.utils.redis_cache import RedisCache
 from sageworks.aws_service_broker.aws_service_connectors.s3_bucket import S3Bucket
 from sageworks.aws_service_broker.aws_service_connectors.data_catalog import DataCatalog
 from sageworks.aws_service_broker.aws_service_connectors.feature_store import FeatureStore
 from sageworks.aws_service_broker.aws_service_connectors.model_registry import ModelRegistry
 from sageworks.aws_service_broker.aws_service_connectors.endpoints import Endpoints
 from sageworks.aws_service_broker.aws_service_connectors.artifact_info import ArtifactInfo
@@ -50,16 +51,16 @@
     @classmethod
     def __class_init__(cls, database_scope):
         """AWSServiceBroker pulls and collects metadata from a bunch of AWS Services"""
         cls.log = logging.getLogger(__file__)
 
         # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
         sageworks_config = SageWorksConfig()
-        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
-        cls.incoming_data_bucket = sageworks_bucket + "/incoming-data"
+        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+        cls.incoming_data_bucket = "s3://" + sageworks_bucket + "/incoming-data"
 
         # SageWorks category mapping to AWS Services
         # - incoming_data = S3
         # - data_sources = Data Catalog, Athena
         # - feature_sets = Data Catalog, Athena, Feature Store
         # - models = Model Registry
         # - endpoints = Sagemaker Endpoints, Model Monitors
@@ -70,18 +71,23 @@
         cls.feature_store = FeatureStore()
         cls.model_registry = ModelRegistry()
         cls.endpoints = Endpoints()
         cls.artifact_info = ArtifactInfo()
 
         # Model Monitors
 
-        # Redis Cache for Metadata
-        cls.meta_cache = RedisCache()
-        cls.fresh_cache = RedisCache(expire=10, postfix=":fresh")
-        cls.open_threads = []
+        # Cache for Metadata
+        if RedisCache().check():
+            cls.meta_cache = RedisCache()
+            cls.fresh_cache = RedisCache(expire=10, postfix=":fresh")
+            cls.open_threads = []
+        else:
+            cls.meta_cache = Cache()
+            cls.fresh_cache = Cache(expire=10)
+            cls.open_threads = []
 
         # This connection map sets up the connector objects for each category of metadata
         # Note: Even though this seems confusing, it makes other code WAY simpler
         cls.connection_map = {
             ServiceCategory.INCOMING_DATA: cls.incoming_data,
             ServiceCategory.DATA_CATALOG: cls.data_catalog,
             ServiceCategory.FEATURE_STORE: cls.feature_store,
```

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 aws_tags = self.sm_session.list_tags(aws_arn)
                 info = self._aws_tags_to_dict(aws_tags)
             except botocore.exceptions.ClientError as exc:
                 if exc.response["Error"]["Code"] == "ValidationException":
                     self.log.error(f"This method doesn't work on DataSources: {exc}")
                     return {}
                 else:
-                    self.log.crtical(f"Unknown Error: {exc}")
+                    self.log.critical(f"Unknown Error: {exc}")
                     raise exc
 
             # Set the artifact info cache
             self.artifact_info_cache.set(aws_arn, info)
         return info
 
     @staticmethod
```

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.4.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 if __name__ == "__main__":
     """Exercises the S3Bucket Class"""
     from pprint import pprint
     from sageworks.utils.sageworks_config import SageWorksConfig
 
     # Grab out incoming data bucket for something to test with
     sageworks_config = SageWorksConfig()
-    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
-    incoming_data_bucket = sageworks_bucket + "/incoming-data"
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+    incoming_data_bucket = "s3://" + sageworks_bucket + "/incoming-data"
 
     # Create the class and check the functionality
     s3_bucket = S3Bucket(incoming_data_bucket)
     s3_bucket.check()
     s3_bucket.refresh()
 
     # List files in the bucket
```

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/Readme.md` & `sageworks-0.1.4.2/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,138 @@
 """S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource"""
 import sys
+import boto3
+from botocore.exceptions import ClientError
+
+# Import all the AWS Glue Python Libraries
 from awsglue.utils import getResolvedOptions
 from awsglue.context import GlueContext
 from awsglue.job import Job
 from pyspark.context import SparkContext
 
-# SageWorks imports
-from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
-
 
-class S3HeavyToDataSource(Transform):
-    def __init__(self, job_name: str, input_uuid: str, output_uuid: str):
+class S3HeavyToDataSource:
+    def __init__(self, glue_context: GlueContext, input_uuid: str, output_uuid: str):
         """S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource
         Args:
-            job_name (str): The name of the AWS Glue Job
+            glue_context: GlueContext, AWS Glue Specific wrapper around SparkContext
             input_uuid (str): The S3 Path to the files to be loaded
             output_uuid (str): The UUID of the SageWorks DataSource to be created
         """
+        self.log = glue_context.get_logger()
 
-        # Call superclass init
-        super().__init__(input_uuid, output_uuid)
+        # FIXME: Pull these from Parameter Store or Config
+        self.input_uuid = input_uuid
+        self.output_uuid = output_uuid
+        self.output_meta = {"sageworks_input": self.input_uuid}
+        sageworks_bucket = "s3://scp-sageworks-artifacts"
+        self.data_source_s3_path = sageworks_bucket + "/data-sources"
 
-        # Set up all my instance attributes
-        self.input_type = TransformInput.S3_OBJECT
-        self.output_type = TransformOutput.DATA_SOURCE
-
-        # These are AWS Glue Job specific
-        sc = SparkContext()
-        self.glueContext = GlueContext(sc)
-        self.job = Job(self.glueContext)
-        self.job.init(job_name, [job_name, input_uuid, output_uuid])
+        # Our Spark Context
+        self.glue_context = glue_context
 
-    def transform_impl(self, overwrite: bool = True):
-        """Convert the CSV data into Parquet Format in the SageWorks S3 Bucket, and
+    def transform(self, input_type: str = "json", overwrite: bool = True):
+        """Convert the CSV or JSON data into Parquet Format in the SageWorks S3 Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
         # Add some tags here
         tags = ["heavy"]
 
         # Create the Output Parquet file S3 Storage Path
         s3_storage_path = f"{self.data_source_s3_path}/{self.output_uuid}"
 
         # Read JSONL files from S3 and infer schema dynamically
         self.log.info(f"Reading JSONL files from {self.input_uuid}...")
-        jsonl_dyf = self.glueContext.create_dynamic_frame_from_options(
+        input_dyf = self.glue_context.create_dynamic_frame.from_options(
             connection_type="s3",
-            connection_options={"paths": [self.input_uuid],
-                                "compressionType": "gzip",
-                                "recurse": "True",
-                                },
-            format="json",
-            format_options={'jsonPath': 'auto'},
-            transformation_ctx='apply_mapping'
+            connection_options={
+                "paths": [self.input_uuid],
+                "recurse": True,
+                "gzip": True,
+            },
+            format=input_type,
+            # format_options={'jsonPath': 'auto'}, Look into this later
+            transformation_ctx="apply_mapping",
         )
+        self.log.info("Incoming DataFrame...")
+        input_dyf.show(5)
 
         # Write Parquet files to S3
         self.log.info(f"Writing Parquet files to {s3_storage_path}...")
-        self.glueContext.write_dynamic_frame.from_options(
-            frame=jsonl_dyf,
-            connection_type='s3',
-            connection_options={'path': s3_storage_path},
-            format='parquet',
-            format_options={'compression': 'snappy', 'parquetVersion': '2.0'},
-            transformation_ctx='datasink'
+        self.glue_context.purge_s3_path(s3_storage_path, {"retentionPeriod": 0})
+        self.glue_context.write_dynamic_frame.from_options(
+            frame=input_dyf,
+            connection_type="s3",
+            connection_options={
+                "path": s3_storage_path
+                # "partitionKeys": ["year", "month", "day"],
+            },
+            format="parquet"
         )
 
-        # Set up our SageWorks metadata
-        sageworks_meta = {"sageworks_tags": tags}
+        # Set up our SageWorks metadata (description, tags, etc)
+        description = f"SageWorks data source: {self.output_uuid}"
+        sageworks_meta = {"sageworks_tags": ":".join(tags)}
         for key, value in self.output_meta.items():
             sageworks_meta[key] = value
 
-        # Generate a Glue Catalog Table
-        description = f"SageWorks data source: {self.output_uuid}"
-        self.glueContext.catalog.create_table(
-            database='sageworks',  # FIXME: Have this in config
-            table_name=self.output_uuid,
-            location=s3_storage_path,
-            schema=jsonl_dyf.schema(),
-            description=description,
-            parameters=sageworks_meta
-        )
+        # Create a new table in the AWS Data Catalog
+        self.log.info(f"Creating Data Catalog Table: {self.output_uuid}...")
+        table_input = {
+            "Name": self.output_uuid,
+            "Description": description,
+            "Parameters": sageworks_meta,
+            "TableType": "EXTERNAL_TABLE",
+            "StorageDescriptor": {
+                "Columns": [{"Name": col.name, "Type": col.dataType.typeName()} for col in input_dyf.schema().fields],
+                "Location": s3_storage_path,
+                "InputFormat": "org.apache.hadoop.mapred.TextInputFormat",
+                "OutputFormat": "org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
+                "Compressed": True,
+                "NumberOfBuckets": -1,
+                "SerdeInfo": {
+                    "SerializationLibrary": "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe",
+                    "Parameters": {"serialization.format": "1"},
+                },
+            },
+        }
+
+        # Delete the Data Catalog Table if it already exists
+        if overwrite:
+            glue_client = boto3.client("glue")
+            try:
+                glue_client.delete_table(DatabaseName="sageworks", Name=self.output_uuid)
+                self.log.info(f"Deleting Data Catalog Table: {self.output_uuid}...")
+            except ClientError as e:
+                if e.response["Error"]["Code"] != "EntityNotFoundException":
+                    raise e
 
-        # Commit the Glue Job
+        self.log.info(f"Creating Data Catalog Table: {self.output_uuid}...")
+        glue_client.create_table(DatabaseName="sageworks", TableInput=table_input)
+
+        # All done!
         self.log.info(f"{self.input_uuid} --> {self.output_uuid} complete!")
-        self.job.commit()
 
 
 if __name__ == "__main__":
     """Glue Job for the S3HeavyToDataSource Class"""
 
     # Get the arguments for this Glue Job
-    args = getResolvedOptions(sys.argv, ["JOB_NAME", "SRC_PATH", "OUTPUT_UUID"])
+    args = getResolvedOptions(sys.argv, ["JOB_NAME"])
 
-    # Create the Data Loader
-    my_loader = S3HeavyToDataSource(args['JOB_NAME'], args['SRC_PATH'], args['OUTPUT_UUID'])
+    # Grab the SparkContext, GlueContext, and Job
+    # These are all AWS Glue Job specific
+    sc = SparkContext()
+    glueContext = GlueContext(sc)
+    job = Job(glueContext)
+    job.init(args["JOB_NAME"], args)
+
+    # Test the Heavy Data Loader
+    input_path = "s3://scp-sageworks-artifacts/incoming-data/jsonl-data/"
+    data_output_uuid = "heavy_data_test"
+    my_loader = S3HeavyToDataSource(glueContext, input_path, data_output_uuid)
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
+
+    # Commit the Glue Job
+    job.commit()
```

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 if __name__ == "__main__":
     """Exercise the S3ToDataSourceLight Class"""
     from sageworks.utils.sageworks_config import SageWorksConfig
 
     # Create my Data Loader
     sageworks_config = SageWorksConfig()
-    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
-    input_path = sageworks_bucket + "/incoming-data/aqsol_public_data.csv"
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+    input_path = "s3://" + sageworks_bucket + "/incoming-data/aqsol_public_data.csv"
     output_uuid = "aqsol_data"
     my_loader = S3ToDataSourceLight(input_path, output_uuid)
     my_loader.set_output_tags(["aqsol", "public"])
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
```

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.4.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.4.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.4.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py` & `sageworks-0.1.4.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/transforms/transform.py` & `sageworks-0.1.4.2/src/sageworks/transforms/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         self.input_uuid = str(input_uuid)  # Occasionally we get a pathlib.Path object
         self.output_uuid = str(output_uuid)  # Occasionally we get a pathlib.Path object
         self.output_meta = {"sageworks_input": self.input_uuid}
 
         # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
         sageworks_config = SageWorksConfig()
         self.data_catalog_db = "sageworks"
-        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
-        self.data_source_s3_path = sageworks_bucket + "/data-sources"
-        self.feature_sets_s3_path = sageworks_bucket + "/feature-sets"
+        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+        self.data_source_s3_path = "s3://" + sageworks_bucket + "/data-sources"
+        self.feature_sets_s3_path = "s3://" + sageworks_bucket + "/feature-sets"
 
         # Grab a SageWorks Role ARN, Boto3, SageMaker Session, and SageMaker Client
         self.aws_account_clamp = AWSAccountClamp()
         self.sageworks_role_arn = self.aws_account_clamp.sageworks_execution_role_arn()
         self.boto_session = self.aws_account_clamp.boto_session()
         self.sm_session = self.aws_account_clamp.sagemaker_session(self.boto_session)
         self.sm_client = self.aws_account_clamp.sagemaker_client(self.boto_session)
```

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/cache.py` & `sageworks-0.1.4.2/src/sageworks/utils/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
          > bar
          time.sleep(11)
          cache.get('foo')
          > None
          cache.clear()
     """
 
-    def __init__(self, max_size=1000, expire=None):
+    def __init__(self, max_size=10000, expire=None):
         """Cache Initialization"""
         self.store = OrderedDict()
         self.max_size = max_size
         self.expire = expire
         self._compression_timer = 600
         self._last_compression = time.time()
```

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.4.2/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/iso_8601.py` & `sageworks-0.1.4.2/src/sageworks/utils/iso_8601.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.4.2/src/sageworks/utils/redis_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A Redis Database Cache Class"""
 import json
+
 import redis
 import logging
 from datetime import datetime, date
 
 # Local Imports
 from sageworks.utils.iso_8601 import datetime_to_iso8601, iso8601_to_datetime
 from sageworks.utils.sageworks_config import SageWorksConfig
@@ -33,22 +34,31 @@
     sageworks_config = SageWorksConfig()
     host = sageworks_config.get_config_value("SAGEWORKS_REDIS", "HOST")
     port = sageworks_config.get_config_value("SAGEWORKS_REDIS", "PORT")
     password = sageworks_config.get_config_value("SAGEWORKS_REDIS", "PASSWORD") or None
 
     # Open the Redis connection (class object)
     log.info(f"Opening Redis connection to: {host}:{port}...")
-    redis_db = redis.Redis(host, port=port, password=password, charset="utf-8", decode_responses=True, db=0)
+    redis_db = None
     try:
-        redis_db.ping()
+        # Create a temporary connection to test the connection
+        _redis_db = redis.Redis(host, port=port, password=password, socket_timeout=1)
+        _redis_db.ping()
+
+        # Now create the actual connection
+        redis_db = redis.Redis(host, port=port, password=password, charset="utf-8",
+                               decode_responses=True, db=0)
         log.info(f"Redis connection success: {host}:{port}...")
     except (redis.exceptions.ConnectionError, redis.exceptions.TimeoutError):
         msg = f"Could not connect to Redis Database: {host}:{port}..."
-        log.critical(msg)
-        raise RuntimeError(msg)
+        log.warning(msg)
+
+    @classmethod
+    def check(cls):
+        return cls.redis_db is not None
 
     def __init__(self, expire=None, prefix="", postfix=""):  # No expiration, standard 0 db, no postfix on keys
         """RedisCache Initialization"""
 
         # Setup instance variables
         self.expire = expire
         self.base_prefix = "sageworks:"  # Prefix all keys with the SageWorks namespace
@@ -131,14 +141,17 @@
 
 if __name__ == "__main__":
     """Exercise the RedisCache class"""
     import time
 
     # Create a RedisCache
     my_redis_cache = RedisCache(prefix="test")
+    if not my_redis_cache.check():
+        print("Redis not available, exiting...")
+        exit(1)
 
     # Delete anything in the test database
     my_redis_cache.clear()
 
     # Test storage
     my_redis_cache.set("foo", "bar")
     assert my_redis_cache.get("foo") == "bar"
```

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/sageworks_config.py` & `sageworks-0.1.4.2/src/sageworks/utils/sageworks_config.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.4.2/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.4.2/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.4.2/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/views/artifacts_summary.py` & `sageworks-0.1.4.2/src/sageworks/views/web_artifacts_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""ArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
+"""WebArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
 import sys
 import argparse
 import pandas as pd
 
 # SageWorks Imports
 from sageworks.views.view import View
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 
 
-class ArtifactsSummary(View):
+class WebArtifactsSummary(View):
     def __init__(self):
-        """ArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
+        """WebArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
         # Call SuperClass Initialization
         super().__init__()
 
         # Get AWS Service information for ALL the categories (data_source, feature_set, endpoints, etc)
-        self.aws_artifact_data = self.aws_broker.get_all_metadata()
-        self.aws_account_clamp = AWSAccountClamp()
+        self.aws_artifact_data = {}
+        self.refresh()
+
+        # Get AWS Account Region
+        self.aws_region = AWSAccountClamp().region()
 
         # Get a handle to the AWS Artifact Information class
         self.artifact_info = self.aws_broker.artifact_info
 
     def check(self) -> bool:
         """Can we connect to this view/service?"""
         return True  # I'm great, thx for asking
@@ -43,15 +46,15 @@
             "DATA_SOURCES": self.data_sources_summary(),
             "FEATURE_SETS": self.feature_sets_summary(),
             "MODELS": self.models_summary(),
             "ENDPOINTS": self.endpoints_summary(),
         }
         return summary_data
 
-    def incoming_data_summary(self):
+    def incoming_data_summary(self) -> pd.DataFrame:
         """Get summary data about data in the incoming-data S3 Bucket"""
         data = self.aws_artifact_data[ServiceCategory.INCOMING_DATA]
         data_summary = []
         for name, info in data.items():
             # Get the size of the S3 Storage Object(s)
             size = info.get("ContentLength") / 1_000_000
             summary = {
@@ -62,17 +65,29 @@
                 "ServerSideEncryption": info.get("ServerSideEncryption", "-"),
                 "Tags": str(
                     info.get("tags", "-"),
                 ),
             }
             data_summary.append(summary)
 
-        return pd.DataFrame(data_summary)
+        # Make sure we have data else return just the column names
+        if data_summary:
+            return pd.DataFrame(data_summary)
+        else:
+            columns = [
+                "Name",
+                "Size(MB)",
+                "Modified",
+                "ContentType",
+                "ServerSideEncryption",
+                "Tags"
+            ]
+            return pd.DataFrame(columns=columns)
 
-    def data_sources_summary(self):
+    def data_sources_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks DataSources"""
         data = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
         data_summary = []
 
         # Get the SageWorks DataSources
         if "sageworks" in data:
             for name, info in data["sageworks"].items():  # Just the sageworks database (not sagemaker_featurestore)
@@ -108,20 +123,20 @@
                 "DataLake",
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
     def hyperlinks(self, name, detail_type):
-        athena_url = f"https://{self.aws_account_clamp.region()}.console.aws.amazon.com/athena/home"
+        athena_url = f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
         link = f"<a href='{detail_type}' target='_blank'>{name}</a>"
         link += f" [<a href='{athena_url}' target='_blank'>query</a>]"
         return link
 
-    def feature_sets_summary(self):
+    def feature_sets_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks FeatureSets"""
         data = self.aws_artifact_data[ServiceCategory.FEATURE_STORE]
         data_summary = []
         for feature_group, group_info in data.items():
             # Get the tags for this Feature Group
             arn = group_info["FeatureGroupArn"]
             sageworks_meta = self.artifact_info.get_sagemaker_obj_info(arn)
@@ -154,15 +169,15 @@
                 "Online",
                 "Created",
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
-    def models_summary(self, concise=False):
+    def models_summary(self, concise=False) -> pd.DataFrame:
         """Get summary data about the SageWorks Models"""
         data = self.aws_artifact_data[ServiceCategory.MODELS]
         model_summary = []
         for model_group, model_list in data.items():
             # Special Case for Model Groups without any Models
             if not model_list:
                 summary = {"Model Group": model_group}
@@ -207,15 +222,15 @@
                 "Description",
                 "Created",
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
-    def endpoints_summary(self):
+    def endpoints_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Endpoints"""
         data = self.aws_artifact_data[ServiceCategory.ENDPOINTS]
         data_summary = []
 
         # Get Summary information for each endpoint
         for endpoint, endpoint_info in data.items():
             # Get the tags for this Model Group
@@ -274,14 +289,14 @@
 
     # Check for unknown args
     if commands:
         print("Unrecognized args: %s" % commands)
         sys.exit(1)
 
     # Create the class and get the AWS Model Registry details
-    artifact_view = ArtifactsSummary()
+    artifact_view = WebArtifactsSummary()
 
     # List the Endpoint Names
-    print("ArtifactsSummary:")
+    print("WebArtifactsSummary:")
     for category, df in artifact_view.view_data().items():
         print(f"\n{category}")
         print(df.head())
```

### Comparing `sageworks-0.1.4.1/src/sageworks/views/view.py` & `sageworks-0.1.4.2/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.4.2/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.4.2/src/sageworks/web_components/feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.4.2/src/sageworks/web_components/feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/histogram.py` & `sageworks-0.1.4.2/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.4.2/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/model_data.py` & `sageworks-0.1.4.2/src/sageworks/web_components/model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/model_details.py` & `sageworks-0.1.4.2/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/scatter_plot.py` & `sageworks-0.1.4.2/src/sageworks/web_components/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/src/sageworks/web_components/table.py` & `sageworks-0.1.4.2/src/sageworks/web_components/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 def create(
     table_id: str,
     df: pd.DataFrame,
     header_color="rgb(60, 60, 60)",
     show_columns: list[str] = None,
     row_select=False,
     markdown_columns: list[str] = None,
+    max_height: str = "200px",
+    columns_editable: bool = False,
+    fixed_headers: bool = False,
 ) -> dash_table:
     """Create a Table"""
 
     # To select rows we need to set up an ID for each row
     df["id"] = df.index
 
     # Only show these columns
@@ -21,47 +24,46 @@
         show_columns = df.columns.to_list()
         show_columns.remove("id")
 
     # Column Setup with name, id, and presentation type
     column_setup = []
     for c in show_columns:
         presentation = "markdown" if markdown_columns and c in markdown_columns else "input"
-        column_setup.append({"name": c, "id": c, "presentation": presentation})
+        if columns_editable:
+            column_setup.append({"name": c, "id": c, "deletable": True, "selectable": True})
+        else:
+            column_setup.append({"name": c, "id": c, "presentation": presentation})
 
     # Create the Dash Table
     table = dash_table.DataTable(
         id=table_id,
         data=df.to_dict("records"),
         columns=column_setup,
         sort_action="native",
         row_selectable=row_select,
         cell_selectable=False,
         selected_rows=[0],
-        # fixed_rows={'headers': True},
-        style_table={"maxHeight": "250px", "overflowY": "auto"},
+        fixed_rows={'headers': fixed_headers},
+        style_table={"maxHeight": max_height, "overflowX": "auto", "overflowY": "auto"},
         style_as_list_view=True,
         style_cell={
             "font-family": "HelveticaNeue",
-            "padding": "10px",
+            "padding": "5px",
             "overflow": "hidden",
             "textOverflow": "ellipsis",
-            "maxWidth": 200,
+            "maxWidth": 250
         },
         style_header={
-            "fontSize": 18,
+            "textAlign": "left",
+            "fontSize": 16,
             "backgroundColor": header_color,
-            "color": "rgb(200, 200, 200)",
+            "color": "rgb(200, 200, 200)"
         },
         style_data={
-            "fontSize": 18,
+            "fontSize": 14,
             "backgroundColor": "rgb(60, 60, 60)",
             "color": "rgb(200, 200, 200)",
+            "border": "0px"
         },
         markdown_options={"html": True},
     )
     return table
-
-
-# Storage
-"""
-
-"""
```

### Comparing `sageworks-0.1.4.1/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.4.2/src/sageworks.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.4.1
-Summary: SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models
+Version: 0.1.4.2
+Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -48,22 +48,19 @@
 <img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
-- [Initial Setup and Installation](https://github.com/SuperCowPowers/sageworks/wiki/Initial-Setup-and-Installation) for initial AWS/config/repository set up. 
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
-- [Coding with SageWorks Video](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
+- [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-### SageWorks Analysis Notebooks
-- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from Start to Finish
-
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
 - SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
 - **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
 - **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
 - Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
 - **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
@@ -76,10 +73,10 @@
 
 
 ### SageWorks Alpha Testers Wanted
 Our experienced team can provide development and consulting services to help you effectively use Amazon’s Machine Learning services within your organization.
 
 The popularity of cloud based Machine Learning services is booming. The problem many companies face is how that capability gets effectively used and harnessed to drive real business decisions and provide concrete value for their organization.
 
-Using SageWorks will minimizize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Alpha Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
```

### Comparing `sageworks-0.1.4.1/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.4.2/src/sageworks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,26 +40,26 @@
 applications/web_admin/flask_test.py
 applications/web_admin/hello-world-http-test.ini
 applications/web_admin/hello-world.ini
 applications/web_admin/hello-world.service
 applications/web_admin/nginx_conf/nginx.conf
 aws_setup/aws_account_check.py
 aws_setup/aws_account_check_deep.py
-aws_setup/sageworks_sandbox/.gitignore
-aws_setup/sageworks_sandbox/README.md
-aws_setup/sageworks_sandbox/app.py
-aws_setup/sageworks_sandbox/cdk.json
-aws_setup/sageworks_sandbox/requirements-dev.txt
-aws_setup/sageworks_sandbox/requirements.txt
-aws_setup/sageworks_sandbox/source.bat
-aws_setup/sageworks_sandbox/sageworks_sandbox/__init__.py
-aws_setup/sageworks_sandbox/sageworks_sandbox/sageworks_sandbox_stack.py
-aws_setup/sageworks_sandbox/tests/__init__.py
-aws_setup/sageworks_sandbox/tests/unit/__init__.py
-aws_setup/sageworks_sandbox/tests/unit/test_sageworks_sandbox_stack.py
+aws_setup/sageworks_cdk/.gitignore
+aws_setup/sageworks_cdk/README.md
+aws_setup/sageworks_cdk/app.py
+aws_setup/sageworks_cdk/cdk.json
+aws_setup/sageworks_cdk/requirements-dev.txt
+aws_setup/sageworks_cdk/requirements.txt
+aws_setup/sageworks_cdk/source.bat
+aws_setup/sageworks_cdk/stacks/__init__.py
+aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+aws_setup/sageworks_cdk/tests/__init__.py
+aws_setup/sageworks_cdk/tests/unit/__init__.py
+aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
 config/sageworks_config.ini
 data/abalone.csv
 data/test_data.csv
 data/test_data.json
 docs/admin_notes.md
 docs/sageworks_classes_concepts.md
 docs/scp_consulting.md
@@ -134,14 +134,15 @@
 src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
 src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
 src/sageworks/transforms/data_to_data/light/__init__.py
 src/sageworks/transforms/data_to_data/light/clean_data.py
 src/sageworks/transforms/data_to_data/light/data_to_data_light.py
 src/sageworks/transforms/data_to_features/__init__.py
 src/sageworks/transforms/data_to_features/heavy/__init__.py
+src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
 src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
 src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
 src/sageworks/transforms/data_to_features/light/__init__.py
 src/sageworks/transforms/data_to_features/light/data_to_features_light.py
 src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
 src/sageworks/transforms/features_to_features/__init__.py
 src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
@@ -162,26 +163,29 @@
 src/sageworks/utils/df_to_endpoint.py
 src/sageworks/utils/iso_8601.py
 src/sageworks/utils/redis_cache.py
 src/sageworks/utils/sageworks_config.py
 src/sageworks/utils/sageworks_event_bridge.py
 src/sageworks/utils/sageworks_logging.py
 src/sageworks/utils/sageworks_sqs.py
-src/sageworks/views/artifacts_summary.py
+src/sageworks/views/artifacts.py
 src/sageworks/views/view.py
+src/sageworks/views/web_artifacts_summary.py
+src/sageworks/views/web_data_source_view.py
 src/sageworks/web_components/box_plot.py
 src/sageworks/web_components/confusion_matrix.py
 src/sageworks/web_components/feature_details.py
 src/sageworks/web_components/feature_importance.py
 src/sageworks/web_components/histogram.py
 src/sageworks/web_components/line_chart.py
 src/sageworks/web_components/model_data.py
 src/sageworks/web_components/model_details.py
 src/sageworks/web_components/scatter_plot.py
 src/sageworks/web_components/table.py
+src/sageworks/web_components/violin_plot.py
 tests/create_sageworks_objs_for_tests.py
 tests/artifacts/data_source_tests.py
 tests/artifacts/endpoint_tests.py
 tests/artifacts/feature_set_tests.py
 tests/artifacts/model_tests.py
 tests/aws_account/aws_account_clamp_tests.py
 tests/aws_account/aws_service_broker_tests.py
```

### Comparing `sageworks-0.1.4.1/tests/artifacts/data_source_tests.py` & `sageworks-0.1.4.2/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.4.2/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/artifacts/feature_set_tests.py` & `sageworks-0.1.4.2/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/artifacts/model_tests.py` & `sageworks-0.1.4.2/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.4.2/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/create_sageworks_objs_for_tests.py` & `sageworks-0.1.4.2/aws_setup/aws_account_check_deep.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,28 +10,48 @@
     - abalone-regression
 Endpoints:
     - abalone-regression-end
 """
 import sys
 import time
 from pathlib import Path
+from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.artifacts.data_sources.data_source import DataSource
 from sageworks.artifacts.feature_sets.feature_set import FeatureSet
 from sageworks.artifacts.models.model import Model
 from sageworks.artifacts.endpoints.endpoint import Endpoint
 from sageworks.transforms.data_loaders.light.csv_to_data_source import CSVToDataSource
 from sageworks.transforms.data_to_features.light.data_to_features_light import DataToFeaturesLight
 from sageworks.transforms.features_to_model.features_to_model import FeaturesToModel
 from sageworks.transforms.model_to_endpoint.model_to_endpoint import ModelToEndpoint
 
+
+def redis_check():
+    """Check if the Redis Database is available"""
+    print("*** Redis Database Check ***")
+    try:
+        from sageworks.utils.redis_cache import RedisCache
+        RedisCache(prefix="test")
+        print("Redis Database Check Success...")
+    except RuntimeError as err:
+        print(f"Redis Database Check Failed: {err} but this is fine.. Redis is optional")
+
+
 if __name__ == "__main__":
     # Get the path to the dataset in the repository data directory
     test_data_path = Path(sys.modules["sageworks"].__file__).parent.parent.parent / "data" / "test_data.csv"
     abalone_data_path = Path(sys.modules["sageworks"].__file__).parent.parent.parent / "data" / "abalone.csv"
 
+    """Check if the AWS Account is Setup Correctly"""
+    print("*** AWS Identity Check ***")
+    AWSAccountClamp().check_aws_identity()
+
+    # Check that the Redis Database is available
+    redis_check()
+
     # Create the test_data DataSource
     if not DataSource("test_data").check():
         my_loader = CSVToDataSource(test_data_path, "test_data")
         my_loader.set_output_tags("test:small")
         my_loader.transform()
         print("Waiting for the test_data to be created...")
         time.sleep(5)
```

### Comparing `sageworks-0.1.4.1/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.4.2/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.4.2/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.4.2/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.4.2/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.4.2/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4.1/tox.ini` & `sageworks-0.1.4.2/tox.ini`

 * *Files identical despite different names*

