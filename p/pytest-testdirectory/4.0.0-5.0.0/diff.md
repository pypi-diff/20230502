# Comparing `tmp/pytest_testdirectory-4.0.0-py2.py3-none-any.whl.zip` & `tmp/pytest_testdirectory-5.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9932 bytes, number of entries: 11
--rw-rw-r--  2.0 unx        0 b- defN 19-Jan-30 14:38 pytest_testdirectory/__init__.py
--rw-rw-r--  2.0 unx     2160 b- defN 22-Feb-21 07:50 pytest_testdirectory/checkoutput.py
--rw-rw-r--  2.0 unx     1138 b- defN 22-Feb-21 07:50 pytest_testdirectory/runresult.py
--rw-rw-r--  2.0 unx      207 b- defN 22-Feb-21 07:50 pytest_testdirectory/runresulterror.py
--rw-rw-r--  2.0 unx    12883 b- defN 22-Feb-21 08:58 pytest_testdirectory/testdirectory.py
--rw-r--r--  2.0 unx     1505 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/LICENSE.rst
--rw-rw-r--  2.0 unx     5119 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       21 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1021 b- defN 22-Feb-21 08:59 pytest_testdirectory-4.0.0.dist-info/RECORD
-11 files, 24226 bytes uncompressed, 8162 bytes compressed:  66.3%
+Zip file size: 10329 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx        0 b- defN 19-Jan-03 07:57 pytest_testdirectory/__init__.py
+-rw-rw-r--  2.0 unx     2161 b- defN 23-May-02 06:14 pytest_testdirectory/checkoutput.py
+-rw-rw-r--  2.0 unx     1138 b- defN 23-May-02 06:14 pytest_testdirectory/runresult.py
+-rw-rw-r--  2.0 unx      207 b- defN 23-May-02 06:14 pytest_testdirectory/runresulterror.py
+-rw-rw-r--  2.0 unx    14304 b- defN 23-May-02 06:14 pytest_testdirectory/testdirectory.py
+-rw-r--r--  2.0 unx     1505 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/LICENSE.rst
+-rw-rw-r--  2.0 unx     4870 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       63 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       21 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1021 b- defN 23-May-02 06:25 pytest_testdirectory-5.0.0.dist-info/RECORD
+11 files, 25400 bytes uncompressed, 8559 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pytest_testdirectory/runresulterror.py
 Comment: 
 
 Filename: pytest_testdirectory/testdirectory.py
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/LICENSE.rst
+Filename: pytest_testdirectory-5.0.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/METADATA
+Filename: pytest_testdirectory-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/WHEEL
+Filename: pytest_testdirectory-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/entry_points.txt
+Filename: pytest_testdirectory-5.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/top_level.txt
+Filename: pytest_testdirectory-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytest_testdirectory-4.0.0.dist-info/RECORD
+Filename: pytest_testdirectory-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_testdirectory/checkoutput.py

```diff
@@ -19,15 +19,15 @@
         self.output = output.splitlines()
 
     def match(self, pattern):
         """Matches the lines in the output with the pattern. The match
         pattern can contain basic wildcards, see
         https://docs.python.org/2/library/fnmatch.html
 
-        For convenience:
+        For convenience::
 
             +-----------------------------------------+
             |Pattern|Meaning                          |
             +-----------------------------------------+
             |*      |matches everything               |
             +-----------------------------------------+
             |?      |matches any single character     |
```

## pytest_testdirectory/testdirectory.py

