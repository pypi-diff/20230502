# Comparing `tmp/vantage6-server-3.8.4.tar.gz` & `tmp/vantage6-server-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-3.8.4.tar", last modified: Tue Apr 25 13:31:04 2023, max compression
+gzip compressed data, was "vantage6-server-3.8.5.tar", last modified: Tue May  2 14:03:46 2023, max compression
```

## Comparing `vantage6-server-3.8.4.tar` & `vantage6-server-3.8.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.782282 vantage6-server-3.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-25 13:31:04.782282 vantage6-server-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:31:04.782282 vantage6-server-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.770281 vantage6-server-3.8.4/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   100968 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.770281 vantage6-server-3.8.4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/node_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/server_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/testnodeconfiguration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/configuration/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/configuration/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.774281 vantage6-server-3.8.4/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/controller/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.778282 vantage6-server-3.8.4/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.778282 vantage6-server-3.8.4/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.778282 vantage6-server-3.8.4/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/common/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    26416 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 13:30:46.000000 vantage6-server-3.8.4/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.782282 vantage6-server-3.8.4/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 13:31:04.000000 vantage6-server-3.8.4/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100968 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.231736 vantage6-server-3.8.5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/node_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/server_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/testnodeconfiguration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.235736 vantage6-server-3.8.5/vantage6/server/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/configuration/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/configuration/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.239736 vantage6-server-3.8.5/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/controller/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.239736 vantage6-server-3.8.5/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/common/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26416 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-02 14:03:31.000000 vantage6-server-3.8.5/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:46.243736 vantage6-server-3.8.5/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 14:03:46.000000 vantage6-server-3.8.5/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-3.8.4/PKG-INFO` & `vantage6-server-3.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.5 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.8.4/setup.py` & `vantage6-server-3.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/tests_server/test_models.py` & `vantage6-server-3.8.5/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/tests_server/test_resources.py` & `vantage6-server-3.8.5/tests_server/test_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/__init__.py` & `vantage6-server-3.8.5/vantage6/server/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/dev/server.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/node_config_skeleton.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/node_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/server_config_skeleton.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/server_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-3.8.5/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/_version.py` & `vantage6-server-3.8.5/vantage6/server/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 4, 'final', __build__, 0)))
+version_info = ((( 3, 8, 5, 'final', __build__, 0)))
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-server-3.8.4/vantage6/server/cli/server.py` & `vantage6-server-3.8.5/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/configuration/configuration_manager.py` & `vantage6-server-3.8.5/vantage6/server/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/context.py` & `vantage6-server-3.8.5/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/controller/fixture.py` & `vantage6-server-3.8.5/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/controller/query.py` & `vantage6-server-3.8.5/vantage6/server/controller/query.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/db.py` & `vantage6-server-3.8.5/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/default_roles.py` & `vantage6-server-3.8.5/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/globals.py` & `vantage6-server-3.8.5/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/mail_service.py` & `vantage6-server-3.8.5/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/__init__.py` & `vantage6-server-3.8.5/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/algorithm_port.py` & `vantage6-server-3.8.5/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/authenticatable.py` & `vantage6-server-3.8.5/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/base.py` & `vantage6-server-3.8.5/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/collaboration.py` & `vantage6-server-3.8.5/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/member.py` & `vantage6-server-3.8.5/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/node.py` & `vantage6-server-3.8.5/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/node_config.py` & `vantage6-server-3.8.5/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/organization.py` & `vantage6-server-3.8.5/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/permission.py` & `vantage6-server-3.8.5/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/result.py` & `vantage6-server-3.8.5/vantage6/server/model/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/role.py` & `vantage6-server-3.8.5/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/rule.py` & `vantage6-server-3.8.5/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/task.py` & `vantage6-server-3.8.5/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/model/user.py` & `vantage6-server-3.8.5/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/permission.py` & `vantage6-server-3.8.5/vantage6/server/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/__init__.py` & `vantage6-server-3.8.5/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/collaboration.py` & `vantage6-server-3.8.5/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/common/_schema.py` & `vantage6-server-3.8.5/vantage6/server/resource/common/_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-3.8.5/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-3.8.5/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/event.py` & `vantage6-server-3.8.5/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/health.py` & `vantage6-server-3.8.5/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/node.py` & `vantage6-server-3.8.5/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/organization.py` & `vantage6-server-3.8.5/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/pagination.py` & `vantage6-server-3.8.5/vantage6/server/resource/pagination.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/port.py` & `vantage6-server-3.8.5/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/recover.py` & `vantage6-server-3.8.5/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/result.py` & `vantage6-server-3.8.5/vantage6/server/resource/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/role.py` & `vantage6-server-3.8.5/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/rule.py` & `vantage6-server-3.8.5/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/stats.py` & `vantage6-server-3.8.5/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/task.py` & `vantage6-server-3.8.5/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/token.py` & `vantage6-server-3.8.5/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/user.py` & `vantage6-server-3.8.5/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/version.py` & `vantage6-server-3.8.5/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/vpn.py` & `vantage6-server-3.8.5/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/resource/websocket_test.py` & `vantage6-server-3.8.5/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6/server/websockets.py` & `vantage6-server-3.8.5/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.4/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-3.8.5/vantage6_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.5 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.8.4/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-3.8.5/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

