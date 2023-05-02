# Comparing `tmp/usa-net-0.0.3.tar.gz` & `tmp/usa-net-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usa-net-0.0.3.tar", last modified: Mon Apr 17 22:08:46 2023, max compression
+gzip compressed data, was "usa-net-0.0.4.tar", last modified: Tue May  2 21:46:42 2023, max compression
```

## Comparing `usa-net-0.0.3.tar` & `usa-net-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 22:08:34.000000 usa-net-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 22:08:46.440763 usa-net-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 22:08:34.000000 usa-net-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-17 22:08:34.000000 usa-net-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:08:34.000000 usa-net-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 22:08:34.000000 usa-net-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 22:08:46.440763 usa-net-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-17 22:08:34.000000 usa-net-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 22:08:34.000000 usa-net-0.0.3/tests/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/__version__.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/semantics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/trajectories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/visualize_semantics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/point2emb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/planners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/clip_sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/occupancy_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/scripts/adhoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/adhoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/adhoc/distribution_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/clip_sdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/usa/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/home_robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/posed_rgbd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/r3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/replica_cad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/usa_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 21:46:28.000000 usa-net-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 21:46:42.480197 usa-net-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 21:46:28.000000 usa-net-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-02 21:46:28.000000 usa-net-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements-ipynb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 21:46:42.480197 usa-net-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-02 21:46:28.000000 usa-net-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 21:46:28.000000 usa-net-0.0.4/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/usa/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/usa/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/visualize_semantics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/point2emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/planners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/clip_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/occupancy_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/scripts/adhoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/distribution_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/show_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/clip_sdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/usa/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/home_robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/posed_rgbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/pybullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/r3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/replica_cad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/usa_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/top_level.txt
```

### Comparing `usa-net-0.0.3/pyproject.toml` & `usa-net-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/setup.py` & `usa-net-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 #!/usr/bin/env python
 
+import re
+
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description: str = f.read()
 
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements: list[str] = f.read().splitlines()
 
 
 with open("requirements-dev.txt", "r", encoding="utf-8") as f:
     requirements_dev: list[str] = f.read().splitlines()
 
 
-with open("usa/__version__.txt", "r", encoding="utf-8") as f:
-    version: str = f.read().strip()
+with open("requirements-ipynb.txt", "r", encoding="utf-8") as f:
+    requirements_ipynb: list[str] = f.read().splitlines()
+
+
+with open("usa/__init__.py", "r", encoding="utf-8") as fh:
+    version_re = re.search(r"^__version__ = \"([^\"]*)\"", fh.read(), re.MULTILINE)
+assert version_re is not None, "Could not find version in ml/__init__.py"
+version: str = version_re.group(1)
 
 
 setup(
     name="usa-net",
     version=version,
     description="USA net project",
     author="Benjamin Bolte",
     url="https://github.com/codekansas/usa-net",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     install_requires=requirements,
     tests_require=requirements_dev,
-    extras_require={"dev": requirements_dev},
+    extras_require={
+        "dev": requirements_dev,  # Testing, linting, etc.
+        "ipynb": requirements_ipynb,  # Jupyter notebook
+    },
 )
```

### Comparing `usa-net-0.0.3/usa/evaluation/path_length.py` & `usa-net-0.0.4/usa/evaluation/path_length.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/evaluation/semantics.py` & `usa-net-0.0.4/usa/evaluation/semantics.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/evaluation/trajectories.py` & `usa-net-0.0.4/usa/evaluation/trajectories.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/evaluation/utils.py` & `usa-net-0.0.4/usa/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/evaluation/visualize_semantics.py` & `usa-net-0.0.4/usa/evaluation/visualize_semantics.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/models/clip.py` & `usa-net-0.0.4/usa/models/clip.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/models/point2emb.py` & `usa-net-0.0.4/usa/models/point2emb.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/planners/base.py` & `usa-net-0.0.4/usa/planners/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,28 +86,36 @@
                 xyz = xyz[~mask_tensor]
                 xy = xyz[:, :2]
 
                 xs = ((xy[:, 0] - origin[0]) / resolution).floor().long()
                 ys = ((xy[:, 1] - origin[1]) / resolution).floor().long()
 
                 if counts is None:
