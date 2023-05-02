# Comparing `tmp/JFIO-0.0.2.tar.gz` & `tmp/JFIO-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JFIO-0.0.2.tar", last modified: Tue May  2 11:32:31 2023, max compression
+gzip compressed data, was "JFIO-1.0.0.tar", last modified: Tue May  2 12:27:59 2023, max compression
```

## Comparing `JFIO-0.0.2.tar` & `JFIO-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:32:31.643612 JFIO-0.0.2/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:32:31.643612 JFIO-0.0.2/JFIO/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:32:31.643612 JFIO-0.0.2/JFIO/ThirdParty/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-02 10:17:16.000000 JFIO-0.0.2/JFIO/ThirdParty/json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-02 10:05:00.000000 JFIO-0.0.2/JFIO/ThirdParty/pybind11_json.hpp
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      152 2023-05-02 11:29:32.000000 JFIO-0.0.2/JFIO/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:32:31.643612 JFIO-0.0.2/JFIO/write/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:19:03.000000 JFIO-0.0.2/JFIO/write/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1903 2023-05-02 11:24:46.000000 JFIO-0.0.2/JFIO/write/writeJSON2File.cpp
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:32:31.643612 JFIO-0.0.2/JFIO.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3030 2023-05-02 11:32:31.000000 JFIO-0.0.2/JFIO.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      294 2023-05-02 11:32:31.000000 JFIO-0.0.2/JFIO.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-02 11:32:31.000000 JFIO-0.0.2/JFIO.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-02 11:32:31.000000 JFIO-0.0.2/JFIO.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-0.0.2/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      105 2023-05-02 10:42:14.000000 JFIO-0.0.2/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3030 2023-05-02 11:32:31.643612 JFIO-0.0.2/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2299 2023-05-02 09:53:52.000000 JFIO-0.0.2/README.md
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      866 2023-05-02 11:32:21.000000 JFIO-0.0.2/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-02 11:32:31.643612 JFIO-0.0.2/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      554 2023-05-02 11:09:47.000000 JFIO-0.0.2/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/JFIO/
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/JFIO/ThirdParty/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)   871200 2023-05-02 10:17:16.000000 JFIO-1.0.0/JFIO/ThirdParty/json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7210 2023-05-02 10:05:00.000000 JFIO-1.0.0/JFIO/ThirdParty/pybind11_json.hpp
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      264 2023-05-02 12:25:30.000000 JFIO-1.0.0/JFIO/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/JFIO/read/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:11:30.000000 JFIO-1.0.0/JFIO/read/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      585 2023-05-02 12:11:18.000000 JFIO-1.0.0/JFIO/read/readJSONFromFile.cpp
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/JFIO/write/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-05-02 11:19:03.000000 JFIO-1.0.0/JFIO/write/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1903 2023-05-02 11:24:46.000000 JFIO-1.0.0/JFIO/write/writeJSON2File.cpp
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-02 12:27:59.381549 JFIO-1.0.0/JFIO.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3267 2023-05-02 12:27:59.000000 JFIO-1.0.0/JFIO.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      347 2023-05-02 12:27:59.000000 JFIO-1.0.0/JFIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-02 12:27:59.000000 JFIO-1.0.0/JFIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-02 12:27:59.000000 JFIO-1.0.0/JFIO.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1069 2023-05-02 09:50:08.000000 JFIO-1.0.0/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      105 2023-05-02 10:42:14.000000 JFIO-1.0.0/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3267 2023-05-02 12:27:59.381549 JFIO-1.0.0/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2523 2023-05-02 12:24:40.000000 JFIO-1.0.0/README.md
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      879 2023-05-02 12:27:03.000000 JFIO-1.0.0/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-02 12:27:59.381549 JFIO-1.0.0/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      786 2023-05-02 12:13:12.000000 JFIO-1.0.0/setup.py
```

### Comparing `JFIO-0.0.2/JFIO/ThirdParty/json.hpp` & `JFIO-1.0.0/JFIO/ThirdParty/json.hpp`

 * *Files identical despite different names*

### Comparing `JFIO-0.0.2/JFIO/ThirdParty/pybind11_json.hpp` & `JFIO-1.0.0/JFIO/ThirdParty/pybind11_json.hpp`

 * *Files identical despite different names*

### Comparing `JFIO-0.0.2/JFIO/write/writeJSON2File.cpp` & `JFIO-1.0.0/JFIO/write/writeJSON2File.cpp`

 * *Files identical despite different names*

### Comparing `JFIO-0.0.2/JFIO.egg-info/PKG-INFO` & `JFIO-1.0.0/JFIO.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 0.0.2
+Version: 1.0.0
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JFIO - Json Fast Input Output
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)](https://www.python.org/downloads/)
@@ -36,23 +36,23 @@
 - C++ compiler with support for C++11 or later
 - Python 3.6 or later
 - [pybind11](https://github.com/pybind/pybind11)
 
 ### Install using pip
 
 ```bash
-pip install jfio
+pip install JFIO
 ```
 
 ### Build from source
 
 ```bash
 git clone git@github.com:PabloIbannez/JFIO.git
-cd jfio
-python setup.py install
+cd JFIO
+python setup.py install (or pip install .)
 ```
 
 ## Usage
 
 Here is a basic example of how to use JFIO for reading and writing JSON files:
 
 ```python
@@ -70,24 +70,25 @@
 # Reading a JSON file
 data_read = jfio.read("output.json")
 print(data_read)
 ```
 
 ## API Reference
 
-### `jfio.write(filename: str, data: Any) -> None`
+### `jfio.write(filename: str, data, formatted: bool = False)`
 
 Write JSON data to a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to write to.
-- `data` (Any): The data to write. This can be any data type that is serializable to JSON.
+- `data`: The data to write. This can be any data type that is serializable to JSON.
+- `formatted` (bool): Write JSON file in a human-readable format. Default: `False`.
 
-### `jfio.read(filename: str) -> Any`
+### `jfio.read(filename: str)`
 
 Read JSON data from a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to read from.
 
@@ -103,7 +104,8 @@
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any questions or suggestions.
 
 ## Acknowledgements
 
 - [nlohmann/json](https://github.com/nlohmann/json) for providing the powerful C++ JSON library
 - [pybind11](https://github.com/pybind/pybind11) for enabling seamless Python-C++ bindings
+- [pybind11_json](https://github.com/pybind/pybind11_json) for simplifying the integration of nlhomann/json with pybind11
```

### Comparing `JFIO-0.0.2/LICENSE` & `JFIO-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JFIO-0.0.2/PKG-INFO` & `JFIO-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: JFIO
-Version: 0.0.2
+Version: 1.0.0
 Summary: JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files.
 Home-page: https://github.com/PabloIbannez/JFIO
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JFIO - Json Fast Input Output
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)](https://www.python.org/downloads/)
@@ -36,23 +36,23 @@
 - C++ compiler with support for C++11 or later
 - Python 3.6 or later
 - [pybind11](https://github.com/pybind/pybind11)
 
 ### Install using pip
 
 ```bash
-pip install jfio
+pip install JFIO
 ```
 
 ### Build from source
 
 ```bash
 git clone git@github.com:PabloIbannez/JFIO.git
-cd jfio
-python setup.py install
+cd JFIO
+python setup.py install (or pip install .)
 ```
 
 ## Usage
 
 Here is a basic example of how to use JFIO for reading and writing JSON files:
 
 ```python
@@ -70,24 +70,25 @@
 # Reading a JSON file
 data_read = jfio.read("output.json")
 print(data_read)
 ```
 
 ## API Reference
 
-### `jfio.write(filename: str, data: Any) -> None`
+### `jfio.write(filename: str, data, formatted: bool = False)`
 
 Write JSON data to a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to write to.
-- `data` (Any): The data to write. This can be any data type that is serializable to JSON.
+- `data`: The data to write. This can be any data type that is serializable to JSON.
+- `formatted` (bool): Write JSON file in a human-readable format. Default: `False`.
 
-### `jfio.read(filename: str) -> Any`
+### `jfio.read(filename: str)`
 
 Read JSON data from a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to read from.
 
@@ -103,7 +104,8 @@
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any questions or suggestions.
 
 ## Acknowledgements
 
 - [nlohmann/json](https://github.com/nlohmann/json) for providing the powerful C++ JSON library
 - [pybind11](https://github.com/pybind/pybind11) for enabling seamless Python-C++ bindings
+- [pybind11_json](https://github.com/pybind/pybind11_json) for simplifying the integration of nlhomann/json with pybind11
```

### Comparing `JFIO-0.0.2/README.md` & `JFIO-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 - C++ compiler with support for C++11 or later
 - Python 3.6 or later
 - [pybind11](https://github.com/pybind/pybind11)
 
 ### Install using pip
 
 ```bash
-pip install jfio
+pip install JFIO
 ```
 
 ### Build from source
 
 ```bash
 git clone git@github.com:PabloIbannez/JFIO.git
-cd jfio
-python setup.py install
+cd JFIO
+python setup.py install (or pip install .)
 ```
 
 ## Usage
 
 Here is a basic example of how to use JFIO for reading and writing JSON files:
 
 ```python
@@ -52,24 +52,25 @@
 # Reading a JSON file
 data_read = jfio.read("output.json")
 print(data_read)
 ```
 
 ## API Reference
 
-### `jfio.write(filename: str, data: Any) -> None`
+### `jfio.write(filename: str, data, formatted: bool = False)`
 
 Write JSON data to a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to write to.
-- `data` (Any): The data to write. This can be any data type that is serializable to JSON.
+- `data`: The data to write. This can be any data type that is serializable to JSON.
+- `formatted` (bool): Write JSON file in a human-readable format. Default: `False`.
 
-### `jfio.read(filename: str) -> Any`
+### `jfio.read(filename: str)`
 
 Read JSON data from a file.
 
 **Arguments:**
 
 - `filename` (str): The name of the file to read from.
 
@@ -85,7 +86,8 @@
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any questions or suggestions.
 
 ## Acknowledgements
 
 - [nlohmann/json](https://github.com/nlohmann/json) for providing the powerful C++ JSON library
 - [pybind11](https://github.com/pybind/pybind11) for enabling seamless Python-C++ bindings
+- [pybind11_json](https://github.com/pybind/pybind11_json) for simplifying the integration of nlhomann/json with pybind11
```

### Comparing `JFIO-0.0.2/pyproject.toml` & `JFIO-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools-cuda-cpp", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="JFIO"
-version="0.0.2"
+version="1.0.0"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "JFIO (Json Fast Input Output) is a high-performance Python package for efficient reading and writing of JSON files."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 license = {text = "MIT License"}
 
 classifiers = [
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
 ]
```

### Comparing `JFIO-0.0.2/setup.py` & `JFIO-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 ext_modules = [
     Extension(
         'JFIO.write.writeJSON2File',
         sources=['JFIO/write/writeJSON2File.cpp'],
         include_dirs=[pybind11.get_include()],
         extra_compile_args=['-std=c++11','-O3'],
         language='c++'
-    )
+    ),
+    Extension(
+        'JFIO.read.readJSONFromFile',
+        sources=['JFIO/read/readJSONFromFile.cpp'],
+        include_dirs=[pybind11.get_include()],
+        extra_compile_args=['-std=c++11','-O3'],
+        language='c++'
+    ),
 ]
 
 setup(
     packages=find_packages(),
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     url="https://github.com/PabloIbannez/JFIO",
```

