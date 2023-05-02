# Comparing `tmp/typegraph-0.1.6.tar.gz` & `tmp/typegraph-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.6.tar", max compression
+gzip compressed data, was "typegraph-0.1.7.tar", max compression
```

## Comparing `typegraph-0.1.6.tar` & `typegraph-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     5252 2023-04-27 09:04:19.742183 typegraph-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     1427 2023-04-27 09:04:19.742183 typegraph-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      225 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/models.py
--rw-r--r--   0        0        0     1953 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     7955 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7499 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     3904 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/injection.py
--rw-r--r--   0        0        0     4338 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/policies.py
--rw-r--r--   0        0        0     1675 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    22924 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    15008 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2209 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     5234 2023-04-27 09:04:19.746183 typegraph-0.1.6/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1403 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2789 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1352 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/python_wasi.py
--rw-r--r--   0        0        0     2880 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1169 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    20388 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2198 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-04-27 09:04:19.750183 typegraph-0.1.6/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5254 2023-05-02 08:12:21.968983 typegraph-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     1445 2023-05-02 08:12:21.968983 typegraph-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/effects.py
+-rw-r--r--   0        0        0     3323 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1868 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3066 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1953 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     5774 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0     7955 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3667 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7499 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4236 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0     8909 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     3904 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/injection.py
+-rw-r--r--   0        0        0     4338 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/policies.py
+-rw-r--r--   0        0        0     1675 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28490 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    22924 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6601 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    15008 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2373 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2209 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1351 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5234 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1403 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2789 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1352 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/python_wasi.py
+-rw-r--r--   0        0        0     2880 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2053 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1169 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    20388 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/types.py
+-rw-r--r--   0        0        0      487 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     1977 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2198 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      185 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.7/PKG-INFO
```

### Comparing `typegraph-0.1.6/LICENSE.md` & `typegraph-0.1.7/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # License
 
 Copyright © Metatype OÜ.
 
-Portions of this software are licensed as follows:
+Portions of this repository are licensed as follows:
 
 - all third party components incorporated into the repository are licensed under
   the original license provided by the owner of the applicable component (see
   relevant file headers)
 - content outside of the above mentioned files or restrictions is available
   under the Elastic License 2.0 (ELv2) as defined below
 - alternatively, the Metatype Commercial Licensing can be substituted to the
```

### Comparing `typegraph-0.1.6/pyproject.toml` & `typegraph-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.6"
+version = "0.1.7"
 description = "Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
 license = "ELv2"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
@@ -36,14 +36,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-snapshot = "^0.9.0"
 pydoc-markdown = { git = "https://github.com/metatypedev/pydoc-markdown", branch = "develop" }
 ruff = "^0.0.261"
 respx = "^0.20.1"
 coverage = "^7.2.3"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = ".."
```

### Comparing `typegraph-0.1.6/typegraph/effects.py` & `typegraph-0.1.7/typegraph/effects.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/graph/auth/__init__.py` & `typegraph-0.1.7/typegraph/graph/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/graph/builder.py` & `typegraph-0.1.7/typegraph/graph/builder.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/graph/models.py` & `typegraph-0.1.7/typegraph/graph/models.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/graph/nodes.py` & `typegraph-0.1.7/typegraph/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/graph/typegraph.py` & `typegraph-0.1.7/typegraph/graph/typegraph.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/importers/base/importer.py` & `typegraph-0.1.7/typegraph/importers/base/importer.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/importers/base/typify.py` & `typegraph-0.1.7/typegraph/importers/base/typify.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/importers/google_discovery.py` & `typegraph-0.1.7/typegraph/importers/google_discovery.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/importers/graphql.py` & `typegraph-0.1.7/typegraph/importers/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/importers/openapi.py` & `typegraph-0.1.7/typegraph/importers/openapi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/injection.py` & `typegraph-0.1.7/typegraph/injection.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/policies.py` & `typegraph-0.1.7/typegraph/policies.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.7/typegraph/providers/aws/runtimes/s3.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/prisma/relations.py` & `typegraph-0.1.7/typegraph/providers/prisma/relations.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/prisma/runtimes/prisma.py` & `typegraph-0.1.7/typegraph/providers/prisma/runtimes/prisma.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/prisma/schema.py` & `typegraph-0.1.7/typegraph/providers/prisma/schema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.7/typegraph/providers/prisma/type_generator.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/prisma/utils.py` & `typegraph-0.1.7/typegraph/providers/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.7/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/base.py` & `typegraph-0.1.7/typegraph/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/deno.py` & `typegraph-0.1.7/typegraph/runtimes/deno.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/graphql.py` & `typegraph-0.1.7/typegraph/runtimes/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/http.py` & `typegraph-0.1.7/typegraph/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/python_wasi.py` & `typegraph-0.1.7/typegraph/runtimes/python_wasi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/random.py` & `typegraph-0.1.7/typegraph/runtimes/random.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/typegate.py` & `typegraph-0.1.7/typegraph/runtimes/typegate.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/runtimes/wasmedge.py` & `typegraph-0.1.7/typegraph/runtimes/wasmedge.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/types.py` & `typegraph-0.1.7/typegraph/types.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/utils/attrs.py` & `typegraph-0.1.7/typegraph/utils/attrs.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/utils/jsonschema.py` & `typegraph-0.1.7/typegraph/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/typegraph/utils/loaders.py` & `typegraph-0.1.7/typegraph/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.6/PKG-INFO` & `typegraph-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.6
+Version: 0.1.7
 Summary: Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
 Home-page: https://metatype.dev
 License: ELv2
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
```