-                    counts = xy.new_zeros((ybins, xbins), dtype=torch.long).flatten()
+                    counts = xy.new_zeros((ybins, xbins), dtype=torch.int32).flatten()
                 if any_counts is None:
-                    any_counts = xy.new_zeros((ybins, xbins), dtype=torch.bool).flatten()
+                    any_counts = xy.new_zeros((ybins, xbins), dtype=torch.int32).flatten()
 
                 # Counts the number of occupying points in each cell.
                 occ_xys = (xyz[:, 2] >= min_height) & (xyz[:, 2] <= max_height)
 
                 if len(occ_xys) != 0:
                     occ_inds = ys[occ_xys] * xbins + xs[occ_xys]
-                    counts.index_add_(0, occ_inds, torch.ones_like(xs[occ_xys], dtype=torch.long))
+                    counts.index_add_(0, occ_inds, torch.ones_like(xs[occ_xys], dtype=torch.int32))
 
                 # Keeps track of the cells that have any points from anywhere.
                 inds = ys * xbins + xs
-                any_counts.index_fill_(0, inds, True)
+
+                # Does the operation on CPU if the tensor is an MPS tensor.
+                # This is slower but necessary because MPS doesn't support
+                # `index_fill_` for some versions.
+                if any_counts.device.type == "mps":
+                    any_counts.copy_(any_counts.cpu().index_fill_(0, inds.cpu(), True).to(any_counts))
+                else:
+                    inds.clamp_(min=0, max=any_counts.numel() - 1)
+                    any_counts.index_fill_(0, inds, True)
 
             assert counts is not None and any_counts is not None, "No points in the dataset"
             counts = counts.reshape((ybins, xbins))
             any_counts = any_counts.reshape((ybins, xbins))
 
             # Clears an area around the robot's poses.
             if clear_around_bot_radius > 0:
```

### Comparing `usa-net-0.0.3/usa/planners/clip_sdf.py` & `usa-net-0.0.4/usa/planners/clip_sdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,16 +375,16 @@
                 losses["sim"] = sim_loss * self.sim_loss_weight
 
             return losses
 
         # Optimization loop, just using gradient descent.
         prev_xys: Tensor | None = None
 
-        opt = torch.optim.Adam([xys], lr=self.lr)
-        # opt = torch.optim.SGD([xys], lr=self.lr, momentum=0.9)
+        # opt = torch.optim.Adam([xys], lr=self.lr)
+        opt = torch.optim.SGD([xys], lr=self.lr, momentum=0.9)
 
         for _ in tqdm.trange(self.num_optimization_steps):
             opt.zero_grad()
             losses = get_losses(xys)
             loss = cast(Tensor, sum(losses.values()))
             loss.backward()
