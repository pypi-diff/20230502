# Comparing `tmp/pants_py_deploy-0.0.10-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12768 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 09:51 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4308 b- defN 23-May-02 09:51 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7744 b- defN 23-May-02 09:51 pants_py_deploy/compose_file_models.py
--rw-r--r--  2.0 unx     7078 b- defN 23-May-02 09:51 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx      261 b- defN 23-May-02 09:51 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     2222 b- defN 23-May-02 09:51 pants_py_deploy/models.py
--rw-r--r--  2.0 unx     5136 b- defN 23-May-02 09:51 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx     2367 b- defN 23-May-02 09:51 pants_py_deploy/ports.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-02 09:51 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2150 b- defN 23-May-02 09:51 pants_py_deploy-0.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 09:51 pants_py_deploy-0.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-02 09:51 pants_py_deploy-0.0.10.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-02 09:51 pants_py_deploy-0.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1202 b- defN 23-May-02 09:51 pants_py_deploy-0.0.10.dist-info/RECORD
-14 files, 32860 bytes uncompressed, 10742 bytes compressed:  67.3%
+Zip file size: 12803 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 23-May-02 13:35 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-02 13:35 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7744 b- defN 23-May-02 13:35 pants_py_deploy/compose_file_models.py
+-rw-r--r--  2.0 unx     7078 b- defN 23-May-02 13:35 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx      261 b- defN 23-May-02 13:35 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     2222 b- defN 23-May-02 13:35 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx     5293 b- defN 23-May-02 13:35 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx     2367 b- defN 23-May-02 13:35 pants_py_deploy/ports.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-02 13:35 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2150 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1202 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/RECORD
+14 files, 33017 bytes uncompressed, 10777 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pants_py_deploy/ports.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.10.dist-info/METADATA
+Filename: pants_py_deploy-0.0.13.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.10.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.13.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.10.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.13.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.10.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.13.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.10.dist-info/RECORD
+Filename: pants_py_deploy-0.0.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/compose_file.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
 from collections import ChainMap
 from itertools import chain
 from typing import Iterable
 
+from pants.engine.fs import FileContent
 from pants_py_deploy.compose_file_models import (
     ComposeServiceInfo,
     export_compose_dict_from_services,
     iter_compose_info,
 )
 from pants_py_deploy.fields import COMPOSE_NETWORK_NAME
 from pants_py_deploy.models import ComposeFiles, ComposeService, FileEnvVars
 from pants_py_deploy.ports import PrefixPort
