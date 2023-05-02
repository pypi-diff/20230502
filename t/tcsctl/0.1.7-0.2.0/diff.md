# Comparing `tmp/tcsctl-0.1.7.tar.gz` & `tmp/tcsctl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcsctl-0.1.7.tar", last modified: Sat Apr 29 21:00:29 2023, max compression
+gzip compressed data, was "tcsctl-0.2.0.tar", last modified: Tue May  2 07:39:21 2023, max compression
```

## Comparing `tcsctl-0.1.7.tar` & `tcsctl-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.162590 tcsctl-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.158590 tcsctl-0.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.158590 tcsctl-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.github/workflows/check-python-syntax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.github/workflows/check-yaml-syntax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-29 21:00:01.000000 tcsctl-0.1.7/.github/workflows/test-python-setup.yml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 21:00:29.000000 tcsctl-0.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 21:00:29.000000 tcsctl-0.1.7/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 21:00:01.000000 tcsctl-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-29 21:00:29.162590 tcsctl-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-29 21:00:01.000000 tcsctl-0.1.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    32257 2023-04-29 21:00:01.000000 tcsctl-0.1.7/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 21:00:01.000000 tcsctl-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-29 21:00:29.162590 tcsctl-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-29 21:00:01.000000 tcsctl-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcs.yaml.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.158590 tcsctl-0.1.7/tcsctl/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28651 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.162590 tcsctl-0.1.7/tcsctl/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/schema.blueprint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/schema.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/schema.environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/schema.flow.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/schemas/schema.template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-29 21:00:01.000000 tcsctl-0.1.7/tcsctl/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:00:29.158590 tcsctl-0.1.7/tcsctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 21:00:29.000000 tcsctl-0.1.7/tcsctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.753518 tcsctl-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.741518 tcsctl-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.741518 tcsctl-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.github/workflows/check-python-syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.github/workflows/check-yaml-syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 07:38:43.000000 tcsctl-0.2.0/.github/workflows/test-python-setup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 07:39:21.000000 tcsctl-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 07:39:21.000000 tcsctl-0.2.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 07:38:43.000000 tcsctl-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 07:39:21.753518 tcsctl-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-02 07:38:43.000000 tcsctl-0.2.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    32644 2023-05-02 07:38:43.000000 tcsctl-0.2.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 07:38:43.000000 tcsctl-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 07:39:21.757518 tcsctl-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 07:38:43.000000 tcsctl-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcs.yaml.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.749518 tcsctl-0.2.0/tcsctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.753518 tcsctl-0.2.0/tcsctl/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/schemas/schema.blueprint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/schemas/schema.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/schemas/schema.environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/schemas/schema.template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 07:38:43.000000 tcsctl-0.2.0/tcsctl/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:39:21.753518 tcsctl-0.2.0/tcsctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 07:39:21.000000 tcsctl-0.2.0/tcsctl.egg-info/top_level.txt
```

### Comparing `tcsctl-0.1.7/.github/workflows/check-yaml-syntax.yml` & `tcsctl-0.2.0/.github/workflows/check-yaml-syntax.yml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/.github/workflows/publish.yml` & `tcsctl-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/.github/workflows/test-python-setup.yml` & `tcsctl-0.2.0/.github/workflows/test-python-setup.yml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/LICENSE` & `tcsctl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/PKG-INFO` & `tcsctl-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsctl
-Version: 0.1.7
+Version: 0.2.0
 Summary: CLI for The Cloudsphere
 Home-page: https://github.com/thecloudsphere/tcsctl
 Author: OSISM GmbH
 Author-email: info@osism.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `tcsctl-0.1.7/Pipfile.lock` & `tcsctl-0.2.0/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9720052083333334%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'50ee1c91ec5e035a2ba5e2fd71c5821bd93d4deb4ddc58fe5b5d122c8ab4ca1f'}}",*

 * * "'default'": "{'rich': {'hashes': "*

 * *              "['sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c', "*

 * *              "'sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704'], "*

 * *              "'version': '==13.3.5'}, 'typer': {'hashes': "*

 * *              "['sha256:50922fd79aea2f4751a8e0408ff10d2662bd0c8bbfa84755a699f3bada2978b2', "*

 * *              "' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4ae8c38038189a9bef5e8ce1f4803beb73a6e622b88626870d645b8800cc9893"
+            "sha256": "50ee1c91ec5e035a2ba5e2fd71c5821bd93d4deb4ddc58fe5b5d122c8ab4ca1f"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -124,21 +124,14 @@
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "version": "==0.4.6"
         },
-        "commonmark": {
-            "hashes": [
-                "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
-                "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
-            ],
-            "version": "==0.9.1"
-        },
         "dynaconf": {
             "hashes": [
                 "sha256:11a60bcd735f82b8a47b288f99e4ffbbd08c6c130a7be93c5d03e93fc260a5e1",
                 "sha256:a79d7b3ad4a35af9b576c49f11cd3b23a1b04b87b63a4e9f92cc82f2b0cafeeb"
             ],
             "index": "pypi",
             "version": "==3.1.12"
@@ -163,14 +156,22 @@
             "hashes": [
                 "sha256:1612053ced6ae84d7959dd7d5e431a0532642237ec21f7fd83ac73fe539e03e1",
                 "sha256:b93aa30099fa6860d4727f1b81f8718e965bb96253fa190fab2077aaad6d15d3"
             ],
             "index": "pypi",
             "version": "==0.7.0"
         },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.0"
+        },
         "markupsafe": {
             "hashes": [
                 "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
                 "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
                 "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
                 "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
                 "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
@@ -219,14 +220,22 @@
                 "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
                 "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
                 "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.1.2"
         },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
         "numpy": {
             "hashes": [
                 "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187",
                 "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812",
                 "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7",
                 "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4",
                 "sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6",
@@ -421,18 +430,18 @@
                 "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
             ],
             "index": "pypi",
             "version": "==2.29.0"
         },
         "rich": {
             "hashes": [
-                "sha256:a4eb26484f2c82589bd9a17c73d32a010b1e29d89f1604cd9bf3a2097b81bb5e",
-                "sha256:ba3a3775974105c221d31141f2c116f4fd65c5ceb0698657a11e9f295ec93fd0"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
-            "version": "==12.6.0"
+            "version": "==13.3.5"
         },
         "shellingham": {
             "hashes": [
                 "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
                 "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
             ],
             "version": "==1.5.0.post1"
@@ -454,19 +463,19 @@
             "version": "==0.9.0"
         },
         "typer": {
             "extras": [
                 "all"
             ],
             "hashes": [
-                "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d",
-                "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"
+                "sha256:50922fd79aea2f4751a8e0408ff10d2662bd0c8bbfa84755a699f3bada2978b2",
+                "sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee"
             ],
             "index": "pypi",
-            "version": "==0.7.0"
+            "version": "==0.9.0"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `tcsctl-0.1.7/README.md` & `tcsctl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/setup.cfg` & `tcsctl-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/__init__.py` & `tcsctl-0.2.0/tcsctl/__init__.py`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/blueprint.py` & `tcsctl-0.2.0/tcsctl/blueprint.py`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/client.py` & `tcsctl-0.2.0/tcsctl/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,68 +471,14 @@
         data = environment.dict()
         if repository_key:
             data["repository_key"] = repository_key
         result = self.client.post(f"environments/{project_id}", data=data)
         environment = Environment(**result.data)
         return environment
 
