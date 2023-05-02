# Comparing `tmp/atatus-1.4.0.tar.gz` & `tmp/atatus-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atatus-1.4.0.tar", last modified: Wed Jan  4 09:21:24 2023, max compression
+gzip compressed data, was "atatus-1.5.0.tar", last modified: Tue May  2 09:37:59 2023, max compression
```

## Comparing `atatus-1.4.0.tar` & `atatus-1.5.0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.658997 atatus-1.4.0/
--rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.4.0/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.4.0/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     2463 2023-01-04 09:21:24.659352 atatus-1.4.0/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      965 2023-01-04 09:02:24.000000 atatus-1.4.0/README.rst
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.094677 atatus-1.4.0/atatus/
--rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/base.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.110512 atatus-1.4.0/atatus/collector/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/collector/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    20658 2022-12-22 05:27:27.000000 atatus-1.4.0/atatus/collector/base.py
--rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/collector/builder.py
--rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/collector/hist.py
--rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/collector/layer.py
--rw-r--r--   0 apple      (501) staff       (20)     5699 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/collector/transport.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.113896 atatus-1.4.0/atatus/conf/
--rw-r--r--   0 apple      (501) staff       (20)    35139 2022-12-22 05:27:27.000000 atatus-1.4.0/atatus/conf/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/conf/constants.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.118896 atatus-1.4.0/atatus/context/
--rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.4.0/atatus/context/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/context/base.py
--rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/context/contextvars.py
--rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/context/threadlocal.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.120713 atatus-1.4.0/atatus/contrib/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/contrib/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.123262 atatus-1.4.0/atatus/contrib/aiohttp/
--rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/aiohttp/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/aiohttp/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/aiohttp/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.125375 atatus-1.4.0/atatus/contrib/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/asyncio/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.126321 atatus-1.4.0/atatus/contrib/celery/
--rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/celery/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.135830 atatus-1.4.0/atatus/contrib/django/
--rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/django/apps.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.138239 atatus-1.4.0/atatus/contrib/django/celery/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/contrib/django/celery/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/contrib/django/celery/models.py
--rw-r--r--   0 apple      (501) staff       (20)    14174 2022-12-22 14:08:57.000000 atatus-1.4.0/atatus/contrib/django/client.py
--rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.4.0/atatus/contrib/django/context_processors.py
--rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/django/handlers.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.139851 atatus-1.4.0/atatus/contrib/django/management/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/contrib/django/management/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.145736 atatus-1.4.0/atatus/contrib/django/management/commands/
--rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/contrib/django/management/commands/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/contrib/django/management/commands/atatus.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.149582 atatus-1.4.0/atatus/contrib/django/middleware/
--rw-r--r--   0 apple      (501) staff       (20)     9184 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/contrib/django/middleware/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.4.0/atatus/contrib/django/middleware/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/django/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.153319 atatus-1.4.0/atatus/contrib/flask/
--rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/contrib/flask/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3602 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/flask/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.161077 atatus-1.4.0/atatus/contrib/opentelemetry/
--rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentelemetry/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentelemetry/context.py
--rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentelemetry/span.py
--rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentelemetry/trace.py
--rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentelemetry/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.166621 atatus-1.4.0/atatus/contrib/opentracing/
--rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentracing/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentracing/span.py
--rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/opentracing/tracer.py
--rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/paste.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.167933 atatus-1.4.0/atatus/contrib/pylons/
--rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/pylons/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.168900 atatus-1.4.0/atatus/contrib/rq/
--rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.4.0/atatus/contrib/rq/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.174613 atatus-1.4.0/atatus/contrib/sanic/
--rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/sanic/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/sanic/patch.py
--rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/sanic/sanic_types.py
--rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/contrib/sanic/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.177593 atatus-1.4.0/atatus/contrib/serverless/
--rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/serverless/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/contrib/serverless/aws.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.181847 atatus-1.4.0/atatus/contrib/starlette/
--rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.4.0/atatus/contrib/starlette/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/starlette/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.184226 atatus-1.4.0/atatus/contrib/tornado/
--rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/tornado/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/contrib/tornado/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.185894 atatus-1.4.0/atatus/contrib/twisted/
--rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/contrib/twisted/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/events.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.190957 atatus-1.4.0/atatus/handlers/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/handlers/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/handlers/logbook.py
--rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/handlers/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/handlers/structlog.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.194152 atatus-1.4.0/atatus/instrumentation/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/instrumentation/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.4.0/atatus/instrumentation/control.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.361029 atatus-1.4.0/atatus/instrumentation/packages/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/instrumentation/packages/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.560736 atatus-1.4.0/atatus/instrumentation/packages/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiobotocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py
--rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiomysql.py
--rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiopg.py
--rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/aioredis.py
--rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/asyncpg.py
--rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/base.py
--rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/asyncio/sleep.py
--rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/azure.py
--rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/base.py
--rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/botocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/cassandra.py
--rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/dbapi2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.567688 atatus-1.4.0/atatus/instrumentation/packages/django/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/instrumentation/packages/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.4.0/atatus/instrumentation/packages/django/template.py
--rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/graphql.py
--rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httplib2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.572188 atatus-1.4.0/atatus/instrumentation/packages/httpx/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.580468 atatus-1.4.0/atatus/instrumentation/packages/httpx/async/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/async/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/async/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/async/httpx.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.589852 atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/httpx.py
--rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/httpx/utils.py
--rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.4.0/atatus/instrumentation/packages/jinja2.py
--rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/kafka.py
--rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/mysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/mysql_connector.py
--rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/psycopg2.py
--rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pylibmc.py
--rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pymemcache.py
--rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pymongo.py
--rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pymssql.py
--rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pymysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/pyodbc.py
--rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/python_memcached.py
--rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/redis.py
--rw-r--r--   0 apple      (501) staff       (20)     2863 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/requests.py
--rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/sqlite.py
--rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/tornado.py
--rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/urllib.py
--rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/packages/urllib3.py
--rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.4.0/atatus/instrumentation/packages/zlib.py
--rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/instrumentation/register.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.592960 atatus-1.4.0/atatus/metrics/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/metrics/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.4.0/atatus/metrics/base_metrics.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.607370 atatus-1.4.0/atatus/metrics/sets/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/metrics/sets/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.4.0/atatus/metrics/sets/breakdown.py
--rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.4.0/atatus/metrics/sets/cpu.py
--rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/metrics/sets/cpu_linux.py
--rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.4.0/atatus/metrics/sets/cpu_psutil.py
--rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/metrics/sets/prometheus.py
--rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.4.0/atatus/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/processors.py
--rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.4.0/atatus/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.618005 atatus-1.4.0/atatus/transport/
--rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/transport/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/transport/base.py
--rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/transport/exceptions.py
--rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/transport/http.py
--rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/transport/http_base.py
--rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.4.0/atatus/transport/http_urllib3.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.643215 atatus-1.4.0/atatus/utils/
--rw-r--r--   0 apple      (501) staff       (20)     7335 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/cgroup.py
--rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/cloud.py
--rw-r--r--   0 apple      (501) staff       (20)     3662 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/compat.py
--rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/deprecation.py
--rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/disttracing.py
--rw-r--r--   0 apple      (501) staff       (20)    10629 2023-01-03 09:24:18.000000 atatus-1.4.0/atatus/utils/encoding.py
--rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.4.0/atatus/utils/hw_info.py
--rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/json_encoder.py
--rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.4.0/atatus/utils/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/module_import.py
--rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/stacks.py
--rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/threading.py
--rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/time.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.657051 atatus-1.4.0/atatus/utils/wrapt/
--rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/_wrappers.c
--rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/arguments.py
--rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/decorators.py
--rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/importer.py
--rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.4.0/atatus/utils/wrapt/wrappers.py
--rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.4.0/atatus/utils/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     1658 2022-12-16 06:48:35.000000 atatus-1.4.0/atatus/version.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-01-04 09:21:24.102275 atatus-1.4.0/atatus.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2463 2023-01-04 09:21:23.000000 atatus-1.4.0/atatus.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     5743 2023-01-04 09:21:23.000000 atatus-1.4.0/atatus.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-01-04 09:21:23.000000 atatus-1.4.0/atatus.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.4.0/atatus.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)      205 2023-01-04 09:21:23.000000 atatus-1.4.0/atatus.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-01-04 09:21:23.000000 atatus-1.4.0/atatus.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.4.0/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)     3524 2023-01-04 09:21:24.661625 atatus-1.4.0/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.4.0/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.430778 atatus-1.5.0/
+-rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.5.0/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.5.0/MANIFEST.in
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-05-02 09:37:59.430956 atatus-1.5.0/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      991 2023-01-04 09:26:05.000000 atatus-1.5.0/README.rst
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.402470 atatus-1.5.0/atatus/
+-rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/base.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.404796 atatus-1.5.0/atatus/collector/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    25451 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/collector/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/collector/builder.py
+-rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/hist.py
+-rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/layer.py
+-rw-r--r--   0 apple      (501) staff       (20)     6418 2023-04-29 10:18:47.000000 atatus-1.5.0/atatus/collector/transport.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.405555 atatus-1.5.0/atatus/conf/
+-rw-r--r--   0 apple      (501) staff       (20)    35250 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/conf/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/conf/constants.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.406246 atatus-1.5.0/atatus/context/
+-rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.5.0/atatus/context/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/contextvars.py
+-rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/threadlocal.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.406506 atatus-1.5.0/atatus/contrib/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407072 atatus-1.5.0/atatus/contrib/aiohttp/
+-rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407476 atatus-1.5.0/atatus/contrib/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/asyncio/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407619 atatus-1.5.0/atatus/contrib/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/celery/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409134 atatus-1.5.0/atatus/contrib/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/apps.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409411 atatus-1.5.0/atatus/contrib/django/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/celery/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/celery/models.py
+-rw-r--r--   0 apple      (501) staff       (20)    14034 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/contrib/django/client.py
+-rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.5.0/atatus/contrib/django/context_processors.py
+-rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/handlers.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409549 atatus-1.5.0/atatus/contrib/django/management/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/management/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409841 atatus-1.5.0/atatus/contrib/django/management/commands/
+-rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/management/commands/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/django/management/commands/atatus.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.410341 atatus-1.5.0/atatus/contrib/django/middleware/
+-rw-r--r--   0 apple      (501) staff       (20)     9184 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/django/middleware/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.5.0/atatus/contrib/django/middleware/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.410751 atatus-1.5.0/atatus/contrib/flask/
+-rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/flask/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3602 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/flask/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.411627 atatus-1.5.0/atatus/contrib/opentelemetry/
+-rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/context.py
+-rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/span.py
+-rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/trace.py
+-rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412007 atatus-1.5.0/atatus/contrib/opentracing/
+-rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/span.py
+-rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/tracer.py
+-rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/paste.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412289 atatus-1.5.0/atatus/contrib/pylons/
+-rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/pylons/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412433 atatus-1.5.0/atatus/contrib/rq/
+-rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.5.0/atatus/contrib/rq/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412964 atatus-1.5.0/atatus/contrib/sanic/
+-rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/patch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/sanic_types.py
+-rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/sanic/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.413442 atatus-1.5.0/atatus/contrib/serverless/
+-rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/serverless/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/serverless/aws.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.413868 atatus-1.5.0/atatus/contrib/starlette/
+-rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.5.0/atatus/contrib/starlette/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/starlette/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.414230 atatus-1.5.0/atatus/contrib/tornado/
+-rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/tornado/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/tornado/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.414350 atatus-1.5.0/atatus/contrib/twisted/
+-rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/twisted/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/events.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.415094 atatus-1.5.0/atatus/handlers/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/handlers/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/handlers/logbook.py
+-rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/handlers/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/handlers/structlog.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.415481 atatus-1.5.0/atatus/instrumentation/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/control.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.420640 atatus-1.5.0/atatus/instrumentation/packages/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/packages/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.422640 atatus-1.5.0/atatus/instrumentation/packages/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiobotocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py
+-rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiomysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiopg.py
+-rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aioredis.py
+-rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/asyncpg.py
+-rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/sleep.py
+-rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/azure.py
+-rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/botocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/cassandra.py
+-rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/dbapi2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.422943 atatus-1.5.0/atatus/instrumentation/packages/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/packages/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/packages/django/template.py
+-rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/graphql.py
+-rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httplib2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.423271 atatus-1.5.0/atatus/instrumentation/packages/httpx/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.423739 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpx.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.424166 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpx.py
+-rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/packages/jinja2.py
+-rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/kafka.py
+-rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/mysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/mysql_connector.py
+-rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/psycopg2.py
+-rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pylibmc.py
+-rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymemcache.py
+-rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymongo.py
+-rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymssql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pyodbc.py
+-rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/python_memcached.py
+-rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/redis.py
+-rw-r--r--   0 apple      (501) staff       (20)     7001 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/instrumentation/packages/requests.py
+-rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/sqlite.py
+-rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/tornado.py
+-rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/urllib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/urllib3.py
+-rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/instrumentation/packages/zlib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/register.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.424431 atatus-1.5.0/atatus/metrics/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/metrics/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.5.0/atatus/metrics/base_metrics.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.425285 atatus-1.5.0/atatus/metrics/sets/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/metrics/sets/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/metrics/sets/breakdown.py
+-rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.5.0/atatus/metrics/sets/cpu.py
+-rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/metrics/sets/cpu_linux.py
+-rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/metrics/sets/cpu_psutil.py
+-rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/metrics/sets/prometheus.py
+-rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.5.0/atatus/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/processors.py
+-rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.5.0/atatus/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.426456 atatus-1.5.0/atatus/transport/
+-rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/transport/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/exceptions.py
+-rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/http.py
+-rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/http_base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.5.0/atatus/transport/http_urllib3.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.428973 atatus-1.5.0/atatus/utils/
+-rw-r--r--   0 apple      (501) staff       (20)     7689 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/utils/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/cgroup.py
+-rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/cloud.py
+-rw-r--r--   0 apple      (501) staff       (20)     3705 2023-04-29 11:08:46.000000 atatus-1.5.0/atatus/utils/compat.py
+-rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/deprecation.py
+-rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/disttracing.py
+-rw-r--r--   0 apple      (501) staff       (20)    10629 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/utils/encoding.py
+-rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/utils/hw_info.py
+-rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/json_encoder.py
+-rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.5.0/atatus/utils/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/module_import.py
+-rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/stacks.py
+-rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/threading.py
+-rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/time.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.430556 atatus-1.5.0/atatus/utils/wrapt/
+-rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/_wrappers.c
+-rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/arguments.py
+-rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/decorators.py
+-rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/importer.py
+-rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/wrappers.py
+-rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     1658 2023-04-26 05:50:12.000000 atatus-1.5.0/atatus/version.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.403534 atatus-1.5.0/atatus.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     5743 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.5.0/atatus.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)      205 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        7 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.5.0/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)     3524 2023-05-02 09:37:59.431549 atatus-1.5.0/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.5.0/setup.py
```

### Comparing `atatus-1.4.0/LICENSE` & `atatus-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/PKG-INFO` & `atatus-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.4.0
+Version: 1.5.0
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
@@ -35,16 +35,16 @@
         Copyright
         ----------
         
         Copyright (c) 2014-2023 Atatus. All rights reserved.
         
         
         .. _`Atatus Python APM agent`: https://www.atatus.com