-from pants.engine.fs import FileContent
 from zero_3rdparty.str_utils import ensure_suffix
 
 from model_lib import FileFormat, dump, parse_payload
 
 
 def create_compose_files(
     new_paths: set[str], env_vars: FileEnvVars, compose_files: ComposeFiles
```

## pants_py_deploy/models.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import Iterable
 
-from pants_py_deploy.ports import PrefixPort
 from pants.backend.docker.target_types import DockerImageTarget
 from pants.engine.collection import Collection
 from pants.util.frozendict import FrozenDict
 from pants.util.ordered_set import FrozenOrderedSet
+from pants_py_deploy.ports import PrefixPort
 
 
 @dataclass(frozen=True)
 class EnvVar:
     name: str
     default: str
```

## pants_py_deploy/plugin.py

```diff
@@ -1,20 +1,10 @@
 from dataclasses import dataclass
 from pathlib import PurePath
 
-from pants_py_deploy.compose_file import create_compose_files, modify_existing_compose
-from pants_py_deploy.export_env import read_env_and_ports
-from pants_py_deploy.fields import ComposeEnabledField
-from pants_py_deploy.models import (
-    ComposeFiles,
-    ComposeService,
-    ComposeServiceRequest,
-    EnvVar,
-    FileEnvVars,
-)
 from pants.backend.docker.target_types import DockerImageTagsField, DockerImageTarget
 from pants.backend.python.target_types import PythonSourceField
 from pants.core.goals.fix import FixFilesRequest, FixResult, Partitions
 from pants.core.util_rules.source_files import SourceFiles, SourceFilesRequest
 from pants.engine.fs import (
     CreateDigest,
     Digest,
@@ -29,14 +19,24 @@
     AllTargets,
     FieldSet,
     TransitiveTargets,
     TransitiveTargetsRequest,
 )
 from pants.util.meta import classproperty
 from pants.util.ordered_set import FrozenOrderedSet
+from pants_py_deploy.compose_file import create_compose_files, modify_existing_compose
+from pants_py_deploy.export_env import read_env_and_ports
+from pants_py_deploy.fields import ComposeEnabledField
+from pants_py_deploy.models import (
+    ComposeFiles,
+    ComposeService,
+    ComposeServiceRequest,
+    EnvVar,
+    FileEnvVars,
+)
 from zero_3rdparty.str_utils import ensure_suffix
 
 
 @dataclass(frozen=True)
 class DockerComposeFieldSet(FieldSet):
     required_fields = (PythonSourceField,)
 
@@ -57,19 +57,21 @@
     @classproperty
     def tool_id(cls) -> str:
         return "dockercompose"
 
 
 @rule
 async def docker_compose_partition(
-    request: DockerComposeFileFixer.PartitionRequest,
+    request: DockerComposeFileFixer.PartitionRequest, compose_files: ComposeFiles
 ) -> Partitions:
-    return Partitions.single_partition(
+    managed_files = [path for path in compose_files.paths_managed.keys()]
+    input_digest = [
         file for file in request.files if PurePath(file).stem == "docker-compose"
-    )
+    ]
+    return Partitions.single_partition(set(input_digest + managed_files))
 
 
 @rule
 async def find_env_vars(targets: AllTargets) -> FileEnvVars:
     # don't understand why targets: Targets doesn't work
     sources = await Get(
         SourceFiles,
```

## pants_py_deploy/register.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
+from pants.backend.docker.target_types import DockerImageTarget
 from pants_py_deploy import plugin
 from pants_py_deploy.fields import ComposeEnabledField
-from pants.backend.docker.target_types import DockerImageTarget
 
 
 def rules():
     return [
         *plugin.rules(),
         DockerImageTarget.register_plugin_field(ComposeEnabledField),
     ]
```

## Comparing `pants_py_deploy-0.0.10.dist-info/METADATA` & `pants_py_deploy-0.0.13.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.10
+Version: 0.0.13
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
```

## Comparing `pants_py_deploy-0.0.10.dist-info/RECORD` & `pants_py_deploy-0.0.13.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pants_py_deploy/compose_file.py,sha256=HGMBI5xquNj5qBTGUHdYviWZw7l0Asx0Tnm5oomhLkI,4308
+pants_py_deploy/compose_file.py,sha256=j3m1t5FSOHLs0dYIVzzsQJEt0ManT4vt9Eg7aIGMsVs,4308
 pants_py_deploy/compose_file_models.py,sha256=KpkmWQcThF7XsRE1pC69ljDrkIi4Jk3P6r4wRvnEQT8,7744
 pants_py_deploy/export_env.py,sha256=yCurh7x07tiMi-MoEcq3WUobrTJkGaiW5b6d55jLv3Q,7078
 pants_py_deploy/fields.py,sha256=gKrdqf6kHaosNHG93syWFDEtVH8cWpO4PaeOWKp1QyA,261
-pants_py_deploy/models.py,sha256=zypfaIyuW5OQSZXjkdFxvTsqxu6xJ3eXyJ2SY_iIWi4,2222
-pants_py_deploy/plugin.py,sha256=Kkz5s_jY7UiIDuUB9v3a1L4KVnosvP3NMroIIAubyxQ,5136
+pants_py_deploy/models.py,sha256=e_2s6RFg5oZrYzKVgfKgsXb6ien6y_nYK4AuJ0QlqWo,2222
+pants_py_deploy/plugin.py,sha256=Y8J_FWxewG_4hFrvPjD4K0mBEG3ndQ8M0uC3B-bQdQw,5293
 pants_py_deploy/ports.py,sha256=b4Kxxnjk9uedTrlJ1cpZmWMuMOTaHhsOuIbcJGbX3YU,2367
-pants_py_deploy/register.py,sha256=ulH_0RoUAvH_cclnpTGTyPqqLbOdmzpZeH_FiOnTptY,283
-pants_py_deploy-0.0.10.dist-info/METADATA,sha256=eWxkRWeL5iRbvLwJNSGPyybPYA0Xg1ysw5E88ryzaJQ,2150
-pants_py_deploy-0.0.10.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.10.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.10.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.10.dist-info/RECORD,,
+pants_py_deploy/register.py,sha256=aVXxmofChwsPDqQU_lEUp608IUlwkjwbrp7Y1hO71nk,283
+pants_py_deploy-0.0.13.dist-info/METADATA,sha256=6eNUKlj4RDT0W7OA5T6UZTsJ7XRXP2DBI6L839EDB7A,2150
+pants_py_deploy-0.0.13.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.13.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.13.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.13.dist-info/RECORD,,
```

