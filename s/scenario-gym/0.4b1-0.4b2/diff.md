# Comparing `tmp/scenario_gym-0.4b1.tar.gz` & `tmp/scenario_gym-0.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenario_gym-0.4b1.tar", last modified: Fri Mar 10 09:18:05 2023, max compression
+gzip compressed data, was "scenario_gym-0.4b2.tar", last modified: Tue Mar 14 23:18:20 2023, max compression
```

## Comparing `scenario_gym-0.4b1.tar` & `scenario_gym-0.4b2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.478342 scenario_gym-0.4b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-10 09:18:05.478342 scenario_gym-0.4b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.466341 scenario_gym-0.4b1/scenario_gym/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.470342 scenario_gym-0.4b1/scenario_gym/entity/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/pedestrian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/entity/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.470342 scenario_gym-0.4b1/scenario_gym/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/integrations/argoverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/integrations/deepmind_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/integrations/nuScenes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/integrations/openaigym.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.470342 scenario_gym-0.4b1/scenario_gym/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/collision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.470342 scenario_gym-0.4b1/scenario_gym/metrics/rss/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/rss/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/rss/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/rss/rss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/metrics/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.470342 scenario_gym-0.4b1/scenario_gym/pedestrian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/pedestrian/social_force.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/road_network/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/road_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/road_network/xodr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/scenario/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/scenario_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/sensor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/sensor/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/sensor/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/state/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/state/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/state/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/viewer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/viewer/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/viewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.474342 scenario_gym-0.4b1/scenario_gym/xosc_interface/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/xosc_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/xosc_interface/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/xosc_interface/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/scenario_gym/xosc_interface/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.466341 scenario_gym-0.4b1/scenario_gym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-10 09:18:05.000000 scenario_gym-0.4b1/scenario_gym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-10 09:18:05.000000 scenario_gym-0.4b1/scenario_gym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:18:05.000000 scenario_gym-0.4b1/scenario_gym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-10 09:18:05.000000 scenario_gym-0.4b1/scenario_gym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 09:18:05.000000 scenario_gym-0.4b1/scenario_gym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 09:18:05.478342 scenario_gym-0.4b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:18:05.478342 scenario_gym-0.4b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test__package.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_scenario_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-03-10 09:17:55.000000 scenario_gym-0.4b1/tests/test_xosc_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.186613 scenario_gym-0.4b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-14 23:18:20.186613 scenario_gym-0.4b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.174612 scenario_gym-0.4b2/scenario_gym/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.178612 scenario_gym-0.4b2/scenario_gym/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/pedestrian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/entity/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.178612 scenario_gym-0.4b2/scenario_gym/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/integrations/argoverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/integrations/deepmind_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/integrations/nuScenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/integrations/openaigym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.178612 scenario_gym-0.4b2/scenario_gym/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/collision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.178612 scenario_gym-0.4b2/scenario_gym/metrics/rss/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/rss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/rss/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/rss/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/rss/rss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/metrics/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/pedestrian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/pedestrian/social_force.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/road_network/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/road_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/road_network/xodr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/scenario/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/scenario_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/sensor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/sensor/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/sensor/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/state/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/state/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.182613 scenario_gym-0.4b2/scenario_gym/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/viewer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/viewer/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/viewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.186613 scenario_gym-0.4b2/scenario_gym/xosc_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/xosc_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/xosc_interface/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/xosc_interface/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/scenario_gym/xosc_interface/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.178612 scenario_gym-0.4b2/scenario_gym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-14 23:18:20.000000 scenario_gym-0.4b2/scenario_gym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-14 23:18:20.000000 scenario_gym-0.4b2/scenario_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 23:18:20.000000 scenario_gym-0.4b2/scenario_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-14 23:18:20.000000 scenario_gym-0.4b2/scenario_gym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-14 23:18:20.000000 scenario_gym-0.4b2/scenario_gym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 23:18:20.186613 scenario_gym-0.4b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:18:20.186613 scenario_gym-0.4b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test__package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_scenario_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-03-14 23:18:10.000000 scenario_gym-0.4b2/tests/test_xosc_interface.py
```

### Comparing `scenario_gym-0.4b1/LICENSE` & `scenario_gym-0.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/PKG-INFO` & `scenario_gym-0.4b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenario_gym
-Version: 0.4b1
+Version: 0.4b2
 Summary: scenario_gym - a lightweight framework for learning from scenario data.
 Author-email: Hamish Scott <hamish@drisk.ai>
 Project-URL: Homepage, https://github.com/driskai/scenario_gym
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `scenario_gym-0.4b1/README.md` & `scenario_gym-0.4b2/README.md`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/pyproject.toml` & `scenario_gym-0.4b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/__init__.py` & `scenario_gym-0.4b2/scenario_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/action.py` & `scenario_gym-0.4b2/scenario_gym/action.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/agent.py` & `scenario_gym-0.4b2/scenario_gym/agent.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/callback.py` & `scenario_gym-0.4b2/scenario_gym/callback.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/catalog_entry.py` & `scenario_gym-0.4b2/scenario_gym/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/controller.py` & `scenario_gym-0.4b2/scenario_gym/controller.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/entity/base.py` & `scenario_gym-0.4b2/scenario_gym/entity/base.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/entity/batch.py` & `scenario_gym-0.4b2/scenario_gym/entity/batch.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/entity/misc.py` & `scenario_gym-0.4b2/scenario_gym/entity/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,21 @@
         if mass is not None:
             mass = float(mass)
         return base_args + (mass,), {}
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]):
         """Load the pedestrian from a dictionary."""
