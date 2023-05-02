# Comparing `tmp/Shimmy-0.2.1.tar.gz` & `tmp/Shimmy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-0.2.1.tar", last modified: Fri Feb 17 12:44:14 2023, max compression
+gzip compressed data, was "Shimmy-1.0.0.tar", last modified: Tue May  2 14:30:37 2023, max compression
```

## Comparing `Shimmy-0.2.1.tar` & `Shimmy-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:44:14.358438 Shimmy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-17 12:44:14.358438 Shimmy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-02-17 12:44:11.000000 Shimmy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:44:14.358438 Shimmy-0.2.1/Shimmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-17 12:44:14.000000 Shimmy-0.2.1/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-17 12:44:11.000000 Shimmy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 12:44:14.358438 Shimmy-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-02-17 12:44:11.000000 Shimmy-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:44:14.358438 Shimmy-0.2.1/shimmy/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/atari_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/dm_control_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/openspiel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:44:14.358438 Shimmy-0.2.1/shimmy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/utils/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/utils/dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-02-17 12:44:11.000000 Shimmy-0.2.1/shimmy/utils/envs_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:44:14.358438 Shimmy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_atari.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_dm_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_dm_control_multiagent.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-02-17 12:44:11.000000 Shimmy-0.2.1/tests/test_openspiel.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.885100 Shimmy-1.0.0/
+-rw-r--r--   0 marktowers   (501) staff       (20)     1650 2023-05-02 14:30:37.883837 Shimmy-1.0.0/PKG-INFO
+-rw-r--r--   0 marktowers   (501) staff       (20)     6012 2023-05-02 14:30:15.000000 Shimmy-1.0.0/README.md
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.861810 Shimmy-1.0.0/Shimmy.egg-info/
+-rw-r--r--   0 marktowers   (501) staff       (20)     1650 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 marktowers   (501) staff       (20)      903 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)        1 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)       72 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)      614 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)        7 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)      535 2023-02-01 20:35:48.000000 Shimmy-1.0.0/pyproject.toml
+-rw-r--r--   0 marktowers   (501) staff       (20)       38 2023-05-02 14:30:37.885245 Shimmy-1.0.0/setup.cfg
+-rw-r--r--   0 marktowers   (501) staff       (20)     2894 2023-05-02 14:30:15.000000 Shimmy-1.0.0/setup.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.871284 Shimmy-1.0.0/shimmy/
+-rw-r--r--   0 marktowers   (501) staff       (20)     2763 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/__init__.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    16080 2023-02-16 23:15:58.000000 Shimmy-1.0.0/shimmy/atari_env.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3452 2023-04-07 10:51:23.000000 Shimmy-1.0.0/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     9609 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     9952 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     6942 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     8553 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    11282 2023-04-07 10:51:23.000000 Shimmy-1.0.0/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    14925 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    10209 2023-04-06 21:59:58.000000 Shimmy-1.0.0/shimmy/registration.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.876132 Shimmy-1.0.0/shimmy/utils/
+-rw-r--r--   0 marktowers   (501) staff       (20)       36 2023-02-01 20:35:48.000000 Shimmy-1.0.0/shimmy/utils/__init__.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     1764 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3054 2023-04-06 21:59:58.000000 Shimmy-1.0.0/shimmy/utils/dm_env.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     4735 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/dm_lab.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5752 2023-02-27 19:48:27.000000 Shimmy-1.0.0/shimmy/utils/envs_configs.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     2183 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.881784 Shimmy-1.0.0/tests/
+-rw-r--r--   0 marktowers   (501) staff       (20)     3729 2023-04-07 10:51:23.000000 Shimmy-1.0.0/tests/test_atari.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     8175 2023-04-07 10:51:23.000000 Shimmy-1.0.0/tests/test_bsuite.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    11017 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_control.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     6288 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3502 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_lab.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3824 2023-02-17 11:19:14.000000 Shimmy-1.0.0/tests/test_gym.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5241 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_meltingpot.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     7075 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_openspiel.py
+-rw-r--r--   0 marktowers   (501) staff       (20)      440 2023-03-27 22:11:25.000000 Shimmy-1.0.0/tests/test_pickling.py
```

### Comparing `Shimmy-0.2.1/PKG-INFO` & `Shimmy-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 0.2.1
-Summary: API for converting popular non-gymnasium environments to a gymnasium compatible environment.
+Version: 1.0.0
+Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: gym
+Provides-Extra: gym-v21
+Provides-Extra: gym-v26
 Provides-Extra: atari
 Provides-Extra: dm-control
 Provides-Extra: dm-control-multi-agent
+Provides-Extra: dm-lab
 Provides-Extra: openspiel
+Provides-Extra: meltingpot
+Provides-Extra: bsuite
 Provides-Extra: all
 Provides-Extra: testing
 
-# Shimmy
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Farama-Foundation/Shimmy/main/shimmy-text.png" width="500px"/>
+</p>
 
