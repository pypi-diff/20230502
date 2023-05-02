# Comparing `tmp/faceid-lib-2.0.0.tar.gz` & `tmp/faceid-lib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid-lib-2.0.0.tar", max compression
+gzip compressed data, was "faceid-lib-2.0.1.tar", max compression
```

## Comparing `faceid-lib-2.0.0.tar` & `faceid-lib-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     2346 2022-06-14 05:21:55.555469 faceid-lib-2.0.0/README.md
--rw-r--r--   0        0        0      494 2022-06-14 05:37:08.275407 faceid-lib-2.0.0/faceid_lib/CHANGELOG.md
--rw-r--r--   0        0        0      207 2022-06-14 05:34:42.430362 faceid-lib-2.0.0/faceid_lib/Makefile
--rw-r--r--   0        0        0       22 2021-09-08 03:10:42.869012 faceid-lib-2.0.0/faceid_lib/__init__.py
--rw-r--r--   0        0        0       89 2021-09-08 03:10:42.869614 faceid-lib-2.0.0/faceid_lib/__main__.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.869886 faceid-lib-2.0.0/faceid_lib/events/__init__.py
--rw-r--r--   0        0        0     2457 2021-11-24 01:10:13.748662 faceid-lib-2.0.0/faceid_lib/events/event_producer.py
--rw-r--r--   0        0        0     2389 2021-11-24 01:10:07.200887 faceid-lib-2.0.0/faceid_lib/events/event_receiver.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.872032 faceid-lib-2.0.0/faceid_lib/logger/__init__.py
--rw-r--r--   0        0        0      199 2021-09-08 03:10:42.872966 faceid-lib-2.0.0/faceid_lib/logger/logger_helper.py
--rw-r--r--   0        0        0     2220 2022-06-14 06:03:39.559713 faceid-lib-2.0.0/faceid_lib/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1754 2021-10-24 16:39:30.134988 faceid-lib-2.0.0/faceid_lib/ratelimiter/depends.py
--rw-r--r--   0        0        0        0 2021-09-08 03:10:42.873272 faceid-lib-2.0.0/faceid_lib/workflow/__init__.py
--rw-r--r--   0        0        0      284 2021-09-08 03:10:42.873899 faceid-lib-2.0.0/faceid_lib/workflow/workflow_helper.py
--rw-r--r--   0        0        0     1253 2022-06-14 06:04:55.101125 faceid-lib-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3461 2022-06-14 06:06:09.481871 faceid-lib-2.0.0/setup.py
--rw-r--r--   0        0        0     3512 2022-06-14 06:06:09.482317 faceid-lib-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2640 2023-05-02 16:15:31.835306 faceid-lib-2.0.1/README.md
+-rw-r--r--   0        0        0      590 2023-05-02 16:07:58.988298 faceid-lib-2.0.1/faceid_lib/CHANGELOG.md
+-rw-r--r--   0        0        0      207 2022-06-14 05:34:42.430362 faceid-lib-2.0.1/faceid_lib/Makefile
+-rw-r--r--   0        0        0       22 2021-09-08 03:10:42.869012 faceid-lib-2.0.1/faceid_lib/__init__.py
+-rw-r--r--   0        0        0       89 2021-09-08 03:10:42.869614 faceid-lib-2.0.1/faceid_lib/__main__.py
+-rw-r--r--   0        0        0        0 2021-09-08 03:10:42.869886 faceid-lib-2.0.1/faceid_lib/events/__init__.py
+-rw-r--r--   0        0        0     2457 2021-11-24 01:10:13.748662 faceid-lib-2.0.1/faceid_lib/events/event_producer.py
+-rw-r--r--   0        0        0     2389 2021-11-24 01:10:07.200887 faceid-lib-2.0.1/faceid_lib/events/event_receiver.py
+-rw-r--r--   0        0        0        0 2021-09-08 03:10:42.872032 faceid-lib-2.0.1/faceid_lib/logger/__init__.py
+-rw-r--r--   0        0        0      199 2021-09-08 03:10:42.872966 faceid-lib-2.0.1/faceid_lib/logger/logger_helper.py
+-rw-r--r--   0        0        0     2220 2022-06-14 06:03:39.559713 faceid-lib-2.0.1/faceid_lib/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     2579 2021-10-24 16:39:30.131894 faceid-lib-2.0.1/faceid_lib/ratelimiter/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1735 2021-10-24 16:39:30.133523 faceid-lib-2.0.1/faceid_lib/ratelimiter/__pycache__/depends.cpython-39.pyc
+-rw-r--r--   0        0        0     1754 2021-10-24 16:39:30.134988 faceid-lib-2.0.1/faceid_lib/ratelimiter/depends.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:06:17.257207 faceid-lib-2.0.1/faceid_lib/vector_similarity/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:06:29.895236 faceid-lib-2.0.1/faceid_lib/vector_similarity/v1/__init__.py
+-rw-r--r--   0        0        0     1263 2023-05-02 16:03:47.093803 faceid-lib-2.0.1/faceid_lib/vector_similarity/v1/power.py
+-rw-r--r--   0        0        0        0 2021-09-08 03:10:42.873272 faceid-lib-2.0.1/faceid_lib/workflow/__init__.py
+-rw-r--r--   0        0        0      284 2021-09-08 03:10:42.873899 faceid-lib-2.0.1/faceid_lib/workflow/workflow_helper.py
+-rw-r--r--   0        0        0     1253 2023-05-02 16:15:39.931279 faceid-lib-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3833 2023-05-02 16:18:08.579347 faceid-lib-2.0.1/setup.py
+-rw-r--r--   0        0        0     3806 2023-05-02 16:18:08.579867 faceid-lib-2.0.1/PKG-INFO
```

### Comparing `faceid-lib-2.0.0/README.md` & `faceid-lib-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Supported functionality:
 
 - API to communicate with RabbitMQ for event receiver/producer
 - Workflow call helper
 - Logger call helper
 - Rate-limiting strategies
