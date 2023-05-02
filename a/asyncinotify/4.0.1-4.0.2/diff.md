# Comparing `tmp/asyncinotify-4.0.1.tar.gz` & `tmp/asyncinotify-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncinotify-4.0.1.tar", last modified: Tue Feb  7 05:20:57 2023, max compression
+gzip compressed data, was "asyncinotify-4.0.2.tar", last modified: Tue May  2 21:34:07 2023, max compression
```

## Comparing `asyncinotify-4.0.1.tar` & `asyncinotify-4.0.2.tar`

### file list

```diff
@@ -1,6 +1,19 @@
--rw-r--r--   0        0        0     1010 2023-02-07 05:20:42.673442 asyncinotify-4.0.1/README.rst
--rw-r--r--   0        0        0     1051 2023-02-07 05:20:42.673442 asyncinotify-4.0.1/pyproject.toml
--rw-r--r--   0        0        0    22746 2023-02-07 05:20:42.674442 asyncinotify-4.0.1/src/asyncinotify/__init__.py
--rw-r--r--   0        0        0     1385 2023-02-07 05:20:42.674442 asyncinotify-4.0.1/src/asyncinotify/_ffi.py
--rw-r--r--   0        0        0        0 2023-02-07 05:20:42.674442 asyncinotify-4.0.1/src/asyncinotify/py.typed
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 asyncinotify-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1355 2020-11-16 23:10:18.120975 asyncinotify-4.0.2/.gitignore
+-rw-r--r--   0        0        0     1737 2023-01-11 22:38:39.505665 asyncinotify-4.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      121 2020-11-16 23:10:18.120975 asyncinotify-4.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-11-16 23:10:18.120975 asyncinotify-4.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1077 2020-11-16 23:10:18.120975 asyncinotify-4.0.2/LICENSE
+-rw-r--r--   0        0        0     1011 2023-05-02 21:30:53.797793 asyncinotify-4.0.2/README.rst
+-rw-r--r--   0        0        0      634 2020-11-16 23:10:18.120975 asyncinotify-4.0.2/docs/Makefile
+-rw-r--r--   0        0        0       68 2020-11-18 20:39:20.954406 asyncinotify-4.0.2/docs/asyncinotify.rst
+-rw-r--r--   0        0        0     2299 2023-02-07 05:16:03.049588 asyncinotify-4.0.2/docs/conf.py
+-rw-r--r--   0        0        0     4524 2023-05-02 21:31:06.879013 asyncinotify-4.0.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-11-16 23:10:18.185975 asyncinotify-4.0.2/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:42:46.707537 asyncinotify-4.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     4275 2021-01-05 03:59:12.048279 asyncinotify-4.0.2/examples/recursivewatch.py
+-rw-r--r--   0        0        0     1052 2023-05-02 21:31:15.151152 asyncinotify-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0    22746 2023-02-07 05:17:25.923700 asyncinotify-4.0.2/src/asyncinotify/__init__.py
+-rw-r--r--   0        0        0     1385 2023-02-07 05:19:32.137870 asyncinotify-4.0.2/src/asyncinotify/_ffi.py
+-rw-r--r--   0        0        0        0 2022-06-02 17:02:28.469706 asyncinotify-4.0.2/src/asyncinotify/py.typed
+-rwxr-xr-x   0        0        0    15688 2023-02-07 05:18:20.320773 asyncinotify-4.0.2/test.py
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 asyncinotify-4.0.2/PKG-INFO
```

### Comparing `asyncinotify-4.0.1/README.rst` & `asyncinotify-4.0.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 possible, while still being flexible and powerful.  This is built on no external
 dependencies, and works through ctypes in a very obvious fashion.
 
 This depends on Python 3.6+ features, and will not work with prior versions.
 
 This works without any other external dependencies.
 
-The code is available on GitLab_ and the documentation is available on
+The code is available on GitHub_ and the documentation is available on
 ReadTheDocs_. The package itself is available on PyPi_.
 
 Installation
 ------------
 
 You know the drill::
 
   pip install asyncinotify
 
 .. _ospackage: https://docs.python.org/3/library/os.html#file-names-command-line-arguments-and-environment-variables
 .. _surrogateescape: https://docs.python.org/3/library/codecs.html#surrogateescape
-.. _GitLab: https://gitlab.com/Taywee/asyncinotify
+.. _GitHub: https://github.com/absperf/asyncinotify
 .. _pathlib: https://docs.python.org/3/library/pathlib.html
 .. _ReadTheDocs: https://asyncinotify.readthedocs.io/en/latest/
 .. _PyPi: https://pypi.org/project/asyncinotify/
```

### Comparing `asyncinotify-4.0.1/pyproject.toml` & `asyncinotify-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'asyncinotify'
 description = 'A simple optionally-async python inotify library, focused on simplicity of use and operation, and leveraging modern Python features'
-version = '4.0.1'
+version = '4.0.2'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = {text = 'MIT'}
 keywords = [
     'async',
     'inotify',
 ]
@@ -23,13 +23,13 @@
 ]
 
 [[project.authors]]
 name = "Taylor C. Richberger"
 email = "tcr@absolute-performance.com"
 
 [project.urls]
-repository  = 'https://gitlab.com/Taywee/asyncinotify/'
+repository  = 'https://github.com/absperf/asyncinotify/'
 documentation = 'https://asyncinotify.readthedocs.io/'
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4", 'wheel']
```

### Comparing `asyncinotify-4.0.1/src/asyncinotify/__init__.py` & `asyncinotify-4.0.2/src/asyncinotify/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.1/src/asyncinotify/_ffi.py` & `asyncinotify-4.0.2/src/asyncinotify/_ffi.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.1/PKG-INFO` & `asyncinotify-4.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncinotify
-Version: 4.0.1
+Version: 4.0.2
 Summary: A simple optionally-async python inotify library, focused on simplicity of use and operation, and leveraging modern Python features
 Keywords: async,inotify
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
@@ -12,37 +12,37 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Project-URL: documentation, https://asyncinotify.readthedocs.io/
-Project-URL: repository, https://gitlab.com/Taywee/asyncinotify/
+Project-URL: repository, https://github.com/absperf/asyncinotify/
 
 asyncinotify
 ============
 
 An async python inotify package.  Kept as simple and easy-to-understand as
 possible, while still being flexible and powerful.  This is built on no external
 dependencies, and works through ctypes in a very obvious fashion.
 
 This depends on Python 3.6+ features, and will not work with prior versions.
 
 This works without any other external dependencies.
 
-The code is available on GitLab_ and the documentation is available on
+The code is available on GitHub_ and the documentation is available on
 ReadTheDocs_. The package itself is available on PyPi_.
 
 Installation
 ------------
 
 You know the drill::
 
   pip install asyncinotify
 
 .. _ospackage: https://docs.python.org/3/library/os.html#file-names-command-line-arguments-and-environment-variables
 .. _surrogateescape: https://docs.python.org/3/library/codecs.html#surrogateescape
-.. _GitLab: https://gitlab.com/Taywee/asyncinotify
+.. _GitHub: https://github.com/absperf/asyncinotify
 .. _pathlib: https://docs.python.org/3/library/pathlib.html
 .. _ReadTheDocs: https://asyncinotify.readthedocs.io/en/latest/
 .. _PyPi: https://pypi.org/project/asyncinotify/
```

