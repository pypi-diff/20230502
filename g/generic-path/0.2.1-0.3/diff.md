# Comparing `tmp/generic-path-0.2.1.tar.gz` & `tmp/generic-path-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-path-0.2.1.tar", last modified: Fri Apr 28 05:44:21 2023, max compression
+gzip compressed data, was "generic-path-0.3.tar", last modified: Tue May  2 02:14:41 2023, max compression
```

## Comparing `generic-path-0.2.1.tar` & `generic-path-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:44:21.571230 generic-path-0.2.1/
--rw-rw-rw-   0        0        0      126 2023-04-28 04:03:00.000000 generic-path-0.2.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    17098 2023-04-27 15:37:26.000000 generic-path-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5548 2023-04-28 05:44:21.570229 generic-path-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3847 2023-04-28 05:41:22.000000 generic-path-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 05:44:21.569229 generic-path-0.2.1/generic_path.egg-info/
--rw-rw-rw-   0        0        0     5548 2023-04-28 05:44:21.000000 generic-path-0.2.1/generic_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-28 05:44:21.000000 generic-path-0.2.1/generic_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:44:21.000000 generic-path-0.2.1/generic_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2023-04-28 05:44:21.000000 generic-path-0.2.1/generic_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 05:44:21.000000 generic-path-0.2.1/generic_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25174 2023-04-28 05:42:51.000000 generic-path-0.2.1/gpath.py
--rw-rw-rw-   0        0        0     2091 2023-04-28 04:22:44.000000 generic-path-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 05:44:21.571230 generic-path-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 05:44:21.569229 generic-path-0.2.1/tests/
--rw-rw-rw-   0        0        0    35409 2023-04-28 03:55:11.000000 generic-path-0.2.1/tests/test_gpath.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.629828 generic-path-0.3/
+-rw-rw-rw-   0        0        0      900 2023-05-02 02:11:59.000000 generic-path-0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0    17098 2023-05-02 02:11:14.000000 generic-path-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     7270 2023-05-02 02:14:41.629828 generic-path-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4712 2023-05-02 02:11:59.000000 generic-path-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.628829 generic-path-0.3/generic_path.egg-info/
+-rw-rw-rw-   0        0        0     7270 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      298 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 02:14:41.000000 generic-path-0.3/generic_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    32101 2023-05-02 02:11:59.000000 generic-path-0.3/gpath.py
+-rw-rw-rw-   0        0        0     2231 2023-05-02 02:11:59.000000 generic-path-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 02:14:41.629828 generic-path-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 02:14:41.628829 generic-path-0.3/tests/
+-rw-rw-rw-   0        0        0    35856 2023-05-02 02:11:59.000000 generic-path-0.3/tests/test_gpath.py
```

### Comparing `generic-path-0.2.1/LICENSE.txt` & `generic-path-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generic-path-0.2.1/PKG-INFO` & `generic-path-0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,119 @@
-Metadata-Version: 2.1
-Name: generic-path
-Version: 0.2.1
-Summary: GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
-Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
-License: MPL-2.0
-Project-URL: Homepage, https://github.com/yushiyangk/GPath
-Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
-Keywords: python,filepath,filesystem,cross-platform
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Filesystems
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: config
-Provides-Extra: package
-Provides-Extra: packagetest
-Provides-Extra: ci
-Provides-Extra: publish
-License-File: LICENSE.txt
-
-# GPath
-
-**GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
-
-## Install
-
-```
-pip install generic-path
-```
-
-## Basic examples
-
-Import GPath:
-```python
-from gpath import GPath
-```
-
-Create a GPath object and manipulate it:
-```python
-g = GPath("/usr/bin")
-
-common = GPath.find_common(g, "/usr/local/bin")  # GPath("/usr")
-relpath = g.relpath_from("/usr/local/bin")       # GPath("../../bin")
-joined = GPath.join("/usr/local/bin", relpath)   # GPath("/usr/bin")
-assert g == joined
-```
-
-For function arguments, strings or `os.PathLike` objects can be used interchangeably with GPaths.
-
-Binary operations are also supported:
-```python
-g1 = GPath("C:/Windows/System32")
-g2 = GPath("../SysWOW64/drivers")
-
-added = g1 + g2      # GPath("C:/Windows/SysWOW64/drivers")
-subtracted = g1 - 1  # GPath("C:/Windows")
-
-# Shift the imaginary current working directory in relative paths
-shifted_right = g2 >> 1  # GPath("../../SysWOW64/drivers")
-shifted_left = g2 << 1   # GPath("SysWOW64/drivers")
-```
-
-The `GPath.partition()` method is useful when dealing with paths from various different sources:
-```python
-partitions = GPath.partition("/usr/bin", "/usr/local/", "../../doc", "C:/Windows", "C:/Program Files")
-
-assert partitions == {
-	GPath("/usr")      : [GPath("bin"), GPath("local")],
-	GPath("../../doc") : [GPath("")],
-	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
-}
-```
-
-## Issues
-
-Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
-
-## Development
-
-Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
-
-The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
-
-### Virtual environment
-
-Create the venv using `python -m venv .`.
-
-To activate the venv, on Linux run `source Scripts/activate`, and on Windows run `Scripts/Activate.ps1` or `Scripts/activate.bat`.
-
-Later, to deactivate the venv, run `deactivate`.
-
-### Dependencies
-
-Run `pip install -r requirements.dev.txt`.
-
-### Install
-
-To install the package locally (in the venv), run `pip install .`. To keep the installed package always in sync with the source code, instead run `pip install -e .`.
-
-### Testing
-
-For unit tests, run `pytest` or `coverage run -m pytest`.
-
-For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`.
-
-### Packaging
-
-Before packaging, check the package config by running `pyroma .`
-
-To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`.
-
-### Automated tests
-
-To test for different supported environments, run `tox -p` or <code>tox -p <var>num_workers</var></code>. This will run unit tests, check for test coverage, and also generate packages.
-
-### Config files
-
-- `pyproject.toml` Package metadata, as well as configs for test and build tools
-- `requirements.dev.txt` Package dependencies for development, in pip format
-- `requirements.publish.txt` Package dependencies for publishing, in pip format
-- `tox.ini` Config file for tox
-
-### Troubleshooting
-
-#### Unable to uninstall the local package
-
-Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
-<pre><code>Found existing installation: gpath <var>version</var>
-Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
-
-In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
-
-## Changelog
-
-### 0.2
-
-- Added support for Python versions 3.7 through 3.9; previously only 3.10 and 3.11 were supported
+# GPath
+
+**GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
+
+[![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/generic-path/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/GPath) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://gpath.gnayihs.uy/)
+
+## Install
+
+```
+pip install generic-path
+```
+
+## Basic examples
+
+Import GPath:
+```python
+from gpath import GPath
+```
+
+Create a GPath object and manipulate it:
+```python
+g = GPath("/usr/bin")
+
+common = GPath.find_common(g, "/usr/local/bin")  # GPath("/usr")
+relpath = g.relpath_from("/usr/local/bin")       # GPath("../../bin")
+joined = GPath.join("/usr/local/bin", relpath)   # GPath("/usr/bin")
+assert g == joined
+```
+
+For function arguments, strings or `os.PathLike` objects can be used interchangeably with GPaths.
+
+Binary operations are also supported:
+```python
+g1 = GPath("C:/Windows/System32")
+g2 = GPath("../SysWOW64/drivers")
+
+added = g1 + g2      # GPath("C:/Windows/SysWOW64/drivers")
+subtracted = g1 - 1  # GPath("C:/Windows")
+
+# Shift the imaginary current working directory in relative paths
+shifted_right = g2 >> 1  # GPath("../../SysWOW64/drivers")
+shifted_left = g2 << 1   # GPath("SysWOW64/drivers")
+```
+
+The `GPath.partition()` method is useful when dealing with paths from various different sources:
+```python
+partitions = GPath.partition("/usr/bin", "/usr/local/bin", "../../doc", "C:/Windows", "C:/Program Files")
+
+assert partitions == {
+	GPath("/usr")      : [GPath("bin"), GPath("local/bin")],
+	GPath("../../doc") : [GPath("")],
+	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
+}
+```
+
+## Issues
+
+Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
+
+## Development
+
+Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
+
+The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
+
+### Virtual environment
+
+Create the venv using `python -m venv .`.
+
+To activate the venv, on Linux run `source Scripts/activate`, and on Windows run `Scripts/Activate.ps1` or `Scripts/activate.bat`.
+
+Later, to deactivate the venv, run `deactivate`.
+
+### Dependencies
+
+Run `pip install -r requirements.dev.txt`.
+
+### Tasks
+
+For unit tests, run `pytest`.
+
+To run unit tests across all supported Python versions, run `tox p -m testall`. This is slower than just `pytest`. Note that only Python versions that are installed locally will be run.
+
+To run the full set of tests and tasks, run `tox p -m prepare`. This should be done prior to package publication. Alternatively, see below for manually running individual steps in this process.
+
+#### Unit tests
+
+Run `pytest` or `coverage run -m pytest`.
+
+For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`. Alternatively, run `tox r -m test` to do both steps automatically.
+
+#### Documentation
+
+Run `tox r -m docs`.
+
+The documentation is generated in `docs/html/`, using template files in `docs/template/`. However, note that the favicon file must be placed at `docs/html/favicon.png` manually as pdoc is unable to do so.
+
+#### Packaging
+
+Before packaging, check the package config by running `pyroma .` or `tox r -m config`.
+
+To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
+
+### Config files
+
+- `pyproject.toml` Package metadata, as well as configs for test and build tools
+- `requirements.dev.txt` Package dependencies for development, in pip format
+- `requirements.publish.txt` Package dependencies for publishing, in pip format
+- `tox.ini` Config file for tox
+
+### Troubleshooting
+
+#### Unable to uninstall the local package
+
+Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
+<pre><code>Found existing installation: gpath <var>version</var>
+Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
+
+In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
```

### Comparing `generic-path-0.2.1/generic_path.egg-info/PKG-INFO` & `generic-path-0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: generic-path
-Version: 0.2.1
+Version: 0.3
 Summary: GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/GPath
+Project-URL: Documentation, https://gpath.gnayihs.uy/
 Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
 Keywords: python,filepath,filesystem,cross-platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -21,25 +22,28 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: config
 Provides-Extra: package
 Provides-Extra: packagetest
 Provides-Extra: ci
 Provides-Extra: publish
 License-File: LICENSE.txt
 
 # GPath
 
 **GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 
+[![](https://img.shields.io/badge/PyPI--inactive?style=social&logo=pypi)](https://pypi.org/project/generic-path/) [![](https://img.shields.io/badge/GitHub--inactive?style=social&logo=github)](https://github.com/yushiyangk/GPath) [![](https://img.shields.io/badge/Documentation--inactive?style=social&logo=readthedocs)](https://gpath.gnayihs.uy/)
+
 ## Install
 
 ```
 pip install generic-path
 ```
 
 ## Basic examples
@@ -72,18 +76,18 @@
 # Shift the imaginary current working directory in relative paths
 shifted_right = g2 >> 1  # GPath("../../SysWOW64/drivers")
 shifted_left = g2 << 1   # GPath("SysWOW64/drivers")
 ```
 
 The `GPath.partition()` method is useful when dealing with paths from various different sources:
 ```python
-partitions = GPath.partition("/usr/bin", "/usr/local/", "../../doc", "C:/Windows", "C:/Program Files")
+partitions = GPath.partition("/usr/bin", "/usr/local/bin", "../../doc", "C:/Windows", "C:/Program Files")
 
 assert partitions == {
-	GPath("/usr")      : [GPath("bin"), GPath("local")],
+	GPath("/usr")      : [GPath("bin"), GPath("local/bin")],
 	GPath("../../doc") : [GPath("")],
 	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
 }
 ```
 
 ## Issues
 
@@ -103,33 +107,39 @@
 
 Later, to deactivate the venv, run `deactivate`.
 
 ### Dependencies
 
 Run `pip install -r requirements.dev.txt`.
 
-### Install
+### Tasks
+
+For unit tests, run `pytest`.
+
+To run unit tests across all supported Python versions, run `tox p -m testall`. This is slower than just `pytest`. Note that only Python versions that are installed locally will be run.
 
-To install the package locally (in the venv), run `pip install .`. To keep the installed package always in sync with the source code, instead run `pip install -e .`.
+To run the full set of tests and tasks, run `tox p -m prepare`. This should be done prior to package publication. Alternatively, see below for manually running individual steps in this process.
 
-### Testing
+#### Unit tests
 
-For unit tests, run `pytest` or `coverage run -m pytest`.
+Run `pytest` or `coverage run -m pytest`.
 
-For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`.
+For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`. Alternatively, run `tox r -m test` to do both steps automatically.
 
-### Packaging
+#### Documentation
 
-Before packaging, check the package config by running `pyroma .`
+Run `tox r -m docs`.
 
-To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`.
+The documentation is generated in `docs/html/`, using template files in `docs/template/`. However, note that the favicon file must be placed at `docs/html/favicon.png` manually as pdoc is unable to do so.
 
-### Automated tests
+#### Packaging
 
-To test for different supported environments, run `tox -p` or <code>tox -p <var>num_workers</var></code>. This will run unit tests, check for test coverage, and also generate packages.
+Before packaging, check the package config by running `pyroma .` or `tox r -m config`.
+
+To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`. Run `twine check dist/*` to check that the packages were generated properly. Alternatively, run `tox r -m package` to do these steps automatically.
 
 ### Config files
 
 - `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
 - `tox.ini` Config file for tox
@@ -142,10 +152,27 @@
 <pre><code>Found existing installation: gpath <var>version</var>
 Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
 
 In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
 
 ## Changelog
 
+### 0.3
+
+- Renamed <code><var>g</var>.current</code> to <code><var>g</var>.current_dir</code> and <code><var>g</var>.parent</code> to <code><var>g</var>.parent_dir</code>
+- Renamed <code><var>g</var>.is_root()</code> to <code><var>g</var>.is_absolute()</code>
+- Renamed the optional arguments in <code><var>g</var>.find_common()</code> and <code><var>g</var>.partition()</code>, from `common_current` and `common_parent` to `allow_current` and `allow_parent`
+- Added a new <code><var>g</var>.is_root()</code> that checks whether the path is exactly root
+- Added <code><var>g</var>.\_\_div\_\_()</code> as an alias of <code><var>g</var>.\_\_add\_\_()</code>
+- Added HTML documentation
+
+### 0.2.1
+
+- Fixed basic example in README
+
 ### 0.2
 
 - Added support for Python versions 3.7 through 3.9; previously only 3.10 and 3.11 were supported
+
+### 0.1
+
+- Initial version
```

### Comparing `generic-path-0.2.1/pyproject.toml` & `generic-path-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 	"Typing :: Typed",
 ]
 keywords = ["python", "filepath", "filesystem", "cross-platform"]
 requires-python = ">=3.7"
 dependencies = []
 
 [project.optional-dependencies]
-dev = ["pytest ~= 7.3.1", "coverage ~= 7.2.3", "pyroma ~= 4.2", "build ~= 0.10.0", "tox~=4.5.1"]
+dev = ["pytest ~= 7.3.1", "coverage ~= 7.2.3", "pdoc ~= 13.1.1", "pyroma ~= 4.2", "build ~= 0.10.0", "tox ~= 4.5.1", "tox-extras >= 0.0.1"]
 test = ["pytest ~= 7.3.1", "coverage ~= 7.2.3"]
+docs = ["pdoc ~= 13.1.1"]
 config = ["pyroma ~= 4.2"]
 package = ["build ~= 0.10.0"]
 packagetest = ["twine ~= 4.0.2"]
-ci = ["tox~=4.5.1"]
+ci = ["tox ~= 4.5.1", "tox-extras >= 0.0.1"]
 publish = ["twine ~= 4.0.2"]
 
 [project.urls]
 # key is used verbatim on PyPI
 Homepage = "https://github.com/yushiyangk/GPath"
+Documentation = "https://gpath.gnayihs.uy/"
 Issues = "https://github.com/yushiyangk/GPath/issues"
 
 [tool.pytest.ini_options]
 addopts = "tests"
 
 [tool.coverage.report]
 include = ["gpath.py"]
```

### Comparing `generic-path-0.2.1/tests/test_gpath.py` & `generic-path-0.3/tests/test_gpath.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 		if request.param is None:
 			return None
 		else:
 			return GPath(request.param)
 
 
 	@pytest.mark.parametrize(
-		('path', 'expected_parts', 'expected_device', 'expected_root', 'expected_dotdot'),
+		('path', 'expected_parts', 'expected_device', 'expected_absolute', 'expected_parent'),
 		[
 			(None, tuple(), "", False, 0),
 			("", tuple(), "", False, 0),
 			(".", tuple(), "", False, 0),
 			("./", tuple(), "", False, 0),
 			("./.", tuple(), "", False, 0),
 			(".//", tuple(), "", False, 0),
@@ -49,56 +49,56 @@
 			("c:/", tuple(), "c:", True, 0),
 		]
 	)
 	def test_constructor_root(self,
 		path: Optional[str],
 		expected_parts: tuple[str, ...],
 		expected_device: str,
-		expected_root: bool,
-		expected_dotdot: int,
+		expected_absolute: bool,
+		expected_parent: int,
 	):
 		"""
-			Test constructor `__init__()` as well as getters `is_root()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`, for paths requiring special treatment.
+			Test constructor `__init__()` as well as getters `is_absolute()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`, for paths requiring special treatment.
 		"""
 		if path is None:
 			gpath = GPath()
 		else:
 			gpath = GPath(path)
 
-		if expected_root and expected_dotdot > 0:
-			expected_dotdot = 0
+		if expected_absolute and expected_parent > 0:
+			expected_parent = 0
 
 		assert gpath._parts == expected_parts
 		assert gpath._device == expected_device
-		assert gpath._root == expected_root
-		assert gpath._dotdot == expected_dotdot
+		assert gpath._absolute == expected_absolute
+		assert gpath._parent == expected_parent
 
-		assert gpath.is_root() == expected_root
+		assert gpath.is_absolute() == expected_absolute
 		assert gpath.get_device() == expected_device
-		assert gpath.get_parent_level() == expected_dotdot
+		assert gpath.get_parent_level() == expected_parent
 
 		gpath_copy = GPath(gpath)
 		assert gpath_copy._parts == expected_parts
 		assert gpath_copy._device == expected_device
-		assert gpath_copy._root == expected_root
-		assert gpath_copy._dotdot == expected_dotdot
+		assert gpath_copy._absolute == expected_absolute
+		assert gpath_copy._parent == expected_parent
 
-		assert gpath_copy.is_root() == expected_root
+		assert gpath_copy.is_absolute() == expected_absolute
 		assert gpath_copy.get_device() == expected_device
-		assert gpath_copy.get_parent_level() == expected_dotdot
+		assert gpath_copy.get_parent_level() == expected_parent
 
 		expected_parent_parts = []
-		for i in range(expected_dotdot):
+		for i in range(expected_parent):
 			expected_parent_parts.append("..")
 		assert gpath.get_parent_parts() == expected_parent_parts
 		assert gpath_copy.get_parent_parts() == expected_parent_parts
 
 
 	@pytest.mark.parametrize(
-		('path', 'expected_parts', 'expected_dotdot'),
+		('path', 'expected_parts', 'expected_parent'),
 		[
 			("..", tuple(), 1),
 			("../..", tuple(), 2),
 			("bin", ("bin", ), 0),
 			("usr/bin", ("usr", "bin"), 0),
 			("../usr/bin", ("usr", "bin"), 1),
 			("../../usr/bin", ("usr", "bin"), 2),
@@ -120,15 +120,15 @@
 			("directory/русский язык", ("directory", "русский язык"), 0),
 			("directory/中文", ("directory", "中文"), 0),
 			("directory/اَلْعَرَبِيَّةُ", ("directory", "اَلْعَرَبِيَّةُ"), 0),
 		]
 	)
 	@pytest.mark.parametrize('path_suffix', ["", "/", "//", "/.", "/./", "/././/"])
 	@pytest.mark.parametrize(
-		('path_prefix', 'expected_device', 'expected_root'),
+		('path_prefix', 'expected_device', 'expected_absolute'),
 		[
 			("", "", False),
 			("/", "", True),
 			#("//", "", True),
 			("C:/", "C:", True),
 			("c:/", "c:", True),
 			#("C:", "C:", False),
@@ -136,46 +136,46 @@
 	)
 	def test_constructor(self,
 		path: str,
 		path_prefix: str,
 		path_suffix: str,
 		expected_parts: tuple[str, ...],
 		expected_device: str,
-		expected_root: bool,
-		expected_dotdot: int,
+		expected_absolute: bool,
+		expected_parent: int,
 	):
 		"""
-			Test constructor `__init__()` as well as getters `is_root()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`.
+			Test constructor `__init__()` as well as getters `is_absolute()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`.
 		"""
 		gpath = GPath(path_prefix + path + path_suffix)
-		if expected_root and expected_dotdot > 0:
-			expected_dotdot = 0
+		if expected_absolute and expected_parent > 0:
+			expected_parent = 0
 
 		assert gpath._parts == expected_parts
 		assert gpath._device == expected_device
-		assert gpath._root == expected_root
-		assert gpath._dotdot == expected_dotdot
+		assert gpath._absolute == expected_absolute
+		assert gpath._parent == expected_parent
 
-		assert gpath.is_root() == expected_root
+		assert gpath.is_absolute() == expected_absolute
 		assert gpath.get_device() == expected_device
-		assert gpath.get_parent_level() == expected_dotdot
+		assert gpath.get_parent_level() == expected_parent
 
 		gpath_copy = GPath(gpath)
 
 		assert gpath_copy._parts == expected_parts
 		assert gpath_copy._device == expected_device
-		assert gpath_copy._root == expected_root
-		assert gpath_copy._dotdot == expected_dotdot
+		assert gpath_copy._absolute == expected_absolute
+		assert gpath_copy._parent == expected_parent
 
-		assert gpath_copy.is_root() == expected_root
+		assert gpath_copy.is_absolute() == expected_absolute
 		assert gpath_copy.get_device() == expected_device
-		assert gpath_copy.get_parent_level() == expected_dotdot
+		assert gpath_copy.get_parent_level() == expected_parent
 
 		expected_parent_parts = []
-		for i in range(expected_dotdot):
+		for i in range(expected_parent):
 			expected_parent_parts.append("..")
 		assert gpath.get_parent_parts() == expected_parent_parts
 		assert gpath_copy.get_parent_parts() == expected_parent_parts
 
 
 	@pytest.mark.parametrize(
 		('gpath1', 'parts'),
@@ -206,14 +206,36 @@
 		assert result == parts
 
 		result = GPath.from_parts(parts)
 		assert result == gpath1
 
 
 	@pytest.mark.parametrize(
+		('gpath1', 'expected'),
+		[
+			("/", True),
+			("", False),
+			("..", False),
+			("C:/", True),
+			("/a", False),
+			("a", False),
+			("../a", False),
+			("C:/a", False),
+		],
+		indirect=['gpath1']
+	)
+	def test_is_root(self, gpath1: GPath, expected: bool):
+		"""
+			Test `is_root()`.
+		"""
+		result = gpath1.is_root()
+		assert result == expected
+
+
+	@pytest.mark.parametrize(
 		('path1', 'path2', 'expected'),
 		[
 			("/", "/", True),
 			("", "", True),
 			("..", "..", True),
 			("C:/", "C:/", True),
 			("/", "", False),
@@ -650,15 +672,15 @@
 
 			if gpath1 != gpath2:
 				result = gpath2.subpath_from(gpath1)
 				assert result == None
 
 		result = gpath1.relpath_from(gpath2)
 		if gpath1._device != "" and result != None:
-			print(result._parts, result._root, result._device, result._dotdot)
+			print(result._parts, result._absolute, result._device, result._parent)
 		assert result == relpath_expected_gpath
 
 
 	@pytest.mark.parametrize(
 		('gpath1', 'gpath2', 'expected_gpath'),
 		[
 			("/", "/", "/"),
@@ -891,16 +913,16 @@
 		result = gpath1 >> shift_value
 		assert result == rshift_expected_gpath
 		result = gpath1 >> (-1 * shift_value)
 		assert result == lshift_expected_gpath
 
 
 	@pytest.mark.parametrize(
-		#('path1', 'path2', 'common_current', 'common_parent', 'expected_path'),
-		('path1', 'path2', 'common_current_expected', 'common_parent_expected', 'common_current_parent_expected', 'no_common_expected'),
+		#('path1', 'path2', 'allow_current', 'allow_parents', 'expected_path'),
+		('path1', 'path2', 'allow_current_expected', 'allow_parents_expected', 'allow_current_parent_expected', 'no_common_expected'),
 		[
 			("/", "/", "/", "/", "/", "/"),
 			("/", "", None, None, None, None),
 			("/", "..", None, None, None, None),
 			("/", "C:/", None, None, None, None),
 			("/", "/a", "/", "/", "/", "/"),
 			("/", "a", None, None, None, None),
@@ -941,98 +963,98 @@
 			("C:/a", "D:/", None, None, None, None),
 			("C:/a", "C:/b", "C:/", "C:/", "C:/", "C:/"),
 		]
 	)
 	def test_find_common(self,
 		path1: str,
 		path2: str,
-		common_current_expected: str,
-		common_parent_expected: str,
-		common_current_parent_expected: str,
+		allow_current_expected: str,
+		allow_parents_expected: str,
+		allow_current_parent_expected: str,
 		no_common_expected: str
 	):
 		"""
 			Test `find_common()`.
 		"""
-		assert common_parent_expected == common_current_parent_expected
+		assert allow_parents_expected == allow_current_parent_expected
 
-		if common_current_expected is not None:
-			common_current_expected_gpath = GPath(common_current_expected)
+		if allow_current_expected is not None:
+			allow_current_expected_gpath = GPath(allow_current_expected)
 		else:
-			common_current_expected_gpath = None
+			allow_current_expected_gpath = None
 
 		result = GPath.find_common(path1, path2)
-		assert result == common_current_expected_gpath
+		assert result == allow_current_expected_gpath
 		result = GPath.find_common(path2, path1)
-		assert result == common_current_expected_gpath
+		assert result == allow_current_expected_gpath
 
 		result = GPath.find_common(GPath(path1), GPath(path2))
-		assert result == common_current_expected_gpath
+		assert result == allow_current_expected_gpath
 		result = GPath.find_common(GPath(path2), GPath(path1))
-		assert result == common_current_expected_gpath
+		assert result == allow_current_expected_gpath
 
-		result = GPath.find_common(path1, path2, common_current=True, common_parent=False)
-		assert result == common_current_expected_gpath
-		result = GPath.find_common(path2, path1, common_current=True, common_parent=False)
-		assert result == common_current_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), common_current=True, common_parent=False)
-		assert result == common_current_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), common_current=True, common_parent=False)
-		assert result == common_current_expected_gpath
+		result = GPath.find_common(path1, path2, allow_current=True, allow_parents=False)
+		assert result == allow_current_expected_gpath
+		result = GPath.find_common(path2, path1, allow_current=True, allow_parents=False)
+		assert result == allow_current_expected_gpath
+
+		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=True, allow_parents=False)
+		assert result == allow_current_expected_gpath
+		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=True, allow_parents=False)
+		assert result == allow_current_expected_gpath
 
-		if common_parent_expected is not None:
-			common_parent_expected_gpath = GPath(common_parent_expected)
+		if allow_parents_expected is not None:
+			allow_parents_expected_gpath = GPath(allow_parents_expected)
 		else:
-			common_parent_expected_gpath = None
+			allow_parents_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, common_current=False, common_parent=True)
-		assert result == common_parent_expected_gpath
-		result = GPath.find_common(path2, path1, common_current=False, common_parent=True)
-		assert result == common_parent_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), common_current=False, common_parent=True)
-		assert result == common_parent_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), common_current=False, common_parent=True)
-		assert result == common_parent_expected_gpath
+		result = GPath.find_common(path1, path2, allow_current=False, allow_parents=True)
+		assert result == allow_parents_expected_gpath
+		result = GPath.find_common(path2, path1, allow_current=False, allow_parents=True)
+		assert result == allow_parents_expected_gpath
+
+		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=False, allow_parents=True)
+		assert result == allow_parents_expected_gpath
+		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=False, allow_parents=True)
+		assert result == allow_parents_expected_gpath
 
-		if common_current_parent_expected is not None:
-			common_current_parent_expected_gpath = GPath(common_current_parent_expected)
+		if allow_current_parent_expected is not None:
+			allow_current_parent_expected_gpath = GPath(allow_current_parent_expected)
 		else:
-			common_current_parent_expected_gpath = None
+			allow_current_parent_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, common_current=True, common_parent=True)
-		assert result == common_current_parent_expected_gpath
-		result = GPath.find_common(path2, path1, common_current=True, common_parent=True)
-		assert result == common_current_parent_expected_gpath
-
-		result = GPath.find_common(GPath(path1), GPath(path2), common_current=True, common_parent=True)
-		assert result == common_current_parent_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), common_current=True, common_parent=True)
-		assert result == common_current_parent_expected_gpath
+		result = GPath.find_common(path1, path2, allow_current=True, allow_parents=True)
+		assert result == allow_current_parent_expected_gpath
+		result = GPath.find_common(path2, path1, allow_current=True, allow_parents=True)
+		assert result == allow_current_parent_expected_gpath
+
+		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=True, allow_parents=True)
+		assert result == allow_current_parent_expected_gpath
+		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=True, allow_parents=True)
+		assert result == allow_current_parent_expected_gpath
 
 		if no_common_expected is not None:
 			no_common_expected_gpath = GPath(no_common_expected)
 		else:
 			no_common_expected_gpath = None
 
-		result = GPath.find_common(path1, path2, common_current=False, common_parent=False)
+		result = GPath.find_common(path1, path2, allow_current=False, allow_parents=False)
 		assert result == no_common_expected_gpath
-		result = GPath.find_common(path2, path1, common_current=False, common_parent=False)
+		result = GPath.find_common(path2, path1, allow_current=False, allow_parents=False)
 		assert result == no_common_expected_gpath
 
-		result = GPath.find_common(GPath(path1), GPath(path2), common_current=False, common_parent=False)
+		result = GPath.find_common(GPath(path1), GPath(path2), allow_current=False, allow_parents=False)
 		assert result == no_common_expected_gpath
-		result = GPath.find_common(GPath(path2), GPath(path1), common_current=False, common_parent=False)
+		result = GPath.find_common(GPath(path2), GPath(path1), allow_current=False, allow_parents=False)
 		assert result == no_common_expected_gpath
 
 
 
 	@pytest.mark.parametrize(
-		('paths', 'common_current', 'common_parent', 'expected'),
+		('paths', 'allow_current', 'allow_parents', 'expected'),
 		[
 			(
 				[
 					"/usr/bin",
 					"/usr/bin/python",
 					"/home/username/Documents/Secret Documents/Secret Document.txt",
 					"usr/bin",
@@ -1128,27 +1150,27 @@
 				],
 				GPath("../../usr/bin"): [
 					GPath(""),
 				],
 			}),
 		]
 	)
-	def test_partition(self, paths: list[str], common_current: bool, common_parent: bool, expected: dict[GPath, list[GPath]]):
+	def test_partition(self, paths: list[str], allow_current: bool, allow_parents: bool, expected: dict[GPath, list[GPath]]):
 		"""
 			Test `partition()`.
 		"""
-		result = GPath.partition(paths, common_current=common_current, common_parent=common_parent)
+		result = GPath.partition(paths, allow_current=allow_current, allow_parents=allow_parents)
 		assert result == expected
-		result = GPath.partition(*paths, common_current=common_current, common_parent=common_parent)
+		result = GPath.partition(*paths, allow_current=allow_current, allow_parents=allow_parents)
 		assert result == expected
 
 		gpaths = [GPath(path) for path in paths]
-		result = GPath.partition(gpaths, common_current=common_current, common_parent=common_parent)
+		result = GPath.partition(gpaths, allow_current=allow_current, allow_parents=allow_parents)
 		assert result == expected
-		result = GPath.partition(*gpaths, common_current=common_current, common_parent=common_parent)
+		result = GPath.partition(*gpaths, allow_current=allow_current, allow_parents=allow_parents)
 		assert result == expected
 
 
 	@pytest.mark.parametrize(
 		('paths', 'expected_gpath'),
 		[
 			(["", "/", "usr", "bin"], "usr/bin"),
```

