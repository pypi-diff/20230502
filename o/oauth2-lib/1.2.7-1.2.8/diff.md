# Comparing `tmp/oauth2-lib-1.2.7.tar.gz` & `tmp/oauth2-lib-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2-lib-1.2.7.tar", last modified: Thu Apr 20 12:49:38 2023, max compression
+gzip compressed data, was "oauth2-lib-1.2.8.tar", last modified: Tue May  2 10:55:14 2023, max compression
```

## Comparing `oauth2-lib-1.2.7.tar` & `oauth2-lib-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      363 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1518 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1103 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.gitignore
--rw-r--r--   0        0        0     2066 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/LICENSE
--rw-r--r--   0        0        0     1051 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/README.md
--rwxr-xr-x   0        0        0      150 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/fmt_code.sh
--rw-r--r--   0        0        0      671 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     7652 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15285 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0        0 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/oauth2_lib/py.typed
--rw-r--r--   0        0        0     2420 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/setup.cfg
--rw-r--r--   0        0        0        0 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/__init__.py
--rw-r--r--   0        0        0      758 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/conftest.py
--rw-r--r--   0        0        0    13749 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_fastapi.py
--rw-r--r--   0        0        0     6570 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_opa_decision.py
--rw-r--r--   0        0        0      474 2023-04-20 12:49:27.734271 oauth2-lib-1.2.7/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 oauth2-lib-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1533 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1103 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.gitignore
+-rw-r--r--   0        0        0     2061 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1754 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/README.md
+-rwxr-xr-x   0        0        0      150 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/fmt_code.sh
+-rw-r--r--   0        0        0      671 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     7665 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    15379 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0        0 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/oauth2_lib/py.typed
+-rw-r--r--   0        0        0     2511 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     3273 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/conftest.py
+-rw-r--r--   0        0        0     7113 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_async_api_client.py
+-rw-r--r--   0        0        0    13734 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_fastapi.py
+-rw-r--r--   0        0        0     6570 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_opa_decision.py
+-rw-r--r--   0        0        0      474 2023-05-02 10:55:09.088606 oauth2-lib-1.2.8/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 oauth2-lib-1.2.8/PKG-INFO
```

### Comparing `oauth2-lib-1.2.7/.github/workflows/publish-release.yml` & `oauth2-lib-1.2.8/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.7/.github/workflows/scheduled-build.yml` & `oauth2-lib-1.2.8/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.7/.github/workflows/test-package.yml` & `oauth2-lib-1.2.8/.github/workflows/test-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   workflow_call:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.10']
+        python-version: ['3.9', '3.10', '3.11']
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
@@ -37,15 +37,15 @@
         run: |
           mypy -p oauth2_lib
       - name: License headers
         run: |
           apache-license-check --copyright "2019-`date +%Y` SURF" oauth2_lib
       - name: Test with pytest
         run: |
-          pytest -vvv --cov-branch --cov-fail-under=58 --cov=oauth2_lib --cov-config=.coveragerc --junitxml=report-pytest-${{ matrix.python-version }}.xml
+          pytest -vvv --cov-branch --cov-fail-under=80 --cov=oauth2_lib --cov-config=.coveragerc --junitxml=report-pytest-${{ matrix.python-version }}.xml
       - name: Upload pytest test results
         uses: actions/upload-artifact@v2
         with:
           name: pytest-results-${{ matrix.python-version }}
           path: report-pytest-${{ matrix.python-version }}.xml
         # Use always() to always run this step to publish test results when there are test failures
         if: ${{ always() }}
```

### Comparing `oauth2-lib-1.2.7/.gitignore` & `oauth2-lib-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.7/.pre-commit-config.yaml` & `oauth2-lib-1.2.8/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args:
-          - --py310-plus
+          - --py39-plus
           - --keep-runtime-typing
   - repo: https://github.com/timothycrosley/isort
     rev: 5.12.0
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
         additional_dependencies: [black==22.10.0]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
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
-    rev: 3.9.2
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-bandit==3.0.0
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-docstrings
           - flake8-logging-format
           - flake8-pep3101
           - flake8-print
           - flake8-rst
           - flake8-rst-docstrings
           - flake8-tidy-imports
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v1.2.0
     hooks:
       - id: mypy