```

### Comparing `usa-net-0.0.3/usa/planners/common.py` & `usa-net-0.0.4/usa/planners/common.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/planners/occupancy_map.py` & `usa-net-0.0.4/usa/planners/occupancy_map.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/scripts/adhoc/distribution_estimates.py` & `usa-net-0.0.4/usa/scripts/adhoc/distribution_estimates.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/tasks/clip_sdf.py` & `usa-net-0.0.4/usa/tasks/clip_sdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,23 @@
     cast_pretrained_model_key as cast_pretrained_clip_model_key,
     load_pretrained as load_pretrained_clip,
 )
 from usa.models.point2emb import Point2EmbModel
 from usa.tasks.datasets.posed_rgbd import Bounds, get_posed_rgbd_dataset
 from usa.tasks.datasets.types import PosedRGBDItem
 from usa.tasks.datasets.utils import (
+    aminmax,
     get_nearest_xyz,
     get_xy_pixel_from_xyz,
     get_xyz_coordinates,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def aminmax(x: Tensor) -> tuple[Tensor, Tensor]:
-    if x.device.type == "mps":
-        return x.min(), x.max()
-    xmin, xmax = torch.aminmax(x)
-    return xmin, xmax
-
-
 def clip_sim(a: Tensor, b: Tensor) -> Tensor:
     assert a.dim() == 2 and b.dim() == 2
     a, b = a / (a.norm(dim=1, keepdim=True) + 1e-3), b / (b.norm(dim=1, keepdim=True) + 1e-3)
     return a @ b.t()
 
 
 def get_image_crop_around(
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/home_robot.py` & `usa-net-0.0.4/usa/tasks/datasets/home_robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,12 +106,13 @@
 
 def chris_lab_home_robot_dataset() -> HomeRobotDataset:
     return HomeRobotDatasetDownload(CHRIS_LAB_URL, "chris_lab")
 
 
 if __name__ == "__main__":
     # python -m usa.tasks.datasets.impl.home_robot
+    ml.configure_logging()
     visualize_posed_rgbd_dataset(
         chris_lab_home_robot_dataset(),
         make_video=True,
         make_point_cloud=True,
     )
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/posed_rgbd.py` & `usa-net-0.0.4/usa/tasks/datasets/posed_rgbd.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 from torch import Tensor
 from torch.utils.data.dataset import Dataset
 
 from usa.tasks.datasets.home_robot import (
     HomeRobotDataset,
     chris_lab_home_robot_dataset,
 )
+from usa.tasks.datasets.pybullet import PyBulletDataset
 from usa.tasks.datasets.r3d import LabR3DDataset, R3DDataset, StudioR3DDataset
 from usa.tasks.datasets.replica_cad import ReplicaCADDataset
 from usa.tasks.datasets.stretch import (
     chess_stretch_dataset,
     kitchen_stretch_dataset,
     lab_stretch_dataset,
 )
 from usa.tasks.datasets.types import PosedRGBDItem
+from usa.tasks.datasets.utils import aminmax, get_inv_intrinsics
 
 logger = logging.getLogger(__name__)
 
 
 def get_posed_rgbd_dataset(
     key: str,
     *,
@@ -36,14 +38,20 @@
     random_crop: bool = True,
 ) -> Dataset[PosedRGBDItem]:
     if key == "home_robot":
         if path is None:
             path = os.environ.get("HOME_ROBOT_DS_PATH")
         assert path is not None, "Path must be specified for `home_robot` dataset; set `HOME_ROBOT_DS_PATH` env var"
         return HomeRobotDataset(path)
+    if key == "pybullet":
+        if path is None:
+            path = os.environ.get("PYBULLET_DS_PATH")
+        assert path is not None, "Path must be specified for `pybullet` dataset; set `PYBULLET_DS_PATH` env var"
+        assert img_dim is None, "`img_dim` and `random_crop` not supported for `pybullet`"
+        return PyBulletDataset(path)
     if key == "r3d":
         if path is None:
             path = os.environ.get("R3D_DS_PATH")
         assert path is not None, "Path must be specified for `r3d` dataset; set `R3D_DS_PATH` env var"
         return R3DDataset(path, img_dim=img_dim, random_crop=random_crop)
     if key == "chris_lab":
         return chris_lab_home_robot_dataset()
@@ -109,17 +117,14 @@
             dim=1,
         )
 
     @classmethod
     def from_xyz(cls, xyz: Tensor) -> Tensor:
         assert xyz.shape[-1] == 3
 
-        # Supports MPS tensors.
-        aminmax = lambda x: (x.min(), x.max()) if x.device.type == "mps" else tuple(torch.aminmax(x))
-
         xmin, xmax = aminmax(xyz[..., 0])
         ymin, ymax = aminmax(xyz[..., 1])
         zmin, zmax = aminmax(xyz[..., 2])
 
         return torch.tensor([[xmin, xmax], [ymin, ymax], [zmin, zmax]], device=xyz.device, dtype=xyz.dtype)
 
 
@@ -144,15 +149,16 @@
         torch.arange(0, height, device=device, dtype=dtype),
         indexing="xy",
     )
     xy = torch.stack([xs, ys], dim=-1).flatten(0, 1).unsqueeze(0).repeat_interleave(bsz, 0)
     xyz = torch.cat((xy, torch.ones_like(xy[..., :1])), dim=-1)
 
     # Applies intrinsics and extrinsics.
