# Comparing `tmp/geometrout-0.1.0.5.tar.gz` & `tmp/geometrout-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometrout-0.1.0.5.tar", last modified: Mon Apr 17 22:40:15 2023, max compression
+gzip compressed data, was "geometrout-0.1.0.6.tar", last modified: Tue May  2 00:54:59 2023, max compression
```

## Comparing `geometrout-0.1.0.5.tar` & `geometrout-0.1.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     2327 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/LICENSE
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       85 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/README.md
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/geometrout/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      100 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/__init__.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     1853 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/pointcloud.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)    22362 2023-04-14 20:57:49.000000 geometrout-0.1.0.5/geometrout/primitive.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)    10397 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/geometrout/transform.py
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/geometrout.egg-info/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      301 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      307 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/SOURCES.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)        1 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/dependency_links.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       20 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/requires.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       11 2023-04-17 22:40:15.000000 geometrout-0.1.0.5/geometrout.egg-info/top_level.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       90 2023-04-14 18:48:20.000000 geometrout-0.1.0.5/pyproject.toml
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      394 2023-04-17 22:40:15.594836 geometrout-0.1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.601587 geometrout-0.1.0.6/geometrout/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/geometrout/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/geometrout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 00:54:59.000000 geometrout-0.1.0.6/geometrout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 00:54:50.000000 geometrout-0.1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-02 00:54:59.605587 geometrout-0.1.0.6/setup.cfg
```

### Comparing `geometrout-0.1.0.5/LICENSE` & `geometrout-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.5/geometrout/pointcloud.py` & `geometrout-0.1.0.6/geometrout/pointcloud.py`

 * *Files identical despite different names*

### Comparing `geometrout-0.1.0.5/geometrout/primitive.py` & `geometrout-0.1.0.6/geometrout/primitive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,12 @@
-import numpy as np
 import numba as nb
+import numpy as np
 
 from geometrout.transform import SE3, _random_rotation
-import geometrout.pointcloud as pc
-
-
-@nb.jit(nopython=True, cache=True)
-def _rand_choice(arr, prob):
-    """
-    :param arr: A 1D numpy array of values to sample from.
-    :param prob: A 1D numpy array of probabilities for the given samples.
-    :return: A random sample from the given array with a given probability.
-    """
-    return arr[np.searchsorted(np.cumsum(prob), np.random.random(), side="right")]
-
-
-@nb.jit(nopython=True, cache=True)
-def _transform(point_cloud, transformation_matrix):
-    """
-
-    Parameters
-    ----------
-    :param point_cloud: A numpy pointcloud, maybe with some addition dimensions.
-        This should have shape N x [3 + M] where N is the number of points
-        are some additional mask dimensions or whatever, but the 3 are x-y-z
-    :param transformation_matrix: A 4x4 homography
-    :param in_place: A flag which says whether to do this in place
-    :return: A pointcloud that has been transformed,
-        either the same as the input or a new one.
-    """
-    assert point_cloud.shape[1] == 3
-    homogeneous_xyz = np.concatenate(
-        (np.transpose(point_cloud), np.ones((1, point_cloud.shape[0]))), axis=0
-    )
-    transformed_xyz = np.dot(transformation_matrix, homogeneous_xyz)
-    point_cloud[:, :3] = np.transpose(transformed_xyz[..., :3, :], (1, 0))
-    return point_cloud
+from geometrout.utils import transform_in_place
 
 
 @nb.jit(nopython=True, cache=True)
 def _cuboid_sample_surface(
     pose_matrix,
     dims,
     num_points,
@@ -66,24 +33,24 @@
     )
     random_points[sides == 0, 0] = dims[0] / 2
     random_points[sides == 1, 0] = -dims[0] / 2
     random_points[sides == 2, 1] = dims[1] / 2
     random_points[sides == 3, 1] = -dims[1] / 2
     random_points[sides == 4, 2] = dims[2] / 2
     random_points[sides == 5, 2] = -dims[2] / 2
-    _transform(random_points, pose_matrix)
+    transform_in_place(random_points, pose_matrix)
     noise = 2 * noise * np.random.random_sample(random_points.shape) - noise
     return random_points + noise
 
 
 @nb.jit(nopython=True, cache=True)
 def _cuboid_sample_volume(pose_matrix, dims, num_points):
     random_points = np.random.uniform(-1.0, 1.0, (num_points, 3))
     random_points = random_points * dims / 2
-    _transform(random_points, pose_matrix)
+    transform_in_place(random_points, pose_matrix)
     return random_points
 
 
 @nb.njit
 def np_apply_along_axis(func1d, axis, arr):
     assert arr.ndim == 2
     assert axis in [0, 1]
@@ -153,15 +120,15 @@
             [x_front, y_front, z_back],
             [x_back, y_back, z_front],
             [x_back, y_front, z_back],
             [x_front, y_back, z_back],
             [x_back, y_back, z_back],
         ]
     )
-    _transform(corners, pose_matrix)
+    transform_in_place(corners, pose_matrix)
     return corners
 
 
 @nb.jit(nopython=True, cache=True)
 def _cuboid_surface_area(dims):
     return 2 * (dims[0] * dims[1] + dims[0] * dims[2] + dims[1] * dims[2])
 
@@ -518,15 +485,15 @@
     z[which_surface == 1] = np.random.uniform(
         -height / 2,
         height / 2,
         size=(np.count_nonzero(which_surface == 1), 1),
     )
     z[which_surface == 2] = height / 2
     surface_points = np.concatenate((circle_points, z), axis=1)
-    _transform(surface_points, pose_matrix)
+    transform_in_place(surface_points, pose_matrix)
     noise = 2 * noise * np.random.random_sample(surface_points.shape) - noise
     return surface_points + noise
 
 
 @nb.jit(nopython=True, cache=True)
 def _cylinder_sample_volume(pose_matrix, radius, height, num_points, noise):
     assert (
@@ -539,15 +506,15 @@
     volume_points = np.concatenate(
         (
             disc_points,
             np.random.uniform(-height / 2, height / 2, size=(num_points, 1)),
         ),
         axis=1,
     )
-    _transform(volume_points, pose_matrix)
+    transform_in_place(volume_points, pose_matrix)
     noise = 2 * noise * np.random.random_sample(volume_points.shape) - noise
     return volume_points + noise
 
 
 class Cylinder:
     pose: SE3
```

### Comparing `geometrout-0.1.0.5/geometrout/transform.py` & `geometrout-0.1.0.6/geometrout/transform.py`

 * *Files identical despite different names*

