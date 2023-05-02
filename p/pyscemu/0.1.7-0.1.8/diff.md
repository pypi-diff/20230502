# Comparing `tmp/pyscemu-0.1.7.tar.gz` & `tmp/pyscemu-0.1.8.tar.gz`

## Comparing `pyscemu-0.1.7.tar` & `pyscemu-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.7/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.7/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.7/.gitignore
--rw-r--r--   0     1000     1000    11671 2023-05-01 10:48:40.000000 pyscemu-0.1.7/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10052 2023-05-01 10:45:28.000000 pyscemu-0.1.7/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.7/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.1.7/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.7/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.7/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.7/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.7/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.7/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.7/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.7/pyproject.toml
--rw-r--r--   0     1000     1000    26607 2023-05-01 10:48:57.000000 pyscemu-0.1.7/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-05-01 10:49:11.000000 pyscemu-0.1.7/Cargo.lock
--rw-r--r--   0        0        0    10378 1970-01-01 00:00:00.000000 pyscemu-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.8/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.8/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.8/.gitignore
+-rw-r--r--   0     1000     1000    11671 2023-05-01 10:48:40.000000 pyscemu-0.1.8/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10073 2023-05-01 10:57:14.000000 pyscemu-0.1.8/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.8/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.1.8/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.8/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.8/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.8/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.8/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-01 14:50:10.000000 pyscemu-0.1.8/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.8/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.1.8/pyproject.toml
+-rw-r--r--   0     1000     1000    26607 2023-05-01 10:48:57.000000 pyscemu-0.1.8/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-05-02 14:50:06.000000 pyscemu-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 pyscemu-0.1.8/PKG-INFO
```

### Comparing `pyscemu-0.1.7/.github/workflows/CI.yml` & `pyscemu-0.1.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/.gitignore` & `pyscemu-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/DOCUMENTATION.md` & `pyscemu-0.1.8/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/README.md` & `pyscemu-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Install
 ```bash
 pip install --upgrade pip
 pip3 install --upgrade pip
 curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
+pip3 install pyscemu
 ```
 
 ## Mac Install
 same procedure, if there is a problem with !tapi-tbd the solution is:
 ```bash
 sudo xcode-select --switch /Library/Developer/CommandLineTools
 ```
```

### Comparing `pyscemu-0.1.7/examples/danabot_rsa.ipynb` & `pyscemu-0.1.8/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/examples/raccoon_strings.ipynb` & `pyscemu-0.1.8/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/examples/scripts/raccoon_strings.py` & `pyscemu-0.1.8/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/examples/scripts/test.py` & `pyscemu-0.1.8/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/examples/scripts/xloader_dexor.py` & `pyscemu-0.1.8/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/examples/xloader_keygen.ipynb` & `pyscemu-0.1.8/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/src/lib.rs` & `pyscemu-0.1.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.7/Cargo.lock` & `pyscemu-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.11.7"
+version = "0.11.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2cffdb15b120776d2eed7a3cb432cc77fb271ea56da588f41a45c82606678845"
+checksum = "69b6a7b3425adce0f6b153904721009046d805ff447783c2dd2e00b03ac6afc9"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.7/PKG-INFO` & `pyscemu-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
 
 ## Install
 ```bash
 pip install --upgrade pip
 pip3 install --upgrade pip
 curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
+pip3 install pyscemu
 ```
 
 ## Mac Install
 same procedure, if there is a problem with !tapi-tbd the solution is:
 ```bash
 sudo xcode-select --switch /Library/Developer/CommandLineTools
 ```
```

