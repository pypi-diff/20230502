# Comparing `tmp/uform-0.2.0.tar.gz` & `tmp/uform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uform-0.2.0.tar", last modified: Wed Mar 29 14:55:46 2023, max compression
+gzip compressed data, was "uform-0.2.1.tar", last modified: Tue May  2 17:53:08 2023, max compression
```

## Comparing `uform-0.2.0.tar` & `uform-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:55:46.485517 uform-0.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11356 2023-03-29 14:55:34.000000 uform-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-03-29 14:55:46.485517 uform-0.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7498 2023-03-29 14:55:34.000000 uform-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-03-29 14:55:34.000000 uform-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 14:55:46.485517 uform-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:55:46.485517 uform-0.2.0/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:55:34.000000 uform-0.2.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:55:46.485517 uform-0.2.0/src/uform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-03-29 14:55:46.000000 uform-0.2.0/src/uform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-29 14:55:46.000000 uform-0.2.0/src/uform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:55:46.000000 uform-0.2.0/src/uform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-29 14:55:46.000000 uform-0.2.0/src/uform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-29 14:55:46.000000 uform-0.2.0/src/uform.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14611 2023-03-29 14:55:34.000000 uform-0.2.0/src/uform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:53:08.767225 uform-0.2.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11356 2023-05-02 17:52:57.000000 uform-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-02 17:53:08.767225 uform-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7482 2023-05-02 17:52:57.000000 uform-0.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-05-02 17:52:57.000000 uform-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:53:08.767225 uform-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:53:08.763225 uform-0.2.1/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:52:57.000000 uform-0.2.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:53:08.767225 uform-0.2.1/src/uform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-02 17:53:08.000000 uform-0.2.1/src/uform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-02 17:53:08.000000 uform-0.2.1/src/uform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:53:08.000000 uform-0.2.1/src/uform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 17:53:08.000000 uform-0.2.1/src/uform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 17:53:08.000000 uform-0.2.1/src/uform.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14611 2023-05-02 17:52:57.000000 uform-0.2.1/src/uform.py
```

### Comparing `uform-0.2.0/LICENSE` & `uform-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uform-0.2.0/PKG-INFO` & `uform-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,24 @@
-Metadata-Version: 2.1
-Name: uform
-Version: 0.2.0
-Summary: Efficient Multi-Modal Semantic Search Models by Unum
-Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
-Maintainer-email: unum <info@unum.cloud>
-Project-URL: Homepage, https://github.com/unum-cloud/uform
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: remote
-License-File: LICENSE
-
-<h1 align="center">Unified Form</h1>
+<h1 align="center">UForm</h1>
 <h3 align="center">
-Multi-Modal Inference Library<br/>
+Multi-Modal Transformers Library<br/>
 For Semantic Search Applications<br/>
 </h3>
 <br/>
 
 <p align="center">
-<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/discord.svg" alt="Discord"></a>
+<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/discord.svg" alt="Discord"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/linkedin.svg" alt="LinkedIn"></a>
+<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/linkedin.svg" alt="LinkedIn"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/twitter.svg" alt="Twitter"></a>
+<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/twitter.svg" alt="Twitter"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/blog.svg" alt="Blog"></a>
+<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/blog.svg" alt="Blog"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/github.svg" alt="GitHub"></a>
+<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
 </p>
 
 ---
 
 UForm is a Multi-Modal Modal Inference package, designed to encode Multi-Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared vector space!
 It comes with a set of homonymous pre-trained networks available on [HuggingFace portal](https://huggingface.co/unum-cloud/uform) and extends the `transfromers` package to support Mid-fusion Models.
 
@@ -109,15 +92,15 @@
     attention_mask=text_data['attention_mask']
 )
 ```
 
 ### Remote Procedure Calls for Cloud Deployments
 
 You can also use our larger, faster, better proprietary models deployed in optimized cloud environments.
-For that, please, choose the cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm with optional dependencies:
+For that, please, choose the cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm with optional dependencies:
 
 ```bash
 pip install uform[remote]
 ```
 
 The only thing that changes after that is calling `get_client` with the IP address of your instance instead of using `get_model` for local usage.
```

#### html2text {}

