# Comparing `tmp/pyqrack-1.7.1.tar.gz` & `tmp/pyqrack-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqrack-1.7.1.tar", last modified: Mon May  1 10:35:04 2023, max compression
+gzip compressed data, was "pyqrack-1.8.0.tar", last modified: Mon May  1 22:35:47 2023, max compression
```

## Comparing `pyqrack-1.7.1.tar` & `pyqrack-1.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 10:35:03.995607 pyqrack-1.7.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.7.1/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 10:35:03.995607 pyqrack-1.7.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-01 10:33:18.000000 pyqrack-1.7.1/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.7.1/pyproject.toml
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 10:35:03.995607 pyqrack-1.7.1/pyqrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      439 2023-04-30 17:06:05.000000 pyqrack-1.7.1/pyqrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.7.1/pyqrack/pauli.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     7413 2023-04-30 17:06:05.000000 pyqrack-1.7.1/pyqrack/qrack_neuron.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-30 17:06:05.000000 pyqrack-1.7.1/pyqrack/qrack_simulator.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 10:35:03.995607 pyqrack-1.7.1/pyqrack/qrack_system/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.7.1/pyqrack/qrack_system/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    27066 2023-05-01 10:33:34.000000 pyqrack-1.7.1/pyqrack/qrack_system/qrack_system.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 10:35:03.995607 pyqrack-1.7.1/pyqrack/util/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.7.1/pyqrack/util/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.7.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 10:35:03.995607 pyqrack-1.7.1/pyqrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 10:35:03.000000 pyqrack-1.7.1/pyqrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      436 2023-05-01 10:35:03.000000 pyqrack-1.7.1/pyqrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 10:35:03.000000 pyqrack-1.7.1/pyqrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 10:35:03.000000 pyqrack-1.7.1/pyqrack.egg-info/not-zip-safe
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-01 10:35:03.000000 pyqrack-1.7.1/pyqrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-01 10:35:03.995607 pyqrack-1.7.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-01 10:33:48.000000 pyqrack-1.7.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:35:47.061296 pyqrack-1.8.0/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.8.0/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 22:35:47.061296 pyqrack-1.8.0/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-05-01 22:33:37.000000 pyqrack-1.8.0/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.8.0/pyproject.toml
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:35:47.061296 pyqrack-1.8.0/pyqrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      492 2023-05-01 22:27:13.000000 pyqrack-1.8.0/pyqrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      597 2023-05-01 22:27:13.000000 pyqrack-1.8.0/pyqrack/neuron_activation_fn.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.8.0/pyqrack/pauli.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     8677 2023-05-01 22:27:13.000000 pyqrack-1.8.0/pyqrack/qrack_neuron.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-30 17:06:05.000000 pyqrack-1.8.0/pyqrack/qrack_simulator.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:35:47.061296 pyqrack-1.8.0/pyqrack/qrack_system/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.8.0/pyqrack/qrack_system/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    27647 2023-05-01 22:33:37.000000 pyqrack-1.8.0/pyqrack/qrack_system/qrack_system.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:35:47.061296 pyqrack-1.8.0/pyqrack/util/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.8.0/pyqrack/util/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.8.0/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-01 22:35:47.061296 pyqrack-1.8.0/pyqrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-05-01 22:35:47.000000 pyqrack-1.8.0/pyqrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      468 2023-05-01 22:35:47.000000 pyqrack-1.8.0/pyqrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 22:35:47.000000 pyqrack-1.8.0/pyqrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-01 22:35:46.000000 pyqrack-1.8.0/pyqrack.egg-info/not-zip-safe
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-05-01 22:35:47.000000 pyqrack-1.8.0/pyqrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-01 22:35:47.061296 pyqrack-1.8.0/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-05-01 22:27:13.000000 pyqrack-1.8.0/setup.py
```

### Comparing `pyqrack-1.7.1/LICENSE` & `pyqrack-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrack-1.7.1/PKG-INFO` & `pyqrack-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.7.1
+Version: 1.8.0
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.7.1/README.md` & `pyqrack-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqrack-1.7.1/pyqrack/pauli.py` & `pyqrack-1.8.0/pyqrack/pauli.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.7.1/pyqrack/qrack_neuron.py` & `pyqrack-1.8.0/pyqrack/qrack_neuron.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Use of this source code is governed by an MIT-style license that can be
 # found in the LICENSE file or at https://opensource.org/licenses/MIT.
 
 import ctypes
 import sys
 
 from .qrack_system import Qrack