-    # flows
-
-    def get_flow_id(self, flow: str, project: str = None) -> uuid_pkg.UUID:
-        if is_valid_uuid(flow):
-            return flow
-
-        project_id = self.get_project_id(self.organisation_id, project)
-
-        result = self.client.get(f"flows/{project_id}", ep_params={"q": flow})
-        flow = Template(**result.data[0])
-        return flow.id
-
-    def delete_flow(self, flow: str, project: str) -> Result:
-        project_id = self.get_project_id(self.organisation_id, project)
-        flow_id = self.get_flow_id(flow, project_id)
-        result = self.client.delete(f"flows/{project_id}/{flow_id}")
-        return result
-
-    def get_flow(self, flow: str, project: str) -> Flow:
-        project_id = self.get_project_id(self.organisation_id, project)
-        flow_id = self.get_flow_id(flow, project_id)
-        result = self.client.get(f"flows/{project_id}/{flow_id}")
-        flow = Flow(**result.data)
-        return flow
-
-    def get_flows(self, project: str) -> Flow:
-        project_id = self.get_project_id(self.organisation_id, project)
-        result = self.client.get(f"flows/{project_id}")
-        flows = [Flow(**flow) for flow in result.data]
-        return flows
-
-    def import_flow(self, path: str, name: str, project: str) -> Flow:
-        project_id = self.get_project_id(self.organisation_id, project)
-
-        logger.debug(f"Validating flow {path}")
-        try:
-            with open(path) as fp:
-                validate_content(fp.read(), "flow")
-        except Exception as e:
-            raise TimonException(f"Flow {path} is not valid:\n{e}")
-
-        with open(path) as fp:
-            data = yaml.safe_load(fp)
-
-        if name not in data:
-            raise TimonException(f"Flow {name} not found in {path}")
-
-        flow_data = data[name]
-        flow_data["steps"] = yaml.dump(flow_data["steps"])
-
-        result = self.client.post(f"flows/{project_id}", data=flow_data)
-        flow = Flow(**result.data)
-        return flow
-
     # templates
 
     def get_template_id(self, template: str, project: str = None) -> uuid_pkg.UUID:
         if is_valid_uuid(template):
             return template
 
         project_id = self.get_project_id(self.organisation_id, project)
