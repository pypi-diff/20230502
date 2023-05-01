# Comparing `tmp/splunk-opentelemetry-1.8.0.tar.gz` & `tmp/splunk_opentelemetry-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunk-opentelemetry-1.8.0.tar", max compression
+gzip compressed data, was "splunk_opentelemetry-1.9.1.tar", max compression
```

## Comparing `splunk-opentelemetry-1.8.0.tar` & `splunk_opentelemetry-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     7439 2022-08-25 23:03:09.184907 splunk-opentelemetry-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/LICENSE
--rw-r--r--   0        0        0     8455 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/README.md
--rw-r--r--   0        0        0     2205 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1025 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/__init__.py
--rw-r--r--   0        0        0        0 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/cmd/__init__.py
--rw-r--r--   0        0        0     2287 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/cmd/bootstrap.py
--rw-r--r--   0        0        0     2178 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/cmd/trace.py
--rw-r--r--   0        0        0      799 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/defaults.py
--rw-r--r--   0        0        0     1567 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/distro.py
--rw-r--r--   0        0        0      695 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/environment_variables.py
--rw-r--r--   0        0        0     9824 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/options.py
--rw-r--r--   0        0        0     1994 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/propagators.py
--rw-r--r--   0        0        0        0 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/py.typed
--rw-r--r--   0        0        0     1699 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/symbols.py
--rw-r--r--   0        0        0     3354 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/tracing.py
--rw-r--r--   0        0        0     1023 2022-08-25 23:03:09.188907 splunk-opentelemetry-1.8.0/splunk_otel/version.py
--rw-r--r--   0        0        0    10386 2022-08-25 23:03:35.970606 splunk-opentelemetry-1.8.0/setup.py
--rw-r--r--   0        0        0     9807 2022-08-25 23:03:35.971293 splunk-opentelemetry-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7575 2023-02-14 13:33:49.419634 splunk_opentelemetry-1.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-02-14 13:33:49.419634 splunk_opentelemetry-1.9.1/LICENSE
+-rw-r--r--   0        0        0     8440 2023-02-14 13:33:49.419634 splunk_opentelemetry-1.9.1/README.md
+-rw-r--r--   0        0        0     2129 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1025 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/cmd/__init__.py
+-rw-r--r--   0        0        0     2287 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/cmd/bootstrap.py
+-rw-r--r--   0        0        0     2178 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/cmd/trace.py
+-rw-r--r--   0        0        0      799 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/defaults.py
+-rw-r--r--   0        0        0     1567 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/distro.py
+-rw-r--r--   0        0        0      695 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/environment_variables.py
+-rw-r--r--   0        0        0     9824 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/options.py
+-rw-r--r--   0        0        0     1994 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/propagators.py
+-rw-r--r--   0        0        0        0 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/py.typed
+-rw-r--r--   0        0        0     1699 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/symbols.py
+-rw-r--r--   0        0        0     3354 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/tracing.py
+-rw-r--r--   0        0        0     1023 2023-02-14 13:33:49.423634 splunk_opentelemetry-1.9.1/splunk_otel/version.py
+-rw-r--r--   0        0        0    10377 1970-01-01 00:00:00.000000 splunk_opentelemetry-1.9.1/setup.py
+-rw-r--r--   0        0        0     9796 1970-01-01 00:00:00.000000 splunk_opentelemetry-1.9.1/PKG-INFO
```

### Comparing `splunk-opentelemetry-1.8.0/CHANGELOG.md` & `splunk_opentelemetry-1.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 ## Unreleased
 
+## 1.9.1 - 2023-02-14
+
+## 1.9.0 - 2023-02-13
+
+- Upgraded Otel dependencies to 1.15.0 and 0.36b0.  This removes support for Python 3.6.
+
 ## 1.8.0 - 2022-08-10
 
 - Upgraded Otel dependencies to 1.12.0 and 0.33b0
 - Vendored in githubrelease package
 
 ## 1.7.0 - 2022-07-14
```

### Comparing `splunk-opentelemetry-1.8.0/LICENSE` & `splunk_opentelemetry-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/README.md` & `splunk_opentelemetry-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <a href="CONTRIBUTING.md">Get Involved</a>
     &nbsp;&nbsp;&bull;&nbsp;&nbsp;
     <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html">Migrating from SignalFx Python Tracing</a>
   </strong>
 </p>
 
 <p align="center">
-  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.12.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.12.0-blueviolet?style=for-the-badge"/></a></span>
+  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.15.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.15.0-blueviolet?style=for-the-badge"/></a></span>
   <a href="https://github.com/signalfx/splunk-otel-python/releases">
     <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/signalfx/splunk-otel-python?style=for-the-badge">
   </a>
   <a href="https://pypi.org/project/splunk-opentelemetry/">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/splunk-opentelemetry?style=for-the-badge">
   </a>
   <a href="https://github.com/signalfx/gdi-specification/releases/tag/v1.0.0">
@@ -68,15 +68,15 @@
 migrate to the Splunk Distribution of OpenTelemetry Python, see [Migrate from
 the SignalFx Tracing Library for Python](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-SignalFX-Python-agent).
 
 ---
 
 ## Requirements
 
-This Splunk Distribution of OpenTelemetry requires Python 3.6 or later.
+This Splunk Distribution of OpenTelemetry requires Python 3.7 or later.
 
 ## Get started
 
 To get started, install the `splunk-opentelemetry[all]` package, run the bootstrap
 script and wrap your run command with `splunk-py-trace`.
 
 For example, if the runtime parameters were:
@@ -130,15 +130,15 @@
 available.
 
 The `OTEL_RESOURCE_ATTRIBUTES` syntax is described in detail in the
 [trace configuration](docs/advanced-config.md#trace-configuration) section.
 
 ### Supported Python Versions
 
-The instrumentation works with Python verion 3.6 or higher. Supported
+The instrumentation works with Python verion 3.7 or higher. Supported
 libraries are listed
 [here](https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation).
 
 ## Advanced Configuration
 
 For the majority of users, the [Getting Started](#get-started) section is
 all you need. Advanced configuration documentation can be found
@@ -149,27 +149,27 @@
 
 Documentation on how to manually instrument a Python application is available
 [here](https://opentelemetry.io/docs/instrumentation/python/).
 
 To extend the instrumentation with the OpenTelemetry Instrumentation for Python,
 you have to use a compatible API version.
 
-The Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.8.0</span> is compatible
+The Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.9.1</span> is compatible
 with:
 
-* OpenTelemetry API version <span class="otel-api-version">1.12.0</span>
-* OpenTelemetry SDK version <span class="otel-sdk-version">1.12.0</span>
-* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.33b0</span>
+* OpenTelemetry API version <span class="otel-api-version">1.15.0</span>
+* OpenTelemetry SDK version <span class="otel-sdk-version">1.15.0</span>
+* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.36b0</span>
 
 ## Correlating traces with logs
 
 The Splunk Distribution of OpenTelemetry Python provides a way
 to correlate traces with logs. See [Connect Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/instrumentation/connect-traces-logs.html).
 
-# License and versioning
+# License
 
 The Splunk distribution of OpenTelemetry Python Instrumentation is a
 distribution of the [OpenTelemetry Python
 project](https://github.com/open-telemetry/opentelemetry-python). It is
 released under the terms of the Apache Software License version 2.0. See [the
 license file](./LICENSE) for more details.
```

#### html2text {}

```diff
@@ -22,15 +22,15 @@
 python/configuration/advanced-python-otel-configuration.html) to support full-
 fidelity traces. If you're currently using the SignalFx Tracing Library for
 Python and want to migrate to the Splunk Distribution of OpenTelemetry Python,
 see [Migrate from the SignalFx Tracing Library for Python](https://
 docs.splunk.com/Observability/gdi/get-data-in/application/python/
 troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-
 SignalFX-Python-agent). --- ## Requirements This Splunk Distribution of
-OpenTelemetry requires Python 3.6 or later. ## Get started To get started,
+OpenTelemetry requires Python 3.7 or later. ## Get started To get started,
 install the `splunk-opentelemetry[all]` package, run the bootstrap script and
 wrap your run command with `splunk-py-trace`. For example, if the runtime
 parameters were: ``` python main.py --port=8000 ``` Then the runtime parameters
 should be updated to: ``` $ pip install splunk-opentelemetry[all] $ splunk-py-
 trace-bootstrap $ OTEL_SERVICE_NAME=my-python-app \ splunk-py-trace python
 main.py --port=8000 ``` To see the Python instrumentation in action with sample
 applications, see our [examples](https://github.com/signalfx/tracing-examples/
@@ -53,31 +53,31 @@
 version resource attribute `service.version` to specify the version of your
 instrumented application. For example: ```
 OTEL_RESOURCE_ATTRIBUTES=service.version=1.2.3 ``` The `deployment.environment`
 and `service.version` resource attributes are not strictly required, but
 recommended to be set if they are available. The `OTEL_RESOURCE_ATTRIBUTES`
 syntax is described in detail in the [trace configuration](docs/advanced-
 config.md#trace-configuration) section. ### Supported Python Versions The
-instrumentation works with Python verion 3.6 or higher. Supported libraries are
+instrumentation works with Python verion 3.7 or higher. Supported libraries are
 listed [here](https://github.com/open-telemetry/opentelemetry-python-contrib/
 tree/main/instrumentation). ## Advanced Configuration For the majority of
 users, the [Getting Started](#get-started) section is all you need. Advanced
 configuration documentation can be found [here](docs/advanced-config.md). In
 addition, special cases for instrumentation are documented [here](docs/
 instrumentation-special-cases.md). ## Manually instrument an application
 Documentation on how to manually instrument a Python application is available
 [here](https://opentelemetry.io/docs/instrumentation/python/). To extend the
 instrumentation with the OpenTelemetry Instrumentation for Python, you have to
 use a compatible API version. The Splunk Distribution of OpenTelemetry Python
-version 1.8.0 is compatible with: * OpenTelemetry API version 1.12.0 *
-OpenTelemetry SDK version 1.12.0 * OpenTelemetry Instrumentation for Python
-version 0.33b0 ## Correlating traces with logs The Splunk Distribution of
+version 1.9.1 is compatible with: * OpenTelemetry API version 1.15.0 *
+OpenTelemetry SDK version 1.15.0 * OpenTelemetry Instrumentation for Python
+version 0.36b0 ## Correlating traces with logs The Splunk Distribution of
 OpenTelemetry Python provides a way to correlate traces with logs. See [Connect
 Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-
 data-in/application/python/instrumentation/connect-traces-logs.html). # License
-and versioning The Splunk distribution of OpenTelemetry Python Instrumentation
-is a distribution of the [OpenTelemetry Python project](https://github.com/
-open-telemetry/opentelemetry-python). It is released under the terms of the
-Apache Software License version 2.0. See [the license file](./LICENSE) for more
+The Splunk distribution of OpenTelemetry Python Instrumentation is a
+distribution of the [OpenTelemetry Python project](https://github.com/open-
+telemetry/opentelemetry-python). It is released under the terms of the Apache
+Software License version 2.0. See [the license file](./LICENSE) for more
 details. >â¹ï¸  SignalFx was acquired by Splunk in October 2019. See [Splunk
 SignalFx](https://www.splunk.com/en_us/investor-relations/acquisitions/
 signalfx.html) for more information.
```

### Comparing `splunk-opentelemetry-1.8.0/pyproject.toml` & `splunk_opentelemetry-1.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splunk-opentelemetry"
-version = "1.8.0"
+version = "1.9.1"
 description = "The Splunk distribution of OpenTelemetry Python Instrumentation provides a Python agent that automatically instruments your Python application to capture and report distributed traces to SignalFx APM."
 authors = ["Splunk <splunk-oss@splunk.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "splunk_otel" },
     { include = "splunk_otel/**/*.py" },
@@ -22,22 +22,22 @@
 splk-py-trace = 'splunk_otel.cmd.trace:run_deprecated'
 splk-py-trace-bootstrap = 'splunk_otel.cmd.bootstrap:run_deprecated'
 
 [tool.poetry.plugins."opentelemetry_distro"]
 splunk_distro = "splunk_otel.distro:_SplunkDistro"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-opentelemetry-api = "1.12.0"
-opentelemetry-sdk = "1.12.0"
-opentelemetry-instrumentation = "0.33b0"
-opentelemetry-semantic-conventions = "0.33b0"
-opentelemetry-propagator-b3 = "1.12.0" 
-opentelemetry-exporter-jaeger-thrift = "1.12.0"
-opentelemetry-exporter-otlp-proto-grpc = "1.12.0"
+python = "^3.7"
+opentelemetry-api = "1.15.0"
+opentelemetry-sdk = "1.15.0"
+opentelemetry-instrumentation = "0.36b0"
+opentelemetry-semantic-conventions = "0.36b0"
+opentelemetry-propagator-b3 = "1.15.0" 
+opentelemetry-exporter-jaeger-thrift = "1.15.0"
+opentelemetry-exporter-otlp-proto-grpc = "1.15.0"
 
 [tool.poetry.extras]
 all = ["opentelemetry-propagator-b3", "opentelemetry-exporter-otlp-proto-grpc", "opentelemetry-exporter-jaeger-thrift"]
 b3 = ["opentelemetry-propagator-b3"]
 otlp = ["opentelemetry-exporter-otlp-proto-grpc"]
 jaeger = ["opentelemetry-exporter-jaeger-thrift"]
 
@@ -49,19 +49,18 @@
 pytest = "7.0.1"
 coverage = "6.1.1"
 pytest-cov = "2.12.1"
 pylint = "2.12.0"
 pylintfileheader = "0.3.2"
 pytest-docker = {version = "1.0.0", platform = "linux"}
 requests-futures = "1.0.0"
-#githubrelease = "1.5.8"
-githubrelease = {path = "./vendor/githubrelease-1.5.8-23-g067d7f1.tar.gz"}
+githubrelease = "1.5.9"
 keepachangelog = "1.0.0"
 click = "8.0.4"
-types-setuptools = "63.4.0"
+types-setuptools = "65.3.0"
 
 [tool.black]
 line-length = 90
 requires = ["poetry>=1.1.11"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/__init__.py` & `splunk_opentelemetry-1.9.1/splunk_otel/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/cmd/bootstrap.py` & `splunk_opentelemetry-1.9.1/splunk_otel/cmd/bootstrap.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/cmd/trace.py` & `splunk_opentelemetry-1.9.1/splunk_otel/cmd/trace.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/defaults.py` & `splunk_opentelemetry-1.9.1/splunk_otel/defaults.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/distro.py` & `splunk_opentelemetry-1.9.1/splunk_otel/distro.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/environment_variables.py` & `splunk_opentelemetry-1.9.1/splunk_otel/environment_variables.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/options.py` & `splunk_opentelemetry-1.9.1/splunk_otel/options.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/propagators.py` & `splunk_opentelemetry-1.9.1/splunk_otel/propagators.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/symbols.py` & `splunk_opentelemetry-1.9.1/splunk_otel/symbols.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/tracing.py` & `splunk_opentelemetry-1.9.1/splunk_otel/tracing.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/splunk_otel/version.py` & `splunk_opentelemetry-1.9.1/splunk_otel/version.py`

 * *Files identical despite different names*

### Comparing `splunk-opentelemetry-1.8.0/setup.py` & `splunk_opentelemetry-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 packages = \
 ['splunk_otel', 'splunk_otel.cmd']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['opentelemetry-api==1.12.0',
- 'opentelemetry-instrumentation==0.33b0',
- 'opentelemetry-sdk==1.12.0',
- 'opentelemetry-semantic-conventions==0.33b0']
+['opentelemetry-api==1.15.0',
+ 'opentelemetry-instrumentation==0.36b0',
+ 'opentelemetry-sdk==1.15.0',
+ 'opentelemetry-semantic-conventions==0.36b0']
 
 extras_require = \
-{':extra == "all" or extra == "b3"': ['opentelemetry-propagator-b3==1.12.0'],
- ':extra == "all" or extra == "jaeger"': ['opentelemetry-exporter-jaeger-thrift==1.12.0'],
- ':extra == "all" or extra == "otlp"': ['opentelemetry-exporter-otlp-proto-grpc==1.12.0']}
+{':extra == "all" or extra == "b3"': ['opentelemetry-propagator-b3==1.15.0'],
+ ':extra == "all" or extra == "jaeger"': ['opentelemetry-exporter-jaeger-thrift==1.15.0'],
+ ':extra == "all" or extra == "otlp"': ['opentelemetry-exporter-otlp-proto-grpc==1.15.0']}
 
 entry_points = \
 {'console_scripts': ['splk-py-trace = splunk_otel.cmd.trace:run_deprecated',
                      'splk-py-trace-bootstrap = '
                      'splunk_otel.cmd.bootstrap:run_deprecated',
                      'splunk-py-trace = splunk_otel.cmd.trace:run',
                      'splunk-py-trace-bootstrap = '
                      'splunk_otel.cmd.bootstrap:run'],
  'opentelemetry_distro': ['splunk_distro = splunk_otel.distro:_SplunkDistro']}
 
 setup_kwargs = {
     'name': 'splunk-opentelemetry',
-    'version': '1.8.0',
+    'version': '1.9.1',
     'description': 'The Splunk distribution of OpenTelemetry Python Instrumentation provides a Python agent that automatically instruments your Python application to capture and report distributed traces to SignalFx APM.',
-    'long_description': '---\n\n<p align="center">\n  <strong>\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/get-started.html">Get Started</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="CONTRIBUTING.md">Get Involved</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html">Migrating from SignalFx Python Tracing</a>\n  </strong>\n</p>\n\n<p align="center">\n  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.12.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.12.0-blueviolet?style=for-the-badge"/></a></span>\n  <a href="https://github.com/signalfx/splunk-otel-python/releases">\n    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/signalfx/splunk-otel-python?style=for-the-badge">\n  </a>\n  <a href="https://pypi.org/project/splunk-opentelemetry/">\n    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/splunk-opentelemetry?style=for-the-badge">\n  </a>\n  <a href="https://github.com/signalfx/gdi-specification/releases/tag/v1.0.0">\n    <img alt="Splunk GDI specification" src="https://img.shields.io/badge/GDI-1.0.0-blueviolet?style=for-the-badge">\n  </a>\n  <a href="https://codecov.io/gh/signalfx/splunk-otel-python">\n    <img alt="Codecov" src="https://img.shields.io/codecov/c/github/signalfx/splunk-otel-python?style=for-the-badge&token=XKXjEQKGaK">\n  </a>\n  <a href="https://github.com/signalfx/splunk-otel-python/actions?query=workflow%3ATests">\n    <img alt="Build Status" src="https://img.shields.io/github/workflow/status/signalfx/splunk-otel-python/Tests?style=for-the-badge">\n  </a>\n</p>\n\n<p align="center">\n  <strong>\n    <a href="https://github.com/signalfx/tracing-examples/tree/main/opentelemetry-tracing/opentelemetry-python-tracing">Examples</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="SECURITY.md">Security</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/README.md">Supported Libraries</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/common-python-troubleshooting.html">Troubleshooting</a>\n  </strong>\n</p>\n\n# Splunk Distribution of OpenTelemetry Python\n\nThe Splunk distribution of [OpenTelemetry\nPython](https://github.com/open-telemetry/opentelemetry-python) provides\nmultiple installable packages that automatically instrument your Python\napplication to capture and report distributed traces to Splunk APM.\nInstrumentation works by patching supported libraries at runtime with an\nOpenTelemetry-compatible tracer to capture and export trace spans.\n\nThis distribution comes with the following defaults:\n\n- [W3C tracecontext](https://www.w3.org/TR/trace-context/) and [W3C\n  baggage](https://www.w3.org/TR/baggage/) context propagation;\n  [B3](https://github.com/openzipkin/b3-propagation) can also be\n  [configured](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/configuration/advanced-python-otel-configuration.html).\n- [OTLP gRPC\n  exporter](https://opentelemetry-python.readthedocs.io/en/latest/exporter/otlp/otlp.html)\n  configured to send spans to a locally running [Splunk OpenTelemetry\n  Connector](https://github.com/signalfx/splunk-otel-collector)\n  (`http://localhost:4317`).\n- Unlimited default limits for [configuration options](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/configuration/advanced-python-otel-configuration.html) to\n  support full-fidelity traces.\n\nIf you\'re currently using the SignalFx Tracing Library for Python and want to\nmigrate to the Splunk Distribution of OpenTelemetry Python, see [Migrate from\nthe SignalFx Tracing Library for Python](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-SignalFX-Python-agent).\n\n---\n\n## Requirements\n\nThis Splunk Distribution of OpenTelemetry requires Python 3.6 or later.\n\n## Get started\n\nTo get started, install the `splunk-opentelemetry[all]` package, run the bootstrap\nscript and wrap your run command with `splunk-py-trace`.\n\nFor example, if the runtime parameters were:\n\n```\npython main.py --port=8000\n```\n\nThen the runtime parameters should be updated to:\n\n```\n$ pip install splunk-opentelemetry[all]\n$ splunk-py-trace-bootstrap\n$ OTEL_SERVICE_NAME=my-python-app \\\n    splunk-py-trace python main.py --port=8000\n```\n\nTo see the Python instrumentation in action with sample applications, see our\n[examples](https://github.com/signalfx/tracing-examples/tree/main/opentelemetry-tracing/opentelemetry-python-tracing).\n\n### Basic configuration\n\nThe service name resource attribute is the only configuration option\nthat needs to be specified. You can set it by adding a `service.name`\nattribute as shown in the [example above](#get-started).\n\nA few other configuration options that may need to be changed or set are:\n\n- Trace propagation format if not sending to other applications using W3C\n  trace-context. For example, if other applications are instrumented with\n  `signalfx-*-tracing` instrumentation. See the [trace\n  propagation](docs/advanced-config.md#trace-propagation-configuration)\n  configuration documentation for more information.\n- Endpoint if not sending to a locally running Splunk OpenTelemetry Connector\n  with default configuration. For example, if the SignalFx Smart Agent is used.\n  See the [exporters](docs/advanced-config.md#trace-exporters) configuration\n  documentation for more information.\n- Environment resource attribute `deployment.environment` to specify what\n  environment the span originated from. For example:\n  ```\n  OTEL_RESOURCE_ATTRIBUTES=deployment.environment=production\n  ```\n- Service version resource attribute `service.version` to specify the version\n  of your instrumented application. For example:\n  ```\n  OTEL_RESOURCE_ATTRIBUTES=service.version=1.2.3\n  ```\n\nThe `deployment.environment` and `service.version` resource attributes are not\nstrictly required, but recommended to be set if they are\navailable.\n\nThe `OTEL_RESOURCE_ATTRIBUTES` syntax is described in detail in the\n[trace configuration](docs/advanced-config.md#trace-configuration) section.\n\n### Supported Python Versions\n\nThe instrumentation works with Python verion 3.6 or higher. Supported\nlibraries are listed\n[here](https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation).\n\n## Advanced Configuration\n\nFor the majority of users, the [Getting Started](#get-started) section is\nall you need. Advanced configuration documentation can be found\n[here](docs/advanced-config.md). In addition, special cases for instrumentation\nare documented [here](docs/instrumentation-special-cases.md).\n\n## Manually instrument an application\n\nDocumentation on how to manually instrument a Python application is available\n[here](https://opentelemetry.io/docs/instrumentation/python/).\n\nTo extend the instrumentation with the OpenTelemetry Instrumentation for Python,\nyou have to use a compatible API version.\n\nThe Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.8.0</span> is compatible\nwith:\n\n* OpenTelemetry API version <span class="otel-api-version">1.12.0</span>\n* OpenTelemetry SDK version <span class="otel-sdk-version">1.12.0</span>\n* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.33b0</span>\n\n## Correlating traces with logs\n\nThe Splunk Distribution of OpenTelemetry Python provides a way\nto correlate traces with logs. See [Connect Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/instrumentation/connect-traces-logs.html).\n\n# License and versioning\n\nThe Splunk distribution of OpenTelemetry Python Instrumentation is a\ndistribution of the [OpenTelemetry Python\nproject](https://github.com/open-telemetry/opentelemetry-python). It is\nreleased under the terms of the Apache Software License version 2.0. See [the\nlicense file](./LICENSE) for more details.\n\n>ℹ️&nbsp;&nbsp;SignalFx was acquired by Splunk in October 2019. See [Splunk SignalFx](https://www.splunk.com/en_us/investor-relations/acquisitions/signalfx.html) for more information.\n',
+    'long_description': '---\n\n<p align="center">\n  <strong>\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/get-started.html">Get Started</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="CONTRIBUTING.md">Get Involved</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html">Migrating from SignalFx Python Tracing</a>\n  </strong>\n</p>\n\n<p align="center">\n  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.15.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.15.0-blueviolet?style=for-the-badge"/></a></span>\n  <a href="https://github.com/signalfx/splunk-otel-python/releases">\n    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/signalfx/splunk-otel-python?style=for-the-badge">\n  </a>\n  <a href="https://pypi.org/project/splunk-opentelemetry/">\n    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/splunk-opentelemetry?style=for-the-badge">\n  </a>\n  <a href="https://github.com/signalfx/gdi-specification/releases/tag/v1.0.0">\n    <img alt="Splunk GDI specification" src="https://img.shields.io/badge/GDI-1.0.0-blueviolet?style=for-the-badge">\n  </a>\n  <a href="https://codecov.io/gh/signalfx/splunk-otel-python">\n    <img alt="Codecov" src="https://img.shields.io/codecov/c/github/signalfx/splunk-otel-python?style=for-the-badge&token=XKXjEQKGaK">\n  </a>\n  <a href="https://github.com/signalfx/splunk-otel-python/actions?query=workflow%3ATests">\n    <img alt="Build Status" src="https://img.shields.io/github/workflow/status/signalfx/splunk-otel-python/Tests?style=for-the-badge">\n  </a>\n</p>\n\n<p align="center">\n  <strong>\n    <a href="https://github.com/signalfx/tracing-examples/tree/main/opentelemetry-tracing/opentelemetry-python-tracing">Examples</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="SECURITY.md">Security</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/README.md">Supported Libraries</a>\n    &nbsp;&nbsp;&bull;&nbsp;&nbsp;\n    <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/common-python-troubleshooting.html">Troubleshooting</a>\n  </strong>\n</p>\n\n# Splunk Distribution of OpenTelemetry Python\n\nThe Splunk distribution of [OpenTelemetry\nPython](https://github.com/open-telemetry/opentelemetry-python) provides\nmultiple installable packages that automatically instrument your Python\napplication to capture and report distributed traces to Splunk APM.\nInstrumentation works by patching supported libraries at runtime with an\nOpenTelemetry-compatible tracer to capture and export trace spans.\n\nThis distribution comes with the following defaults:\n\n- [W3C tracecontext](https://www.w3.org/TR/trace-context/) and [W3C\n  baggage](https://www.w3.org/TR/baggage/) context propagation;\n  [B3](https://github.com/openzipkin/b3-propagation) can also be\n  [configured](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/configuration/advanced-python-otel-configuration.html).\n- [OTLP gRPC\n  exporter](https://opentelemetry-python.readthedocs.io/en/latest/exporter/otlp/otlp.html)\n  configured to send spans to a locally running [Splunk OpenTelemetry\n  Connector](https://github.com/signalfx/splunk-otel-collector)\n  (`http://localhost:4317`).\n- Unlimited default limits for [configuration options](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/configuration/advanced-python-otel-configuration.html) to\n  support full-fidelity traces.\n\nIf you\'re currently using the SignalFx Tracing Library for Python and want to\nmigrate to the Splunk Distribution of OpenTelemetry Python, see [Migrate from\nthe SignalFx Tracing Library for Python](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-SignalFX-Python-agent).\n\n---\n\n## Requirements\n\nThis Splunk Distribution of OpenTelemetry requires Python 3.7 or later.\n\n## Get started\n\nTo get started, install the `splunk-opentelemetry[all]` package, run the bootstrap\nscript and wrap your run command with `splunk-py-trace`.\n\nFor example, if the runtime parameters were:\n\n```\npython main.py --port=8000\n```\n\nThen the runtime parameters should be updated to:\n\n```\n$ pip install splunk-opentelemetry[all]\n$ splunk-py-trace-bootstrap\n$ OTEL_SERVICE_NAME=my-python-app \\\n    splunk-py-trace python main.py --port=8000\n```\n\nTo see the Python instrumentation in action with sample applications, see our\n[examples](https://github.com/signalfx/tracing-examples/tree/main/opentelemetry-tracing/opentelemetry-python-tracing).\n\n### Basic configuration\n\nThe service name resource attribute is the only configuration option\nthat needs to be specified. You can set it by adding a `service.name`\nattribute as shown in the [example above](#get-started).\n\nA few other configuration options that may need to be changed or set are:\n\n- Trace propagation format if not sending to other applications using W3C\n  trace-context. For example, if other applications are instrumented with\n  `signalfx-*-tracing` instrumentation. See the [trace\n  propagation](docs/advanced-config.md#trace-propagation-configuration)\n  configuration documentation for more information.\n- Endpoint if not sending to a locally running Splunk OpenTelemetry Connector\n  with default configuration. For example, if the SignalFx Smart Agent is used.\n  See the [exporters](docs/advanced-config.md#trace-exporters) configuration\n  documentation for more information.\n- Environment resource attribute `deployment.environment` to specify what\n  environment the span originated from. For example:\n  ```\n  OTEL_RESOURCE_ATTRIBUTES=deployment.environment=production\n  ```\n- Service version resource attribute `service.version` to specify the version\n  of your instrumented application. For example:\n  ```\n  OTEL_RESOURCE_ATTRIBUTES=service.version=1.2.3\n  ```\n\nThe `deployment.environment` and `service.version` resource attributes are not\nstrictly required, but recommended to be set if they are\navailable.\n\nThe `OTEL_RESOURCE_ATTRIBUTES` syntax is described in detail in the\n[trace configuration](docs/advanced-config.md#trace-configuration) section.\n\n### Supported Python Versions\n\nThe instrumentation works with Python verion 3.7 or higher. Supported\nlibraries are listed\n[here](https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation).\n\n## Advanced Configuration\n\nFor the majority of users, the [Getting Started](#get-started) section is\nall you need. Advanced configuration documentation can be found\n[here](docs/advanced-config.md). In addition, special cases for instrumentation\nare documented [here](docs/instrumentation-special-cases.md).\n\n## Manually instrument an application\n\nDocumentation on how to manually instrument a Python application is available\n[here](https://opentelemetry.io/docs/instrumentation/python/).\n\nTo extend the instrumentation with the OpenTelemetry Instrumentation for Python,\nyou have to use a compatible API version.\n\nThe Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.9.1</span> is compatible\nwith:\n\n* OpenTelemetry API version <span class="otel-api-version">1.15.0</span>\n* OpenTelemetry SDK version <span class="otel-sdk-version">1.15.0</span>\n* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.36b0</span>\n\n## Correlating traces with logs\n\nThe Splunk Distribution of OpenTelemetry Python provides a way\nto correlate traces with logs. See [Connect Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/instrumentation/connect-traces-logs.html).\n\n# License\n\nThe Splunk distribution of OpenTelemetry Python Instrumentation is a\ndistribution of the [OpenTelemetry Python\nproject](https://github.com/open-telemetry/opentelemetry-python). It is\nreleased under the terms of the Apache Software License version 2.0. See [the\nlicense file](./LICENSE) for more details.\n\n>ℹ️&nbsp;&nbsp;SignalFx was acquired by Splunk in October 2019. See [Splunk SignalFx](https://www.splunk.com/en_us/investor-relations/acquisitions/signalfx.html) for more information.\n',
     'author': 'Splunk',
     'author_email': 'splunk-oss@splunk.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['splunk_otel', 'splunk_otel.cmd'] package_data = \ {'': ['*']}
-install_requires = \ ['opentelemetry-api==1.12.0', 'opentelemetry-
-instrumentation==0.33b0', 'opentelemetry-sdk==1.12.0', 'opentelemetry-semantic-
-conventions==0.33b0'] extras_require = \ {':extra == "all" or extra == "b3"':
-['opentelemetry-propagator-b3==1.12.0'], ':extra == "all" or extra ==
-"jaeger"': ['opentelemetry-exporter-jaeger-thrift==1.12.0'], ':extra == "all"
-or extra == "otlp"': ['opentelemetry-exporter-otlp-proto-grpc==1.12.0']}
+install_requires = \ ['opentelemetry-api==1.15.0', 'opentelemetry-
+instrumentation==0.36b0', 'opentelemetry-sdk==1.15.0', 'opentelemetry-semantic-
+conventions==0.36b0'] extras_require = \ {':extra == "all" or extra == "b3"':
+['opentelemetry-propagator-b3==1.15.0'], ':extra == "all" or extra ==
+"jaeger"': ['opentelemetry-exporter-jaeger-thrift==1.15.0'], ':extra == "all"
+or extra == "otlp"': ['opentelemetry-exporter-otlp-proto-grpc==1.15.0']}
 entry_points = \ {'console_scripts': ['splk-py-trace = splunk_otel.cmd.trace:
 run_deprecated', 'splk-py-trace-bootstrap = ' 'splunk_otel.cmd.bootstrap:
 run_deprecated', 'splunk-py-trace = splunk_otel.cmd.trace:run', 'splunk-py-
 trace-bootstrap = ' 'splunk_otel.cmd.bootstrap:run'], 'opentelemetry_distro':
 ['splunk_distro = splunk_otel.distro:_SplunkDistro']} setup_kwargs = { 'name':
-'splunk-opentelemetry', 'version': '1.8.0', 'description': 'The Splunk
+'splunk-opentelemetry', 'version': '1.9.1', 'description': 'The Splunk
 distribution of OpenTelemetry Python Instrumentation provides a Python agent
 that automatically instruments your Python application to capture and report
 distributed traces to SignalFx APM.', 'long_description': '---\n\n
   \n \n Get_Started\n   •  \n Get_Involved\n   •  \n Migrating_from_SignalFx
                               Python_Tracing\n\n
 \n\n
 \n [OpenTelemetry_Python_Version]\n \n_[GitHub_release_(latest_SemVer)]\n\n \n_
@@ -43,15 +43,15 @@
 Observability/gdi/get-data-in/application/python/configuration/advanced-python-
 otel-configuration.html) to\n support full-fidelity traces.\n\nIf you\'re
 currently using the SignalFx Tracing Library for Python and want to\nmigrate to
 the Splunk Distribution of OpenTelemetry Python, see [Migrate from\nthe
 SignalFx Tracing Library for Python](https://docs.splunk.com/Observability/gdi/
 get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-
 to-otel.html#nav-Migrate-from-SignalFX-Python-agent).\n\n---\n\n##
-Requirements\n\nThis Splunk Distribution of OpenTelemetry requires Python 3.6
+Requirements\n\nThis Splunk Distribution of OpenTelemetry requires Python 3.7
 or later.\n\n## Get started\n\nTo get started, install the `splunk-
 opentelemetry[all]` package, run the bootstrap\nscript and wrap your run
 command with `splunk-py-trace`.\n\nFor example, if the runtime parameters were:
 \n\n```\npython main.py --port=8000\n```\n\nThen the runtime parameters should
 be updated to:\n\n```\n$ pip install splunk-opentelemetry[all]\n$ splunk-py-
 trace-bootstrap\n$ OTEL_SERVICE_NAME=my-python-app \\\n splunk-py-trace python
 main.py --port=8000\n```\n\nTo see the Python instrumentation in action with
@@ -76,36 +76,37 @@
 instrumented application. For example:\n ```\n
 OTEL_RESOURCE_ATTRIBUTES=service.version=1.2.3\n ```\n\nThe
 `deployment.environment` and `service.version` resource attributes are
 not\nstrictly required, but recommended to be set if they
 are\navailable.\n\nThe `OTEL_RESOURCE_ATTRIBUTES` syntax is described in detail
 in the\n[trace configuration](docs/advanced-config.md#trace-configuration)
 section.\n\n### Supported Python Versions\n\nThe instrumentation works with
-Python verion 3.6 or higher. Supported\nlibraries are listed\n[here](https://
+Python verion 3.7 or higher. Supported\nlibraries are listed\n[here](https://
 github.com/open-telemetry/opentelemetry-python-contrib/tree/main/
 instrumentation).\n\n## Advanced Configuration\n\nFor the majority of users,
 the [Getting Started](#get-started) section is\nall you need. Advanced
 configuration documentation can be found\n[here](docs/advanced-config.md). In
 addition, special cases for instrumentation\nare documented [here](docs/
 instrumentation-special-cases.md).\n\n## Manually instrument an
 application\n\nDocumentation on how to manually instrument a Python application
 is available\n[here](https://opentelemetry.io/docs/instrumentation/python/
 ).\n\nTo extend the instrumentation with the OpenTelemetry Instrumentation for
 Python,\nyou have to use a compatible API version.\n\nThe Splunk Distribution
-of OpenTelemetry Python version 1.8.0 is compatible\nwith:\n\n* OpenTelemetry
-API version 1.12.0\n* OpenTelemetry SDK version 1.12.0\n* OpenTelemetry
-Instrumentation for Python version 0.33b0\n\n## Correlating traces with
+of OpenTelemetry Python version 1.9.1 is compatible\nwith:\n\n* OpenTelemetry
+API version 1.15.0\n* OpenTelemetry SDK version 1.15.0\n* OpenTelemetry
+Instrumentation for Python version 0.36b0\n\n## Correlating traces with
 logs\n\nThe Splunk Distribution of OpenTelemetry Python provides a way\nto
 correlate traces with logs. See [Connect Python trace data with logs](https://
 docs.splunk.com/Observability/gdi/get-data-in/application/python/
-instrumentation/connect-traces-logs.html).\n\n# License and versioning\n\nThe
-Splunk distribution of OpenTelemetry Python Instrumentation is a\ndistribution
-of the [OpenTelemetry Python\nproject](https://github.com/open-telemetry/
+instrumentation/connect-traces-logs.html).\n\n# License\n\nThe Splunk
+distribution of OpenTelemetry Python Instrumentation is a\ndistribution of the
+[OpenTelemetry Python\nproject](https://github.com/open-telemetry/
 opentelemetry-python). It is\nreleased under the terms of the Apache Software
 License version 2.0. See [the\nlicense file](./LICENSE) for more
 details.\n\n>â¹ï¸  SignalFx was acquired by Splunk in October 2019. See
 [Splunk SignalFx](https://www.splunk.com/en_us/investor-relations/acquisitions/
 signalfx.html) for more information.\n', 'author': 'Splunk', 'author_email':
-'splunk-oss@splunk.com', 'maintainer': None, 'maintainer_email': None, 'url':
-None, 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'entry_points':
-entry_points, 'python_requires': '>=3.6,<4.0', } setup(**setup_kwargs)
+'splunk-oss@splunk.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'None', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'extras_require': extras_require,
+'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `splunk-opentelemetry-1.8.0/PKG-INFO` & `splunk_opentelemetry-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: splunk-opentelemetry
-Version: 1.8.0
+Version: 1.9.1
 Summary: The Splunk distribution of OpenTelemetry Python Instrumentation provides a Python agent that automatically instruments your Python application to capture and report distributed traces to SignalFx APM.
 License: Apache-2.0
 Author: Splunk
 Author-email: splunk-oss@splunk.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: b3
 Provides-Extra: jaeger
 Provides-Extra: otlp
-Requires-Dist: opentelemetry-api (==1.12.0)
-Requires-Dist: opentelemetry-exporter-jaeger-thrift (==1.12.0); extra == "all" or extra == "jaeger"
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.12.0); extra == "all" or extra == "otlp"
-Requires-Dist: opentelemetry-instrumentation (==0.33b0)
-Requires-Dist: opentelemetry-propagator-b3 (==1.12.0); extra == "all" or extra == "b3"
-Requires-Dist: opentelemetry-sdk (==1.12.0)
-Requires-Dist: opentelemetry-semantic-conventions (==0.33b0)
+Requires-Dist: opentelemetry-api (==1.15.0)
+Requires-Dist: opentelemetry-exporter-jaeger-thrift (==1.15.0) ; extra == "all" or extra == "jaeger"
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.15.0) ; extra == "all" or extra == "otlp"
+Requires-Dist: opentelemetry-instrumentation (==0.36b0)
+Requires-Dist: opentelemetry-propagator-b3 (==1.15.0) ; extra == "all" or extra == "b3"
+Requires-Dist: opentelemetry-sdk (==1.15.0)
+Requires-Dist: opentelemetry-semantic-conventions (==0.36b0)
 Description-Content-Type: text/markdown
 
 ---
 
 <p align="center">
   <strong>
     <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/get-started.html">Get Started</a>
@@ -35,15 +35,15 @@
     <a href="CONTRIBUTING.md">Get Involved</a>
     &nbsp;&nbsp;&bull;&nbsp;&nbsp;
     <a href="https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html">Migrating from SignalFx Python Tracing</a>
   </strong>
 </p>
 
 <p align="center">
-  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.12.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.12.0-blueviolet?style=for-the-badge"/></a></span>
+  <span class="otel-version-badge"><a href="https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.15.0"><img alt="OpenTelemetry Python Version" src="https://img.shields.io/badge/otel-1.15.0-blueviolet?style=for-the-badge"/></a></span>
   <a href="https://github.com/signalfx/splunk-otel-python/releases">
     <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/signalfx/splunk-otel-python?style=for-the-badge">
   </a>
   <a href="https://pypi.org/project/splunk-opentelemetry/">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/splunk-opentelemetry?style=for-the-badge">
   </a>
   <a href="https://github.com/signalfx/gdi-specification/releases/tag/v1.0.0">
@@ -96,15 +96,15 @@
 migrate to the Splunk Distribution of OpenTelemetry Python, see [Migrate from
 the SignalFx Tracing Library for Python](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-SignalFX-Python-agent).
 
 ---
 
 ## Requirements
 
-This Splunk Distribution of OpenTelemetry requires Python 3.6 or later.
+This Splunk Distribution of OpenTelemetry requires Python 3.7 or later.
 
 ## Get started
 
 To get started, install the `splunk-opentelemetry[all]` package, run the bootstrap
 script and wrap your run command with `splunk-py-trace`.
 
 For example, if the runtime parameters were:
@@ -158,15 +158,15 @@
 available.
 
 The `OTEL_RESOURCE_ATTRIBUTES` syntax is described in detail in the
 [trace configuration](docs/advanced-config.md#trace-configuration) section.
 
 ### Supported Python Versions
 
-The instrumentation works with Python verion 3.6 or higher. Supported
+The instrumentation works with Python verion 3.7 or higher. Supported
 libraries are listed
 [here](https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation).
 
 ## Advanced Configuration
 
 For the majority of users, the [Getting Started](#get-started) section is
 all you need. Advanced configuration documentation can be found
@@ -177,27 +177,27 @@
 
 Documentation on how to manually instrument a Python application is available
 [here](https://opentelemetry.io/docs/instrumentation/python/).
 
 To extend the instrumentation with the OpenTelemetry Instrumentation for Python,
 you have to use a compatible API version.
 
-The Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.8.0</span> is compatible
+The Splunk Distribution of OpenTelemetry Python version <span class="splunk-version">1.9.1</span> is compatible
 with:
 
-* OpenTelemetry API version <span class="otel-api-version">1.12.0</span>
-* OpenTelemetry SDK version <span class="otel-sdk-version">1.12.0</span>
-* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.33b0</span>
+* OpenTelemetry API version <span class="otel-api-version">1.15.0</span>
+* OpenTelemetry SDK version <span class="otel-sdk-version">1.15.0</span>
+* OpenTelemetry Instrumentation for Python version <span class="otel-instrumentation-version">0.36b0</span>
 
 ## Correlating traces with logs
 
 The Splunk Distribution of OpenTelemetry Python provides a way
 to correlate traces with logs. See [Connect Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-data-in/application/python/instrumentation/connect-traces-logs.html).
 
-# License and versioning
+# License
 
 The Splunk distribution of OpenTelemetry Python Instrumentation is a
 distribution of the [OpenTelemetry Python
 project](https://github.com/open-telemetry/opentelemetry-python). It is
 released under the terms of the Apache Software License version 2.0. See [the
 license file](./LICENSE) for more details.
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: splunk-opentelemetry Version: 1.8.0 Summary: The
+Metadata-Version: 2.1 Name: splunk-opentelemetry Version: 1.9.1 Summary: The
 Splunk distribution of OpenTelemetry Python Instrumentation provides a Python
 agent that automatically instruments your Python application to capture and
 report distributed traces to SignalFx APM. License: Apache-2.0 Author: Splunk
-Author-email: splunk-oss@splunk.com Requires-Python: >=3.6,<4.0 Classifier:
+Author-email: splunk-oss@splunk.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Provides-Extra: all Provides-
-Extra: b3 Provides-Extra: jaeger Provides-Extra: otlp Requires-Dist:
-opentelemetry-api (==1.12.0) Requires-Dist: opentelemetry-exporter-jaeger-
-thrift (==1.12.0); extra == "all" or extra == "jaeger" Requires-Dist:
-opentelemetry-exporter-otlp-proto-grpc (==1.12.0); extra == "all" or extra ==
-"otlp" Requires-Dist: opentelemetry-instrumentation (==0.33b0) Requires-Dist:
-opentelemetry-propagator-b3 (==1.12.0); extra == "all" or extra == "b3"
-Requires-Dist: opentelemetry-sdk (==1.12.0) Requires-Dist: opentelemetry-
-semantic-conventions (==0.33b0) Description-Content-Type: text/markdown ---
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
+Provides-Extra: b3 Provides-Extra: jaeger Provides-Extra: otlp Requires-Dist:
+opentelemetry-api (==1.15.0) Requires-Dist: opentelemetry-exporter-jaeger-
+thrift (==1.15.0) ; extra == "all" or extra == "jaeger" Requires-Dist:
+opentelemetry-exporter-otlp-proto-grpc (==1.15.0) ; extra == "all" or extra ==
+"otlp" Requires-Dist: opentelemetry-instrumentation (==0.36b0) Requires-Dist:
+opentelemetry-propagator-b3 (==1.15.0) ; extra == "all" or extra == "b3"
+Requires-Dist: opentelemetry-sdk (==1.15.0) Requires-Dist: opentelemetry-
+semantic-conventions (==0.36b0) Description-Content-Type: text/markdown ---
   Get_Started   •   Get_Involved   •   Migrating_from_SignalFx_Python_Tracing
 [OpenTelemetry_Python_Version] [GitHub_release_(latest_SemVer)] [PyPI_-_Python
          Version] [Splunk_GDI_specification] [Codecov] [Build_Status]
     Examples   •   Security   •   Supported_Libraries   •   Troubleshooting
 # Splunk Distribution of OpenTelemetry Python The Splunk distribution of
 [OpenTelemetry Python](https://github.com/open-telemetry/opentelemetry-python)
 provides multiple installable packages that automatically instrument your
@@ -39,15 +39,15 @@
 python/configuration/advanced-python-otel-configuration.html) to support full-
 fidelity traces. If you're currently using the SignalFx Tracing Library for
 Python and want to migrate to the Splunk Distribution of OpenTelemetry Python,
 see [Migrate from the SignalFx Tracing Library for Python](https://
 docs.splunk.com/Observability/gdi/get-data-in/application/python/
 troubleshooting/migrate-signalfx-python-agent-to-otel.html#nav-Migrate-from-
 SignalFX-Python-agent). --- ## Requirements This Splunk Distribution of
-OpenTelemetry requires Python 3.6 or later. ## Get started To get started,
+OpenTelemetry requires Python 3.7 or later. ## Get started To get started,
 install the `splunk-opentelemetry[all]` package, run the bootstrap script and
 wrap your run command with `splunk-py-trace`. For example, if the runtime
 parameters were: ``` python main.py --port=8000 ``` Then the runtime parameters
 should be updated to: ``` $ pip install splunk-opentelemetry[all] $ splunk-py-
 trace-bootstrap $ OTEL_SERVICE_NAME=my-python-app \ splunk-py-trace python
 main.py --port=8000 ``` To see the Python instrumentation in action with sample
 applications, see our [examples](https://github.com/signalfx/tracing-examples/
@@ -70,31 +70,31 @@
 version resource attribute `service.version` to specify the version of your
 instrumented application. For example: ```
 OTEL_RESOURCE_ATTRIBUTES=service.version=1.2.3 ``` The `deployment.environment`
 and `service.version` resource attributes are not strictly required, but
 recommended to be set if they are available. The `OTEL_RESOURCE_ATTRIBUTES`
 syntax is described in detail in the [trace configuration](docs/advanced-
 config.md#trace-configuration) section. ### Supported Python Versions The
-instrumentation works with Python verion 3.6 or higher. Supported libraries are
+instrumentation works with Python verion 3.7 or higher. Supported libraries are
 listed [here](https://github.com/open-telemetry/opentelemetry-python-contrib/
 tree/main/instrumentation). ## Advanced Configuration For the majority of
 users, the [Getting Started](#get-started) section is all you need. Advanced
 configuration documentation can be found [here](docs/advanced-config.md). In
 addition, special cases for instrumentation are documented [here](docs/
 instrumentation-special-cases.md). ## Manually instrument an application
 Documentation on how to manually instrument a Python application is available
 [here](https://opentelemetry.io/docs/instrumentation/python/). To extend the
 instrumentation with the OpenTelemetry Instrumentation for Python, you have to
 use a compatible API version. The Splunk Distribution of OpenTelemetry Python
-version 1.8.0 is compatible with: * OpenTelemetry API version 1.12.0 *
-OpenTelemetry SDK version 1.12.0 * OpenTelemetry Instrumentation for Python
-version 0.33b0 ## Correlating traces with logs The Splunk Distribution of
+version 1.9.1 is compatible with: * OpenTelemetry API version 1.15.0 *
+OpenTelemetry SDK version 1.15.0 * OpenTelemetry Instrumentation for Python
+version 0.36b0 ## Correlating traces with logs The Splunk Distribution of
 OpenTelemetry Python provides a way to correlate traces with logs. See [Connect
 Python trace data with logs](https://docs.splunk.com/Observability/gdi/get-
 data-in/application/python/instrumentation/connect-traces-logs.html). # License
-and versioning The Splunk distribution of OpenTelemetry Python Instrumentation
-is a distribution of the [OpenTelemetry Python project](https://github.com/
-open-telemetry/opentelemetry-python). It is released under the terms of the
-Apache Software License version 2.0. See [the license file](./LICENSE) for more
+The Splunk distribution of OpenTelemetry Python Instrumentation is a
+distribution of the [OpenTelemetry Python project](https://github.com/open-
+telemetry/opentelemetry-python). It is released under the terms of the Apache
+Software License version 2.0. See [the license file](./LICENSE) for more
 details. >â¹ï¸  SignalFx was acquired by Splunk in October 2019. See [Splunk
 SignalFx](https://www.splunk.com/en_us/investor-relations/acquisitions/
 signalfx.html) for more information.
```