+        catalog = (
+            Catalog.from_dict(data["catalog"])
+            if data.get("catalog") is not None
+            else None
+        )
         return cls(
-            Catalog.from_dict(data["catalog"]) if "catalog" in data else None,
+            catalog,
             data["catalog_entry"],
             data["catalog_category"],
             data["catalog_type"],
             BoundingBox.from_dict(data["bounding_box"]),
             data.get("properties", {}),
             data.get("files", []),
             data.get("mass"),
```

### Comparing `scenario_gym-0.4b1/scenario_gym/entity/pedestrian.py` & `scenario_gym-0.4b2/scenario_gym/entity/pedestrian.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,21 @@
         if mass is not None:
             mass = float(mass)
         return base_args + (mass,), {}
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]):
         """Load the pedestrian from a dictionary."""
+        catalog = (
+            Catalog.from_dict(data["catalog"])
+            if data.get("catalog") is not None
+            else None
+        )
         return cls(
-            Catalog.from_dict(data["catalog"]) if "catalog" in data else None,
+            catalog,
             data["catalog_entry"],
             data["catalog_category"],
             data["catalog_type"],
             BoundingBox.from_dict(data["bounding_box"]),
             data.get("properties", {}),
             data.get("files", []),
             data.get("mass"),
```

### Comparing `scenario_gym-0.4b1/scenario_gym/entity/vehicle.py` & `scenario_gym-0.4b2/scenario_gym/entity/vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,16 +122,21 @@
             rear_axle,
         )
         return base_args + veh_args, {}
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]):
         """Load the vehicle from a dictionary."""