```

### Comparing `tcsctl-0.1.7/tcsctl/common.py` & `tcsctl-0.2.0/tcsctl/common.py`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/deployment.py` & `tcsctl-0.2.0/tcsctl/deployment.py`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/enums.py` & `tcsctl-0.2.0/tcsctl/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     destroy = "DESTROY"
     none = "NONE"
     reconcile = "RECONCILE"
 
 
 @unique
 class DeploymentType(str, Enum):
-    flow = "FLOW"
     environment = "ENVIRONMENT"
 
 
 @unique
 class DeploymentStatus(str, Enum):
     check = "CHECK"
     create = "CREATE"
@@ -27,28 +26,12 @@
     none = "NONE"
     reconcile = "RECONCILE"
     reconciled = "RECONCILED"
     validate = "VALIDATE"
 
 
 @unique
-class FlowAction(str, Enum):
-    create = "CREATE"
-    destroy = "DESTROY"
-    none = "NONE"
-
-
-@unique
-class FlowStatus(str, Enum):
-    create = "CREATE"
-    created = "CREATED"
-    destroy = "DESTROY"
-    destroyed = "DESTROYED"
-    none = "NONE"
-
-
-@unique
 class Visibility(str, Enum):
     community = "COMMUNITY"
     private = "PRIVATE"
     public = "PUBLIC"
     shared = "SHARED"
```

### Comparing `tcsctl-0.1.7/tcsctl/environment.py` & `tcsctl-0.2.0/tcsctl/environment.py`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/flow.py` & `tcsctl-0.2.0/tcsctl/project.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 from typing import List
 
 from pandas import DataFrame
 from tabulate import tabulate
 import typer
 
 from . import logger
-from .exceptions import TimonApiException, TimonException
+from .exceptions import TimonApiException
 from .models import *
 
-
 app = typer.Typer()
 
 
-@app.command("import")
-def import_flow(ctx: typer.Context, path: str, name: str):
-    try:
-        flow = ctx.obj.client.import_flow(path, name, ctx.obj.project_id)
-        print(tabulate(flow, headers=["Field", "Value"], tablefmt="psql"))
-    except TimonApiException as e:
-        logger.error(str(e))
-    except TimonException as e:
-        print(str(e))
-
-
 @app.command("list")
-def list_flows(
+def list_project(
     ctx: typer.Context,
     column: List[str] = typer.Option(
         default=[],
         help="Specify the column(s) to include, can be repeated to show multiple columns",
     ),
 ):
     try:
-        flows = ctx.obj.client.get_flows(ctx.obj.project_id)
+        projects = ctx.obj.client.get_projects(ctx.obj.organisation_id)
         df = DataFrame(
-            (x.dict().values() for x in flows),
-            columns=Flow.get_field_names(),
+            (x.dict().values() for x in projects),
+            columns=Project.get_field_names(),
         )
         if column:
             result = tabulate(df.filter(items=column), headers=column, tablefmt="psql")
         else:
             result = tabulate(
                 df,
                 headers=df.columns,
@@ -48,32 +36,31 @@
 
         print(result)
     except TimonApiException as e:
         logger.error(str(e))
 
 
 @app.command("show")
-def show_flow(ctx: typer.Context, name: str):
+def show_project(ctx: typer.Context, name: str):
     try:
-        flow = ctx.obj.client.get_flow(name, ctx.obj.project_id)
-        print(tabulate(flow, headers=["Field", "Value"], tablefmt="psql"))
+        project = ctx.obj.client.get_project(name, ctx.obj.organisation_id)
+        print(tabulate(project, headers=["Field", "Value"], tablefmt="psql"))
     except TimonApiException as e:
         logger.error(str(e))
 
 
-@app.command("edit")
-def edit_flow(ctx: typer.Context, name: str):
-    logger.info("STUB: edit_flow")
-
-
-@app.command("update")
-def update_flow(ctx: typer.Context, name: str):
-    logger.info("STUB: update_flow")
+@app.command("create")
+def create_project(ctx: typer.Context, name: str):
+    try:
+        project = ctx.obj.client.create_project(name, ctx.obj.organisation_id)
+        print(tabulate(project, headers=["Field", "Value"], tablefmt="psql"))
+    except TimonApiException as e:
+        logger.error(str(e))
 
 
 @app.command("delete")
-def delete_flow(ctx: typer.Context, name: str):
+def delete_project(ctx: typer.Context, name: str):
     try:
-        ctx.obj.client.delete_flow(name, ctx.obj.project_id)
-        logger.info(f"Flow {name} deleted")
+        ctx.obj.client.delete_project(name, ctx.obj.organisation_id)
+        logger.info(f"Project {name} deleted")
     except TimonApiException as e:
         logger.error(str(e))
```

