# Comparing `tmp/cryton_worker-2023.1.0a0.tar.gz` & `tmp/cryton_worker-2023.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryton_worker-2023.1.0a0.tar", max compression
+gzip compressed data, was "cryton_worker-2023.1.1.tar", max compression
```

## Comparing `cryton_worker-2023.1.0a0.tar` & `cryton_worker-2023.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1075 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/LICENSE
--rw-r--r--   0        0        0     2843 2023-02-16 14:48:38.739418 cryton_worker-2023.1.0a0/README.md
--rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/etc/__init__.py
--rw-r--r--   0        0        0     1719 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/etc/config.py
--rw-r--r--   0        0        0      262 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/etc/systemd-service/cryton-executor.service
--rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/__init__.py
--rw-r--r--   0        0        0     3581 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/cli.py
--rw-r--r--   0        0        0    12617 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/consumer.py
--rw-r--r--   0        0        0    12213 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/empire.py
--rw-r--r--   0        0        0     4553 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/event.py
--rw-r--r--   0        0        0    12272 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/task.py
--rw-r--r--   0        0        0     1046 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/__init__.py
--rw-r--r--   0        0        0     3269 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_base.py
--rw-r--r--   0        0        0     6939 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_http.py
--rw-r--r--   0        0        0     6207 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_msf.py
--rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/__init__.py
--rw-r--r--   0        0        0     4205 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/constants.py
--rw-r--r--   0        0        0     1609 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/exceptions.py
--rw-r--r--   0        0        0     2703 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/logger.py
--rw-r--r--   0        0        0     2951 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/module_util.py
--rw-r--r--   0        0        0    18232 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/util/util.py
--rw-r--r--   0        0        0    13217 2023-02-08 20:33:07.288886 cryton_worker-2023.1.0a0/cryton_worker/lib/worker.py
--rw-r--r--   0        0        0     1343 2023-02-16 12:38:45.849027 cryton_worker-2023.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     4157 1970-01-01 00:00:00.000000 cryton_worker-2023.1.0a0/setup.py
--rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 cryton_worker-2023.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/LICENSE
+-rw-r--r--   0        0        0     2507 2023-03-09 21:23:55.851342 cryton_worker-2023.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/etc/__init__.py
+-rw-r--r--   0        0        0     1941 2023-03-08 21:34:30.409214 cryton_worker-2023.1.1/cryton_worker/etc/config.py
+-rw-r--r--   0        0        0      262 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/etc/systemd-service/cryton-executor.service
+-rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/__init__.py
+-rw-r--r--   0        0        0     3581 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/cli.py
+-rw-r--r--   0        0        0    12617 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/consumer.py
+-rw-r--r--   0        0        0    12213 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/empire.py
+-rw-r--r--   0        0        0     4553 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/event.py
+-rw-r--r--   0        0        0    12272 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/task.py
+-rw-r--r--   0        0        0     1046 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/triggers/__init__.py
+-rw-r--r--   0        0        0     3269 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_base.py
+-rw-r--r--   0        0        0     6939 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_http.py
+-rw-r--r--   0        0        0     6207 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_msf.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/__init__.py
+-rw-r--r--   0        0        0     4205 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/constants.py
+-rw-r--r--   0        0        0     1609 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/exceptions.py
+-rw-r--r--   0        0        0     2703 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/logger.py
+-rw-r--r--   0        0        0     2951 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/module_util.py
+-rw-r--r--   0        0        0    18232 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/util/util.py
+-rw-r--r--   0        0        0    13217 2023-02-08 20:33:07.288886 cryton_worker-2023.1.1/cryton_worker/lib/worker.py
+-rw-r--r--   0        0        0     1360 2023-03-09 21:46:36.153311 cryton_worker-2023.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 cryton_worker-2023.1.1/setup.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 cryton_worker-2023.1.1/PKG-INFO
```

### Comparing `cryton_worker-2023.1.0a0/LICENSE` & `cryton_worker-2023.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/README.md` & `cryton_worker-2023.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,33 +17,29 @@
 Modules provided by Cryton can be found [here](https://gitlab.ics.muni.cz/cryton/cryton-modules). **Their installation will
 be covered in this section**.
 
 Make sure Git, Docker, and Docker Compose plugin are installed:
 - [Git](https://git-scm.com/)
 - [Docker Compose](https://docs.docker.com/compose/install/)
 
-Optionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
+Optionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
 
 The following script clones the necessary repositories (Worker and modules), updates Worker's settings, and runs the 
 Docker Compose configuration which starts the Worker, and its prerequisites (Metasploit and Empire framework).
 ```shell
 git clone https://gitlab.ics.muni.cz/cryton/cryton-modules.git
 cd cryton-modules
 git checkout $(git tag --list "2023.1.*" | tail -n 1)
 cd ..
 export CRYTON_MODULES_PATH=$(pwd)/cryton-modules/modules
 git clone https://gitlab.ics.muni.cz/cryton/cryton-worker.git
 cd cryton-worker
 git checkout $(git tag --list "2023.1.*" | tail -n 1)
-sed -i "s|CRYTON_WORKER_NAME=CHANGE_ME|CRYTON_WORKER_NAME=LocalWorker|" .env
 sed -i "s|CRYTON_WORKER_MODULES_DIR=CHANGE_ME|CRYTON_WORKER_MODULES_DIR=$CRYTON_MODULES_PATH|" .env
-sed -i "s|CRYTON_WORKER_MSFRPCD_HOST=CHANGE_ME|CRYTON_WORKER_MSFRPCD_HOST=localhost|" .env
-sed -i "s|CRYTON_WORKER_RABBIT_HOST=CHANGE_ME|CRYTON_WORKER_RABBIT_HOST=localhost|" .env
-sed -i "s|CRYTON_WORKER_EMPIRE_HOST=CHANGE_ME|CRYTON_WORKER_EMPIRE_HOST=cryton-empire|" .env
 docker compose up -d
 ```
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Contributing
 Contributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.
-For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).
+For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).
```

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/etc/config.py` & `cryton_worker-2023.1.1/cryton_worker/etc/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from os import getenv, path, mkdir
 from dotenv import load_dotenv
 
 
-APP_DIRECTORY = getenv('CRYTON_WORKER_APP_DIRECTORY', path.expanduser("~/.local/cryton-worker/"))
+APP_DIRECTORY = getenv("CRYTON_WORKER_APP_DIRECTORY", path.expanduser("~/.local/cryton-worker/"))
 
 load_dotenv(path.join(APP_DIRECTORY, ".env"))
 
 LOG_DIRECTORY = path.join(APP_DIRECTORY, "log/")
 
 for file_path in [APP_DIRECTORY, LOG_DIRECTORY]:
     if not path.exists(file_path):
         mkdir(file_path)
 
 LOG_FILE_PATH = path.join(LOG_DIRECTORY, "cryton-worker.log")
 LOG_FILE_PATH_DEBUG = path.join(LOG_DIRECTORY, "cryton-worker-debug.log")
 
-WORKER_NAME = getenv("CRYTON_WORKER_NAME")
-MODULES_DIR = getenv("CRYTON_WORKER_MODULES_DIR")
-DEBUG = True if getenv("CRYTON_WORKER_DEBUG").lower() == "true" else False
-INSTALL_REQUIREMENTS = True if getenv("CRYTON_WORKER_INSTALL_REQUIREMENTS").lower() == "true" else False
-CONSUMER_COUNT = int(getenv("CRYTON_WORKER_CONSUMER_COUNT"))
-PROCESSOR_COUNT = int(getenv("CRYTON_WORKER_PROCESSOR_COUNT"))
-MAX_RETRIES = int(getenv("CRYTON_WORKER_MAX_RETRIES"))
-
-MSFRPCD_HOST = getenv("CRYTON_WORKER_MSFRPCD_HOST")
-MSFRPCD_PORT = int(getenv("CRYTON_WORKER_MSFRPCD_PORT"))
-MSFRPCD_SSL = True if getenv("CRYTON_WORKER_MSFRPCD_SSL").lower() == "true" else False
-MSFRPCD_PASSWORD = getenv("CRYTON_WORKER_MSFRPCD_PASSWORD")
-MSFRPCD_USERNAME = getenv("CRYTON_WORKER_MSFRPCD_USERNAME")
-
-RABBIT_HOST = getenv("CRYTON_WORKER_RABBIT_HOST")
-RABBIT_PORT = int(getenv("CRYTON_WORKER_RABBIT_PORT"))
-RABBIT_USERNAME = getenv("CRYTON_WORKER_RABBIT_USERNAME")
-RABBIT_PASSWORD = getenv("CRYTON_WORKER_RABBIT_PASSWORD")
-
-EMPIRE_HOST = getenv("CRYTON_WORKER_EMPIRE_HOST")
-EMPIRE_PORT = getenv("CRYTON_WORKER_EMPIRE_PORT")
-EMPIRE_USERNAME = getenv("CRYTON_WORKER_EMPIRE_USERNAME")
-EMPIRE_PASSWORD = getenv("CRYTON_WORKER_EMPIRE_PASSWORD")
+WORKER_NAME = getenv("CRYTON_WORKER_NAME", "Worker")
+MODULES_DIR = getenv("CRYTON_WORKER_MODULES_DIR")  # TODO: The default should point to the app directory
+DEBUG = True if getenv("CRYTON_WORKER_DEBUG", "false").lower() == "true" else False
+INSTALL_REQUIREMENTS = True if getenv("CRYTON_WORKER_INSTALL_REQUIREMENTS", "true").lower() == "true" else False
+CONSUMER_COUNT = int(getenv("CRYTON_WORKER_CONSUMER_COUNT", 7))
+PROCESSOR_COUNT = int(getenv("CRYTON_WORKER_PROCESSOR_COUNT", 7))
+MAX_RETRIES = int(getenv("CRYTON_WORKER_MAX_RETRIES", 3))
+
+MSFRPCD_HOST = getenv("CRYTON_WORKER_MSFRPCD_HOST", "127.0.0.1")
+MSFRPCD_PORT = int(getenv("CRYTON_WORKER_MSFRPCD_PORT", 55553))
+MSFRPCD_SSL = True if getenv("CRYTON_WORKER_MSFRPCD_SSL", "true").lower() == "true" else False
+MSFRPCD_PASSWORD = getenv("CRYTON_WORKER_MSFRPCD_PASSWORD", "cryton")
+MSFRPCD_USERNAME = getenv("CRYTON_WORKER_MSFRPCD_USERNAME", "cryton")
+
+RABBIT_HOST = getenv("CRYTON_WORKER_RABBIT_HOST", "127.0.0.1")
+RABBIT_PORT = int(getenv("CRYTON_WORKER_RABBIT_PORT", 5672))
+RABBIT_USERNAME = getenv("CRYTON_WORKER_RABBIT_USERNAME", "cryton")
+RABBIT_PASSWORD = getenv("CRYTON_WORKER_RABBIT_PASSWORD", "cryton")
+
+EMPIRE_HOST = getenv("CRYTON_WORKER_EMPIRE_HOST", "127.0.0.1")
+EMPIRE_PORT = int(getenv("CRYTON_WORKER_EMPIRE_PORT", 1337))
+EMPIRE_USERNAME = getenv("CRYTON_WORKER_EMPIRE_USERNAME", "cryton")
+EMPIRE_PASSWORD = getenv("CRYTON_WORKER_EMPIRE_PASSWORD", "cryton")
```

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/cli.py` & `cryton_worker-2023.1.1/cryton_worker/lib/cli.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/consumer.py` & `cryton_worker-2023.1.1/cryton_worker/lib/consumer.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/empire.py` & `cryton_worker-2023.1.1/cryton_worker/lib/empire.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/event.py` & `cryton_worker-2023.1.1/cryton_worker/lib/event.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/task.py` & `cryton_worker-2023.1.1/cryton_worker/lib/task.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/__init__.py` & `cryton_worker-2023.1.1/cryton_worker/lib/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_base.py` & `cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_base.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_http.py` & `cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_http.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/triggers/listener_msf.py` & `cryton_worker-2023.1.1/cryton_worker/lib/triggers/listener_msf.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/util/constants.py` & `cryton_worker-2023.1.1/cryton_worker/lib/util/constants.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/util/exceptions.py` & `cryton_worker-2023.1.1/cryton_worker/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/util/logger.py` & `cryton_worker-2023.1.1/cryton_worker/lib/util/logger.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/util/module_util.py` & `cryton_worker-2023.1.1/cryton_worker/lib/util/module_util.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/util/util.py` & `cryton_worker-2023.1.1/cryton_worker/lib/util/util.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/cryton_worker/lib/worker.py` & `cryton_worker-2023.1.1/cryton_worker/lib/worker.py`

 * *Files identical despite different names*

### Comparing `cryton_worker-2023.1.0a0/pyproject.toml` & `cryton_worker-2023.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryton-worker"
-version = "2023.1.0a0"
+version = "2023.1.1"
 description = "Attack scenario orchestrator for Cryton"
 authors = [
     "Ivo Nutár <nutar@ics.muni.cz>",
     "Milan Boháček <bohacek@ics.muni.cz>",
     "Jiří Rája <raja@ics.muni.cz>",
     "Andrej Tomči <tomci@ics.muni.cz>"
 ]
@@ -18,36 +18,37 @@
 documentation = "https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/"
 keywords = [
     "cryton", "worker", "orchestrator", "attacker"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pymetasploit3 = "~1.0.3"
-amqpstorm = "~2.10.4"
-structlog = "~21.5.0"
-PyYAML = "~6.0"
-schema = "~0.7.5"
-click = "~8.1.2"
-bottle = "~0.12.19"
-pyfiglet = "~0.8.post1"
-paramiko = "~2.11.0"
-requests = "~2.27.0"
-utinni = "~0.5.0"
-python-dotenv = "~0.20.0"
+python = ">=3.8,<3.12"
+pymetasploit3 = "^1.0.3"
+amqpstorm = "^2.10.4"
+structlog = "^22.3.0"
+PyYAML = "^6.0"
+schema = "^0.7.5"
+click = "^8.1.2"
+bottle = "^0.12.19"
+pyfiglet = "^0.8.post1"
+paramiko = "^3.0.0"
+requests = "^2.28.2"
+utinni = "^0.5.0"
+python-dotenv = "^1.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "~6.2.5"
-pytest-cov = "~3.0.0"
-pytest-asyncio = "~0.16.0"
-pytest-mock = "~3.6.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.2.5"
+pytest-cov = "^3.0.0"
+pytest-asyncio = "^0.16.0"
+pytest-mock = "^3.6.1"
+tox = "^4.4.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cryton-worker = 'cryton_worker.lib.cli:cli'
 
 [tool.pytest.ini_options]
 python_files = ["tests.py", "test_*.py", "*_tests.py"]
```

### Comparing `cryton_worker-2023.1.0a0/setup.py` & `cryton_worker-2023.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,42 +8,42 @@
  'cryton_worker.lib.triggers',
  'cryton_worker.lib.util']
 
 package_data = \
 {'': ['*'], 'cryton_worker.etc': ['systemd-service/*']}
 
 install_requires = \
-['PyYAML>=6.0,<6.1',
- 'amqpstorm>=2.10.4,<2.11.0',
+['PyYAML>=6.0,<7.0',
+ 'amqpstorm>=2.10.4,<3.0.0',
  'bottle>=0.12.19,<0.13.0',
- 'click>=8.1.2,<8.2.0',
- 'paramiko>=2.11.0,<2.12.0',
+ 'click>=8.1.2,<9.0.0',
+ 'paramiko>=3.0.0,<4.0.0',
  'pyfiglet>=0.8.post1,<0.9',
- 'pymetasploit3>=1.0.3,<1.1.0',
- 'python-dotenv>=0.20.0,<0.21.0',
- 'requests>=2.27.0,<2.28.0',
+ 'pymetasploit3>=1.0.3,<2.0.0',
+ 'python-dotenv>=1.0.0,<2.0.0',
+ 'requests>=2.28.2,<3.0.0',
  'schema>=0.7.5,<0.8.0',
- 'structlog>=21.5.0,<21.6.0',
+ 'structlog>=22.3.0,<23.0.0',
  'utinni>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['cryton-worker = cryton_worker.lib.cli:cli']}
 
 setup_kwargs = {
     'name': 'cryton-worker',
-    'version': '2023.1.0a0',
+    'version': '2023.1.1',
     'description': 'Attack scenario orchestrator for Cryton',
-    'long_description': '![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-worker/badges/master/coverage.svg)\n\n[//]: # (TODO: add badges for python versions, black, pylint, flake8, unit tests, integration tests)\n\n# Cryton Worker\nCryton Worker is used for executing attack modules remotely. It utilizes [RabbitMQ](https://www.rabbitmq.com/) \nas its asynchronous remote procedures call protocol. It connects to the Rabbit MQ server and consumes messages from \nthe Core component or any other app that implements its RabbitMQ API.\n\nCryton toolset is tested and targeted primarily on **Debian** and **Kali Linux**. Please keep in mind that **only \nthe latest version is supported** and issues regarding different OS or distributions may **not** be resolved.\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Quick-start\nTo be able to execute attack scenarios, you also need to install **[Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core)**.  \nModules provided by Cryton can be found [here](https://gitlab.ics.muni.cz/cryton/cryton-modules). **Their installation will\nbe covered in this section**.\n\nMake sure Git, Docker, and Docker Compose plugin are installed:\n- [Git](https://git-scm.com/)\n- [Docker Compose](https://docs.docker.com/compose/install/)\n\nOptionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).\n\nThe following script clones the necessary repositories (Worker and modules), updates Worker\'s settings, and runs the \nDocker Compose configuration which starts the Worker, and its prerequisites (Metasploit and Empire framework).\n```shell\ngit clone https://gitlab.ics.muni.cz/cryton/cryton-modules.git\ncd cryton-modules\ngit checkout $(git tag --list "2023.1.*" | tail -n 1)\ncd ..\nexport CRYTON_MODULES_PATH=$(pwd)/cryton-modules/modules\ngit clone https://gitlab.ics.muni.cz/cryton/cryton-worker.git\ncd cryton-worker\ngit checkout $(git tag --list "2023.1.*" | tail -n 1)\nsed -i "s|CRYTON_WORKER_NAME=CHANGE_ME|CRYTON_WORKER_NAME=LocalWorker|" .env\nsed -i "s|CRYTON_WORKER_MODULES_DIR=CHANGE_ME|CRYTON_WORKER_MODULES_DIR=$CRYTON_MODULES_PATH|" .env\nsed -i "s|CRYTON_WORKER_MSFRPCD_HOST=CHANGE_ME|CRYTON_WORKER_MSFRPCD_HOST=localhost|" .env\nsed -i "s|CRYTON_WORKER_RABBIT_HOST=CHANGE_ME|CRYTON_WORKER_RABBIT_HOST=localhost|" .env\nsed -i "s|CRYTON_WORKER_EMPIRE_HOST=CHANGE_ME|CRYTON_WORKER_EMPIRE_HOST=cryton-empire|" .env\ndocker compose up -d\n```\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Contributing\nContributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.\nFor more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).\n',
+    'long_description': '![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-worker/badges/master/coverage.svg)\n\n[//]: # (TODO: add badges for python versions, black, pylint, flake8, unit tests, integration tests)\n\n# Cryton Worker\nCryton Worker is used for executing attack modules remotely. It utilizes [RabbitMQ](https://www.rabbitmq.com/) \nas its asynchronous remote procedures call protocol. It connects to the Rabbit MQ server and consumes messages from \nthe Core component or any other app that implements its RabbitMQ API.\n\nCryton toolset is tested and targeted primarily on **Debian** and **Kali Linux**. Please keep in mind that **only \nthe latest version is supported** and issues regarding different OS or distributions may **not** be resolved.\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Quick-start\nTo be able to execute attack scenarios, you also need to install **[Cryton Core](https://gitlab.ics.muni.cz/cryton/cryton-core)**.  \nModules provided by Cryton can be found [here](https://gitlab.ics.muni.cz/cryton/cryton-modules). **Their installation will\nbe covered in this section**.\n\nMake sure Git, Docker, and Docker Compose plugin are installed:\n- [Git](https://git-scm.com/)\n- [Docker Compose](https://docs.docker.com/compose/install/)\n\nOptionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).\n\nThe following script clones the necessary repositories (Worker and modules), updates Worker\'s settings, and runs the \nDocker Compose configuration which starts the Worker, and its prerequisites (Metasploit and Empire framework).\n```shell\ngit clone https://gitlab.ics.muni.cz/cryton/cryton-modules.git\ncd cryton-modules\ngit checkout $(git tag --list "2023.1.*" | tail -n 1)\ncd ..\nexport CRYTON_MODULES_PATH=$(pwd)/cryton-modules/modules\ngit clone https://gitlab.ics.muni.cz/cryton/cryton-worker.git\ncd cryton-worker\ngit checkout $(git tag --list "2023.1.*" | tail -n 1)\nsed -i "s|CRYTON_WORKER_MODULES_DIR=CHANGE_ME|CRYTON_WORKER_MODULES_DIR=$CRYTON_MODULES_PATH|" .env\ndocker compose up -d\n```\n\nFor more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).\n\n## Contributing\nContributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.\nFor more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).\n',
     'author': 'Ivo Nutár',
     'author_email': 'nutar@ics.muni.cz',
     'maintainer': 'Jiří Rája',
     'maintainer_email': 'raja@ics.muni.cz',
     'url': 'https://gitlab.ics.muni.cz/cryton',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `cryton_worker-2023.1.0a0/PKG-INFO` & `cryton_worker-2023.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: cryton-worker
-Version: 2023.1.0a0
+Version: 2023.1.1
 Summary: Attack scenario orchestrator for Cryton
 Home-page: https://gitlab.ics.muni.cz/cryton
 License: MIT
 Keywords: cryton,worker,orchestrator,attacker
 Author: Ivo Nutár
 Author-email: nutar@ics.muni.cz
 Maintainer: Jiří Rája
 Maintainer-email: raja@ics.muni.cz
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<6.1)
-Requires-Dist: amqpstorm (>=2.10.4,<2.11.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: amqpstorm (>=2.10.4,<3.0.0)
 Requires-Dist: bottle (>=0.12.19,<0.13.0)
-Requires-Dist: click (>=8.1.2,<8.2.0)
-Requires-Dist: paramiko (>=2.11.0,<2.12.0)
+Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: paramiko (>=3.0.0,<4.0.0)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
-Requires-Dist: pymetasploit3 (>=1.0.3,<1.1.0)
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
-Requires-Dist: requests (>=2.27.0,<2.28.0)
+Requires-Dist: pymetasploit3 (>=1.0.3,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
-Requires-Dist: structlog (>=21.5.0,<21.6.0)
+Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: utinni (>=0.5.0,<0.6.0)
 Project-URL: Documentation, https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/
 Project-URL: Repository, https://gitlab.ics.muni.cz/cryton/cryton-worker
 Description-Content-Type: text/markdown
 
 ![Coverage](https://gitlab.ics.muni.cz/cryton/cryton-worker/badges/master/coverage.svg)
 
@@ -51,34 +51,30 @@
 Modules provided by Cryton can be found [here](https://gitlab.ics.muni.cz/cryton/cryton-modules). **Their installation will
 be covered in this section**.
 
 Make sure Git, Docker, and Docker Compose plugin are installed:
 - [Git](https://git-scm.com/)
 - [Docker Compose](https://docs.docker.com/compose/install/)
 
-Optionally, check out these [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
+Optionally, check out these Docker [post-installation steps](https://docs.docker.com/engine/install/linux-postinstall/).
 
 The following script clones the necessary repositories (Worker and modules), updates Worker's settings, and runs the 
 Docker Compose configuration which starts the Worker, and its prerequisites (Metasploit and Empire framework).
 ```shell
 git clone https://gitlab.ics.muni.cz/cryton/cryton-modules.git
 cd cryton-modules
 git checkout $(git tag --list "2023.1.*" | tail -n 1)
 cd ..
 export CRYTON_MODULES_PATH=$(pwd)/cryton-modules/modules
 git clone https://gitlab.ics.muni.cz/cryton/cryton-worker.git
 cd cryton-worker
 git checkout $(git tag --list "2023.1.*" | tail -n 1)
-sed -i "s|CRYTON_WORKER_NAME=CHANGE_ME|CRYTON_WORKER_NAME=LocalWorker|" .env
 sed -i "s|CRYTON_WORKER_MODULES_DIR=CHANGE_ME|CRYTON_WORKER_MODULES_DIR=$CRYTON_MODULES_PATH|" .env
-sed -i "s|CRYTON_WORKER_MSFRPCD_HOST=CHANGE_ME|CRYTON_WORKER_MSFRPCD_HOST=localhost|" .env
-sed -i "s|CRYTON_WORKER_RABBIT_HOST=CHANGE_ME|CRYTON_WORKER_RABBIT_HOST=localhost|" .env
-sed -i "s|CRYTON_WORKER_EMPIRE_HOST=CHANGE_ME|CRYTON_WORKER_EMPIRE_HOST=cryton-empire|" .env
 docker compose up -d
 ```
 
 For more information see the [documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/).
 
 ## Contributing
 Contributions are welcome. Please **contribute to the [project mirror](https://gitlab.com/cryton-toolset)** on gitlab.com.
-For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/contribution-guide/).
+For more information see the [contribution page](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/contribution-guide/).
```