-An API conversion tool for popular external reinforcement learning environments to [Gymnasium](https://github.com/farama-Foundation/gymnasium) and [PettingZoo](https://github.com/farama-Foundation/pettingZoo/) APIs.
+Shimmy is an API conversion tool providing [Gymnasium](https://github.com/farama-Foundation/gymnasium) and [PettingZoo](https://github.com/farama-Foundation/pettingZoo/) bindings for popular external reinforcement learning environments.
+
+The documentation website is at [shimmy.farama.org](https://shimmy.farama.org/) and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/nhvKkYa6qX
 
 ## Supported APIs
```

### Comparing `Shimmy-0.2.1/Shimmy.egg-info/PKG-INFO` & `Shimmy-1.0.0/Shimmy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 0.2.1
-Summary: API for converting popular non-gymnasium environments to a gymnasium compatible environment.
+Version: 1.0.0
+Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: gym
+Provides-Extra: gym-v21
+Provides-Extra: gym-v26
 Provides-Extra: atari
 Provides-Extra: dm-control
 Provides-Extra: dm-control-multi-agent
+Provides-Extra: dm-lab
 Provides-Extra: openspiel
+Provides-Extra: meltingpot
+Provides-Extra: bsuite
 Provides-Extra: all
 Provides-Extra: testing
 
-# Shimmy
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Farama-Foundation/Shimmy/main/shimmy-text.png" width="500px"/>
+</p>
 
-An API conversion tool for popular external reinforcement learning environments to [Gymnasium](https://github.com/farama-Foundation/gymnasium) and [PettingZoo](https://github.com/farama-Foundation/pettingZoo/) APIs.
+Shimmy is an API conversion tool providing [Gymnasium](https://github.com/farama-Foundation/gymnasium) and [PettingZoo](https://github.com/farama-Foundation/pettingZoo/) bindings for popular external reinforcement learning environments.
+
+The documentation website is at [shimmy.farama.org](https://shimmy.farama.org/) and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/nhvKkYa6qX
 
 ## Supported APIs
```

### Comparing `Shimmy-0.2.1/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.0.0/Shimmy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 Shimmy.egg-info/SOURCES.txt
 Shimmy.egg-info/dependency_links.txt
 Shimmy.egg-info/entry_points.txt
 Shimmy.egg-info/requires.txt
 Shimmy.egg-info/top_level.txt
 shimmy/__init__.py
 shimmy/atari_env.py
+shimmy/bsuite_compatibility.py
 shimmy/dm_control_compatibility.py
 shimmy/dm_control_multiagent_compatibility.py
 shimmy/dm_lab_compatibility.py
+shimmy/meltingpot_compatibility.py
 shimmy/openai_gym_compatibility.py
 shimmy/openspiel_compatibility.py
 shimmy/registration.py
 shimmy/utils/__init__.py
+shimmy/utils/dm_control_multiagent.py
 shimmy/utils/dm_env.py
 shimmy/utils/dm_lab.py
 shimmy/utils/envs_configs.py
+shimmy/utils/meltingpot.py
 tests/test_atari.py
+tests/test_bsuite.py
 tests/test_dm_control.py
-tests/test_dm_control_multiagent.py
+tests/test_dm_control_multi_agent.py
 tests/test_dm_lab.py
 tests/test_gym.py
-tests/test_openspiel.py
+tests/test_meltingpot.py
+tests/test_openspiel.py
+tests/test_pickling.py
```

### Comparing `Shimmy-0.2.1/pyproject.toml` & `Shimmy-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Shimmy-0.2.1/setup.py` & `Shimmy-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setups up the Shimmy module."""
 from setuptools import find_packages, setup
 
 
 def get_description():
     """Gets the description from the readme."""
-    with open("README.md") as fh:
+    with open("README.md", encoding="utf-8") as fh:
         long_description = ""
         header_count = 0
         for line in fh:
             if line.startswith("##"):
                 header_count += 1
             if header_count < 2:
                 long_description += line
@@ -29,34 +29,43 @@
     raise RuntimeError("bad version data in __init__.py")
 
 
 version = get_version()
 header_count, long_description = get_description()
 
 extras = {
-    "gym": ["gym>=0.21"],
+    "gym-v21": ["gym>=0.21.0", "pyglet==1.5.11"],
+    "gym-v26": ["gym>=0.26.2"],
     "atari": ["ale-py~=0.8.1"],
     # "imageio" should be "gymnasium[mujoco]>=0.26" but there are install conflicts
     "dm-control": ["dm-control>=1.0.10", "imageio", "h5py>=3.7.0"],
-    "dm-control-multi-agent": ["dm-control>=1.0.10", "pettingzoo>=1.22"],
-    "openspiel": ["open_spiel>=1.2", "pettingzoo>=1.22"],
+    "dm-control-multi-agent": [
+        "dm-control>=1.0.10",
+        "imageio",
+        "h5py>=3.7.0",
+        "pettingzoo>=1.22.3",
+    ],
+    "dm-lab": ["dm-env>=1.6"],
+    "openspiel": ["open_spiel>=1.2", "pettingzoo>=1.22.3"],
+    "meltingpot": ["pettingzoo>=1.22.3"],
+    "bsuite": ["bsuite>=0.3.5"],
 }
 extras["all"] = list({lib for libs in extras.values() for lib in libs})
 extras["testing"] = [
     "pytest==7.1.3",
     "pillow>=9.3.0",
-    "autorom[accept-rom-license]~=0.4.2",
+    "autorom[accept-rom-license]~=0.6.0",
 ]
 
 setup(
     name="Shimmy",
     version=version,
     author="Farama Foundation",
     author_email="contact@farama.org",
-    description="API for converting popular non-gymnasium environments to a gymnasium compatible environment.",
+    description="An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.",
     url="https://github.com/Farama-Foundation/Shimmy",
     license_files=("LICENSE.txt",),
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["Reinforcement Learning", "game", "RL", "AI"],
     python_requires=">=3.7",
     packages=find_packages(),
```

### Comparing `Shimmy-0.2.1/shimmy/__init__.py` & `Shimmy-1.0.0/shimmy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from __future__ import annotations
 
 from typing import Any
 
 from shimmy.dm_lab_compatibility import DmLabCompatibilityV0
 from shimmy.openai_gym_compatibility import GymV21CompatibilityV0, GymV26CompatibilityV0
 
-__version__ = "0.2.1"
-
 
 class NotInstallClass:
     """Rather than an attribute error, this raises a more helpful import error with install instructions for shimmy."""
 
     def __init__(self, install_message: str, import_exception: ImportError):
         self.install_message = install_message
         self.import_exception = import_exception
@@ -31,28 +29,59 @@
 
 try:
     from shimmy.dm_control_multiagent_compatibility import (
         DmControlMultiAgentCompatibilityV0,
     )
 except ImportError as e:
     DmControlMultiAgentCompatibilityV0 = NotInstallClass(
-        "Dm-control or Pettingzoo is not installed, run `pip install 'shimmy[dm-control-multi-agent]'`",
+        "Dm-control or PettingZoo is not installed, run `pip install 'shimmy[dm-control-multi-agent]'`",
         e,
     )
 
 try:
-    from shimmy.openspiel_compatibility import OpenspielCompatibilityV0
+    from shimmy.openspiel_compatibility import OpenSpielCompatibilityV0
 except ImportError as e:
-    OpenspielCompatibilityV0 = NotInstallClass(
-        "Openspiel or Pettingzoo is not installed, run `pip install 'shimmy[openspiel]'`",
+    OpenSpielCompatibilityV0 = NotInstallClass(
+        "OpenSpiel or PettingZoo is not installed, run `pip install 'shimmy[openspiel]'`",
         e,
     )
 
+try:
+    from shimmy.bsuite_compatibility import BSuiteCompatibilityV0
+except ImportError as e:
+    BSuiteCompatibilityV0 = NotInstallClass(
+        "BSuite is not installed, run `pip install 'shimmy[bsuite]'`",
+        e,
+    )
+
+try:
+    from shimmy.meltingpot_compatibility import MeltingPotCompatibilityV0
+except ImportError as e:
+    MeltingPotCompatibilityV0 = NotInstallClass(
+        "Melting Pot or PettingZoo is not installed, run `pip install 'shimmy[melting-pot]' and install Melting Pot via https://github.com/deepmind/meltingpot#installation`",
+        e,
+    )
 
 __all__ = [
+    "BSuiteCompatibilityV0",
     "DmControlCompatibilityV0",
     "DmControlMultiAgentCompatibilityV0",
-    "OpenspielCompatibilityV0",
+    "OpenSpielCompatibilityV0",
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
+    "MeltingPotCompatibilityV0",
 ]
+
+
+__version__ = "1.0.0"
+
+
+try:
+    import sys
+
+    from farama_notifications import notifications
+
+    if "shimmy" in notifications and __version__ in notifications["shimmy"]:
+        print(notifications["shimmy"][__version__], file=sys.stderr)
+except Exception:  # nosec
+    pass
```

### Comparing `Shimmy-0.2.1/shimmy/atari_env.py` & `Shimmy-1.0.0/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-0.2.1/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.0.0/tests/test_dm_control_multi_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,180 @@
-"""Wrapper to convert a dm_env multiagent environment into a pettingzoo compatible environment."""
-from __future__ import annotations
+"""Tests the multi-agent dm-control soccer environment."""
+import pickle
 
-import functools
-from itertools import repeat
-from typing import Any
-
-import dm_control.composer
-import dm_env
-import gymnasium
-from gymnasium.envs.mujoco.mujoco_rendering import MujocoRenderer
-from pettingzoo import ParallelEnv
-
-from shimmy.utils.dm_env import dm_obs2gym_obs, dm_spec2gym_space
-
-
-def _unravel_ma_timestep(
-    timestep: dm_env.TimeStep, agents: list[str]
-) -> tuple[
-    dict[str, Any],
-    dict[str, float],
-    dict[str, bool],
-    dict[str, bool],
-    dict[str, Any],
-]:
-    """Opens up the timestep to return obs, reward, terminated, truncated, info."""
-    # set terminated and truncated
-    term, trunc = False, False
-    if timestep.last():
-        if timestep.discount == 0:
-            trunc = True
-        else:
-            term = True
-
-    # expand the observations
-    list_observations = [dm_obs2gym_obs(obs) for obs in timestep.observation]
-    observations: dict[str, Any] = dict(zip(agents, list_observations))
-
-    # sometimes deepmind decides not to reward people
-    rewards: dict[str, float] = dict(zip(agents, repeat(0.0)))
-    if timestep.reward:
-        rewards = dict(zip(agents, timestep.reward))
-
-    # expand everything else
-    terminations: dict[str, bool] = dict(zip(agents, repeat(term)))
-    truncations: dict[str, bool] = dict(zip(agents, repeat(trunc)))
-
-    # duplicate infos
-    info = {
-        "timestep.discount": timestep.discount,
-        "timestep.step_type": timestep.step_type,
-    }
-    info: dict[str, Any] = dict(zip(agents, repeat(info)))
-
-    return (
-        observations,
-        rewards,
-        terminations,
-        truncations,
-        info,
+import pytest
+from dm_control.locomotion import soccer as dm_soccer
+from gymnasium.utils.env_checker import data_equivalence
+from pettingzoo.test import parallel_api_test
+
+from shimmy.dm_control_multiagent_compatibility import (
+    DmControlMultiAgentCompatibilityV0,
+)
+from shimmy.utils.dm_control_multiagent import load_dm_control_soccer
+
+TEAM_SIZE = [2, 5, 7]
+TIME_LIMITS = [0.0, 10.0]
+DISABLE_WALKER_CONTACTS = [True, False]
+ENABLE_FIELD_BOX = [True, False]
+TERMINATE_ON_GOAL = [True, False]
+WALKER_TYPE = [
+    dm_soccer.WalkerType.BOXHEAD,
+    dm_soccer.WalkerType.ANT,
+    dm_soccer.WalkerType.HUMANOID,
+]
+
+CONFIGS = []
+
+for val in TEAM_SIZE:
+    CONFIGS.append((val, None, None, None, None, None))
+
+for val in TIME_LIMITS:
+    CONFIGS.append((None, val, None, None, None, None))
+
+for val in DISABLE_WALKER_CONTACTS:
+    CONFIGS.append((None, None, val, None, None, None))
+
+for val in ENABLE_FIELD_BOX:
+    CONFIGS.append((None, None, None, val, None, None))
+
+for val in TERMINATE_ON_GOAL:
+    CONFIGS.append((None, None, None, None, val, None))
+
+for val in WALKER_TYPE:
+    CONFIGS.append((None, None, None, None, None, val))
+
+
+@pytest.mark.parametrize("config", CONFIGS)
+def test_loading_env(config):
+    """Tests the loading of all DM Control Soccer environments using the DmControlMultiAgentCompatibility wrapper."""
+    team_size, time_limit, disable_walker_contacts, enable_field_box, terminate_on_goal, walker_type = config  # fmt: skip
+
+    env = DmControlMultiAgentCompatibilityV0(
+        team_size=team_size,
+        time_limit=time_limit,
+        disable_walker_contacts=disable_walker_contacts,
+        enable_field_box=enable_field_box,
+        terminate_on_goal=terminate_on_goal,
+        walker_type=walker_type,
+        render_mode=None,
     )
 
+    parallel_api_test(env)
 
-class DmControlMultiAgentCompatibilityV0(ParallelEnv):
-    """This compatibility wrapper converts multi-agent dm-control environments, primarily soccer, into a Pettingzoo environment.
+    # run through the environment
+    env.reset()
+    while env.agents:
+        actions = {agent: env.action_space(agent).sample() for agent in env.agents}
+        obs1, rewards1, terminations1, truncations1, infos1 = env.step(actions)
+    env.close()
+
+
+@pytest.mark.parametrize("config", CONFIGS)
+def test_existing_env(config):
+    """Tests wrapping existing DM Control Soccer environments with the DmControlMultiAgentCompatibility wrapper."""
+    team_size, time_limit, disable_walker_contacts, enable_field_box, terminate_on_goal, walker_type = config  # fmt: skip
+    env = load_dm_control_soccer(
+        team_size,
+        time_limit,
+        disable_walker_contacts,
+        enable_field_box,
+        terminate_on_goal,
+        walker_type,
+    )
+
+    env = DmControlMultiAgentCompatibilityV0(env)
+
+    parallel_api_test(env)
+
+    env.close()
+
+
+@pytest.mark.parametrize("config", CONFIGS)
+def test_seeding(config):
+    """Tests the seeding of the DmControlMultiAgentCompatibility wrapper."""
+    team_size, time_limit, disable_walker_contacts, enable_field_box, terminate_on_goal, walker_type = config  # fmt: skip
 
-    Dm-control is DeepMind's software stack for physics-based simulation and Reinforcement Learning environments,
-    using MuJoCo physics. This compatibility wrapper converts a dm-control environment into a gymnasium environment.
-    """
-
-    metadata = {"render_modes": ["human"]}
-
-    def __init__(
-        self,
-        env: dm_control.composer.Environment,
-        render_mode: str | None = None,
-    ):
-        """Wrapper that converts a dm control multi-agent environment into a pettingzoo environment.
-
-        Due to how the underlying environment is setup, this environment is nondeterministic, so seeding doesn't work.
-
-        Args:
-            env (dm_env.Environment): dm control multi-agent environment
-            render_mode (Optional[str]): render_mode
-        """
-        super().__init__()
-        self._env = env
-        self.render_mode = render_mode
-
-        # get action and observation specs first
-        all_obs_spaces = [
-            dm_spec2gym_space(spec) for spec in self._env.observation_spec()
-        ]
-        all_act_spaces = [dm_spec2gym_space(spec) for spec in self._env.action_spec()]
-        num_players = len(all_obs_spaces)
-
-        # agent definitions
-        self.possible_agents = ["player_" + str(r) for r in range(num_players)]
-        self.agent_id_name_mapping = dict(zip(range(num_players), self.possible_agents))
-        self.agent_name_id_mapping = dict(zip(self.possible_agents, range(num_players)))
-
-        # the official spaces
-        self.obs_spaces = dict(zip(self.possible_agents, all_obs_spaces))
-        self.act_spaces = dict(zip(self.possible_agents, all_act_spaces))
-
-        if self.render_mode == "human":
-            self.viewer = MujocoRenderer(
-                self._env.physics.model.ptr, self._env.physics.data.ptr
-            )
-
-    @functools.lru_cache(maxsize=None)
-    def observation_space(self, agent):
-        """The observation space for agent."""
-        return self.obs_spaces[agent]
-
-    @functools.lru_cache(maxsize=None)
-    def action_space(self, agent):
-        """The action space for agent."""
-        return self.act_spaces[agent]
-
-    def render(self):
-        """Renders the environment."""
-        if self.render_mode is None:
-            gymnasium.logger.warn(
-                "You are calling render method without specifying any render mode."
-            )
-            return
-
-    def close(self):
-        """Closes the environment."""
-        self._env.physics.free()
-        self._env.close()
-
-        if hasattr(self, "viewer"):
-            self.viewer.close()
-
-    def reset(self, seed=None, return_info=False, options=None):
-        """Resets the dm-control environment."""
-        self.agents = self.possible_agents[:]
-        self.num_moves = 0
-
-        timestep = self._env.reset()
-
-        observations, _, _, _, infos = _unravel_ma_timestep(timestep, self.agents)
-
-        if not return_info:
-            return observations
-        else:
-            return observations, infos
-
-    def step(self, actions):
-        """Steps through all agents with the actions."""
-        # assert that the actions _must_ have actions for all agents
-        assert len(actions) == len(
-            self.agents
-        ), f"Must have actions for all {len(self.agents)} agents, currently only found {len(actions)}."
-
-        actions = actions.values()
-        timestep = self._env.step(actions)
-
-        obs, rewards, terminations, truncations, infos = _unravel_ma_timestep(
-            timestep, self.agents
-        )
+    env1 = load_dm_control_soccer(
+        team_size,
+        time_limit,
+        disable_walker_contacts,
+        enable_field_box,
+        terminate_on_goal,
+        walker_type,
+    )
+    env2 = load_dm_control_soccer(
+        team_size,
+        time_limit,
+        disable_walker_contacts,
+        enable_field_box,
+        terminate_on_goal,
+        walker_type,
+    )
+
+    env1 = DmControlMultiAgentCompatibilityV0(env1, render_mode=None)
+    env2 = DmControlMultiAgentCompatibilityV0(env2, render_mode=None)
+
+    env1.reset(seed=42)
+    env2.reset(seed=42)
+
+    for agent in env1.possible_agents:
+        env1.action_space(agent).seed(42)
+        env2.action_space(agent).seed(42)
+
+    while env1.agents:
+        actions1 = {agent: env1.action_space(agent).sample() for agent in env1.agents}
+        actions2 = {agent: env2.action_space(agent).sample() for agent in env2.agents}
+
+        assert data_equivalence(actions1, actions2), "Incorrect action seeding"
+
+        obs1, rewards1, terminations1, truncations1, infos1 = env1.step(actions1)
+        obs2, rewards2, terminations2, truncations2, infos2 = env2.step(actions2)
+
+        assert data_equivalence(obs1, obs2)
+        assert data_equivalence(rewards1, rewards2), "Incorrect values for rewards"
+        assert data_equivalence(terminations1, terminations2), "Incorrect terminations."
+        assert data_equivalence(truncations1, truncations2), "Incorrect truncations"
+        assert data_equivalence(infos1, infos2), "Incorrect infos"
+    env1.close()
+    env2.close()
+
+
+@pytest.mark.skip(reason="Cannot pickle weakref objects used in dm_soccer envs.")
+@pytest.mark.parametrize("config", CONFIGS)
+def test_pickle(config):
+    """Tests that environments using the DmControlMultiAgentCompatibility wrapper can be serialized and deserialized via pickle."""
+    team_size, time_limit, disable_walker_contacts, enable_field_box, terminate_on_goal, walker_type = config  # fmt: skip
+    env1 = load_dm_control_soccer(
+        team_size,
+        time_limit,
+        disable_walker_contacts,
+        enable_field_box,
+        terminate_on_goal,
+        walker_type,
+    )
 
-        if self.render_mode == "human":
-            self.viewer.render(self.render_mode)
+    env1 = DmControlMultiAgentCompatibilityV0(env1, render_mode=None)
+    env2 = pickle.loads(pickle.dumps(env1))
 
-        if any(terminations.values()) or any(truncations.values()):
-            self.agents = []
+    env1.reset(seed=42)
+    env2.reset(seed=42)
 
-        return obs, rewards, terminations, truncations, infos
+    for agent in env1.possible_agents:
+        env1.action_space(agent).seed(42)
+        env2.action_space(agent).seed(42)
+
+    while env1.agents:
+        actions1 = {agent: env1.action_space(agent).sample() for agent in env1.agents}
+        actions2 = {agent: env2.action_space(agent).sample() for agent in env2.agents}
+
+        assert data_equivalence(actions1, actions2), "Incorrect action seeding"
+
+        obs1, rewards1, terminations1, truncations1, infos1 = env1.step(actions1)
+        obs2, rewards2, terminations2, truncations2, infos2 = env2.step(actions2)
+
+        assert data_equivalence(obs1, obs2), "Incorrect observations"
+        assert data_equivalence(rewards1, rewards2), "Incorrect values for rewards"
+        assert data_equivalence(terminations1, terminations2), "Incorrect terminations."
+        assert data_equivalence(truncations1, truncations2), "Incorrect truncations"
+        assert data_equivalence(infos1, infos2), "Incorrect infos"
+    env1.close()
+    env2.close()
```

### Comparing `Shimmy-0.2.1/shimmy/openai_gym_compatibility.py` & `Shimmy-1.0.0/shimmy/openai_gym_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Compatibility wrappers for OpenAI gym V22 and V26."""
+"""Compatibility wrappers for OpenAI gym V21 and V26."""
 # pyright: reportGeneralTypeIssues=false, reportPrivateImportUsage=false
 from __future__ import annotations
 
 import sys
 from typing import Any
 
 import gymnasium
@@ -234,18 +234,20 @@
 
         # Options are ignored - https://github.com/openai/gym/blob/c755d5c35a25ab118746e2ba885894ff66fb8c43/gym/core.py
         if options is not None:
             warn(
                 f"Gym v21 environment do not accept options as a reset parameter, options={options}"
             )
 
+        obs = self.gym_env.reset()
+
         if self.render_mode == "human":
             self.render()
 
-        return self.gym_env.reset(), {}
+        return obs, {}
 
     def step(self, action: ActType) -> tuple[Any, float, bool, bool, dict]:
         """Steps through the environment.
 
         Args:
             action: action to step through the environment with
```

### Comparing `Shimmy-0.2.1/shimmy/openspiel_compatibility.py` & `Shimmy-1.0.0/shimmy/openspiel_compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,140 +1,175 @@
-"""Wrapper to convert a openspiel environment into a pettingzoo compatible environment."""
+"""Wrapper to convert an OpenSpiel environment into a pettingzoo compatible environment."""
 from __future__ import annotations
 
 import functools
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
 import numpy as np
 import pettingzoo as pz
 import pyspiel
 from gymnasium import spaces
-from gymnasium.utils import seeding
-from pettingzoo.utils.env import AgentID
+from gymnasium.utils import EzPickle, seeding
+from pettingzoo.utils.env import AgentID, ObsType
 
 
-class OpenspielCompatibilityV0(pz.AECEnv):
-    """This compatibility wrapper that converts an openspiel environment into a pettingzoo environment.
+class OpenSpielCompatibilityV0(pz.AECEnv, EzPickle):
+    """This compatibility wrapper converts an OpenSpiel environment into a PettingZoo environment.
 
     OpenSpiel is a collection of environments and algorithms for research in general reinforcement learning
     and search/planning in games. OpenSpiel supports n-player (single- and multi- agent) zero-sum,
     cooperative and general-sum, one-shot and sequential, strictly turn-taking and simultaneous-move,
     perfect and imperfect information games, as well as traditional multiagent environments such as
     (partially- and fully- observable) grid worlds and social dilemmas.
     """
 
-    metadata = {"render_modes": []}
+    metadata = {
+        "render_modes": ["human"],
+        "name": "OpenSpielCompatibilityV0",
+        "is_parallelizable": False,
+    }
 
     def __init__(
         self,
-        game: pyspiel.Game,
-        render_mode: str | None,
+        env: pyspiel.Game | None = None,
+        game_name: str | None = None,
+        render_mode: str | None = None,
     ):
-        """Wrapper that converts a openspiel environment into a pettingzoo environment.
+        """Wrapper to convert a OpenSpiel environment into a PettingZoo environment.
 
         Args:
-            game (pyspiel.Game): game
-            render_mode (Optional[str]): render_mode
+            env (Optional[pyspiel.Game]): existing OpenSpiel environment to wrap
+            game_name (Optional[str]): name of OpenSpiel game to load
+            render_mode (Optional[str]): rendering mode
         """
+        EzPickle.__init__(self, env, game_name, render_mode)
         super().__init__()
-        self.game = game
+
+        # Only one of game_name and env can be provided, the other should be None
+        if env is None and game_name is None:
+            raise ValueError(
+                "No environment provided. Use `env` to specify an existing environment, or load an environment with `game_name`."
+            )
+        elif env is not None and game_name is not None:
+            raise ValueError(
+                "Two environments provided. Use `env` to specify an existing environment, or load an environment with `game_name`."
+            )
+        elif game_name is not None:
+            self._env = pyspiel.load_game(game_name)
+        elif env is not None:
+            self._env = env
+
         self.possible_agents = [
-            "player_" + str(r) for r in range(self.game.num_players())
+            "player_" + str(r) for r in range(self._env.num_players())
         ]
         self.agent_id_name_mapping = dict(
-            zip(range(self.game.num_players()), self.possible_agents)
+            zip(range(self._env.num_players()), self.possible_agents)
         )
         self.agent_name_id_mapping = dict(
-            zip(self.possible_agents, range(self.game.num_players()))
+            zip(self.possible_agents, range(self._env.num_players()))
         )
 
-        self.game_type = self.game.get_type()
+        self.game_type = self._env.get_type()
 
         self.render_mode = render_mode
 
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent: AgentID):
         """observation_space.
 
         We get the observation space from the underlying game.
         OpenSpiel possibly provides information and observation in several forms.
         This wrapper chooses which one to use depending on the following precedence:
-            1. Observation Tensor
-            2. Information Tensor
-            3. Observation String
-            4. Information String
+        1. Observation Tensor
+        2. Information Tensor
+        3. Observation String
+        4. Information String
 
         Args:
             agent (AgentID): agent
         """
         if self.game_type.provides_observation_tensor:
             return spaces.Box(
                 low=-np.inf,
                 high=np.inf,
-                shape=self.game.observation_tensor_shape(),
+                shape=self._env.observation_tensor_shape(),
                 dtype=np.float64,
             )
         elif self.game_type.provides_information_state_tensor:
             return spaces.Box(
                 low=-np.inf,
                 high=np.inf,
-                shape=self.game.information_state_tensor_shape(),
+                shape=self._env.information_state_tensor_shape(),
                 dtype=np.float64,
             )
         elif (
             self.game_type.provides_information_state_string
             or self.game_type.provides_observation_string
         ):
             return spaces.Text(max_length=2**16)
         else:
             raise NotImplementedError(
-                f"No information/observation tensor/string implemented for {self.game}."
+                f"No information/observation tensor/string implemented for {self._env}."
             )
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent: AgentID):
         """action_space.
 
+        Get the action space from the underlying OpenSpiel game.
+
         Args:
             agent (AgentID): agent
+
+        Returns:
+            space
         """
         try:
-            return spaces.Discrete(self.game.num_distinct_actions())
+            return spaces.Discrete(self._env.num_distinct_actions())
         except pyspiel.SpielError as e:
             raise NotImplementedError(
-                f"{str(e)[:-1]} for action space for {self.game}."
+                f"{str(e)[:-1]} for action space for {self._env}."
             )
 
     def render(self):
-        """render."""
-        raise NotImplementedError("No render available for openspiel.")
+        """render.
 
-    def observe(self, agent: AgentID):
+        Print the current game state.
+        """
+        if not hasattr(self, "game_state"):
+            raise UserWarning(
+                "You must reset the environment using reset() before calling render()."
+            )
+
+        print(self.game_state)
+
+    def observe(self, agent: AgentID) -> ObsType:
         """observe.
 
         Args:
             agent (AgentID): agent
+
+        Returns:
+            observation
         """
         return self.observations[agent]
 
     def close(self):
         """close."""
         pass
 
     def reset(
         self,
         seed: int | None = None,
-        return_info: bool | None = False,
         options: dict | None = None,
     ):
         """reset.
 
         Args:
             seed (Optional[int]): seed
-            return_info (Optional[bool]): return_info
             options (Optional[Dict]): options
         """
         # initialize the seed
         self.np_random, seed = seeding.np_random(seed)
 
         # all agents
         self.agents = self.possible_agents[:]
@@ -145,15 +180,15 @@
         self.rewards = {a: 0 for a in self.agents}
         self.terminations = {a: False for a in self.agents}
         self.truncations = {a: False for a in self.agents}
         self.infos = {a: {} for a in self.agents}
 
         # get a new game state, game_length = number of game nodes
         self.game_length = 1
-        self.game_state = self.game.new_initial_state()
+        self.game_state = self._env.new_initial_state()
 
         # holders in case of simultaneous actions
         self.simultaneous_actions = dict()
 
         # step through chance nodes
         # then update obs and act masks
         # then choose next agent
@@ -173,15 +208,15 @@
         while self.game_state.is_chance_node():
             self.game_length += 1
             outcomes_with_probs = self.game_state.chance_outcomes()
             action_list, prob_list = zip(*outcomes_with_probs)
             action = self.np_random.choice(action_list, p=prob_list)
             self.game_state.apply_action(action)
 
-    def _execute_action_node(self, action: int):
+    def _execute_action_node(self, action: int | np.integer[Any]):
         """_execute_action_node.
 
         Advances the game state.
         We need to deal with 2 possible cases:
             - simultaneous game state where all the agents must step together
             - non-simultaneous game state where only one agent steps at a time
 
@@ -304,26 +339,26 @@
     def _update_termination_truncation(self):
         """Updates all terminations and truncations of the environment."""
         # check for terminal
         self.terminations = {a: self.terminations[a] for a in self.agents}
         if self.game_state.current_player() <= -4:
             self.terminations = {a: True for a in self.agents}
 
-        # check for action masks because openspiel doesn't do it themselves
+        # check for action masks because OpenSpiel doesn't do it themselves
         action_mask_sum = 0
         for agent in self.agents:
             action_mask_sum += np.sum(self.infos[agent]["action_mask"])
 
         # if all actions are illegal for all agents, declare terminal
         if action_mask_sum == 0:
             self.terminations = {a: True for a in self.agents}
 
         # check for truncation
         self.truncations = {a: self.truncations[a] for a in self.agents}
-        if self.game_length > self.game.max_game_length():
+        if self.game_length > self._env.max_game_length():
             self.truncations = {a: True for a in self.agents}
 
     def _end_routine(self):
         """Method that handles the routines that happen at environment termination.
 
         Since all agents end together we can hack our way around it.
         """
@@ -339,16 +374,18 @@
             self.truncations.pop(self.agent_selection)
             self.infos.pop(self.agent_selection)
 
             return True
 
         return False
 
-    def step(self, action: int):
-        """Steps the environment.
+    def step(self, action: int | np.integer[Any]):
+        """Steps.
+
+        Steps the agent with an action.
 
         Args:
             action (int): action
         """
         # handle the possibility of an end step
         if not self._end_routine():
             # step the environment
```

### Comparing `Shimmy-0.2.1/shimmy/registration.py` & `Shimmy-1.0.0/shimmy/registration.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,57 @@
 from typing import Any, Callable, Mapping, NamedTuple, Sequence
 
 import numpy as np
 from gymnasium.envs.registration import register, registry
 
 from shimmy.utils.envs_configs import (
     ALL_ATARI_GAMES,
+    BSUITE_ENVS,
     DM_CONTROL_MANIPULATION_ENVS,
     DM_CONTROL_SUITE_ENVS,
     LEGACY_ATARI_GAMES,
 )
 
 
+def _register_bsuite_envs():
+    """Registers all bsuite environments in gymnasium."""
+    try:
+        import bsuite
+    except ImportError:
+        return
+
+    from bsuite.environments import Environment
+
+    from shimmy.bsuite_compatibility import BSuiteCompatibilityV0
+
+    # Add generic environment support
+    def _make_bsuite_generic_env(env: Environment, render_mode: str):
+        return BSuiteCompatibilityV0(env, render_mode=render_mode)
+
+    register(
+        "bsuite/compatibility-env-v0",
+        _make_bsuite_generic_env,  # pyright: ignore[reportGeneralTypeIssues]
+    )
+
+    # register all prebuilt envs
+    def _make_bsuite_env(env_id: str, **env_kwargs: Mapping[str, Any]):
+        env = bsuite.load(env_id, env_kwargs)
+        return BSuiteCompatibilityV0(env)
+
+    # non deterministic envs
+    nondeterministic = ["deep_sea", "bandit", "discounting_chain"]
+
+    for env_id in BSUITE_ENVS:
+        register(
+            f"bsuite/{env_id}-v0",
+            partial(_make_bsuite_env, env_id=env_id),
+            nondeterministic=env_id in nondeterministic,
+        )
+
+
 def _register_dm_control_envs():
     """Registers all dm-control environments in gymnasium."""
     try:
         import dm_control
     except ImportError:
         return
 
@@ -237,15 +274,18 @@
 
     def _make_dm_lab_env(
         env_id: str, observations, config: dict[str, Any], renderer: str
     ):
         env = deepmind_lab.Lab(env_id, observations, config=config, renderer=renderer)
         return DmLabCompatibilityV0(env)
 
-    register(id="DmLabCompatibility-v0", entry_point=_make_dm_lab_env)
+    register(
+        id="DmLabCompatibility-v0",
+        entry_point=_make_dm_lab_env,  # pyright: ignore[reportGeneralTypeIssues]
+    )
 
 
 def register_gymnasium_envs():
     """This function is called when gymnasium is imported."""
     if "GymV26Environment-v0" in registry:
         registry.pop("GymV26Environment-v0")
     register(
@@ -255,10 +295,11 @@
     if "GymV21Environment-v0" in registry:
         registry.pop("GymV21Environment-v0")
     register(
         id="GymV21Environment-v0",
         entry_point="shimmy.openai_gym_compatibility:GymV21CompatibilityV0",
     )
 
+    _register_bsuite_envs()
     _register_dm_control_envs()
     _register_atari_envs()
     _register_dm_lab()
```

### Comparing `Shimmy-0.2.1/shimmy/utils/envs_configs.py` & `Shimmy-1.0.0/shimmy/utils/envs_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 """Environment configures."""
 
+BSUITE_ENVS = (
+    "bandit",
+    "bandit_noise",
+    "bandit_scale",
+    "cartpole",
+    "cartpole_noise",
+    "cartpole_scale",
+    "cartpole_swingup",
+    "catch",
+    "catch_noise",
+    "catch_scale",
+    "deep_sea",
+    "deep_sea_stochastic",
+    "discounting_chain",
+    "memory_len",
+    "memory_size",
+    "mnist",
+    "mnist_noise",
+    "mnist_scale",
+    "mountain_car",
+    "mountain_car_noise",
+    "mountain_car_scale",
+    "umbrella_distract",
+    "umbrella_length",
+)
+
 DM_CONTROL_SUITE_ENVS = (
     ("acrobot", "swingup"),
     ("acrobot", "swingup_sparse"),
     ("ball_in_cup", "catch"),
     ("cartpole", "balance"),
     ("cartpole", "balance_sparse"),
     ("cartpole", "swingup"),
```

### Comparing `Shimmy-0.2.1/tests/test_dm_control.py` & `Shimmy-1.0.0/tests/test_dm_control.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Tests the functionality of the DMEnvWrapper on dm_control envs."""
+"""Tests the functionality of the DmControlCompatibility Wrapper on dm_control envs."""
+import pickle
 import warnings
 from typing import Callable
 
 import dm_control.suite
 import gymnasium as gym
 import numpy as np
 import pytest
@@ -86,14 +87,44 @@
         # LQR fails this test currently.
         return
 
     obs_1, info_1 = env_1.reset(seed=42)
     obs_2, info_2 = env_2.reset(seed=42)
     assert data_equivalence(obs_1, obs_2)
     assert data_equivalence(info_1, info_2)
+    for _ in range(10):
+        actions = env_1.action_space.sample()
+        obs_1, reward_1, term_1, trunc_1, info_1 = env_1.step(actions)
+        obs_2, reward_2, term_2, trunc_2, info_2 = env_2.step(actions)
+        assert data_equivalence(obs_1, obs_2)
+        assert reward_1 == reward_2
+        assert term_1 == term_2 and trunc_1 == trunc_2
+        assert data_equivalence(info_1, info_2)
+
+    env_1.close()
+    env_2.close()
+
+
+@pytest.mark.skip(
+    reason="Fatal Python error: Segmentation fault (with or without EzPickle)"
+)
+@pytest.mark.parametrize("env_id", DM_CONTROL_ENV_IDS[0])
+def test_pickle(env_id):
+    """Test that dm-control seeding works."""
+    env_1 = gym.make(env_id)
+    env_2 = pickle.loads(pickle.dumps(env_1))
+
+    if "lqr" in env_id or (env_1.spec is not None and env_1.spec.nondeterministic):
+        # LQR fails this test currently.
+        return
+
+    obs_1, info_1 = env_1.reset(seed=42)
+    obs_2, info_2 = env_2.reset(seed=42)
+    assert data_equivalence(obs_1, obs_2)
+    assert data_equivalence(info_1, info_2)
     for _ in range(100):
         actions = env_1.action_space.sample()
         obs_1, reward_1, term_1, trunc_1, info_1 = env_1.step(actions)
         obs_2, reward_2, term_2, trunc_2, info_2 = env_2.step(actions)
         assert data_equivalence(obs_1, obs_2)
         assert reward_1 == reward_2
         assert term_1 == term_2 and trunc_1 == trunc_2
@@ -113,14 +144,50 @@
     )
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
+    env.close()
+
+
+@pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
+def test_rendering_multiple_cameras(height, width):
+    """Test that multi_camera rendering mode works for dm-control environments."""
+    env = gym.make(
+        DM_CONTROL_ENV_IDS[0],
+        render_mode="multi_camera",
+        render_height=height,
+        render_width=width,
+    )
+    env.reset()
+    frames = []
+    for _ in range(10):
+        frames.append(env.render())
+        env.step(env.action_space.sample())
+
+    env.close()
+
+
+@pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
+def test_rendering_depth(height, width):
+    """Test that depth rendering mode works for dm-control environments."""
+    env = gym.make(
+        DM_CONTROL_ENV_IDS[0],
+        render_mode="depth_array",
+        render_height=height,
+        render_width=width,
+    )
+    env.reset()
+    frames = []
+    for _ in range(10):
+        frames.append(env.render())
+        env.step(env.action_space.sample())
+
     env.close()
 
 
 @pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
 def test_render_height_widths(height, width):
     """Tests that dm-control rendering heights and widths works."""
     env = gym.make(
```

### Comparing `Shimmy-0.2.1/tests/test_gym.py` & `Shimmy-1.0.0/tests/test_gym.py`

 * *Files identical despite different names*

