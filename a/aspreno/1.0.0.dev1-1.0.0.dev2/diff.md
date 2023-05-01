# Comparing `tmp/aspreno-1.0.0.dev1.tar.gz` & `tmp/aspreno-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspreno-1.0.0.dev1.tar", max compression
+gzip compressed data, was "aspreno-1.0.0.dev2.tar", max compression
```

## Comparing `aspreno-1.0.0.dev1.tar` & `aspreno-1.0.0.dev2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      993 2023-04-29 23:47:13.880460 aspreno-1.0.0.dev1/aspreno/__init__.py
--rw-r--r--   0        0        0      265 2023-04-23 18:27:59.801769 aspreno-1.0.0.dev1/aspreno/_utils.py
--rw-r--r--   0        0        0     7596 2023-04-30 10:45:13.094958 aspreno-1.0.0.dev1/aspreno/global_handler.py
--rw-r--r--   0        0        0        0 2023-04-19 15:21:20.492325 aspreno-1.0.0.dev1/aspreno/py.typed
--rw-r--r--   0        0        0     1091 2023-04-15 00:33:39.364826 aspreno-1.0.0.dev1/LICENSE
--rw-r--r--   0        0        0     1049 2023-04-30 10:44:33.497121 aspreno-1.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      924 2023-04-18 18:31:30.978362 aspreno-1.0.0.dev1/README.md
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 aspreno-1.0.0.dev1/setup.py
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 aspreno-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      993 2023-04-29 23:47:13.880460 aspreno-1.0.0.dev2/aspreno/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-01 21:48:05.499218 aspreno-1.0.0.dev2/aspreno/_utils.py
+-rw-r--r--   0        0        0     7718 2023-05-01 21:46:56.266697 aspreno-1.0.0.dev2/aspreno/global_handler.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:21:20.492325 aspreno-1.0.0.dev2/aspreno/py.typed
+-rw-r--r--   0        0        0     1091 2023-04-15 00:33:39.364826 aspreno-1.0.0.dev2/LICENSE
+-rw-r--r--   0        0        0     1425 2023-05-01 21:52:02.486846 aspreno-1.0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-04-18 18:31:30.978362 aspreno-1.0.0.dev2/README.md
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 aspreno-1.0.0.dev2/setup.py
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 aspreno-1.0.0.dev2/PKG-INFO
```

### Comparing `aspreno-1.0.0.dev1/aspreno/__init__.py` & `aspreno-1.0.0.dev2/aspreno/__init__.py`

 * *Files identical despite different names*

### Comparing `aspreno-1.0.0.dev1/aspreno/global_handler.py` & `aspreno-1.0.0.dev2/aspreno/global_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,50 +12,50 @@
 
 class ArgumentedException(Exception):
     """
     This class is the same as the builtin Exception class in Python, however, it allows keyword
     arguments to feed "handle" methods with arguments.
     """
 
-    additional_args: dict[str, typing.Any]
+    additional_args: typing.Dict[str, typing.Any]
 
     def __init__(self, *args: object, **kwargs: typing.Any) -> None:
         self.additional_args = kwargs
         super().__init__(*args)
 
-    def get_kwargs_for_handle(self) -> dict[str, typing.Any]:
+    def get_kwargs_for_handle(self) -> typing.Dict[str, typing.Any]:
         return self.get_kwargs_for_method(getattr(self, "handle"))
 
-    def get_kwargs_for_report(self) -> dict[str, typing.Any]:
+    def get_kwargs_for_report(self) -> typing.Dict[str, typing.Any]:
         return self.get_kwargs_for_method(getattr(self, "report"))
 
     def get_kwargs_for_method(
         self, method: typing.Callable[..., typing.Any]
-    ) -> dict[str, typing.Any]:
+    ) -> typing.Dict[str, typing.Any]:
         method_signature = signature(method)
 
