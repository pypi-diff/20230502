# Comparing `tmp/jinjat-0.3.tar.gz` & `tmp/jinjat-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjat-0.3.tar", max compression
+gzip compressed data, was "jinjat-0.4.tar", max compression
```

## Comparing `jinjat-0.3.tar` & `jinjat-0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-04-30 20:19:09.645611 jinjat-0.3/LICENSE
--rw-r--r--   0        0        0     1612 2023-04-30 20:19:09.645611 jinjat-0.3/README.md
--rw-r--r--   0        0        0     2648 2023-04-30 20:19:21.893707 jinjat-0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/__init__.py
--rw-r--r--   0        0        0       93 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/__main__.py
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/dbt/__init__.py
--rw-r--r--   0        0        0     2348 2023-04-30 20:19:09.645611 jinjat-0.3/src/jinjat/core/dbt/config.py
--rw-r--r--   0        0        0    23495 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/dbt/dbt_project.py
--rw-r--r--   0        0        0      878 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/exceptions.py
--rw-r--r--   0        0        0     4486 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/generator.py
--rw-r--r--   0        0        0     2641 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/log_controller.py
--rw-r--r--   0        0        0     5373 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/models.py
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/__init__.py
--rw-r--r--   0        0        0     8917 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/admin.py
--rw-r--r--   0        0        0     9164 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/routes/analysis.py
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/schema/__init__.py
--rw-r--r--   0        0        0      693 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/schema/validator.py
--rw-r--r--   0        0        0     5947 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/server.py
--rw-r--r--   0        0        0        0 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/__init__.py
--rw-r--r--   0        0        0     6947 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/api.py
--rw-r--r--   0        0        0     1068 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/filesystem.py
--rw-r--r--   0        0        0     2068 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/core/util/jmespath.py
--rw-r--r--   0        0        0    12288 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/jaffle_shop.duckdb
--rw-r--r--   0        0        0     5889 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/main.py
--rw-r--r--   0        0        0    10094 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/playground.py
--rw-r--r--   0        0        0      210 2023-04-30 20:19:09.649611 jinjat-0.3/src/jinjat/requirements.txt
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 jinjat-0.3/setup.py
--rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 jinjat-0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 00:00:49.669895 jinjat-0.4/LICENSE
+-rw-r--r--   0        0        0     1612 2023-05-02 00:00:49.669895 jinjat-0.4/README.md
+-rw-r--r--   0        0        0     2648 2023-05-02 00:01:01.405990 jinjat-0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/__init__.py
+-rw-r--r--   0        0        0     2348 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/config.py
+-rw-r--r--   0        0        0    23495 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/dbt_project.py
+-rw-r--r--   0        0        0      878 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/exceptions.py
+-rw-r--r--   0        0        0     4486 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/generator.py
+-rw-r--r--   0        0        0     2641 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/log_controller.py
+-rw-r--r--   0        0        0     5373 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/models.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/admin.py
+-rw-r--r--   0        0        0     9164 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/schema/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/schema/validator.py
+-rw-r--r--   0        0        0     5947 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/server.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/__init__.py
+-rw-r--r--   0        0        0     6947 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/api.py
+-rw-r--r--   0        0        0     1068 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/filesystem.py
+-rw-r--r--   0        0        0     2068 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/jmespath.py
+-rw-r--r--   0        0        0    12288 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/jaffle_shop.duckdb
+-rw-r--r--   0        0        0     5853 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/main.py
+-rw-r--r--   0        0        0    10094 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/playground.py
+-rw-r--r--   0        0        0      210 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/requirements.txt
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 jinjat-0.4/setup.py
+-rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 jinjat-0.4/PKG-INFO
```

### Comparing `jinjat-0.3/LICENSE` & `jinjat-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/README.md` & `jinjat-0.4/README.md`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/pyproject.toml` & `jinjat-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinjat"
-version = "0.3"
+version = "0.4"
 description = "A low-code data application framework that uses dbt Core and OpenAPI"
 authors = ["buremba <emrekabakci@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `jinjat-0.3/src/jinjat/core/dbt/config.py` & `jinjat-0.4/src/jinjat/core/dbt/config.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/dbt/dbt_project.py` & `jinjat-0.4/src/jinjat/core/dbt/dbt_project.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/exceptions.py` & `jinjat-0.4/src/jinjat/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/generator.py` & `jinjat-0.4/src/jinjat/core/generator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/log_controller.py` & `jinjat-0.4/src/jinjat/core/log_controller.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/models.py` & `jinjat-0.4/src/jinjat/core/models.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/routes/admin.py` & `jinjat-0.4/src/jinjat/core/routes/admin.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/routes/analysis.py` & `jinjat-0.4/src/jinjat/core/routes/analysis.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/schema/validator.py` & `jinjat-0.4/src/jinjat/core/schema/validator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/server.py` & `jinjat-0.4/src/jinjat/core/server.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/util/api.py` & `jinjat-0.4/src/jinjat/core/util/api.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/util/filesystem.py` & `jinjat-0.4/src/jinjat/core/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/core/util/jmespath.py` & `jinjat-0.4/src/jinjat/core/util/jmespath.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/src/jinjat/main.py` & `jinjat-0.4/src/jinjat/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 from pathlib import Path
 from typing import Callable, Optional
 
 import click
 import uvicorn
 from dbt.cli.option_types import YAML