-    xyz = xyz @ intrinsics.inverse().transpose(-1, -2)
+    # xyz = xyz @ intrinsics.inverse().transpose(-1, -2)
+    xyz = xyz @ get_inv_intrinsics(intrinsics).transpose(-1, -2)
     xyz = xyz * depth.flatten(1).unsqueeze(-1)
     xyz = (xyz[..., None, :] * pose[..., None, :3, :3]).sum(dim=-1) + pose[..., None, :3, 3]
 
     # Mask out bad depth points.
     xyz = xyz.unflatten(1, (height, width))
     xyz[mask.squeeze(1)] = 0.0
 
@@ -238,15 +244,15 @@
     bounds: np.ndarray | None = None
 
     if cache_loc is not None and cache_loc.is_file():
         bounds = np.load(cache_loc)
     else:
         for xyz, mask in iter_xyz(ds, "Bounds"):
             xyz_flat = xyz[~mask]
-            minv_torch, maxv_torch = xyz_flat.aminmax(dim=0)
+            minv_torch, maxv_torch = aminmax(xyz_flat, dim=0)
             minv, maxv = minv_torch.cpu().numpy(), maxv_torch.cpu().numpy()
             if bounds is None:
                 bounds = np.stack((minv, maxv), axis=1)
             else:
                 bounds[:, 0] = np.minimum(bounds[:, 0], minv)
                 bounds[:, 1] = np.maximum(bounds[:, 1], maxv)
         assert bounds is not None, "No samples found"
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/r3d.py` & `usa-net-0.0.4/usa/tasks/datasets/r3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     start_pose: np.ndarray  # (4, 4) initial camera pose matrix
 
 
 def as_pose_matrix(pose: list[float]) -> np.ndarray:
     """Converts a list of pose parameters to a pose matrix.
 
     Args:
-        pose: The list of pose parametres, (qx, qy, qz, qw, px, py, pz)
+        pose: The list of pose parameters, (qx, qy, qz, qw, px, py, pz)
 
     Returns:
         A (4, 4) pose matrix
     """
 
     mat = np.eye(4, dtype=np.float64)
     qx, qy, qz, qw, px, py, pz = pose
@@ -280,14 +280,15 @@
         if not self.file_path.exists():
             download_url(STUDIO_DATASET_URL, self.file_path.parent, filename=filename)
         super().__init__(self.file_path, img_dim=img_dim, random_crop=random_crop)
 
 
 if __name__ == "__main__":
     # python -m ml.tasks.datasets.impl.r3d
