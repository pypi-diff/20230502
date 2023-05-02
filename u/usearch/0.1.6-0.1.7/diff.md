# Comparing `tmp/usearch-0.1.6-cp39-cp39-manylinux_2_24_x86_64.manylinux_2_28_x86_64.whl.zip` & `tmp/usearch-0.1.7-cp39-cp39-manylinux_2_24_x86_64.manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 119391 bytes, number of entries: 7
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-02 07:58 usearch./
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-02 07:58 usearch-0.1.6.dist-info/
--rwxr-xr-x  2.0 unx   305224 b- defN 23-May-02 07:58 usearch.cpython-39-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      400 b- defN 23-May-02 07:58 usearch-0.1.6.dist-info/RECORD
--rw-r--r--  2.0 unx     3585 b- defN 23-May-02 07:58 usearch-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx        8 b- defN 23-May-02 07:58 usearch-0.1.6.dist-info/top_level.txt
--rw-r--r--  2.0 unx      149 b- defN 23-May-02 07:58 usearch-0.1.6.dist-info/WHEEL
-7 files, 309366 bytes uncompressed, 118439 bytes compressed:  61.7%
+Zip file size: 119475 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-02 17:19 usearch-0.1.7.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-02 17:19 usearch./
+-rwxr-xr-x  2.0 unx   305224 b- defN 23-May-02 17:19 usearch.cpython-39-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      400 b- defN 23-May-02 17:19 usearch-0.1.7.dist-info/RECORD
+-rw-r--r--  2.0 unx     3833 b- defN 23-May-02 17:19 usearch-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx        8 b- defN 23-May-02 17:19 usearch-0.1.7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      149 b- defN 23-May-02 17:19 usearch-0.1.7.dist-info/WHEEL
+7 files, 309614 bytes uncompressed, 118523 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: usearch./
+Filename: usearch-0.1.7.dist-info/
 Comment: 
 
-Filename: usearch-0.1.6.dist-info/
+Filename: usearch./
 Comment: 
 
 Filename: usearch.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: usearch-0.1.6.dist-info/RECORD
+Filename: usearch-0.1.7.dist-info/RECORD
 Comment: 
 
-Filename: usearch-0.1.6.dist-info/METADATA
+Filename: usearch-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.1.6.dist-info/top_level.txt
+Filename: usearch-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.1.6.dist-info/WHEEL
+Filename: usearch-0.1.7.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## Comparing `usearch-0.1.6.dist-info/METADATA` & `usearch-0.1.7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Mighty Tiny Vector Search Engine with Automatic Quantization and Hardware Acceleration
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,17 +46,19 @@
   - [x] Euclidean, Dot-product, Cosine,
   - [x] Jaccard, Hamming, Haversine.
   - [x] Hardware-accelerated [`ashvardanian/simsimd`](https://github.com/ashvardanian/simsimd). 
 - [x] Variable dimensionality vectors.
 - [x] Don't copy vectors if not needed.
 - [x] Bring your threads.
 - [x] Multiple vectors per label.
-- [x] Python bindings: `pip install usearch`
-- [x] JavaScript bindings: `npm install usearch`
-- [x] Rust bindings: `cargo add usearch`
+- [x] Python bindings: `pip install usearch`.
+- [x] JavaScript bindings: `npm install usearch`.
+- [x] Rust bindings: `cargo add usearch`.
+- [x] Java bindings: `cloud.unum:usearch` on GitHub.
+- [ ] GoLang bindings.
 - [ ] Wolfram language bindings.
 - [x] For Linux: GCC, Clang.
 - [x] For MacOS: Apple Clang.
 - [ ] For Windows.
 - [ ] Multi-index lookups in Python.
 - [ ] Thread-safe `reserve`.
 - [ ] Distributed construction.
@@ -72,23 +74,29 @@
 
 index_gt<cos_gt<float>> index;
 float vec[3] = {0.1, 0.3, 0.2};
 index.add(/* label: */ 42, /* vector: */ {&vec, 3});
 index.search(
   /* query: */ {&vec, 3}, 10 /* results */,
   /* callback: */ [](std::size_t label, float distance) { });
+
+index.save("index.usearch"); // Serializing to disk
+index.load("index.usearch"); // Reconstructing from disk
+index.view("index.usearch"); // Memory-mapping from disk
 ```
 
 Alternatively fetch it with CMake:
 
 ```cmake
 FetchContent_Declare(usearch GIT_REPOSITORY https://github.com/unum-cloud/usearch.git)
 FetchContent_MakeAvailable(usearch)
 ```
 
+
+
 ## Features
 
 ### Bring your Threads
 
 ## Performance
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 0.1.6 Summary: The Mighty Tiny
+Metadata-Version: 2.1 Name: usearch Version: 0.1.7 Summary: The Mighty Tiny
 Vector Search Engine with Automatic Quantization and Hardware Acceleration
 License: Apache-2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: C++ Classifier:
@@ -21,22 +21,25 @@
 space efficient point-clouds with `uint40_t`. - [x] Half-precision support with
 [`maratyszcza/fp16`](https://github.com/maratyszcza/fp16). - [x] View from
 disk, without loading into RAM. - [x] Any metric, includes: - [x] Euclidean,
 Dot-product, Cosine, - [x] Jaccard, Hamming, Haversine. - [x] Hardware-
 accelerated [`ashvardanian/simsimd`](https://github.com/ashvardanian/simsimd).
 - [x] Variable dimensionality vectors. - [x] Don't copy vectors if not needed.
 - [x] Bring your threads. - [x] Multiple vectors per label. - [x] Python
-bindings: `pip install usearch` - [x] JavaScript bindings: `npm install
-usearch` - [x] Rust bindings: `cargo add usearch` - [ ] Wolfram language
+bindings: `pip install usearch`. - [x] JavaScript bindings: `npm install
+usearch`. - [x] Rust bindings: `cargo add usearch`. - [x] Java bindings:
+`cloud.unum:usearch` on GitHub. - [ ] GoLang bindings. - [ ] Wolfram language
 bindings. - [x] For Linux: GCC, Clang. - [x] For MacOS: Apple Clang. - [ ] For
 Windows. - [ ] Multi-index lookups in Python. - [ ] Thread-safe `reserve`. -
 [ ] Distributed construction. ## Usage ### C++ To use in a C++ project simply
 copy the `include/usearch/usearch.hpp` header into your project. ```c++ using
 namespace unum::usearch; index_gt
 float>> index; float vec[3] = {0.1, 0.3, 0.2}; index.add(/* label: */ 42, /
 * vector: */ {&vec, 3}); index.search( /* query: */ {&vec, 3}, 10 /* results
-*/, /* callback: */ [](std::size_t label, float distance) { }); ```
-Alternatively fetch it with CMake: ```cmake FetchContent_Declare(usearch
-GIT_REPOSITORY https://github.com/unum-cloud/usearch.git)
+*/, /* callback: */ [](std::size_t label, float distance) { }); index.save
+("index.usearch"); // Serializing to disk index.load("index.usearch"); /
+/ Reconstructing from disk index.view("index.usearch"); // Memory-mapping from
+disk ``` Alternatively fetch it with CMake: ```cmake FetchContent_Declare
+(usearch GIT_REPOSITORY https://github.com/unum-cloud/usearch.git)
 FetchContent_MakeAvailable(usearch) ``` ## Features ### Bring your Threads ##
 Performance ## TODO - JavaScript: Allow calling from "worker threads". - Rust:
 Allow passing a custom thread ID.
```

