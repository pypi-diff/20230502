# Comparing `tmp/subdivisions-1.8.0.tar.gz` & `tmp/subdivisions-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdivisions-1.8.0.tar", last modified: Wed Jul 14 11:39:16 2021, max compression
+gzip compressed data, was "subdivisions-1.9.0.tar", last modified: Thu Aug 12 13:56:24 2021, max compression
```

## Comparing `subdivisions-1.8.0.tar` & `subdivisions-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4352 2021-07-14 11:38:48.976068 subdivisions-1.8.0/README.md
--rw-r--r--   0        0        0     1739 2021-07-14 11:38:56.004216 subdivisions-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       22 2021-07-14 11:38:56.004216 subdivisions-1.8.0/subdivisions/__init__.py
--rw-r--r--   0        0        0     2637 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/base.py
--rw-r--r--   0        0        0      768 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/builders/__init__.py
--rw-r--r--   0        0        0     3123 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/builders/events.py
--rw-r--r--   0        0        0     1991 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/builders/sns.py
--rw-r--r--   0        0        0     3234 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/builders/sqs.py
--rw-r--r--   0        0        0    11482 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/client.py
--rw-r--r--   0        0        0     6530 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/config.py
--rw-r--r--   0        0        0     1660 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/events.py
--rw-r--r--   0        0        0       43 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/exceptions.py
--rw-r--r--   0        0        0     1149 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/policies.py
--rw-r--r--   0        0        0      715 2021-07-14 11:38:48.976068 subdivisions-1.8.0/subdivisions/utils.py
--rw-r--r--   0        0        0     5117 1970-01-01 00:00:00.000000 subdivisions-1.8.0/setup.py
--rw-r--r--   0        0        0     5023 1970-01-01 00:00:00.000000 subdivisions-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4352 2021-08-12 13:55:43.731807 subdivisions-1.9.0/README.md
+-rw-r--r--   0        0        0     1739 2021-08-12 13:55:52.591944 subdivisions-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-08-12 13:55:52.591944 subdivisions-1.9.0/subdivisions/__init__.py
+-rw-r--r--   0        0        0     2637 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/base.py
+-rw-r--r--   0        0        0      768 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/builders/__init__.py
+-rw-r--r--   0        0        0     3123 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/builders/events.py
+-rw-r--r--   0        0        0     1991 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/builders/sns.py
+-rw-r--r--   0        0        0     3234 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/builders/sqs.py
+-rw-r--r--   0        0        0    11482 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/client.py
+-rw-r--r--   0        0        0     6530 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/config.py
+-rw-r--r--   0        0        0     1716 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/events.py
+-rw-r--r--   0        0        0       43 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/exceptions.py
+-rw-r--r--   0        0        0     1149 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/policies.py
+-rw-r--r--   0        0        0      715 2021-08-12 13:55:43.731807 subdivisions-1.9.0/subdivisions/utils.py
+-rw-r--r--   0        0        0     5117 1970-01-01 00:00:00.000000 subdivisions-1.9.0/setup.py
+-rw-r--r--   0        0        0     5023 1970-01-01 00:00:00.000000 subdivisions-1.9.0/PKG-INFO
```

### Comparing `subdivisions-1.8.0/README.md` & `subdivisions-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/pyproject.toml` & `subdivisions-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "subdivisions"
-version = "1.8.0"
+version = "1.9.0"
 description = "A55 AWS PubSub Library"
 authors = ["A55 Tech <tech@a55.tech>"]
 readme = "README.md"
 repository = "https://github.com/access55/subdivisions"
 keywords = ["pubsub"]
 license = "GPL-3.0"
```

### Comparing `subdivisions-1.8.0/subdivisions/base.py` & `subdivisions-1.9.0/subdivisions/base.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/builders/__init__.py` & `subdivisions-1.9.0/subdivisions/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/builders/events.py` & `subdivisions-1.9.0/subdivisions/builders/events.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/builders/sns.py` & `subdivisions-1.9.0/subdivisions/builders/sns.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/builders/sqs.py` & `subdivisions-1.9.0/subdivisions/builders/sqs.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/client.py` & `subdivisions-1.9.0/subdivisions/client.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/config.py` & `subdivisions-1.9.0/subdivisions/config.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/events.py` & `subdivisions-1.9.0/subdivisions/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     USER_LOGGED_IN = "user_logged_in"
 
 
 class AccountEvents(Enum):
     BANK_ACCOUNT_REGISTERED = "bank_account_registered"
     AD_ACCOUNT_REGISTERED = "google_ad_account_registered"
     POLISHED_STATEMENT_TABLE = "polished_statement_table"
+    STATEMENT_TABLE_UPDATED = "statement_table_updated"
 
 
 class ProposalEvents(Enum):
     PROPOSAL_SELECTED = "proposal_selected"
     PROPOSAL_APPROVED = "proposal_approved"
     PROPOSAL_ACCEPTED = "proposal_accepted"
     PROPOSAL_INDICATIVE = "proposal_indicative"