+- Computing vector similarity helper (ex. Face Similarity Search)
 
 ## Author
 picaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan
 
 ## Instructions
 Version number should be updated in __init__.py and pyproject.toml
 
@@ -106,17 +107,25 @@
 │       └── depends.py
 │   ├── logger
 │       ├── __init__.py
 │       └── logger_helper.py
 │   ├── workflow
 │       ├── __init__.py
 │       └── workflow_helper.py
+│   ├── vector_similarity
+│       ├── __init__.py
+│       ├── v1
+│           ├── __init__.py
+│           └── power.py
 └── README.md
 ```
 
+## Changelogs 2.0.0 - 2.0.1 (2023-05-02)
+- compute similarity helper
+
 ## Changelogs 1.0.9 (2022-06-14)
 - modify response & handler
 
 ## Changelogs 1.0.5 (2021-10-24)
 - downgrade pika version to 1.1.0
 
 ## Changelogs 1.0.4 (2021-10-24)
```

### Comparing `faceid-lib-2.0.0/faceid_lib/events/event_producer.py` & `faceid-lib-2.0.1/faceid_lib/events/event_producer.py`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.0/faceid_lib/events/event_receiver.py` & `faceid-lib-2.0.1/faceid_lib/events/event_receiver.py`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.0/faceid_lib/ratelimiter/__init__.py` & `faceid-lib-2.0.1/faceid_lib/ratelimiter/__init__.py`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.0/faceid_lib/ratelimiter/depends.py` & `faceid-lib-2.0.1/faceid_lib/ratelimiter/depends.py`

 * *Files identical despite different names*

### Comparing `faceid-lib-2.0.0/pyproject.toml` & `faceid-lib-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faceid-lib"
-version = "2.0.0"
+version = "2.0.1"
 description = "Simple and flexible AI/ML workflow engine by Picaso - FaceID"
 authors = ["Dani Gunawan <danigunawan.elektroug@gmail.com>"]
 # New attributes
 license = "Apache License"
 readme = "README.md"
 homepage = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
 repository = "https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib"