```diff
@@ -1,135 +1,147 @@
 import pytest
 import py
 import glob
 import subprocess
 import time
 import os
 import sys
+import pathlib
+import shutil
 
 from . import runresult
 from . import runresulterror
 from . import checkoutput
 
 
 @pytest.fixture
 def testdirectory(tmpdir):
     """Creates the py.test fixture to make it usable withing the unit tests.
     See the TestDirectory class for more information.
     """
-    return TestDirectory(tmpdir)
+    return TestDirectory(tmpdir=pathlib.Path(str(tmpdir)))
 
 
-class TestDirectory(object):
+class TestDirectory:
     """Testing code by invoking executable which potentially creates and deletes
     files and directories can be hard and error prone.
 
     The purpose of this module is to simplify this task.
 
     To make it easy to use in with pytest the TestDirectory object can be
     injected into a test function by using the testdirectory fixture.
 
-    Example:
+    Example::
 
         def test_this_function(testdirectory):
             images = testdirectory.mkdir('images')
             images.copy_files('test/images/*')
 
             r = testdirectory.run('imagecompress --path=images')
 
             # r is an RunResult object containing information about the command
             # we just executed
             assert r.returncode == 0
 
+
     The testdirectory is an instance of TestDirectory and represents an actual
     temporary directory somewhere on the machine running the test code. Using
     the API we can create additional temporary directories, populate them with
     an initial set of files and finally run some executable and observe its
     behavior.
 
     Inspiration:
      - http://search.cpan.org/~sanbeg/Test-Directory-0.041/lib/Test/Directory.pm
      - pytest internal plugin for doing the same thing:
            https://github.com/pytest-dev/pytest/blob/master/_pytest/capture.py
+
     """
 
     def __init__(self, tmpdir):
+        """Create a new TestDirectory instance.
 
-        if isinstance(tmpdir, py.path.local):
-            self.tmpdir = tmpdir
-        else:
-            self.tmpdir = py.path.local(path=tmpdir)
+        :param tmpdir: The temporary directory as a py.path.local instance or str.
+        """
+        self.tmpdir = tmpdir
 
     @staticmethod
     def from_path(path):
         """Create a new TestDirectory instance from a path.
 
-        :param path: The path as a string.
+        :param path: The path as a string or pathlib.Path object.
         """
-        assert os.path.isdir(path)
-        return TestDirectory(py.path.local(path))
+        path = pathlib.Path(path)
+
+        if not path.is_dir():
+            raise ValueError(f"{path} does not exist or is not a directory")
+
+        return TestDirectory(tmpdir=path)
 
     def mkdir(self, directory):
         """Create a sub-directory in the temporary / test dir.
 
-        :param directory: The
+        :param directory: The sub-directory to create as a string or pathlib.Path.
         """
-        return TestDirectory(self.tmpdir.mkdir(directory))
+        directory = pathlib.Path(directory)
+
+        child_directory = self.tmpdir / directory
+        child_directory.mkdir(parents=True, exist_ok=True)
+
+        return TestDirectory(tmpdir=child_directory)
 
     def rmdir(self):
-        """Remove the directory."""
-        self.tmpdir.remove()
+        """Remove the directory. If the directory is not empty, remove all
+        files and directories recursively."""
+        if self.tmpdir.exists():
+            shutil.rmtree(self.tmpdir)
 
         # @todo not sure if this is a good idea, but I guess the tmpdir is
         # invalid after the remove?
         self.tmpdir = None
 
     def join(self, *args):
-        """Get a TestDirectory instance representing a path."""
-        path = self.tmpdir.join(*args)
-        assert path.isdir()
+        """Get a TestDirectory instance representing an existing path"""
 
-        return TestDirectory(tmpdir=path)
+        new_path = self.tmpdir.joinpath(*args)
+
+        if not new_path.exists():
+            raise ValueError(f"{new_path} does not exist")
+
+        return TestDirectory(tmpdir=new_path)
 
     def rmfile(self, filename):
         """Remove a file.
 
-        :param filename The name of the file to remove as a string
+        :param filename: The name of the file to remove as a pathlib.Path or string.
         """
-        os.remove(os.path.join(self.path(), filename))
+        file_path = self.tmpdir / pathlib.Path(filename)
+
+        if file_path.is_file():
+            file_path.unlink()
+        else:
+            raise FileNotFoundError(f"{filename} does not exist or is not a file.")
 
     def path(self):
         """:return: The path to the temporary directory as a string"""
         return str(self.tmpdir)
 
     def copy_file(self, filename, rename_as=""):
-        """Copy the file to the test directory.
+        """Copy the file to the test directory. Preserve file flags.
 
-        :param filename: The filename as a string.
+        :param filename: The filename as a string or pathlib.Path object.
         :param rename_as: If specified rename the file represented by filename
             to the name given in rename_as as a string.
-        :return: The path to the file in its new location as a string.
+        :return: The path to the file in its new location as a pathlib.Path object.
         """
-
-        filename = self._expand_filename(filename=filename)
-
-        # Copy the file to the tmpdir
-        filepath = py.path.local(filename)
-        filepath.copy(self.tmpdir)
-
-        print("Copy: {} -> {}".format(filepath, self.tmpdir))
-
-        filepath = self.tmpdir.join(filepath.basename)
-        if rename_as:
-            target = self.tmpdir.join(rename_as)
-            filepath.rename(target)
-            print("Rename: {} -> {}".format(filepath, target))
-            filepath = target
-
-        return str(filepath)
+        file_path = pathlib.Path(filename)
+        new_path = pathlib.Path(str(self.tmpdir)) / (
+            rename_as if rename_as else file_path.name
+        )
+        shutil.copy2(str(file_path), str(new_path))
+        return new_path
 
     def symlink_file(self, filename, rename_as="", relative=True):
         """Create a symlink to the file in the test directory.
 
         :param filename: The filename as a string. This is the original
             file we want to create a symlink to.
         :param rename_as: If specified rename the file represented by filename
@@ -141,17 +153,17 @@
         filename = self._expand_filename(filename=filename)
 
         filepath = str(py.path.local(filename))
 
         if relative:
             filepath = os.path.relpath(start=str(self.tmpdir), path=filepath)
 
-        link_name = self.tmpdir.join(os.path.basename(filepath))
+        link_name = self.tmpdir.joinpath(os.path.basename(filepath))
         if rename_as:
-            link_name = self.tmpdir.join(rename_as)
+            link_name = self.tmpdir.joinpath(rename_as)
 
         self._create_symlink(str(filepath), str(link_name), isdir=False)
 
         print("Symlink file: {} -> {}".format(filepath, link_name))
 
         return str(link_name)
 
@@ -173,102 +185,103 @@
         # Get the name of the directory:
         # https://stackoverflow.com/a/3925147/1717320
         directory_name = os.path.basename(os.path.normpath(directory))
 
         if relative:
             directory = os.path.relpath(start=str(self.tmpdir), path=directory)
 
-        link_name = self.tmpdir.join(directory_name)
+        link_name = self.tmpdir.joinpath(directory_name)
 
         if rename_as:
-            link_name = self.tmpdir.join(rename_as)
+            link_name = self.tmpdir.joinpath(rename_as)
 
         self._create_symlink(source=directory, link_name=str(link_name), isdir=True)
 
         return str(link_name)
 
     def copy_files(self, filename):
+        """Copy files into testdirectory. Expand filename by expanding wildcards
+        e.g. ``dir/*``
+
+        :param filename: The filename as a string or pathlib.Path. This
+            represents a single file or glob pattern.
+        """
 
         # Expand filename by expanding wildcards e.g. 'dir/*', the
         # glob returns a list of files
         files = glob.glob(filename)
 
-        for f in files:
-            self.copy_file(f)
+        for file in files:
+            self.copy_file(filename=file)
 
     def copy_dir(self, directory):
         """Copy a directory into the test directory.
 
-        Example (using the test fixture test_directory):
+        Example (using the test fixture test_directory)::
 
             def test_something(test_directory):
 
                 # Prints /tmp/pytest-9/some_test
                 print(test_directory.path())
 
                 app_dir = test_directory.copy_dir('/home/ok/app')
 
                 # Prints /tmp/pytest-9/some_test/app
                 print(app_dir.path())
 
-        :param directory: Path to the directory as a string
+        :param directory: Path to the directory as a string or pathlib.Path
         :return: TestDirectory object representing the copied directory
         """
+        src_dir = pathlib.Path(directory)
+        dst_dir = self.tmpdir / src_dir.name
+        shutil.copytree(src_dir, dst_dir)
 
-        # From: http://stackoverflow.com/a/3925147
-        name = os.path.basename(os.path.normpath(directory))
-
-        # We need to create the directory
-        target_dir = self.tmpdir.mkdir(name)
+        return TestDirectory(tmpdir=dst_dir)
 
-        source_dir = py.path.local(directory)
-        source_dir.copy(target_dir)
-
-        print("Copy Dir: {} -> {}".format(source_dir, target_dir))
-
-        return TestDirectory(target_dir)
-
-    def write_text(self, filename, data, encoding):
+    def write_text(self, filename, data, encoding="utf-8"):
         """Writes a file in the temporary directory.
 
-        :return: The path to the file as a string
-        """
-
-        f = self.tmpdir.join(filename)
-        f.write_text(data=data, encoding=encoding)
-        return str(f)
+        :param filename: Filename as string or pathlib.Path
+        :param data: The text data to write
+        :param encoding: The encoding to use (default utf-8)
+        :return: The path to the file as a pathlib.Path
+        """
+        file_path = self.tmpdir / pathlib.Path(filename)
+        file_path.write_text(data, encoding=encoding)
+        return file_path
 
     def write_binary(self, filename, data):
-        """Writes a file in the temporary directory."""
+        """Writes binary data to a file in the temporary directory.
 
-        f = self.tmpdir.join(filename)
-
-        print(type(f.strpath))
-
-        f.write_binary(data=data)
+        :param filename: Filename as string or pathlib.Path
+        :param data: The binary data to write
+        :return: The path to the file as a pathlib.Path
+        """
+        file_path = self.tmpdir / pathlib.Path(filename)
+        file_path.write_bytes(data)
+        return file_path
 
     def contains_file(self, filename):
-        """Checks for the existance of a file.
+        """Checks for the existence of a file.
 
-        :param filename: The filename to check for.
+        :param filename: The filename to check for as a string or pathlib.Path.
+                        May contain glob patterns.
         :return: True if the file is contained within the test directory.
+        :raises: ValueError if there is more than one match.
         """
-        files = glob.glob(os.path.join(self.path(), filename))
-
-        if len(files) == 0:
+        matches = list(self.tmpdir.glob(filename))
+        if len(matches) == 1 and matches[0].is_file():
+            return True
+        elif len(matches) > 1:
+            raise ValueError(f"Found multiple matches for {filename}")
+        else:
             return False
 
-        assert len(files) == 1
-
-        filename = files[0]
-
-        return os.path.isfile(filename)
-
     def contains_dir(self, *directories):
-        """Checks for the existance of a directory.
+        """Checks for the existence of a directory.
 
         :param dirname: The directory name to check for.
         :return: True if the directory is contained within the test directory.
         """
 
         # Expand filename by expanding wildcards e.g. 'dir/*/file.txt', the
         # glob should return only one file
@@ -321,15 +334,15 @@
         start_time = time.time()
 
         popen = subprocess.Popen(
             args,
             # Need to decode the stdout and stderr with the correct
             # character encoding (http://stackoverflow.com/a/28996987)
             universal_newlines=True,
-            **kwargs
+            **kwargs,
         )
 
         stdout, stderr = popen.communicate()
 
         end_time = time.time()
 
         # The stdout and stderr are wrapped in a CheckOutput object to make
@@ -356,16 +369,18 @@
 
         if popen.returncode != 0:
             raise runresulterror.RunResultError(result)
 
         return result
 
     def __str__(self):
-        """:return: String representation of the testdirectory which is
-        the path.
+        """Generate a single string representation of the testdirectory.
+
+        :return: String representation of the testdirectory which is
+            the path.
         """
         return str(self.tmpdir)
 
     def _create_symlink(self, source, link_name, isdir):
         """Create a symbolic link pointing to source named link_name."""
 
         # os.symlink() is not available in Python 2.7 on Windows.
@@ -387,21 +402,21 @@
                 self.run(" ".join(cmd), shell=True)
 
             os_symlink = symlink_windows
 
         os_symlink(source, link_name)
 
     def _expand_filename(self, filename):
-        """Expand filename by expanding wildcards e.g. 'dir/*/file.txt'.
+        r"""Expand filename by expanding wildcards e.g. ``'dir/*/file.txt'``.
 
         The glob should return only one file
         """
-        files = glob.glob(filename)
-
-        print(filename)
-        print(files)
 
-        assert len(files) == 1
+        filename = pathlib.Path(filename)
+        files = list(filename.parent.glob(filename.name))
 
-        filename = files[0]
+        if len(files) != 1:
+            raise ValueError(
+                f"Expected one file matching {filename}, found {len(files)}."
+            )
 
-        return filename
+        return files[0]
```

