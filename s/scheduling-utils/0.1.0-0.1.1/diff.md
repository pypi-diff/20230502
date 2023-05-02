# Comparing `tmp/scheduling_utils-0.1.0.tar.gz` & `tmp/scheduling_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dserez/Documents/Work/Github/scheduling_utils/dist/.tmp-26h2rjcm/scheduling_utils-0.1.0.tar", last modified: Fri Feb  3 09:24:34 2023, max compression
+gzip compressed data, was "scheduling_utils-0.1.1.tar", last modified: Tue May  2 07:08:48 2023, max compression
```

## Comparing `scheduling_utils-0.1.0.tar` & `scheduling_utils-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1063 2023-01-24 12:20:04.000000 scheduling_utils-0.1.0/LICENSE
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-02-03 09:13:57.000000 scheduling_utils-0.1.0/MANIFEST.in
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      998 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/images/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    15837 2023-02-03 08:45:24.000000 scheduling_utils-0.1.0/images/cosine_decay.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    15046 2023-02-03 08:47:14.000000 scheduling_utils-0.1.0/images/cosine_ramp.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    16089 2023-02-03 08:45:56.000000 scheduling_utils-0.1.0/images/linear_decay.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    14761 2023-02-03 08:47:45.000000 scheduling_utils-0.1.0/images/linear_ramp.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      739 2023-02-03 09:21:07.000000 scheduling_utils-0.1.0/readme.md
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-09 07:27:26.000000 scheduling_utils-0.1.0/scheduling_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2054 2023-02-03 08:41:23.000000 scheduling_utils-0.1.0/scheduling_utils/schedulers.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      997 2023-02-03 08:44:50.000000 scheduling_utils-0.1.0/scheduling_utils/test.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      998 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      416 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       17 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/scheduling_utils.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-02-03 09:24:34.000000 scheduling_utils-0.1.0/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      574 2023-02-03 09:23:03.000000 scheduling_utils-0.1.0/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1063 2023-01-24 12:20:04.000000 scheduling_utils-0.1.1/LICENSE
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-02-03 09:13:57.000000 scheduling_utils-0.1.1/MANIFEST.in
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      801 2023-05-02 07:05:00.000000 scheduling_utils-0.1.1/README.md
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/images/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    15837 2023-02-03 08:45:24.000000 scheduling_utils-0.1.1/images/cosine_decay.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    15046 2023-02-03 08:47:14.000000 scheduling_utils-0.1.1/images/cosine_ramp.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    22196 2023-05-02 06:58:05.000000 scheduling_utils-0.1.1/images/linear_cosine.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    16089 2023-02-03 08:45:56.000000 scheduling_utils-0.1.1/images/linear_decay.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    14761 2023-02-03 08:47:45.000000 scheduling_utils-0.1.1/images/linear_ramp.png
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/scheduling_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-09 07:27:26.000000 scheduling_utils-0.1.1/scheduling_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     3190 2023-05-02 06:56:13.000000 scheduling_utils-0.1.1/scheduling_utils/schedulers.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1922 2023-05-02 07:05:10.000000 scheduling_utils-0.1.1/scheduling_utils/test.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/scheduling_utils.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      441 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-02-03 09:24:34.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       17 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      574 2023-05-02 07:08:46.000000 scheduling_utils-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scheduling_utils-0.1.0/LICENSE` & `scheduling_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.0/PKG-INFO` & `scheduling_utils-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scheduling_utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: implementation of scheduling function utils
 Home-page: https://github.com/SerezD/scheduling_utils
 Author: DSerez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,8 +35,10 @@
 Available Schedulers at current version:
 - Linear
     ![linear-ramp](images/linear_ramp.png)
     ![linear-decay](images/linear_decay.png)
 - Cosine
     ![cosine-ramp](images/cosine_ramp.png)
     ![cosine-decay](images/cosine_decay.png)
+- LinearCosine
+    ![linear-cosine](images/linear_cosine.png)
```

### Comparing `scheduling_utils-0.1.0/images/cosine_decay.png` & `scheduling_utils-0.1.1/images/cosine_decay.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.0/images/cosine_ramp.png` & `scheduling_utils-0.1.1/images/cosine_ramp.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.0/images/linear_decay.png` & `scheduling_utils-0.1.1/images/linear_decay.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.0/images/linear_ramp.png` & `scheduling_utils-0.1.1/images/linear_ramp.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.0/readme.md` & `scheduling_utils-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 Available Schedulers at current version:
 - Linear
     ![linear-ramp](images/linear_ramp.png)
     ![linear-decay](images/linear_decay.png)
 - Cosine
     ![cosine-ramp](images/cosine_ramp.png)
     ![cosine-decay](images/cosine_decay.png)
