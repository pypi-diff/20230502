# Comparing `tmp/cxr-foundation-0.0.8.tar.gz` & `tmp/cxr-foundation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cxr-foundation-0.0.8.tar", last modified: Thu Oct 27 16:52:48 2022, max compression
+gzip compressed data, was "dist/cxr-foundation-0.0.9.tar", last modified: Thu Oct 27 17:09:14 2022, max compression
```

## Comparing `cxr-foundation-0.0.8.tar` & `cxr-foundation-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/
--rw-r--r--   0 asellerg (110095) primarygroup (89939)      231 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/PKG-INFO
--rw-r--r--   0 asellerg (110095) primarygroup (89939)     6259 2022-08-30 23:59:55.000000 cxr-foundation-0.0.8/README.md
-drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation/
--rw-r--r--   0 asellerg (110095) primarygroup (89939)        0 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/__init__.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)      827 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/constants.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     6879 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/example_generator_lib.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     1281 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/example_generator_lib_test.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     7270 2022-09-26 22:47:41.000000 cxr-foundation-0.0.8/cxr_foundation/inference_beam_lib.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     7949 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/inference_beam_lib_test.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     3963 2022-10-27 16:50:54.000000 cxr-foundation-0.0.8/cxr_foundation/run_inference.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     3368 2022-10-24 18:14:46.000000 cxr-foundation-0.0.8/cxr_foundation/train.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     6319 2022-09-26 23:54:44.000000 cxr-foundation-0.0.8/cxr_foundation/train_lib.py
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     2612 2022-07-18 22:32:59.000000 cxr-foundation-0.0.8/cxr_foundation/train_lib_test.py
-drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/
--rw-r--r--   0 asellerg (110095) primarygroup (89939)      231 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/PKG-INFO
--rw-r--r--   0 asellerg (110095) primarygroup (89939)      543 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/SOURCES.txt
--rw-r--r--   0 asellerg (110095) primarygroup (89939)        1 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/dependency_links.txt
--rw-r--r--   0 asellerg (110095) primarygroup (89939)      199 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/requires.txt
--rw-r--r--   0 asellerg (110095) primarygroup (89939)       15 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/cxr_foundation.egg-info/top_level.txt
--rw-r--r--   0 asellerg (110095) primarygroup (89939)       38 2022-10-27 16:52:48.000000 cxr-foundation-0.0.8/setup.cfg
--rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     1102 2022-10-27 16:52:02.000000 cxr-foundation-0.0.8/setup.py
+drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)      231 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/PKG-INFO
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)     6259 2022-08-30 23:59:55.000000 cxr-foundation-0.0.9/README.md
+drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation/
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)        0 2022-07-18 22:32:59.000000 cxr-foundation-0.0.9/cxr_foundation/__init__.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)      827 2022-07-18 22:32:59.000000 cxr-foundation-0.0.9/cxr_foundation/constants.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     6890 2022-10-27 17:08:05.000000 cxr-foundation-0.0.9/cxr_foundation/example_generator_lib.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     1281 2022-07-18 22:32:59.000000 cxr-foundation-0.0.9/cxr_foundation/example_generator_lib_test.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     7292 2022-10-27 17:07:49.000000 cxr-foundation-0.0.9/cxr_foundation/inference_beam_lib.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     7949 2022-07-18 22:32:59.000000 cxr-foundation-0.0.9/cxr_foundation/inference_beam_lib_test.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     3963 2022-10-27 16:50:54.000000 cxr-foundation-0.0.9/cxr_foundation/run_inference.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     3368 2022-10-24 18:14:46.000000 cxr-foundation-0.0.9/cxr_foundation/train.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     6319 2022-09-26 23:54:44.000000 cxr-foundation-0.0.9/cxr_foundation/train_lib.py
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     2612 2022-07-18 22:32:59.000000 cxr-foundation-0.0.9/cxr_foundation/train_lib_test.py
+drwxr-xr-x   0 asellerg (110095) primarygroup (89939)        0 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)      231 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/PKG-INFO
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)      543 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/SOURCES.txt
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)        1 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/dependency_links.txt
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)      199 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/requires.txt
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)       15 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/cxr_foundation.egg-info/top_level.txt
+-rw-r--r--   0 asellerg (110095) primarygroup (89939)       38 2022-10-27 17:09:14.000000 cxr-foundation-0.0.9/setup.cfg
+-rwxr-xr-x   0 asellerg (110095) primarygroup (89939)     1102 2022-10-27 17:08:29.000000 cxr-foundation-0.0.9/setup.py
```

### Comparing `cxr-foundation-0.0.8/README.md` & `cxr-foundation-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/constants.py` & `cxr-foundation-0.0.9/cxr_foundation/constants.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/example_generator_lib.py` & `cxr-foundation-0.0.9/cxr_foundation/example_generator_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Methods to create tf.examples for model inference via pydicom."""
 
-from lib import constants
+from cxr_foundation import constants
 
 import io
 from typing import Iterable, Union
 
 import numpy as np
 import png
 import pydicom
```

### Comparing `cxr-foundation-0.0.8/cxr_foundation/example_generator_lib_test.py` & `cxr-foundation-0.0.9/cxr_foundation/example_generator_lib_test.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/inference_beam_lib.py` & `cxr-foundation-0.0.9/cxr_foundation/inference_beam_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Collection of Beam DoFns to generate embeddings."""
-from lib import constants
-from lib import example_generator_lib
+from cxr_foundation import constants
+from cxr_foundation import example_generator_lib
 
 import base64
 import contextlib
 from enum import Enum
 import io
 from apache_beam.utils import retry
```

### Comparing `cxr-foundation-0.0.8/cxr_foundation/inference_beam_lib_test.py` & `cxr-foundation-0.0.9/cxr_foundation/inference_beam_lib_test.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/run_inference.py` & `cxr-foundation-0.0.9/cxr_foundation/run_inference.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/train.py` & `cxr-foundation-0.0.9/cxr_foundation/train.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/train_lib.py` & `cxr-foundation-0.0.9/cxr_foundation/train_lib.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation/train_lib_test.py` & `cxr-foundation-0.0.9/cxr_foundation/train_lib_test.py`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/cxr_foundation.egg-info/SOURCES.txt` & `cxr-foundation-0.0.9/cxr_foundation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxr-foundation-0.0.8/setup.py` & `cxr-foundation-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import setuptools
 
 setuptools.setup(
   name='cxr-foundation',
-  version='0.0.8',
+  version='0.0.9',
   description='CXR Foundation: chest x-ray embeddings generation.',
   install_requires=[
     'google-api-python-client',
     'google-apitools',
     'google-cloud-aiplatform',
     'google-cloud-storage',
     'apache_beam',
```