-        language_version: python3.10
+        language_version: python3.9
         additional_dependencies: [pydantic]
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
-    rev: v0.31.0
+    rev: v0.33.1
     hooks:
       - id: nitpick
```

### Comparing `oauth2-lib-1.2.7/LICENSE` & `oauth2-lib-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.7/oauth2_lib/__init__.py` & `oauth2-lib-1.2.8/oauth2_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.2.7"
+__version__ = "1.2.8"
```

### Comparing `oauth2-lib-1.2.7/oauth2_lib/async_api_client.py` & `oauth2-lib-1.2.8/oauth2_lib/async_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import contextlib
 from asyncio import new_event_loop
 from collections.abc import Generator
 from http import HTTPStatus
-from typing import Any
+from typing import Any, Union
 
 import structlog
 import urllib3
 from authlib.integrations.base_client import BaseOAuth
 from opentelemetry import context, trace
 from opentelemetry.instrumentation.utils import http_status_to_status_code
 from opentelemetry.propagate import inject
@@ -89,15 +89,15 @@
         from fubar_client import BlahApi
 
         fac = FubarApiClient('https://api.staging.automation.surf.net/fubar')
         foo = await BlaApi(fac).get_foo_by_id(foo_id)
 
     """
 
-    _token: dict | None
+    _token: Union[dict, None]
 
     def __init__(
         self,
         oauth_client: BaseOAuth,
         oauth_client_name: str,
         oauth_active: bool,
         tracing_enabled: bool,
```

### Comparing `oauth2-lib-1.2.7/oauth2_lib/fastapi.py` & `oauth2-lib-1.2.8/oauth2_lib/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
+from collections.abc import AsyncGenerator, Coroutine, Mapping
 from http import HTTPStatus
 from json import JSONDecodeError
-from typing import Any, AsyncGenerator, Callable, Coroutine, Mapping, cast
+from typing import Any, Callable, Union, cast
 
 from fastapi.exceptions import HTTPException
 from fastapi.param_functions import Depends
 from fastapi.requests import Request
 from fastapi.security.http import HTTPBearer
 from httpx import AsyncClient, BasicAuth, NetworkError
 from pydantic import BaseModel
@@ -164,37 +165,37 @@
     OIDCUser class extends the HTTPBearer class to do extra verification.
 
     The class will act as follows:
         1. Validate the Credentials at SURFconext by calling the UserInfo endpoint
         2. When receiving an active token it will enrich the response through the database roles
     """
 
-    openid_config: OIDCConfig | None = None
+    openid_config: Union[OIDCConfig, None] = None
     openid_url: str
     resource_server_id: str
     resource_server_secret: str
     enabled: bool
 
     def __init__(
         self,
         openid_url: str,
         resource_server_id: str,
         resource_server_secret: str,
         enabled: bool = True,
         auto_error: bool = True,
-        scheme_name: str | None = None,
+        scheme_name: Union[str, None] = None,
     ):
         super().__init__(auto_error=auto_error)
         self.openid_url = openid_url
         self.resource_server_id = resource_server_id
         self.resource_server_secret = resource_server_secret
         self.enabled = enabled
         self.scheme_name = scheme_name or self.__class__.__name__
 
