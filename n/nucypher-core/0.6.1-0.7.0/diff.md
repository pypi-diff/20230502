# Comparing `tmp/nucypher_core-0.6.1.tar.gz` & `tmp/nucypher_core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucypher_core-0.6.1.tar", last modified: Sun Feb 19 00:52:42 2023, max compression
+gzip compressed data, was "nucypher_core-0.7.0.tar", last modified: Tue May  2 04:30:01 2023, max compression
```

## Comparing `nucypher_core-0.6.1.tar` & `nucypher_core-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/nucypher_core/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/nucypher_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/nucypher_core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/nucypher_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/nucypher_core/umbral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/nucypher_core/umbral.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/nucypher_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/nucypher_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/nucypher_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/nucypher_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/nucypher_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-19 00:52:42.000000 nucypher_core-0.6.1/nucypher_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:52:42.406201 nucypher_core-0.6.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    29260 2023-02-19 00:52:39.000000 nucypher_core-0.6.1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.974393 nucypher_core-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/nucypher_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/umbral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/umbral.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/nucypher_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:30:01.974393 nucypher_core-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32681 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/src/lib.rs
```

### Comparing `nucypher_core-0.6.1/LICENSE` & `nucypher_core-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.6.1/PKG-INFO` & `nucypher_core-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nucypher_core
-Version: 0.6.1
+Version: 0.7.0
 Summary: Protocol structures of Nucypher network
-Home-page: https://github.com/nucypher/nucypher-core/tree/master/nucypher-core-python
+Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
@@ -33,8 +33,8 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/nucypher-core
 [pypi-link]: https://pypi.org/project/nucypher-core/
 [pypi-license-image]: https://img.shields.io/pypi/l/nucypher-core
 [rtd-image]: https://readthedocs.org/projects/nucypher-core/badge/?version=latest
 [rtd-link]: https://nucypher-core.readthedocs.io/en/latest/
