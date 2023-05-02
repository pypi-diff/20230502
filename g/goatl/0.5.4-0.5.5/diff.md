# Comparing `tmp/goatl-0.5.4.tar.gz` & `tmp/goatl-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goatl-0.5.4.tar", max compression
+gzip compressed data, was "goatl-0.5.5.tar", max compression
```

## Comparing `goatl-0.5.4.tar` & `goatl-0.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.5.4/LICENSE
--rw-r--r--   0        0        0     3735 2023-05-01 21:12:03.779858 goatl-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3714 2023-05-01 21:09:47.753862 goatl-0.5.4/README.md
--rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.5.4/src/goatl/__init__.py
--rw-r--r--   0        0        0    11718 2023-05-01 19:22:05.810863 goatl-0.5.4/src/goatl/core.py
--rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.5.4/src/goatl/utils.py
--rw-r--r--   0        0        0     4312 2023-05-01 21:12:21.445271 goatl-0.5.4/setup.py
--rw-r--r--   0        0        0     4432 2023-05-01 21:12:21.445271 goatl-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3785 2023-05-02 11:05:15.114792 goatl-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4590 2023-05-02 08:24:00.828236 goatl-0.5.5/README.md
+-rw-r--r--   0        0        0      478 2023-05-01 21:17:22.000540 goatl-0.5.5/src/goatl/__init__.py
+-rw-r--r--   0        0        0    11731 2023-05-02 10:55:02.197690 goatl-0.5.5/src/goatl/core.py
+-rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.5.5/src/goatl/utils.py
+-rw-r--r--   0        0        0     5178 2023-05-02 11:09:11.855395 goatl-0.5.5/setup.py
+-rw-r--r--   0        0        0     5326 2023-05-02 11:09:11.855395 goatl-0.5.5/PKG-INFO
```

### Comparing `goatl-0.5.4/LICENSE` & `goatl-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goatl-0.5.4/pyproject.toml` & `goatl-0.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "goatl"
-version = "0.5.4"
-description = "Greatest of all time logger"
+version = "0.5.5"
+description = "The goat logger"
 readme = "README.md"
 authors = ["goatl <EytanDn@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/EytanDn/goatl"
 homepage = "https://github.com/EytanDn/goatl"
 
 keywords = ["logging", "logger", "log", "goat", "goatl", "goatlogger", "goat-logger", "goat-logging", "goat-log"] 
@@ -17,22 +17,23 @@
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^23.3", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^1.0"
@@ -81,15 +82,15 @@
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.9
+python_version = 3.9 #currently unused
 pretty = true
 show_traceback = true
 color_output = true
 
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `goatl-0.5.4/README.md` & `goatl-0.5.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 <div align="center">
 
 [![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/EytanDn/goatl/blob/master/.pre-commit-config.yaml)
 ![Coverage Report](assets/images/coverage.svg)
 
 </div>
 
 ## Installation
 
 ```bash
@@ -37,29 +36,50 @@
 by replacing repetitive boilerplate code with a simple function call:
 the magic "log" function.
 
 ```python
 from goatl import log
 ```
 
+goatl usage is all about the log
+
+### two important core concepts
+
+In order to justify the existence of goatl,
+it must fulfill three important core concepts:
+
+1. Unobtrusive - it should not interfere\* with the existing code.
+2. Ease of use - using it should be intuitive and pythonic.
+3. Clean - the amount of code added to the existing code should be minimal.
+
+<sub>\* - logging will always carry a performative cost, goatl will aim at keeping it to a minimum.</sub>
+
+### means of achieving the core concepts
+
+extensive testing of goatl must be implemented to ensure that it does not interfere with the existing code.
+it should be tested by wrapping other popular libraries and modules with goatl.
+this will ensure that goatl does not interfere with the existing code.
+performance tests should be implemented to measure the performance cost of goatl,
+it should not exceed a reasonable threshold, in comparison to adding logging manually.
+
 ### main features
 
 the log function provides an easy interace for:
 
 - out of and in context log calls
 - wrapping existing functions with log calls
 - wrapping existing classes with log calls
+- wrapping existing modules with log calls #not implemented yet, is this even possible?
 - logging configuration #not implemented yet
+- support multiple logging backends #not implemented yet
 
 all in an intuitive and pythonic way.
 
 ## Usage
 
-goatl usage is all about the log
-
 ### as a function
 
 ```python
 log("hello world")
 # 2020-07-19 16:00:00,000 - goatl - INFO - hello world
 log.debug("hello world?")
 # 2020-07-19 16:00:00,000 - goatl - DEBUG - hello world?
@@ -130,14 +150,14 @@
 This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/eytandn/goatl/blob/master/LICENSE) for more details.
 
 ## Citation
 
 ```bibtex
 @misc{goatl,
   author = {goatl},
-  title = {Greatest of all time logger},
+  title = {goat logger},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/EytanDn/goatl}}
 }
 ```
```