-    async def __call__(self, request: Request, token: str | None = None) -> OIDCUserModel | None:  # type: ignore
+    async def __call__(self, request: Request, token: Union[str, None] = None) -> Union[OIDCUserModel, None]:  # type: ignore
         """
         Return the OIDC user from OIDC introspect endpoint.
 
         This is used as a security module in Fastapi projects
 
         Args:
             request: Starlette request method.
@@ -281,21 +282,21 @@
 
 
 def opa_decision(
     opa_url: str,
     oidc_security: OIDCUser,
     enabled: bool = True,
     auto_error: bool = True,
-    opa_kwargs: Mapping[str, str] | None = None,
-) -> Callable[[Request, OIDCUserModel, AsyncClient], Coroutine[Any, Any, bool | None]]:
+    opa_kwargs: Union[Mapping[str, str], None] = None,
+) -> Callable[[Request, OIDCUserModel, AsyncClient], Coroutine[Any, Any, Union[bool, None]]]:
     async def _opa_decision(
         request: Request,
         user_info: OIDCUserModel = Depends(oidc_security),
         async_request: AsyncClient = Depends(async_client),
-    ) -> bool | None:
+    ) -> Union[bool, None]:
         """
         Check OIDCUserModel against the OPA policy.
 
         This is used as a security module in Fastapi projects
         This method will make an async call towards the Policy agent.
 
         Args:
@@ -368,20 +369,20 @@
 
 
 def opa_graphql_decision(
     opa_url: str,
     _oidc_security: OIDCUser,
     enabled: bool = True,
     auto_error: bool = True,
-    opa_kwargs: Mapping[str, str] | None = None,
-) -> Callable[[str, OIDCUserModel], Coroutine[Any, Any, bool | None]]:
+    opa_kwargs: Union[Mapping[str, str], None] = None,
+) -> Callable[[str, OIDCUserModel], Coroutine[Any, Any, Union[bool, None]]]:
     async def _opa_decision(
         path: str,
         oidc_user: OIDCUserModel = Depends(_oidc_security),
-    ) -> bool | None:
+    ) -> Union[bool, None]:
         """
         Check OIDCUserModel against the OPA policy.
 
         This is used as a security module in Graphql projects
         This method will make an async call towards the Policy agent.
 
         Args:
```

### Comparing `oauth2-lib-1.2.7/pyproject.toml` & `oauth2-lib-1.2.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     "Typing :: Typed",
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
 ]
 requires = [
     "requests>=2.19.0",
-    "ruamel.yaml~=0.16.10",
     "structlog>=20.2.0",
     "fastapi>=0.90.1",
     "opentelemetry-distro",
     "httpx[http2]==0.23.0",
     "authlib==1.0.1",
     "pydantic>=1.8.0",
 ]
 description-file = "README.md"
-requires-python = ">3.8"
+requires-python = ">=3.9"
 
 [tool.flit.metadata.urls]
 Documentation = "https://workfloworchestrator.org/"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "apache-license-check",
@@ -58,20 +58,22 @@
     "flake8-pep3101",
     "flake8-print",
     "flake8-rst",
     "flake8-rst-docstrings",
     "flake8-tidy-imports",
     "isort",
     "mypy",
+    "opentelemetry-instrumentation-urllib3",
     "pygments",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-xdist",
     "requests_mock",
+    "urllib3_mock==0.3.3",
 ]
 dev = ["bumpversion", "pre-commit"]
 
 [tool.isort]
 profile = "black"
 line_length = 120
 skip = ["src", "venv"]
```

### Comparing `oauth2-lib-1.2.7/setup.cfg` & `oauth2-lib-1.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `oauth2-lib-1.2.7/tests/test_fastapi.py` & `oauth2-lib-1.2.8/tests/test_fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     async def mock_introspect_token(client, token):
         return {"wrong_data": "wrong_data"}
 
     openid_bearer = OIDCUser("openid_url", "id", "secret", auto_error=False)
     openid_bearer.openid_config = OIDCConfig.parse_obj(discovery)
     openid_bearer.introspect_token = mock_introspect_token  # type:ignore
 
-    result = await openid_bearer(mock_request, None)  # type:ignore
+    result = await openid_bearer(mock_request, None)
 
     assert result is None
 
 
 @pytest.mark.asyncio
 async def test_OIDCUser_disabled():
     mock_request = mock.MagicMock(spec=Request)
```

### Comparing `oauth2-lib-1.2.7/tests/test_opa_decision.py` & `oauth2-lib-1.2.8/tests/test_opa_decision.py`

 * *Files identical despite different names*

