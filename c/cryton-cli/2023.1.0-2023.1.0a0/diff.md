# Comparing `tmp/cryton_cli-2023.1.0.tar.gz` & `tmp/cryton_cli-2023.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryton_cli-2023.1.0.tar", max compression
+gzip compressed data, was "cryton_cli-2023.1.0a0.tar", max compression
```

## Comparing `cryton_cli-2023.1.0.tar` & `cryton_cli-2023.1.0a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1075 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/LICENSE
--rw-r--r--   0        0        0     1629 2023-03-09 11:37:14.195759 cryton_cli-2023.1.0/README.md
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/etc/__init__.py
--rw-r--r--   0        0        0      601 2023-03-03 18:48:26.810411 cryton_cli-2023.1.0/cryton_cli/etc/config.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/__init__.py
--rwxr-xr-x   0        0        0     2468 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/cli.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/__init__.py
--rw-r--r--   0        0        0      341 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/dynamic_runs.py
--rw-r--r--   0        0        0     5034 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/execution_variable.py
--rw-r--r--   0        0        0     1647 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/log.py
--rw-r--r--   0        0        0    14687 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/plan.py
--rw-r--r--   0        0        0     5040 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/plan_template.py
--rw-r--r--   0        0        0    13020 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/run.py
--rw-r--r--   0        0        0    13483 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/stage.py
--rw-r--r--   0        0        0    13255 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/step.py
--rw-r--r--   0        0        0     4840 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/commands/worker.py
--rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/__init__.py
--rw-r--r--   0        0        0     6553 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/api.py
--rw-r--r--   0        0        0       82 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/constants.py
--rw-r--r--   0        0        0    11462 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0/cryton_cli/lib/util/util.py
--rw-r--r--   0        0        0     1170 2023-03-09 11:37:14.195759 cryton_cli-2023.1.0/pyproject.toml
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0/setup.py
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1622 2023-02-16 14:29:50.890849 cryton_cli-2023.1.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/etc/__init__.py
+-rw-r--r--   0        0        0      573 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/etc/config.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/__init__.py
+-rwxr-xr-x   0        0        0     2468 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/cli.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/__init__.py
+-rw-r--r--   0        0        0      341 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/dynamic_runs.py
+-rw-r--r--   0        0        0     5034 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/execution_variable.py
+-rw-r--r--   0        0        0     1647 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/log.py
+-rw-r--r--   0        0        0    14687 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/plan.py
+-rw-r--r--   0        0        0     5040 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/plan_template.py
+-rw-r--r--   0        0        0    13020 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/run.py
+-rw-r--r--   0        0        0    13483 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/stage.py
+-rw-r--r--   0        0        0    13255 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/step.py
+-rw-r--r--   0        0        0     4840 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/commands/worker.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/util/__init__.py
+-rw-r--r--   0        0        0     6553 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/util/api.py
+-rw-r--r--   0        0        0       82 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/util/constants.py
+-rw-r--r--   0        0        0    11462 2023-02-08 20:29:51.389499 cryton_cli-2023.1.0a0/cryton_cli/lib/util/util.py
+-rw-r--r--   0        0        0     1152 2023-02-16 12:35:41.489165 cryton_cli-2023.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0a0/setup.py
+-rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 cryton_cli-2023.1.0a0/PKG-INFO
```

### Comparing `cryton_cli-2023.1.0/LICENSE` & `cryton_cli-2023.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/README.md` & `cryton_cli-2023.1.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Quick-start
 Please keep in mind that [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) must be running and its REST API must be reachable.
 
 Make sure [Docker](https://docs.docker.com/engine/install/) is installed.
-Optionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
+Optionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
 
 The following script starts an interactive shell using Docker. 
 ```shell
-docker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli
+docker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli:latest
 ```
 
 Use the following to invoke the app:
 ```shell
 cryton-cli
 ```
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Contributing
 Contributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.
-For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).
+For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).
```

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/cli.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/cli.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/execution_variable.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/execution_variable.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/log.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/log.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/plan.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/plan.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/plan_template.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/plan_template.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/run.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/run.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/stage.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/stage.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/step.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/step.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/commands/worker.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/commands/worker.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/util/api.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/util/api.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/cryton_cli/lib/util/util.py` & `cryton_cli-2023.1.0a0/cryton_cli/lib/util/util.py`

 * *Files identical despite different names*