```diff
@@ -1,19 +1,9 @@
-Metadata-Version: 2.1 Name: uform Version: 0.2.0 Summary: Efficient Multi-Modal
-Semantic Search Models by Unum Author-email: Mikhail Kim
-kim@unum.cloud>, Vladimir Orshulevich
-orshulevich@unum.cloud> Maintainer-email: unum
-unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
-Classifier: Programming Language :: Python :: 3 Classifier: Development Status
-:: 4 - Beta Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: remote License-File: LICENSE
-                          ****** Unified Form ******
-                      **** Multi-Modal Inference Library
+                              ****** UForm ******
+                     **** Multi-Modal Transformers Library
                        For Semantic Search Applications
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
 --- UForm is a Multi-Modal Modal Inference package, designed to encode Multi-
 Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared
 vector space! It comes with a set of homonymous pre-trained networks available
@@ -48,15 +38,15 @@
 (text_data, return_features=True) ``` These features can later be used to
 produce joint multimodal encodings faster, as the first layers of the
 transformer can be skipped: ```python joint_embedding = model.encode_multimodal
 ( image_features=image_features, text_features=text_features,
 attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
 Cloud Deployments You can also use our larger, faster, better proprietary
 models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm
+cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
 with optional dependencies: ```bash pip install uform[remote] ``` The only
 thing that changes after that is calling `get_client` with the IP address of
 your instance instead of using `get_model` for local usage. ```python model =
 uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
 calculate semantic compatibility between an image and a text: [Cosine
 Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
 Cosine Similarity ```python import torch.nn.functional as F similarity =
```

### Comparing `uform-0.2.0/README.md` & `uform-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,54 @@
-<h1 align="center">Unified Form</h1>
+Metadata-Version: 2.1
+Name: uform
+Version: 0.2.1
+Summary: Multi-Modal Transformers library for Semantic Search and other Vision-Language tasks
+Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
+Maintainer-email: unum <info@unum.cloud>
+Project-URL: Homepage, https://github.com/unum-cloud/uform
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Natural Language :: English
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Korean
+Classifier: Natural Language :: German
+Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Polish
+Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Japanese
+Classifier: Natural Language :: Russian
+Classifier: Natural Language :: Turkish
+Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: remote
+License-File: LICENSE
+
+<h1 align="center">UForm</h1>
 <h3 align="center">
-Multi-Modal Inference Library<br/>
+Multi-Modal Transformers Library<br/>
 For Semantic Search Applications<br/>
 </h3>
 <br/>
 
 <p align="center">
-<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/discord.svg" alt="Discord"></a>
+<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/discord.svg" alt="Discord"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/linkedin.svg" alt="LinkedIn"></a>
+<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/linkedin.svg" alt="LinkedIn"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/twitter.svg" alt="Twitter"></a>
+<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/twitter.svg" alt="Twitter"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/blog.svg" alt="Blog"></a>
+<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/blog.svg" alt="Blog"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/github.svg" alt="GitHub"></a>
+<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
 </p>
 
 ---
 
 UForm is a Multi-Modal Modal Inference package, designed to encode Multi-Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared vector space!
 It comes with a set of homonymous pre-trained networks available on [HuggingFace portal](https://huggingface.co/unum-cloud/uform) and extends the `transfromers` package to support Mid-fusion Models.
 
@@ -92,15 +122,15 @@
     attention_mask=text_data['attention_mask']
 )
 ```
 
 ### Remote Procedure Calls for Cloud Deployments
 
 You can also use our larger, faster, better proprietary models deployed in optimized cloud environments.
-For that, please, choose the cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm with optional dependencies:
+For that, please, choose the cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm with optional dependencies:
 
 ```bash
 pip install uform[remote]
 ```
 
 The only thing that changes after that is calling `get_client` with the IP address of your instance instead of using `get_model` for local usage.
```

#### html2text {}

```diff
@@ -1,9 +1,28 @@
-                          ****** Unified Form ******
-                      **** Multi-Modal Inference Library
+Metadata-Version: 2.1 Name: uform Version: 0.2.1 Summary: Multi-Modal
+Transformers library for Semantic Search and other Vision-Language tasks
+Author-email: Mikhail Kim
+kim@unum.cloud>, Vladimir Orshulevich
+orshulevich@unum.cloud> Maintainer-email: unum
+unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
+Classifier: Programming Language :: Python :: 3 Classifier: Development Status
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
+Engineering :: Image Recognition Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Natural Language :: Korean
+Classifier: Natural Language :: German Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Polish Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Japanese Classifier: Natural Language ::
+Russian Classifier: Natural Language :: Turkish Classifier: Natural Language ::
+Chinese (Simplified) Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: remote License-File: LICENSE
+                              ****** UForm ******
+                     **** Multi-Modal Transformers Library
                        For Semantic Search Applications
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
 --- UForm is a Multi-Modal Modal Inference package, designed to encode Multi-
 Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared
 vector space! It comes with a set of homonymous pre-trained networks available
@@ -38,15 +57,15 @@
 (text_data, return_features=True) ``` These features can later be used to
 produce joint multimodal encodings faster, as the first layers of the
 transformer can be skipped: ```python joint_embedding = model.encode_multimodal
 ( image_features=image_features, text_features=text_features,
 attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
 Cloud Deployments You can also use our larger, faster, better proprietary
 models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm
+cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
 with optional dependencies: ```bash pip install uform[remote] ``` The only
 thing that changes after that is calling `get_client` with the IP address of
 your instance instead of using `get_model` for local usage. ```python model =
 uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
 calculate semantic compatibility between an image and a text: [Cosine
 Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
 Cosine Similarity ```python import torch.nn.functional as F similarity =
```

### Comparing `uform-0.2.0/src/uform.egg-info/PKG-INFO` & `uform-0.2.1/src/uform.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 0.2.0
-Summary: Efficient Multi-Modal Semantic Search Models by Unum
+Version: 0.2.1
+Summary: Multi-Modal Transformers library for Semantic Search and other Vision-Language tasks
 Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
 Maintainer-email: unum <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Natural Language :: English
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Korean
+Classifier: Natural Language :: German
+Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Polish
+Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Japanese
+Classifier: Natural Language :: Russian
+Classifier: Natural Language :: Turkish
+Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: remote
 License-File: LICENSE
 
-<h1 align="center">Unified Form</h1>
+<h1 align="center">UForm</h1>
 <h3 align="center">
-Multi-Modal Inference Library<br/>
+Multi-Modal Transformers Library<br/>
 For Semantic Search Applications<br/>
 </h3>
 <br/>
 
 <p align="center">
-<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/discord.svg" alt="Discord"></a>
+<a href="https://discord.gg/jsMURnSFM2"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/discord.svg" alt="Discord"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/linkedin.svg" alt="LinkedIn"></a>
+<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/linkedin.svg" alt="LinkedIn"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/twitter.svg" alt="Twitter"></a>
+<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/twitter.svg" alt="Twitter"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/blog.svg" alt="Blog"></a>
+<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/blog.svg" alt="Blog"></a>
 &nbsp;&nbsp;&nbsp;
-<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/github.svg" alt="GitHub"></a>
+<a href="https://github.com/unum-cloud/uform"><img height="25" src="https://github.com/unum-cloud/.github/raw/main/assets/github.svg" alt="GitHub"></a>
 </p>
 
 ---
 
 UForm is a Multi-Modal Modal Inference package, designed to encode Multi-Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared vector space!
 It comes with a set of homonymous pre-trained networks available on [HuggingFace portal](https://huggingface.co/unum-cloud/uform) and extends the `transfromers` package to support Mid-fusion Models.
 
@@ -109,15 +122,15 @@
     attention_mask=text_data['attention_mask']
 )
 ```
 
 ### Remote Procedure Calls for Cloud Deployments
 
 You can also use our larger, faster, better proprietary models deployed in optimized cloud environments.
-For that, please, choose the cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm with optional dependencies:
+For that, please, choose the cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm with optional dependencies:
 
 ```bash
 pip install uform[remote]
 ```
 
 The only thing that changes after that is calling `get_client` with the IP address of your instance instead of using `get_model` for local usage.
```

#### html2text {}

```diff
@@ -1,19 +1,28 @@
-Metadata-Version: 2.1 Name: uform Version: 0.2.0 Summary: Efficient Multi-Modal
-Semantic Search Models by Unum Author-email: Mikhail Kim
+Metadata-Version: 2.1 Name: uform Version: 0.2.1 Summary: Multi-Modal
+Transformers library for Semantic Search and other Vision-Language tasks
+Author-email: Mikhail Kim
 kim@unum.cloud>, Vladimir Orshulevich
 orshulevich@unum.cloud> Maintainer-email: unum
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
-:: 4 - Beta Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: remote License-File: LICENSE
-                          ****** Unified Form ******
-                      **** Multi-Modal Inference Library
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
+Engineering :: Image Recognition Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Natural Language :: Korean
+Classifier: Natural Language :: German Classifier: Natural Language :: Italian
+Classifier: Natural Language :: Polish Classifier: Natural Language :: Spanish
+Classifier: Natural Language :: Japanese Classifier: Natural Language ::
+Russian Classifier: Natural Language :: Turkish Classifier: Natural Language ::
+Chinese (Simplified) Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: remote License-File: LICENSE
+                              ****** UForm ******
+                     **** Multi-Modal Transformers Library
                        For Semantic Search Applications
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
 --- UForm is a Multi-Modal Modal Inference package, designed to encode Multi-
 Lingual Texts, Images, and, soon, Audio, Video, and Documents, into a shared
 vector space! It comes with a set of homonymous pre-trained networks available
@@ -48,15 +57,15 @@
 (text_data, return_features=True) ``` These features can later be used to
 produce joint multimodal encodings faster, as the first layers of the
 transformer can be skipped: ```python joint_embedding = model.encode_multimodal
 ( image_features=image_features, text_features=text_features,
 attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
 Cloud Deployments You can also use our larger, faster, better proprietary
 models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UniForm" and reinstall UForm
+cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
 with optional dependencies: ```bash pip install uform[remote] ``` The only
 thing that changes after that is calling `get_client` with the IP address of
 your instance instead of using `get_model` for local usage. ```python model =
 uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
 calculate semantic compatibility between an image and a text: [Cosine
 Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
 Cosine Similarity ```python import torch.nn.functional as F similarity =
```

### Comparing `uform-0.2.0/src/uform.py` & `uform-0.2.1/src/uform.py`

 * *Files identical despite different names*