+- LinearCosine
+    ![linear-cosine](images/linear_cosine.png)
```

### Comparing `scheduling_utils-0.1.0/scheduling_utils/schedulers.py` & `scheduling_utils-0.1.1/scheduling_utils/schedulers.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,7 +65,35 @@
 
     def warp_func(self, perc_step: float):
 
         # Identity warp
         return perc_step
 
 
+class LinearCosineScheduler:
+    def __init__(self, start_step: int, stop_step: int, start_value: float, stop_value: float, th_step: int):
+        """
+        Linear Warmup Followed by Cosine Decay.
+        Learning rate increases from start_step tp th_step (0.0 to start_value) and then decays to stop_value
+        """
+
+        if start_value <= stop_value:
+            raise AttributeError('the LinearCosine Scheduler must decay.')
+
+        if start_step >= stop_step:
+            raise AttributeError('In the scheduler, start step must be minor that stop step!')
+
+        if not start_step < th_step and th_step < stop_step:
+            raise AttributeError('In the scheduler, threshold step must lay between start and stop steps!')
+
+        super().__init__()
+
+        self.th_step = th_step
+        self.linear_wu = LinearScheduler(start_step, th_step, 0, start_value)
+        self.cosine_decay = CosineScheduler(th_step, stop_step, start_value, stop_value)
+
+    def step(self, step: int):
+
+        if step < self.th_step:
+            return self.linear_wu.step(step)
+        else:
+            return self.cosine_decay.step(step)
```

### Comparing `scheduling_utils-0.1.0/scheduling_utils/test.py` & `scheduling_utils-0.1.1/scheduling_utils/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from matplotlib import pyplot as plt
 import random
 
-from schedulers import CosineScheduler, LinearScheduler
+from schedulers import CosineScheduler, LinearScheduler, LinearCosineScheduler
 
 
 def plot_schedulers():
 
     for name, scheduler in zip(['cosine', 'linear'], [CosineScheduler, LinearScheduler]):
 
         # may raise Error if stop step < start step (intended)
@@ -27,10 +27,40 @@
             plt.show()
 
         except AttributeError as e:
             print(f'start_step: {start_step} - stop_step: {stop_step}')
             print(e)
 
 
+def plot_linear_cosine():
+
+    # may raise Error if threshold is not between start and stop (intended)
+    start_step = random.randint(0, 20)
+    th_step = random.randint(15, 25)
+    stop_step = random.randint(20, 40)
+
+    # always decay
+    start_value = random.randint(30, 50)
+    stop_value = random.randint(0, 20)
+
+    try:
+        s = LinearCosineScheduler(start_step, stop_step, start_value, stop_value, th_step)
+
+        values = []
+        for i in range(stop_step + 5):
+            values.append(s.step(i))
+
+        plt.suptitle(f'LinearCosine: Linear from ({start_step}, 0) to ({th_step}, {start_value})\n'
+                     f'Cosine from ({th_step}, {start_value}) to ({stop_step}, {stop_value})')
+        plt.plot(values)
+        plt.show()
+
+    except AttributeError as e:
+        print(f'start_step: {start_step} - stop_step: {stop_step}')
+        print(e)
+
+
 if __name__ == '__main__':
 
     plot_schedulers()
+
+    plot_linear_cosine()
```

### Comparing `scheduling_utils-0.1.0/scheduling_utils.egg-info/PKG-INFO` & `scheduling_utils-0.1.1/scheduling_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scheduling-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: implementation of scheduling function utils
 Home-page: https://github.com/SerezD/scheduling_utils
 Author: DSerez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -35,8 +35,10 @@
 Available Schedulers at current version:
 - Linear
     ![linear-ramp](images/linear_ramp.png)
     ![linear-decay](images/linear_decay.png)
 - Cosine
     ![cosine-ramp](images/cosine_ramp.png)
     ![cosine-decay](images/cosine_decay.png)
+- LinearCosine
+    ![linear-cosine](images/linear_cosine.png)
```

### Comparing `scheduling_utils-0.1.0/setup.py` & `scheduling_utils-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "readme.md").read_text()
+long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='scheduling_utils',
-      version='0.1.0',
+      version='0.1.1',
       description='implementation of scheduling function utils',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/SerezD/scheduling_utils',
       author='DSerez',
       license='MIT',
       packages=find_packages(),
```

