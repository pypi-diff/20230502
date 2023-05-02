# Comparing `tmp/votable_cli-0.2.0.tar.gz` & `tmp/votable_cli-0.2.3.tar.gz`

## Comparing `votable_cli-0.2.0.tar` & `votable_cli-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 votable_cli-0.2.0/local_dependencies/votable/Cargo.toml
--rw-r--r--   0     1001      123      310 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/clitest.yml
--rw-r--r--   0     1001      123     6858 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/deploy.yml
--rw-r--r--   0     1001      123     1433 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/deploy_aarch64.yml
--rw-r--r--   0     1001      123      340 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/libtest.yml
--rw-r--r--   0     1001      123     6049 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/release.yml
--rw-r--r--   0     1001      123      454 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/.github/workflows/wasmtest.yml
--rw-r--r--   0     1001      123      459 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/CHANGELOG.md
--rw-r--r--   0     1001      123    10852 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/LICENSE-APACHE
--rw-r--r--   0     1001      123     1076 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/LICENSE-MIT
--rw-r--r--   0     1001      123    18866 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/README.md
--rw-r--r--   0     1001      123    14681 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/coosys.rs
--rw-r--r--   0     1001      123     3886 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/binary.rs
--rw-r--r--   0     1001      123     3881 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/binary2.rs
--rw-r--r--   0     1001      123     3171 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/fits.rs
--rw-r--r--   0     1001      123     8822 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/mod.rs
--rw-r--r--   0     1001      123     8852 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/stream.rs
--rw-r--r--   0     1001      123     1744 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/data/tabledata.rs
--rw-r--r--   0     1001      123     2117 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/datatype.rs
--rw-r--r--   0     1001      123     3697 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/desc.rs
--rw-r--r--   0     1001      123     2768 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/error.rs
--rw-r--r--   0     1001      123    11094 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/field.rs
--rw-r--r--   0     1001      123     3000 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/fieldref.rs
--rw-r--r--   0     1001      123    12277 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/group.rs
--rw-r--r--   0     1001      123      123 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/b64/mod.rs
--rw-r--r--   0     1001      123    10885 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/b64/read.rs
--rw-r--r--   0     1001      123     9152 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/b64/write.rs
--rw-r--r--   0     1001      123    14232 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/mem.rs
--rw-r--r--   0     1001      123    47587 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/mod.rs
--rw-r--r--   0     1001      123     6316 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/impls/visitors.rs
--rw-r--r--   0     1001      123     7340 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/info.rs
--rw-r--r--   0     1001      123     8540 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/iter/elems.rs
--rw-r--r--   0     1001      123     8737 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/iter/mod.rs
--rw-r--r--   0     1001      123     3978 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/iter/strings.rs
--rw-r--r--   0     1001      123    16748 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/lib.rs
--rw-r--r--   0     1001      123     4579 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/link.rs
--rw-r--r--   0     1001      123    14218 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/macros.rs
--rw-r--r--   0     1001      123     7681 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/param.rs
--rw-r--r--   0     1001      123     2978 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/paramref.rs
--rw-r--r--   0     1001      123    14451 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/resource.rs
--rw-r--r--   0     1001      123     9844 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/table.rs
--rw-r--r--   0     1001      123    12228 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/timesys.rs
--rw-r--r--   0     1001      123    12930 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/values.rs
--rw-r--r--   0     1001      123      756 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/vodml.rs
--rw-r--r--   0     1001      123    30056 2023-03-30 12:22:05.000000 votable_cli-0.2.0/local_dependencies/votable/src/votable.rs
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 votable_cli-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      209 2023-03-30 12:22:05.000000 votable_cli-0.2.0/CHANGELOG.md
--rw-r--r--   0     1001      123      123 2023-03-30 12:22:05.000000 votable_cli-0.2.0/COPYING
--rw-r--r--   0     1001      123    10852 2023-03-30 12:22:05.000000 votable_cli-0.2.0/LICENSE-APACHE
--rw-r--r--   0     1001      123     1076 2023-03-30 12:22:05.000000 votable_cli-0.2.0/LICENSE-MIT
--rw-r--r--   0     1001      123     3927 2023-03-30 12:22:05.000000 votable_cli-0.2.0/README.md
--rw-r--r--   0     1001      123      962 2023-03-30 12:22:05.000000 votable_cli-0.2.0/doc/vot.1.txt.tpl
--rw-r--r--   0     1001      123      652 2023-03-30 12:22:05.000000 votable_cli-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     2902 2023-03-30 12:22:05.000000 votable_cli-0.2.0/src/main.rs
--rw-r--r--   0        0        0    13854 2023-03-30 12:24:01.000000 votable_cli-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     4616 1970-01-01 00:00:00.000000 votable_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 votable_cli-0.2.3/local_dependencies/votable/Cargo.toml
+-rw-r--r--   0     1001      123      310 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/clitest.yml
+-rw-r--r--   0     1001      123     6858 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     1433 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/deploy_aarch64.yml
+-rw-r--r--   0     1001      123      340 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/libtest.yml
+-rw-r--r--   0     1001      123     6049 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      454 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/.github/workflows/wasmtest.yml
+-rw-r--r--   0     1001      123      848 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/CHANGELOG.md
+-rw-r--r--   0     1001      123    10852 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1076 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/LICENSE-MIT
+-rw-r--r--   0     1001      123    18890 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/README.md
+-rw-r--r--   0     1001      123    14681 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/coosys.rs
+-rw-r--r--   0     1001      123     3886 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/binary.rs
+-rw-r--r--   0     1001      123     3881 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/binary2.rs
+-rw-r--r--   0     1001      123     3171 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/fits.rs
+-rw-r--r--   0     1001      123     8822 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/mod.rs
+-rw-r--r--   0     1001      123     8852 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/stream.rs
+-rw-r--r--   0     1001      123     1744 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/data/tabledata.rs
+-rw-r--r--   0     1001      123     2117 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/datatype.rs
+-rw-r--r--   0     1001      123     4240 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/definitions.rs
+-rw-r--r--   0     1001      123     3697 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/desc.rs
+-rw-r--r--   0     1001      123     2768 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/error.rs
+-rw-r--r--   0     1001      123    11136 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/field.rs
+-rw-r--r--   0     1001      123     3000 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/fieldref.rs
+-rw-r--r--   0     1001      123    12277 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/group.rs
+-rw-r--r--   0     1001      123      123 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/b64/mod.rs
+-rw-r--r--   0     1001      123    10885 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/b64/read.rs
+-rw-r--r--   0     1001      123     9152 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/b64/write.rs
+-rw-r--r--   0     1001      123    14232 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/mem.rs
+-rw-r--r--   0     1001      123    47587 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/mod.rs
+-rw-r--r--   0     1001      123     6316 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/impls/visitors.rs
+-rw-r--r--   0     1001      123     7340 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/info.rs
+-rw-r--r--   0     1001      123     8540 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/iter/elems.rs
+-rw-r--r--   0     1001      123     8737 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/iter/mod.rs
+-rw-r--r--   0     1001      123     3978 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/iter/strings.rs
+-rw-r--r--   0     1001      123    16769 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/lib.rs
+-rw-r--r--   0     1001      123     4623 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/link.rs
+-rw-r--r--   0     1001      123    15936 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/macros.rs
+-rw-r--r--   0     1001      123     7724 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/param.rs
+-rw-r--r--   0     1001      123     2978 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/paramref.rs
+-rw-r--r--   0     1001      123    14451 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/resource.rs
+-rw-r--r--   0     1001      123     9844 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/table.rs
+-rw-r--r--   0     1001      123    12228 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/timesys.rs
+-rw-r--r--   0     1001      123    13010 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/values.rs
+-rw-r--r--   0     1001      123      756 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/vodml.rs
+-rw-r--r--   0     1001      123    32427 2023-05-02 13:22:14.000000 votable_cli-0.2.3/local_dependencies/votable/src/votable.rs
+-rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 votable_cli-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123      847 2023-05-02 13:22:14.000000 votable_cli-0.2.3/CHANGELOG.md
+-rw-r--r--   0     1001      123      123 2023-05-02 13:22:14.000000 votable_cli-0.2.3/COPYING
+-rw-r--r--   0     1001      123    10852 2023-05-02 13:22:14.000000 votable_cli-0.2.3/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1076 2023-05-02 13:22:14.000000 votable_cli-0.2.3/LICENSE-MIT
+-rw-r--r--   0     1001      123     3927 2023-05-02 13:22:14.000000 votable_cli-0.2.3/README.md
+-rw-r--r--   0     1001      123      962 2023-05-02 13:22:14.000000 votable_cli-0.2.3/doc/vot.1.txt.tpl
+-rw-r--r--   0     1001      123      652 2023-05-02 13:22:14.000000 votable_cli-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123     2902 2023-05-02 13:22:14.000000 votable_cli-0.2.3/src/main.rs
+-rw-r--r--   0        0        0    13842 2023-05-02 13:23:31.000000 votable_cli-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     4616 1970-01-01 00:00:00.000000 votable_cli-0.2.3/PKG-INFO
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/Cargo.toml` & `votable_cli-0.2.3/local_dependencies/votable/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "votable"
-version = "0.2.0"
+version = "0.2.3"
 authors = [
   "F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>",
   "T. Dumortier <thibault.dumortier@astro.unistra.fr>"
 ]
 description = """
 Rust implementation of a VOTable serializer/deserializer with support for
 format other than XML, such as JSON, TOML or YAML.
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/.github/workflows/deploy.yml` & `votable_cli-0.2.3/local_dependencies/votable/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/.github/workflows/deploy_aarch64.yml` & `votable_cli-0.2.3/local_dependencies/votable/.github/workflows/deploy_aarch64.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/.github/workflows/release.yml` & `votable_cli-0.2.3/local_dependencies/votable/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/LICENSE-APACHE` & `votable_cli-0.2.3/local_dependencies/votable/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/LICENSE-MIT` & `votable_cli-0.2.3/local_dependencies/votable/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/README.md` & `votable_cli-0.2.3/local_dependencies/votable/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Status
 
 This library is in an early stage of development.  
 We are (reasonably) open to changes in the various format, e.g.:
 * we could flag attributes with a '@' prefix
 * we could use upper case elements tag names
 * we could remove the 's' suffix in elements arrays
-* we could change the `pos_infos` name for something else
+* we could change the `post_infos` name for something else
 * ...
 
 More testing is required, especially the bit type and arrays.
 Please, provide us with your VOTable examples!
 
 
 ## Why JSON, TOML, YAML in addition to XML
@@ -548,14 +548,15 @@
     let votable = votable_it.end_of_it();
     println!("VOTable: {:?}", votable);
 ```
 
 
 ## To-do list
 
+* [ ] Support `CDATA`?
 * [ ] Fill the doc for the Rust library (but I so far do not know people interested in such a lib since Rust is not very used in the astronomy community so far, so...)
 * [ ] Add a check method ensuring that user input VOTAbleValue (using the API to build a VOTable) 
       matches the table schema (or automatically converting in the right VOTableValue)
 * [ ] Add much more tests!
 * [ ] Add possibility to convert to/from `TABLEDATA`, `BINARY`, `BINARY2`
 * [ ] Enrich `votable::impls::Schema.serialize_seed` (possible bugs when deserializing JSON/TOML/YAML arrays and converting to BINARY or BINARY2)
 * [ ] Write a custom deserializer for `VOTableValue` (look at cargo-expand output for a basis)
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/coosys.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/coosys.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/binary.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/binary.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/binary2.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/binary2.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/fits.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/fits.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/mod.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/stream.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/stream.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/data/tabledata.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/data/tabledata.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/datatype.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/datatype.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/desc.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/desc.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/error.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/error.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/field.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/field.rs`

 * *Files 1% similar despite different names*

```diff
@@ -192,16 +192,16 @@
         b"name" => { field.name = value.to_string(); field },
         b"datatype" =>  { 
           field.datatype = value.parse::<Datatype>().map_err(VOTableError::ParseDatatype)?;
           has_datatype = true;
           field
         },
         b"unit" => field.set_unit(value),
-        b"precision" => field.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?),
-        b"width" => field.set_width(value.parse().map_err(VOTableError::ParseInt)?),
+        b"precision" if !value.is_empty() => field.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?),
+        b"width" if !value.is_empty() => field.set_width(value.parse().map_err(VOTableError::ParseInt)?),
         b"xtype" => field.set_xtype(value),
         b"ref" => field.set_ref(value),
         b"ucd" => field.set_ucd(value),
         b"utype" => field.set_utype(value),
         b"arraysize" => field.set_arraysize(value),
         _ => field.insert_extra(
           str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/fieldref.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/fieldref.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/group.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/group.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/impls/b64/read.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/impls/b64/read.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/impls/b64/write.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/impls/b64/write.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/impls/mem.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/impls/mem.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/impls/mod.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/impls/visitors.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/impls/visitors.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/info.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/info.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/iter/elems.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/iter/elems.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/iter/mod.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/iter/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/iter/strings.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/iter/strings.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/lib.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 pub mod macros;
 pub mod error;
 pub mod impls;
 pub mod coosys;
 pub mod data;
 pub mod datatype;
 pub mod desc;
+pub mod definitions;
 pub mod field;
 pub mod fieldref;
 pub mod group;
 pub mod info;
 pub mod link;
 pub mod param;
 pub mod paramref;
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/link.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/link.rs`

 * *Files 3% similar despite different names*

```diff
@@ -125,19 +125,19 @@
     _context: &Self::Context,
   ) -> Result<Reader<R>, VOTableError> {
     read_content!(Self, self, reader, reader_buff)
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    _reader: &mut Reader<R>,
-    _reader_buff: &mut Vec<u8>,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    todo!()
+    read_content_by_ref!(Self, self, reader, reader_buff)
   }
   
   fn write<W: Write>(
     &mut self, 
     writer: &mut Writer<W>, 
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/macros.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/macros.rs`

 * *Files 6% similar despite different names*

```diff
@@ -139,68 +139,98 @@
     }
   }
 }
 
 macro_rules! read_content {
   ($Self:ident, $self:ident, $reader:ident, $reader_buff:ident) => {
     {
-      let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
-      let link_content = match &event {
+      /*let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
+      let content = match &event {
         Event::Text(e) => e.unescape_and_decode(&$reader).map_err(VOTableError::Read),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: Text. Actual: {:?}.", $Self::TAG, event))),
       }?;
-      $self.content = Some(link_content);
+      $self.content = Some(content);
       let event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
       match &event {
         Event::End(e) if e.local_name() == $Self::TAG_BYTES => Ok($reader),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End. Actual: {:?}.", $Self::TAG, event))),
+      }*/
+      let mut content = String::new();
+      loop {
+        let mut event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
+        match &mut event {
+          Event::Text(e) => content.push_str(e.unescape_and_decode(&$reader).map_err(VOTableError::Read)?.as_str()),
+          Event::CData(e) => content.push_str(str::from_utf8(e.clone().into_inner().as_ref()).map_err(VOTableError::Utf8)?),
+          Event::End(e) if e.local_name() == $Self::TAG_BYTES => { 
+            $self.content = Some(content);
+            return Ok($reader);
+          },
+          Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
+          _ => eprintln!("Discarded event in {}: {:?}", Self::TAG, event),
+          // _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End or Text or CDATA. Actual: {:?}.", $Self::TAG, event))),
+        }
       }
     }
   };
   ($Self:ident, $self:ident, $reader:ident, $reader_buff:ident, $content:tt) => {
     {
-      let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
-      let link_content = match &event {
+      /*let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
+      let content = match &event {
         Event::Text(e) => e.unescape_and_decode(&$reader).map_err(VOTableError::Read),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: Text. Actual: {:?}.", $Self::TAG, event))),
       }?;
-      $self.$content = link_content;
+      $self.$content = content;
       let event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
       match &event {
         Event::End(e) if e.local_name() == $Self::TAG_BYTES => Ok($reader),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End. Actual: {:?}.", $Self::TAG, event))),
+      }*/
+      let mut content = String::new();
+      loop {
+        let mut event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
+        match &mut event {
+          Event::Text(e) => content.push_str(e.unescape_and_decode(&$reader).map_err(VOTableError::Read)?.as_str()),
+          Event::CData(e) => content.push_str(std::str::from_utf8(e.clone().into_inner().as_ref()).map_err(VOTableError::Utf8)?),
+          Event::End(e) if e.local_name() == $Self::TAG_BYTES => { 
+            $self.$content = content;
+            return Ok($reader);
+          },
+          Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
+          _ => eprintln!("Discarded event in {}: {:?}", Self::TAG, event),
+          // _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End or Text or CDATA. Actual: {:?}.", $Self::TAG, event))),
+        }
       }
     }
   };
 }
 
 macro_rules! read_content_by_ref {
   ($Self:ident, $self:ident, $reader:ident, $reader_buff:ident) => {
     {
       let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
-      let link_content = match &event {
+      let content = match &event {
         Event::Text(e) => e.unescape_and_decode(&$reader).map_err(VOTableError::Read),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: Text. Actual: {:?}.", $Self::TAG, event))),
       }?;
-      $self.content = Some(link_content);
+      $self.content = Some(content);
       let event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
       match &event {
         Event::End(e) if e.local_name() == $Self::TAG_BYTES => Ok(()),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End. Actual: {:?}.", $Self::TAG, event))),
       }
     }
   };
   ($Self:ident, $self:ident, $reader:ident, $reader_buff:ident, $content:tt) => {
     {
       let event: Event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
-      let link_content = match &event {
+      let content = match &event {
         Event::Text(e) => e.unescape_and_decode(&$reader).map_err(VOTableError::Read),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: Text. Actual: {:?}.", $Self::TAG, event))),
       }?;
-      $self.$content = link_content;
+      $self.$content = content;
       let event = $reader.read_event($reader_buff).map_err(VOTableError::Read)?;
       match &event {
         Event::End(e) if e.local_name() == $Self::TAG_BYTES => Ok(()),
         _ => Err(VOTableError::Custom(format!("Unexpected {} event. Expected: End. Actual: {:?}.", $Self::TAG, event))),
       }
     }
   };
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/param.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/param.rs`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
           param
         }
         b"datatype" => {
           param.field.datatype = value.parse::<Datatype>().map_err(VOTableError::ParseDatatype)?;
           param
         }
         b"unit" => param.set_utype(value),
-        b"precision" => param.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?),
-        b"width" => param.set_width(value.parse().map_err(VOTableError::ParseInt)?),
+        b"precision" if !value.is_empty() => param.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?),
+        b"width"  if !value.is_empty() => param.set_width(value.parse().map_err(VOTableError::ParseInt)?),
         b"xtype" => param.set_xtype(value),
         b"ref" => param.set_ref(value),
         b"ucd" => param.set_ucd(value),
         b"utype" => param.set_utype(value),
         b"arraysize" => param.set_arraysize(value),
         b"value" => {
           param.value = value.to_string();
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/paramref.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/paramref.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/resource.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/resource.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/table.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/table.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/timesys.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/timesys.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/values.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/values.rs`

 * *Files 2% similar despite different names*

```diff
@@ -350,50 +350,50 @@
     }
     Ok(values)
   }
 
   fn read_sub_elements<R: BufRead>(
     &mut self,
     mut reader: Reader<R>,
-    mut reader_buff: &mut Vec<u8>,
+    reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<Reader<R>, VOTableError> {
+    self.read_sub_elements_by_ref(&mut reader, reader_buff, _context).map(|()| reader)
+  }
+
+  fn read_sub_elements_by_ref<R: BufRead>(
+    &mut self,
+    mut reader: &mut Reader<R>,
+    mut reader_buff: &mut Vec<u8>,
+    _context: &Self::Context,
+  ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => {
           match e.local_name() {
-            Opt::TAG_BYTES => self.opts.push(from_event_start!(Opt, reader, reader_buff, e)),
+            Opt::TAG_BYTES => self.opts.push(from_event_start_by_ref!(Opt, reader, reader_buff, e)),
             _ => return Err(VOTableError::UnexpectedStartTag(e.local_name().to_vec(), Self::TAG)),
           }
         }
         Event::Empty(ref e) => {
           match e.local_name() {
             Min::TAG_BYTES => self.min = Some(Min::from_event_empty(e)?),
             Max::TAG_BYTES => self.max = Some(Max::from_event_empty(e)?),
             Opt::TAG_BYTES => self.opts.push(Opt::from_event_empty(e)?),
             _ => return Err(VOTableError::UnexpectedEmptyTag(e.local_name().to_vec(), Self::TAG)),
           }
         }
-        Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(reader),
+        Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => eprintln!("Discarded event in {}: {:?}", Self::TAG, event),
       }
     }
   }
 
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    _reader: &mut Reader<R>,
-    _reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    todo!()
-  }
-
   fn write<W: Write>(
     &mut self, 
     writer: &mut Writer<W>,
     context: &Self::Context
   ) -> Result<(), VOTableError> {
     if self.min.is_none() && self.max.is_none() && self.opts.is_empty() {
       let mut elem_writer = writer.create_element(Self::TAG_BYTES);
```

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/vodml.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/vodml.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/local_dependencies/votable/src/votable.rs` & `votable_cli-0.2.3/local_dependencies/votable/src/votable.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
   fs::File,
   path::Path,
   str::{self, FromStr},
   io::{BufRead, Write, BufReader, BufWriter},
   collections::HashMap,
 };
 
-
 use quick_xml::{
   Reader, Writer,
   events::{
     BytesStart, Event,
     attributes::Attributes,
   },
 };
@@ -23,69 +22,84 @@
 use crate::is_empty;
 
 use super::{
   QuickXmlReadWrite, TableDataContent,
   error::VOTableError,
   coosys::CooSys,
   desc::Description,
+  definitions::Definitions,
   group::Group,
   info::Info,
   param::Param,
   resource::Resource,
   timesys::TimeSys,
 };
 
 
 #[derive(Clone, Debug, serde::Serialize, serde::Deserialize)]
 pub enum Version {
+  #[serde(rename = "1.0")]
+  V1_0,
+  #[serde(rename = "1.1")]
+  V1_1,
+  #[serde(rename = "1.2")]
+  V1_2,
   #[serde(rename = "1.3")]
   V1_3,
   #[serde(rename = "1.4")]
   V1_4,
 }
 
 impl FromStr for Version {
   type Err = String;
 
   fn from_str(s: &str) -> Result<Self, Self::Err> {
     match s {
+      "1.0" => Ok(Version::V1_0),
+      "1.1" => Ok(Version::V1_1),
+      "1.2" => Ok(Version::V1_2),
       "1.3" => Ok(Version::V1_3),
       "1.4" => Ok(Version::V1_4),
-      _ => Err(format!("Unrecognized version. Actual: '{}'. Expected: '1.3' or '1.4'", s)),
+      _ => Err(format!("Unrecognized version. Actual: '{}'. Expected: '1.1', '1.2', '1.3' or '1.4'", s)),
     }
   }
 }
 
 impl From<&Version> for &'static str {
   fn from(version: &Version) -> Self {
     match version {
+      Version::V1_0 => "1.0",
+      Version::V1_1 => "1.1",
+      Version::V1_2 => "1.2",
       Version::V1_3 => "1.3",
       Version::V1_4 => "1.4",
     }
   }
 }
 
 #[derive(Clone, Debug, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum VOTableElem {
   CooSys(CooSys),
   TimeSys(TimeSys),
   Group(Group),
   Param(Param),
   Info(Info),
+  Definitions(Definitions), // Deprecated since v1.1
 }
 
 impl VOTableElem {
   fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
     match self {
       VOTableElem::CooSys(elem) => elem.write(writer, &()),
       VOTableElem::TimeSys(elem) => elem.write(writer, &()),
       VOTableElem::Group(elem) => elem.write(writer, &()),
       VOTableElem::Param(elem) => elem.write(writer, &()),
       VOTableElem::Info(elem) => elem.write(writer, &()),
+      VOTableElem::Definitions(elem) => elem.write(writer, &()),
     }
   }
 }
 
 #[derive(Clone, Debug, serde::Serialize, serde::Deserialize)]
 pub struct VOTableWrapper<C: TableDataContent> {
   votable: VOTable<C>,
@@ -373,19 +387,19 @@
     Self::from_reader(s)
   }*/
 
   pub(crate) fn from_reader<R: BufRead>(reader: R) -> Result<Self, VOTableError> {
     let mut reader = Reader::from_reader(reader);
     let mut buff: Vec<u8> = Vec::with_capacity(1024);
     loop {
-      let mut event = reader.read_event(&mut buff).unwrap();
+      let mut event = reader.read_event(&mut buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Decl(ref e) => check_declaration(e),
         Event::Start(ref mut e) if e.local_name() == VOTable::<C>::TAG_BYTES => {
-          let mut votable = VOTable::<C>::from_attributes(e.attributes()).unwrap();
+          let mut votable = VOTable::<C>::from_attributes(e.attributes())?;
           votable.read_sub_elements_and_clean(reader, &mut buff, &())?;
           // ignore the remaining of the reader !
           return Ok(votable);
         }
         Event::Text(e) if is_empty(e) => {}
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => eprintln!("Discarded event in {}: {:?}", Self::TAG, event),
@@ -393,19 +407,19 @@
     }
   }
 
   pub(crate) fn from_reader_till_next_resource<R: BufRead>(reader: R, mut reader_buff: &mut Vec<u8>)
     -> Result<(VOTable<C>, Resource<C>, Reader<R>), VOTableError> {
     let mut reader = Reader::from_reader(reader);
     loop {
-      let mut event = reader.read_event(&mut reader_buff).unwrap();
+      let mut event = reader.read_event(&mut reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Decl(ref e) => check_declaration(e),
         Event::Start(ref mut e) if e.local_name() == VOTable::<C>::TAG_BYTES => {
-          let mut votable = VOTable::<C>::from_attributes(e.attributes()).unwrap();
+          let mut votable = VOTable::<C>::from_attributes(e.attributes())?;
           let (resource, reader) = votable.read_till_next_resource(reader, &mut reader_buff)?;
           reader_buff.clear();
           return Ok((votable, resource, reader));
         }
         Event::Text(e) if is_empty(e) => {}
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => eprintln!("Discarded event in {}: {:?}", Self::TAG, event),
@@ -422,14 +436,15 @@
   impl_builder_opt_attr!(description, Description);
 
   impl_builder_push_elem!(CooSys, VOTableElem);
   impl_builder_push_elem!(TimeSys, VOTableElem);
   impl_builder_push_elem!(Group, VOTableElem);
   impl_builder_push_elem!(Param, VOTableElem);
   impl_builder_push_elem!(Info, VOTableElem);
+  impl_builder_push_elem!(Definitions, VOTableElem);
 
   impl_builder_push!(Resource, C);
 
   impl_builder_push_post_info!();
 
   pub fn read_till_next_resource_by_ref<R: BufRead>(
     &mut self,
@@ -500,14 +515,16 @@
               from_event_start_desc!(self, Description, reader, reader_buff, e),
             Info::TAG_BYTES if self.resources.is_empty() =>
               self.elems.push(VOTableElem::Info(from_event_start!(Info, reader, reader_buff, e))),
             Group::TAG_BYTES =>
               self.elems.push(VOTableElem::Group(from_event_start!(Group, reader, reader_buff, e))),
             Param::TAG_BYTES =>
               self.elems.push(VOTableElem::Param(from_event_start!(Param, reader, reader_buff, e))),
+            Definitions::TAG_BYTES =>
+              self.elems.push(VOTableElem::Definitions(from_event_start!(Definitions, reader, reader_buff, e))),
             Resource::<C>::TAG_BYTES => {
               let resource = Resource::<C>::from_attributes(e.attributes())?;
               return Ok((resource, reader));
             }
             Info::TAG_BYTES =>
               self.post_infos.push(from_event_start!(Info, reader, reader_buff, e)),
             _ => return Err(VOTableError::UnexpectedStartTag(e.local_name().to_vec(), Self::TAG)),
@@ -516,14 +533,15 @@
         Event::Empty(ref e) => {
           match e.local_name() {
             Info::TAG_BYTES if self.resources.is_empty() => self.elems.push(VOTableElem::Info(Info::from_event_empty(e)?)),
             CooSys::TAG_BYTES => self.elems.push(VOTableElem::CooSys(CooSys::from_event_empty(e)?)),
             TimeSys::TAG_BYTES => self.elems.push(VOTableElem::TimeSys(TimeSys::from_event_empty(e)?)),
             Group::TAG_BYTES => self.elems.push(VOTableElem::Group(Group::from_event_empty(e)?)),
             Param::TAG_BYTES => self.elems.push(VOTableElem::Param(Param::from_event_empty(e)?)),
+            Definitions::TAG_BYTES => self.elems.push(VOTableElem::Definitions(Definitions::from_event_empty(e)?)),
             Info::TAG_BYTES => self.post_infos.push(Info::from_event_empty(e)?),
             _ => return Err(VOTableError::UnexpectedEmptyTag(e.local_name().to_vec(), Self::TAG)),
           }
         }
         Event::End(e) if e.local_name() == Self::TAG_BYTES =>
           return Err(VOTableError::Custom(String::from("No resource found in the VOTable"))),
         Event::Text(e) if is_empty(e) => {}
@@ -588,28 +606,31 @@
               from_event_start_desc!(self, Description, reader, reader_buff, e),
             Info::TAG_BYTES if self.resources.is_empty() =>
               self.elems.push(VOTableElem::Info(from_event_start!(Info, reader, reader_buff, e))),
             Group::TAG_BYTES =>
               self.elems.push(VOTableElem::Group(from_event_start!(Group, reader, reader_buff, e))),
             Param::TAG_BYTES =>
               self.elems.push(VOTableElem::Param(from_event_start!(Param, reader, reader_buff, e))),
+            Definitions::TAG_BYTES =>
+              self.elems.push(VOTableElem::Definitions(from_event_start!(Definitions, reader, reader_buff, e))),
             Resource::<C>::TAG_BYTES =>
               self.resources.push(from_event_start!(Resource, reader, reader_buff, e)),
             Info::TAG_BYTES =>
               self.post_infos.push(from_event_start!(Info, reader, reader_buff, e)),
             _ => return Err(VOTableError::UnexpectedStartTag(e.local_name().to_vec(), Self::TAG)),
           }
         }
         Event::Empty(ref e) => {
           match e.local_name() {
             Info::TAG_BYTES if self.resources.is_empty() => self.elems.push(VOTableElem::Info(Info::from_event_empty(e)?)),
             CooSys::TAG_BYTES => self.elems.push(VOTableElem::CooSys(CooSys::from_event_empty(e)?)),
             TimeSys::TAG_BYTES => self.elems.push(VOTableElem::TimeSys(TimeSys::from_event_empty(e)?)),
             Group::TAG_BYTES => self.elems.push(VOTableElem::Group(Group::from_event_empty(e)?)),
             Param::TAG_BYTES => self.elems.push(VOTableElem::Param(Param::from_event_empty(e)?)),
+            Definitions::TAG_BYTES => self.elems.push(VOTableElem::Definitions(Definitions::from_event_empty(e)?)),
             Info::TAG_BYTES => self.post_infos.push(Info::from_event_empty(e)?),
             _ => return Err(VOTableError::UnexpectedEmptyTag(e.local_name().to_vec(), Self::TAG)),
           }
         }
         Event::End(e) if e.local_name() == Self::TAG_BYTES =>
           return if self.resources.is_empty() {
             Err(VOTableError::Custom(String::from("No resource found in the VOTable")))
@@ -718,14 +739,57 @@
     match quick_xml::se::to_string(&votable) {
       Ok(content) => println!("{}", &content),
       Err(error) => println!("{:?}", &error),
     }*/
   }
 
   #[test]
+  fn test_votable_read_with_namespace_file() {
+    let votable = VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/IMCCE.with_namespace.vot");
+    assert!(votable.is_ok())
+  }
+  
+  #[test]
+  fn test_votable_read_obscore_file() {
+    let votable = VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/obscore.vot");
+    assert!(votable.is_ok())
+  }
+
+  #[test]
+  fn test_votable_read_with_cdata() {
+    let votable = VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/vot_with_cdata.vot");
+    assert!(votable.is_ok())
+  }
+  
+  #[test]
+  fn test_votable_read_with_definitions_file() {
+    let votable = VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/vot_with_definitions.vot");
+    assert!(votable.is_ok())
+  }
+
+
+  #[test]
+  fn test_votable_read_with_empty_precision() {
+    let votable = VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/vot_with_empty_prec.vot");
+    assert!(votable.is_ok())
+  }
+  
+  #[test]
+  fn test_votable_read_dataLink_003_file() {
+    match VOTableWrapper::<InMemTableDataRows>::from_ivoa_xml_file("resources/dataLink_003.xml") {
+      Ok(_) => { },
+      Err(e) => {
+        eprintln!("Error: {:?}", e);
+        assert!(false);
+      },
+    }
+    // assert!(votable.is_ok())
+  }
+
+  #[test]
   fn test_votable_read_iter_datatable_from_file() {
     use crate::iter::VOTableIterator;
     
     /*
     println!();
     println!("-- next_table_row_string_iter dss12.vot --");
     println!();
```

### Comparing `votable_cli-0.2.0/Cargo.toml` & `votable_cli-0.2.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "votable-cli"
-version = "0.2.0"
+version = "0.2.3"
 authors = ["F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>"]
 description = "Command-line to convert IVOA VOTables in XML, JSON, YAML and TOML"
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 categories = ["command-line-utilities", "science", "data-structures"]
 keywords = ["ivoa", "votable", "xml", "json", "toml", "yaml"]
 documentation = "https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli"
```

### Comparing `votable_cli-0.2.0/LICENSE-APACHE` & `votable_cli-0.2.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/LICENSE-MIT` & `votable_cli-0.2.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/README.md` & `votable_cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/doc/vot.1.txt.tpl` & `votable_cli-0.2.3/doc/vot.1.txt.tpl`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/pyproject.toml` & `votable_cli-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/src/main.rs` & `votable_cli-0.2.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.2.0/Cargo.lock` & `votable_cli-0.2.3/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "anstream"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "342258dd14006105c2b75ab1bd7543a03bdf0cfc94383303ac212a04939dff6f"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
+ "anstyle-query",
  "anstyle-wincon",
- "concolor-override",
- "concolor-query",
+ "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7d1bb534e9efed14f3e5f44e7dd1a4f709384023a4165199a4241e18dff0116"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
 name = "anstyle-wincon"
-version = "0.2.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3127af6145b149f3287bb9a0d10ad9c5692dba8c53ad48285e5bec4063834fa"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys",
 ]
 
 [[package]]
 name = "autocfg"
@@ -89,28 +98,28 @@
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "clap"
-version = "4.2.1"
+version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046ae530c528f252094e4a77886ee1374437744b2bff1497aa898bbddbbb29b3"
+checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.1"
+version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "223163f58c9a40c3b0a43e1c4b50a9ce09f007ea2cb1ec258a687945b4b7929f"
+checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -130,33 +139,24 @@
 [[package]]
 name = "clap_lex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
-name = "concolor-override"
+name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
-
-[[package]]
-name = "concolor-query"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d11d52c3d7ca2e6d0040212be9e4dbbcd78b6447f535b6b561f449427944cf"
-dependencies = [
- "windows-sys",
-]
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
@@ -201,28 +201,28 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "256017f749ab3117e93acb91063009e1f1bb56d03965b14c2c8df4eb02c524d8"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi",
  "io-lifetimes",
  "rustix",
  "windows-sys",
 ]
 
@@ -230,23 +230,23 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.0"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd550e73688e6d578f0ac2119e32b797a327631a42f9433e59d02e139c8df60d"
+checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -260,17 +260,17 @@
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quick-error"
 version = "2.0.1"
@@ -299,17 +299,17 @@
 name = "radium"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
 
 [[package]]
 name = "rustix"
-version = "0.37.5"
+version = "0.37.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e78cc525325c06b4a7ff02db283472f3c042b7ff0c391f96c6d5ac6f4f91b75"
+checksum = "8bbfc1d1c7c40c01715f47d71444744a81669ca84e8b63e25a55e169b1f86433"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
@@ -319,49 +319,49 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.19"
+version = "0.9.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f82e6c8c047aa50a7328632d067bcae6ef38772a79e28daf32f735e0e4f3dd10"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -370,17 +370,17 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "2.0.11"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21e3787bb71465627110e7d87ed4faaa36c1f61042ee67badb9e2ef173accc40"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -411,27 +411,27 @@
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad2024452afd3874bf539695e04af6732ba06517424dbf958fdb16a01f3bef6c"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "votable"
-version = "0.2.0"
+version = "0.2.3"
 dependencies = [
  "base64",
  "bitvec",
  "byteorder",
  "paste",
  "quick-error",
  "quick-xml",
@@ -440,85 +440,85 @@
  "serde_yaml",
  "toml",
  "ucs2",
 ]
 
 [[package]]
 name = "votable-cli"
-version = "0.2.0"
+version = "0.2.3"
 dependencies = [
  "clap",
  "votable",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
```

### Comparing `votable_cli-0.2.0/PKG-INFO` & `votable_cli-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: votable-cli
-Version: 0.2.0
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 License-File: COPYING
 Summary: Command-line to convert IVOA VOTables in XML, JSON, YAML and TOML
 Keywords: ivoa,votable,xml,json,toml,yaml
 Home-Page: https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli
```