## Comparing `pytest_testdirectory-4.0.0.dist-info/LICENSE.rst` & `pytest_testdirectory-5.0.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `pytest_testdirectory-4.0.0.dist-info/METADATA` & `pytest_testdirectory-5.0.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-testdirectory
-Version: 4.0.0
+Version: 5.0.0
 Summary: A py.test plugin providing temporary directories in unit tests.
 Home-page: https://github.com/steinwurf/pytest-testdirectory
 Author: Steinwurf ApS
 Author-email: contact@steinwurf.com
 License: BSD 3-clause "New" or "Revised" License
 Keywords: pytest py.test testing unit tests plugin
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: pytest
 
 ============
 Introduction
```

## Comparing `pytest_testdirectory-4.0.0.dist-info/RECORD` & `pytest_testdirectory-5.0.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pytest_testdirectory/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytest_testdirectory/checkoutput.py,sha256=sXe2Abm7DvXy7XnRFXcoJMNXIAeXN33TyQ8xGeIxMqQ,2160
+pytest_testdirectory/checkoutput.py,sha256=4DiZoQY1EJGVJWOLupT3BidYdvWcM7E6B3Hin2-uad0,2161
 pytest_testdirectory/runresult.py,sha256=K4PMte9biSJnpUkL4meWneGOs5Loz_XAWoAG2DFyonw,1138
 pytest_testdirectory/runresulterror.py,sha256=czqqy89yml989DBjE8Mtv65Vc9xUw0W4iJkGj38XXP4,207
