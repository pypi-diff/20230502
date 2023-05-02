# Comparing `tmp/eventiq-0.1.3.tar.gz` & `tmp/eventiq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventiq-0.1.3.tar", max compression
+gzip compressed data, was "eventiq-0.1.4.tar", max compression
```

## Comparing `eventiq-0.1.3.tar` & `eventiq-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,69 @@
--rw-r--r--   0        0        0    11357 2023-03-16 13:22:54.139105 eventiq-0.1.3/LICENSE
--rw-r--r--   0        0        0     3554 2023-03-16 13:22:54.139105 eventiq-0.1.3/README.md
--rw-r--r--   0        0        0      660 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/__init__.py
--rw-r--r--   0        0        0       59 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/__main__.py
--rw-r--r--   0        0        0       22 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/_version.py
--rw-r--r--   0        0        0      171 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/asyncapi/__init__.py
--rw-r--r--   0        0        0     2598 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/asyncapi/generator.py
--rw-r--r--   0        0        0     1579 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/asyncapi/models.py
--rw-r--r--   0        0        0      426 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/asyncapi/registry.py
--rw-r--r--   0        0        0        0 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/__init__.py
--rw-r--r--   0        0        0       59 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/kafka/__init__.py
--rw-r--r--   0        0        0     3673 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/kafka/broker.py
--rw-r--r--   0        0        0      482 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/kafka/settings.py
--rw-r--r--   0        0        0      181 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/nats/__init__.py
--rw-r--r--   0        0        0     5560 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/nats/broker.py
--rw-r--r--   0        0        0     2841 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/nats/middlewares.py
--rw-r--r--   0        0        0      617 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/nats/settings.py
--rw-r--r--   0        0        0       61 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/pubsub/__init__.py
--rw-r--r--   0        0        0     2359 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/pubsub/broker.py
--rw-r--r--   0        0        0      179 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/pubsub/settings.py
--rw-r--r--   0        0        0       65 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5054 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/rabbitmq/broker.py
--rw-r--r--   0        0        0      816 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/rabbitmq/middlewares.py
--rw-r--r--   0        0        0      437 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/rabbitmq/settings.py
--rw-r--r--   0        0        0       59 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/redis/__init__.py
--rw-r--r--   0        0        0     1894 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/redis/broker.py
--rw-r--r--   0        0        0     1745 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/redis/middlewares.py
--rw-r--r--   0        0        0      305 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/redis/settings.py
--rw-r--r--   0        0        0     2006 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/backends/stub.py
--rw-r--r--   0        0        0     9709 2023-03-16 13:22:54.143105 eventiq-0.1.3/eventiq/broker.py
--rw-r--r--   0        0        0     2466 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/cli.py
--rw-r--r--   0        0        0     4298 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/consumer.py
--rw-r--r--   0        0        0      201 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/context.py
--rw-r--r--   0        0        0       92 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/defaults.py
--rw-r--r--   0        0        0      282 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/encoders/__init__.py
--rw-r--r--   0        0        0      670 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/encoders/json.py
--rw-r--r--   0        0        0      706 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/encoders/msgpack.py
--rw-r--r--   0        0        0      645 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/encoders/orjson.py
--rw-r--r--   0        0        0      494 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/encoders/pickle.py
--rw-r--r--   0        0        0      873 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/exceptions.py
--rw-r--r--   0        0        0     1619 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/http.py
--rw-r--r--   0        0        0     1103 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/logger.py
--rw-r--r--   0        0        0     3348 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middleware.py
--rw-r--r--   0        0        0      354 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/__init__.py
--rw-r--r--   0        0        0      871 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/debug.py
--rw-r--r--   0        0        0      862 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/error.py
--rw-r--r--   0        0        0     1682 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/healthcheck.py
--rw-r--r--   0        0        0     4658 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/prometheus.py
--rw-r--r--   0        0        0     2080 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/middlewares/retries.py
--rw-r--r--   0        0        0     2302 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/models.py
--rw-r--r--   0        0        0      343 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/plugins.py
--rw-r--r--   0        0        0        0 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/py.typed
--rw-r--r--   0        0        0      740 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/runner.py
--rw-r--r--   0        0        0     3087 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/service.py
--rw-r--r--   0        0        0      720 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/settings.py
--rw-r--r--   0        0        0     1066 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/types.py
--rw-r--r--   0        0        0      216 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/utils/__init__.py
--rw-r--r--   0        0        0      192 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/utils/datetime.py
--rw-r--r--   0        0        0      390 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/utils/enum.py
--rw-r--r--   0        0        0      915 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/utils/functools.py
--rw-r--r--   0        0        0      212 2023-03-16 13:22:54.147105 eventiq-0.1.3/eventiq/utils/imports.py
--rw-r--r--   0        0        0     3268 2023-03-16 13:22:54.147105 eventiq-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 eventiq-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 19:28:01.090240 eventiq-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4666 2023-05-02 19:28:01.090240 eventiq-0.1.4/README.md
+-rw-r--r--   0        0        0      704 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/__main__.py
+-rw-r--r--   0        0        0      407 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/_compat.py
+-rw-r--r--   0        0        0       22 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/_version.py
+-rw-r--r--   0        0        0      171 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/__init__.py
+-rw-r--r--   0        0        0     2598 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/generator.py
+-rw-r--r--   0        0        0     1579 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/models.py
+-rw-r--r--   0        0        0      426 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/registry.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/__init__.py
+-rw-r--r--   0        0        0     3673 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/broker.py
+-rw-r--r--   0        0        0      482 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/settings.py
+-rw-r--r--   0        0        0      181 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/__init__.py
+-rw-r--r--   0        0        0     5867 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/broker.py
+-rw-r--r--   0        0        0     2841 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/middlewares.py
+-rw-r--r--   0        0        0      617 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/settings.py
+-rw-r--r--   0        0        0       61 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/__init__.py
+-rw-r--r--   0        0        0     2359 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/broker.py
+-rw-r--r--   0        0        0      179 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/settings.py
+-rw-r--r--   0        0        0       65 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     5037 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/broker.py
+-rw-r--r--   0        0        0      816 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/middlewares.py
+-rw-r--r--   0        0        0      437 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/settings.py
+-rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/__init__.py
+-rw-r--r--   0        0        0     1894 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/broker.py
+-rw-r--r--   0        0        0     1745 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/middlewares.py
+-rw-r--r--   0        0        0      305 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/settings.py
+-rw-r--r--   0        0        0     1978 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/stub.py
+-rw-r--r--   0        0        0     9233 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/broker.py
+-rw-r--r--   0        0        0     2466 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/cli.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/config/__init__.py
+-rw-r--r--   0        0        0      995 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/config/factory.py
+-rw-r--r--   0        0        0     1723 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/config/models.py
+-rw-r--r--   0        0        0      226 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/config/settings.py
+-rw-r--r--   0        0        0     4353 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/consumer.py
+-rw-r--r--   0        0        0       92 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/defaults.py
+-rw-r--r--   0        0        0      282 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/json.py
+-rw-r--r--   0        0        0      706 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/msgpack.py
+-rw-r--r--   0        0        0      645 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/orjson.py
+-rw-r--r--   0        0        0      494 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/pickle.py
+-rw-r--r--   0        0        0      955 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/exceptions.py
+-rw-r--r--   0        0        0     1584 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/http.py
+-rw-r--r--   0        0        0     1014 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/logger.py
+-rw-r--r--   0        0        0      784 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/message.py
+-rw-r--r--   0        0        0     3333 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middleware.py
+-rw-r--r--   0        0        0      354 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/debug.py
+-rw-r--r--   0        0        0      862 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/error.py
+-rw-r--r--   0        0        0     1682 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/healthcheck.py
+-rw-r--r--   0        0        0     4435 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/opentelemetry.py
+-rw-r--r--   0        0        0     5115 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/prometheus.py
+-rw-r--r--   0        0        0     3926 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/retries.py
+-rw-r--r--   0        0        0     2144 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/models.py
+-rw-r--r--   0        0        0     1665 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/py.typed
+-rw-r--r--   0        0        0      740 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/runner.py
+-rw-r--r--   0        0        0     3668 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/service.py
+-rw-r--r--   0        0        0      643 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/settings.py
+-rw-r--r--   0        0        0     1116 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/types.py
+-rw-r--r--   0        0        0      216 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/datetime.py
+-rw-r--r--   0        0        0      390 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/enum.py
+-rw-r--r--   0        0        0      915 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/functools.py
+-rw-r--r--   0        0        0     1106 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/imports.py
+-rw-r--r--   0        0        0     4360 2023-05-02 19:28:01.094240 eventiq-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7562 1970-01-01 00:00:00.000000 eventiq-0.1.4/PKG-INFO
```

### Comparing `eventiq-0.1.3/LICENSE` & `eventiq-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/README.md` & `eventiq-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 ![Build](https://github.com/performancemedia/eventiq/workflows/Publish/badge.svg)
 ![License](https://img.shields.io/github/license/performancemedia/eventiq)
 ![Python](https://img.shields.io/pypi/pyversions/eventiq)
 ![Format](https://img.shields.io/pypi/format/eventiq)
 ![PyPi](https://img.shields.io/pypi/v/eventiq)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.3
+Version: 0.1.4
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
@@ -41,22 +42,22 @@
 
 - Stub (in memory using `asyncio.Queue` for PoC, local development and testing)
 - NATS (with JetStream)
 - Redis Pub/Sub
 - Kafka
 - Rabbitmq
 - Google Cloud PubSub
-- And more comming
+- And more coming
 
 ## Optional Dependencies
   - `cli` - `typer` and `aiorun`
   - broker of choice: `nats`, `kafka`, `rabbitmq`, `redis`, `pubsub`
   - custom message serializers: `msgpack`, `orjson`
   - `prometheus` - Metric exposure via `PrometheusMiddleware`
-
+  - `opentelemetry` - tracing support
 ## Motivation
 
 - [Celery](https://docs.celeryq.dev/en/stable/getting-started/introduction.html)
 - [Dramatiq](https://dramatiq.io/)
 - [Huey](https://huey.readthedocs.io/en/latest/)
 - [arq](https://arq-docs.helpmanual.io/)
 
@@ -99,13 +100,25 @@
 
 ## Scaling
 
 Each message is load-balanced (depending on broker) between all service instances with the same `name`.
 To scale number of processes you can use containers (docker/k8s), [supervisor](http://supervisord.org/),
 or web server like gunicorn.
 
+## Features
 
-## TODOS:
-- More tests
-  - Integration tests with docker-compose and all backends
-- Docs + tutorials
-- [OpenTelemetry](https://opentelemetry.io/) Middleware (?)
+- Modern, `asyncio` based python 3.8+ syntax
+- Minimal dependencies, only `pydantic`, `async_timeout` and `python-json-logger` are required
+- Automatic message parsing based on type annotations (like FastAPI)
+- Code hot-reload
+- Highly scalable: each service can process hundreds of tasks concurrently,
+    all messages are load balanced between all instances by default
+- Resilient - at least once delivery for all messages by default 
+- Customizable & pluggable message encoders (json, msgpack, custom)
+- Json formatted logger
+- Multiple broker support (Nats, Kafka, Rabbitmq, Redis, PubSub, and more coming)
+- Easily extensible via Middlewares and Plugins
+- Cloud Events standard as base message structure (no more python specific `*args` and `**kwargs` in messages)
+- AsyncAPI documentation generation from code
+- Twelve factor app approach - stdout logging, configuration through environment variables
+- Out-of-the-box integration with Prometheus (metrics) and OpenTelemetry (tracing)
+- Application bootstrap via `.yaml` file (see examples/configuration)
```

### Comparing `eventiq-0.1.3/eventiq/__init__.py` & `eventiq-0.1.4/eventiq/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ._version import __version__
 from .asyncapi import publishes
 from .broker import Broker
 from .consumer import Consumer, ConsumerGroup, ForwardResponse, GenericConsumer
+from .message import Message
 from .middleware import Middleware
 from .models import CloudEvent
 from .plugins import BrokerPlugin, ServicePlugin
 from .runner import ServiceRunner
 from .service import Service
 from .types import RawMessage
 
@@ -14,14 +15,15 @@
     "Broker",
     "BrokerPlugin",
     "Consumer",
     "ConsumerGroup",
     "CloudEvent",
     "ForwardResponse",
     "GenericConsumer",
+    "Message",
     "Middleware",
     "RawMessage",
     "Service",
     "ServicePlugin",
     "ServiceRunner",
     "publishes",
 ]
```

### Comparing `eventiq-0.1.3/eventiq/asyncapi/generator.py` & `eventiq-0.1.4/eventiq/asyncapi/generator.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/asyncapi/models.py` & `eventiq-0.1.4/eventiq/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/kafka/broker.py` & `eventiq-0.1.4/eventiq/backends/kafka/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/nats/broker.py` & `eventiq-0.1.4/eventiq/backends/nats/broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,27 @@
 from nats.aio.msg import Msg as NatsMsg
 from nats.js import JetStreamContext
 
 from eventiq.broker import Broker
 from eventiq.exceptions import BrokerError, PublishError
 from eventiq.utils.functools import retry_async
 
+from ...message import Message
 from .settings import JetStreamSettings, NatsSettings
 
 if TYPE_CHECKING:
     from eventiq import CloudEvent, Consumer, Service
 
 
+class NatsMessageProxy(Message[NatsMsg]):
+    def __init__(self, message: NatsMsg):
+        super().__init__(message)
+        self._num_delivered = message.metadata.num_delivered
+
+
 class NatsBroker(Broker[NatsMsg]):
     """
     :param url: Url to nats server(s)
     :param connection_options: additional connection options passed to nats.connect(...)
     :param auto_flush: auto flush messages on publish
     :param kwargs: options for base class
     """
@@ -39,14 +46,18 @@
         super().__init__(**kwargs)
         self.url = url
         self.connection_options = connection_options or {}
         self._auto_flush = auto_flush
         self._nc = None
 
     @property
+    def message_proxy_class(self) -> type[Message]:
+        return NatsMessageProxy
+
+    @property
     def nc(self) -> nats.NATS:
         if self._nc is None:
             raise BrokerError("Broker not connected. Call await broker.connect() first")
         return self._nc
 
     def parse_incoming_message(self, message: NatsMsg) -> Any:
         return self.encoder.decode(message.data)
@@ -160,14 +171,14 @@
                     await asyncio.sleep(5)
         except Exception:
             self.logger.exception("Cancelling consumer")
         finally:
             if consumer.dynamic:
                 await subscription.unsubscribe()
 
-    async def _ack(self, message: NatsMsg) -> None:
+    async def _ack(self, message: Message) -> None:
         if not message._ackd:
             await message.ack()
 
-    async def _nack(self, message: NatsMsg, delay=None) -> None:
+    async def _nack(self, message: Message) -> None:
         if not message._ackd:
-            await message.nak(delay=delay)
+            await message.nak(delay=message.delay)
```

### Comparing `eventiq-0.1.3/eventiq/backends/nats/middlewares.py` & `eventiq-0.1.4/eventiq/backends/nats/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/nats/settings.py` & `eventiq-0.1.4/eventiq/backends/nats/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/pubsub/broker.py` & `eventiq-0.1.4/eventiq/backends/pubsub/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/rabbitmq/broker.py` & `eventiq-0.1.4/eventiq/backends/rabbitmq/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,30 +115,28 @@
         )
 
         await self.exchange.publish(msg, routing_key=message.topic, **kwargs)
 
     async def _ack(self, message: aio_pika.abc.AbstractIncomingMessage) -> None:
         await message.ack()
 
-    async def _nack(
-        self, message: aio_pika.abc.AbstractIncomingMessage, delay: int | None = None
-    ) -> None:
+    async def _nack(self, message: aio_pika.abc.AbstractIncomingMessage) -> None:
         await message.reject(requeue=True)
 
     @property
     def is_connected(self) -> bool:
         return not self.connection.is_closed
 
     def parse_incoming_message(
         self, message: aio_pika.abc.AbstractIncomingMessage
     ) -> Any:
-        return dict(
-            id=message.message_id,
-            trace_id=message.headers.get("X-Trace-ID"),
-            type=message.type,
-            data=self.encoder.decode(message.body),
-            source=message.app_id,
-            content_type=message.content_type,
-            version=message.headers.get("specversion"),
-            time=message.timestamp,
-            topic=message.routing_key,
-        )
+        return {
+            "id": message.message_id,
+            "trace_id": message.headers.get("X-Trace-ID"),
+            "type": message.type,
+            "data": self.encoder.decode(message.body),
+            "source": message.app_id,
+            "content_type": message.content_type,
+            "version": message.headers.get("specversion"),
+            "time": message.timestamp,
+            "topic": message.routing_key,
+        }
```

### Comparing `eventiq-0.1.3/eventiq/backends/rabbitmq/middlewares.py` & `eventiq-0.1.4/eventiq/backends/rabbitmq/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/redis/broker.py` & `eventiq-0.1.4/eventiq/backends/redis/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/redis/middlewares.py` & `eventiq-0.1.4/eventiq/backends/redis/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/backends/stub.py` & `eventiq-0.1.4/eventiq/backends/stub.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from typing import TYPE_CHECKING, Any
 
 from eventiq.broker import Broker
 from eventiq.middleware import Middleware
 
 if TYPE_CHECKING:
     from eventiq import CloudEvent, Consumer, Service
+    from eventiq.message import Message
     from eventiq.types import Encoder
 
 
 @dataclass
-class Message:
+class StubMessage:
     data: bytes
     queue: asyncio.Queue
 
 
-class StubBroker(Broker[Message]):
+class StubBroker(Broker[StubMessage]):
     """This is in-memory implementation of a broker class, mainly designed for testing."""
 
     protocol = "in-memory"
 
     def __init__(
         self,
         *,
@@ -31,15 +32,15 @@
         middlewares: list[Middleware] | None = None,
         **options: Any,
     ) -> None:
         super().__init__(encoder=encoder, middlewares=middlewares, **options)
         self.topics: dict[str, asyncio.Queue] = defaultdict(asyncio.Queue)
         self._stopped = False
 
-    def parse_incoming_message(self, message: Message) -> Any:
+    def parse_incoming_message(self, message: StubMessage) -> Any:
         return self.encoder.decode(message.data)
 
     async def _disconnect(self) -> None:
         self._stopped = True
 
     async def _start_consumer(self, service: Service, consumer: Consumer):
         queue = self.topics[consumer.topic]
@@ -50,21 +51,18 @@
 
     async def _connect(self) -> None:
         pass
 
     async def _publish(self, message: CloudEvent, **_) -> None:
         queue = self.topics[message.topic]
         data = self.encoder.encode(message.dict())
-        msg = Message(data=data, queue=queue)
+        msg = StubMessage(data=data, queue=queue)
         await queue.put(msg)
 
     async def _ack(self, message: Message) -> None:
         message.queue.task_done()
 
-    async def _nack(self, message: Message, delay: int | None = None) -> None:
-
-        if delay:
-            await asyncio.sleep(delay)
+    async def _nack(self, message: Message) -> None:
         await message.queue.put(message)
 
     def is_connected(self) -> bool:
         return True
```

### Comparing `eventiq-0.1.3/eventiq/broker.py` & `eventiq-0.1.4/eventiq/broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Awaitable, Callable, Generic
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Generic, Type, cast
 
 import async_timeout
 from pydantic import ValidationError
 
-from .context import context
 from .exceptions import DecodeError, Fail, Skip
 from .logger import LoggerMixin
+from .message import Message
 from .middleware import Middleware
 from .models import CloudEvent
-from .settings import BrokerSettings, Settings
+from .settings import BrokerSettings
 from .types import Encoder, RawMessage
-from .utils import str_uuid
 
 if TYPE_CHECKING:
     from eventiq import Consumer, Service
 
 
 class AbstractBroker(ABC, Generic[RawMessage]):
     @abstractmethod
@@ -44,18 +43,18 @@
     async def _disconnect(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
         raise NotImplementedError
 
-    async def _ack(self, message: RawMessage) -> None:
+    async def _ack(self, message: Message) -> None:
         """Empty default implementation for backends that do not support explicit ack"""
 
-    async def _nack(self, message: RawMessage, delay: int | None = None) -> None:
+    async def _nack(self, message: Message) -> None:
         """Same as for ._ack()"""
 
 
 class Broker(AbstractBroker[RawMessage], LoggerMixin, ABC):
     """Base broker class
     :param description: Broker (Server) Description
     :param encoder: Encoder (Serializer) class
@@ -82,94 +81,90 @@
         self.middlewares: list[Middleware] = middlewares or []
         self._lock = asyncio.Lock()
         self._stopped = True
 
     def __repr__(self):
         return type(self).__name__
 
+    @property
+    def message_proxy_class(self) -> type[Message]:
+        return Message
+
     def get_handler(
         self, service: Service, consumer: Consumer
     ) -> Callable[[RawMessage], Awaitable[Any | None]]:
         async def handler(raw_message: RawMessage) -> None:
             exc: Exception | None = None
             result: Any = None
+            msg = self.message_proxy_class(raw_message)
             try:
                 parsed = self.parse_incoming_message(raw_message)
                 message = consumer.validate_message(parsed)
-                setattr(message, "_raw", raw_message)
-                token = context.set(message.context)
-
+                message.set_raw(msg)
             except (DecodeError, ValidationError) as e:
-                self.logger.exception(
-                    "Parsing error Decode/Validation error", exc_info=e
-                )
-                await self._ack(raw_message)
+                self.logger.exception("Message parsing error", exc_info=e)
+                msg.fail()
+                await self.ack(service, consumer, msg)
                 return
 
             try:
                 await self.dispatch_before(
                     "process_message", service, consumer, message
                 )
             except Skip:
                 self.logger.info(f"Skipped message {message.id}")
                 await self.dispatch_after("skip_message", service, consumer, message)
-                await self.ack(service, consumer, raw_message)
+                await self.ack(service, consumer, msg)
                 return
             try:
                 async with async_timeout.timeout(consumer.timeout):
                     self.logger.info(f"Running consumer {consumer.name}")
                     result = await consumer.process(message)
                 if consumer.forward_response and result is not None:
                     await self.publish_event(
                         CloudEvent(
                             type=consumer.forward_response.as_type,
                             topic=consumer.forward_response.topic,
                             data=result,
-                            trace_id=message.trace_id,
                             source=service.name,
                         )
                     )
             # TODO: asyncio.CanceledError handling (?)
             except Exception as e:
                 self.logger.error(f"Exception in {consumer.name} {e}")
                 exc = e
             finally:
-                if isinstance(exc, Fail):
-                    self.logger.error(f"Failing message due to {exc}")
-                    await self.ack(service, consumer, raw_message)
-                    return
                 await self.dispatch_after(
                     "process_message", service, consumer, message, result, exc
                 )
-                await self.ack(service, consumer, raw_message)
-                context.reset(token)
+                if exc is None or isinstance(exc, Fail) or msg.failed:
+                    await self.ack(service, consumer, msg)
+                else:
+                    await self.nack(service, consumer, msg)
 
         return handler
 
-    async def ack(
-        self, service: Service, consumer: Consumer, message: RawMessage
-    ) -> None:
+    async def ack(self, service: Service, consumer: Consumer, message: Message) -> None:
         await self.dispatch_before("ack", service, consumer, message)
         await self._ack(message)
         await self.dispatch_after("ack", service, consumer, message)
 
     async def nack(
         self,
         service: Service,
         consumer: Consumer,
-        message: RawMessage,
-        delay: int | None = None,
+        message: Message,
     ) -> None:
         await self.dispatch_after(
             "nack",
             service,
             consumer,
             message,
         )
-        await self._nack(message, delay)
+        await self._nack(message)
         await self.dispatch_after(
             "nack",
             service,
             consumer,
             message,
         )
 
@@ -201,42 +196,35 @@
 
     async def publish(
         self,
         topic: str,
         data: Any | None = None,
         type_: type[CloudEvent] | str = "CloudEvent",
         source: str = "",
-        trace_id: str | None = None,
         **kwargs: Any,
     ) -> None:
         """Publish message to broker
-        :param trace_id:
         :param topic: Topic to publish data
         :param data: Message content
         :param type_: Event type, name or class
         :param source: message sender (service/app name)
         :param kwargs: additional params passed to underlying broker implementation, such as headers
         :rtype: None
         """
 
         if isinstance(type_, str):
             cls = functools.partial(CloudEvent, type=type_)
         else:
             cls = type_  # type: ignore
-        if trace_id is None:
-            ctx = context.get()
-            trace_id = ctx["trace_id"]
 
-        trace_id = trace_id or str_uuid()
         message: CloudEvent = cls(
             content_type=self.encoder.CONTENT_TYPE,
             topic=topic,
             data=data,
             source=source,
-            trace_id=trace_id,
         )
         await self.publish_event(message, **kwargs)
 
     async def start_consumer(self, service: Service, consumer: Consumer):
         await self.dispatch_before("consumer_start", service, consumer)
         await self._start_consumer(service, consumer)
         await self.dispatch_after("consumer_start", service, consumer)
@@ -262,19 +250,19 @@
     async def dispatch_before(self, event: str, *args, **kwargs) -> None:
         await self._dispatch(f"before_{event}", *args, **kwargs)
 
     async def dispatch_after(self, event: str, *args, **kwargs) -> None:
         await self._dispatch(f"after_{event}", *args, **kwargs)
 
     @classmethod
+    def from_settings(cls, settings: BrokerSettings, **kwargs: Any) -> Broker:
+        broker_cls: type[Broker] = cast(Type[Broker], settings.broker_class)
+        kw = settings.dict(exclude={"broker_cls"})
+        kw.update(kwargs)
+        return broker_cls(**kw)
+
+    @classmethod
     def from_env(
         cls,
-        description: str | None = None,
-        middlewares: list[Middleware] | None = None,
         **kwargs,
     ) -> Broker:
-        broker_cls: type[Broker] = Settings().get_broker_class()
-        broker_settings = broker_cls.Settings(
-            description=description, middlewares=middlewares, **kwargs
-        )
-        instance = broker_cls(**broker_settings.dict())
-        return instance
+        return cls.from_settings(BrokerSettings(), **kwargs)
```

### Comparing `eventiq-0.1.3/eventiq/cli.py` & `eventiq-0.1.4/eventiq/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 @cli.command(help="Run service")
 def run(
     service_or_runner: str,
     log_level: str = typer.Option(default="info"),
     use_uvloop: bool = typer.Option(False),
 ) -> None:
-    logger.info(f"Running [{service_or_runner}]...")
     setup_logging(log_level.upper())
+    logger.info(f"Running [{service_or_runner}]...")
     obj = import_from_string(service_or_runner)
     obj.run(use_uvloop=use_uvloop)
 
 
 @cli.command(help="Watch and reload on files change")
 def watch(
     service_or_runner: str = typer.Argument(...),
```

### Comparing `eventiq-0.1.3/eventiq/consumer.py` & `eventiq-0.1.4/eventiq/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,25 +82,27 @@
 
     @property
     def description(self) -> str:
         return self.fn.__doc__ or ""
 
 
 class GenericConsumer(Consumer[T], ABC):
-    name: str
-
     def __init__(self, *, topic: str, name: str | None = None, **options: Any):
 
-        super().__init__(name=name or type(self).__name__, topic=topic, **options)
+        super().__init__(
+            name=name or str(getattr(type(self), "name", type(self).__name__)),
+            topic=topic,
+            **options,
+        )
 
     def __init_subclass__(cls, **kwargs):
         if "abstract" not in kwargs:
             cls.event_type = cls.__orig_bases__[0].__args__[0]
             if not hasattr(cls, "name"):
-                setattr(cls, "name", cls.__name__)
+                cls.name = cls.__name__
             if not asyncio.iscoroutinefunction(cls.process):
                 cls.process = run_async(cls.process)
 
     @property
     def description(self) -> str:
         return self.__doc__ or ""
```

### Comparing `eventiq-0.1.3/eventiq/encoders/json.py` & `eventiq-0.1.4/eventiq/encoders/json.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/encoders/msgpack.py` & `eventiq-0.1.4/eventiq/encoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/encoders/orjson.py` & `eventiq-0.1.4/eventiq/encoders/orjson.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/exceptions.py` & `eventiq-0.1.4/eventiq/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 
 class ConfigurationError(Exception):
     """Raised by framework when invalid configuration is supplied"""
 
 
+class PluginLoadError(ImportError):
+    """Raised when unable to load plugin"""
+
+
 class BrokerError(Exception):
     """Base Exception for broker related errors"""
 
 
 class PublishError(BrokerError):
     """Raised when publishing a message fails"""
```

### Comparing `eventiq-0.1.3/eventiq/http.py` & `eventiq-0.1.4/eventiq/http.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 ) -> None:
     app.on_event("startup")(service.start)
     app.on_event("shutdown")(service.stop)
 
     if add_health_endpoint:
         from fastapi.responses import JSONResponse
 
-        for m in service.broker.middlewares:
-            if hasattr(m, "get_health_status") and callable(m.get_health_status):  # type: ignore
-
-                @app.get(path, response_class=JSONResponse)
-                def get_health_status():
-                    """Return get broker connection status"""
-                    status = m.get_health_status()
-                    return (
-                        JSONResponse({"status": "ok"})
-                        if status
-                        else JSONResponse(
-                            {"status": "Connection error"}, status_code=503
-                        )
-                    )
+        middlewares = [
+            m for m in service.broker.middlewares if hasattr(m, "get_health_status")
+        ]
+        if len(middlewares) and middlewares[0]:
+            m = middlewares[0]
+
+            @app.get(path, response_class=JSONResponse)
+            def get_health_status():
+                """Return get broker connection status"""
+                status = m.get_health_status()
+                return (
+                    JSONResponse({"status": "ok"})
+                    if status
+                    else JSONResponse({"status": "Connection error"}, status_code=503)
+                )
 
         raise ConfigurationError("HealthCheckMiddleware expected")
 
 
 def add_serve_async_api_endpoint(
     app: FastAPI, service: Service, endpoint: str = "/docs/asyncapi.json"
 ):
```

### Comparing `eventiq-0.1.3/eventiq/logger.py` & `eventiq-0.1.4/eventiq/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import inspect
 import logging
 from typing import Type, Union
 
 from pythonjsonlogger import jsonlogger
 
-from eventiq.context import context
 from eventiq.utils.datetime import utc_now
 
 
-class ContextAwareJsonFormatter(jsonlogger.JsonFormatter):
+class EventiqJsonFormatter(jsonlogger.JsonFormatter):
     def add_fields(self, log_record, record, message_dict):
         super().add_fields(log_record, record, message_dict)
-        log_record.update(**context.get())
         if "timestamp" not in log_record:
             log_record["timestamp"] = utc_now()
 
         log_record["level"] = record.levelname.upper()
 
 
 def setup_logging(level, fmt: str = "%(name) %(level) %(message)") -> None:
     handler = logging.StreamHandler()
-    handler.setFormatter(ContextAwareJsonFormatter(fmt))
+    handler.setFormatter(EventiqJsonFormatter(fmt))
     logging.basicConfig(handlers=[handler], level=level)
 
 
 def get_logger(module: str, name: Union[str, Type]) -> logging.Logger:
     if inspect.isclass(name):
         name = name.__name__
```

### Comparing `eventiq-0.1.3/eventiq/middleware.py` & `eventiq-0.1.4/eventiq/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from .logger import LoggerMixin
 
 if TYPE_CHECKING:
-    from eventiq import Broker, CloudEvent, Consumer, RawMessage, Service
+    from eventiq import Broker, CloudEvent, Consumer, Message, Service
 
 
 class Middleware(LoggerMixin):
     """Base class for middlewares"""
 
     async def before_broker_connect(self, broker: Broker) -> None:
         """Called before broker connects"""
@@ -46,34 +46,34 @@
         """Called after consumer is started"""
 
     async def before_ack(
         self,
         broker: Broker,
         service: Service,
         consumer: Consumer,
-        message: RawMessage,
+        message: Message,
     ) -> None:
         """Called before message is acknowledged"""
 
     async def after_ack(
         self,
         broker: Broker,
         service: Service,
         consumer: Consumer,
-        message: RawMessage,
+        message: Message,
     ) -> None:
         """Called after message is acknowledged"""
 
     async def before_nack(
-        self, broker: Broker, service: Service, consumer: Consumer, message: RawMessage
+        self, broker: Broker, service: Service, consumer: Consumer, message: Message
     ) -> None:
         """Called before message is rejected"""
 
     async def after_nack(
-        self, broker: Broker, service: Service, consumer: Consumer, message: RawMessage
+        self, broker: Broker, service: Service, consumer: Consumer, message: Message
     ) -> None:
         """Called after message is rejected"""
 
     async def before_publish(
         self, broker: Broker, message: CloudEvent, **kwargs
     ) -> None:
         """Called before message is published"""
```

### Comparing `eventiq-0.1.3/eventiq/middlewares/debug.py` & `eventiq-0.1.4/eventiq/middlewares/debug.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/middlewares/error.py` & `eventiq-0.1.4/eventiq/middlewares/error.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/middlewares/healthcheck.py` & `eventiq-0.1.4/eventiq/middlewares/healthcheck.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/middlewares/prometheus.py` & `eventiq-0.1.4/eventiq/middlewares/prometheus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from eventiq.middleware import Middleware
+from eventiq.types import ID
 from eventiq.utils.datetime import current_millis
 
 if TYPE_CHECKING:
     from prometheus_client.registry import CollectorRegistry
 
-    from eventiq import Broker, CloudEvent, Consumer, RawMessage, Service
+    from eventiq import Broker, CloudEvent, Consumer, Message, Service
 
 
 DEFAULT_BUCKETS = (
     5,
     10,
     25,
     50,
@@ -46,15 +47,15 @@
         from prometheus_client import REGISTRY, Counter, Gauge, Histogram
 
         self.run_server = run_server
         self.registry = registry or REGISTRY
         self.buckets = buckets or DEFAULT_BUCKETS
         self.server_host = server_host
         self.server_port = server_port
-        self.message_start_times: dict[str, int] = {}
+        self.message_start_times: dict[tuple[str, str, ID], int] = {}
         self.in_progress = Gauge(
             "messages_in_progress",
             "Total number of messages being processed.",
             ["topic", "service", "consumer"],
             registry=self.registry,
         )
         self.total_messages = Counter(
@@ -76,17 +77,17 @@
         )
         self.total_errored_messages = Counter(
             "message_error_total",
             "Total number of errored messages.",
             ["topic", "service", "consumer"],
             registry=self.registry,
         )
-        self.total_rejected_messages = Counter(
-            "message_rejected_total",
-            "Total number of messages rejected",
+        self.total_failed_messages = Counter(
+            "message_failed_total",
+            "Total number of messages failed",
             ["topic", "service", "consumer"],
             registry=self.registry,
         )
         self.message_durations = Histogram(
             "message_duration_ms",
             "Time spend processing message",
             ["topic", "service", "consumer"],
@@ -95,15 +96,17 @@
         )
 
     async def before_process_message(
         self, broker: Broker, service: Service, consumer: Consumer, message: CloudEvent
     ):
         labels = (consumer.topic, service.name, consumer.name)
         self.in_progress.labels(*labels).inc()
-        self.message_start_times[message.id] = current_millis()
+        self.message_start_times[
+            (service.name, consumer.name, message.id)
+        ] = current_millis()
 
     async def after_process_message(
         self,
         broker: Broker,
         service: Service,
         consumer: Consumer,
         message: CloudEvent,
@@ -112,32 +115,45 @@
     ) -> None:
         labels = (consumer.topic, service.name, consumer.name)
         self.in_progress.labels(*labels).dec()
         self.total_messages.labels(*labels).inc()
         if exc:
             self.total_errored_messages.labels(*labels).inc()
 
-        message_start_time = self.message_start_times.pop(message.id, current_millis())
+        message_start_time = self.message_start_times.pop(
+            (service.name, consumer.name, message.id), current_millis()
+        )
         message_duration = current_millis() - message_start_time
         self.message_durations.labels(*labels).observe(message_duration)
 
     async def after_skip_message(
         self, broker: Broker, service: Service, consumer: Consumer, message: CloudEvent
     ) -> None:
         labels = (consumer.topic, service.name, consumer.name)
         self.total_skipped_messages.labels(*labels).inc()
 
     async def after_publish(self, broker: Broker, message: CloudEvent, **kwargs):
         self.total_messages_published.labels(message.topic, message.source).inc()
 
     async def after_nack(
-        self, broker: Broker, service: Service, consumer: Consumer, message: RawMessage
+        self, broker: Broker, service: Service, consumer: Consumer, message: Message
     ):
-        labels = (consumer.topic, service, consumer.name)
-        self.total_rejected_messages.labels(*labels).inc()
+        labels = (consumer.topic, service.name, consumer.name)
+        self.total_errored_messages.labels(*labels).inc()
+
+    async def after_ack(
+        self,
+        broker: Broker,
+        service: Service,
+        consumer: Consumer,
+        message: Message,
+    ) -> None:
+        if message.failed:
+            labels = (consumer.topic, service.name, consumer.name)
+            self.total_failed_messages.labels(*labels).inc()
 
     async def after_broker_connect(self, broker: Broker):
         if self.run_server:
             from prometheus_client import start_http_server
 
             start_http_server(
                 self.server_port, self.server_host, registry=self.registry
```

### Comparing `eventiq-0.1.3/eventiq/models.py` & `eventiq-0.1.4/eventiq/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,71 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import Any, Dict, Generic, Optional
 
 from pydantic import Extra, Field, validator
 from pydantic.fields import PrivateAttr
 from pydantic.generics import GenericModel
 
-from .types import D, RawMessage
+from .message import Message
+from .types import ID, D
 from .utils import str_uuid
 from .utils.datetime import utc_now
 
 
 class CloudEvent(GenericModel, Generic[D]):
     specversion: Optional[str] = "1.0"
     content_type: str = Field("application/json", alias="datacontenttype")
-    id: str = Field(default_factory=str_uuid)
-    trace_id: str = Field(default_factory=str_uuid, alias="traceid")
+    id: ID = Field(default_factory=str_uuid)
     time: datetime = Field(default_factory=utc_now)
     topic: str = Field(..., alias="subject")
     type: Optional[str] = None
     source: Optional[str] = None
     data: Optional[D] = None
+    trace_ctx: Dict[str, str] = {}
 
     _raw: Optional[Any] = PrivateAttr()
 
     def __eq__(self, other):
         if not isinstance(other, CloudEvent):
             return False
         return self.id == other.id
 
-    def __hash__(self):
-        return hash((self.trace_id, self.id))
-
     @validator("type", allow_reuse=True, always=True, pre=True)
     def get_type_from_cls_name(cls, v) -> str:
         return v or cls.__name__
 
     @property
-    def raw(self) -> RawMessage:
+    def raw(self) -> Message:
         if self._raw is None:
             raise AttributeError("raw property accessible only for incoming messages")
         return self._raw
 
+    def _set(self, name: str, value: Any):
+        object.__setattr__(self, name, value)
+
     def set_source(self, value: str) -> None:
         self._set("source", value)
 
-    def set_trace_id(self, value: str):
-        self._set("trace_id", value)
-
-    def _set(self, name: str, value: Any):
-        object.__setattr__(self, name, value)
+    def set_raw(self, value: Message):
+        self._set("_raw", value)
 
     def dict(self, **kwargs: Any) -> Dict[str, Any]:
         kwargs.setdefault("by_alias", True)
         return super().dict(**kwargs)
 
     @classmethod
-    def from_object(cls, obj: D, **kwargs):
+    def new(cls, obj: D, **kwargs):
         return cls(data=obj, **kwargs)
 
     @property
-    def context(self) -> Dict[str, Any]:
-        return self.dict(include={"trace_id", "id"})
+    def age(self) -> timedelta:
+        return utc_now() - self.time
 
-    @property
-    def age(self) -> int:
-        return (utc_now() - self.time).seconds
+    def fail(self):
+        self.raw.fail()
 
     class Config:
         use_enum_values = True
         allow_population_by_field_name = True
         extra = Extra.allow
         # events are immutable, however it's sometimes useful to set source or traceid for unpublished events
         allow_mutation = False
```

### Comparing `eventiq-0.1.3/eventiq/runner.py` & `eventiq-0.1.4/eventiq/runner.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/eventiq/service.py` & `eventiq-0.1.4/eventiq/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any, Callable
 
-from .consumer import ConsumerGroup, ForwardResponse
+from .consumer import Consumer, ConsumerGroup, ForwardResponse
 from .defaults import DEFAULT_CONSUMER_TIME_LIMIT
 from .logger import LoggerMixin
 from .models import CloudEvent
+from .settings import ServiceSettings
 from .utils import generate_instance_id
 
 if TYPE_CHECKING:
     from .broker import Broker
     from .types import TagMeta
 
 
@@ -21,23 +22,23 @@
         self,
         name: str,
         broker: Broker,
         title: str | None = None,
         version: str = "0.1.0",
         description: str = "",
         tags_metadata: list[TagMeta] | None = None,
-        instance_id_generator: Callable[[], str] = generate_instance_id,
+        instance_id_generator: Callable[[], str] | None = None,
     ):
         self.broker = broker
         self.name = name
         self.title = title or name.title()
         self.version = version
         self.description = description
         self.tags_metadata = tags_metadata or []
-        self.id = instance_id_generator()
+        self.id = (instance_id_generator or generate_instance_id)()
         self.consumer_group = ConsumerGroup()
         # TODO: task gathering?
         self._tasks: list[asyncio.Task] = []
 
     def subscribe(
         self,
         topic: str,
@@ -53,14 +54,17 @@
             name=name,
             timeout=timeout,
             dynamic=dynamic,
             forward_response=forward_response,
             **options,
         )
 
+    def add_consumer(self, consumer: Consumer):
+        self.consumer_group.add_consumer(consumer)
+
     def add_consumer_group(self, consumer_group: ConsumerGroup) -> None:
         self.consumer_group.add_consumer_group(consumer_group)
 
     async def publish(
         self,
         topic: str,
         data: Any | None = None,
@@ -92,7 +96,18 @@
         await self.broker.dispatch_after("service_stop", self)
 
     def run(self, *args, **kwargs):
         from .runner import ServiceRunner
 
         runner = ServiceRunner([self])
         runner.run(*args, **kwargs)
+
+    @classmethod
+    def from_settings(cls, settings: ServiceSettings, **kwargs: Any) -> Service:
+        kw = settings.dict(exclude={"broker_settings"})
+        kw.update(**kwargs)
+        broker = Broker.from_settings(settings.broker_settings)
+        return cls(broker=broker, **kw)
+
+    @classmethod
+    def from_env(cls, **kwargs: Any) -> Service:
+        return cls.from_settings(ServiceSettings(), **kwargs)
```

### Comparing `eventiq-0.1.3/eventiq/types.py` & `eventiq-0.1.4/eventiq/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,21 @@
     Optional,
     Protocol,
     Type,
     TypedDict,
     TypeVar,
     Union,
 )
+from uuid import UUID
 
 if TYPE_CHECKING:
     from eventiq import CloudEvent, GenericConsumer
 
+ID = Union[str, int, UUID]
+
 
 RawMessage = TypeVar("RawMessage")
 
 T = TypeVar("T", bound="CloudEvent")
 D = TypeVar("D")
```

### Comparing `eventiq-0.1.3/eventiq/utils/functools.py` & `eventiq-0.1.4/eventiq/utils/functools.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.3/PKG-INFO` & `eventiq-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventiq
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cloud native framework for building event driven applications in Python.
 Home-page: https://github.com/performancemedia/eventiq
 License: Apache-2.0
 Keywords: framework,asyncio,microservice,event-driven
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
@@ -21,36 +21,40 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Provides-Extra: cli
-Provides-Extra: commons
+Provides-Extra: common
 Provides-Extra: kafka
 Provides-Extra: nats
+Provides-Extra: opentelemetry
 Provides-Extra: orjson
 Provides-Extra: ormsgpack
 Provides-Extra: prometheus
 Provides-Extra: pubsub
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Requires-Dist: aio-pika (>=9.0.4) ; extra == "all" or extra == "rabbitmq"
 Requires-Dist: aiokafka (>=0.8,<1.0) ; extra == "all" or extra == "kafka"
 Requires-Dist: aioredis (>=2.0,<3.0) ; extra == "all" or extra == "redis"
-Requires-Dist: aiorun (>=2022.11.1,<2023.0.0) ; extra == "all" or extra == "commons" or extra == "cli"
+Requires-Dist: aiorun (>=2022.11.1,<2023.0.0) ; extra == "all" or extra == "common" or extra == "cli"
 Requires-Dist: async-timeout (>=4.0)
 Requires-Dist: gcloud-aio-pubsub (>=5.2.0,<6.0) ; extra == "all" or extra == "pubsub"
 Requires-Dist: nats-py (>=2.2,<3.0) ; extra == "all" or extra == "nats"
-Requires-Dist: orjson (>=3.8.7,<4.0) ; extra == "all" or extra == "commons" or extra == "orjson"
+Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0) ; extra == "all" or extra == "common" or extra == "opentelemetry"
+Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0) ; extra == "all" or extra == "common" or extra == "opentelemetry"
+Requires-Dist: opentelemetry-semantic-conventions (>=0.38b0,<0.39) ; extra == "all" or extra == "common" or extra == "opentelemetry"
+Requires-Dist: orjson (>=3.8.7,<4.0) ; extra == "all" or extra == "common" or extra == "orjson"
 Requires-Dist: ormsgpack (>=1.2.5,<2.0) ; extra == "all" or extra == "ormsgpack"
-Requires-Dist: prometheus-client (>=0.16.0,<1.0) ; extra == "all" or extra == "commons" or extra == "prometheus"
+Requires-Dist: prometheus-client (>=0.16.0,<1.0) ; extra == "all" or extra == "common" or extra == "prometheus"
 Requires-Dist: pydantic (>=1.0)
 Requires-Dist: python-json-logger (>=2.0)
-Requires-Dist: typer (>=0.7.0) ; extra == "all" or extra == "commons" or extra == "cli"
+Requires-Dist: typer (>=0.7.0) ; extra == "all" or extra == "common" or extra == "cli"
 Project-URL: Documentation, https://performancemedia.github.io/eventiq/
 Project-URL: Repository, https://github.com/performancemedia/eventiq
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://performancemedia.github.io/eventiq/assets/logo.svg" style="width: 250px">
 
@@ -63,19 +67,20 @@
 ![Build](https://github.com/performancemedia/eventiq/workflows/Publish/badge.svg)
 ![License](https://img.shields.io/github/license/performancemedia/eventiq)
 ![Python](https://img.shields.io/pypi/pyversions/eventiq)
 ![Format](https://img.shields.io/pypi/format/eventiq)
 ![PyPi](https://img.shields.io/pypi/v/eventiq)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.3
+Version: 0.1.4
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
@@ -94,22 +99,22 @@
 
 - Stub (in memory using `asyncio.Queue` for PoC, local development and testing)
 - NATS (with JetStream)
 - Redis Pub/Sub
 - Kafka
 - Rabbitmq
 - Google Cloud PubSub
-- And more comming
+- And more coming
 
 ## Optional Dependencies
   - `cli` - `typer` and `aiorun`
   - broker of choice: `nats`, `kafka`, `rabbitmq`, `redis`, `pubsub`
   - custom message serializers: `msgpack`, `orjson`
   - `prometheus` - Metric exposure via `PrometheusMiddleware`
-
+  - `opentelemetry` - tracing support
 ## Motivation
 
 - [Celery](https://docs.celeryq.dev/en/stable/getting-started/introduction.html)
 - [Dramatiq](https://dramatiq.io/)
 - [Huey](https://huey.readthedocs.io/en/latest/)
 - [arq](https://arq-docs.helpmanual.io/)
 
@@ -152,13 +157,25 @@
 
 ## Scaling
 
 Each message is load-balanced (depending on broker) between all service instances with the same `name`.
 To scale number of processes you can use containers (docker/k8s), [supervisor](http://supervisord.org/),
 or web server like gunicorn.
 
+## Features
 
-## TODOS:
-- More tests
-  - Integration tests with docker-compose and all backends
-- Docs + tutorials
-- [OpenTelemetry](https://opentelemetry.io/) Middleware (?)
+- Modern, `asyncio` based python 3.8+ syntax
+- Minimal dependencies, only `pydantic`, `async_timeout` and `python-json-logger` are required
+- Automatic message parsing based on type annotations (like FastAPI)
+- Code hot-reload
+- Highly scalable: each service can process hundreds of tasks concurrently,
+    all messages are load balanced between all instances by default
+- Resilient - at least once delivery for all messages by default 
+- Customizable & pluggable message encoders (json, msgpack, custom)
+- Json formatted logger
+- Multiple broker support (Nats, Kafka, Rabbitmq, Redis, PubSub, and more coming)
+- Easily extensible via Middlewares and Plugins
+- Cloud Events standard as base message structure (no more python specific `*args` and `**kwargs` in messages)
+- AsyncAPI documentation generation from code
+- Twelve factor app approach - stdout logging, configuration through environment variables
+- Out-of-the-box integration with Prometheus (metrics) and OpenTelemetry (tracing)
+- Application bootstrap via `.yaml` file (see examples/configuration)
```