-        .. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/django.html
-        .. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/flask.html
+        .. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/django.html
+        .. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/flask.html
         .. _`Release notes`: https://docs.atatus.com/docs/release-notes/python.html
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

### Comparing `atatus-1.4.0/README.rst` & `atatus-1.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 Copyright
 ----------
 
 Copyright (c) 2014-2023 Atatus. All rights reserved.
 
 
 .. _`Atatus Python APM agent`: https://www.atatus.com
-.. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/django.html
-.. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/flask.html
+.. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/django.html
+.. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/flask.html
 .. _`Release notes`: https://docs.atatus.com/docs/release-notes/python.html
```

### Comparing `atatus-1.4.0/atatus/__init__.py` & `atatus-1.5.0/atatus/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/base.py` & `atatus-1.5.0/atatus/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/collector/base.py` & `atatus-1.5.0/atatus/collector/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -308,21 +308,21 @@
                 if "remote_address" in txn["context"]["request"]["socket"]:
                     analytics_txn["ip"] = txn["context"]["request"]["socket"]["remote_address"]
 
         if "context" in txn and \
             "response" in txn["context"]:
                 if "body" in txn["context"]["response"]:
                     analytics_txn["responseBody"] = txn["context"]["response"]["body"]
-                    requestBodyLen = len(analytics_txn["responseBody"])
+                    responseBodyLen = len(analytics_txn["responseBody"])
 
         if "context" in txn and \
             "custom_response" in txn["context"]:
                 if "body" in txn["context"]["custom_response"]:
                     analytics_txn["responseBody"] = txn["context"]["custom_response"]["body"]