-from fal_serverless import sync_dir
 
 from jinjat.core.dbt.config import DEFAULT_PROFILES_DIR
 from jinjat.core.generator import compile_macro
 from jinjat.core.log_controller import logger
 from jinjat.core.server import DbtTarget, SERVER_OPT, app
 
 CONTEXT = {"max_content_width": 800}
```

### Comparing `jinjat-0.3/src/jinjat/playground.py` & `jinjat-0.4/src/jinjat/playground.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.3/setup.py` & `jinjat-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 'feedparser>=6.0.10,<7.0.0']}
 
 entry_points = \
 {'console_scripts': ['jinjat = jinjat.main:cli']}
 
 setup_kwargs = {
     'name': 'jinjat',
-    'version': '0.3',
+    'version': '0.4',
     'description': 'A low-code data application framework that uses dbt Core and OpenAPI',
     'long_description': '# Jinjat\n\n## Develop data applications with dbt, SQL, and OpenAPI\n\n### Installation\n\n```commandline\npip install jinjat\n```\n\n### Create your first API\n\nCreate an [analysis]() in `analysis/my_first_api.sql`:\n```sql\n{%- set query = request().query %}\n\nselect \'{{query.example}}\' as col1\n```\n\nAnd create a YML file in `analysis/schema.yml`:\n\n```yml\nversion: 2\n\nanalyses:\n  - name: my_first_api\n    config:\n      jinjat:\n        method: get\n        openapi:\n          parameters:\n            - in: query\n              name: example\n              schema:\n                type: number\n```\n\nStart Jinjat as follows:\n\n```commandline\njinjat serve --project-dir [YOUR_DBT_PROJECT_DIRECTORY]\n```\n\nAnd then run the following CURL command to test the API:\n\n```commandline\ncurl -XGET \'http://127.0.0.1:8581?example=value\'\n```\n\nIt should return the following response:\n\n```json\n[\n  "col1": "3"\n]\n```\n\nJinjat uses OpenAPI to validate the requests and create an API documentation automatically for your API.\n\n## Integrations\n\npoetry install --extras "duckdb"\n\n### Playground\n\npoetry install --extras "playground"\n\n\n#### Installation\n\n```commandline\npip install jinjat[playground]\n```\n\nJinjat Playground is a Streamlit app that lets you develop APIs in your browser.\nOnce you write the template, you can save it to your dbt project as an analysis and expose the API.\n\n### [Refine.dev](https://refine.dev) Integration\n\n#### Installation\n\n```commandline\npip install jinjat[refine]\n```\n\nJinjat Refine integration creates a Refine app from your OpenAPI spec \n\n\n> Jinjat is a fork of [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis)',
     'author': 'buremba',
     'author_email': 'emrekabakci@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jinjat-data/jinjat',
```

### Comparing `jinjat-0.3/PKG-INFO` & `jinjat-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjat
-Version: 0.3
+Version: 0.4
 Summary: A low-code data application framework that uses dbt Core and OpenAPI
 Home-page: https://github.com/jinjat-data/jinjat
 License: Apache 2.0
 Keywords: dbt,server,streamlit,git,refine,data-app,snowflake
 Author: buremba
 Author-email: emrekabakci@gmail.com
 Requires-Python: >=3.6,<4
```

