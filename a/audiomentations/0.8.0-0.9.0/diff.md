# Comparing `tmp/audiomentations-0.8.0.tar.gz` & `tmp/audiomentations-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\audiomentations-0.8.0.tar", last modified: Tue Jan 28 08:18:54 2020, max compression
+gzip compressed data, was "dist\audiomentations-0.9.0.tar", last modified: Thu Feb 20 09:15:53 2020, max compression
```

## Comparing `audiomentations-0.8.0.tar` & `audiomentations-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2020-01-28 08:18:54.000000 audiomentations-0.8.0/
-drwxrwxrwx   0        0        0        0 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations/
-drwxrwxrwx   0        0        0        0 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations/augmentations/
--rw-rw-rw-   0        0        0    12285 2020-01-28 08:14:35.000000 audiomentations-0.8.0/audiomentations/augmentations/transforms.py
--rw-rw-rw-   0        0        0        0 2019-02-12 17:17:51.000000 audiomentations-0.8.0/audiomentations/augmentations/__init__.py
-drwxrwxrwx   0        0        0        0 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations/core/
--rw-rw-rw-   0        0        0      687 2020-01-28 08:14:35.000000 audiomentations-0.8.0/audiomentations/core/composition.py
--rw-rw-rw-   0        0        0      367 2019-03-04 08:07:25.000000 audiomentations-0.8.0/audiomentations/core/transforms_interface.py
--rw-rw-rw-   0        0        0      123 2019-07-25 08:40:12.000000 audiomentations-0.8.0/audiomentations/core/utils.py
--rw-rw-rw-   0        0        0        0 2019-02-12 17:11:06.000000 audiomentations-0.8.0/audiomentations/core/__init__.py
--rw-rw-rw-   0        0        0      141 2020-01-28 08:14:59.000000 audiomentations-0.8.0/audiomentations/__init__.py
-drwxrwxrwx   0        0        0        0 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/
--rw-rw-rw-   0        0        0        1 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3364 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       50 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/requires.txt
--rw-rw-rw-   0        0        0      470 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2020-01-28 08:18:54.000000 audiomentations-0.8.0/audiomentations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3364 2020-01-28 08:18:54.000000 audiomentations-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2223 2019-07-25 08:40:12.000000 audiomentations-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2020-01-28 08:18:54.000000 audiomentations-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1572 2020-01-28 08:14:48.000000 audiomentations-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-02-20 09:15:53.000000 audiomentations-0.9.0/
+drwxrwxrwx   0        0        0        0 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations/
+drwxrwxrwx   0        0        0        0 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations/augmentations/
+-rw-rw-rw-   0        0        0    30889 2020-02-19 15:45:00.000000 audiomentations-0.9.0/audiomentations/augmentations/transforms.py
+-rw-rw-rw-   0        0        0        0 2019-02-12 17:17:51.000000 audiomentations-0.9.0/audiomentations/augmentations/__init__.py
+drwxrwxrwx   0        0        0        0 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations/core/
+-rw-rw-rw-   0        0        0     1279 2020-02-19 09:51:51.000000 audiomentations-0.9.0/audiomentations/core/composition.py
+-rw-rw-rw-   0        0        0     1350 2020-02-19 09:51:32.000000 audiomentations-0.9.0/audiomentations/core/transforms_interface.py
+-rw-rw-rw-   0        0        0      954 2020-02-18 16:16:42.000000 audiomentations-0.9.0/audiomentations/core/utils.py
+-rw-rw-rw-   0        0        0        0 2019-02-12 17:11:06.000000 audiomentations-0.9.0/audiomentations/core/__init__.py
+-rw-rw-rw-   0        0        0      141 2020-02-20 09:11:25.000000 audiomentations-0.9.0/audiomentations/__init__.py
+drwxrwxrwx   0        0        0        0 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3490 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      470 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2020-02-20 09:15:53.000000 audiomentations-0.9.0/audiomentations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3490 2020-02-20 09:15:53.000000 audiomentations-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2223 2019-07-25 08:40:12.000000 audiomentations-0.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2020-02-20 09:15:53.000000 audiomentations-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2020-02-11 15:51:50.000000 audiomentations-0.9.0/setup.py
```

### Comparing `audiomentations-0.8.0/audiomentations.egg-info/PKG-INFO` & `audiomentations-0.9.0/audiomentations.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiomentations
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for audio data augmentation. Inspired by albumentations. Useful for machine learning.
 Home-page: https://github.com/iver56/audiomentations
 Author: Iver Jordal
 License: MIT
 Description: # Audiomentations
         
         [![Build status](https://img.shields.io/circleci/project/github/iver56/audiomentations/master.svg)](https://circleci.com/gh/iver56/audiomentations) [![Code coverage](https://img.shields.io/codecov/c/github/iver56/audiomentations/master.svg)](https://codecov.io/gh/iver56/audiomentations) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black) [![Licence: MIT](https://img.shields.io/pypi/l/audiomentations)](https://github.com/iver56/audiomentations/blob/master/LICENSE)
@@ -64,9 +64,12 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `audiomentations-0.8.0/PKG-INFO` & `audiomentations-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiomentations
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for audio data augmentation. Inspired by albumentations. Useful for machine learning.
 Home-page: https://github.com/iver56/audiomentations
 Author: Iver Jordal
 License: MIT
 Description: # Audiomentations
         
         [![Build status](https://img.shields.io/circleci/project/github/iver56/audiomentations/master.svg)](https://circleci.com/gh/iver56/audiomentations) [![Code coverage](https://img.shields.io/codecov/c/github/iver56/audiomentations/master.svg)](https://codecov.io/gh/iver56/audiomentations) [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black) [![Licence: MIT](https://img.shields.io/pypi/l/audiomentations)](https://github.com/iver56/audiomentations/blob/master/LICENSE)
@@ -64,9 +64,12 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `audiomentations-0.8.0/README.md` & `audiomentations-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `audiomentations-0.8.0/setup.py` & `audiomentations-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,18 +30,21 @@
     description="A Python library for audio data augmentation. Inspired by albumentations."
     " Useful for machine learning.",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iver56/audiomentations",
     packages=find_packages(exclude=["demo", "tests"]),
-    install_requires=["numpy>=1.13.0", "librosa>=0.6.1,<0.7", "scipy>=1.0.0,<2"],
+    install_requires=["numpy>=1.13.0", "librosa>=0.6.1,<=0.7.1", "scipy>=1.0.0,<2"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
+        "Topic :: Multimedia",
+        "Topic :: Multimedia :: Sound/Audio",
+        "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