-pytest_testdirectory/testdirectory.py,sha256=uLInGH6x8ihrHA3c5PQy_9RUIC6Kt7uqFybGVReDMjQ,12883
-pytest_testdirectory-4.0.0.dist-info/LICENSE.rst,sha256=HArmY8aYqGyVqtLfpBVBWf1vgzJbKUS-QmZfvekTA3Q,1505
-pytest_testdirectory-4.0.0.dist-info/METADATA,sha256=aiZTSnakVsGTjJMI51IQsqDVhZHT0kuDEFLKJP7fZ7Q,5119
-pytest_testdirectory-4.0.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-pytest_testdirectory-4.0.0.dist-info/entry_points.txt,sha256=EiqV4mCwEawpjddV96Z9TMTKBoq6nssgyoqJYZ17ggg,62
-pytest_testdirectory-4.0.0.dist-info/top_level.txt,sha256=PEzlu-W8nx0a-74PHHqVmjTOpuCqO2kNYAjGH5_7EH4,21
-pytest_testdirectory-4.0.0.dist-info/RECORD,,
+pytest_testdirectory/testdirectory.py,sha256=PFmfroDVseg3aU_kBqLQyqx2ZXXUjSA7OdoKA1PU3Jw,14304
+pytest_testdirectory-5.0.0.dist-info/LICENSE.rst,sha256=HArmY8aYqGyVqtLfpBVBWf1vgzJbKUS-QmZfvekTA3Q,1505
+pytest_testdirectory-5.0.0.dist-info/METADATA,sha256=1FLhB7Uda-2HkalEP5xsmHWQtFmKI_OwRq2ZSfYF9mE,4870
+pytest_testdirectory-5.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pytest_testdirectory-5.0.0.dist-info/entry_points.txt,sha256=5D2qPl7g7g3G9YKWwgPjExMirn3mggDb-fsrvew3GWY,63
+pytest_testdirectory-5.0.0.dist-info/top_level.txt,sha256=PEzlu-W8nx0a-74PHHqVmjTOpuCqO2kNYAjGH5_7EH4,21
+pytest_testdirectory-5.0.0.dist-info/RECORD,,
```