### Comparing `tcsctl-0.1.7/tcsctl/main.py` & `tcsctl-0.2.0/tcsctl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 from .deployment import app as app_deployment
 from .environment import app as app_environment
 from .exceptions import (
     TimonApiException,
     TimonLoginRequiredException,
     TimonTokenExpiredException,
 )
-from .flow import app as app_flow
 from .project import app as app_project
 from .schemas import validate_content
 from .template import app as app_template
 
 
 app = typer.Typer()
 app.add_typer(app_blueprint, name="blueprint")
 app.add_typer(app_deployment, name="deployment")
 app.add_typer(app_environment, name="environment")
-app.add_typer(app_flow, name="flow")
 app.add_typer(app_project, name="project")
 app.add_typer(app_template, name="template")
 
 
 @app.command()
 def login(
     ctx: typer.Context,
```

### Comparing `tcsctl-0.1.7/tcsctl/models.py` & `tcsctl-0.2.0/tcsctl/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 from pydantic import BaseModel, Json
 
 from .enums import (
     DeploymentAction,
     DeploymentStatus,
     DeploymentType,
-    FlowAction,
-    FlowStatus,
 )
 
 
 class Result(BaseModel):
     status_code: int
     headers: Dict
     message: str = ""
@@ -136,30 +134,14 @@
     pass
 
 
 class TemplateWithInputs(TimonBaseModel, TemplateWithInputsBase):
     pass
 
 
-# flow
-
-
-class FlowBase(BaseModel):
-    name: Optional[str]
-
-
-class Flow(TimonBaseModel, FlowBase):
-    action: Optional[FlowAction] = FlowAction.none
-    status: Optional[FlowStatus] = FlowStatus.none
-
-
-class FlowWithSteps(Flow):
-    steps: Optional[str]
-
-
 # other
 
 
 class Token(BaseModel):
     access_token: str
     expires_in: int
     issue_timestamp: int
```

### Comparing `tcsctl-0.1.7/tcsctl/project.py` & `tcsctl-0.2.0/tcsctl/template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from typing import List
 
 from pandas import DataFrame
 from tabulate import tabulate
 import typer
 
 from . import logger
-from .exceptions import TimonApiException
+from .exceptions import TimonApiException, TimonException
 from .models import *
 
+
 app = typer.Typer()
 
 
+@app.command("import")
+def import_template(ctx: typer.Context, path: str, name: str):
+    try:
+        template = ctx.obj.client.import_template(path, name, ctx.obj.project_id)
+        print(tabulate(template, headers=["Field", "Value"], tablefmt="psql"))
+    except TimonApiException as e:
+        logger.error(str(e))
+    except TimonException as e:
+        print(str(e))
+
+
 @app.command("list")
-def list_project(
+def list_templates(
     ctx: typer.Context,
     column: List[str] = typer.Option(
         default=[],
         help="Specify the column(s) to include, can be repeated to show multiple columns",
     ),
 ):
     try:
-        projects = ctx.obj.client.get_projects(ctx.obj.organisation_id)
+        templates = ctx.obj.client.get_templates(ctx.obj.project_id)
         df = DataFrame(
-            (x.dict().values() for x in projects),
-            columns=Project.get_field_names(),
+            (x.dict().values() for x in templates),
+            columns=Template.get_field_names(),
         )
         if column:
             result = tabulate(df.filter(items=column), headers=column, tablefmt="psql")
         else:
             result = tabulate(
                 df,
                 headers=df.columns,
@@ -36,31 +48,32 @@
 
         print(result)
     except TimonApiException as e:
         logger.error(str(e))
 
 
 @app.command("show")
-def show_project(ctx: typer.Context, name: str):
+def show_template(ctx: typer.Context, name: str):
     try:
-        project = ctx.obj.client.get_project(name, ctx.obj.organisation_id)
-        print(tabulate(project, headers=["Field", "Value"], tablefmt="psql"))
+        template = ctx.obj.client.get_template(name, ctx.obj.project_id)
+        print(tabulate(template, headers=["Field", "Value"], tablefmt="psql"))
     except TimonApiException as e:
         logger.error(str(e))
 
 
-@app.command("create")
-def create_project(ctx: typer.Context, name: str):
-    try:
-        project = ctx.obj.client.create_project(name, ctx.obj.organisation_id)
-        print(tabulate(project, headers=["Field", "Value"], tablefmt="psql"))
-    except TimonApiException as e:
-        logger.error(str(e))
+@app.command("edit")
+def edit_template(ctx: typer.Context, name: str):
+    logger.info("STUB: edit_template")
+
+
+@app.command("update")
+def update_template(ctx: typer.Context, name: str):
+    logger.info("STUB: update_template")
 
 
 @app.command("delete")
-def delete_project(ctx: typer.Context, name: str):
+def delete_template(ctx: typer.Context, name: str):
     try:
-        ctx.obj.client.delete_project(name, ctx.obj.organisation_id)
-        logger.info(f"Project {name} deleted")
+        ctx.obj.client.delete_template(name, ctx.obj.project_id)
+        logger.info(f"Template {name} deleted")
     except TimonApiException as e:
         logger.error(str(e))
```

### Comparing `tcsctl-0.1.7/tcsctl/schemas/schema.blueprint.yaml` & `tcsctl-0.2.0/tcsctl/schemas/schema.blueprint.yaml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/schemas/schema.environment.yaml` & `tcsctl-0.2.0/tcsctl/schemas/schema.environment.yaml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl/schemas/schema.template.yaml` & `tcsctl-0.2.0/tcsctl/schemas/schema.template.yaml`

 * *Files identical despite different names*

### Comparing `tcsctl-0.1.7/tcsctl.egg-info/PKG-INFO` & `tcsctl-0.2.0/tcsctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsctl
-Version: 0.1.7
+Version: 0.2.0
 Summary: CLI for The Cloudsphere
 Home-page: https://github.com/thecloudsphere/tcsctl
 Author: OSISM GmbH
 Author-email: info@osism.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `tcsctl-0.1.7/tcsctl.egg-info/SOURCES.txt` & `tcsctl-0.2.0/tcsctl.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 tcsctl/blueprint.py
 tcsctl/client.py
 tcsctl/common.py
 tcsctl/deployment.py
 tcsctl/enums.py
 tcsctl/environment.py
 tcsctl/exceptions.py
-tcsctl/flow.py
 tcsctl/main.py
 tcsctl/models.py
 tcsctl/project.py
 tcsctl/template.py
 tcsctl.egg-info/PKG-INFO
 tcsctl.egg-info/SOURCES.txt
 tcsctl.egg-info/dependency_links.txt
@@ -34,9 +33,8 @@
 tcsctl.egg-info/pbr.json
 tcsctl.egg-info/requires.txt
 tcsctl.egg-info/top_level.txt
 tcsctl/schemas/__init__.py
 tcsctl/schemas/schema.blueprint.yaml
 tcsctl/schemas/schema.config.yaml
 tcsctl/schemas/schema.environment.yaml
-tcsctl/schemas/schema.flow.yaml
 tcsctl/schemas/schema.template.yaml
```