### Comparing `goatl-0.5.4/src/goatl/core.py` & `goatl-0.5.5/src/goatl/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import inspect
 import functools
 from dataclasses import dataclass, field
-from typing import Any, Callable, Optional, Union, TypeVar
+from typing import Any, Callable, Optional, Union, TypeVar, Tuple, Dict
 from .utils import _wrap_and_bind, _transfer_class_meta
 
 import sys
 _logger = logging.getLogger()
 handler = logging.StreamHandler(stream=sys.stdout)
 handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
 _logger.addHandler(handler)
@@ -30,16 +30,16 @@
 DEFAULT_INIT_LEVEL = logging.INFO
 
 @dataclass
 class Log:
     level: Optional[int] = None
     message: Optional[str] = None
     
-    args: Optional[tuple] = field(default_factory=tuple)
-    kwargs: Optional[dict] = field(default_factory=dict)
+    args: Optional[Tuple] = field(default_factory=tuple)
+    kwargs: Optional[Dict] = field(default_factory=dict)
     
     logger: Optional[logging.Logger] = None
     
     def __post_init__(self):
         if isinstance(self.level, str):
             self.level = getattr(logging, self.level.upper())       
         elif self.level in log.levels:
@@ -55,15 +55,15 @@
     def __call__(self, *args, **kwargs) -> None:
         """log the message"""
         args = (*self.args, *args)
         kwargs = {**self.kwargs, **kwargs}
         self.logger.log(self.level, BraceMessage(self.message, *args, **kwargs))
     
     @staticmethod
