# Comparing `tmp/async-channel-2.1.0.tar.gz` & `tmp/async-channel-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-channel-2.1.0.tar", last modified: Thu Dec 22 23:15:15 2022, max compression
+gzip compressed data, was "async-channel-2.2.0.tar", last modified: Tue May  2 15:40:28 2023, max compression
```

## Comparing `async-channel-2.1.0.tar` & `async-channel-2.2.0.tar`

### file list

```diff
@@ -1,38 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 23:15:15.402199 async-channel-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2022-12-22 23:14:52.000000 async-channel-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-22 23:14:52.000000 async-channel-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-22 23:14:52.000000 async-channel-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      742 2022-12-22 23:15:15.402199 async-channel-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2022-12-22 23:14:52.000000 async-channel-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 23:15:15.398199 async-channel-2.1.0/async_channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 23:15:15.402199 async-channel-2.1.0/async_channel/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/channel.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/channel_instances.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/channels/channel_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/consumer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/producer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 23:15:15.402199 async-channel-2.1.0/async_channel/util/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/util/channel_creator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/util/channel_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2022-12-22 23:14:52.000000 async-channel-2.1.0/async_channel/util/logging_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 23:15:15.402199 async-channel-2.1.0/async_channel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-22 23:15:15.000000 async-channel-2.1.0/async_channel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-22 23:14:52.000000 async-channel-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 23:15:15.402199 async-channel-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2022-12-22 23:14:52.000000 async-channel-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:28.732794 async-channel-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-05-02 15:39:56.000000 async-channel-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 15:39:56.000000 async-channel-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-02 15:39:56.000000 async-channel-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 15:40:28.728794 async-channel-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-02 15:39:56.000000 async-channel-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:28.728794 async-channel-2.2.0/async_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:28.728794 async-channel-2.2.0/async_channel/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/channels/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/channels/channel_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:28.728794 async-channel-2.2.0/async_channel/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/util/channel_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-02 15:39:56.000000 async-channel-2.2.0/async_channel/util/logging_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:28.728794 async-channel-2.2.0/async_channel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 15:40:28.000000 async-channel-2.2.0/async_channel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 15:40:28.000000 async-channel-2.2.0/async_channel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:40:28.000000 async-channel-2.2.0/async_channel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:40:28.000000 async-channel-2.2.0/async_channel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 15:40:28.000000 async-channel-2.2.0/async_channel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:56.000000 async-channel-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:40:28.732794 async-channel-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 15:39:56.000000 async-channel-2.2.0/setup.py
```

### Comparing `async-channel-2.1.0/CHANGELOG.md` & `async-channel-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.0] - 2023-05-02
+### Updated
+- Supported python versions
+### Removed
+- Cython
+
 ## [2.1.0] - 2022-12-23
 ### Updated
 - [Cython] update to 0.29.32
 
 ## [2.0.14] - 2022-12-22
 ### Added
 - [Channel] get_prioritized_consumers