+    ml.configure_logging()
     visualize_posed_rgbd_dataset(
         StudioR3DDataset(),
         make_video=True,
         make_point_cloud=True,
         max_point_cloud_samples=5,
         point_cloud_sample_stride=5,
         concat_horizontal=True,
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/replica_cad.py` & `usa-net-0.0.4/usa/tasks/datasets/replica_cad.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,8 +140,9 @@
         if ml.is_debugging():
             item.check()
         return item
 
 
 if __name__ == "__main__":
     # python -m usa.tasks.datasets.impl.replica_cad
+    ml.configure_logging()
     visualize_posed_rgbd_dataset(ReplicaCADDataset("apt_3_mnp"), max_point_cloud_samples=10)
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/stretch.py` & `usa-net-0.0.4/usa/tasks/datasets/stretch.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,12 +203,13 @@
 
 def chess_stretch_dataset() -> StretchDataset:
     return StretchDatasetDownload(CHESS_CLIP_URL, "chess")
 
 
 if __name__ == "__main__":
     # python -m usa.tasks.datasets.impl.stretch
+    ml.configure_logging()
     visualize_posed_rgbd_dataset(
         lab_stretch_dataset(),
         make_video=False,
         make_point_cloud=True,
     )
```

### Comparing `usa-net-0.0.3/usa/tasks/datasets/types.py` & `usa-net-0.0.4/usa/tasks/datasets/types.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.3/usa/tasks/datasets/utils.py` & `usa-net-0.0.4/usa/tasks/datasets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 from torch.utils.data.dataset import Dataset, IterableDataset
 
 from usa.tasks.datasets.types import PosedRGBDItem
 
 logger = logging.getLogger(__name__)
 
 
+def aminmax(x: Tensor, dim: int | None = None) -> tuple[Tensor, Tensor]:
+    if x.device.type == "mps":
+        if dim is None:
+            return x.min(), x.max()
+        return x.min(dim=dim)[0], x.max(dim=dim)[0]
+    xmin, xmax = torch.aminmax(x, dim=dim)
+    return xmin, xmax
+
+
 def test_dataset(ds: Dataset | IterableDataset | DataLoader, max_samples: int = 3) -> None:
     """Iterates through a dataset.
 
     Args:
         ds: The dataset to iterate through
         max_samples: Maximum number of samples to loop through
     """
@@ -221,15 +230,15 @@
             # C, H, W -> H, W, C
             yield concatted.permute(1, 2, 0).numpy()
 
             i += 1
             if max_samples is not None and i >= max_samples:
                 break
 
-    ml.WRITERS["ffmpeg"](iter_frames(), save_path)
+    ml.write_video(iter_frames(), save_path)
 
 
 def make_point_cloud_from_dataset(
     ds: Dataset[PosedRGBDItem],
     batch_size: int = 4,
     num_workers: int = 0,
     voxel_size: float = 5e-2,
@@ -342,17 +351,14 @@
         rotate: If set, rotate the video 90 degrees
         concat_horizontal: If set, concatenate the video horizontally
     """
 
     # Disabling Metal because it doesn't support fp64.
     os.environ["DISABLE_METAL"] = "1"
 
-    ml.Debugging.set(True)  # Always log debug information here.
-    ml.configure_logging()
-
     # Gets the output directory.
     (output_dir_path := Path(output_dir)).mkdir(exist_ok=True, parents=True)
     video_path = (output_dir_path / "video.mp4").resolve()
     point_cloud_path = (output_dir_path / "point_cloud.ply").resolve()
 
     # Generates a video from the dataset.
     if make_video:
```

### Comparing `usa-net-0.0.3/usa_net.egg-info/SOURCES.txt` & `usa-net-0.0.4/usa_net.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
+requirements-ipynb.txt
 requirements.txt
 setup.cfg
 setup.py
+notebooks/__init__.py
+notebooks/test_dataset.py
+notebooks/test_planner.py
 tests/test_dummy.py
 usa/__init__.py
-usa/__version__.txt
 usa/evaluation/__init__.py
 usa/evaluation/path_length.py
 usa/evaluation/semantics.py
 usa/evaluation/trajectories.py
 usa/evaluation/utils.py
 usa/evaluation/visualize_semantics.py
 usa/models/__init__.py
 usa/models/clip.py
 usa/models/point2emb.py
+usa/models/sam.py
 usa/planners/__init__.py
 usa/planners/base.py
 usa/planners/clip_sdf.py
 usa/planners/common.py
 usa/planners/occupancy_map.py
 usa/scripts/__init__.py
 usa/scripts/cli.py
 usa/scripts/adhoc/__init__.py
 usa/scripts/adhoc/distribution_estimates.py
+usa/scripts/adhoc/show_point_cloud.py
 usa/tasks/__init__.py
 usa/tasks/clip_sdf.py
 usa/tasks/datasets/__init__.py
 usa/tasks/datasets/home_robot.py
 usa/tasks/datasets/posed_rgbd.py
+usa/tasks/datasets/pybullet.py
 usa/tasks/datasets/r3d.py
 usa/tasks/datasets/replica_cad.py
 usa/tasks/datasets/stretch.py
 usa/tasks/datasets/types.py
 usa/tasks/datasets/utils.py
 usa_net.egg-info/PKG-INFO
 usa_net.egg-info/SOURCES.txt
```

