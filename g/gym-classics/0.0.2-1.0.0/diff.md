# Comparing `tmp/gym-classics-0.0.2.tar.gz` & `tmp/gym-classics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-classics-0.0.2.tar", last modified: Thu Mar 16 06:48:39 2023, max compression
+gzip compressed data, was "gym-classics-1.0.0.tar", last modified: Tue May  2 00:15:25 2023, max compression
```

## Comparing `gym-classics-0.0.2.tar` & `gym-classics-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.580791 gym-classics-0.0.2/
--rw-r--r--   0 brett     (1000) brett     (1000)    35149 2023-02-28 12:05:08.000000 gym-classics-0.0.2/LICENSE
--rw-r--r--   0 brett     (1000) brett     (1000)    16738 2023-03-16 06:48:39.580791 gym-classics-0.0.2/PKG-INFO
--rw-r--r--   0 brett     (1000) brett     (1000)    16202 2023-03-16 06:47:13.000000 gym-classics-0.0.2/README.md
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.570791 gym-classics-0.0.2/gym_classics/
--rw-r--r--   0 brett     (1000) brett     (1000)     1638 2023-03-15 22:45:16.000000 gym-classics-0.0.2/gym_classics/__init__.py
--rw-r--r--   0 brett     (1000) brett     (1000)     2104 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/dynamic_programming.py
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.580791 gym-classics-0.0.2/gym_classics/envs/
--rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/__init__.py
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.580791 gym-classics-0.0.2/gym_classics/envs/abstract/
--rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/abstract/__init__.py
--rw-r--r--   0 brett     (1000) brett     (1000)     6216 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/abstract/base_env.py
--rw-r--r--   0 brett     (1000) brett     (1000)     2555 2023-03-15 21:00:33.000000 gym-classics-0.0.2/gym_classics/envs/abstract/gridworld.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1067 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/abstract/linear_walk.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1223 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/abstract/noisy_gridworld.py
--rw-r--r--   0 brett     (1000) brett     (1000)     4660 2023-03-16 06:40:16.000000 gym-classics-0.0.2/gym_classics/envs/abstract/racetrack.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1103 2023-03-16 06:47:13.000000 gym-classics-0.0.2/gym_classics/envs/classic_gridworld.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1064 2023-03-15 22:24:04.000000 gym-classics-0.0.2/gym_classics/envs/cliff_walk.py
--rw-r--r--   0 brett     (1000) brett     (1000)      826 2023-03-15 22:29:58.000000 gym-classics-0.0.2/gym_classics/envs/dyna_maze.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1054 2023-03-15 22:31:31.000000 gym-classics-0.0.2/gym_classics/envs/four_rooms.py
--rw-r--r--   0 brett     (1000) brett     (1000)     8146 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/jacks_car_rental.py
--rw-r--r--   0 brett     (1000) brett     (1000)      893 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/envs/linear_walks.py
--rw-r--r--   0 brett     (1000) brett     (1000)     3223 2023-03-15 22:48:17.000000 gym-classics-0.0.2/gym_classics/envs/racetracks.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1041 2023-03-15 21:28:58.000000 gym-classics-0.0.2/gym_classics/envs/sparse_gridworld.py
--rw-r--r--   0 brett     (1000) brett     (1000)     4061 2023-03-15 21:16:51.000000 gym-classics-0.0.2/gym_classics/envs/windy_gridworld.py
--rw-r--r--   0 brett     (1000) brett     (1000)     2327 2023-02-28 12:05:08.000000 gym-classics-0.0.2/gym_classics/utils.py
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.570791 gym-classics-0.0.2/gym_classics.egg-info/
--rw-r--r--   0 brett     (1000) brett     (1000)    16738 2023-03-16 06:48:39.000000 gym-classics-0.0.2/gym_classics.egg-info/PKG-INFO
--rw-r--r--   0 brett     (1000) brett     (1000)      960 2023-03-16 06:48:39.000000 gym-classics-0.0.2/gym_classics.egg-info/SOURCES.txt
--rw-r--r--   0 brett     (1000) brett     (1000)        1 2023-03-16 06:48:39.000000 gym-classics-0.0.2/gym_classics.egg-info/dependency_links.txt
--rw-r--r--   0 brett     (1000) brett     (1000)       19 2023-03-16 06:48:39.000000 gym-classics-0.0.2/gym_classics.egg-info/top_level.txt
--rw-r--r--   0 brett     (1000) brett     (1000)       38 2023-03-16 06:48:39.580791 gym-classics-0.0.2/setup.cfg
--rw-r--r--   0 brett     (1000) brett     (1000)      771 2023-03-16 06:47:13.000000 gym-classics-0.0.2/setup.py
-drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-03-16 06:48:39.580791 gym-classics-0.0.2/tests/
--rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-03-15 22:43:33.000000 gym-classics-0.0.2/tests/__init__.py
--rw-r--r--   0 brett     (1000) brett     (1000)     4729 2023-03-15 21:55:38.000000 gym-classics-0.0.2/tests/test_envs.py
--rw-r--r--   0 brett     (1000) brett     (1000)     5374 2023-02-28 12:05:08.000000 gym-classics-0.0.2/tests/test_model.py
--rw-r--r--   0 brett     (1000) brett     (1000)     1125 2023-02-28 12:05:08.000000 gym-classics-0.0.2/tests/test_policy_iteration.py
--rw-r--r--   0 brett     (1000) brett     (1000)     3001 2023-02-28 12:05:08.000000 gym-classics-0.0.2/tests/test_value_iteration.py
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.601968 gym-classics-1.0.0/
+-rw-r--r--   0 brett     (1000) brett     (1000)    35149 2023-02-28 12:05:08.000000 gym-classics-1.0.0/LICENSE
+-rw-r--r--   0 brett     (1000) brett     (1000)    17697 2023-05-02 00:15:25.601968 gym-classics-1.0.0/PKG-INFO
+-rw-r--r--   0 brett     (1000) brett     (1000)    17147 2023-05-02 00:13:11.000000 gym-classics-1.0.0/README.md
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.591968 gym-classics-1.0.0/gym_classics/
+-rw-r--r--   0 brett     (1000) brett     (1000)     2513 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/__init__.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     2104 2023-02-28 12:05:08.000000 gym-classics-1.0.0/gym_classics/dynamic_programming.py
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.601968 gym-classics-1.0.0/gym_classics/envs/
+-rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-02-28 12:05:08.000000 gym-classics-1.0.0/gym_classics/envs/__init__.py
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.601968 gym-classics-1.0.0/gym_classics/envs/abstract/
+-rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-02-28 12:05:08.000000 gym-classics-1.0.0/gym_classics/envs/abstract/__init__.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     6248 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/envs/abstract/base_env.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     2552 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/envs/abstract/gridworld.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1067 2023-02-28 12:05:08.000000 gym-classics-1.0.0/gym_classics/envs/abstract/linear_walk.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1225 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/envs/abstract/noisy_gridworld.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     4660 2023-03-16 06:40:16.000000 gym-classics-1.0.0/gym_classics/envs/abstract/racetrack.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1103 2023-03-16 06:47:13.000000 gym-classics-1.0.0/gym_classics/envs/classic_gridworld.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1064 2023-03-15 22:24:04.000000 gym-classics-1.0.0/gym_classics/envs/cliff_walk.py
+-rw-r--r--   0 brett     (1000) brett     (1000)      826 2023-03-15 22:29:58.000000 gym-classics-1.0.0/gym_classics/envs/dyna_maze.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1054 2023-03-15 22:31:31.000000 gym-classics-1.0.0/gym_classics/envs/four_rooms.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     7956 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/envs/jacks_car_rental.py
+-rw-r--r--   0 brett     (1000) brett     (1000)      893 2023-02-28 12:05:08.000000 gym-classics-1.0.0/gym_classics/envs/linear_walks.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     3223 2023-03-15 22:48:17.000000 gym-classics-1.0.0/gym_classics/envs/racetracks.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     1041 2023-03-15 21:28:58.000000 gym-classics-1.0.0/gym_classics/envs/sparse_gridworld.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     4061 2023-03-15 21:16:51.000000 gym-classics-1.0.0/gym_classics/envs/windy_gridworld.py
+-rw-r--r--   0 brett     (1000) brett     (1000)     2323 2023-05-02 00:13:11.000000 gym-classics-1.0.0/gym_classics/utils.py
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.591968 gym-classics-1.0.0/gym_classics.egg-info/
+-rw-r--r--   0 brett     (1000) brett     (1000)    17697 2023-05-02 00:15:25.000000 gym-classics-1.0.0/gym_classics.egg-info/PKG-INFO
+-rw-r--r--   0 brett     (1000) brett     (1000)      860 2023-05-02 00:15:25.000000 gym-classics-1.0.0/gym_classics.egg-info/SOURCES.txt
+-rw-r--r--   0 brett     (1000) brett     (1000)        1 2023-05-02 00:15:25.000000 gym-classics-1.0.0/gym_classics.egg-info/dependency_links.txt
+-rw-r--r--   0 brett     (1000) brett     (1000)       19 2023-05-02 00:15:25.000000 gym-classics-1.0.0/gym_classics.egg-info/top_level.txt
+-rw-r--r--   0 brett     (1000) brett     (1000)       38 2023-05-02 00:15:25.601968 gym-classics-1.0.0/setup.cfg
+-rw-r--r--   0 brett     (1000) brett     (1000)      785 2023-05-02 00:13:11.000000 gym-classics-1.0.0/setup.py
+drwxr-xr-x   0 brett     (1000) brett     (1000)        0 2023-05-02 00:15:25.601968 gym-classics-1.0.0/tests/
+-rw-r--r--   0 brett     (1000) brett     (1000)        0 2023-05-01 21:59:50.000000 gym-classics-1.0.0/tests/__init__.py
```

### Comparing `gym-classics-0.0.2/LICENSE` & `gym-classics-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/PKG-INFO` & `gym-classics-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gym-classics
-Version: 0.0.2
-Summary: Classic environments for reinforcement learning and dynamic programming, implemented in OpenAI Gym.
+Version: 1.0.0
+Summary: Classic environments for reinforcement learning and dynamic programming, implemented in OpenAI Gym and Gymnasium.
 Home-page: https://github.com/brett-daley/gym-classics
 Author: Brett Daley
 Author-email: brett.daley@ualberta.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gym Classics