-                    requestBodyLen = len(analytics_txn["responseBody"])
+                    responseBodyLen = len(analytics_txn["responseBody"])
 
         if "context" in txn and \
             "response" in txn["context"]:
 
             if "headers" in txn["context"]["response"]:
                 analytics_txn["responseHeaders"] = txn["context"]["response"]["headers"]
 
@@ -361,14 +361,109 @@
                 analytics_txn["companyId"] = str(txn["context"]["company"]["id"])
 
         analytics_txn["body_len"] = requestBodyLen + responseBodyLen
         with self._analytics_lock:
              if len(self._analytics_agg) < 10000:
                 self._analytics_agg.append(analytics_txn)
 
+    def add_analytics_outgoing(self, txn, span):
+        analytics_txn = {}
+
+        if not all(k in txn for k in ("name", "id", "timestamp", "duration")):
+            return
+
+        if not all(k in span for k in ("name", "timestamp", "duration", "context")):
+            return
+
+        if "analytics_captured" not in span["context"]:
+            return
+
+        analytics_txn["timestamp"] = txn["timestamp"]
+        analytics_txn["txnId"] = txn["id"]
+        if "trace_id" in txn:
+            analytics_txn["traceId"] = txn["trace_id"]
+        
+        analytics_txn["name"] = span["name"]
+        analytics_txn["duration"] = span["duration"]
+
+        requestBodyLen = 0
+        responseBodyLen = 0
+        if "context" in span and \
+            "http" in span["context"] and \
+            "request" in span["context"]["http"]:
+
+            if "method" in span["context"]["http"]["request"]:
+                analytics_txn["method"] = span["context"]["http"]["request"]["method"]
+
+            if "headers" in span["context"]["http"]["request"]:
+                analytics_txn["requestHeaders"] = span["context"]["http"]["request"]["headers"]
+                if "User-Agent" in analytics_txn["requestHeaders"]:
+                    analytics_txn["userAgent"] = analytics_txn["requestHeaders"]["User-Agent"]
+                elif "user-agent" in analytics_txn["requestHeaders"]:
+                    analytics_txn["userAgent"] = analytics_txn["requestHeaders"]["user-agent"]
+
+            if "body" in span["context"]["http"]["request"]:
+                if span["context"]["http"]["request"]["body"] != "[REDACTED]":
+                    if span["context"]["http"]["request"]["body"] != "":
+                        instance_dict_convert = False
+                        string_body = ""
+                        if isinstance(span["context"]["http"]["request"]["body"], dict):
+                            try:
+                                string_body = json.dumps(span["context"]["http"]["request"]["body"])
+                                instance_dict_convert = True
+                            except Exception:
+                                pass
+                        if instance_dict_convert == False:
+                            string_body = str(span["context"]["http"]["request"]["body"])
+
+                        analytics_txn["requestBody"] = encoding.body_field(string_body)
+                        requestBodyLen = len(analytics_txn["requestBody"])
+
+        if "context" in span and \
+            "http" in span["context"] and \
+            "response" in span["context"]["http"]:
+                if "headers" in span["context"]["http"]["response"]:
+                     analytics_txn["responseHeaders"] = span["context"]["http"]["response"]["headers"]
+
+                if "body" in span["context"]["http"]["response"]:
+                    analytics_txn["responseBody"] = span["context"]["http"]["response"]["body"]
+                    responseBodyLen = len(analytics_txn["responseBody"])
+
+        if "context" in span and \
+            "http" in span["context"]:
+            
+            if "url" in span["context"]["http"]:
+                analytics_txn["url"] = span["context"]["http"]["url"]
+            if "status_code" in span["context"]["http"]:
+                analytics_txn["statusCode"] = span["context"]["http"]["status_code"]
+
+        if "context" in txn and \
+            "user" in txn["context"]:
+            
+            if "id" in txn["context"]["user"]:
+                analytics_txn["userId"] = str(txn["context"]["user"]["id"])
+
+            if "username" in txn["context"]["user"]:
+                analytics_txn["userName"] = txn["context"]["user"]["username"]
+
+            if "email" in txn["context"]["user"]:
+                analytics_txn["userEmail"] = txn["context"]["user"]["email"]
+
+        if "context" in txn and \
+            "company" in txn["context"]:
+
+            if "id" in txn["context"]["company"]:
+                analytics_txn["companyId"] = str(txn["context"]["company"]["id"])
+
+        analytics_txn["body_len"] = requestBodyLen + responseBodyLen
+        analytics_txn["direction"] = "outgoing"
+        with self._analytics_lock:
+             if len(self._analytics_agg) < 10000:
+                self._analytics_agg.append(analytics_txn)
+
     def add_span(self, span):
 
         if not all(k in span for k in ("transaction_id", "name", "type", "subtype", "duration")):
             return
 
         span_id = span["transaction_id"]
         if span_id not in self._spans:
@@ -422,14 +517,22 @@
                         continue
                     span_name = span["name"]
                     if not span_name:
                         continue
                     if span["timestamp"] >= txn["timestamp"]:
                         timestamp = ((span["timestamp"] - txn["timestamp"]) / 1000)
                         spans_tuple.append(SpanTiming(timestamp, timestamp + span["duration"]))
+
+                        if self._config.analytics_capture_outgoing is True:
+                            if span["type"] == "external" and span["subtype"] == "http":
+                                if "analytics" in self._hostinfo_response:
+                                    if self._hostinfo_response["analytics"] == True and self._analytics == True:
+                                        if background == False:
+                                            self.add_analytics_outgoing(txn, span)
+
                         if span_name not in self._txns_agg[txn_name].spans:
                             kind = Layer.kinds_dict.get(span["type"], span["type"])
                             type = Layer.types_dict.get(span["subtype"], span["subtype"])
                             self._txns_agg[txn_name].spans[span_name] = Layer(type, kind, span["duration"])
                         else:
                             self._txns_agg[txn_name].spans[span_name].aggregate(span["duration"])
```

### Comparing `atatus-1.4.0/atatus/collector/builder.py` & `atatus-1.5.0/atatus/collector/builder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/collector/hist.py` & `atatus-1.5.0/atatus/collector/hist.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/collector/layer.py` & `atatus-1.5.0/atatus/collector/layer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/collector/transport.py` & `atatus-1.5.0/atatus/collector/transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,39 +21,44 @@
         self._post_params = {
             'license_key': self._config.license_key,
             'agent_name': atatus.PYTHON_AGENT,
             "version": atatus.VERSION
         }
 
     def _post(self, endpoint, data):
