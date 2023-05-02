# Comparing `tmp/django_simple_ip_restrict-1.0.40.tar.gz` & `tmp/django_simple_ip_restrict-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_ip_restrict-1.0.40.tar", last modified: Mon Jan 17 15:30:53 2022, max compression
+gzip compressed data, was "django_simple_ip_restrict-1.0.41.tar", max compression
```

## Comparing `django_simple_ip_restrict-1.0.40.tar` & `django_simple_ip_restrict-1.0.41.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-17 15:30:53.069479 django_simple_ip_restrict-1.0.40/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2022-01-17 15:30:53.069479 django_simple_ip_restrict-1.0.40/PKG-INFO
--rw-rw-rw-   0 circleci  (3434) circleci  (3434)      474 2021-11-18 10:36:48.000000 django_simple_ip_restrict-1.0.40/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-17 15:30:53.069479 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict/
--rw-rw-rw-   0 circleci  (3434) circleci  (3434)        0 2021-11-18 10:36:48.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict/__init__.py
--rw-rw-rw-   0 circleci  (3434) circleci  (3434)     1773 2021-11-18 10:36:48.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict/middleware.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-17 15:30:53.069479 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1513 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      340 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/django_simple_ip_restrict.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-01-17 15:30:53.069479 django_simple_ip_restrict-1.0.40/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1394 2022-01-17 15:30:52.000000 django_simple_ip_restrict-1.0.40/setup.py
+-rw-r--r--   0        0        0      688 2023-05-02 12:46:48.631942 django_simple_ip_restrict-1.0.41/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 12:46:48.631942 django_simple_ip_restrict-1.0.41/django_simple_ip_restrict/__init__.py
+-rw-r--r--   0        0        0     1602 2023-05-02 12:46:48.631942 django_simple_ip_restrict-1.0.41/django_simple_ip_restrict/middleware.py
+-rw-r--r--   0        0        0     1263 2023-05-02 12:46:48.631942 django_simple_ip_restrict-1.0.41/pyproject.toml
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 django_simple_ip_restrict-1.0.41/PKG-INFO
```

### Comparing `django_simple_ip_restrict-1.0.40/PKG-INFO` & `django_simple_ip_restrict-1.0.41/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
-Name: django_simple_ip_restrict
-Version: 1.0.40
-Summary: Apply an IP restriction to specific routes
-Home-page: UNKNOWN
-Author: STITCH (Aleksey Panov, Mario Brito, Daniel Hengeveld, André Pereira, Kellie English)
-Author-email: panovitch@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Name: django-simple-ip-restrict
+Version: 1.0.41
+Summary: This middleware allows you to mark Django URL namespaces as unavailable to all requests except those coming from a whitelisted IP subnet.
+Home-page: https://github.com/hatch-studio/django-simple-ip-restrict
+Author: stitchdev
+Author-email: dev@stitchdesignlab.com
+Requires-Python: >=3.5,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Dist: django (==2.2.28)
+Requires-Dist: netaddr (>=0.8.0,<0.9.0)
+Project-URL: Repository, https://github.com/hatch-studio/django-simple-ip-restrict
 Description-Content-Type: text/markdown
 
 # django-simple-ip-restrict
 
 This middleware allows you to mark Django URL namespaces as unavailable to all
 requests except those coming from a whitelisted IP subnet.
 
@@ -38,7 +47,16 @@
 
 Then you can set the following keys on settings.py:
 
   - IP_PROTECTED_NAMESPACES: list of namespaces to block (default: ["admin"])
   - IP_NETWORKS_WHITELIST: list of subnets to allow, in CIDR notation
 
 
+## Creating a new release
+
+Update the version in pyproject.toml and create a new tag with that version number and push it,
+this will trigger the release.yml GitHub Action.
+
+```bash
+git push origin <tag_name>
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_simple_ip_restrict-1.0.40/setup.py` & `django_simple_ip_restrict-1.0.41/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-#!/usr/bin/env python3
-
-from io import open
-
-from setuptools import find_packages, setup
-
-
-def readall(path):
-    with open(path, encoding="utf-8") as fp:
-        return fp.read()
-
-
-setup(
-    name="django_simple_ip_restrict",
-    version="1.0.40",
-    description="Apply an IP restriction to specific routes",
-    long_description=readall("README.md"),
-    long_description_content_type="text/markdown",
-    author="STITCH (Aleksey Panov, Mario Brito, Daniel Hengeveld, André Pereira, Kellie English)",
-    author_email="panovitch@gmail.com",
-    packages=find_packages(exclude=("tests.*", "tests")),
-    python_requires=">=3.5",
-    install_requires=["Django>=2.2", "netaddr"],
-    include_package_data=True,
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Environment :: Web Environment",
-        "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-)
+[tool.poetry]
+name = "django-simple-ip-restrict"
+version = "1.0.41"
+description = "This middleware allows you to mark Django URL namespaces as unavailable to all requests except those coming from a whitelisted IP subnet."
+authors = ["stitchdev <dev@stitchdesignlab.com>"]
+readme = "README.md"
+packages = [{include = "django_simple_ip_restrict"}]
+repository = "https://github.com/hatch-studio/django-simple-ip-restrict"
+exclude = [
+    "tests",
+    "tests.*",
+    "poetry.lock"
+]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Django :: 2.2",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+
+[tool.poetry.dependencies]
+python = "^3.5"
+django = "2.2.28"
+netaddr = "^0.8.0"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