-        kwargs: dict[str, typing.Any] = {
+        kwargs: typing.Dict[str, typing.Any] = {
             argument_name: self.additional_args[argument_name]
             for argument_name in method_signature.parameters
             if argument_name in self.additional_args
         }
 
         return kwargs
 
 
 class ExceptionHandler:
-    ignore_errors: list[type[BaseException]] = []
+    ignore_errors: typing.List[typing.Type[BaseException]] = []
     """
     A list of exceptions to ignore.
     If an exception has been set to be ignored, the "handle" method will not be called.
     """
 
-    old_excepthook: TYPE_EXCEPTHOOK | None = None
+    old_excepthook: typing.Optional[TYPE_EXCEPTHOOK] = None
 
-    _last_exception: type[BaseException] | None = None
+    _last_exception: typing.Optional[typing.Type[BaseException]] = None
     """
     Store the last exception that has been received.
 
     .. warning::
        Because the last exception has been received, it does not mean it has been handled.
     """
 
@@ -70,17 +70,17 @@
         bool
             True if the error should be reported, or False if not.
         """
         return self._last_exception not in self.ignore_errors
 
     def _global_handler(
         self,
-        error_type: type[BaseException],
+        error_type: typing.Type[BaseException],
         value: BaseException,
-        traceback: types.TracebackType | None,
+        traceback: typing.Optional[types.TracebackType],
     ) -> None:
         _log.debug(f"Received new error: {error_type}")
         self._last_exception = error_type
         if error_type in self.ignore_errors:
             _log.debug("Ignoring, error has been set to be ignored.")
             return
 
@@ -102,15 +102,16 @@
         if exceptions_info[0] is None:
             raise RuntimeError("No exceptions have been caught.")
 
         self._global_handler(*exceptions_info)
 
     def handle(
         self, error: BaseException, **kwargs: typing.Any
-    ) -> typing.Coroutine[None, None, None] | None:
+    ) -> typing.Optional[typing.Coroutine[None, None, None]]:
+        # sourcery skip: dict-assign-update-to-union
         """
         Handles an exception.
 
         Parameters
         ----------
         error : BaseException
             The exception that was raised.
@@ -123,29 +124,27 @@
             If the handle method is async, a coroutine is returned.
         """
         _log.debug(
             f"{error.__class__.__name__} is being treated by the default's Aspreno handler."
         )
         handled = False
 
-        kwargs |= {"error": error}
-
         # Attempt to call "handle" if available
         if hasattr(error, "handle"):
             _log.info(f"{error.__class__.__name__} has defined handle, letting it self-handle.")
             handle_kwargs = kwargs.copy()
 
             # Detect if the raised exception is an argumented exception.
             if isinstance(error, ArgumentedException):
                 _log.debug("This is an ArgumentedException, obtaining additional kwargs.")
                 # Obtain kwargs for the handle method.
                 additional_kwargs = error.get_kwargs_for_handle()
 
                 # Merge kwargs together
-                handle_kwargs |= additional_kwargs.copy()
+                handle_kwargs.update(additional_kwargs)
 
             try:
                 _log.debug("Final kwargs for handle: %s", handle_kwargs)
                 if iscoroutinefunction(error.handle):
                     event_loop = asyncio.get_running_loop()
                     event_loop.create_task(error.handle(**handle_kwargs))
                 else:
@@ -178,15 +177,15 @@
             _log.info(f"{error.__class__.__name__} has defined report, letting it report.")
 
             report_kwargs = kwargs.copy()
             if isinstance(error, ArgumentedException):
                 _log.debug("This is an ArgumentedException, obtaining additional kwargs.")
                 additional_kwargs = error.get_kwargs_for_report()
 
-                report_kwargs |= additional_kwargs
+                report_kwargs.update(additional_kwargs)
 
             try:
                 _log.debug("Final kwargs for report: %s", report_kwargs)
                 if iscoroutinefunction(error.report):
                     loop = asyncio.get_running_loop()
                     loop.create_task(error.report(**report_kwargs))
                 else:
```

### Comparing `aspreno-1.0.0.dev1/LICENSE` & `aspreno-1.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `aspreno-1.0.0.dev1/pyproject.toml` & `aspreno-1.0.0.dev2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -3,37 +3,44 @@
 
 [tool.isort]
 profile = "black"
 line_length = 99
 
 [tool.poetry]
 name = "aspreno"
-version = "1.0.0dev1"
-description = ""
+version = "1.0.0dev2"
+description = "Exception handler/reporter for exception & global exception handle using Python class"
 authors = ["Predeactor <pro.julien.mauroy@gmail.com>"]
+maintainers = ["Predeactor <pro.julien.mauroy@gmail.com>"]
+repository = "https://github.com/Predeactor/Aspreno"
+documentation = "https://aspreno.readthedocs.org"
+license = "MIT"
 readme = "README.md"
+include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 sphinx = {version = "^6.1.3", optional = true}
 insegel = {version = "^1.3.1", optional = true}
 sphinxcontrib-fulltoc = {version = "^1.2.0", optional = true}
+typing-extensions = {version = "^4.5.0", python = "<=3.9"}
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.8"
 mypy = "^1.1.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pytest-html = "^3.2.0"
 coverage = "^7.2.2"
 pytest-pretty = "^1.2.0"
 pre-commit = "^3.2.2"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
+tox-gh-actions = "^3.1.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 insegel = "^1.3.1"
```

### Comparing `aspreno-1.0.0.dev1/README.md` & `aspreno-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `aspreno-1.0.0.dev1/setup.py` & `aspreno-1.0.0.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 packages = \
 ['aspreno']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{'docs': ['sphinx>=6.1.3,<7.0.0',
+{':python_full_version <= "3.9.0"': ['typing-extensions>=4.5.0,<5.0.0'],
+ 'docs': ['sphinx>=6.1.3,<7.0.0',
           'insegel>=1.3.1,<2.0.0',
           'sphinxcontrib-fulltoc>=1.2.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'aspreno',
-    'version': '1.0.0.dev1',
-    'description': '',
+    'version': '1.0.0.dev2',
+    'description': 'Exception handler/reporter for exception & global exception handle using Python class',
     'long_description': '# Aspreno\n\n<div align="center">\n    <!-- License -->\n    <a href="https://github.com/Predeactor/Aspreno/blob/main/README.md">\n        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/aspreno">\n    </a>\n    <!-- Version -->\n    <a href="https://pypi.org/project/aspreno">\n        <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/aspreno">\n    </a>\n    <!-- Supported Python version -->\n    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/aspreno">\n    <!-- Codecov -->\n    <a href="https://codecov.io/github/Predeactor/Aspreno" >\n        <img alt="Codecov report" src="https://codecov.io/github/Predeactor/Aspreno/branch/main/graph/badge.svg?token=YTLWE8VQYM"/>\n    </a>\n</div>\n\nPython 3 global error handling & self-handling exceptions.\n\n## Features\n\n- Global exception handling\n- Self-handleable exceptions\n- Able to report specific exceptions\n',
     'author': 'Predeactor',
     'author_email': 'pro.julien.mauroy@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'maintainer': 'Predeactor',
+    'maintainer_email': 'pro.julien.mauroy@gmail.com',
+    'url': 'https://github.com/Predeactor/Aspreno',
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['aspreno']
-package_data = \ {'': ['*']} extras_require = \ {'docs':
-['sphinx>=6.1.3,<7.0.0', 'insegel>=1.3.1,<2.0.0', 'sphinxcontrib-
-fulltoc>=1.2.0,<2.0.0']} setup_kwargs = { 'name': 'aspreno', 'version':
-'1.0.0.dev1', 'description': '', 'long_description': '# Aspreno\n\n
+package_data = \ {'': ['*']} extras_require = \ {':python_full_version <=
+"3.9.0"': ['typing-extensions>=4.5.0,<5.0.0'], 'docs': ['sphinx>=6.1.3,<7.0.0',
+'insegel>=1.3.1,<2.0.0', 'sphinxcontrib-fulltoc>=1.2.0,<2.0.0']} setup_kwargs =
+{ 'name': 'aspreno', 'version': '1.0.0.dev2', 'description': 'Exception
+handler/reporter for exception & global exception handle using Python class',
+'long_description': '# Aspreno\n\n
   \n \n \n_[PyPI_-_License]\n\n \n \n_[PyPI_-_Version]\n\n \n [PyPI - Python
                      Version]\n \n \n_[Codecov_report]\n\n
 \n\nPython 3 global error handling & self-handling exceptions.\n\n##
 Features\n\n- Global exception handling\n- Self-handleable exceptions\n- Able
 to report specific exceptions\n', 'author': 'Predeactor', 'author_email':
-'pro.julien.mauroy@gmail.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'extras_require': extras_require, 'python_requires': '>=3.11,<4.0', } setup
-(**setup_kwargs)
+'pro.julien.mauroy@gmail.com', 'maintainer': 'Predeactor', 'maintainer_email':
+'pro.julien.mauroy@gmail.com', 'url': 'https://github.com/Predeactor/Aspreno',
+'packages': packages, 'package_data': package_data, 'extras_require':
+extras_require, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