+from .neuron_activation_fn import NeuronActivationFn
 
 class QrackNeuron:
     """Class that exposes the QNeuron class of Qrack
 
     This model of a "quantum neuron" is based on the concept of a "uniformly controlled"
     rotation of a single output qubit around the Pauli Y axis, and has been developed by
     others. In our case, the primary relevant gate could also be called a
@@ -40,28 +41,32 @@
             raise RuntimeError("QrackNeuron C++ library raised exception.")
 
     def __init__(
         self,
         simulator,
         controls,
         target,
+        activation_fn = NeuronActivationFn.Sigmoid,
+        alpha = 1.0,
         tolerance = sys.float_info.epsilon,
         _init = True
     ):
         self.simulator = simulator
         self.controls = controls
         self.target = target
+        self.activation_fn = activation_fn
+        self.alpha = alpha
         self.tolerance = tolerance
 
         self.amp_count = 1 << (len(controls) + 1)
 
         if not _init:
             return
 
-        self.nid = Qrack.qrack_lib.init_qneuron(simulator.sid, len(controls), self._ulonglong_byref(controls), target, tolerance)
+        self.nid = Qrack.qrack_lib.init_qneuron(simulator.sid, len(controls), self._ulonglong_byref(controls), target, activation_fn, alpha, tolerance)
 
         self._throw_if_error()
 
     def __del__(self):
         if self.nid is not None:
             Qrack.qrack_lib.destroy_qneuron(self.nid)
             self.nid = None
@@ -71,58 +76,87 @@
 
         Create a new, independent neuron instance with identical angles,
         inputs, output, and tolerance, for the same QrackSimulator.
 
         Raises:
             RuntimeError: QrackNeuron C++ library raised an exception.
         """
-        result = QrackNeuron(self.simulator, self.controls, self.target, self.tolerance)
+        result = QrackNeuron(self.simulator, self.controls, self.target, self.activation_fn, self.alpha, self.tolerance)
         self.nid = Qrack.qrack_lib.clone_qneuron(self.simulator.sid)
         self._throw_if_error()
         return result
 
     def _ulonglong_byref(self, a):
         return (ctypes.c_ulonglong * len(a))(*a)
 
     def _real1_byref(self, a):
         # This needs to be c_double, if PyQrack is built with fp64.
         if Qrack.fppow < 6:
             return (ctypes.c_float * len(a))(*a)
         return (ctypes.c_double * len(a))(*a)
 
-    def set_qneuron_angles(self, a):
+    def set_angles(self, a):
         """Directly sets the neuron parameters.
 
         Set all synaptic parameters of the neuron directly, by a list
         enumerated over the integer permutations of input qubits.
 
         Args:
             a(list(double)): List of input permutation angles
 
         Raises:
             RuntimeError: QrackNeuron C++ library raised an exception.
         """
         Qrack.qrack_lib.set_qneuron_angles(self.nid, self._real1_byref(a))
         self._throw_if_error()
 
-    def get_qneuron_angles(self):
+    def get_angles(self):
         """Directly gets the neuron parameters.
 
         Get all synaptic parameters of the neuron directly, as a list
         enumerated over the integer permutations of input qubits.
 
         Raises:
             RuntimeError: QrackNeuron C++ library raised an exception.
         """
         ket = self._real1_byref([0.0] * self.amp_count)
         Qrack.qrack_lib.get_qneuron_angles(self.nid, ket)
         if self._get_error() != 0:
             raise RuntimeError("QrackSimulator C++ library raised exception.")
         return list(ket)
 
