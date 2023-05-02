# Comparing `tmp/nwa-stdlib-1.4.6.tar.gz` & `tmp/nwa-stdlib-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwa-stdlib-1.4.6.tar", last modified: Tue Mar 14 08:38:28 2023, max compression
+gzip compressed data, was "nwa-stdlib-1.4.7.tar", last modified: Tue May  2 08:30:58 2023, max compression
```

## Comparing `nwa-stdlib-1.4.6.tar` & `nwa-stdlib-1.4.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      363 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.github/workflows/publish-release.yaml
--rw-r--r--   0        0        0     1895 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0      800 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.github/workflows/test-package.yaml
--rw-r--r--   0        0        0     1111 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.gitignore
--rw-r--r--   0        0        0     2110 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/.stignore
--rw-r--r--   0        0        0    11381 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/LICENSE
--rw-r--r--   0        0        0      109 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/NOTICE
--rw-r--r--   0        0        0      718 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/README.md
--rw-r--r--   0        0        0     1580 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_json.py
--rw-r--r--   0        0        0     1724 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_orjson.py
--rw-r--r--   0        0        0     1287 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_pickle.py
--rw-r--r--   0        0        0      985 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/benchmarks/shared.py
--rw-r--r--   0        0        0     2399 2023-03-14 08:38:24.210989 nwa-stdlib-1.4.6/docs/debugging.md
--rw-r--r--   0        0        0      709 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/__init__.py
--rw-r--r--   0        0        0     2596 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/asyncio.py
--rw-r--r--   0        0        0     8069 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/asyncio_cache.py
--rw-r--r--   0        0        0     1796 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/debugging.py
--rw-r--r--   0        0        0     1134 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/ex.py
--rw-r--r--   0        0        0     1096 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/f.py
--rw-r--r--   0        0        0     4224 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/logging.py
--rw-r--r--   0        0        0        0 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/py.typed
--rw-r--r--   0        0        0      803 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/settings.py
--rw-r--r--   0        0        0     3239 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/url.py
--rw-r--r--   0        0        0     1240 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/nwastdlib/version.py
--rw-r--r--   0        0        0     2141 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/pyproject.toml
--rw-r--r--   0        0        0       35 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/requirements/all.txt
--rw-r--r--   0        0        0       78 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/requirements/base.txt
--rw-r--r--   0        0        0       36 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/requirements/dev.txt
--rw-r--r--   0        0        0      306 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/requirements/test.txt
--rw-r--r--   0        0        0     1108 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/tests/__init__.py
--rw-r--r--   0        0        0     1311 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/tests/test_asyncio.py
--rw-r--r--   0        0        0     4604 2023-03-14 08:38:24.214990 nwa-stdlib-1.4.6/tests/test_asyncio_cache.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 nwa-stdlib-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-05-02 08:30:51.328867 nwa-stdlib-1.4.7/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-05-02 08:30:51.328867 nwa-stdlib-1.4.7/.github/workflows/publish-release.yaml
+-rw-r--r--   0        0        0     1895 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0      807 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.github/workflows/test-package.yaml
+-rw-r--r--   0        0        0     1111 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.gitignore
+-rw-r--r--   0        0        0     2130 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/.stignore
+-rw-r--r--   0        0        0    11381 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/LICENSE
+-rw-r--r--   0        0        0      109 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/NOTICE
+-rw-r--r--   0        0        0     1420 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/README.md
+-rw-r--r--   0        0        0     1580 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_json.py
+-rw-r--r--   0        0        0     1724 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_orjson.py
+-rw-r--r--   0        0        0     1287 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_pickle.py
+-rw-r--r--   0        0        0      985 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/benchmarks/shared.py
+-rw-r--r--   0        0        0     2399 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/docs/debugging.md
+-rw-r--r--   0        0        0      709 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/__init__.py
+-rw-r--r--   0        0        0     2609 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/asyncio.py
+-rw-r--r--   0        0        0     8098 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/asyncio_cache.py
+-rw-r--r--   0        0        0     1796 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/debugging.py
+-rw-r--r--   0        0        0     1165 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/ex.py
+-rw-r--r--   0        0        0     1096 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/f.py
+-rw-r--r--   0        0        0     4237 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/logging.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/py.typed
+-rw-r--r--   0        0        0      803 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/settings.py
+-rw-r--r--   0        0        0     3239 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/url.py
+-rw-r--r--   0        0        0     1271 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/nwastdlib/version.py
+-rw-r--r--   0        0        0     2233 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/all.txt
+-rw-r--r--   0        0        0       78 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/base.txt
+-rw-r--r--   0        0        0       36 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/dev.txt
+-rw-r--r--   0        0        0      306 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/requirements/test.txt
+-rw-r--r--   0        0        0     1108 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     1311 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/test_asyncio.py
+-rw-r--r--   0        0        0     4730 2023-05-02 08:30:51.332867 nwa-stdlib-1.4.7/tests/test_asyncio_cache.py
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 nwa-stdlib-1.4.7/PKG-INFO
```

### Comparing `nwa-stdlib-1.4.6/.github/workflows/publish-release.yaml` & `nwa-stdlib-1.4.7/.github/workflows/publish-release.yaml`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/.github/workflows/scheduled-build.yml` & `nwa-stdlib-1.4.7/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/.github/workflows/test-package.yaml` & `nwa-stdlib-1.4.7/.github/workflows/test-package.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11"]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `nwa-stdlib-1.4.6/.gitignore` & `nwa-stdlib-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/.pre-commit-config.yaml` & `nwa-stdlib-1.4.7/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.2.2
     hooks:
       - id: pyupgrade
         args:
