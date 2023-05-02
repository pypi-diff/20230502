# Comparing `tmp/katalytic-pkg-0.3.0.tar.gz` & `tmp/katalytic-pkg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.3.0.tar", last modified: Fri Apr 28 10:35:32 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.4.0.tar", last modified: Tue May  2 05:42:16 2023, max compression
```

## Comparing `katalytic-pkg-0.3.0.tar` & `katalytic-pkg-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic-pkg-0.3.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-pkg-0.3.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:14:43.739675 katalytic-pkg-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1907 2023-04-28 10:27:14.416328 katalytic-pkg-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic-pkg-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1664 2023-04-14 19:07:14.523511 katalytic-pkg-0.3.0/README.md
--rw-r--r--   0        0        0     1315 2023-04-28 10:33:33.839879 katalytic-pkg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4664 2023-04-28 10:15:23.681535 katalytic-pkg-0.3.0/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2829 2023-04-28 10:02:55.132516 katalytic-pkg-0.3.0/tests/test_pkg.py
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 katalytic-pkg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic-pkg-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-pkg-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3258 2023-04-30 14:18:45.239106 katalytic-pkg-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2085 2023-05-02 05:41:51.432198 katalytic-pkg-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic-pkg-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1507 2023-04-30 14:21:04.979530 katalytic-pkg-0.4.0/README.md
+-rw-r--r--   0        0        0     1119 2023-05-02 05:41:51.432198 katalytic-pkg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4757 2023-05-02 05:32:43.902113 katalytic-pkg-0.4.0/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2829 2023-04-28 10:02:55.132516 katalytic-pkg-0.4.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 katalytic-pkg-0.4.0/PKG-INFO
```

### Comparing `katalytic-pkg-0.3.0/.gitignore` & `katalytic-pkg-0.4.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __pycache__/*
 .cache/*
 .*.swp
 */.ipynb_checkpoints/*
 .DS_Store
 data/
 logs/
+sandbox.*
 
 # Project files
 .ropeproject
 .project
 .pydevproject
 .settings
 .idea
```

### Comparing `katalytic-pkg-0.3.0/.gitlab-ci.yml` & `katalytic-pkg-0.4.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
 image: python:3.9
 
 stages:
   - coverage
-  - security
   - test
+  - security
   - release
 
 variables:
   TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
-test_cov:
+coverage:
   image: python:3.6
   stage: coverage
   script:
     - pip install --upgrade pip
-    - pip install pytest pytest-cov pytest-randomly
-    - pip install -e .
-    - python -m pytest --cov-fail-under=100 --cov=src --cov-report term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
+    - pip install -e .[dev]
+    - python -m pytest --cov-fail-under=100 --cov=src --cov-report=xml --cov-report=term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
   rules:
     - if: '$CI_COMMIT_MESSAGE =~ /(feat|fix|refactor|perf|test|chore|style)/i'
       when: always
     - when: never
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: "coverage.xml"
   allow_failure: false
 
 
 # test_py36:
 #   image: python:3.6
 #   stage: test
 #   script:
```

### Comparing `katalytic-pkg-0.3.0/CHANGELOG.md` & `katalytic-pkg-0.4.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.4.0 (2023-05-02)
+### feat
+- [[`1afcf66`](https://gitlab.com/katalytic/katalytic-pkg/commit/1afcf66f65a6a208039af7929da42a2dc1fcef24)] **get_version:** support subpackages
+
+
 ## 0.3.0 (2023-04-28)
 ### feat
 - [[`655bfc7`](https://gitlab.com/katalytic/katalytic-pkg/commit/655bfc7c069f244366fb12c09fe3f06e61fcd7d6)] **get_modules:** find editable installs
 
 
 ## 0.2.6 (2023-04-14)
 ### Fix
```

### Comparing `katalytic-pkg-0.3.0/LICENSE.txt` & `katalytic-pkg-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.3.0/README.md` & `katalytic-pkg-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-pkg.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-pkg?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-pkg/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-pkg?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-pkg/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-pkg/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-pkg
 ```
```

### Comparing `katalytic-pkg-0.3.0/pyproject.toml` & `katalytic-pkg-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.3.0"
+version = "0.4.0"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -26,33 +26,20 @@
 
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
+    "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-pkg.git"
 repository = "https://gitlab.com/katalytic/katalytic-pkg.git"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-env_list = py36, py37, py38, py39
-isolated_build = True
-
-[testenv]
-extras = dev
-deps = -e .
-
-commands =
-	pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
-"""
-
 [tool.flit.module]
 name = "katalytic.pkg"
```

### Comparing `katalytic-pkg-0.3.0/src/katalytic/pkg.py` & `katalytic-pkg-0.4.0/src/katalytic/pkg.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,17 @@
                 if Path(f'{p2}/PKG-INFO').is_file():
                     yield f'{p2}/PKG-INFO'
 
 
 def get_version(dunder_name):  # pragma: no cover -- I can't test all branches at the same time
     if sys.version_info >= (3, 8):
         from importlib import metadata
-        version = metadata.version(dunder_name.replace('.', '-'))
+        dunder_name = dunder_name.replace('.', '-')
+        dunder_name = dunder_name.replace('-__init__', '')
+        version = metadata.version(dunder_name)
         version_info = tuple(map(int, version.split('.')))
         return version, version_info
 
     version = None
     for p in __find_paths(dunder_name):
         if p.endswith('.dist-info'):
             version = re.search(r'\w+-(\d+\.\d+\.\d+)', p)
```

### Comparing `katalytic-pkg-0.3.0/tests/test_pkg.py` & `katalytic-pkg-0.4.0/tests/test_pkg.py`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.3.0/PKG-INFO` & `katalytic-pkg-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.3.0
+Version: 0.4.0
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-pkg.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-pkg.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-pkg.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-pkg?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-pkg/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-pkg?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-pkg/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-pkg/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-pkg
 ```
```