-[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/master/nucypher-core
+[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core
```

### Comparing `nucypher_core-0.6.1/README.md` & `nucypher_core-0.7.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/nucypher-core
 [pypi-link]: https://pypi.org/project/nucypher-core/
 [pypi-license-image]: https://img.shields.io/pypi/l/nucypher-core
 [rtd-image]: https://readthedocs.org/projects/nucypher-core/badge/?version=latest
 [rtd-link]: https://nucypher-core.readthedocs.io/en/latest/
-[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/master/nucypher-core
+[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core
```

### Comparing `nucypher_core-0.6.1/nucypher_core/__init__.pyi` & `nucypher_core-0.7.0/nucypher_core/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from typing import List, Dict, Sequence, Optional, Mapping, Tuple, Set
 
 from .umbral import (
-    SecretKey, PublicKey, Signer, Capsule, VerifiedKeyFrag, VerifiedCapsuleFrag,
-    RecoverableSignature)
+    SecretKey,
+    PublicKey,
+    Signer,
+    Capsule,
+    VerifiedKeyFrag,
+    VerifiedCapsuleFrag,
+    RecoverableSignature
+)
 
 
 class Address:
 
     def __init__(self, address_bytes: bytes):
         ...
 
@@ -290,27 +296,30 @@
     def __init__(
         self,
         staking_provider_address: Address,
         domain: str,
         timestamp_epoch: int,
         verifying_key: PublicKey,
         encrypting_key: PublicKey,
+        ferveo_public_key: bytes,
         certificate_der: bytes,
         host: str,
         port: int,
         operator_signature: RecoverableSignature,
     ):
         ...
 
     staking_provider_address: Address
 
     verifying_key: PublicKey
 
     encrypting_key: PublicKey
 
+    ferveo_public_key: bytes
+
     operator_signature: RecoverableSignature
 
     domain: str
 
     host: str
 
     port: int
@@ -388,7 +397,51 @@
 
     @staticmethod
     def from_bytes(data: bytes) -> MetadataResponse:
         ...
 
     def __bytes__(self) -> bytes:
         ...
+
+
+class ThresholdDecryptionRequest:
+
+    def __init__(self, ritual_id: int, variant: int, ciphertext: bytes, conditions: Optional[Conditions], context: Optional[Context]):
+        ...
+
+    def id(self) -> int:
+        ...
+
+    def conditions(self) -> Optional[Conditions]:
+        ...
+
+    def context(self) -> Optional[Context]:
+        ...
+
+    def variant(self) -> int:
+        ...
+
+    def ciphertext(self) -> bytes:
+        ...
+
+    @staticmethod
+    def from_bytes(data: bytes) -> ThresholdDecryptionRequest:
+        ...
+
+    def __bytes__(self) -> bytes:
+        ...
+
+
+class ThresholdDecryptionResponse:
+
+    def __init__(self, decryption_share: bytes):
+        ...
+
+    def decryption_share(self) -> bytes:
+        ...
+
+    @staticmethod
+    def from_bytes(data: bytes) -> ThresholdDecryptionResponse:
+        ...
+
+    def __bytes__(self) -> bytes:
+        ...
```

### Comparing `nucypher_core-0.6.1/nucypher_core/umbral.py` & `nucypher_core-0.7.0/nucypher_core/umbral.py`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.6.1/nucypher_core/umbral.pyi` & `nucypher_core-0.7.0/nucypher_core/umbral.pyi`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.6.1/nucypher_core.egg-info/PKG-INFO` & `nucypher_core-0.7.0/nucypher_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nucypher-core
-Version: 0.6.1
+Version: 0.7.0
 Summary: Protocol structures of Nucypher network
-Home-page: https://github.com/nucypher/nucypher-core/tree/master/nucypher-core-python
+Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
@@ -33,8 +33,8 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/nucypher-core
 [pypi-link]: https://pypi.org/project/nucypher-core/
 [pypi-license-image]: https://img.shields.io/pypi/l/nucypher-core
 [rtd-image]: https://readthedocs.org/projects/nucypher-core/badge/?version=latest
 [rtd-link]: https://nucypher-core.readthedocs.io/en/latest/
-[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/master/nucypher-core
+[nucypher-core]: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core
```

### Comparing `nucypher_core-0.6.1/setup.py` & `nucypher_core-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="nucypher_core",
     description="Protocol structures of Nucypher network",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.1",
+    version="0.7.0",
     author="Bogdan Opanchuk",
     author_email="bogdan@opanchuk.net",
-    url="https://github.com/nucypher/nucypher-core/tree/master/nucypher-core-python",
+    url="https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python",
     rust_extensions=[RustExtension("nucypher_core._nucypher_core", binding=Binding.PyO3, debug=False)],
     packages=["nucypher_core"],
     package_data = {
         'nucypher_core': ['py.typed', '__init__.pyi', 'umbral.pyi'],
     },
     # rust extensions are not zip safe, just like C-extensions.
     zip_safe=False,
```

### Comparing `nucypher_core-0.6.1/src/lib.rs` & `nucypher_core-0.7.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 use alloc::collections::{BTreeMap, BTreeSet};
 
 use pyo3::class::basic::CompareOp;
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::pyclass::PyClass;
 use pyo3::types::{PyBytes, PyUnicode};
-
-use nucypher_core::ProtocolObject;
 use umbral_pre::bindings_python::{
     Capsule, PublicKey, RecoverableSignature, SecretKey, Signer, VerificationError,
     VerifiedCapsuleFrag, VerifiedKeyFrag,
 };
 
+use nucypher_core::FerveoVariant;
+use nucypher_core::ProtocolObject;
+
 fn to_bytes<'a, T, U>(obj: &T) -> PyObject
 where
     T: AsRef<U>,
     U: ProtocolObject<'a>,
 {
     let serialized = obj.as_ref().to_bytes();
     Python::with_gil(|py| -> PyObject { PyBytes::new(py, &serialized).into() })
@@ -627,14 +628,137 @@
 
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 //
+// Threshold Decryption Request
+//
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct ThresholdDecryptionRequest {
+    backend: nucypher_core::ThresholdDecryptionRequest,
+}
+
+#[pymethods]
+impl ThresholdDecryptionRequest {
+    #[new]
+    pub fn new(
+        id: u16,
+        variant: u8,
+        ciphertext: &[u8], // TODO use ferveo Ciphertext type
+        conditions: Option<&Conditions>,
+        context: Option<&Context>,
+    ) -> PyResult<Self> {
+        let ferveo_variant = match variant {
+            0 => FerveoVariant::SIMPLE,
+            1 => FerveoVariant::PRECOMPUTED,
+            _ => {
+                return Err(PyValueError::new_err(
+                    "Invalid ThresholdDecryptionRequest variant",
+                ))
+            }
+        };
+
+        Ok(Self {
+            backend: nucypher_core::ThresholdDecryptionRequest::new(
+                id,
+                ciphertext,
+                conditions
+                    .map(|conditions| conditions.backend.clone())
+                    .as_ref(),
+                context.map(|context| context.backend.clone()).as_ref(),
+                ferveo_variant,
+            ),
+        })
+    }
+
+    #[getter]
+    pub fn id(&self) -> u16 {
+        self.backend.ritual_id
+    }
+
+    #[getter]
+    pub fn conditions(&self) -> Option<Conditions> {
+        self.backend
+            .conditions
+            .clone()
+            .map(|conditions| Conditions {
+                backend: conditions,
+            })
+    }
+
+    #[getter]
+    pub fn context(&self) -> Option<Context> {
+        self.backend
+            .context
+            .clone()
+            .map(|context| Context { backend: context })
+    }
+
+    #[getter]
+    pub fn ciphertext(&self) -> &[u8] {
+        self.backend.ciphertext.as_ref()
+    }
+
+    #[getter]
+    pub fn variant(&self) -> u8 {
+        match self.backend.variant {
+            FerveoVariant::SIMPLE => 0,
+            FerveoVariant::PRECOMPUTED => 1,
+        }
+    }
+
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::ThresholdDecryptionRequest>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+}
+
+//
+// Threshold Decryption Response
+//
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct ThresholdDecryptionResponse {
+    backend: nucypher_core::ThresholdDecryptionResponse,
+}
+
+#[pymethods]
+impl ThresholdDecryptionResponse {
+    #[new]
+    pub fn new(decryption_share: &[u8]) -> Self {
+        ThresholdDecryptionResponse {
+            backend: nucypher_core::ThresholdDecryptionResponse::new(decryption_share),
+        }
+    }
+
+    #[getter]
+    pub fn decryption_share(&self) -> &[u8] {
+        self.backend.decryption_share.as_ref()
+    }
+
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::ThresholdDecryptionResponse>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+}
+
+//
 // RetrievalKit
 //
 
 #[pyclass(module = "nucypher_core")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct RetrievalKit {
     backend: nucypher_core::RetrievalKit,
@@ -767,26 +891,28 @@
     #[new]
     pub fn new(
         staking_provider_address: &Address,
         domain: &str,
         timestamp_epoch: u32,
         verifying_key: &PublicKey,
         encrypting_key: &PublicKey,
+        ferveo_public_key: &[u8], // TODO use ferveo PublicKey type
         certificate_der: &[u8],
         host: &str,
         port: u16,
         operator_signature: &RecoverableSignature,
     ) -> PyResult<Self> {
         Ok(Self {
             backend: nucypher_core::NodeMetadataPayload {
                 staking_provider_address: staking_provider_address.backend,
                 domain: domain.to_string(),
                 timestamp_epoch,
                 verifying_key: *verifying_key.as_ref(),
                 encrypting_key: *encrypting_key.as_ref(),
+                ferveo_public_key: ferveo_public_key.into(),
                 certificate_der: certificate_der.into(),
                 host: host.to_string(),
                 port,
                 operator_signature: operator_signature.as_ref().clone(),
             },
         })
     }
@@ -805,14 +931,19 @@
 
     #[getter]
     fn encrypting_key(&self) -> PublicKey {
         self.backend.encrypting_key.into()
     }
 
     #[getter]
+    fn ferveo_public_key(&self) -> &[u8] {
+        self.backend.ferveo_public_key.as_ref()
+    }
+
+    #[getter]
     fn operator_signature(&self) -> RecoverableSignature {
         self.backend.operator_signature.clone().into()
     }
 
     #[getter]
     fn domain(&self) -> &str {
         &self.backend.domain
@@ -1084,14 +1215,16 @@
     m.add_class::<RevocationOrder>()?;
     m.add_class::<NodeMetadata>()?;
     m.add_class::<NodeMetadataPayload>()?;
     m.add_class::<FleetStateChecksum>()?;
     m.add_class::<MetadataRequest>()?;
     m.add_class::<MetadataResponsePayload>()?;
     m.add_class::<MetadataResponse>()?;
+    m.add_class::<ThresholdDecryptionRequest>()?;
+    m.add_class::<ThresholdDecryptionResponse>()?;
 
     let umbral_module = PyModule::new(py, "umbral")?;
 
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKeyFactory>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::PublicKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::Capsule>()?;
```