-          - --py310-plus
+          - --py39-plus
           - --keep-runtime-typing
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.10
+        language_version: python3.9
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.1.0]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
         exclude: (charts/*|.gitlab-ci.yml)
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: detect-private-key
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-bandit
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-docstrings
@@ -45,33 +45,34 @@
           - flake8-pep3101
           - flake8-print
           - flake8-rst
           - flake8-rst-docstrings
           - flake8-tidy-imports
           - pygments
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
       - id: mypy
-        language_version: python310
+        language_version: python39
         additional_dependencies:
           - pydantic
           - types-pytz
+          - types-redis
         args:
           - --no-warn-unused-ignores
           - --allow-untyped-decorators
         exclude: (test/*|migrations/*)
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-use-type-annotations
       - id: python-check-mock-methods
       - id: rst-backticks
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.8.0.4
+    rev: v0.9.0.2
     hooks:
       - id: shellcheck
   - repo: https://github.com/andreoliwa/nitpick
-    rev: v0.32.0
+    rev: v0.33.1
     hooks:
       - id: nitpick
```

### Comparing `nwa-stdlib-1.4.6/.stignore` & `nwa-stdlib-1.4.7/.stignore`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/LICENSE` & `nwa-stdlib-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_json.py` & `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_json.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_orjson.py` & `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_orjson.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/benchmarks/benchmark_async_cache_with_pickle.py` & `nwa-stdlib-1.4.7/benchmarks/benchmark_async_cache_with_pickle.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/benchmarks/shared.py` & `nwa-stdlib-1.4.7/benchmarks/shared.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/docs/debugging.md` & `nwa-stdlib-1.4.7/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/nwastdlib/__init__.py` & `nwa-stdlib-1.4.7/nwastdlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """The NWA-stdlib module."""
 
-__version__ = "1.4.6"
+__version__ = "1.4.7"
 
 from nwastdlib.f import const, identity
 
 __all__ = ["const", "identity"]
```

### Comparing `nwa-stdlib-1.4.6/nwastdlib/asyncio.py` & `nwa-stdlib-1.4.7/nwastdlib/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 import warnings
 from collections.abc import Awaitable, Callable, Iterable
-from typing import TypeVar
+from typing import TypeVar, Union
 
 A = TypeVar("A")
 R = TypeVar("R")
 
 try:
     from anyio import CapacityLimiter, to_thread
 except ImportError:
@@ -41,15 +41,15 @@
             def my_function_2(arg1, arg2):
                 ...
 
             await gather_nice_sync(my_function_2, [("arg10", "arg11"), ("arg20", "arg21")])
 
         """
 
-        def make_args(func_args: Iterable | object) -> Iterable:
+        def make_args(func_args: Union[Iterable, object]) -> Iterable:
             # When one argument is passed, wrap it in a list so run_sync can unpack it again
             if not isinstance(func_args, (tuple, list, set)):
                 return [func_args]
             return func_args
 
         limiter = CapacityLimiter(limit)
         tasks = [to_thread.run_sync(function, *make_args(arg), limiter=limiter) for arg in args]
```

### Comparing `nwa-stdlib-1.4.6/nwastdlib/asyncio_cache.py` & `nwa-stdlib-1.4.7/nwastdlib/asyncio_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  limitations under the License.
 #
 import hashlib
 import hmac
 import pickle  # noqa S403
 import sys
 from functools import wraps
-from typing import Any, Callable, Protocol, runtime_checkable
+from typing import Any, Callable, Protocol, Union, runtime_checkable
 
 import structlog
 from redis.asyncio import Redis as AIORedis
 
 logger = structlog.get_logger(__name__)
 
 
@@ -41,30 +41,30 @@
     """Implementation of the default protocol that uses pickle."""
 
     @staticmethod
     def deserialize(data: Any) -> Any:
         return pickle.loads(data)  # noqa S403
 
     @staticmethod
-    def serialize(data: bytes | bytearray | str) -> Any:
+    def serialize(data: Union[bytes, bytearray, str]) -> Any:
         return pickle.dumps(data)  # noqa S403
 
 
 def _deserialize(data: Any, serializer: SerializerProtocol) -> Any:
     try:
         data = serializer.deserialize(data)
     except Exception as e:
         logger.error(
             "Cache deserialization failed, returning None, so cache will be overwritten with a new value", error=e
         )
         return None
     return data
 
 
-def get_hmac_checksum(secret: str, message: bytes | bytearray | str) -> str:
+def get_hmac_checksum(secret: str, message: Union[bytes, bytearray, str]) -> str:
     if isinstance(message, str):
         message = message.encode()
     h = hmac.new(secret.encode(), message, hashlib.sha512)
     return h.hexdigest()
 
 
 async def set_cache_value(
@@ -111,16 +111,16 @@
         return None
     return _deserialize(pickled_value, serializer)
 
 
 def cached_result(
     pool: AIORedis,
     prefix: str,
-    secret: str | None,
-    key_name: str | None = None,
+    secret: Union[str, None],
+    key_name: Union[str, None] = None,
     expiry_seconds: int = 120,
     serializer: SerializerProtocol = DefaultSerializer,
 ) -> Callable:
     """Pass returned result objects from a async function call into redis.
 
     Returns a decorator function that will cache every result of a function to redis. This only works
     for functions with string, int or UUID arguments and result objects that can be serialized by the
```

### Comparing `nwa-stdlib-1.4.6/nwastdlib/debugging.py` & `nwa-stdlib-1.4.7/nwastdlib/debugging.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/nwastdlib/ex.py` & `nwa-stdlib-1.4.7/nwastdlib/ex.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 #  limitations under the License.
 #
 
 """Module containing functions to deal with `Exception`s."""
 
 
 import traceback
+from typing import Union
 
 
-def show_ex(ex: Exception, stacklimit: int | None = None) -> str:
+def show_ex(ex: Exception, stacklimit: Union[int, None] = None) -> str:
     """
     Show an exception, including its class name, message and (limited) stacktrace.
 
     >>> try:
     ...     raise Exception("Something went wrong")
     ... except Exception as e:
     ...     print(show_ex(e))
```

### Comparing `nwa-stdlib-1.4.6/nwastdlib/f.py` & `nwa-stdlib-1.4.7/nwastdlib/f.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/nwastdlib/logging.py` & `nwa-stdlib-1.4.7/nwastdlib/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging.config
 import os
-from typing import Any
+from typing import Any, Union
 
 import structlog
 
 pre_chain = [
     structlog.contextvars.merge_contextvars,
     # Add the log level and a timestamp to the event_dict if the log entry
     # is not from structlog.
@@ -59,15 +59,15 @@
         "error_console": {"class": "logging.StreamHandler", "formatter": LOG_OUTPUT},
         "console": {"class": "logging.StreamHandler", "formatter": LOG_OUTPUT},
         "gunicorn.error": {"class": "logging.StreamHandler", "formatter": LOG_OUTPUT},
     },
 }
 
 
-def initialise_logging(additional_loggers: dict[str, dict[str, Any]] | None = None) -> None:
+def initialise_logging(additional_loggers: Union[dict[str, dict[str, Any]], None] = None) -> None:
     """
     Initialise the StructLog logging setup.
 
     An example of the additional_loggers format:
 
     additional_logging = {
         "zeep.transports": {  # set to debug to see XML in loggging
```

### Comparing `nwa-stdlib-1.4.6/nwastdlib/settings.py` & `nwa-stdlib-1.4.7/nwastdlib/settings.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/nwastdlib/url.py` & `nwa-stdlib-1.4.7/nwastdlib/url.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/nwastdlib/version.py` & `nwa-stdlib-1.4.7/nwastdlib/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from subprocess import check_output  # noqa: S404
+from typing import Union
 
 import structlog
 
 logger = structlog.getLogger(__name__)
 
 
-def __getattr__(name: str) -> str | None:
+def __getattr__(name: str) -> Union[str, None]:
     """
     Return the GIT_COMMIT_HASH.
 
     Usage::
 
         from server.version import GIT_COMMIT_HASH
         print(GIT_COMMIT_HASH)
```

### Comparing `nwa-stdlib-1.4.6/pyproject.toml` & `nwa-stdlib-1.4.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,23 +21,25 @@
     "Typing :: Typed",
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
 ]
 requires = [
     "structlog~=22.1.0",
     "colorama~=0.4.3",
     "redis~=4.4.2"
 ]
 description-file = "README.md"
-requires-python = ">3.9"
+requires-python = ">=3.9"
 
 [tool.flit.metadata.urls]
 Documentation = "https://workfloworchestrator.org/"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "anyio",
```

### Comparing `nwa-stdlib-1.4.6/setup.cfg` & `nwa-stdlib-1.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/tests/test_asyncio.py` & `nwa-stdlib-1.4.7/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `nwa-stdlib-1.4.6/tests/test_asyncio_cache.py` & `nwa-stdlib-1.4.7/tests/test_asyncio_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import json
 import sys
 from copy import copy
 
+import pytest
 from fakeredis.aioredis import FakeRedis
 
 from nwastdlib.asyncio_cache import cached_result
 
 
+@pytest.fixture(autouse=True)
+async def clear_fake_redis():
+    redis = FakeRedis()
+    await redis.flushdb()
+
+
 class JsonSerializer:
     """A class that implements a simple JSON serializer/deserializer."""
 
     @staticmethod
     def deserialize(data):
         return json.loads(data)
```