-        if (self._blocked is True) and (endpoint != 'track/apm/hostinfo'):
-            return
+        if endpoint != 'track/apm/analytics/txn':
+            if (self._blocked is True) and (endpoint != 'track/apm/hostinfo'):
+                return
 
         try:
             time.sleep(0.01)
 
             notify_host = self._notify_host
             if endpoint == 'track/apm/analytics/txn':
                 notify_host = self._analytics_notify_host
 
             r = requests.post(notify_host + endpoint, params=self._post_params, timeout=30, json=data)
 
-            self._blocked = False
-
             if r.status_code == 200:
+                if endpoint != 'track/apm/analytics/txn':
+                    self._blocked = False
+
                 if endpoint == 'track/apm/hostinfo':
                     self._capture_percentiles = False
                     c = r.content
                     if not c:
                         return
 
                     c = c.decode('UTF-8')
 
                     resp = json.loads(c)
                     if resp:
+                        if "blocked" in resp:
+                            self._blocked = resp["blocked"]
+
                         if "analytics" in resp:
                             self._hostinfo_response["analytics"] = resp["analytics"]
 
                         if "capturePercentiles" in resp:
                             self._capture_percentiles = resp["capturePercentiles"]
                             self._hostinfo_response["capturePercentiles"] = self._capture_percentiles
 
@@ -76,25 +81,36 @@
                 if not c:
                     self._error_logger.error("Atatus transport status 400, failed without content")
                     return
 
                 if compat.PY3:
                     c = c.decode('UTF-8')
 
+                print_message = True
+                hostinfo_analytics = False
                 resp = json.loads(c)
                 if resp:
+                    if "analytics" in resp:
+                        self._hostinfo_response["analytics"] = resp["analytics"]
+
                     if "blocked" in resp:
                         self._blocked = resp["blocked"]
-                        if self._blocked is True:
-                            if "errorMessage" in resp:
-                                self._error_logger.error(
-                                    "Atatus blocked from sending data as: %s ", resp["errorMessage"])
-                                return
 
-                self._error_logger.error("Atatus transport status 400, failed with content: %r", c)
+                    if "analytics" in self._hostinfo_response:
+                        hostinfo_analytics = self._hostinfo_response["analytics"]
+                    
+                    if self._blocked and hostinfo_analytics and (endpoint != 'track/apm/analytics/txn'):
+                        print_message = False
+                    
+                    if print_message and "errorMessage" in resp:
+                        self._error_logger.error(
+                            "Atatus blocked from sending data as: %s ", resp["errorMessage"])
+
+                if print_message:
+                    self._error_logger.error("Atatus transport status 400, failed with content: %r", c)
                 return
 
             if r.status_code != 200:
                 self._error_logger.error(
                     "Atatus transport unexpected non-200 response [%s] [status_code: %r]." % (self._notify_host + endpoint, r.status_code))
 
         except Exception as e:
```

### Comparing `atatus-1.4.0/atatus/conf/__init__.py` & `atatus-1.5.0/atatus/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,14 +540,15 @@
 
 class Config(_ConfigBase):
     app_name = _ConfigValue("APP_NAME", default=None, required=True)
     version = _ConfigValue("APP_VERSION", default=None, required=False)
     license_key = _ConfigValue("LICENSE_KEY", default=None, required=True)
     notify_host = _ConfigValue("NOTIFY_HOST", default="https://apm-rx.atatus.com/", required=True)
     analytics = _BoolConfigValue("ANALYTICS", default=False, required=False)
