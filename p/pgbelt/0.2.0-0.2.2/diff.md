# Comparing `tmp/pgbelt-0.2.0.tar.gz` & `tmp/pgbelt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.2.0.tar", max compression
+gzip compressed data, was "pgbelt-0.2.2.tar", max compression
```

## Comparing `pgbelt-0.2.0.tar` & `pgbelt-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10758 2023-04-28 19:32:49.082422 pgbelt-0.2.0/LICENSE
--rw-r--r--   0        0        0     2047 2023-04-28 19:32:49.086422 pgbelt-0.2.0/README.md
--rw-r--r--   0        0        0      137 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5191 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3043 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/login.py
--rw-r--r--   0        0        0     8215 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     3148 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     5082 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     3190 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     8080 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3754 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3724 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/config.py
--rw-r--r--   0        0        0     5311 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/models.py
--rw-r--r--   0        0        0     5152 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/remote.py
--rw-r--r--   0        0        0      186 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/main.py
--rw-r--r--   0        0        0       40 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0     9698 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1424 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/logs.py
--rw-r--r--   0        0        0    12309 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    13669 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1202 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 pgbelt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-02 19:33:15.888850 pgbelt-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2047 2023-05-02 19:33:15.888850 pgbelt-0.2.2/README.md
+-rw-r--r--   0        0        0      137 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     2275 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5292 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0     8215 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     3148 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     5082 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     3190 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     8080 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3754 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3817 2023-05-02 19:33:15.888850 pgbelt-0.2.2/pgbelt/config/config.py
+-rw-r--r--   0        0        0     5421 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5247 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0     9698 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1424 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    12309 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    13669 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1202 2023-05-02 19:33:15.892850 pgbelt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pgbelt-0.2.2/PKG-INFO
```

### Comparing `pgbelt-0.2.0/LICENSE` & `pgbelt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/README.md` & `pgbelt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/convenience.py` & `pgbelt-0.2.2/pgbelt/cmd/convenience.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/helpers.py` & `pgbelt-0.2.2/pgbelt/cmd/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 from collections.abc import Awaitable
 from collections.abc import Callable
 from functools import wraps
 from inspect import iscoroutinefunction
 from inspect import Parameter
 from inspect import signature
 from typing import Any