```

### Comparing `faceid-lib-2.0.0/setup.py` & `faceid-lib-2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 from setuptools import setup
 
 packages = \
 ['faceid_lib',
  'faceid_lib.events',
  'faceid_lib.logger',
  'faceid_lib.ratelimiter',
+ 'faceid_lib.vector_similarity',
+ 'faceid_lib.vector_similarity.v1',
  'faceid_lib.workflow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aioredis==1.3.1', 'fastapi', 'pika>=1.2.0,<2.0.0', 'requests>=2.25.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['faceid-lib = faceid_lib:main']}
 
 setup_kwargs = {
     'name': 'faceid-lib',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Simple and flexible AI/ML workflow engine by Picaso - FaceID',
-    'long_description': '# picaso-engine ML faceid workflow\n\n## Overview\n\nThis is a helper library for picaso-engine ML faceid workflow product. The idea of this library is to wrap all reusable code to simplify and improve workflow implementation.\n\nSupported functionality:\n\n- API to communicate with RabbitMQ for event receiver/producer\n- Workflow call helper\n- Logger call helper\n- Rate-limiting strategies\n\n## Author\npicaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan\n\n## Instructions\nVersion number should be updated in __init__.py and pyproject.toml\n\n1. Install Poetry\n\n```\npip install poetry\n```\n\n2. Add pika and requests libraries\n\n```\npoetry add pika\npoetry add requests\n```\n\n3. Build\n\n```\npoetry lock --no-update\npoetry install\npoetry build\n```\n\n4. Publish to TestPyPI\n\n```\npoetry publish -r testpypi\n```\n\n5. Install from TestPyPI\n\n```\npip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple  faceid-lib\n```\n\n6. Publish to PyPI\n\n```\npoetry publish\n```\n\n7. Install from PyPI\n\n```\npip install faceid-lib\n```\n\n8. Test imported library from CMD\n\n```\npython -m faceid_lib\n```\n\n9. Import EventReceiver\n\n```\nfrom faceid_lib.events.event_receiver import EventReceiver\n```\n\n10. Import EventProducer\n\n```\nfrom faceid_lib.events.event_producer import EventProducer\n```\n\n11. Import FastAPILimiter, RateLimiter\n\n```\nfrom faceid_lib.ratelimiter import FastAPILimiter\nfrom faceid_lib.ratelimiter.depends import RateLimiter\n```\n\n## Structure\n\n```\n.\n├── LICENSE\n├── poetry.lock\n├── pyproject.toml\n├── faceid_lib\n│   ├── __init__.py\n│   ├── __main__.py\n│   ├── events\n│       ├── __init__.py\n│       ├── event_producer.py\n│       └── event_receiver.py\n│   ├── ratelimiter\n│       ├── __init__.py\n│       └── depends.py\n│   ├── logger\n│       ├── __init__.py\n│       └── logger_helper.py\n│   ├── workflow\n│       ├── __init__.py\n│       └── workflow_helper.py\n└── README.md\n```\n\n## Changelogs 1.0.9 (2022-06-14)\n- modify response & handler\n\n## Changelogs 1.0.5 (2021-10-24)\n- downgrade pika version to 1.1.0\n\n## Changelogs 1.0.4 (2021-10-24)\n- enhancment rate limiting\n\n## License\nLicensed under the Apache License, Version 2.0. Copyright 2020-2021 picaso-engine ML, Dani Gunawan.\n',
+    'long_description': '# picaso-engine ML faceid workflow\n\n## Overview\n\nThis is a helper library for picaso-engine ML faceid workflow product. The idea of this library is to wrap all reusable code to simplify and improve workflow implementation.\n\nSupported functionality:\n\n- API to communicate with RabbitMQ for event receiver/producer\n- Workflow call helper\n- Logger call helper\n- Rate-limiting strategies\n- Computing vector similarity helper (ex. Face Similarity Search)\n\n## Author\npicaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan\n\n## Instructions\nVersion number should be updated in __init__.py and pyproject.toml\n\n1. Install Poetry\n\n```\npip install poetry\n```\n\n2. Add pika and requests libraries\n\n```\npoetry add pika\npoetry add requests\n```\n\n3. Build\n\n```\npoetry lock --no-update\npoetry install\npoetry build\n```\n\n4. Publish to TestPyPI\n\n```\npoetry publish -r testpypi\n```\n\n5. Install from TestPyPI\n\n```\npip install -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple  faceid-lib\n```\n\n6. Publish to PyPI\n\n```\npoetry publish\n```\n\n7. Install from PyPI\n\n```\npip install faceid-lib\n```\n\n8. Test imported library from CMD\n\n```\npython -m faceid_lib\n```\n\n9. Import EventReceiver\n\n```\nfrom faceid_lib.events.event_receiver import EventReceiver\n```\n\n10. Import EventProducer\n\n```\nfrom faceid_lib.events.event_producer import EventProducer\n```\n\n11. Import FastAPILimiter, RateLimiter\n\n```\nfrom faceid_lib.ratelimiter import FastAPILimiter\nfrom faceid_lib.ratelimiter.depends import RateLimiter\n```\n\n## Structure\n\n```\n.\n├── LICENSE\n├── poetry.lock\n├── pyproject.toml\n├── faceid_lib\n│   ├── __init__.py\n│   ├── __main__.py\n│   ├── events\n│       ├── __init__.py\n│       ├── event_producer.py\n│       └── event_receiver.py\n│   ├── ratelimiter\n│       ├── __init__.py\n│       └── depends.py\n│   ├── logger\n│       ├── __init__.py\n│       └── logger_helper.py\n│   ├── workflow\n│       ├── __init__.py\n│       └── workflow_helper.py\n│   ├── vector_similarity\n│       ├── __init__.py\n│       ├── v1\n│           ├── __init__.py\n│           └── power.py\n└── README.md\n```\n\n## Changelogs 2.0.0 - 2.0.1 (2023-05-02)\n- compute similarity helper\n\n## Changelogs 1.0.9 (2022-06-14)\n- modify response & handler\n\n## Changelogs 1.0.5 (2021-10-24)\n- downgrade pika version to 1.1.0\n\n## Changelogs 1.0.4 (2021-10-24)\n- enhancment rate limiting\n\n## License\nLicensed under the Apache License, Version 2.0. Copyright 2020-2021 picaso-engine ML, Dani Gunawan.\n',
     'author': 'Dani Gunawan',
     'author_email': 'danigunawan.elektroug@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `faceid-lib-2.0.0/PKG-INFO` & `faceid-lib-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faceid-lib
-Version: 2.0.0
+Version: 2.0.1
 Summary: Simple and flexible AI/ML workflow engine by Picaso - FaceID
 Home-page: https://gitlab.playcourt.id/picaso-faceid/picaso-faceid-engine/v1/faceid-lib
 License: Apache License
 Keywords: machine learning,Deep Learning,Message Broker,Distributed System,pipeline,rabbitmq,ratelimiter
 Author: Dani Gunawan
 Author-email: danigunawan.elektroug@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -32,14 +32,15 @@
 
 Supported functionality:
 
 - API to communicate with RabbitMQ for event receiver/producer
 - Workflow call helper
 - Logger call helper
 - Rate-limiting strategies
+- Computing vector similarity helper (ex. Face Similarity Search)
 
 ## Author
 picaso-engine ML (https://pypi.org/project/faceid-lib/), Dani Gunawan
 
 ## Instructions
 Version number should be updated in __init__.py and pyproject.toml
 
@@ -132,17 +133,25 @@
 │       └── depends.py
 │   ├── logger
 │       ├── __init__.py
 │       └── logger_helper.py
 │   ├── workflow
 │       ├── __init__.py
 │       └── workflow_helper.py
+│   ├── vector_similarity
+│       ├── __init__.py
+│       ├── v1
+│           ├── __init__.py
+│           └── power.py
 └── README.md
 ```
 
+## Changelogs 2.0.0 - 2.0.1 (2023-05-02)
+- compute similarity helper
+
 ## Changelogs 1.0.9 (2022-06-14)
 - modify response & handler
 
 ## Changelogs 1.0.5 (2021-10-24)
 - downgrade pika version to 1.1.0
 
 ## Changelogs 1.0.4 (2021-10-24)
```

