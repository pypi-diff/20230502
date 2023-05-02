# Comparing `tmp/evervault_attestation_bindings-0.1.0a5.tar.gz` & `tmp/evervault_attestation_bindings-0.2.0.tar.gz`

## Comparing `evervault_attestation_bindings-0.1.0a5.tar` & `evervault_attestation_bindings-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 evervault_attestation_bindings-0.1.0a5/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/.gitignore
--rw-r--r--   0     1001      123      447 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/Makefile.toml
--rw-r--r--   0     1001      123      123 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/README.md
--rw-r--r--   0     1001      123      360 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/pyproject.toml
--rw-r--r--   0     1001      123     3055 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/src/lib.rs
--rw-r--r--   0     1001      123    42970 2023-02-09 08:36:28.000000 evervault_attestation_bindings-0.1.0a5/Cargo.lock
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 evervault_attestation_bindings-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 evervault_attestation_bindings-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      447 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/Makefile.toml
+-rw-r--r--   0     1001      123      123 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/README.md
+-rw-r--r--   0     1001      123      358 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     3411 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    42950 2023-05-02 09:20:28.000000 evervault_attestation_bindings-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 evervault_attestation_bindings-0.2.0/PKG-INFO
```

### Comparing `evervault_attestation_bindings-0.1.0a5/Cargo.toml` & `evervault_attestation_bindings-0.2.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "evervault_attestation_bindings"
 crate-type = ["cdylib"]
 
 [dependencies]
-attestation-doc-validation = { version = "0.5.0-beta" }
+attestation-doc-validation = { version = "0.6.0" }
 pyo3 = { version = "0.18", features = ["extension-module"] }
```

### Comparing `evervault_attestation_bindings-0.1.0a5/.gitignore` & `evervault_attestation_bindings-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `evervault_attestation_bindings-0.1.0a5/src/lib.rs` & `evervault_attestation_bindings-0.2.0/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -83,27 +83,36 @@
     }
 
     fn pcr_8(&self) -> Option<&str> {
         self.pcr_8.as_deref()
     }
 }
 
-/// Top level function to attest the Cage being connected to. Returns true on successful attestation, or errors if attestation fails.
+/// Top level function to attest the Cage being connected to.
+/// * If the cert fails to parse, return an error
+/// * If the attestation doc fails to validate, return an error
+/// * If the list of PCRs to check is empty, return true
+/// * If any of the PCRs in the list match, return true
+/// * If they all fail, return the last error
 #[pyfunction]
-pub fn attest_connection(cert: &[u8], expected_pcrs: &PCRs) -> PyResult<bool> {
+pub fn attest_connection(cert: &[u8], expected_pcrs_list: Vec<PCRs>) -> PyResult<bool> {
     let cert =
         parse_cert(cert).map_err(|parse_err| PyValueError::new_err(format!("{parse_err}")))?;
 
     let validated_attestation_doc = validate_attestation_doc_in_cert(&cert)
         .map_err(|cert_err| PyValueError::new_err(format!("{cert_err}")))?;
 
-    validate_expected_pcrs(&validated_attestation_doc, expected_pcrs)
-        .map_err(|pcr_err| PyValueError::new_err(format!("{pcr_err}")))?;
-
-    Ok(true)
+    let mut result = Ok(true);
+    for expected_pcrs in expected_pcrs_list {
+        match validate_expected_pcrs(&validated_attestation_doc, &expected_pcrs) {
+            Ok(_) => return Ok(true),
+            Err(err) => result = Err(PyValueError::new_err(format!("{err}"))),
+        }
+    }
+    result
 }
 
 /// A small python module offering bindings to the rust attestation doc validation project
 #[pymodule]
 fn evervault_attestation_bindings(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(attest_connection, m)?)?;
     m.add_class::<PCRs>()?;
```

### Comparing `evervault_attestation_bindings-0.1.0a5/Cargo.lock` & `evervault_attestation_bindings-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "attestation-doc-validation"
-version = "0.5.0-beta"
+version = "0.6.0"
 dependencies = [
  "aes",
  "aes-gcm",
  "aws-nitro-enclaves-cose",
  "base64 0.21.0",
  "der",
  "ecdsa",
@@ -119,17 +119,17 @@
  "thiserror",
  "webpki",
  "x509-parser",
 ]
 
 [[package]]
 name = "attestation-doc-validation"
-version = "0.5.0-beta"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c1d46e832e4a525c36b005cda831994d00cabf5842ff4c07078a0f8a2b9398"
+checksum = "07f41a9d17e59a15b9208f55985f3f0eea9830695cd6280acce32e9619ded698"
 dependencies = [
  "aes",
  "aes-gcm",
  "aws-nitro-enclaves-cose",
  "base64 0.21.0",
  "der",
  "ecdsa",
@@ -521,27 +521,27 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -798,15 +798,15 @@
  "libloading",
 ]
 
 [[package]]
 name = "node-attestation-bindings"
 version = "0.0.0"
 dependencies = [
- "attestation-doc-validation 0.5.0-beta (registry+https://github.com/rust-lang/crates.io-index)",
+ "attestation-doc-validation 0.6.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "napi",
  "napi-build",
  "napi-derive",
 ]
 
 [[package]]
 name = "nom"
@@ -1064,15 +1064,15 @@
  "syn",
 ]
 
 [[package]]
 name = "python-attestation-bindings"
 version = "0.0.0"
 dependencies = [
- "attestation-doc-validation 0.5.0-beta (registry+https://github.com/rust-lang/crates.io-index)",
+ "attestation-doc-validation 0.6.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `evervault_attestation_bindings-0.1.0a5/PKG-INFO` & `evervault_attestation_bindings-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evervault_attestation_bindings
-Version: 0.1.0a5
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A Python library for attesting Nitro Enclaves according to the Evervault Cages attestation protocol.
 Home-Page: https://github.com/evervault/attestation-doc-validation
 License: Apache-2.0
 Requires-Python: >=3.6
```