```

### Comparing `async-channel-2.1.0/LICENSE` & `async-channel-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/README.md` & `async-channel-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Async-Channel [2.1.0](https://github.com/Drakkar-Software/Async-Channel/blob/master/CHANGELOG.md)
+# Async-Channel [2.2.0](https://github.com/Drakkar-Software/Async-Channel/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/523d43c62f1d4de08395752367f5fddc)](https://www.codacy.com/gh/Drakkar-Software/Async-Channel/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Drakkar-Software/Async-Channel&amp;utm_campaign=Badge_Grade)
 [![PyPI](https://img.shields.io/pypi/v/async-channel.svg)](https://pypi.python.org/pypi/async-channel/)
 [![Github-Action-CI](https://github.com/Drakkar-Software/Async-Channel/workflows/Async-Channel-Default-CI/badge.svg)](https://github.com/Drakkar-Software/Async-Channel/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/Async-Channel/status.svg)](https://cloud.drone.io/Drakkar-Software/Async-Channel)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Channels/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Channels?branch=master)
 [![Doc Status](https://readthedocs.org/projects/octobot-channels/badge/?version=stable)](https://octobot-channels.readthedocs.io/en/stable/?badge=stable)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `async-channel-2.1.0/async_channel/__init__.pxd` & `async-channel-2.2.0/async_channel/util/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software Async-Channel
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,26 +9,27 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+"""
+Define Channel helping methods
+"""
+from async_channel.util import channel_creator
+from async_channel.util import logging_util
 
-from async_channel cimport producer
-from async_channel cimport consumer
-
-from async_channel.producer cimport (
-    Producer,
+from async_channel.util.channel_creator import (
+    create_all_subclasses_channel,
+    create_channel_instance,
 )
-from async_channel.consumer cimport (
-    Consumer,
-    InternalConsumer,
-    SupervisedConsumer,
+
+from async_channel.util.logging_util import (
+    get_logger,
 )
 
 __all__ = [
-    "Producer",
-    "Consumer",
-    "InternalConsumer",
-    "SupervisedConsumer",
+    "create_all_subclasses_channel",
+    "create_channel_instance",
+    "get_logger",
 ]
```

### Comparing `async-channel-2.1.0/async_channel/__init__.py` & `async-channel-2.2.0/async_channel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from async_channel.consumer import (
     Consumer,
     InternalConsumer,
     SupervisedConsumer,
 )
 
 PROJECT_NAME = "async-channel"
-VERSION = "2.1.0"  # major.minor.revision
+VERSION = "2.2.0"  # major.minor.revision
 
 __all__ = [
     "CHANNEL_WILDCARD",
     "DEFAULT_QUEUE_SIZE",
     "ChannelConsumerPriorityLevels",
     "Producer",
     "Consumer",
```

### Comparing `async-channel-2.1.0/async_channel/channels/__init__.pxd` & `async-channel-2.2.0/async_channel/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software Async-Channel
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,22 +9,13 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+"""
+Define async_channel global constants
+"""
+CHANNEL_WILDCARD = "*"
 
-from async_channel.channels cimport channel
-from async_channel.channels.channel cimport (
-    Channel
-)
-
-from async_channel.channels cimport channel_instances
-from async_channel.channels.channel_instances cimport (
-    ChannelInstances
-)
-
-__all__ = [
-    "ChannelInstances",
-    "Channel",
-]
+DEFAULT_QUEUE_SIZE = 0  # unlimited
```

### Comparing `async-channel-2.1.0/async_channel/channels/__init__.py` & `async-channel-2.2.0/async_channel/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/channels/channel.py` & `async-channel-2.2.0/async_channel/channels/channel.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/channels/channel_instances.py` & `async-channel-2.2.0/async_channel/channels/channel_instances.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/consumer.py` & `async-channel-2.2.0/async_channel/consumer.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/enums.py` & `async-channel-2.2.0/async_channel/enums.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/producer.py` & `async-channel-2.2.0/async_channel/producer.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel/util/__init__.py` & `async-channel-2.2.0/async_channel/util/logging_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,26 +10,24 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 """
-Define Channel helping methods
+Define async_channel logger implementation
 """
-from async_channel.util import channel_creator
-from async_channel.util import logging_util
+import logging
 
-from async_channel.util.channel_creator import (
-    create_all_subclasses_channel,
-    create_channel_instance,
-)
 
-from async_channel.util.logging_util import (
-    get_logger,
-)
+# pylint: disable=no-member, import-outside-toplevel
+def get_logger(name: str = "") -> logging.Logger:
+    """
+    :param name: the logger name
+    :return: the logger implementation, can be octobot_commons one or default python logging
+    """
+    try:
+        import octobot_commons.logging as common_logging
 
-__all__ = [
-    "create_all_subclasses_channel",
-    "create_channel_instance",
-    "get_logger",
-]
+        return common_logging.get_logger(logger_name=name)
+    except ImportError:
+        return logging.getLogger(name)
```

### Comparing `async-channel-2.1.0/async_channel/util/channel_creator.py` & `async-channel-2.2.0/async_channel/util/channel_creator.py`

 * *Files identical despite different names*

### Comparing `async-channel-2.1.0/async_channel.egg-info/SOURCES.txt` & `async-channel-2.2.0/async_channel.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-async_channel/__init__.pxd
 async_channel/__init__.py
 async_channel/constants.py
-async_channel/consumer.pxd
 async_channel/consumer.py
 async_channel/enums.py
-async_channel/producer.pxd
 async_channel/producer.py
 async_channel.egg-info/PKG-INFO
 async_channel.egg-info/SOURCES.txt
 async_channel.egg-info/dependency_links.txt
 async_channel.egg-info/not-zip-safe
-async_channel.egg-info/requires.txt
 async_channel.egg-info/top_level.txt
-async_channel/channels/__init__.pxd
 async_channel/channels/__init__.py
-async_channel/channels/channel.pxd
 async_channel/channels/channel.py
-async_channel/channels/channel_instances.pxd
 async_channel/channels/channel_instances.py
-async_channel/util/__init__.pxd
 async_channel/util/__init__.py
-async_channel/util/channel_creator.pxd
 async_channel/util/channel_creator.py
 async_channel/util/logging_util.py
```

### Comparing `async-channel-2.1.0/setup.py` & `async-channel-2.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,76 +10,41 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
-import os
-
-from setuptools import dist
-dist.Distribution().fetch_build_eggs(['Cython>=0.29.32'])
-
-try:
-    from Cython.Distutils import build_ext
-    from Cython.Build import cythonize
-except ImportError:
-    # create closure for deferred import
-    def cythonize(*args, **kwargs):
-        from Cython.Build import cythonize
-        return cythonize(*args, **kwargs)
-
-    def build_ext(*args, **kwargs):
-        from Cython.Distutils import build_ext
-        return build_ext(*args, **kwargs)
-
 from setuptools import find_packages
-from setuptools import setup, Extension
+from setuptools import setup
 
 from async_channel import PROJECT_NAME, VERSION
 
 PACKAGES = find_packages(exclude=["tests"])
 
-packages_list = ["async_channel.consumer",
-                 "async_channel.producer",
-                 "async_channel.channels.channel",
-                 "async_channel.channels.channel_instances",
-                 "async_channel.util.channel_creator"]
-
-ext_modules = [
-    Extension(package, [f"{package.replace('.', '/')}.py"])
-    for package in packages_list]
-
-# long description from README file
-# with open('README.md', encoding='utf-8') as f:
-#     DESCRIPTION = f.read()
 
 REQUIRED = open('requirements.txt').readlines()
 REQUIRES_PYTHON = '>=3.8'
-CYTHON_DEBUG = False if not os.getenv('CYTHON_DEBUG') else os.getenv('CYTHON_DEBUG')
 
 setup(
     name=PROJECT_NAME,
     version=VERSION,
     url='https://github.com/Drakkar-Software/Async-Channel',
     license='LGPL-3.0',
     author='Drakkar-Software',
-    author_email='drakkar-software@protonmail.com',
+    author_email='contact@drakkar.software',
     description='Python channel based communication library',
     packages=PACKAGES,
     include_package_data=True,
-    # long_description=DESCRIPTION,
-    cmdclass={'build_ext': build_ext},
     tests_require=["pytest"],
     test_suite="tests",
     zip_safe=False,
     data_files=[],
-    setup_requires=REQUIRED if not CYTHON_DEBUG else [],
+    setup_requires=REQUIRED,
     install_requires=REQUIRED,
-    ext_modules=cythonize(ext_modules, gdb_debug=CYTHON_DEBUG),
     python_requires=REQUIRES_PYTHON,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
```

