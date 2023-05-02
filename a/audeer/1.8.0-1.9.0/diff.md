# Comparing `tmp/audeer-1.8.0.tar.gz` & `tmp/audeer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/audeer-1.8.0.tar", last modified: Thu Dec  3 10:34:37 2020, max compression
+gzip compressed data, was "audeer-1.9.0.tar", last modified: Thu Jan 21 16:22:47 2021, max compression
```

## Comparing `audeer-1.8.0.tar` & `audeer-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.809052 audeer-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.805052 audeer-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.805052 audeer-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2027 2020-12-03 10:34:26.000000 audeer-1.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2020-12-03 10:34:26.000000 audeer-1.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)       74 2020-12-03 10:34:26.000000 audeer-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     7162 2020-12-03 10:34:26.000000 audeer-1.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2067 2020-12-03 10:34:26.000000 audeer-1.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1143 2020-12-03 10:34:26.000000 audeer-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3012 2020-12-03 10:34:37.809052 audeer-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2020-12-03 10:34:26.000000 audeer-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.805052 audeer-1.8.0/audeer/
--rw-r--r--   0 runner    (1001) docker     (116)      816 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.809052 audeer-1.8.0/audeer/core/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      612 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/core/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     8955 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/core/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     1897 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/core/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (116)    13652 2020-12-03 10:34:26.000000 audeer-1.8.0/audeer/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.805052 audeer-1.8.0/audeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3012 2020-12-03 10:34:37.000000 audeer-1.8.0/audeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      671 2020-12-03 10:34:37.000000 audeer-1.8.0/audeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-03 10:34:37.000000 audeer-1.8.0/audeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-12-03 10:34:37.000000 audeer-1.8.0/audeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-03 10:34:37.000000 audeer-1.8.0/audeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.809052 audeer-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     1201 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/api-audeer.rst
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (116)      531 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      286 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)       89 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      786 2020-12-03 10:34:26.000000 audeer-1.8.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-12-03 10:34:26.000000 audeer-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1288 2020-12-03 10:34:37.809052 audeer-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-12-03 10:34:26.000000 audeer-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:34:37.809052 audeer-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       51 2020-12-03 10:34:26.000000 audeer-1.8.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     9544 2020-12-03 10:34:26.000000 audeer-1.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     1159 2020-12-03 10:34:26.000000 audeer-1.8.0/tests/test_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (116)     7710 2020-12-03 10:34:26.000000 audeer-1.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2027 2021-01-21 16:22:35.000000 audeer-1.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1087 2021-01-21 16:22:35.000000 audeer-1.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2021-01-21 16:22:35.000000 audeer-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     7256 2021-01-21 16:22:35.000000 audeer-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2067 2021-01-21 16:22:35.000000 audeer-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1143 2021-01-21 16:22:35.000000 audeer-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     3012 2021-01-21 16:22:47.574871 audeer-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1682 2021-01-21 16:22:35.000000 audeer-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/audeer/
+-rw-r--r--   0 runner    (1001) docker     (116)      836 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/audeer/core/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      612 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9494 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1897 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/core/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13652 2021-01-21 16:22:35.000000 audeer-1.9.0/audeer/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/audeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3012 2021-01-21 16:22:47.000000 audeer-1.9.0/audeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      671 2021-01-21 16:22:47.000000 audeer-1.9.0/audeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-21 16:22:47.000000 audeer-1.9.0/audeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-01-21 16:22:47.000000 audeer-1.9.0/audeer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2021-01-21 16:22:47.000000 audeer-1.9.0/audeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     1267 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/api-audeer.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1355 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      531 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      286 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      786 2021-01-21 16:22:35.000000 audeer-1.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-01-21 16:22:35.000000 audeer-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1288 2021-01-21 16:22:47.578872 audeer-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2021-01-21 16:22:35.000000 audeer-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-21 16:22:47.574871 audeer-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)       51 2021-01-21 16:22:35.000000 audeer-1.9.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    10161 2021-01-21 16:22:35.000000 audeer-1.9.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1159 2021-01-21 16:22:35.000000 audeer-1.9.0/tests/test_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7710 2021-01-21 16:22:35.000000 audeer-1.9.0/tests/test_utils.py
```

### Comparing `audeer-1.8.0/.github/workflows/publish.yml` & `audeer-1.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/.github/workflows/test.yml` & `audeer-1.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/CHANGELOG.rst` & `audeer-1.9.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.9.0 (2021-01-21)
+--------------------------
+
+* Added: ``audeer.list_dir_names()``
+
+
 Version 1.8.0 (2020-12-03)
 --------------------------
 
 * Added: :func:`audeer.is_uid`
 
 
 Version 1.7.0 (2020-12-02)
```

### Comparing `audeer-1.8.0/CONTRIBUTING.rst` & `audeer-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/LICENSE` & `audeer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/PKG-INFO` & `audeer-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audeer
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helpful Python functions
 Home-page: https://github.com/audeering/audeer/
 Author: Hagen Wierstorf, Johannes Wagner
 Author-email: hwierstorf@audeering.com, jwagner@audeering.com
 Maintainer: Hagen Wierstorf
 Maintainer-email: hwierstorf@audeering.com
 License: MIT