```

### Comparing `subdivisions-1.8.0/subdivisions/policies.py` & `subdivisions-1.9.0/subdivisions/policies.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/subdivisions/utils.py` & `subdivisions-1.9.0/subdivisions/utils.py`

 * *Files identical despite different names*

### Comparing `subdivisions-1.8.0/setup.py` & `subdivisions-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['arrow', 'asbool', 'boto3', 'loguru', 'python-dotenv', 'stringcase']
 
 setup_kwargs = {
     'name': 'subdivisions',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'A55 AWS PubSub Library',
     'long_description': '# Welcome to Subdivisions\n\n[![PyPI](https://img.shields.io/pypi/v/subdivisions)](https://pypi.org/project/subdivisions/)\n[![Publish](https://github.com/access55/subdivisions/workflows/publish/badge.svg)](https://github.com/access55/subdivisions/actions)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subdivisions)](https://www.python.org)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n[A55 Python library for PubSub Messaging](https://www.youtube.com/watch?v=EYYdQB0mkEU)\n\n### Install in Project\n\n```toml\n# pyproject.toml\n# Add in every project which will\n# receive or send messages\n[tool.subdivisions]\nsource_name = "ProjectName" # ex.: "Client-Manager"\n\n[tool.poetry.dependencies]\nsubdivisions = "*"\n```\nRun `poetry update`\n\n### Usage\n#### Send Messages\n```python\nfrom subdivisions.client import SubClient\nfrom subdivisions.events import UserEvents\n\nclient = SubClient()\nclient.topic = UserEvents.USER_REGISTERED\nclient.send({"foo": "bar"})\n```\n\n#### Receive Messages\n```python\nfrom subdivisions.client import SubClient\nfrom subdivisions.events import UserEvents\n\nclient = SubClient()\nclient.topic = UserEvents.USER_REGISTERED\nmessages = client.get_messages()\n# Process messages\nclient.delete_received_messages()  # use the ``from_dead_letter=True` to receive Dead Letter messages\n```\n\n#### Add new Topic\nTo avoid different names in different projects for the same topic, (i.e: "client_registered" and\n"customer_registered") please add new events using Python Enum on `subdivisions.event` module:\n\n```python\n# subdivisions.events\nfrom enum import unique, Enum\n\n@unique\nclass MyNewEvents(Enum):\n    MY_NEW_EVENT = "my_new_event"\n```\n\nThen upload a new pypi version, using the provided Github Actions workflows. This new topic will be created in AWS\n(Eventbridge Rules, SQS Queues and SNS topics) when you send his first new message.\n\n### AWS Credentials\n\nSubdivisions will use AWS default environment variables. If you need to define another credentials, use the following variables:\n\n```env\nSUBDIVISIONS_USE_AWS_ENV_VARS="false"\nSUBDIVISIONS_AWS_ACCESS_KEY_ID="your id"\nSUBDIVISIONS_AWS_SECRET_ACCESS_KEY="your key"\nSUBDIVISIONS_AWS_SESSION_TOKEN="your token" # optional\n```\n\n### Configuration\n\nConfigure subdivisions options in `pyproject.toml` file, inside `[tool.subdivisions]` table:\n\n```toml\n# pyproject.toml\n[tool.subdivisions]\naws_region = "us-east-1"            # AWS Region\npub_key = "alias/PubSubKey"         # KMS PubSubKey (must be created first)\nsqs_tags = []                       # SQS tags for new queues. Example [{"foo": "bar"}]\nqueue_prefix = ""                   # Prefix for new SQS queues\nqueue_suffix = ""                   # Suffix for new SQS queues\nqueue_max_receive_count = 1000      # SQS MaxReceiveCount setting\nsns_prefix = ""                     # Prefix for new SNS topics\nsns_suffix = ""                     # Suffix for new SNS topics\nsns_tags = []                       # SNS tags for new topics. Example [{"foo": "bar"}]\nevent_prefix = ""                   # Prefix for new Eventbride rules\nevent_suffix = ""                   # Suffix for new Eventbride rules\nevent_tags = []                     # Eventbridge tags for new rules. Example [{"foo": "bar"}]\nevent_bus = "default"               # Eventbridge Bus\nsource_name = ""                    # Eventbridge default source name. No default, must inform\nauto_create_new_topic = true        # Auto create new topic if not exists in Eventbridge\nauto_remove_from_queue = false      # Acknowledge first messages on receive\nuse_aws_env_vars = true             # Use AWS default env vars. If false append "SUBDIVISION_" on env vars. Example: "SUBDIVISION_AWS_ACCESS_KEY_ID"\ndefault_prefix = "a55"              # Default prefix for all sns, sqs and rule created\ndefault_suffix = ""                 # Default suffix for all sns, sqs and rule created\n```\n\nAll options above can be configured in environment variables. Just append `SUBDIVISIONS_` on name. Example: `SUBDIVISIONS_SOURCE_NAME="my_project"`\n',
     'author': 'A55 Tech',
     'author_email': 'tech@a55.tech',
     'url': 'https://github.com/access55/subdivisions',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `subdivisions-1.8.0/PKG-INFO` & `subdivisions-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdivisions
-Version: 1.8.0
+Version: 1.9.0
 Summary: A55 AWS PubSub Library
 Home-page: https://github.com/access55/subdivisions
 License: GPL-3.0
 Keywords: pubsub
 Author: A55 Tech
 Author-email: tech@a55.tech
 Requires-Python: >=3.7,<4.0
```