-    def _from_kwargs(kwargs: dict, 
+    def _from_kwargs(kwargs: Dict, 
                     default_message: str, 
                     default_level: int,
                     prefix: str) -> "Log | None":
         
         message = kwargs.get(f"{prefix}_message", None)
         level = kwargs.get(f"{prefix}_level", None)
             
@@ -82,15 +82,15 @@
         if message is None and level is None:
             return None
                 
         return Log(message=message, level=level, logger=kwargs.get("logger", None))
     
 @dataclass
 class CallLogParams:
-    kwargs: Optional[dict] = field(default_factory=dict)
+    kwargs: Optional[Dict] = field(default_factory=dict)
 
     def __post_init__(self): # TODO: seperate between level, call_level, reutrn_level
         # if call_message is present use it, 
         # else use message if present, else use default
         # if call_level is present use it, else use level if present, else use default
 
         self.call_log = Log._from_kwargs(self.kwargs, 
@@ -100,15 +100,15 @@
         self.return_log = Log._from_kwargs(self.kwargs, 
                                         DEFAULT_RETURN_MESSAGE,
                                         DEFAULT_RETURN_LEVEL,
                                         prefix="return")
 
 @dataclass
 class ClassLogParams:
-    kwargs: Optional[dict] = field(default_factory=dict)
+    kwargs: Optional[Dict] = field(default_factory=dict)
 
     def __post_init__(self):
         self.method_log: Optional[CallLogParams] = CallLogParams(kwargs=self.kwargs)
         self.private_log: Optional[CallLogParams] = None
         self.property_log: Optional[CallLogParams] = None
         self.init_log: Optional[Log] = Log._from_kwargs(self.kwargs, 
                                                          DEFAULT_INIT_MESSAGE,
@@ -180,15 +180,15 @@
         return _wrap_class(wrapped, class_log_params)
     else: # TODO: maybe seperate between class kwargs and function kwargs
         call_log_params = CallLogParams(kwargs)
         return _wrap_function(wrapped, call_log_params)
 
 
 def log(magic: Union[Wrappable, Reprable]=None, /,
-        *args: Optional[tuple[Any]],
+        *args: Optional[Tuple[Any]],
         message: Optional[str]=None,
         level: Optional[int]=None,
         logger: Optional[logging.Logger]=None,
         call_message: Optional[str]=None,
         call_level: Optional[int]=None,
         return_message: Optional[str]=None,
         return_level: Optional[int]=None,
@@ -309,16 +309,16 @@
 warning: Callable = functools.partial(log, level=logging.WARNING)
 setattr(log, "warning", warning)  
 error: Callable = functools.partial(log, level=logging.ERROR)
 setattr(log, "error", error)
 critical: Callable = functools.partial(log, level=logging.CRITICAL)
 setattr(log, "critical", critical)
 
-levels: dict[Callable, int] = {
+levels: Dict[Callable, int] = {
     info: logging.INFO,
     debug: logging.DEBUG,
     warning: logging.WARNING,
     error: logging.ERROR,
     critical: logging.CRITICAL
 }
 
-log.levels: dict[Callable, int] = levels
+log.levels: Dict[Callable, int] = levels
```

### Comparing `goatl-0.5.4/src/goatl/utils.py` & `goatl-0.5.5/src/goatl/utils.py`

 * *Files identical despite different names*

### Comparing `goatl-0.5.4/PKG-INFO` & `goatl-0.5.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: goatl
-Version: 0.5.4
-Summary: Greatest of all time logger
+Version: 0.5.5
+Summary: The goat logger
 Home-page: https://github.com/EytanDn/goatl
 License: MIT
 Keywords: logging,logger,log,goat,goatl,goatlogger,goat-logger,goat-logging,goat-log
 Author: goatl
 Author-email: EytanDn@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/EytanDn/goatl
 Description-Content-Type: text/markdown
 
 # goatl
 
@@ -32,15 +33,14 @@
 <div align="center">
 
 [![Build status](https://github.com/EytanDn/goatl/workflows/build/badge.svg?branch=master&event=push)](https://github.com/EytanDn/goatl/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/goatl.svg)](https://pypi.org/project/goatl/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/EytanDn/goatl/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/EytanDn/goatl/blob/master/.pre-commit-config.yaml)
 ![Coverage Report](assets/images/coverage.svg)
 
 </div>
 
 ## Installation
 
 ```bash
@@ -59,29 +59,50 @@
 by replacing repetitive boilerplate code with a simple function call:
 the magic "log" function.
 
 ```python
 from goatl import log
 ```
 
+goatl usage is all about the log
+
+### two important core concepts
+
+In order to justify the existence of goatl,
+it must fulfill three important core concepts:
+
+1. Unobtrusive - it should not interfere\* with the existing code.
+2. Ease of use - using it should be intuitive and pythonic.
+3. Clean - the amount of code added to the existing code should be minimal.
+
+<sub>\* - logging will always carry a performative cost, goatl will aim at keeping it to a minimum.</sub>
+
+### means of achieving the core concepts
+
+extensive testing of goatl must be implemented to ensure that it does not interfere with the existing code.
+it should be tested by wrapping other popular libraries and modules with goatl.
+this will ensure that goatl does not interfere with the existing code.
+performance tests should be implemented to measure the performance cost of goatl,
+it should not exceed a reasonable threshold, in comparison to adding logging manually.
+
 ### main features
 
 the log function provides an easy interace for:
 
 - out of and in context log calls
 - wrapping existing functions with log calls
 - wrapping existing classes with log calls
+- wrapping existing modules with log calls #not implemented yet, is this even possible?
 - logging configuration #not implemented yet
+- support multiple logging backends #not implemented yet
 
 all in an intuitive and pythonic way.
 
 ## Usage
 
-goatl usage is all about the log
-
 ### as a function
 
 ```python
 log("hello world")
 # 2020-07-19 16:00:00,000 - goatl - INFO - hello world
 log.debug("hello world?")
 # 2020-07-19 16:00:00,000 - goatl - DEBUG - hello world?
@@ -152,15 +173,15 @@
 This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/eytandn/goatl/blob/master/LICENSE) for more details.
 
 ## Citation
 
 ```bibtex
 @misc{goatl,
   author = {goatl},
-  title = {Greatest of all time logger},
+  title = {goat logger},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/EytanDn/goatl}}
 }
 ```
```