```

### Comparing `audeer-1.8.0/README.rst` & `audeer-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/audeer/__init__.py` & `audeer-1.9.0/audeer/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from audeer.core.config import config
 from audeer.core.io import (
     basename_wo_ext,
     common_directory,
     extract_archive,
     extract_archives,
     file_extension,
+    list_dir_names,
     list_file_names,
     mkdir,
     safe_path,
 )
 from audeer.core.tqdm import (
     format_display_message,
     progress_bar,
```

### Comparing `audeer-1.8.0/audeer/core/config.py` & `audeer-1.9.0/audeer/core/config.py`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/audeer/core/io.py` & `audeer-1.9.0/audeer/core/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,14 +229,37 @@
         'wav'
 
     """
     path = safe_path(path)
     return os.path.splitext(path)[-1][1:]
 
 
+def list_dir_names(
+        path: typing.Union[str, bytes],
+) -> typing.List:
+    """List of folder names located inside provided path.
+
+    Args:
+        path: path to directory
+
+    Returns:
+        list of paths to directories
+
+    Example:
+        >>> path = mkdir('path1/path2')
+        >>> dirs = list_dir_names('path1')
+        >>> os.path.basename(dirs[0])
+        'path2'
+
+    """
+    path = safe_path(path)
+    paths = [os.path.join(path, p) for p in os.listdir(path)]
+    return sorted([p for p in paths if os.path.isdir(p)])
+
+
 def list_file_names(
         path: typing.Union[str, bytes],
         *,
         filetype: str = ''
 ) -> typing.List:
     """List of file names inferred from provided path.
```

### Comparing `audeer-1.8.0/audeer/core/tqdm.py` & `audeer-1.9.0/audeer/core/tqdm.py`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/audeer/core/utils.py` & `audeer-1.9.0/audeer/core/utils.py`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/audeer.egg-info/PKG-INFO` & `audeer-1.9.0/audeer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audeer
-Version: 1.8.0
+Version: 1.9.0
 Summary: Helpful Python functions
 Home-page: https://github.com/audeering/audeer/
 Author: Hagen Wierstorf, Johannes Wagner
 Author-email: hwierstorf@audeering.com, jwagner@audeering.com
 Maintainer: Hagen Wierstorf
 Maintainer-email: hwierstorf@audeering.com
 License: MIT
```

### Comparing `audeer-1.8.0/audeer.egg-info/SOURCES.txt` & `audeer-1.9.0/audeer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/docs/api-audeer.rst` & `audeer-1.9.0/docs/api-audeer.rst`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,19 @@
 .. autofunction:: freeze_requirements
 
 is_uid
 ------
 
 .. autofunction:: is_uid
 
+list_dir_names
+---------------
+
+.. autofunction:: list_dir_names
+
 list_file_names
 ---------------
 
 .. autofunction:: list_file_names
 
 mkdir
 -----
```

### Comparing `audeer-1.8.0/docs/conf.py` & `audeer-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/docs/index.rst` & `audeer-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/docs/usage.rst` & `audeer-1.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/setup.cfg` & `audeer-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/tests/test_io.py` & `audeer-1.9.0/tests/test_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,29 +157,53 @@
     _, expected = os.path.splitdrive(expected)
     common = common.replace('\\', '/')
     expected = expected.replace('\\', '/')
     assert common == expected
 
 
 @pytest.mark.parametrize('path,extension', [
+    ('', ''),
     ('~/.bashrc', ''),
     ('file.tar.gz', 'gz'),
     ('/a/c.d/g', ''),
     ('/a/c.d/g.exe', 'exe'),
     ('../.././README.md', 'md'),
     (b'../.././README.md', 'md'),
     ('folder/file.txt', 'txt'),
     (b'folder/file.txt', 'txt'),
+    ('test.WAV', 'WAV'),
+    ('test.WaV', 'WaV'),
 ])
 def test_file_extension(path, extension):
     ext = audeer.file_extension(path)
     assert ext == extension
     assert type(ext) is str
 
 
+@pytest.mark.parametrize('dir_list', [
+    [],
+    ['a', 'b', 'c'],
+    ['a'],
+])
+def test_list_dir_names(tmpdir, dir_list):
+    dir_tmp = tmpdir.mkdir('folder')
+    directories = []
+    for directory in dir_list:
+        directory = os.path.join(str(dir_tmp), directory)
+        directories.append(audeer.mkdir(directory))
+
+    for directory in directories:
+        assert os.path.isdir(directory)
+
+    path = os.path.join(str(dir_tmp), '.')
+    dirs = audeer.list_dir_names(path)
+    assert dirs == sorted(directories)
+    assert type(dirs) is list
+
+
 @pytest.mark.parametrize('files,path,filetype,file_list', [
     ([], '.', '', []),
     ([], '.', 'wav', []),
     (['t1.wav', 't2.wav', 't3.ogg'], '.', '', ['t1.wav', 't2.wav', 't3.ogg']),
     (['t1.wav', 't2.wav', 't3.ogg'], '.', 'ogg', ['t3.ogg']),
     (['t1.wav'], 't1.wav', '', ['t1.wav']),
 ])
```

### Comparing `audeer-1.8.0/tests/test_tqdm.py` & `audeer-1.9.0/tests/test_tqdm.py`

 * *Files identical despite different names*

### Comparing `audeer-1.8.0/tests/test_utils.py` & `audeer-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