+        catalog = (
+            Catalog.from_dict(data["catalog"])
+            if data.get("catalog") is not None
+            else None
+        )
         return cls(
-            Catalog.from_dict(data["catalog"]) if "catalog" in data else None,
+            catalog,
             data["catalog_entry"],
             data["catalog_category"],
             data["catalog_type"],
             BoundingBox.from_dict(data["bounding_box"]),
             data.get("properties", {}),
             data.get("files", []),
             data.get("mass"),
```

### Comparing `scenario_gym-0.4b1/scenario_gym/integrations/argoverse.py` & `scenario_gym-0.4b2/scenario_gym/integrations/argoverse.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/integrations/deepmind_env.py` & `scenario_gym-0.4b2/scenario_gym/integrations/deepmind_env.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/integrations/nuScenes.py` & `scenario_gym-0.4b2/scenario_gym/integrations/nuScenes.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/integrations/openaigym.py` & `scenario_gym-0.4b2/scenario_gym/integrations/openaigym.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/manager.py` & `scenario_gym-0.4b2/scenario_gym/manager.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/base.py` & `scenario_gym-0.4b2/scenario_gym/metrics/base.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/collision.py` & `scenario_gym-0.4b2/scenario_gym/metrics/collision.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/rss/callback.py` & `scenario_gym-0.4b2/scenario_gym/metrics/rss/callback.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/rss/rss.py` & `scenario_gym-0.4b2/scenario_gym/metrics/rss/rss.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/rss/rss_utils.py` & `scenario_gym-0.4b2/scenario_gym/metrics/rss/rss_utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/metrics/trajectory.py` & `scenario_gym-0.4b2/scenario_gym/metrics/trajectory.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/observation.py` & `scenario_gym-0.4b2/scenario_gym/observation.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/agent.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/agent.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/behaviour.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/behaviour.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/config.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/config.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/controller.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/controller.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/observation.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/observation.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/random_walk.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/random_walk.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/route.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/route.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/sensor.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/sensor.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/pedestrian/social_force.py` & `scenario_gym-0.4b2/scenario_gym/pedestrian/social_force.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/road_network/base.py` & `scenario_gym-0.4b2/scenario_gym/road_network/base.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/road_network/objects.py` & `scenario_gym-0.4b2/scenario_gym/road_network/objects.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/road_network/road_network.py` & `scenario_gym-0.4b2/scenario_gym/road_network/road_network.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/road_network/utils.py` & `scenario_gym-0.4b2/scenario_gym/road_network/utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/road_network/xodr.py` & `scenario_gym-0.4b2/scenario_gym/road_network/xodr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Dict, List, Optional, Tuple
-from uuid import uuid4
 
 import numpy as np
 from pyxodr.road_objects.lane import Lane as xodrLane
 from pyxodr.road_objects.network import RoadNetwork as xodrRoadNetwork
 from shapely.geometry import LineString, Polygon
 
 from scenario_gym.road_network import Lane, LaneType, Road
@@ -34,15 +33,15 @@
     except KeyError as e:
         raise KeyError(
             f"Lane {lane.id} has an invalid lane type: {lane.type}. Allowed lane "
             f"types are {list(LaneType.__members__)}."
         ) from e
 
     return Lane(
-        str(uuid4()),
+        repr(lane),
         lane_boundary,
         lane_traffic_flow_line,
         [],
         [],
         lane_type,
         elevation=elevation,
     )
@@ -75,15 +74,15 @@
         for lane in xodr_lane_section.lanes:
             sg_lane = xodr_lane_to_sg(lane, simplify_tolerance)
             if sg_lane is not None:
                 lanes.append(sg_lane)
                 old_to_new_lanes[lane] = sg_lane
 
         road = Road(
-            str(uuid4()),
+            repr(xodr_road),
             road_boundary,
             road_center,
             lanes=lanes,
             elevation=road_elevation,
         )
         roads.append(road)
```

### Comparing `scenario_gym-0.4b1/scenario_gym/scenario/actions.py` & `scenario_gym-0.4b2/scenario_gym/scenario/actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,7 +140,30 @@
     def _apply(self, state: State, entity: Optional[Entity]) -> None:
         """Update the entity with action variables."""
         if entity is not None:
             if state.entity_state[entity] is None:
                 state.entity_state[entity] = {}
             for k, v in self.action_variables.items():
                 state.entity_state[entity][k] = v
+
+    def trigger_condition(self, state: State) -> bool:
+        """Update when the state time is greater than action time."""
+        return state.t > self.t
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Write the action to a dictionary."""
+        return {
+            "t": self.t,
+            "action_class": self.action_class,
+            "entity_ref": self.entity_ref,
+            "action_variables": self.action_variables,
+        }
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]):
+        """Load the action from a dictionary."""
+        return cls(
+            data["t"],
+            data["action_class"],
+            data["entity_ref"],
+            data["action_variables"],
+        )
```

### Comparing `scenario_gym-0.4b1/scenario_gym/scenario/scenario.py` & `scenario_gym-0.4b2/scenario_gym/scenario/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,15 +198,20 @@
                     break
             entities.append(Ent.from_dict(e_data))
 
         road_network = data.get("road_network")
         if road_network is not None:
             if road_network.get("path") is not None:
                 path = Path(road_network["path"])
-                road_network = RoadNetwork.create_from_file(path)
+                if path.exists():
+                    road_network = RoadNetwork.create_from_file(path)
+                elif road_network.get("name") is not None:
+                    road_network = RoadNetwork(name=road_network["name"])
+                else:
+                    road_network = None
             else:
                 road_network = RoadNetwork.create_from_dict(road_network)
 
         actions = []
         for a_data in data.get("actions", ()):
             for Act in a_classes:
                 if Act.__name__ == a_data.get(
@@ -357,21 +362,15 @@
             The figure size.
 
         show : bool
             If set to False will not call `plt.show` so the figure can be modified
             or saved.
 
         """
-        name = (
-            self.name.replace(".xosc", "")
-            if self.name
-            else (
-                self.path.split("/")[-1].split(".")[0] if self.path else "Scenario"
-            )
-        )
+        name = self.name if self.name is not None else "Scenario"
         plt.figure(figsize=figsize)
         if self.road_network is not None:
             for geom in self.road_network.driveable_surface.geoms:
                 plt.fill(*geom.exterior.xy, c="gray", alpha=0.25)
                 for i in geom.interiors:
                     plt.fill(*i.xy, c="white")
             for r in self.road_network.roads:
```

### Comparing `scenario_gym-0.4b1/scenario_gym/scenario_gym.py` & `scenario_gym-0.4b2/scenario_gym/scenario_gym.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/sensor/base.py` & `scenario_gym-0.4b2/scenario_gym/sensor/base.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/sensor/common.py` & `scenario_gym-0.4b2/scenario_gym/sensor/common.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/sensor/map.py` & `scenario_gym-0.4b2/scenario_gym/sensor/map.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/state/state.py` & `scenario_gym-0.4b2/scenario_gym/state/state.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/state/utils.py` & `scenario_gym-0.4b2/scenario_gym/state/utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/trajectory.py` & `scenario_gym-0.4b2/scenario_gym/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         Returns
         -------
         Optional[np.ndarray]
             The position as a numpy array. If the time given is outside of the
             range of the trajectory and extrapolate is False then None is returned.
 
         """
+        t = np.array(t)
         if self._interpolated is None:
             data = self.data
             if data.shape[0] == 1:
                 data = np.repeat(data, 2, axis=0)
                 data[-1, 0] += 1e-3
             self._interpolated = interp1d(
                 data[:, 0],
@@ -172,15 +173,15 @@
                 axis=0,
             )
         if isinstance(extrapolate, tuple):
             ext_bck, ext_fwd = extrapolate
             extrapolate = True
         else:
             ext_bck = ext_fwd = extrapolate
-        if isinstance(t, float):
+        if t.ndim == 0:
             if not extrapolate and (t < self.min_t or t > self.max_t):
                 return None
             elif t < self.min_t and not ext_bck:
                 return self.data[0, 1:]
             elif t > self.max_t and not ext_fwd:
                 return self.data[-1, 1:]
             return self._interpolated(t)
```

### Comparing `scenario_gym-0.4b1/scenario_gym/utils.py` & `scenario_gym-0.4b2/scenario_gym/utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/viewer/base.py` & `scenario_gym-0.4b2/scenario_gym/viewer/base.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/viewer/opencv.py` & `scenario_gym-0.4b2/scenario_gym/viewer/opencv.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,16 @@
         """Render the given state around a given entity (by reference)."""
         ego_pose = self.get_center_pose(state, e_ref)
 
         for layer in self.render_layers:
             if layer != "entity" and layer != "text":
                 getattr(self, f"render_{layer}")(state, ego_pose)
 
-        for entity_idx, (entity, pose) in enumerate(state.poses.items()):
+        for entity, pose in state.poses.items():
+            entity_idx = state.scenario.entities.index(entity)
             self.draw_entity(state, entity_idx, entity, pose, ego_pose)
 
         if "text" in self.render_layers:
             self.render_text(state)
 
     def get_center_pose(self, state: State, e_ref: str) -> np.ndarray:
         """Get the pose for the center of the frame."""
```

### Comparing `scenario_gym-0.4b1/scenario_gym/viewer/utils.py` & `scenario_gym-0.4b2/scenario_gym/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/xosc_interface/catalogs.py` & `scenario_gym-0.4b2/scenario_gym/xosc_interface/catalogs.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/xosc_interface/read.py` & `scenario_gym-0.4b2/scenario_gym/xosc_interface/read.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym/xosc_interface/write.py` & `scenario_gym-0.4b2/scenario_gym/xosc_interface/write.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym.egg-info/PKG-INFO` & `scenario_gym-0.4b2/scenario_gym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenario-gym
-Version: 0.4b1
+Version: 0.4b2
 Summary: scenario_gym - a lightweight framework for learning from scenario data.
 Author-email: Hamish Scott <hamish@drisk.ai>
 Project-URL: Homepage, https://github.com/driskai/scenario_gym
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `scenario_gym-0.4b1/scenario_gym.egg-info/SOURCES.txt` & `scenario_gym-0.4b2/scenario_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/scenario_gym.egg-info/requires.txt` & `scenario_gym-0.4b2/scenario_gym.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_actions.py` & `scenario_gym-0.4b2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_callback.py` & `scenario_gym-0.4b2/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_catalog_entry.py` & `scenario_gym-0.4b2/tests/test_catalog_entry.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_controller.py` & `scenario_gym-0.4b2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_entity.py` & `scenario_gym-0.4b2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_manager.py` & `scenario_gym-0.4b2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_metrics.py` & `scenario_gym-0.4b2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_observation.py` & `scenario_gym-0.4b2/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_rss.py` & `scenario_gym-0.4b2/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_scenario.py` & `scenario_gym-0.4b2/tests/test_scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 def test_describe(example_scenario):
     """Test the `describe` method."""
     example_scenario.describe()
 
 
 def test_plot(example_scenario):
-    """Test the `describe` method."""
+    """Test the `plot` method."""
     example_scenario.plot(show=False)
 
 
 def test_translate(example_scenario):
     """Test the translating a scenario."""
     shift = np.arange(7) + 1
     new_scenario = example_scenario.translate(shift)
```

### Comparing `scenario_gym-0.4b1/tests/test_scenario_gym.py` & `scenario_gym-0.4b2/tests/test_scenario_gym.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_sensor.py` & `scenario_gym-0.4b2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_speeds.py` & `scenario_gym-0.4b2/tests/test_speeds.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_state.py` & `scenario_gym-0.4b2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_trajectory.py` & `scenario_gym-0.4b2/tests/test_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,17 @@
     assert np.allclose(
         traj.position_at_t(0.5, extrapolate=True)[:2], [0.5, 0.5]
     ), "Should be 0.5."
     assert np.allclose(
         traj.position_at_t(1.5, extrapolate=True)[:2], [1.5, 1.5]
     ), "Should be 1.5."
 
+    # test position with int
+    traj.position_at_t(1)
+
     # test simple extrapolation
     assert np.allclose(
         traj.position_at_t(2.5, extrapolate=True)[:2], [2.5, 2.5]
     ), "Should be 2.5."
     assert np.allclose(
         traj.position_at_t(-1.0, extrapolate=True)[:2], [-1.0, -1.0]
     ), "Should be -1."
```

### Comparing `scenario_gym-0.4b1/tests/test_utils.py` & `scenario_gym-0.4b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_viewer.py` & `scenario_gym-0.4b2/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `scenario_gym-0.4b1/tests/test_xosc_interface.py` & `scenario_gym-0.4b2/tests/test_xosc_interface.py`

 * *Files identical despite different names*