-![pypi](https://img.shields.io/badge/pypi-0.0.2-blue)
+![pypi](https://img.shields.io/badge/pypi-1.0.0-blue)
 [![license](https://img.shields.io/badge/license-GPL%20v3.0-blue)](./LICENSE)
 ![python](https://img.shields.io/badge/python-3.5%2B-green)
 
 Gym Classics is a collection of well-known discrete MDPs from the reinforcement learning
 literature implemented as OpenAI Gym environments.
 API support for dynamic programming is also provided.
 
@@ -34,38 +34,23 @@
 
 1. [Example: Reinforcement Learning](#example-reinforcement-learning)
 
 1. [Example: Dynamic Programming](#example-dynamic-programming)
 
 1. [Environments Glossary](#environments-glossary)
 
-1. [References](#references)
-
-### Citing
-
-You can cite this repository in published work using the following bibtex:
-
-```
-@misc{daley2021gym,
-  author={Daley, Brett},
-  title={Gym Classics},
-  year={2021},
-  publisher={GitHub},
-  journal={GitHub repository},
-  howpublished={\url{https://github.com/brett-daley/gym-classics}},
-}
-```
+1. [Citing and References](#citing-and-references)
 
 ## Installation
 
 Prerequisites:
-- python 3.5+
-- gym
-- numpy
-- scipy (`JacksCarRental-v0` and `JacksCarRentalModified-v0` only)
+- Python 3.5+
+- `gym==0.26.2` or `gymnasium`
+- `numpy`
+- `scipy` (for `JacksCarRental` and `JacksCarRentalModified` only)
 
 ### Option 1: `pip`
 
 ```
 pip install gym-classics
 ```
 
@@ -77,45 +62,52 @@
 python setup.py install
 ```
 
 ---
 
 ## API Overview
 
-Once installed, the environments are automatically registered for `gym.make` by
-importing the `gym_classics` package in your Python script.
-The basic API is identical to that of OpenAI Gym.
+The basic API is identical to that of [OpenAI Gym](https://www.gymlibrary.dev/) (as of `0.26.2`) and [Gymnasium](https://gymnasium.farama.org/).
+The environments must be explictly registered for `gym.make` by
+importing the `gym_classics` package in your Python script and then calling `gym_classics.register('gym')` or `gym_classics.register('gymnasium')`, depending on which library you want to use as the backend.
+Note that registration cannot be changed after calling `register`, and mixing `gym` and `gymnasium` environments in a single script is not possible.
+
 A minimal working example:
 
 ```python
-import gym
+import gym                    # or `import gymnasium as gym`
 import gym_classics
+gym_classics.register('gym')  # or `gym_classics.register('gymnasium')`
 
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
+state, _ = env.reset(seed=0)
+
 for t in range(1, 100 + 1):
     action = env.action_space.sample()  # Select a random action
-    next_state, reward, done, info = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
     print("t={}, state={}, action={}, reward={}, next_state={}, done={}".format(
         t, state, action, reward, next_state, done))
-    state = next_state if not done else env.reset()
-env.close()
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
+
+env.close()  # Optional, not currently implemented by any environments
 ```
 
-Gym Classics also implements methods for querying a model of the environment.
+Gym Classics also implements methods for querying the model of the environment.
 The full interface of a Gym Classics environment therefore looks like this:
 
 ```yaml
 class Env:
     # Standard Gym API:
     - step(self, action)
-    - reset(self)
-    - render(self, mode='human')  # *currently not implemented by all environments*
+    - reset(self, seed=None, options=None)
+    - render(self)  # *currently not implemented by all environments*
     - close(self)
-    - seed(self, seed=None)
 
     # Extended Gym Classics API:
     - states(self)                # returns a generator over all feasible states
     - actions(self)               # returns a generator over all feasible actions
     - model(self, state, action)  # returns all transitions from the given state-action pair
 ```
 
@@ -123,76 +115,76 @@
 [Example: Dynamic Programming](#example-dynamic-programming).
 
 State and action spaces for all environments are type `gym.spaces.Discrete`.
 The size of these spaces can be queried as usual:
 `env.observation_space.n` and `env.action_space.n`.
 This means that states and actions are represented as unique integers, which is useful
 for advanced `numpy` indexing.
-Note that states and actions are enumerated in an arbitrary order for each environment.
+Note that states and actions are enumerated in an arbitrary but consistent order for each environment.
 
-> **Tip:** Gym Classics environments also implement private methods called `_encode` and `_decode` which convert states between their integral and human-interpretable forms.
+> **Tip:** Gym Classics environments also implement methods called `encode` and `decode` which convert states between their integer and human-interpretable forms.
 > These should never be used by the agent, but can be useful for displaying results or debugging.
 > See the abstract [BaseEnv](gym_classics/envs/abstract/base_env.py) class for implementation details.
 
 ## Example: Reinforcement Learning
 
 Let's test the classic Q-Learning algorithm [[4]](#references) on `ClassicGridworld-v0`.
 
 ```python
 import gym
 import gym_classics
+gym_classics.register('gym')
 import numpy as np
 
 # Hyperparameters for Q-Learning
 discount = 0.9
 epsilon = 0.5
 learning_rate = 0.025
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
+state, _ = env.reset(seed=0)
 
 # Our Q-function is a numpy array
 Q = np.zeros([env.observation_space.n, env.action_space.n])
 
 # Loop for 500k timesteps
 for _ in range(500000):
     # Select action from ε-greedy policy
-    if np.random.rand() < epsilon:
+    if env.np_random.random() < epsilon:
         action = env.action_space.sample()
     else:
         action = np.argmax(Q[state])
 
     # Step the environment
-    next_state, reward, done, _ = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
 
     # Q-Learning update:
     # Q(s,a) <-- Q(s,a) + α * (r + γ max_a' Q(s',a') - Q(s,a))
-    target = reward - Q[state, action]
+    td_error = reward - Q[state, action]
     if not done:
-        target += discount * np.max(Q[next_state])
-    Q[state, action] += learning_rate * target
+        td_error += discount * np.max(Q[next_state])
+    Q[state, action] += learning_rate * td_error
 
     # Reset the environment if we're done
-    state = env.reset() if done else next_state
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
 
 # Now let's see what the value function looks like after training:
 V = np.max(Q, axis=1)
 print(V)
 ```
 
 Output:
 
 ```
-[ 0.5618515   0.75169693  1.          0.49147301  0.26363411 -1.
-  0.58655406  0.51379727  0.86959422  0.43567445  0.64966203]
+[ 0.56303004  0.72570493  0.56160538  0.48701053 -1.          0.44497334
+  0.2242687   0.63966295  0.84551377  0.42840196  1.        ]
 ```
 
 These values seem reasonable, but in the next section, we will certify their correctness
 by using dynamic programming.
 
 ## Example: Dynamic Programming
 
@@ -257,44 +249,47 @@
 Value Iteration and other dynamic programming methods are already implemented in
 [dynamic_programming.py](gym_classics/dynamic_programming.py).
 Let's use Value Iteration to check that our Q-Learning implemention from
 [Example: Reinforcement Learning](#example-reinforcement-learning) is correct:
 
 ```python
 import gym
+import gym_classics
+gym_classics.register('gym')
 from gym_classics.dynamic_programming import value_iteration
 import numpy as np
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
 
 # Compute the near-optimal values with Value Iteration
 V_star = value_iteration(env, discount=0.9, precision=1e-9)
+print(V_star, end='\n\n')
 
 # Our Q-Learning values from earlier:
-V = [0.5618515,  0.75169693, 1.,         0.49147301, 0.26363411, -1.,
-     0.58655406, 0.51379727, 0.86959422, 0.43567445, 0.64966203]
+V = [0.56303004, 0.72570493, 0.56160538, 0.48701053, -1., 0.44497334,
+     0.2242687,  0.63966295, 0.84551377, 0.42840196, 1.]
 
 # Root Mean Square error:
-print("RMS error: {}".format(np.sqrt(np.square(V - V_star).mean())))
+rms_error = np.sqrt(np.mean(np.square(V - V_star)))
+print("RMS error:", rms_error)
 
 # Maximum absolute difference:
-print("Max abs diff: {}".format(np.abs(V - V_star).max()))
+max_abs_diff = np.max(np.abs(V - V_star))
+print("Maximum absolute difference:", max_abs_diff)
 ```
 
 Output:
 
 ```
-RMS error: 0.014976847878141084
-Max abs diff: 0.03832613967716292
+[ 0.56631445  0.74438015  0.57185903  0.49068396 -1.          0.47547113
+  0.27729584  0.64496924  0.84776628  0.43084446  1.        ]
+
+RMS error: 0.01967779454940685
+Maximum absolute difference: 0.053027139347779195
 ```
 
 Both error metrics are very close to zero;
 we can conclude that our Q-Learning implementation
 is working!
 
 ## Environments Glossary
@@ -316,15 +311,30 @@
 | 13 | `WindyGridworldKings-v0` | Same as `WindyGridworld` but with diagonal "King's" moves permitted.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 4 cardinal directions and 4 intermediate directions. |
 | 14 | `WindyGridworldKingsNoOp-v0` | Same as `WindyGridworldKings` but with an extra "no-op" (do nothing) action.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 8 cardinal/intermediate directions or take a no-op action. |
 | 15 | `WindyGridworldKingsStochastic-v0` | Same as `WindyGridworldKings` but windy cells exhibit stochastic behavior: -1, +0, or +1 wind strength with probability 1/3 each.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.10). |
 
 
 ---
 
-## References
+## Citing and References
+
+You can cite this repository in published work using the following bibtex:
+
+```
+@misc{daley2021gym,
+  author={Daley, Brett},
+  title={Gym Classics},
+  year={2021},
+  publisher={GitHub},
+  journal={GitHub repository},
+  howpublished={\url{https://github.com/brett-daley/gym-classics}},
+}
+```
+
+### References
 
 1. [Russell & Norvig. Artificial Intelligence: A Modern Approach. 2009, 3rd Ed.](https://cs.calvin.edu/courses/cs/344/kvlinden/resources/AIMA-3rd-edition.pdf)
 
 1. [Sutton, Precup, & Singh. Between MDPs and Semi-MDPs: A Framework for Temporal Abstraction in Reinforcement Learning. 1999.](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf)
 
 1. [Sutton & Barto. Reinforcement Learning: An Introduction. 2018, 2nd Ed.](http://incompleteideas.net/book/RLbook2020.pdf)
```

### Comparing `gym-classics-0.0.2/README.md` & `gym-classics-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Gym Classics
-![pypi](https://img.shields.io/badge/pypi-0.0.2-blue)
+![pypi](https://img.shields.io/badge/pypi-1.0.0-blue)
 [![license](https://img.shields.io/badge/license-GPL%20v3.0-blue)](./LICENSE)
 ![python](https://img.shields.io/badge/python-3.5%2B-green)
 
 Gym Classics is a collection of well-known discrete MDPs from the reinforcement learning
 literature implemented as OpenAI Gym environments.
 API support for dynamic programming is also provided.
 
@@ -20,38 +20,23 @@
 
 1. [Example: Reinforcement Learning](#example-reinforcement-learning)
 
 1. [Example: Dynamic Programming](#example-dynamic-programming)
 
 1. [Environments Glossary](#environments-glossary)
 
-1. [References](#references)
-
-### Citing
-
-You can cite this repository in published work using the following bibtex:
-
-```
-@misc{daley2021gym,
-  author={Daley, Brett},
-  title={Gym Classics},
-  year={2021},
-  publisher={GitHub},
-  journal={GitHub repository},
-  howpublished={\url{https://github.com/brett-daley/gym-classics}},
-}
-```
+1. [Citing and References](#citing-and-references)
 
 ## Installation
 
 Prerequisites:
-- python 3.5+
-- gym
-- numpy
-- scipy (`JacksCarRental-v0` and `JacksCarRentalModified-v0` only)
+- Python 3.5+
+- `gym==0.26.2` or `gymnasium`
+- `numpy`
+- `scipy` (for `JacksCarRental` and `JacksCarRentalModified` only)
 
 ### Option 1: `pip`
 
 ```
 pip install gym-classics
 ```
 
@@ -63,45 +48,52 @@
 python setup.py install
 ```
 
 ---
 
 ## API Overview
 
-Once installed, the environments are automatically registered for `gym.make` by
-importing the `gym_classics` package in your Python script.
-The basic API is identical to that of OpenAI Gym.
+The basic API is identical to that of [OpenAI Gym](https://www.gymlibrary.dev/) (as of `0.26.2`) and [Gymnasium](https://gymnasium.farama.org/).
+The environments must be explictly registered for `gym.make` by
+importing the `gym_classics` package in your Python script and then calling `gym_classics.register('gym')` or `gym_classics.register('gymnasium')`, depending on which library you want to use as the backend.
+Note that registration cannot be changed after calling `register`, and mixing `gym` and `gymnasium` environments in a single script is not possible.
+
 A minimal working example:
 
 ```python
-import gym
+import gym                    # or `import gymnasium as gym`
 import gym_classics
+gym_classics.register('gym')  # or `gym_classics.register('gymnasium')`
 
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
+state, _ = env.reset(seed=0)
+
 for t in range(1, 100 + 1):
     action = env.action_space.sample()  # Select a random action
-    next_state, reward, done, info = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
     print("t={}, state={}, action={}, reward={}, next_state={}, done={}".format(
         t, state, action, reward, next_state, done))
-    state = next_state if not done else env.reset()
-env.close()
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
+
+env.close()  # Optional, not currently implemented by any environments
 ```
 
-Gym Classics also implements methods for querying a model of the environment.
+Gym Classics also implements methods for querying the model of the environment.
 The full interface of a Gym Classics environment therefore looks like this:
 
 ```yaml
 class Env:
     # Standard Gym API:
     - step(self, action)
-    - reset(self)
-    - render(self, mode='human')  # *currently not implemented by all environments*
+    - reset(self, seed=None, options=None)
+    - render(self)  # *currently not implemented by all environments*
     - close(self)
-    - seed(self, seed=None)
 
     # Extended Gym Classics API:
     - states(self)                # returns a generator over all feasible states
     - actions(self)               # returns a generator over all feasible actions
     - model(self, state, action)  # returns all transitions from the given state-action pair
 ```
 
@@ -109,76 +101,76 @@
 [Example: Dynamic Programming](#example-dynamic-programming).
 
 State and action spaces for all environments are type `gym.spaces.Discrete`.
 The size of these spaces can be queried as usual:
 `env.observation_space.n` and `env.action_space.n`.
 This means that states and actions are represented as unique integers, which is useful
 for advanced `numpy` indexing.
-Note that states and actions are enumerated in an arbitrary order for each environment.
+Note that states and actions are enumerated in an arbitrary but consistent order for each environment.
 
-> **Tip:** Gym Classics environments also implement private methods called `_encode` and `_decode` which convert states between their integral and human-interpretable forms.
+> **Tip:** Gym Classics environments also implement methods called `encode` and `decode` which convert states between their integer and human-interpretable forms.
 > These should never be used by the agent, but can be useful for displaying results or debugging.
 > See the abstract [BaseEnv](gym_classics/envs/abstract/base_env.py) class for implementation details.
 
 ## Example: Reinforcement Learning
 
 Let's test the classic Q-Learning algorithm [[4]](#references) on `ClassicGridworld-v0`.
 
 ```python
 import gym
 import gym_classics
+gym_classics.register('gym')
 import numpy as np
 
 # Hyperparameters for Q-Learning
 discount = 0.9
 epsilon = 0.5
 learning_rate = 0.025
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
+state, _ = env.reset(seed=0)
 
 # Our Q-function is a numpy array
 Q = np.zeros([env.observation_space.n, env.action_space.n])
 
 # Loop for 500k timesteps
 for _ in range(500000):
     # Select action from ε-greedy policy
-    if np.random.rand() < epsilon:
+    if env.np_random.random() < epsilon:
         action = env.action_space.sample()
     else:
         action = np.argmax(Q[state])
 
     # Step the environment
-    next_state, reward, done, _ = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
 
     # Q-Learning update:
     # Q(s,a) <-- Q(s,a) + α * (r + γ max_a' Q(s',a') - Q(s,a))
-    target = reward - Q[state, action]
+    td_error = reward - Q[state, action]
     if not done:
-        target += discount * np.max(Q[next_state])
-    Q[state, action] += learning_rate * target
+        td_error += discount * np.max(Q[next_state])
+    Q[state, action] += learning_rate * td_error
 
     # Reset the environment if we're done
-    state = env.reset() if done else next_state
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
 
 # Now let's see what the value function looks like after training:
 V = np.max(Q, axis=1)
 print(V)
 ```
 
 Output:
 
 ```
-[ 0.5618515   0.75169693  1.          0.49147301  0.26363411 -1.
-  0.58655406  0.51379727  0.86959422  0.43567445  0.64966203]
+[ 0.56303004  0.72570493  0.56160538  0.48701053 -1.          0.44497334
+  0.2242687   0.63966295  0.84551377  0.42840196  1.        ]
 ```
 
 These values seem reasonable, but in the next section, we will certify their correctness
 by using dynamic programming.
 
 ## Example: Dynamic Programming
 
@@ -243,44 +235,47 @@
 Value Iteration and other dynamic programming methods are already implemented in
 [dynamic_programming.py](gym_classics/dynamic_programming.py).
 Let's use Value Iteration to check that our Q-Learning implemention from
 [Example: Reinforcement Learning](#example-reinforcement-learning) is correct:
 
 ```python
 import gym
+import gym_classics
+gym_classics.register('gym')
 from gym_classics.dynamic_programming import value_iteration
 import numpy as np
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
 
 # Compute the near-optimal values with Value Iteration
 V_star = value_iteration(env, discount=0.9, precision=1e-9)
+print(V_star, end='\n\n')
 
 # Our Q-Learning values from earlier:
-V = [0.5618515,  0.75169693, 1.,         0.49147301, 0.26363411, -1.,
-     0.58655406, 0.51379727, 0.86959422, 0.43567445, 0.64966203]
+V = [0.56303004, 0.72570493, 0.56160538, 0.48701053, -1., 0.44497334,
+     0.2242687,  0.63966295, 0.84551377, 0.42840196, 1.]
 
 # Root Mean Square error:
-print("RMS error: {}".format(np.sqrt(np.square(V - V_star).mean())))
+rms_error = np.sqrt(np.mean(np.square(V - V_star)))
+print("RMS error:", rms_error)
 
 # Maximum absolute difference:
-print("Max abs diff: {}".format(np.abs(V - V_star).max()))
+max_abs_diff = np.max(np.abs(V - V_star))
+print("Maximum absolute difference:", max_abs_diff)
 ```
 
 Output:
 
 ```
-RMS error: 0.014976847878141084
-Max abs diff: 0.03832613967716292
+[ 0.56631445  0.74438015  0.57185903  0.49068396 -1.          0.47547113
+  0.27729584  0.64496924  0.84776628  0.43084446  1.        ]
+
+RMS error: 0.01967779454940685
+Maximum absolute difference: 0.053027139347779195
 ```
 
 Both error metrics are very close to zero;
 we can conclude that our Q-Learning implementation
 is working!
 
 ## Environments Glossary
@@ -302,15 +297,30 @@
 | 13 | `WindyGridworldKings-v0` | Same as `WindyGridworld` but with diagonal "King's" moves permitted.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 4 cardinal directions and 4 intermediate directions. |
 | 14 | `WindyGridworldKingsNoOp-v0` | Same as `WindyGridworldKings` but with an extra "no-op" (do nothing) action.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 8 cardinal/intermediate directions or take a no-op action. |
 | 15 | `WindyGridworldKingsStochastic-v0` | Same as `WindyGridworldKings` but windy cells exhibit stochastic behavior: -1, +0, or +1 wind strength with probability 1/3 each.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.10). |
 
 
 ---
 
-## References
+## Citing and References
+
+You can cite this repository in published work using the following bibtex:
+
+```
+@misc{daley2021gym,
+  author={Daley, Brett},
+  title={Gym Classics},
+  year={2021},
+  publisher={GitHub},
+  journal={GitHub repository},
+  howpublished={\url{https://github.com/brett-daley/gym-classics}},
+}
+```
+
+### References
 
 1. [Russell & Norvig. Artificial Intelligence: A Modern Approach. 2009, 3rd Ed.](https://cs.calvin.edu/courses/cs/344/kvlinden/resources/AIMA-3rd-edition.pdf)
 
 1. [Sutton, Precup, & Singh. Between MDPs and Semi-MDPs: A Framework for Temporal Abstraction in Reinforcement Learning. 1999.](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf)
 
 1. [Sutton & Barto. Reinforcement Learning: An Introduction. 2018, 2nd Ed.](http://incompleteideas.net/book/RLbook2020.pdf)
```

### Comparing `gym-classics-0.0.2/gym_classics/dynamic_programming.py` & `gym-classics-1.0.0/gym_classics/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/abstract/base_env.py` & `gym-classics-1.0.0/gym_classics/envs/abstract/base_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from abc import ABCMeta, abstractmethod
 
-import gym
-from gym.spaces import Discrete
-from gym.utils import seeding
 import numpy as np
 
+import gym_classics
 
-class BaseEnv(gym.Env, metaclass=ABCMeta):
+
+if gym_classics._backend == 'gym':
+     from gym import Env
+     from gym.spaces import Discrete
+elif gym_classics._backend == 'gymnasium':
+    from gymnasium import Env
+    from gymnasium.spaces import Discrete
+
+
+class BaseEnv(Env, metaclass=ABCMeta):
     """Abstract base class for shared functionality between all environments."""
 
     def __init__(self, starts, n_actions, reachable_states=None):
         self._starts = tuple(starts)
         self.action_space = Discrete(n_actions)
+        self.np_random = None  # Initialized by calling reset()
 
-        self._state = None
+        self.state = None
         self._transition_cache = {}
 
         if reachable_states is None:
             # Get reachable states by searching through the state space
             self._reachable_states = set()
             for s in self._starts:
                 self._search(s, self._reachable_states)
@@ -32,46 +40,43 @@
         i = 0
         for state in self._reachable_states:
             self._encoder[state] = i
             self._decoder[i] = state
             i += 1
         self.observation_space = Discrete(i)
 
-        # Initialize the np_random module (user can override the seed later if desired)
-        self.seed()
-
-        self._use_sparse_model = False  # Set True for debug only
-
     def _search(self, state, visited):
         """A recursive depth-first search that adds all reachable states to the visited set."""
         visited.add(state)
         for a in self.actions():
             for transition in self._generate_transitions(state, a):
                 next_state, _, done, prob = transition
                 if prob > 0.0:
                     if not done and next_state not in visited:
                         self._search(next_state, visited)
 
-    def seed(self, seed=None):
-        self.np_random, seed = seeding.np_random(seed)
-        self.action_space.seed(seed)
-        return [seed]
+    def reset(self, seed=None, options=None):
+        if self.np_random is None and seed is None:
+            seed = np.random.default_rng().integers(2**32)
+
+        if seed is not None:
+            self.action_space.seed(seed)
+            self.np_random = np.random.default_rng(seed)
 
-    def reset(self):
         i = self.np_random.choice(len(self._starts))
-        self._state = self._starts[i]
-        return self._encode(self._state)
+        self.state = self._starts[i]
+        return self.encode(self.state), {}
 
     def step(self, action):
         assert self.action_space.contains(action)
-        state = self._state
+        state = self.state
         elements = self._sample_random_elements(state, action)
         next_state, reward, done, _ = self._deterministic_step(state, action, *elements)
-        self._state = next_state
-        return self._encode(next_state), reward, done, {}
+        self.state = next_state
+        return self.encode(next_state), reward, done, False, {}
 
     def _sample_random_elements(self, state, action):
         """Samples values for random elements (if any) that influence the environment
         transition from the current state-action pair (S, A).
 
         If the environment is deterministic, no need to override this method.
         """
@@ -107,23 +112,23 @@
         """Returns True if this (S,A,S') outcome should terminate, False otherwise."""
         raise NotImplementedError
 
     def states(self):
         """Returns a generator over all possible environment states."""
         return range(self.observation_space.n)
 
-    def _encode(self, state):
+    def encode(self, state):
         """Converts a raw state into a unique integer."""
         return self._encoder[state]
 
-    def _decode(self, i):
+    def decode(self, i):
         """Reverts an encoded integer back to its raw state."""
         return self._decoder[i]
 
-    def _is_reachable(self, state):
+    def is_reachable(self, state):
         """Returns True if the state can be reached from at least one start location,
         False otherwise."""
         return state in self._reachable_states
 
     def actions(self):
         """Returns a generator over all possible agent actions."""
         return range(self.action_space.n)
@@ -136,29 +141,25 @@
 
         n = self.observation_space.n
         next_states = np.arange(n)
         dones = np.zeros(n)
         rewards = np.zeros(n)
         probabilities = np.zeros(n)
 
-        for ns, r, d, p in self._generate_transitions(self._decode(state), action):
-            ns = self._encode(ns)
+        for ns, r, d, p in self._generate_transitions(self.decode(state), action):
+            ns = self.encode(ns)
             dones[ns] = float(d)
             rewards[ns] = r
             probabilities[ns] += p
 
         assert (probabilities >= 0.0).all(), "transition probabilities must be nonnegative"
         assert abs(probabilities.sum() - 1.0) <= 0.01, "transition probabilities must sum to 1"
 
-        if not self._use_sparse_model:
-            i = np.nonzero(probabilities)
-            transition = (next_states[i], rewards[i], dones[i], probabilities[i])
-        else:
-            transition = (next_states, rewards, dones, probabilities)
-
+        i = np.nonzero(probabilities)
+        transition = (next_states[i], rewards[i], dones[i], probabilities[i])
         self._transition_cache[sa_pair] = transition
         return transition
 
     @abstractmethod
     def _generate_transitions(self, state, action):
         """Returns a generator over all transitions from this state-action pair.
```

### Comparing `gym-classics-0.0.2/gym_classics/envs/abstract/gridworld.py` & `gym-classics-1.0.0/gym_classics/envs/abstract/gridworld.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from gym_classics.envs.abstract.base_env import BaseEnv
 
 
 class Gridworld(BaseEnv):
     """Abstract class for creating gridworld-type environments."""
 
     def __init__(self, layout_string, n_actions=None):
-        self._dims, starts, self._goals, self._blocks = parse_gridworld(layout_string)
+        self.dims, starts, self._goals, self._blocks = parse_gridworld(layout_string)
 
         if n_actions is None:
             n_actions = 4
         super().__init__(starts, n_actions)
 
     def _next_state(self, state, action):
         next_state = self._move(state, action)
@@ -25,16 +25,16 @@
             2: (x,   y-1),  # Down
             3: (x-1, y)     # Left
         }[action]
 
     def _clamp(self, state):
         """Clamps the state within the grid dimensions."""
         x, y = state
-        x = max(0, min(x, self._dims[0] - 1))
-        y = max(0, min(y, self._dims[1] - 1))
+        x = max(0, min(x, self.dims[0] - 1))
+        y = max(0, min(y, self.dims[1] - 1))
         return (x, y)
 
     def _is_blocked(self, state):
         """Returns True if this state cannot be occupied, False otherwise."""
         return state in self._blocks
 
     def _generate_transitions(self, state, action):
```

### Comparing `gym-classics-0.0.2/gym_classics/envs/abstract/linear_walk.py` & `gym-classics-1.0.0/gym_classics/envs/abstract/linear_walk.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/abstract/noisy_gridworld.py` & `gym-classics-1.0.0/gym_classics/envs/abstract/noisy_gridworld.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def _next_state(self, state, action, noisy_action):
         next_state, _ = super()._next_state(state, noisy_action)
         if action == noisy_action:
             return next_state, 0.8
         return next_state, 0.1
 
     def _noisy_action(self, action):
-        p = self.np_random.rand()
+        p = self.np_random.random()
         # 10% chance: rotate the action clockwise
         if 0.8 <= p < 0.9:
             action += 1
         # 10% chance: rotate the action counter-clockwise
         elif 0.9 <= p:
             action -= 1
         return action % self.action_space.n
```

### Comparing `gym-classics-0.0.2/gym_classics/envs/abstract/racetrack.py` & `gym-classics-1.0.0/gym_classics/envs/abstract/racetrack.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/classic_gridworld.py` & `gym-classics-1.0.0/gym_classics/envs/classic_gridworld.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/cliff_walk.py` & `gym-classics-1.0.0/gym_classics/envs/cliff_walk.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/dyna_maze.py` & `gym-classics-1.0.0/gym_classics/envs/dyna_maze.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/four_rooms.py` & `gym-classics-1.0.0/gym_classics/envs/four_rooms.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/jacks_car_rental.py` & `gym-classics-1.0.0/gym_classics/envs/jacks_car_rental.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,49 +33,39 @@
         self._lot2_requests_distr = TruncatedPoisson(4)
         self._lot2_dropoffs_distr = TruncatedPoisson(2)
 
         # Precompute the factored transition and reward functions for both lots
         self.P1, self.R1 = open_to_close(self._lot1_requests_distr, self._lot1_dropoffs_distr)
         self.P2, self.R2 = open_to_close(self._lot2_requests_distr, self._lot2_dropoffs_distr)
 
-        # Episode terminates after 100 days (timesteps)
-        self._t = 0
-        self._time_limit = 100
-
         # Bypass the search for reachable states because we know the whole grid is valid
         states = [(i, j) for i in range(21) for j in range(21)]
         super().__init__(starts={(10, 10)}, n_actions=11, reachable_states=states)
 
-    def seed(self, seed=None):
-        seeds = super().seed(seed)
+    def reset(self, seed=None, options=None):
         # Make sure each distribution has access to the np_random module
         for distr in [self._lot1_requests_distr, self._lot1_dropoffs_distr,
                       self._lot2_requests_distr, self._lot2_dropoffs_distr]:
             distr.np_random = self.np_random
-        return seeds
-
-    def reset(self):
-        self._t = 0
-        return super().reset()
+        return super().reset(seed)
 
     def step(self, action):
-        self._t += 1
         assert self.action_space.contains(action)
-        state = self._state
+        state = self.state
         action = decode_action(action)
 
         next_state = move_cars(state, action)
 
         requests, dropoffs = self._sample_random_elements()
         for i in range(len(next_state)):
             next_state[i] = handle_requests_and_dropoffs(next_state[i], requests[i], dropoffs[i])
 
         next_state, reward, done, _ = self._deterministic_step(state, action, next_state)
-        self._state = next_state
-        return self._encode(next_state), reward, done, {}
+        self.state = next_state
+        return self.encode(next_state), reward, done, False, {}
 
     def _sample_random_elements(self):
         lot1_requests = self._lot1_requests_distr.sample()
         lot1_dropoffs = self._lot1_dropoffs_distr.sample()
         lot2_requests = self._lot2_requests_distr.sample()
         lot2_dropoffs = self._lot2_dropoffs_distr.sample()
         requests = [lot1_requests, lot2_requests]
@@ -103,20 +93,20 @@
         # Reward = (10 * expected requests - 2 * attempted moves)
         # Note that this implicitly discourages the agent from trying to move more cars
         # than are available, which makes the optimal action unambiguous
         n1, n2 = state_after_move
         return -2.0 * abs(action) + self.R1[n1] + self.R2[n2]
 
     def _done(self):
-        return self._t == self._time_limit
+        return False  # Environment has no terminal state
 
     def _generate_transitions(self, state, action):
         action = decode_action(action)
         for next_state in self.states():
-            next_state = self._decode(next_state)
+            next_state = self.decode(next_state)
             yield self._deterministic_step(state, action, next_state)
 
 
 class JacksCarRentalModified(JacksCarRental):
     """Same as `JacksCarRental` but with two modifications to the reward function. On
     each timestep:
```

### Comparing `gym-classics-0.0.2/gym_classics/envs/linear_walks.py` & `gym-classics-1.0.0/gym_classics/envs/linear_walks.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/racetracks.py` & `gym-classics-1.0.0/gym_classics/envs/racetracks.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/sparse_gridworld.py` & `gym-classics-1.0.0/gym_classics/envs/sparse_gridworld.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/envs/windy_gridworld.py` & `gym-classics-1.0.0/gym_classics/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `gym-classics-0.0.2/gym_classics/utils.py` & `gym-classics-1.0.0/gym_classics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     # First get the string length of the longest number
     def formatter(x):
         string = '{:' + ('+' if signed else '') + '.' + str(decimals) + 'f}'
         return string.format(x)
     maxlen = max([len(formatter(x)) for x in array])
 
     # Now we can actually print the values
-    for y in reversed(range(env._dims[1])):
-        for x in range(env._dims[0]):
+    for y in reversed(range(env.dims[1])):
+        for x in range(env.dims[0]):
             state = (x, y) if not transpose else (y, x)
-            if env._is_reachable(state):
-                s = env._encode(state)
+            if env.is_reachable(state):
+                s = env.encode(state)
                 print(formatter(array[s]).rjust(maxlen), end=separator)
             else:
                 print(' ' * maxlen, end=separator)
         print()
 
 
 def print_racetrack(env, V):
```

### Comparing `gym-classics-0.0.2/gym_classics.egg-info/PKG-INFO` & `gym-classics-1.0.0/gym_classics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gym-classics
-Version: 0.0.2
-Summary: Classic environments for reinforcement learning and dynamic programming, implemented in OpenAI Gym.
+Version: 1.0.0
+Summary: Classic environments for reinforcement learning and dynamic programming, implemented in OpenAI Gym and Gymnasium.
 Home-page: https://github.com/brett-daley/gym-classics
 Author: Brett Daley
 Author-email: brett.daley@ualberta.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gym Classics
-![pypi](https://img.shields.io/badge/pypi-0.0.2-blue)
+![pypi](https://img.shields.io/badge/pypi-1.0.0-blue)
 [![license](https://img.shields.io/badge/license-GPL%20v3.0-blue)](./LICENSE)
 ![python](https://img.shields.io/badge/python-3.5%2B-green)
 
 Gym Classics is a collection of well-known discrete MDPs from the reinforcement learning
 literature implemented as OpenAI Gym environments.
 API support for dynamic programming is also provided.
 
@@ -34,38 +34,23 @@
 
 1. [Example: Reinforcement Learning](#example-reinforcement-learning)
 
 1. [Example: Dynamic Programming](#example-dynamic-programming)
 
 1. [Environments Glossary](#environments-glossary)
 
-1. [References](#references)
-
-### Citing
-
-You can cite this repository in published work using the following bibtex:
-
-```
-@misc{daley2021gym,
-  author={Daley, Brett},
-  title={Gym Classics},
-  year={2021},
-  publisher={GitHub},
-  journal={GitHub repository},
-  howpublished={\url{https://github.com/brett-daley/gym-classics}},
-}
-```
+1. [Citing and References](#citing-and-references)
 
 ## Installation
 
 Prerequisites:
-- python 3.5+
-- gym
-- numpy
-- scipy (`JacksCarRental-v0` and `JacksCarRentalModified-v0` only)
+- Python 3.5+
+- `gym==0.26.2` or `gymnasium`
+- `numpy`
+- `scipy` (for `JacksCarRental` and `JacksCarRentalModified` only)
 
 ### Option 1: `pip`
 
 ```
 pip install gym-classics
 ```
 
@@ -77,45 +62,52 @@
 python setup.py install
 ```
 
 ---
 
 ## API Overview
 
-Once installed, the environments are automatically registered for `gym.make` by
-importing the `gym_classics` package in your Python script.
-The basic API is identical to that of OpenAI Gym.
+The basic API is identical to that of [OpenAI Gym](https://www.gymlibrary.dev/) (as of `0.26.2`) and [Gymnasium](https://gymnasium.farama.org/).
+The environments must be explictly registered for `gym.make` by
+importing the `gym_classics` package in your Python script and then calling `gym_classics.register('gym')` or `gym_classics.register('gymnasium')`, depending on which library you want to use as the backend.
+Note that registration cannot be changed after calling `register`, and mixing `gym` and `gymnasium` environments in a single script is not possible.
+
 A minimal working example:
 
 ```python
-import gym
+import gym                    # or `import gymnasium as gym`
 import gym_classics
+gym_classics.register('gym')  # or `gym_classics.register('gymnasium')`
 
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
+state, _ = env.reset(seed=0)
+
 for t in range(1, 100 + 1):
     action = env.action_space.sample()  # Select a random action
-    next_state, reward, done, info = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
     print("t={}, state={}, action={}, reward={}, next_state={}, done={}".format(
         t, state, action, reward, next_state, done))
-    state = next_state if not done else env.reset()
-env.close()
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
+
+env.close()  # Optional, not currently implemented by any environments
 ```
 
-Gym Classics also implements methods for querying a model of the environment.
+Gym Classics also implements methods for querying the model of the environment.
 The full interface of a Gym Classics environment therefore looks like this:
 
 ```yaml
 class Env:
     # Standard Gym API:
     - step(self, action)
-    - reset(self)
-    - render(self, mode='human')  # *currently not implemented by all environments*
+    - reset(self, seed=None, options=None)
+    - render(self)  # *currently not implemented by all environments*
     - close(self)
-    - seed(self, seed=None)
 
     # Extended Gym Classics API:
     - states(self)                # returns a generator over all feasible states
     - actions(self)               # returns a generator over all feasible actions
     - model(self, state, action)  # returns all transitions from the given state-action pair
 ```
 
@@ -123,76 +115,76 @@
 [Example: Dynamic Programming](#example-dynamic-programming).
 
 State and action spaces for all environments are type `gym.spaces.Discrete`.
 The size of these spaces can be queried as usual:
 `env.observation_space.n` and `env.action_space.n`.
 This means that states and actions are represented as unique integers, which is useful
 for advanced `numpy` indexing.
-Note that states and actions are enumerated in an arbitrary order for each environment.
+Note that states and actions are enumerated in an arbitrary but consistent order for each environment.
 
-> **Tip:** Gym Classics environments also implement private methods called `_encode` and `_decode` which convert states between their integral and human-interpretable forms.
+> **Tip:** Gym Classics environments also implement methods called `encode` and `decode` which convert states between their integer and human-interpretable forms.
 > These should never be used by the agent, but can be useful for displaying results or debugging.
 > See the abstract [BaseEnv](gym_classics/envs/abstract/base_env.py) class for implementation details.
 
 ## Example: Reinforcement Learning
 
 Let's test the classic Q-Learning algorithm [[4]](#references) on `ClassicGridworld-v0`.
 
 ```python
 import gym
 import gym_classics
+gym_classics.register('gym')
 import numpy as np
 
 # Hyperparameters for Q-Learning
 discount = 0.9
 epsilon = 0.5
 learning_rate = 0.025
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
+state, _ = env.reset(seed=0)
 
 # Our Q-function is a numpy array
 Q = np.zeros([env.observation_space.n, env.action_space.n])
 
 # Loop for 500k timesteps
 for _ in range(500000):
     # Select action from ε-greedy policy
-    if np.random.rand() < epsilon:
+    if env.np_random.random() < epsilon:
         action = env.action_space.sample()
     else:
         action = np.argmax(Q[state])
 
     # Step the environment
-    next_state, reward, done, _ = env.step(action)
+    next_state, reward, terminated, truncated, _ = env.step(action)
+    done = terminated or truncated
 
     # Q-Learning update:
     # Q(s,a) <-- Q(s,a) + α * (r + γ max_a' Q(s',a') - Q(s,a))
-    target = reward - Q[state, action]
+    td_error = reward - Q[state, action]
     if not done:
-        target += discount * np.max(Q[next_state])
-    Q[state, action] += learning_rate * target
+        td_error += discount * np.max(Q[next_state])
+    Q[state, action] += learning_rate * td_error
 
     # Reset the environment if we're done
-    state = env.reset() if done else next_state
+    if done:
+        next_state, _ = env.reset()
+    state = next_state
 
 # Now let's see what the value function looks like after training:
 V = np.max(Q, axis=1)
 print(V)
 ```
 
 Output:
 
 ```
-[ 0.5618515   0.75169693  1.          0.49147301  0.26363411 -1.
-  0.58655406  0.51379727  0.86959422  0.43567445  0.64966203]
+[ 0.56303004  0.72570493  0.56160538  0.48701053 -1.          0.44497334
+  0.2242687   0.63966295  0.84551377  0.42840196  1.        ]
 ```
 
 These values seem reasonable, but in the next section, we will certify their correctness
 by using dynamic programming.
 
 ## Example: Dynamic Programming
 
@@ -257,44 +249,47 @@
 Value Iteration and other dynamic programming methods are already implemented in
 [dynamic_programming.py](gym_classics/dynamic_programming.py).
 Let's use Value Iteration to check that our Q-Learning implemention from
 [Example: Reinforcement Learning](#example-reinforcement-learning) is correct:
 
 ```python
 import gym
+import gym_classics
+gym_classics.register('gym')
 from gym_classics.dynamic_programming import value_iteration
 import numpy as np
 
 # Instantiate the environment
 env = gym.make('ClassicGridworld-v0')
-state = env.reset()
-
-# Set seeds for reproducibility
-np.random.seed(0)
-env.seed(0)
 
 # Compute the near-optimal values with Value Iteration
 V_star = value_iteration(env, discount=0.9, precision=1e-9)
+print(V_star, end='\n\n')
 
 # Our Q-Learning values from earlier:
-V = [0.5618515,  0.75169693, 1.,         0.49147301, 0.26363411, -1.,
-     0.58655406, 0.51379727, 0.86959422, 0.43567445, 0.64966203]
+V = [0.56303004, 0.72570493, 0.56160538, 0.48701053, -1., 0.44497334,
+     0.2242687,  0.63966295, 0.84551377, 0.42840196, 1.]
 
 # Root Mean Square error:
-print("RMS error: {}".format(np.sqrt(np.square(V - V_star).mean())))
+rms_error = np.sqrt(np.mean(np.square(V - V_star)))
+print("RMS error:", rms_error)
 
 # Maximum absolute difference:
-print("Max abs diff: {}".format(np.abs(V - V_star).max()))
+max_abs_diff = np.max(np.abs(V - V_star))
+print("Maximum absolute difference:", max_abs_diff)
 ```
 
 Output:
 
 ```
-RMS error: 0.014976847878141084
-Max abs diff: 0.03832613967716292
+[ 0.56631445  0.74438015  0.57185903  0.49068396 -1.          0.47547113
+  0.27729584  0.64496924  0.84776628  0.43084446  1.        ]
+
+RMS error: 0.01967779454940685
+Maximum absolute difference: 0.053027139347779195
 ```
 
 Both error metrics are very close to zero;
 we can conclude that our Q-Learning implementation
 is working!
 
 ## Environments Glossary
@@ -316,15 +311,30 @@
 | 13 | `WindyGridworldKings-v0` | Same as `WindyGridworld` but with diagonal "King's" moves permitted.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 4 cardinal directions and 4 intermediate directions. |
 | 14 | `WindyGridworldKingsNoOp-v0` | Same as `WindyGridworldKings` but with an extra "no-op" (do nothing) action.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.9).<br><br>**actions:** Move in the 8 cardinal/intermediate directions or take a no-op action. |
 | 15 | `WindyGridworldKingsStochastic-v0` | Same as `WindyGridworldKings` but windy cells exhibit stochastic behavior: -1, +0, or +1 wind strength with probability 1/3 each.<br><br>**reference:** [[3]](#references) (page 131, exercise 6.10). |
 
 
 ---
 
-## References
+## Citing and References
+
+You can cite this repository in published work using the following bibtex:
+
+```
+@misc{daley2021gym,
+  author={Daley, Brett},
+  title={Gym Classics},
+  year={2021},
+  publisher={GitHub},
+  journal={GitHub repository},
+  howpublished={\url{https://github.com/brett-daley/gym-classics}},
+}
+```
+
+### References
 
 1. [Russell & Norvig. Artificial Intelligence: A Modern Approach. 2009, 3rd Ed.](https://cs.calvin.edu/courses/cs/344/kvlinden/resources/AIMA-3rd-edition.pdf)
 
 1. [Sutton, Precup, & Singh. Between MDPs and Semi-MDPs: A Framework for Temporal Abstraction in Reinforcement Learning. 1999.](https://people.cs.umass.edu/~barto/courses/cs687/Sutton-Precup-Singh-AIJ99.pdf)
 
 1. [Sutton & Barto. Reinforcement Learning: An Introduction. 2018, 2nd Ed.](http://incompleteideas.net/book/RLbook2020.pdf)
```

### Comparing `gym-classics-0.0.2/setup.py` & `gym-classics-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gym-classics",
-    version="0.0.2",
+    version="1.0.0",
     author="Brett Daley",
     author_email="brett.daley@ualberta.ca",
     description="Classic environments for reinforcement learning and dynamic"
-                " programming, implemented in OpenAI Gym.",
+                " programming, implemented in OpenAI Gym and Gymnasium.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/brett-daley/gym-classics",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