### Comparing `cryton_cli-2023.1.0/pyproject.toml` & `cryton_cli-2023.1.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryton-cli"
-version = "2023.1.0"
+version = "2023.1.0a0"
 description = "Command line interface for Cryton Core"
 authors = [
     "Ivo Nutár <nutar@ics.muni.cz>",
     "Milan Boháček <bohacek@ics.muni.cz>",
     "Jiří Rája <raja@ics.muni.cz>",
     "Andrej Tomči <tomci@ics.muni.cz>"
 ]
@@ -18,31 +18,30 @@
 documentation = "https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/"
 keywords = [
     "cryton", "cli", "client"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-PyYAML = "^6.0"
-Jinja2 = "^3.0.3"
-pyfiglet = "^0.8.post1"
-termcolor = "^2.2.0"
-requests = "^2.27.0"
-click = "^8.1.2"
-tzlocal = "^4.1"
-pytz = "^2022.7"
-python-dotenv = "^1.0.0"
+python = "^3.8"
+PyYAML = "~6.0"
+Jinja2 = "~3.0.3"
+pyfiglet = "~0.8.post1"
+termcolor = "~1.1.0"
+requests = "~2.27.0"
+click = "~8.1.2"
+tzlocal = "~4.1"
+pytz = "~2021.3"
+python-dotenv = "~0.20.0"
 
-[tool.poetry.group.dev.dependencies]
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-pytest-mock = "^3.6.1"
-requests-mock = "^1.9.3"
-tox = "^4.4.4"
+[tool.poetry.dev-dependencies]
+pytest = "~6.2.5"
+pytest-cov = "~3.0.0"
+pytest-mock = "~3.6.1"
+requests-mock = "~1.9.3"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cryton-cli = 'cryton_cli.lib.cli:cli'
```

### Comparing `cryton_cli-2023.1.0/setup.py` & `cryton_cli-2023.1.0a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,39 @@
  'cryton_cli.lib.commands',
  'cryton_cli.lib.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Jinja2>=3.0.3,<4.0.0',
- 'PyYAML>=6.0,<7.0',
- 'click>=8.1.2,<9.0.0',
+['Jinja2>=3.0.3,<3.1.0',
+ 'PyYAML>=6.0,<6.1',
+ 'click>=8.1.2,<8.2.0',
  'pyfiglet>=0.8.post1,<0.9',
- 'python-dotenv>=1.0.0,<2.0.0',
- 'pytz>=2022.7,<2023.0',
- 'requests>=2.27.0,<3.0.0',
- 'termcolor>=2.2.0,<3.0.0',
- 'tzlocal>=4.1,<5.0']
+ 'python-dotenv>=0.20.0,<0.21.0',
+ 'pytz>=2021.3,<2021.4',
+ 'requests>=2.27.0,<2.28.0',
+ 'termcolor>=1.1.0,<1.2.0',
+ 'tzlocal>=4.1,<4.2']
 
 entry_points = \
 {'console_scripts': ['cryton-cli = cryton_cli.lib.cli:cli']}
 
 setup_kwargs = {
     'name': 'cryton-cli',
-    'version': '2023.1.0',
+    'version': '2023.1.0a0',
     'description': 'Command line interface for Cryton Core',
-    'long_description': '![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-cli/badges/master/coverage.svg)\n\n[//]: # (TODO: add badges for python versions, black, pylint, flake8, unit tests, integration tests)\n\n# Cryton CLI\nCryton CLI is a command line interface used to interact with [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) (its API).\n\nCryton toolset is tested and targeted primarily on **Debian** and **Kali Linux**. Please keep in mind that **only \nthe latest version is supported** and issues regarding different OS or distributions may **not** be resolved.\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Quick-start\nPlease keep in mind that [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) must be running and its REST API must be reachable.\n\nMake sure [Docker](https://docs.docker.com/engine/install/) is installed.\nOptionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).\n\nThe following script starts an interactive shell using Docker. \n```shell\ndocker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli\n```\n\nUse the following to invoke the app:\n```shell\ncryton-cli\n```\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Contributing\nContributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.\nFor more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).\n',
+    'long_description': '![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-cli/badges/master/coverage.svg)\n\n[//]: # (TODO: add badges for python versions, black, pylint, flake8, unit tests, integration tests)\n\n# Cryton CLI\nCryton CLI is a command line interface used to interact with [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) (its API).\n\nCryton toolset is tested and targeted primarily on **Debian** and **Kali Linux**. Please keep in mind that **only \nthe latest version is supported** and issues regarding different OS or distributions may **not** be resolved.\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Quick-start\nPlease keep in mind that [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) must be running and its REST API must be reachable.\n\nMake sure [Docker](https://docs.docker.com/engine/install/) is installed.\nOptionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).\n\nThe following script starts an interactive shell using Docker. \n```shell\ndocker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli:latest\n```\n\nUse the following to invoke the app:\n```shell\ncryton-cli\n```\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Contributing\nContributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.\nFor more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).\n',
     'author': 'Ivo Nutár',
     'author_email': 'nutar@ics.muni.cz',
     'maintainer': 'Jiří Rája',
     'maintainer_email': 'raja@ics.muni.cz',
     'url': 'https://gitlab.ics.muni.cz/cryton',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `cryton_cli-2023.1.0/PKG-INFO` & `cryton_cli-2023.1.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cryton-cli
-Version: 2023.1.0
+Version: 2023.1.0a0
 Summary: Command line interface for Cryton Core
 Home-page: https://gitlab.ics.muni.cz/cryton
 License: MIT
 Keywords: cryton,cli,client
 Author: Ivo Nutár
 Author-email: nutar@ics.muni.cz
 Maintainer: Jiří Rája
 Maintainer-email: raja@ics.muni.cz
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: Jinja2 (>=3.0.3,<3.1.0)
+Requires-Dist: PyYAML (>=6.0,<6.1)
+Requires-Dist: click (>=8.1.2,<8.2.0)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pytz (>=2022.7,<2023.0)
-Requires-Dist: requests (>=2.27.0,<3.0.0)
-Requires-Dist: termcolor (>=2.2.0,<3.0.0)
-Requires-Dist: tzlocal (>=4.1,<5.0)
+Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: pytz (>=2021.3,<2021.4)
+Requires-Dist: requests (>=2.27.0,<2.28.0)
+Requires-Dist: termcolor (>=1.1.0,<1.2.0)
+Requires-Dist: tzlocal (>=4.1,<4.2)
 Project-URL: Documentation, https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/
 Project-URL: Repository, https://gitlab.ics.muni.cz/cryton/cryton-cli
 Description-Content-Type: text/markdown
 
 ![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-cli/badges/master/coverage.svg)
 
 [//]: # (TODO: add badges for python versions, black, pylint, flake8, unit tests, integration tests)
@@ -41,25 +41,25 @@
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Quick-start
 Please keep in mind that [Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core) must be running and its REST API must be reachable.
 
 Make sure [Docker](https://docs.docker.com/engine/install/) is installed.
-Optionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
+Optionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
 
 The following script starts an interactive shell using Docker. 
 ```shell
-docker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli
+docker run -it --network host registry.gitlab.ics.muni.cz:443/cryton/cryton-cli:latest
 ```
 
 Use the following to invoke the app:
 ```shell
 cryton-cli
 ```
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Contributing
 Contributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.
-For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).
+For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).
```