+from typing import Optional  # noqa: F401 # Needed until tiangolo/typer#522 is fixed)
 from typing import TypeVar
 
 from pgbelt.config import get_all_configs_async
 from pgbelt.config import get_config_async
 from typer import Argument
 from typer import Typer
 
 
 T = TypeVar("T")
 
 
 def run_with_configs(
-    decorated_func: Callable[..., Awaitable[T | None]] = None,
+    decorated_func: Callable[..., Awaitable[Optional[T]]] = None,
     skip_src: bool = False,
     skip_dst: bool = False,
-    results_callback: Callable[[list[T]], Awaitable[Any | None]] | None = None,
+    results_callback: Optional[Callable[[list[T]], Awaitable[Optional[Any]]]] = None,
 ) -> Callable:
     """
     Decorator for async commands. Implementations should take one Awaitable[DbupgradeConfig] arg
     and do some operation on the databases in it. This wrapper handles looking up the
     config and executing the command. The decorated result can be run either on one db only
     or on the entire datacenter concurrently.
 
@@ -46,15 +47,15 @@
         else:
             func.__doc__ += (
                 "\n\n    Requires both src and dst to be not null in the config file."
             )
 
         # The name, docstring, and signature of the implementation is preserved. Important for add_command
         @wraps(func)
-        async def wrapper(dc: str, db: str | None, **kwargs):
+        async def wrapper(dc: str, db: Optional[str], **kwargs):
             # If db is specified we only want to run on one of them
             if db is not None:
                 results = [
                     await func(
                         get_config_async(db, dc, skip_src=skip_src, skip_dst=skip_dst),
                         **kwargs
                     )
@@ -96,15 +97,15 @@
     # Give typer the name of the actual implementing function
     name = command.__name__.replace("_", "-")
 
     # If async assume command can be run on a whole datacenter and make db optional
     if iscoroutinefunction(command):
 
         @app.command(name=name)
-        def cmdwrapper(dc: str, db: str | None = Argument(None), **kwargs):
+        def cmdwrapper(dc: str, db: Optional[str] = Argument(None), **kwargs):
             run(command(dc, db, **kwargs))
 
     # Synchronous commands can only be run on one db at a time
     else:
 
         @app.command(name=name)
         def cmdwrapper(dc: str, db: str, **kwargs):
```

### Comparing `pgbelt-0.2.0/pgbelt/cmd/login.py` & `pgbelt-0.2.2/pgbelt/cmd/login.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/preflight.py` & `pgbelt-0.2.2/pgbelt/cmd/preflight.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/schema.py` & `pgbelt-0.2.2/pgbelt/cmd/schema.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/setup.py` & `pgbelt-0.2.2/pgbelt/cmd/setup.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/status.py` & `pgbelt-0.2.2/pgbelt/cmd/status.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/sync.py` & `pgbelt-0.2.2/pgbelt/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/cmd/teardown.py` & `pgbelt-0.2.2/pgbelt/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/config/config.py` & `pgbelt-0.2.2/pgbelt/config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import asyncio
 from collections.abc import AsyncGenerator
 from collections.abc import Awaitable
 from os.path import join
+from typing import Optional  # noqa: F401 # Needed until tiangolo/typer#522 is fixed)
 
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.config.remote import resolve_remote_config
 from pgbelt.util import get_logger
 from pgbelt.util.asyncfuncs import isdir
 from pgbelt.util.asyncfuncs import isfile
 from pgbelt.util.asyncfuncs import listdir
 
 
 def get_config(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> DbupgradeConfig | None:
+) -> Optional[DbupgradeConfig]:
     """
     Get a configuration for one database pair synchronously.
     """
     config = asyncio.run(get_config_async(db, dc, skip_src, skip_dst))
 
     if config is None:
         exit(1)
 
     return config
 
 
 async def get_config_async(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> DbupgradeConfig | None:
+) -> Optional[DbupgradeConfig]:
     """
     Get configuration for one database pair asynchronously. Always prefers
     locally cached configuration but attempts to resolve any uncached configuration
     if it is required. Locally cached config never expires, so it may become stale.
     """
     logger = get_logger(db, dc, "config")
     logger.info("Getting configuration...")
@@ -67,27 +68,27 @@
 
 async def find_available_configs(confdir: str, dc: str) -> set[str]:
     """
     Search for all the database configs in a datacenter directory within a config directory.
     """
     result = set()
     dc_dir = join(confdir, dc)
-    if not await (isdir(dc_dir)):
+    if not await isdir(dc_dir):
         return set()
     for db in await listdir(dc_dir):
         if await isdir(join(dc_dir, db)) and await isfile(
             join(dc_dir, db, "config.json")
         ):
             result.add(db)
     return result
 
 
 async def get_all_configs_async(
     dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> AsyncGenerator[Awaitable[DbupgradeConfig | None], None]:
+) -> AsyncGenerator[Awaitable[Optional[DbupgradeConfig]], None]:
     """
     A generator that produces Awaitables that resolve to DbupgradeConfigs or None
 
     Will produce all possible configs in the given dc whether they are remote
     or already resolved and cached.
     """
     logger = get_logger("all", dc, "config")
```

### Comparing `pgbelt-0.2.0/pgbelt/config/models.py` & `pgbelt-0.2.2/pgbelt/config/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from os.path import join
+from typing import Optional  # noqa: F401 # Needed until tiangolo/typer#522 is fixed)
 
 from aiofiles import open as aopen
 from aiofiles.os import remove
 from pgbelt.util import get_logger
 from pgbelt.util.asyncfuncs import makedirs
 from pydantic import BaseModel
 from pydantic import ValidationError
@@ -15,30 +16,30 @@
     return f"configs/{dc}/{db}"
 
 
 def config_file(db: str, dc: str) -> str:
     return join(config_dir(db, dc), "config.json")
 
 
-def not_empty(v) -> str | None:
+def not_empty(v) -> Optional[str]:
     if v == "":
         raise ValueError
     return v
 
 
 class User(BaseModel):
     """
     Represents a user in a postgres db.
 
     name: str The user name.
     pw: str The user's password. Only required for users pgbelt needs to log in as.
     """
 
     name: str
-    pw: str | None = None
+    pw: Optional[str] = None
 
     _not_empty = validator("name", "pw", allow_reuse=True)(not_empty)
 
 
 class DbConfig(BaseModel):
     """
     Represents a postgres db instance.
@@ -57,15 +58,15 @@
     host: str
     ip: str
     db: str
     port: str
     root_user: User
     owner_user: User
     pglogical_user: User
-    other_users: list[User] | None = None
+    other_users: Optional[list[User]] = None
 
     _not_empty = validator("host", "ip", "db", "port", allow_reuse=True)(not_empty)
 
     @validator("root_user", "owner_user", "pglogical_user")
     def has_password(cls, v) -> User:  # noqa: N805
         if not v.pw:
             raise ValueError
