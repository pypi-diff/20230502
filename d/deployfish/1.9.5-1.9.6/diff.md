# Comparing `tmp/deployfish-1.9.5.tar.gz` & `tmp/deployfish-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deployfish-1.9.5.tar", last modified: Fri Oct  7 21:22:26 2022, max compression
+gzip compressed data, was "deployfish-1.9.6.tar", last modified: Wed Nov  2 23:51:11 2022, max compression
```

## Comparing `deployfish-1.9.5.tar` & `deployfish-1.9.6.tar`

### file list

```diff
@@ -1,145 +1,147 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.192609 deployfish-1.9.5/
--rw-rw-r--   0 cmalek     (501) admin       (80)       79 2022-07-28 20:44:14.000000 deployfish-1.9.5/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     5934 2022-10-07 21:22:26.192806 deployfish-1.9.5/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     4575 2022-08-26 22:39:15.000000 deployfish-1.9.5/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.132594 deployfish-1.9.5/deployfish/
--rw-rw-r--   0 cmalek     (501) admin       (80)      176 2022-10-07 21:22:16.000000 deployfish-1.9.5/deployfish/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.135661 deployfish-1.9.5/deployfish/config/
--rw-rw-r--   0 cmalek     (501) admin       (80)      358 2022-08-31 20:20:08.000000 deployfish-1.9.5/deployfish/config/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6200 2022-08-31 20:21:04.000000 deployfish-1.9.5/deployfish/config/config.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.138044 deployfish-1.9.5/deployfish/config/processors/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1317 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/config/processors/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2898 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/config/processors/abstract.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4206 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/config/processors/environment.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8165 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/config/processors/terraform.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.143917 deployfish-1.9.5/deployfish/config/test/
--rw-rw-r--   0 cmalek     (501) admin       (80)       22 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)       86 2021-06-01 19:42:21.000000 deployfish-1.9.5/deployfish/config/test/env_file.env
--rw-rw-r--   0 cmalek     (501) admin       (80)     1806 2021-06-01 19:43:17.000000 deployfish-1.9.5/deployfish/config/test/interpolate.yml
--rw-rw-r--   0 cmalek     (501) admin       (80)     2821 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/terraform.tfstate
--rw-rw-r--   0 cmalek     (501) admin       (80)     2413 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/terraform.tfstate.0.12
--rw-rw-r--   0 cmalek     (501) admin       (80)     1891 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/terraform.tfstate.prod
--rw-rw-r--   0 cmalek     (501) admin       (80)     1875 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/terraform.tfstate.qa
--rw-rw-r--   0 cmalek     (501) admin       (80)     1740 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/terraform_interpolate.yml
--rw-rw-r--   0 cmalek     (501) admin       (80)     6823 2021-06-01 19:46:51.000000 deployfish-1.9.5/deployfish/config/test/test_Config.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     3232 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/config/test/test_Terraform.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.152947 deployfish-1.9.5/deployfish/controllers/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1041 2022-09-01 17:08:53.000000 deployfish-1.9.5/deployfish/controllers/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6751 2022-09-16 16:20:59.000000 deployfish-1.9.5/deployfish/controllers/base.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6992 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/cluster.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    15554 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/commands.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     9325 2022-09-03 21:28:48.000000 deployfish-1.9.5/deployfish/controllers/crud.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2109 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/elb.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4997 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/elbv2.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2654 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/invoked_task.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11333 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/logs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13978 2022-08-30 17:24:16.000000 deployfish-1.9.5/deployfish/controllers/network.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7584 2022-08-31 20:34:07.000000 deployfish-1.9.5/deployfish/controllers/secrets.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    16034 2022-09-03 21:28:48.000000 deployfish-1.9.5/deployfish/controllers/service.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13647 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/controllers/task.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    10097 2022-08-31 20:00:15.000000 deployfish-1.9.5/deployfish/controllers/tunnel.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2246 2022-08-30 23:34:34.000000 deployfish-1.9.5/deployfish/controllers/utils.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.155630 deployfish-1.9.5/deployfish/core/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.156735 deployfish-1.9.5/deployfish/core/adapters/
--rw-rw-r--   0 cmalek     (501) admin       (80)       44 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/adapters/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2474 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/abstract.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.161908 deployfish-1.9.5/deployfish/core/adapters/deployfish/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1621 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4321 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/appscaling.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2610 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/cloudwatch.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    50627 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/ecs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2273 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/events.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      393 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/mixins.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4036 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/secrets.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      918 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/service_discovery.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      293 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/ssh.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.164530 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    26267 2022-05-04 23:04:35.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_ServiceHelperTaskAdapter.py
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_ServiceHelperTask_new.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11743 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_Service_new.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    14649 2022-05-04 23:04:35.000000 deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_StandaloneTaskAdapter.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5040 2022-09-15 18:24:37.000000 deployfish-1.9.5/deployfish/core/aws.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5245 2022-08-31 20:30:29.000000 deployfish-1.9.5/deployfish/core/loaders.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.174428 deployfish-1.9.5/deployfish/core/models/
--rw-rw-r--   0 cmalek     (501) admin       (80)      552 2022-07-21 00:02:24.000000 deployfish-1.9.5/deployfish/core/models/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6878 2022-08-30 17:24:16.000000 deployfish-1.9.5/deployfish/core/models/abstract.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6840 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/appscaling.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2483 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/cloudwatch.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13707 2022-08-30 17:24:16.000000 deployfish-1.9.5/deployfish/core/models/cloudwatchlogs.py
--rw-r--r--   0 cmalek     (501) admin       (80)       67 2022-05-25 16:09:37.000000 deployfish-1.9.5/deployfish/core/models/deployfish.code-workspace
--rw-rw-r--   0 cmalek     (501) admin       (80)    16672 2022-10-07 21:18:13.000000 deployfish-1.9.5/deployfish/core/models/ec2.py
--rw-rw-r--   0 cmalek     (501) admin       (80)   102990 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/ecs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1592 2022-10-07 21:19:09.000000 deployfish-1.9.5/deployfish/core/models/efs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6913 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/elb.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20435 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/elbv2.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     9076 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/events.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    14071 2022-08-30 23:02:43.000000 deployfish-1.9.5/deployfish/core/models/mixins.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    12423 2022-08-30 23:03:09.000000 deployfish-1.9.5/deployfish/core/models/secrets.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11657 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/service_discovery.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5246 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/models/ssh.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.175258 deployfish-1.9.5/deployfish/core/models/test/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/models/test/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    10900 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/models/test/test_TaskDefinitionFARGATEMixin.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    17121 2022-10-07 20:08:28.000000 deployfish-1.9.5/deployfish/core/ssh.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      176 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/core/utils.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.175965 deployfish-1.9.5/deployfish/core/waiters/
--rw-rw-r--   0 cmalek     (501) admin       (80)     8165 2022-05-25 16:00:00.000000 deployfish-1.9.5/deployfish/core/waiters/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.177676 deployfish-1.9.5/deployfish/core/waiters/hooks/
--rw-rw-r--   0 cmalek     (501) admin       (80)       91 2021-05-17 22:41:37.000000 deployfish-1.9.5/deployfish/core/waiters/hooks/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2974 2022-05-04 23:04:35.000000 deployfish-1.9.5/deployfish/core/waiters/hooks/abstract.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7828 2022-09-03 21:28:48.000000 deployfish-1.9.5/deployfish/core/waiters/hooks/ecs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2521 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/exceptions.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.179507 deployfish-1.9.5/deployfish/ext/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/ext/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1973 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/ext/ext_df_argparse.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7875 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/ext/ext_df_jinja2.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4930 2022-09-03 21:28:48.000000 deployfish-1.9.5/deployfish/ext/ext_df_plugin.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7557 2022-09-16 18:10:05.000000 deployfish-1.9.5/deployfish/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-08-30 17:24:16.000000 deployfish-1.9.5/deployfish/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1252 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/registry.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.181864 deployfish-1.9.5/deployfish/renderers/
--rw-rw-r--   0 cmalek     (501) admin       (80)       91 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/renderers/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      194 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/renderers/abstract.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2054 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/renderers/misc.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    14566 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/renderers/table.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.188594 deployfish-1.9.5/deployfish/templates/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1670 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--classicloadbalancer.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      734 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--cloudwatchloggroup.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      992 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--cloudwatchlogstream.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1620 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--cluster.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1284 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--invokedtask.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1162 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--loadbalancer.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      573 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--loadbalancerlistener.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      918 2022-08-31 20:35:31.000000 deployfish-1.9.5/deployfish/templates/detail--secrets--diff.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)       80 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--secrets.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1477 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--service--short.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1081 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--service.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1479 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--servicehelpertask.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      502 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--sshtunnel.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1309 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--standalonetask--short.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      313 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--standalonetask.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      582 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail--targetgroup.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/detail.jinja2
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.192175 deployfish-1.9.5/deployfish/templates/macros/
--rw-rw-r--   0 cmalek     (501) admin       (80)      283 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/awslogs.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      394 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/classicloadbalancer.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     2393 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/invoked-task.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      868 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/secrets.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     1577 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/service.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      440 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/target-group.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     8049 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/task-definition.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      974 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/task.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)      774 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/templates/macros/utils.jinja2
--rw-rw-r--   0 cmalek     (501) admin       (80)     3371 2022-08-26 22:39:15.000000 deployfish-1.9.5/deployfish/types.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-10-07 21:22:26.134728 deployfish-1.9.5/deployfish.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     5934 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     4834 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       76 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      178 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       11 2022-10-07 21:22:26.000000 deployfish-1.9.5/deployfish.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      600 2022-10-07 21:22:26.193546 deployfish-1.9.5/setup.cfg
--rwxrwxr-x   0 cmalek     (501) admin       (80)     1199 2022-10-07 21:22:16.000000 deployfish-1.9.5/setup.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.322708 deployfish-1.9.6/
+-rw-r--r--   0 glenn      (504) admin       (80)       33 2017-05-04 22:31:28.000000 deployfish-1.9.6/AUTHORS.txt
+-rw-r--r--   0 glenn      (504) admin       (80)     1462 2019-10-10 18:08:35.000000 deployfish-1.9.6/LICENSE.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       79 2021-07-02 21:46:39.000000 deployfish-1.9.6/MANIFEST.in
+-rw-r--r--   0 glenn      (504) admin       (80)     4962 2022-11-02 23:51:11.322821 deployfish-1.9.6/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     4575 2022-10-02 22:43:12.000000 deployfish-1.9.6/README.md
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.285554 deployfish-1.9.6/deployfish/
+-rw-r--r--   0 glenn      (504) admin       (80)     6148 2017-08-01 21:07:09.000000 deployfish-1.9.6/deployfish/.DS_Store
+-rw-r--r--   0 glenn      (504) admin       (80)      176 2022-11-02 23:41:45.000000 deployfish-1.9.6/deployfish/__init__.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.287613 deployfish-1.9.6/deployfish/config/
+-rw-r--r--   0 glenn      (504) admin       (80)      358 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6200 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/config.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.288597 deployfish-1.9.6/deployfish/config/processors/
+-rw-r--r--   0 glenn      (504) admin       (80)     1317 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/processors/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2898 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/processors/abstract.py
+-rw-r--r--   0 glenn      (504) admin       (80)     4206 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/processors/environment.py
+-rw-r--r--   0 glenn      (504) admin       (80)     8165 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/config/processors/terraform.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.292732 deployfish-1.9.6/deployfish/config/test/
+-rw-r--r--   0 glenn      (504) admin       (80)       22 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)       86 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/env_file.env
+-rw-r--r--   0 glenn      (504) admin       (80)     1806 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/interpolate.yml
+-rw-r--r--   0 glenn      (504) admin       (80)     2821 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/terraform.tfstate
+-rw-r--r--   0 glenn      (504) admin       (80)     2413 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/terraform.tfstate.0.12
+-rw-r--r--   0 glenn      (504) admin       (80)     1891 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/terraform.tfstate.prod
+-rw-r--r--   0 glenn      (504) admin       (80)     1875 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/terraform.tfstate.qa
+-rw-r--r--   0 glenn      (504) admin       (80)     1740 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/terraform_interpolate.yml
+-rw-r--r--   0 glenn      (504) admin       (80)     6823 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/test_Config.py
+-rw-r--r--   0 glenn      (504) admin       (80)     3232 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/config/test/test_Terraform.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.297524 deployfish-1.9.6/deployfish/controllers/
+-rw-r--r--   0 glenn      (504) admin       (80)     1041 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6751 2022-10-25 20:58:50.000000 deployfish-1.9.6/deployfish/controllers/base.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6992 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/cluster.py
+-rw-r--r--   0 glenn      (504) admin       (80)    15554 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/commands.py
+-rw-r--r--   0 glenn      (504) admin       (80)     9325 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/crud.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2109 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/elb.py
+-rw-r--r--   0 glenn      (504) admin       (80)     4997 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/elbv2.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2654 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/invoked_task.py
+-rw-r--r--   0 glenn      (504) admin       (80)    11333 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/logs.py
+-rw-r--r--   0 glenn      (504) admin       (80)    13978 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/network.py
+-rw-r--r--   0 glenn      (504) admin       (80)     7584 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/secrets.py
+-rw-r--r--   0 glenn      (504) admin       (80)    16034 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/service.py
+-rw-r--r--   0 glenn      (504) admin       (80)    13647 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/task.py
+-rw-r--r--   0 glenn      (504) admin       (80)    10097 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/tunnel.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2246 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/controllers/utils.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.298674 deployfish-1.9.6/deployfish/core/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/__init__.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.299125 deployfish-1.9.6/deployfish/core/adapters/
+-rw-r--r--   0 glenn      (504) admin       (80)       44 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/adapters/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2474 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/abstract.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.301618 deployfish-1.9.6/deployfish/core/adapters/deployfish/
+-rw-r--r--   0 glenn      (504) admin       (80)     1621 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     4321 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/appscaling.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2610 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/cloudwatch.py
+-rw-r--r--   0 glenn      (504) admin       (80)    50627 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/ecs.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2273 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/events.py
+-rw-r--r--   0 glenn      (504) admin       (80)      393 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/mixins.py
+-rw-r--r--   0 glenn      (504) admin       (80)     4036 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/secrets.py
+-rw-r--r--   0 glenn      (504) admin       (80)      918 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/service_discovery.py
+-rw-r--r--   0 glenn      (504) admin       (80)      293 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/ssh.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.303322 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)    26267 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_ServiceHelperTaskAdapter.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_ServiceHelperTask_new.py
+-rw-r--r--   0 glenn      (504) admin       (80)    11743 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_Service_new.py
+-rw-r--r--   0 glenn      (504) admin       (80)    14649 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_StandaloneTaskAdapter.py
+-rw-r--r--   0 glenn      (504) admin       (80)     5040 2022-10-25 20:58:50.000000 deployfish-1.9.6/deployfish/core/aws.py
+-rw-r--r--   0 glenn      (504) admin       (80)     5245 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/loaders.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.310458 deployfish-1.9.6/deployfish/core/models/
+-rw-r--r--   0 glenn      (504) admin       (80)      552 2022-04-15 21:07:50.000000 deployfish-1.9.6/deployfish/core/models/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6878 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/abstract.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6840 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/appscaling.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2483 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/cloudwatch.py
+-rw-r--r--   0 glenn      (504) admin       (80)    13707 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/cloudwatchlogs.py
+-rw-r--r--   0 glenn      (504) admin       (80)    16672 2022-10-25 20:58:50.000000 deployfish-1.9.6/deployfish/core/models/ec2.py
+-rw-r--r--   0 glenn      (504) admin       (80)   103143 2022-10-28 21:53:38.000000 deployfish-1.9.6/deployfish/core/models/ecs.py
+-rw-r--r--   0 glenn      (504) admin       (80)     1592 2022-10-25 20:58:50.000000 deployfish-1.9.6/deployfish/core/models/efs.py
+-rw-r--r--   0 glenn      (504) admin       (80)     6913 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/elb.py
+-rw-r--r--   0 glenn      (504) admin       (80)    20435 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/elbv2.py
+-rw-r--r--   0 glenn      (504) admin       (80)     9076 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/events.py
+-rw-r--r--   0 glenn      (504) admin       (80)    14071 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/mixins.py
+-rw-r--r--   0 glenn      (504) admin       (80)    12423 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/secrets.py
+-rw-r--r--   0 glenn      (504) admin       (80)    11657 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/service_discovery.py
+-rw-r--r--   0 glenn      (504) admin       (80)     5246 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/models/ssh.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.311201 deployfish-1.9.6/deployfish/core/models/test/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/models/test/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)    10900 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/models/test/test_TaskDefinitionFARGATEMixin.py
+-rw-r--r--   0 glenn      (504) admin       (80)    17121 2022-10-26 20:44:37.000000 deployfish-1.9.6/deployfish/core/ssh.py
+-rw-r--r--   0 glenn      (504) admin       (80)      176 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/utils.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.311451 deployfish-1.9.6/deployfish/core/waiters/
+-rw-r--r--   0 glenn      (504) admin       (80)     8165 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/waiters/__init__.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.312844 deployfish-1.9.6/deployfish/core/waiters/hooks/
+-rw-r--r--   0 glenn      (504) admin       (80)       91 2021-07-02 21:46:39.000000 deployfish-1.9.6/deployfish/core/waiters/hooks/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2974 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/waiters/hooks/abstract.py
+-rw-r--r--   0 glenn      (504) admin       (80)     7828 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/core/waiters/hooks/ecs.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2521 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/exceptions.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.314425 deployfish-1.9.6/deployfish/ext/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/ext/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     1973 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/ext/ext_df_argparse.py
+-rw-r--r--   0 glenn      (504) admin       (80)     7875 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/ext/ext_df_jinja2.py
+-rw-r--r--   0 glenn      (504) admin       (80)     4930 2022-10-27 15:57:16.000000 deployfish-1.9.6/deployfish/ext/ext_df_plugin.py
+-rw-r--r--   0 glenn      (504) admin       (80)     7557 2022-10-27 15:45:45.000000 deployfish-1.9.6/deployfish/main.py
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/py.typed
+-rw-r--r--   0 glenn      (504) admin       (80)     1252 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/registry.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.315439 deployfish-1.9.6/deployfish/renderers/
+-rw-r--r--   0 glenn      (504) admin       (80)       91 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/renderers/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)      194 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/renderers/abstract.py
+-rw-r--r--   0 glenn      (504) admin       (80)     2054 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/renderers/misc.py
+-rw-r--r--   0 glenn      (504) admin       (80)    14566 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/renderers/table.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.320087 deployfish-1.9.6/deployfish/templates/
+-rw-r--r--   0 glenn      (504) admin       (80)        0 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/__init__.py
+-rw-r--r--   0 glenn      (504) admin       (80)     1670 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--classicloadbalancer.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      734 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--cloudwatchloggroup.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      992 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--cloudwatchlogstream.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1620 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--cluster.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1284 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--invokedtask.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1162 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--loadbalancer.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      573 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--loadbalancerlistener.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      918 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--secrets--diff.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)       80 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--secrets.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1477 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--service--short.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1081 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--service.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1479 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--servicehelpertask.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      502 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--sshtunnel.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1309 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--standalonetask--short.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      313 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--standalonetask.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      582 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail--targetgroup.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      255 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/detail.jinja2
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.322497 deployfish-1.9.6/deployfish/templates/macros/
+-rw-r--r--   0 glenn      (504) admin       (80)      283 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/awslogs.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      394 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/classicloadbalancer.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     2393 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/invoked-task.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      868 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/secrets.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     1577 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/service.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      440 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/target-group.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     8049 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/task-definition.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      974 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/task.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)      774 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/templates/macros/utils.jinja2
+-rw-r--r--   0 glenn      (504) admin       (80)     3371 2022-10-02 22:43:12.000000 deployfish-1.9.6/deployfish/types.py
+drwxr-xr-x   0 glenn      (504) admin       (80)        0 2022-11-02 23:51:11.287129 deployfish-1.9.6/deployfish.egg-info/
+-rw-r--r--   0 glenn      (504) admin       (80)     4962 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (504) admin       (80)     4830 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (504) admin       (80)        1 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       75 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/entry_points.txt
+-rw-r--r--   0 glenn      (504) admin       (80)      178 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/requires.txt
+-rw-r--r--   0 glenn      (504) admin       (80)       11 2022-11-02 23:51:11.000000 deployfish-1.9.6/deployfish.egg-info/top_level.txt
+-rw-r--r--   0 glenn      (504) admin       (80)      600 2022-11-02 23:51:11.323350 deployfish-1.9.6/setup.cfg
+-rwxr-xr-x   0 glenn      (504) admin       (80)     1199 2022-11-02 23:41:45.000000 deployfish-1.9.6/setup.py
```

### Comparing `deployfish-1.9.5/PKG-INFO` & `deployfish-1.9.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: deployfish
-Version: 1.9.5
+Version: 1.9.6
 Summary: AWS ECS related deployment tools
 Home-page: https://github.com/caltechads/deployfish
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
-License: UNKNOWN
-Description: ```
-              _            _              __ _     _
-             | |          | |            / _(_)   | |
-           __| | ___ _ __ | | ___  _   _| |_ _ ___| |__
-          / _` |/ _ \ '_ \| |/ _ \| | | |  _| / __| '_ \
-         | (_| |  __/ |_) | | (_) | |_| | | | \__ \ | | |
-          \__,_|\___| .__/|_|\___/ \__, |_| |_|___/_| |_|
-                    | |             __/ |
-                    |_|            |___/
-        ```
-        
-        `deployfish` has commands for managing the whole lifecycle of your application:
-        
-        * Safely and easily create, update, destroy and restart ECS services
-        * Safely and easily create, update, run, schedule and unschedule ECS tasks
-        * Extensive support for ECS related services like load balancing, application
-          autoscaling and service discovery
-        * Easily scale the number of containers in your service, optionally scaling its
-          associated autoscaling group at the same time
-        * Manage multiple environments for your service (test, qa, prod, etc.) in
-          multiple AWS accounts.
-        * Uses AWS Parameter Store for secrets for your containers
-        * View the configuration and status of running ECS services
-        * Run a one-off command related to your service
-        * Easily exec through your VPC bastion host into your running containers, or
-          ssh into a ECS container machine in your cluster.
-        * Setup SSH tunnels to the private AWS resources in VPC that your service
-          uses so that you can connect to them from your work machine.
-        
-        * Extensible! Add additional functionality through custom deployfish modules.
-        * Works great in CodeBuild steps in a CodePipeline based CI/CD system!
-        
-        
-        Additionally, `deployfish` integrates with
-        [terraform](https://www.terraform.io) state files so that you can use the
-        values of terraform outputs directly in your `deployfish` configurations.
-        
-        To use `deployfish`, you
-        
-        * Install `deployfish`
-        * Define your service in `deployfish.yml`
-        * Use `deploy` to start managing your service
-        
-        A simple `deployfish.yml` looks like this:
-        
-            services:
-              - name: my-service
-                environment: prod
-                cluster: my-cluster
-                count: 2
-                load_balancer:
-                  service_role_arn: arn:aws:iam::123142123547:role/ecsServiceRole
-                  load_balancer_name: my-service-elb
-                  container_name: my-service
-                  container_port: 80
-                family: my-service
-                network_mode: bridge
-                task_role_arn: arn:aws:iam::123142123547:role/myTaskRole
-                containers:
-                  - name: my-service
-                    image: 123142123547.dkr.ecr.us-west-2.amazonaws.com/my-service:0.0.1
-                    cpu: 128
-                    memory: 256
-                    memoryReservation: 128
-                    ports:
-                      - "80"
-                    environment:
-                      - ENVIRONMENT=prod
-                      - ANOTHER_ENV_VAR=value
-                      - THIRD_ENV_VAR=value
-        
-        See the `examples/` folder in this repository for example `deployfish.yml`
-        files.
-        
-        ## Documentation
-        
-        [deployfish.readthedocs.io](http://deployfish.readthedocs.io/) is the full
-        reference for deployfish, including a full `deployfish.yml` reference and
-        tutorials.
-        
-        
-        ## Installing deployfish
-        
-        deployfish is a pure python package.  As such, it can be installed in the
-        usual python ways.  For the following instructions, either install it into your
-        global python install, or use a python [virtual environment](https://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/) to install it
-        without polluting your global python environment.
-        
-        ### Install deployfish
-        
-            pip install deployfish
-        
-        ### Install AWS CLI v2
-        
-        deployfish requries AWS CLI v2 for some of its functionality, notably EXEC'ing into FARGATE containers.  While AWS CLI
-        v1 was installable via `pip`, AWS CLI v2 is not, so we have to do the install manually.  Here's how to set that up on a
-        Mac:
-        
-            # Uninstall any old versions of the cli
-            pip uninstall awscli
-        
-            # Deactivate any pyenv environment so we can be in the system-wide Python interpreter
-            cd ~
-        
-            # Install the new AWS CLI from brew -- it's no longer pip installable
-            brew update
-            brew install awscli
-        
-            # Install the Session Manager plugin
-            curl "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/sessionmanager-bundle.zip" -o "sessionmanager-bundle.zip"
-            unzip sessionmanager-bundle.zip
-            sudo ./sessionmanager-bundle/install -i /usr/local/sessionmanagerplugin -b /usr/local/bin/session-manager-plugin
-        
-        
-        If later on you have issues with EXEC'ing or with the `aws` command in general, check to ensure you're getting your
-        global version of `aws` instead of an old one in your current virtual environment:
-        
-            aws --version
-        
-        If the version string shows version < 2:
-        
-            pip uninstall awscli
-        
 Keywords: aws,ecs,docker,devops
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+```
+      _            _              __ _     _
+     | |          | |            / _(_)   | |
+   __| | ___ _ __ | | ___  _   _| |_ _ ___| |__
+  / _` |/ _ \ '_ \| |/ _ \| | | |  _| / __| '_ \
+ | (_| |  __/ |_) | | (_) | |_| | | | \__ \ | | |
+  \__,_|\___| .__/|_|\___/ \__, |_| |_|___/_| |_|
+            | |             __/ |
+            |_|            |___/
+```
+
+`deployfish` has commands for managing the whole lifecycle of your application:
+
+* Safely and easily create, update, destroy and restart ECS services
+* Safely and easily create, update, run, schedule and unschedule ECS tasks
+* Extensive support for ECS related services like load balancing, application
+  autoscaling and service discovery
+* Easily scale the number of containers in your service, optionally scaling its
+  associated autoscaling group at the same time
+* Manage multiple environments for your service (test, qa, prod, etc.) in
+  multiple AWS accounts.
+* Uses AWS Parameter Store for secrets for your containers
+* View the configuration and status of running ECS services
+* Run a one-off command related to your service
+* Easily exec through your VPC bastion host into your running containers, or
+  ssh into a ECS container machine in your cluster.
+* Setup SSH tunnels to the private AWS resources in VPC that your service
+  uses so that you can connect to them from your work machine.
+
+* Extensible! Add additional functionality through custom deployfish modules.
+* Works great in CodeBuild steps in a CodePipeline based CI/CD system!
+
+
+Additionally, `deployfish` integrates with
+[terraform](https://www.terraform.io) state files so that you can use the
+values of terraform outputs directly in your `deployfish` configurations.
+
+To use `deployfish`, you
+
+* Install `deployfish`
+* Define your service in `deployfish.yml`
+* Use `deploy` to start managing your service
+
+A simple `deployfish.yml` looks like this:
+
+    services:
+      - name: my-service
+        environment: prod
+        cluster: my-cluster
+        count: 2
+        load_balancer:
+          service_role_arn: arn:aws:iam::123142123547:role/ecsServiceRole
+          load_balancer_name: my-service-elb
+          container_name: my-service
+          container_port: 80
+        family: my-service
+        network_mode: bridge
+        task_role_arn: arn:aws:iam::123142123547:role/myTaskRole
+        containers:
+          - name: my-service
+            image: 123142123547.dkr.ecr.us-west-2.amazonaws.com/my-service:0.0.1
+            cpu: 128
+            memory: 256
+            memoryReservation: 128
+            ports:
+              - "80"
+            environment:
+              - ENVIRONMENT=prod
+              - ANOTHER_ENV_VAR=value
+              - THIRD_ENV_VAR=value
+
+See the `examples/` folder in this repository for example `deployfish.yml`
+files.
+
+## Documentation
+
+[deployfish.readthedocs.io](http://deployfish.readthedocs.io/) is the full
+reference for deployfish, including a full `deployfish.yml` reference and
+tutorials.
+
+
+## Installing deployfish
+
+deployfish is a pure python package.  As such, it can be installed in the
+usual python ways.  For the following instructions, either install it into your
+global python install, or use a python [virtual environment](https://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/) to install it
+without polluting your global python environment.
+
+### Install deployfish
+
+    pip install deployfish
+
+### Install AWS CLI v2
+
+deployfish requries AWS CLI v2 for some of its functionality, notably EXEC'ing into FARGATE containers.  While AWS CLI
+v1 was installable via `pip`, AWS CLI v2 is not, so we have to do the install manually.  Here's how to set that up on a
+Mac:
+
+    # Uninstall any old versions of the cli
+    pip uninstall awscli
+
+    # Deactivate any pyenv environment so we can be in the system-wide Python interpreter
+    cd ~
+
+    # Install the new AWS CLI from brew -- it's no longer pip installable
+    brew update
+    brew install awscli
+
+    # Install the Session Manager plugin
+    curl "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/sessionmanager-bundle.zip" -o "sessionmanager-bundle.zip"
+    unzip sessionmanager-bundle.zip
+    sudo ./sessionmanager-bundle/install -i /usr/local/sessionmanagerplugin -b /usr/local/bin/session-manager-plugin
+
+
+If later on you have issues with EXEC'ing or with the `aws` command in general, check to ensure you're getting your
+global version of `aws` instead of an old one in your current virtual environment:
+
+    aws --version
+
+If the version string shows version < 2:
+
+    pip uninstall awscli
```

### Comparing `deployfish-1.9.5/README.md` & `deployfish-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/config.py` & `deployfish-1.9.6/deployfish/config/config.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/processors/__init__.py` & `deployfish-1.9.6/deployfish/config/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/processors/abstract.py` & `deployfish-1.9.6/deployfish/config/processors/abstract.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/processors/environment.py` & `deployfish-1.9.6/deployfish/config/processors/environment.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/processors/terraform.py` & `deployfish-1.9.6/deployfish/config/processors/terraform.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/interpolate.yml` & `deployfish-1.9.6/deployfish/config/test/interpolate.yml`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/terraform.tfstate` & `deployfish-1.9.6/deployfish/config/test/terraform.tfstate`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/terraform.tfstate.0.12` & `deployfish-1.9.6/deployfish/config/test/terraform.tfstate.0.12`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/terraform.tfstate.prod` & `deployfish-1.9.6/deployfish/config/test/terraform.tfstate.prod`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/terraform.tfstate.qa` & `deployfish-1.9.6/deployfish/config/test/terraform.tfstate.qa`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/terraform_interpolate.yml` & `deployfish-1.9.6/deployfish/config/test/terraform_interpolate.yml`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/test_Config.py` & `deployfish-1.9.6/deployfish/config/test/test_Config.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/config/test/test_Terraform.py` & `deployfish-1.9.6/deployfish/config/test/test_Terraform.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/__init__.py` & `deployfish-1.9.6/deployfish/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/base.py` & `deployfish-1.9.6/deployfish/controllers/base.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/cluster.py` & `deployfish-1.9.6/deployfish/controllers/cluster.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/commands.py` & `deployfish-1.9.6/deployfish/controllers/commands.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/crud.py` & `deployfish-1.9.6/deployfish/controllers/crud.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/elb.py` & `deployfish-1.9.6/deployfish/controllers/elb.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/elbv2.py` & `deployfish-1.9.6/deployfish/controllers/elbv2.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/invoked_task.py` & `deployfish-1.9.6/deployfish/controllers/invoked_task.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/logs.py` & `deployfish-1.9.6/deployfish/controllers/logs.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/network.py` & `deployfish-1.9.6/deployfish/controllers/network.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/secrets.py` & `deployfish-1.9.6/deployfish/controllers/secrets.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/service.py` & `deployfish-1.9.6/deployfish/controllers/service.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/task.py` & `deployfish-1.9.6/deployfish/controllers/task.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/tunnel.py` & `deployfish-1.9.6/deployfish/controllers/tunnel.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/controllers/utils.py` & `deployfish-1.9.6/deployfish/controllers/utils.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/abstract.py` & `deployfish-1.9.6/deployfish/core/adapters/abstract.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/__init__.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/__init__.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/appscaling.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/appscaling.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/cloudwatch.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/ecs.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/ecs.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/events.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/events.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/secrets.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/secrets.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/service_discovery.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/service_discovery.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_ServiceHelperTaskAdapter.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_ServiceHelperTaskAdapter.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_Service_new.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_Service_new.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/adapters/deployfish/test/test_StandaloneTaskAdapter.py` & `deployfish-1.9.6/deployfish/core/adapters/deployfish/test/test_StandaloneTaskAdapter.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/aws.py` & `deployfish-1.9.6/deployfish/core/aws.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/loaders.py` & `deployfish-1.9.6/deployfish/core/loaders.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/__init__.py` & `deployfish-1.9.6/deployfish/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/abstract.py` & `deployfish-1.9.6/deployfish/core/models/abstract.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/appscaling.py` & `deployfish-1.9.6/deployfish/core/models/appscaling.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/cloudwatch.py` & `deployfish-1.9.6/deployfish/core/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/cloudwatchlogs.py` & `deployfish-1.9.6/deployfish/core/models/cloudwatchlogs.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/ec2.py` & `deployfish-1.9.6/deployfish/core/models/ec2.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/ecs.py` & `deployfish-1.9.6/deployfish/core/models/ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2575,14 +2575,17 @@
     @ssh_proxy_type.setter
     def ssh_proxy_type(self, value: str) -> None:
         self._ssh_proxy_type = value
 
     @property
     def ssh_target(self) -> Optional[Instance]:
         if self.task_definition.is_fargate():
+            if self.vpc_configuration is not None:
+                vpc = self.vpc_configuration['subnets'][0].vpc
+                return vpc.provisioner
             return None
         if self.container_instances:
             return self.container_instances[0].ec2_instance
         raise self.NoRunningTasks(
             'Service "{}" has no running tasks.'.format(self.data['serviceName'])
         )
```

### Comparing `deployfish-1.9.5/deployfish/core/models/efs.py` & `deployfish-1.9.6/deployfish/core/models/efs.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/elb.py` & `deployfish-1.9.6/deployfish/core/models/elb.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/elbv2.py` & `deployfish-1.9.6/deployfish/core/models/elbv2.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/events.py` & `deployfish-1.9.6/deployfish/core/models/events.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/mixins.py` & `deployfish-1.9.6/deployfish/core/models/mixins.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/secrets.py` & `deployfish-1.9.6/deployfish/core/models/secrets.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/service_discovery.py` & `deployfish-1.9.6/deployfish/core/models/service_discovery.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/ssh.py` & `deployfish-1.9.6/deployfish/core/models/ssh.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/models/test/test_TaskDefinitionFARGATEMixin.py` & `deployfish-1.9.6/deployfish/core/models/test/test_TaskDefinitionFARGATEMixin.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/ssh.py` & `deployfish-1.9.6/deployfish/core/ssh.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/waiters/__init__.py` & `deployfish-1.9.6/deployfish/core/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/waiters/hooks/abstract.py` & `deployfish-1.9.6/deployfish/core/waiters/hooks/abstract.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/core/waiters/hooks/ecs.py` & `deployfish-1.9.6/deployfish/core/waiters/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/exceptions.py` & `deployfish-1.9.6/deployfish/exceptions.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/ext/ext_df_argparse.py` & `deployfish-1.9.6/deployfish/ext/ext_df_argparse.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/ext/ext_df_jinja2.py` & `deployfish-1.9.6/deployfish/ext/ext_df_jinja2.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/ext/ext_df_plugin.py` & `deployfish-1.9.6/deployfish/ext/ext_df_plugin.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/main.py` & `deployfish-1.9.6/deployfish/main.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/registry.py` & `deployfish-1.9.6/deployfish/registry.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/renderers/misc.py` & `deployfish-1.9.6/deployfish/renderers/misc.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/renderers/table.py` & `deployfish-1.9.6/deployfish/renderers/table.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--classicloadbalancer.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--classicloadbalancer.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--cloudwatchloggroup.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--cloudwatchloggroup.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--cloudwatchlogstream.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--cloudwatchlogstream.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--cluster.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--cluster.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--invokedtask.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--invokedtask.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--loadbalancer.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--loadbalancer.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--loadbalancerlistener.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--loadbalancerlistener.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--secrets--diff.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--secrets--diff.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--service--short.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--service--short.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--service.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--service.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--servicehelpertask.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--servicehelpertask.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--standalonetask--short.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--standalonetask--short.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/detail--targetgroup.jinja2` & `deployfish-1.9.6/deployfish/templates/detail--targetgroup.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/invoked-task.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/invoked-task.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/secrets.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/secrets.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/service.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/service.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/task-definition.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/task-definition.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/task.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/task.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/templates/macros/utils.jinja2` & `deployfish-1.9.6/deployfish/templates/macros/utils.jinja2`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish/types.py` & `deployfish-1.9.6/deployfish/types.py`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/deployfish.egg-info/PKG-INFO` & `deployfish-1.9.6/deployfish.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,135 @@
 Metadata-Version: 2.1
 Name: deployfish
-Version: 1.9.5
+Version: 1.9.6
 Summary: AWS ECS related deployment tools
 Home-page: https://github.com/caltechads/deployfish
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
-License: UNKNOWN
-Description: ```
-              _            _              __ _     _
-             | |          | |            / _(_)   | |
-           __| | ___ _ __ | | ___  _   _| |_ _ ___| |__
-          / _` |/ _ \ '_ \| |/ _ \| | | |  _| / __| '_ \
-         | (_| |  __/ |_) | | (_) | |_| | | | \__ \ | | |
-          \__,_|\___| .__/|_|\___/ \__, |_| |_|___/_| |_|
-                    | |             __/ |
-                    |_|            |___/
-        ```
-        
-        `deployfish` has commands for managing the whole lifecycle of your application:
-        
-        * Safely and easily create, update, destroy and restart ECS services
-        * Safely and easily create, update, run, schedule and unschedule ECS tasks
-        * Extensive support for ECS related services like load balancing, application
-          autoscaling and service discovery
-        * Easily scale the number of containers in your service, optionally scaling its
-          associated autoscaling group at the same time
-        * Manage multiple environments for your service (test, qa, prod, etc.) in
-          multiple AWS accounts.
-        * Uses AWS Parameter Store for secrets for your containers
-        * View the configuration and status of running ECS services
-        * Run a one-off command related to your service
-        * Easily exec through your VPC bastion host into your running containers, or
-          ssh into a ECS container machine in your cluster.
-        * Setup SSH tunnels to the private AWS resources in VPC that your service
-          uses so that you can connect to them from your work machine.
-        
-        * Extensible! Add additional functionality through custom deployfish modules.
-        * Works great in CodeBuild steps in a CodePipeline based CI/CD system!
-        
-        
-        Additionally, `deployfish` integrates with
-        [terraform](https://www.terraform.io) state files so that you can use the
-        values of terraform outputs directly in your `deployfish` configurations.
-        
-        To use `deployfish`, you
-        
-        * Install `deployfish`
-        * Define your service in `deployfish.yml`
-        * Use `deploy` to start managing your service
-        
-        A simple `deployfish.yml` looks like this:
-        
-            services:
-              - name: my-service
-                environment: prod
-                cluster: my-cluster
-                count: 2
-                load_balancer:
-                  service_role_arn: arn:aws:iam::123142123547:role/ecsServiceRole
-                  load_balancer_name: my-service-elb
-                  container_name: my-service
-                  container_port: 80
-                family: my-service
-                network_mode: bridge
-                task_role_arn: arn:aws:iam::123142123547:role/myTaskRole
-                containers:
-                  - name: my-service
-                    image: 123142123547.dkr.ecr.us-west-2.amazonaws.com/my-service:0.0.1
-                    cpu: 128
-                    memory: 256
-                    memoryReservation: 128
-                    ports:
-                      - "80"
-                    environment:
-                      - ENVIRONMENT=prod
-                      - ANOTHER_ENV_VAR=value
-                      - THIRD_ENV_VAR=value
-        
-        See the `examples/` folder in this repository for example `deployfish.yml`
-        files.
-        
-        ## Documentation
-        
-        [deployfish.readthedocs.io](http://deployfish.readthedocs.io/) is the full
-        reference for deployfish, including a full `deployfish.yml` reference and
-        tutorials.
-        
-        
-        ## Installing deployfish
-        
-        deployfish is a pure python package.  As such, it can be installed in the
-        usual python ways.  For the following instructions, either install it into your
-        global python install, or use a python [virtual environment](https://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/) to install it
-        without polluting your global python environment.
-        
-        ### Install deployfish
-        
-            pip install deployfish
-        
-        ### Install AWS CLI v2
-        
-        deployfish requries AWS CLI v2 for some of its functionality, notably EXEC'ing into FARGATE containers.  While AWS CLI
-        v1 was installable via `pip`, AWS CLI v2 is not, so we have to do the install manually.  Here's how to set that up on a
-        Mac:
-        
-            # Uninstall any old versions of the cli
-            pip uninstall awscli
-        
-            # Deactivate any pyenv environment so we can be in the system-wide Python interpreter
-            cd ~
-        
-            # Install the new AWS CLI from brew -- it's no longer pip installable
-            brew update
-            brew install awscli
-        
-            # Install the Session Manager plugin
-            curl "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/sessionmanager-bundle.zip" -o "sessionmanager-bundle.zip"
-            unzip sessionmanager-bundle.zip
-            sudo ./sessionmanager-bundle/install -i /usr/local/sessionmanagerplugin -b /usr/local/bin/session-manager-plugin
-        
-        
-        If later on you have issues with EXEC'ing or with the `aws` command in general, check to ensure you're getting your
-        global version of `aws` instead of an old one in your current virtual environment:
-        
-            aws --version
-        
-        If the version string shows version < 2:
-        
-            pip uninstall awscli
-        
 Keywords: aws,ecs,docker,devops
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+```
+      _            _              __ _     _
+     | |          | |            / _(_)   | |
+   __| | ___ _ __ | | ___  _   _| |_ _ ___| |__
+  / _` |/ _ \ '_ \| |/ _ \| | | |  _| / __| '_ \
+ | (_| |  __/ |_) | | (_) | |_| | | | \__ \ | | |
+  \__,_|\___| .__/|_|\___/ \__, |_| |_|___/_| |_|
+            | |             __/ |
+            |_|            |___/
+```
+
+`deployfish` has commands for managing the whole lifecycle of your application:
+
+* Safely and easily create, update, destroy and restart ECS services
+* Safely and easily create, update, run, schedule and unschedule ECS tasks
+* Extensive support for ECS related services like load balancing, application
+  autoscaling and service discovery
+* Easily scale the number of containers in your service, optionally scaling its
+  associated autoscaling group at the same time
+* Manage multiple environments for your service (test, qa, prod, etc.) in
+  multiple AWS accounts.
+* Uses AWS Parameter Store for secrets for your containers
+* View the configuration and status of running ECS services
+* Run a one-off command related to your service
+* Easily exec through your VPC bastion host into your running containers, or
+  ssh into a ECS container machine in your cluster.
+* Setup SSH tunnels to the private AWS resources in VPC that your service
+  uses so that you can connect to them from your work machine.
+
+* Extensible! Add additional functionality through custom deployfish modules.
+* Works great in CodeBuild steps in a CodePipeline based CI/CD system!
+
+
+Additionally, `deployfish` integrates with
+[terraform](https://www.terraform.io) state files so that you can use the
+values of terraform outputs directly in your `deployfish` configurations.
+
+To use `deployfish`, you
+
+* Install `deployfish`
+* Define your service in `deployfish.yml`
+* Use `deploy` to start managing your service
+
+A simple `deployfish.yml` looks like this:
+
+    services:
+      - name: my-service
+        environment: prod
+        cluster: my-cluster
+        count: 2
+        load_balancer:
+          service_role_arn: arn:aws:iam::123142123547:role/ecsServiceRole
+          load_balancer_name: my-service-elb
+          container_name: my-service
+          container_port: 80
+        family: my-service
+        network_mode: bridge
+        task_role_arn: arn:aws:iam::123142123547:role/myTaskRole
+        containers:
+          - name: my-service
+            image: 123142123547.dkr.ecr.us-west-2.amazonaws.com/my-service:0.0.1
+            cpu: 128
+            memory: 256
+            memoryReservation: 128
+            ports:
+              - "80"
+            environment:
+              - ENVIRONMENT=prod
+              - ANOTHER_ENV_VAR=value
+              - THIRD_ENV_VAR=value
+
+See the `examples/` folder in this repository for example `deployfish.yml`
+files.
+
+## Documentation
+
+[deployfish.readthedocs.io](http://deployfish.readthedocs.io/) is the full
+reference for deployfish, including a full `deployfish.yml` reference and
+tutorials.
+
+
+## Installing deployfish
+
+deployfish is a pure python package.  As such, it can be installed in the
+usual python ways.  For the following instructions, either install it into your
+global python install, or use a python [virtual environment](https://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/) to install it
+without polluting your global python environment.
+
+### Install deployfish
+
+    pip install deployfish
+
+### Install AWS CLI v2
+
+deployfish requries AWS CLI v2 for some of its functionality, notably EXEC'ing into FARGATE containers.  While AWS CLI
+v1 was installable via `pip`, AWS CLI v2 is not, so we have to do the install manually.  Here's how to set that up on a
+Mac:
+
+    # Uninstall any old versions of the cli
+    pip uninstall awscli
+
+    # Deactivate any pyenv environment so we can be in the system-wide Python interpreter
+    cd ~
+
+    # Install the new AWS CLI from brew -- it's no longer pip installable
+    brew update
+    brew install awscli
+
+    # Install the Session Manager plugin
+    curl "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/sessionmanager-bundle.zip" -o "sessionmanager-bundle.zip"
+    unzip sessionmanager-bundle.zip
+    sudo ./sessionmanager-bundle/install -i /usr/local/sessionmanagerplugin -b /usr/local/bin/session-manager-plugin
+
+
+If later on you have issues with EXEC'ing or with the `aws` command in general, check to ensure you're getting your
+global version of `aws` instead of an old one in your current virtual environment:
+
+    aws --version
+
+If the version string shows version < 2:
+
+    pip uninstall awscli
```

### Comparing `deployfish-1.9.5/deployfish.egg-info/SOURCES.txt` & `deployfish-1.9.6/deployfish.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+AUTHORS.txt
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+deployfish/.DS_Store
 deployfish/__init__.py
 deployfish/exceptions.py
 deployfish/main.py
 deployfish/py.typed
 deployfish/registry.py
 deployfish/types.py
 deployfish.egg-info/PKG-INFO
@@ -67,15 +70,14 @@
 deployfish/core/adapters/deployfish/test/test_Service_new.py
 deployfish/core/adapters/deployfish/test/test_StandaloneTaskAdapter.py
 deployfish/core/models/__init__.py
 deployfish/core/models/abstract.py
 deployfish/core/models/appscaling.py
 deployfish/core/models/cloudwatch.py
 deployfish/core/models/cloudwatchlogs.py
-deployfish/core/models/deployfish.code-workspace
 deployfish/core/models/ec2.py
 deployfish/core/models/ecs.py
 deployfish/core/models/efs.py
 deployfish/core/models/elb.py
 deployfish/core/models/elbv2.py
 deployfish/core/models/events.py
 deployfish/core/models/mixins.py
```

### Comparing `deployfish-1.9.5/setup.cfg` & `deployfish-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `deployfish-1.9.5/setup.py` & `deployfish-1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="deployfish",
-    version="1.9.5",
+    version="1.9.6",
     description="AWS ECS related deployment tools",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/deployfish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['aws', 'ecs', 'docker', 'devops'],
```