+    def set_alpha(self, a):
+        """Set the neuron 'alpha' parameter.
+
+        To enable nonlinear activation, `QrackNeuron` has an 'alpha'
+        parameter that is applied as a power to its angles, before
+        learning and prediction. This makes the activation function
+        sharper (or less sharp).
+
+        Raises:
+            RuntimeError: QrackNeuron C++ library raised an exception.
+        """
+        self.alpha = a
+        Qrack.qrack_lib.set_qneuron_alpha(self.nid, a)
+        self._throw_if_error()
+
+    def set_activation_fn(self, f):
+        """Sets the activation function of this QrackNeuron
+
+        Nonlinear activation functions can be important to neural net
+        applications, like DNN. The available activation functions are
+        enumerated in `NeuronActivationFn`. 
+
+        Raises:
+            RuntimeError: QrackNeuron C++ library raised an exception.
+        """
+        self.activation_fn = f
+        Qrack.qrack_lib.set_qneuron_activation_fn(self.nid, f)
+        self._throw_if_error()
+
     def predict(self, e=True, r=True):
         """Predict based on training
 
         "Predict" the anticipated output, based on input and training.
         By default, "predict()" will initialize the output qubit as by
         resetting to |0> and then acting a Hadamard gate. From that
         state, the method amends the output qubit upon the basis of
```

### Comparing `pyqrack-1.7.1/pyqrack/qrack_simulator.py` & `pyqrack-1.8.0/pyqrack/qrack_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.7.1/pyqrack/qrack_system/qrack_system.py` & `pyqrack-1.8.0/pyqrack/qrack_system/qrack_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -854,15 +854,15 @@
         self.qrack_lib.SetReactiveSeparate.restype = c_bool
         self.qrack_lib.SetReactiveSeparate.argtypes = [c_ulonglong, c_bool]
 
         self.qrack_lib.SetTInjection.restype = c_bool
         self.qrack_lib.SetTInjection.argtypes = [c_ulonglong, c_bool]
 
         self.qrack_lib.init_qneuron.restype = c_ulonglong
-        self.qrack_lib.init_qneuron.argtypes = [c_ulonglong, c_ulonglong, POINTER(c_ulonglong), c_ulonglong, c_double]
+        self.qrack_lib.init_qneuron.argtypes = [c_ulonglong, c_ulonglong, POINTER(c_ulonglong), c_ulonglong, c_ulonglong, c_double, c_double]
 
         self.qrack_lib.clone_qneuron.restype = c_ulonglong
         self.qrack_lib.clone_qneuron.argtypes = [c_ulonglong]
 
         self.qrack_lib.destroy_qneuron.restype = None
         self.qrack_lib.destroy_qneuron.argtypes = [c_ulonglong]
 
@@ -872,14 +872,26 @@
         if self.fppow == 5:
             self.qrack_lib.set_qneuron_angles.argtypes = [c_ulonglong, POINTER(c_float)]
             self.qrack_lib.get_qneuron_angles.argtypes = [c_ulonglong, POINTER(c_float)]
         if self.fppow == 6:
             self.qrack_lib.set_qneuron_angles.argtypes = [c_ulonglong, POINTER(c_double)]
             self.qrack_lib.get_qneuron_angles.argtypes = [c_ulonglong, POINTER(c_double)]
 
+        self.qrack_lib.set_qneuron_alpha.restype = None
+        self.qrack_lib.set_qneuron_alpha.argtypes = [c_ulonglong, c_double]
+
+        self.qrack_lib.get_qneuron_alpha.restype = c_double
+        self.qrack_lib.get_qneuron_alpha.argtypes = [c_ulonglong]
+
+        self.qrack_lib.set_qneuron_activation_fn.restype = None
+        self.qrack_lib.set_qneuron_activation_fn.argtypes = [c_ulonglong, c_ulonglong]
+
+        self.qrack_lib.get_qneuron_activation_fn.restype = c_ulonglong
+        self.qrack_lib.get_qneuron_activation_fn.argtypes = [c_ulonglong]
+
         self.qrack_lib.qneuron_predict.restype = c_double
         self.qrack_lib.qneuron_predict.argtypes = [c_ulonglong, c_bool, c_bool]
 
         self.qrack_lib.qneuron_unpredict.restype = c_double
         self.qrack_lib.qneuron_unpredict.argtypes = [c_ulonglong, c_bool]
 
         self.qrack_lib.qneuron_learn_cycle.restype = c_double
```

### Comparing `pyqrack-1.7.1/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py` & `pyqrack-1.8.0/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.7.1/pyqrack.egg-info/PKG-INFO` & `pyqrack-1.8.0/pyqrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.7.1
+Version: 1.8.0
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.7.1/setup.py` & `pyqrack-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 
 requirements = []
 
-VERSION = "1.7.1"
+VERSION = "1.8.0"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 setup(
```