@@ -104,18 +105,18 @@
     dc: str A name used to identify the environment this database pair is in. Used in cli commands.
     src: DbConfig The database we are moving data out of.
     dst: DbConfig The database we are moving data into.
     """
 
     db: str
     dc: str
-    src: DbConfig | None = None
-    dst: DbConfig | None = None
-    tables: list[str] | None = None
-    sequences: list[str] | None = None
+    src: Optional[DbConfig] = None
+    dst: Optional[DbConfig] = None
+    tables: Optional[list[str]] = None
+    sequences: Optional[list[str]] = None
 
     _not_empty = validator("db", "dc", allow_reuse=True)(not_empty)
 
     @property
     def file(self) -> str:
         return config_file(self.db, self.dc)
 
@@ -142,15 +143,15 @@
 
         async with aopen(self.file, "w") as f:
             await f.write(self.json(indent=4))
 
         logger.info("Cached config to disk.")
 
     @classmethod
-    async def load(cls, db: str, dc: str) -> DbupgradeConfig | None:
+    async def load(cls, db: str, dc: str) -> Optional[DbupgradeConfig]:
         """
         Load the specified configuration from disk if present.
         If the existing config is invalid or does not exist return None.
         """
         logger = get_logger(db, dc, "config")
         logger.debug("Trying to load cached config...")
```

### Comparing `pgbelt-0.2.0/pgbelt/config/remote.py` & `pgbelt-0.2.2/pgbelt/config/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from importlib import import_module
 from json import JSONDecodeError
 from logging import Logger
+from typing import Optional  # noqa: F401 # Needed until tiangolo/typer#522 is fixed)
 
 from aiofiles import open as aopen
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.logs import get_logger
 from pydantic import BaseModel
 from pydantic import ValidationError
 
@@ -55,28 +56,28 @@
     skip_dst: bool
     logger: Logger
 
     class Config:
         arbitrary_types_allowed = True
         extra = "ignore"
 
-    async def resolve(self) -> DbupgradeConfig | None:
+    async def resolve(self) -> Optional[DbupgradeConfig]:
         """
         Called to retrieve the configuration from wherever your resolver gets it.
         Return configuration as a DbupgradeConfig.
 
         If you should have been able to get configuration but encountered an error
         then throw a RemoteConfigError. If there was no config and no error return None
         """
         raise NotImplementedError
 
 
 async def load_remote_conf_def(
     config_file: str, logger: Logger
-) -> RemoteConfigDefinition | None:
+) -> Optional[RemoteConfigDefinition]:
     try:
         logger.debug(f"Reading remote config definition from file {config_file}")
         async with aopen(config_file, mode="r") as f:
             raw_json = await f.read()
 
         return RemoteConfigDefinition.parse_raw(raw_json)
     except FileNotFoundError:
@@ -85,15 +86,15 @@
         logger.error(f"Remote config definition in {config_file} was malformed JSON.")
     except ValidationError:
         logger.error(f"Remote config definition in {config_file} was not valid.")
 
 
 async def resolve_remote_config(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> DbupgradeConfig | None:
+) -> Optional[DbupgradeConfig]:
     """
     Loads the referenced remote configuration json file, tries to import the
     specified resolver class, executes its resolve method, and returns the
     resulting DbupgradeConfig or None if there was an error
     """
 
     # set up the logger
```

### Comparing `pgbelt-0.2.0/pgbelt/util/asyncfuncs.py` & `pgbelt-0.2.2/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/util/dump.py` & `pgbelt-0.2.2/pgbelt/util/dump.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/util/logs.py` & `pgbelt-0.2.2/pgbelt/util/logs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/util/pglogical.py` & `pgbelt-0.2.2/pgbelt/util/pglogical.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pgbelt/util/postgres.py` & `pgbelt-0.2.2/pgbelt/util/postgres.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.0/pyproject.toml` & `pgbelt-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.2.0"
+version = "0.2.2"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiofiles = ">=0.8,<23.2"
 asyncpg = "^0.27.0"
 pydantic = "^1.10.0"
 tabulate = "^0.9.0"
-typer = "^0.7.0"
+typer = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 black = "~23.3.0"
-pre-commit = "~3.2.1"
+pre-commit = "~3.3.1"
 flake8 = "^6.0.0"
 pytest-cov = "~4.0.0"
 pytest = "^7.1.3"
-coverage = {extras = ["toml"], version = "^6.5"}
+coverage = {extras = ["toml"], version = "^7.2"}
 safety = "^2.3.1"
 mypy = "^1.1"
 xdoctest = {extras = ["colors"], version = "^1.1.0"}
 flake8-bandit = "~4.1.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.3.0"
```

### Comparing `pgbelt-0.2.0/PKG-INFO` & `pgbelt-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgbelt
-Version: 0.2.0
+Version: 0.2.2
 Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
 Author: Varjitt Jeeva
 Author-email: varjitt.jeeva@autodesk.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.8,<23.2)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Pgbelt
 
 <p align="center">
     <img src="https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true" width="400">
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: pgbelt Version: 0.2.0 Summary: A CLI tool used to
+Metadata-Version: 2.1 Name: pgbelt Version: 0.2.2 Summary: A CLI tool used to
 manage Postgres data migrations from beginning to end, for a single database or
 a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
 varjitt.jeeva@autodesk.com Requires-Python: >=3.11,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.8,<23.2) Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tabulate
-(>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.7.0,<0.8.0) Description-Content-
+(>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-
 Type: text/markdown # Pgbelt
       [https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true]
  [Latest_Commit] [https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/
       badge.svg] [https://img.shields.io/github/license/Autodesk/pgbelt]
 PgBelt is a CLI tool used to manage Postgres data migrations from beginning to
 end, for a single database or a fleet, leveraging pglogical replication. It was
 built to assist in migrating data between postgres databases with as little
```