+    analytics_capture_outgoing = _BoolConfigValue("ANALYTICS_CAPTURE_OUTGOING", default=False, required=False)
     analytics_notify_host = _ConfigValue("ANALYTICS_NOTIFY_HOST", default="https://an-rx.atatus.com/", required=True)
     trace_threshold = _DurationConfigValue(
         "TRACE_THRESHOLD",
         default=timedelta(seconds=2),
     )
 
     service_name = _ConfigValue(
```

### Comparing `atatus-1.4.0/atatus/conf/constants.py` & `atatus-1.5.0/atatus/conf/constants.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/context/__init__.py` & `atatus-1.5.0/atatus/context/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/context/base.py` & `atatus-1.5.0/atatus/context/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/context/contextvars.py` & `atatus-1.5.0/atatus/context/contextvars.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/context/threadlocal.py` & `atatus-1.5.0/atatus/context/threadlocal.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/__init__.py` & `atatus-1.5.0/atatus/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/aiohttp/__init__.py` & `atatus-1.5.0/atatus/contrib/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/aiohttp/middleware.py` & `atatus-1.5.0/atatus/contrib/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/aiohttp/utils.py` & `atatus-1.5.0/atatus/contrib/aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/asyncio/__init__.py` & `atatus-1.5.0/atatus/contrib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/asyncio/traces.py` & `atatus-1.5.0/atatus/contrib/asyncio/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/celery/__init__.py` & `atatus-1.5.0/atatus/contrib/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/__init__.py` & `atatus-1.5.0/atatus/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/apps.py` & `atatus-1.5.0/atatus/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/celery/__init__.py` & `atatus-1.5.0/atatus/contrib/django/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/celery/models.py` & `atatus-1.5.0/atatus/contrib/django/celery/models.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/client.py` & `atatus-1.5.0/atatus/contrib/django/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,15 @@
 
         if request.method in constants.HTTP_WITH_BODY:
             capture_body = self.config.capture_body in ("all", "request")
             if not capture_body:
                 result["body"] = "[REDACTED]"
             else:
                 content_type = request.META.get("CONTENT_TYPE")
-                if content_type == "application/x-www-form-urlencoded":
-                    data = compat.multidict_to_dict(request.POST)
-                elif content_type and content_type.startswith("multipart/form-data"):
+                if content_type and content_type.startswith("multipart/form-data"):
                     data = compat.multidict_to_dict(request.POST)
                     if request.FILES:
                         data["_files"] = {field: file.name for field, file in request.FILES.items()}
                 else:
                     try:
                         if isinstance(request.body, bytes):
                             data = self.body_decode(request.body)
```

### Comparing `atatus-1.4.0/atatus/contrib/django/context_processors.py` & `atatus-1.5.0/atatus/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/handlers.py` & `atatus-1.5.0/atatus/contrib/django/handlers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/management/__init__.py` & `atatus-1.5.0/atatus/contrib/django/management/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/management/commands/__init__.py` & `atatus-1.5.0/atatus/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/management/commands/atatus.py` & `atatus-1.5.0/atatus/contrib/django/management/commands/atatus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/middleware/__init__.py` & `atatus-1.5.0/atatus/contrib/django/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/middleware/wsgi.py` & `atatus-1.5.0/atatus/contrib/django/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/django/utils.py` & `atatus-1.5.0/atatus/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/flask/__init__.py` & `atatus-1.5.0/atatus/contrib/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/flask/utils.py` & `atatus-1.5.0/atatus/contrib/flask/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentelemetry/__init__.py` & `atatus-1.5.0/atatus/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentelemetry/context.py` & `atatus-1.5.0/atatus/contrib/opentelemetry/context.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentelemetry/span.py` & `atatus-1.5.0/atatus/contrib/opentelemetry/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentelemetry/trace.py` & `atatus-1.5.0/atatus/contrib/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentelemetry/utils.py` & `atatus-1.5.0/atatus/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentracing/__init__.py` & `atatus-1.5.0/atatus/contrib/opentracing/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentracing/span.py` & `atatus-1.5.0/atatus/contrib/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/opentracing/tracer.py` & `atatus-1.5.0/atatus/contrib/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/paste.py` & `atatus-1.5.0/atatus/contrib/paste.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/pylons/__init__.py` & `atatus-1.5.0/atatus/contrib/pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/rq/__init__.py` & `atatus-1.5.0/atatus/contrib/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/sanic/__init__.py` & `atatus-1.5.0/atatus/contrib/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/sanic/patch.py` & `atatus-1.5.0/atatus/contrib/sanic/patch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/sanic/sanic_types.py` & `atatus-1.5.0/atatus/contrib/sanic/sanic_types.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/sanic/utils.py` & `atatus-1.5.0/atatus/contrib/sanic/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/serverless/__init__.py` & `atatus-1.5.0/atatus/contrib/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/serverless/aws.py` & `atatus-1.5.0/atatus/contrib/serverless/aws.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/starlette/__init__.py` & `atatus-1.5.0/atatus/contrib/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/starlette/utils.py` & `atatus-1.5.0/atatus/contrib/starlette/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/tornado/__init__.py` & `atatus-1.5.0/atatus/contrib/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/tornado/utils.py` & `atatus-1.5.0/atatus/contrib/tornado/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/contrib/twisted/__init__.py` & `atatus-1.5.0/atatus/contrib/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/events.py` & `atatus-1.5.0/atatus/events.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/handlers/__init__.py` & `atatus-1.5.0/atatus/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/handlers/logbook.py` & `atatus-1.5.0/atatus/handlers/logbook.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/handlers/logging.py` & `atatus-1.5.0/atatus/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/handlers/structlog.py` & `atatus-1.5.0/atatus/handlers/structlog.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/__init__.py` & `atatus-1.5.0/atatus/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/control.py` & `atatus-1.5.0/atatus/instrumentation/control.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiobotocore.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiobotocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiomysql.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiomysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/aiopg.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiopg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/aioredis.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aioredis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/asyncpg.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/asyncpg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/base.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/elasticsearch.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/asyncio/sleep.py` & `atatus-1.5.0/atatus/instrumentation/packages/asyncio/sleep.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/azure.py` & `atatus-1.5.0/atatus/instrumentation/packages/azure.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/base.py` & `atatus-1.5.0/atatus/instrumentation/packages/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/botocore.py` & `atatus-1.5.0/atatus/instrumentation/packages/botocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/cassandra.py` & `atatus-1.5.0/atatus/instrumentation/packages/cassandra.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/dbapi2.py` & `atatus-1.5.0/atatus/instrumentation/packages/dbapi2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/django/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/django/template.py` & `atatus-1.5.0/atatus/instrumentation/packages/django/template.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/elasticsearch.py` & `atatus-1.5.0/atatus/instrumentation/packages/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/graphql.py` & `atatus-1.5.0/atatus/instrumentation/packages/graphql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httplib2.py` & `atatus-1.5.0/atatus/instrumentation/packages/httplib2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/async/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/async/httpcore.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/async/httpx.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/__init__.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/httpcore.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/sync/httpx.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/httpx/utils.py` & `atatus-1.5.0/atatus/instrumentation/packages/httpx/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/jinja2.py` & `atatus-1.5.0/atatus/instrumentation/packages/jinja2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/kafka.py` & `atatus-1.5.0/atatus/instrumentation/packages/kafka.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/mysql.py` & `atatus-1.5.0/atatus/instrumentation/packages/mysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/mysql_connector.py` & `atatus-1.5.0/atatus/instrumentation/packages/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/psycopg2.py` & `atatus-1.5.0/atatus/instrumentation/packages/psycopg2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pylibmc.py` & `atatus-1.5.0/atatus/instrumentation/packages/pylibmc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pymemcache.py` & `atatus-1.5.0/atatus/instrumentation/packages/pymemcache.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pymongo.py` & `atatus-1.5.0/atatus/instrumentation/packages/pymongo.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pymssql.py` & `atatus-1.5.0/atatus/instrumentation/packages/pymssql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pymysql.py` & `atatus-1.5.0/atatus/instrumentation/packages/pymysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/pyodbc.py` & `atatus-1.5.0/atatus/instrumentation/packages/pyodbc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/python_memcached.py` & `atatus-1.5.0/atatus/instrumentation/packages/python_memcached.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/redis.py` & `atatus-1.5.0/atatus/instrumentation/packages/redis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/requests.py` & `atatus-1.5.0/atatus/instrumentation/packages/zlib.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,39 +26,17 @@
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from atatus.instrumentation.packages.base import AbstractInstrumentedModule
 from atatus.traces import capture_span
-from atatus.utils import get_host_from_url, sanitize_url
 
 
-class RequestsInstrumentation(AbstractInstrumentedModule):
-    name = "requests"
-
-    instrument_list = [("requests.sessions", "Session.send")]
+class ZLibInstrumentation(AbstractInstrumentedModule):
+    name = "zlib"
+    instrument_list = [("zlib", "compress"), ("zlib", "decompress")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
-        if "request" in kwargs:
-            request = kwargs["request"]
-        else:
-            request = args[0]
-
-        signature = request.method.upper()
-        signature += " " + get_host_from_url(request.url)
-        url = sanitize_url(request.url)
-
-        with capture_span(
-            signature,
-            span_type="external",
-            span_subtype="http",
-            extra={"http": {"url": url}},
-            leaf=True,
-        ) as span:
-            response = wrapped(*args, **kwargs)
-            # requests.Response objects are falsy if status code > 400, so we have to check for None instead
-            if response is not None:
-                if span.context:
-                    span.context["http"]["status_code"] = response.status_code
-                span.set_success() if response.status_code < 400 else span.set_failure()
-            return response
+        wrapped_name = module + "." + method
+        with capture_span(wrapped_name, span_type="compression", span_subtype="zlib"):
+            return wrapped(*args, **kwargs)
```

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/sqlite.py` & `atatus-1.5.0/atatus/instrumentation/packages/sqlite.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/tornado.py` & `atatus-1.5.0/atatus/instrumentation/packages/tornado.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/urllib.py` & `atatus-1.5.0/atatus/instrumentation/packages/urllib.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/urllib3.py` & `atatus-1.5.0/atatus/instrumentation/packages/urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/instrumentation/packages/zlib.py` & `atatus-1.5.0/atatus/transport/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# -*- coding: utf-8 -*-
+
+
 #  BSD 3-Clause License
 #
 #  Copyright (c) 2019, Elasticsearch BV
 #  All rights reserved.
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are met:
@@ -24,19 +27,13 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from atatus.instrumentation.packages.base import AbstractInstrumentedModule
-from atatus.traces import capture_span
-
-
-class ZLibInstrumentation(AbstractInstrumentedModule):
-    name = "zlib"
-    instrument_list = [("zlib", "compress"), ("zlib", "decompress")]
 
-    def call(self, module, method, wrapped, instance, args, kwargs):
-        wrapped_name = module + "." + method
-        with capture_span(wrapped_name, span_type="compression", span_subtype="zlib"):
-            return wrapped(*args, **kwargs)
+class TransportException(Exception):
+    def __init__(self, message, data=None, print_trace=True):
+        super(TransportException, self).__init__(message)
+        self.data = data
+        self.print_trace = print_trace
```

### Comparing `atatus-1.4.0/atatus/instrumentation/register.py` & `atatus-1.5.0/atatus/instrumentation/register.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/__init__.py` & `atatus-1.5.0/atatus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/base_metrics.py` & `atatus-1.5.0/atatus/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/__init__.py` & `atatus-1.5.0/atatus/metrics/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/breakdown.py` & `atatus-1.5.0/atatus/metrics/sets/breakdown.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/cpu.py` & `atatus-1.5.0/atatus/metrics/sets/cpu.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/cpu_linux.py` & `atatus-1.5.0/atatus/metrics/sets/cpu_linux.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/cpu_psutil.py` & `atatus-1.5.0/atatus/metrics/sets/cpu_psutil.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/metrics/sets/prometheus.py` & `atatus-1.5.0/atatus/metrics/sets/prometheus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/middleware.py` & `atatus-1.5.0/atatus/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/processors.py` & `atatus-1.5.0/atatus/processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/traces.py` & `atatus-1.5.0/atatus/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/transport/__init__.py` & `atatus-1.5.0/atatus/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/transport/base.py` & `atatus-1.5.0/atatus/transport/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/transport/exceptions.py` & `atatus-1.5.0/atatus/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# -*- coding: utf-8 -*-
-
-
 #  BSD 3-Clause License
 #
 #  Copyright (c) 2019, Elasticsearch BV
 #  All rights reserved.
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are met:
@@ -27,13 +24,9 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-
-class TransportException(Exception):
-    def __init__(self, message, data=None, print_trace=True):
-        super(TransportException, self).__init__(message)
-        self.data = data
-        self.print_trace = print_trace
+__version__ = (1, 5, 0)
+VERSION = ".".join(map(str, __version__))
```

### Comparing `atatus-1.4.0/atatus/transport/http.py` & `atatus-1.5.0/atatus/transport/http.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/transport/http_base.py` & `atatus-1.5.0/atatus/transport/http_base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/transport/http_urllib3.py` & `atatus-1.5.0/atatus/transport/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/__init__.py` & `atatus-1.5.0/atatus/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,29 @@
     host = parsed_url.hostname or " "
 
     if parsed_url.port and default_ports.get(parsed_url.scheme) != parsed_url.port:
         host += ":" + str(parsed_url.port)
 
     return host
 
+def get_external_headers(headers):
+    try:
+        headers = {k: v for k, v in headers.items()}
+    except:
+        headers = {}
+    return headers
+
+def external_body_decode(body):
+    if isinstance(body, bytes):
+        try:
+            string_data = body.decode('UTF-8')
+            return string_data
+        except:
+            pass
+    return body
 
 def url_to_destination_resource(url: str) -> str:
     parts = urllib.parse.urlsplit(url)
     hostname = parts.hostname if parts.hostname else ""
     # preserve brackets for IPv6 URLs
     if "://[" in url:
         hostname = "[%s]" % hostname
```

### Comparing `atatus-1.4.0/atatus/utils/cgroup.py` & `atatus-1.5.0/atatus/utils/cgroup.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/cloud.py` & `atatus-1.5.0/atatus/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/compat.py` & `atatus-1.5.0/atatus/utils/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,22 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import sys
 import atexit
 import functools
 import platform
 
 
+PY3 = sys.version_info[0] == 3
+
 def noop_decorator(func):
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapped
```

### Comparing `atatus-1.4.0/atatus/utils/deprecation.py` & `atatus-1.5.0/atatus/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/disttracing.py` & `atatus-1.5.0/atatus/utils/disttracing.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/encoding.py` & `atatus-1.5.0/atatus/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/hw_info.py` & `atatus-1.5.0/atatus/utils/hw_info.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/json_encoder.py` & `atatus-1.5.0/atatus/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/logging.py` & `atatus-1.5.0/atatus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/module_import.py` & `atatus-1.5.0/atatus/utils/module_import.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/stacks.py` & `atatus-1.5.0/atatus/utils/stacks.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/threading.py` & `atatus-1.5.0/atatus/utils/threading.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/time.py` & `atatus-1.5.0/atatus/utils/time.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/__init__.py` & `atatus-1.5.0/atatus/utils/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/_wrappers.c` & `atatus-1.5.0/atatus/utils/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/arguments.py` & `atatus-1.5.0/atatus/utils/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/decorators.py` & `atatus-1.5.0/atatus/utils/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/importer.py` & `atatus-1.5.0/atatus/utils/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wrapt/wrappers.py` & `atatus-1.5.0/atatus/utils/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus/utils/wsgi.py` & `atatus-1.5.0/atatus/utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/atatus.egg-info/PKG-INFO` & `atatus-1.5.0/atatus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.4.0
+Version: 1.5.0
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
@@ -35,16 +35,16 @@
         Copyright
         ----------
         
         Copyright (c) 2014-2023 Atatus. All rights reserved.
         
         
         .. _`Atatus Python APM agent`: https://www.atatus.com
-        .. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/django.html
-        .. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/flask.html
+        .. _`Django installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/django.html
+        .. _`Flask installation`: https://docs.atatus.com/docs/application-monitoring/python-agent/installation/flask.html
         .. _`Release notes`: https://docs.atatus.com/docs/release-notes/python.html
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

### Comparing `atatus-1.4.0/atatus.egg-info/SOURCES.txt` & `atatus-1.5.0/atatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/setup.cfg` & `atatus-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `atatus-1.4.0/setup.py` & `atatus-1.5.0/setup.py`

 * *Files identical despite different names*

