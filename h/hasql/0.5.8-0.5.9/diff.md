# Comparing `tmp/hasql-0.5.8.tar.gz` & `tmp/hasql-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasql-0.5.8.tar", last modified: Mon Aug  1 15:45:26 2022, max compression
+gzip compressed data, was "hasql-0.5.9.tar", last modified: Thu Mar 23 09:03:40 2023, max compression
```

## Comparing `hasql-0.5.8.tar` & `hasql-0.5.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2022-08-01 15:45:26.783867 hasql-0.5.8/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    11357 2022-07-27 18:23:43.000000 hasql-0.5.8/LICENSE
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       89 2022-07-29 13:57:21.000000 hasql-0.5.8/MANIFEST.in
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    16480 2022-08-01 15:45:26.784025 hasql-0.5.8/PKG-INFO
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    14985 2022-07-30 17:27:09.000000 hasql-0.5.8/README.rst
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2022-08-01 15:45:26.769163 hasql-0.5.8/hasql/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      568 2022-08-01 15:45:15.000000 hasql-0.5.8/hasql/__init__.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1375 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/aiopg.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      484 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/aiopg_sa.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1237 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/asyncpg.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      341 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/asyncpgsa.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1705 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/asyncsqlalchemy.py
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2022-08-01 15:45:26.783494 hasql-0.5.8/hasql/balancer_policy/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      261 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/balancer_policy/__init__.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1324 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/balancer_policy/base.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1161 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/balancer_policy/greedy.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2214 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/balancer_policy/random_weighted.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2430 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/balancer_policy/round_robin.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    19970 2022-08-01 15:44:20.000000 hasql-0.5.8/hasql/base.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2656 2022-08-01 15:44:20.000000 hasql-0.5.8/hasql/psycopg3.py
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     6309 2022-07-29 13:57:21.000000 hasql-0.5.8/hasql/utils.py
-drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2022-08-01 15:45:26.771794 hasql-0.5.8/hasql.egg-info/
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    16480 2022-08-01 15:45:26.000000 hasql-0.5.8/hasql.egg-info/PKG-INFO
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      526 2022-08-01 15:45:26.000000 hasql-0.5.8/hasql.egg-info/SOURCES.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2022-08-01 15:45:26.000000 hasql-0.5.8/hasql.egg-info/dependency_links.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      493 2022-08-01 15:45:26.000000 hasql-0.5.8/hasql.egg-info/requires.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       12 2022-08-01 15:45:26.000000 hasql-0.5.8/hasql.egg-info/top_level.txt
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      460 2022-08-01 15:45:26.785895 hasql-0.5.8/setup.cfg
--rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2665 2022-07-29 14:03:12.000000 hasql-0.5.8/setup.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-03-23 09:03:40.609372 hasql-0.5.9/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    11357 2022-07-27 18:23:43.000000 hasql-0.5.9/LICENSE
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       89 2022-07-29 13:57:21.000000 hasql-0.5.9/MANIFEST.in
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    17361 2023-03-23 09:03:40.609512 hasql-0.5.9/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    15866 2023-03-23 09:03:08.000000 hasql-0.5.9/README.rst
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-03-23 09:03:40.592734 hasql-0.5.9/hasql/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      568 2023-03-23 09:03:29.000000 hasql-0.5.9/hasql/__init__.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1375 2023-03-23 09:03:02.000000 hasql-0.5.9/hasql/aiopg.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      484 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/aiopg_sa.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1237 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/asyncpg.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      341 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/asyncpgsa.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1705 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/asyncsqlalchemy.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-03-23 09:03:40.608994 hasql-0.5.9/hasql/balancer_policy/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      261 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/balancer_policy/__init__.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1324 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/balancer_policy/base.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     1161 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/balancer_policy/greedy.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2214 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/balancer_policy/random_weighted.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2430 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/balancer_policy/round_robin.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    19970 2023-03-23 09:03:02.000000 hasql-0.5.9/hasql/base.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2656 2022-08-01 15:44:20.000000 hasql-0.5.9/hasql/psycopg3.py
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     6309 2022-07-29 13:57:21.000000 hasql-0.5.9/hasql/utils.py
+drwxr-xr-x   0 mosquito (610789169) LD\Domain Users (593637566)        0 2023-03-23 09:03:40.596104 hasql-0.5.9/hasql.egg-info/
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)    17361 2023-03-23 09:03:40.000000 hasql-0.5.9/hasql.egg-info/PKG-INFO
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      526 2023-03-23 09:03:40.000000 hasql-0.5.9/hasql.egg-info/SOURCES.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)        1 2023-03-23 09:03:40.000000 hasql-0.5.9/hasql.egg-info/dependency_links.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      493 2023-03-23 09:03:40.000000 hasql-0.5.9/hasql.egg-info/requires.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)       12 2023-03-23 09:03:40.000000 hasql-0.5.9/hasql.egg-info/top_level.txt
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)      460 2023-03-23 09:03:40.610618 hasql-0.5.9/setup.cfg
+-rw-r--r--   0 mosquito (610789169) LD\Domain Users (593637566)     2665 2022-07-29 14:03:12.000000 hasql-0.5.9/setup.py
```

### Comparing `hasql-0.5.8/LICENSE` & `hasql-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/PKG-INFO` & `hasql-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasql
-Version: 0.5.8
+Version: 0.5.9
 Summary: hasql is a module for acquiring actual connections with masters and replicas
 Home-page: UNKNOWN
 Author: Vladislav Bakaev <vlad@bakaev.tech>, Dmitry Orlov <me@mosquito.su>
 Author-email: vlad@bakaev.tech, me@mosquito.su
 License: Apache 2
 Project-URL: Source, https://github.com/aiokitchen/hasql
 Project-URL: Tracker, https://github.com/aiokitchen/hasql/issues
@@ -53,15 +53,15 @@
 * completely asynchronous api
 * automatic detection of the host role in the cluster
 * health-checks for each host and automatic traffic outage for
   unavailable hosts
 * autodetection of hosts role changes, in case replica
   host will be promoted to master
 * different policies for load balancing
-* support for ``asyncpg``, ``psycopg3`` and ``aiopg``
+* support for ``asyncpg``, ``psycopg3``, ``aiopg``, ``sqlalchemy`` and ``asyncpgsa``
 
 
 Usage
 =====
 
 Some useful examples
 
@@ -127,15 +127,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 Code example using ``aiopg.sa``:
 
 .. code-block:: python
 
     from hasql.aiopg_sa import PoolManager
@@ -148,15 +148,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 For ``asyncpg``
 ~~~~~~~~~~~~~~~
 
 **asyncpg** must be installed as a requirement
 
@@ -172,17 +172,54 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
+For ``sqlalchemy``
+~~~~~~~~~~~~~~~~~~
+
+**sqlalchemy[asyncio] & asyncpg** must be installed as requirements
+
+.. code-block:: python
+
+    from hasql.asyncsqlalchemy import PoolManager
+
+    hosts = ",".join([
+        "master-host:5432",
+        "replica-host-1:5432",
+        "replica-host-2:5432",
+    ])
+
+    multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
+
+
+    async def create_pool(dsn) -> PoolManager:
+        pool = PoolManager(
+            multihost_dsn,
+
+            # Use master for acquire_replica, if no replicas available
+            fallback_master=True,
+
+            # You can pass pool-specific options
+            pool_factory_kwargs=dict(
+                pool_size=10,
+                max_overflow=5
+            )
+        )
+
+        # Waiting for 1 master and 1 replica will be available
+        await pool.ready(masters_count=1, replicas_count=1)
+        return pool
+
+
 For ``asyncpgsa``
 ~~~~~~~~~~~~~~~~~
 
 **asyncpgsa** must be installed as a requirement
 
 .. code-block:: python
 
@@ -197,16 +234,16 @@
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
         await asyncio.gather(
-            pool_manager.wait_masters_ready(1),
-            pool_manager.wait_replicas_ready(1)
+            pool.wait_masters_ready(1),
+            pool.wait_replicas_ready(1)
         )
         return pool
 
 
 For ``psycopg3``
 ~~~~~~~~~~~~~~~~
 
@@ -224,15 +261,15 @@
     ])
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 
 Acquiring connections
 *********************
 
 Connections should be acquired with async context manager:
```

### Comparing `hasql-0.5.8/README.rst` & `hasql-0.5.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * completely asynchronous api
 * automatic detection of the host role in the cluster
 * health-checks for each host and automatic traffic outage for
   unavailable hosts
 * autodetection of hosts role changes, in case replica
   host will be promoted to master
 * different policies for load balancing
-* support for ``asyncpg``, ``psycopg3`` and ``aiopg``
+* support for ``asyncpg``, ``psycopg3``, ``aiopg``, ``sqlalchemy`` and ``asyncpgsa``
 
 
 Usage
 =====
 
 Some useful examples
 
@@ -90,15 +90,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 Code example using ``aiopg.sa``:
 
 .. code-block:: python
 
     from hasql.aiopg_sa import PoolManager
@@ -111,15 +111,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 For ``asyncpg``
 ~~~~~~~~~~~~~~~
 
 **asyncpg** must be installed as a requirement
 
@@ -135,17 +135,54 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
+For ``sqlalchemy``
+~~~~~~~~~~~~~~~~~~
+
+**sqlalchemy[asyncio] & asyncpg** must be installed as requirements
+
+.. code-block:: python
+
+    from hasql.asyncsqlalchemy import PoolManager
+
+    hosts = ",".join([
+        "master-host:5432",
+        "replica-host-1:5432",
+        "replica-host-2:5432",
+    ])
+
+    multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
+
+
+    async def create_pool(dsn) -> PoolManager:
+        pool = PoolManager(
+            multihost_dsn,
+
+            # Use master for acquire_replica, if no replicas available
+            fallback_master=True,
+
+            # You can pass pool-specific options
+            pool_factory_kwargs=dict(
+                pool_size=10,
+                max_overflow=5
+            )
+        )
+
+        # Waiting for 1 master and 1 replica will be available
+        await pool.ready(masters_count=1, replicas_count=1)
+        return pool
+
+
 For ``asyncpgsa``
 ~~~~~~~~~~~~~~~~~
 
 **asyncpgsa** must be installed as a requirement
 
 .. code-block:: python
 
@@ -160,16 +197,16 @@
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
         await asyncio.gather(
-            pool_manager.wait_masters_ready(1),
-            pool_manager.wait_replicas_ready(1)
+            pool.wait_masters_ready(1),
+            pool.wait_replicas_ready(1)
         )
         return pool
 
 
 For ``psycopg3``
 ~~~~~~~~~~~~~~~~
 
@@ -187,15 +224,15 @@
     ])
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 
 Acquiring connections
 *********************
 
 Connections should be acquired with async context manager:
```

### Comparing `hasql-0.5.8/hasql/__init__.py` & `hasql-0.5.9/hasql/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version_info__ = (0, 5, 8)
+__version_info__ = (0, 5, 9)
 __version__ = ".".join(map(str, __version_info__))
 
 package_info = (
     "hasql is a module for acquiring actual connections with masters "
     "and replicas"
 )
```

### Comparing `hasql-0.5.8/hasql/aiopg.py` & `hasql-0.5.9/hasql/aiopg.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/asyncpg.py` & `hasql-0.5.9/hasql/asyncpg.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/asyncsqlalchemy.py` & `hasql-0.5.9/hasql/asyncsqlalchemy.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/balancer_policy/base.py` & `hasql-0.5.9/hasql/balancer_policy/base.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/balancer_policy/greedy.py` & `hasql-0.5.9/hasql/balancer_policy/greedy.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/balancer_policy/random_weighted.py` & `hasql-0.5.9/hasql/balancer_policy/random_weighted.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/balancer_policy/round_robin.py` & `hasql-0.5.9/hasql/balancer_policy/round_robin.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/base.py` & `hasql-0.5.9/hasql/base.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/psycopg3.py` & `hasql-0.5.9/hasql/psycopg3.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql/utils.py` & `hasql-0.5.9/hasql/utils.py`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/hasql.egg-info/PKG-INFO` & `hasql-0.5.9/hasql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasql
-Version: 0.5.8
+Version: 0.5.9
 Summary: hasql is a module for acquiring actual connections with masters and replicas
 Home-page: UNKNOWN
 Author: Vladislav Bakaev <vlad@bakaev.tech>, Dmitry Orlov <me@mosquito.su>
 Author-email: vlad@bakaev.tech, me@mosquito.su
 License: Apache 2
 Project-URL: Source, https://github.com/aiokitchen/hasql
 Project-URL: Tracker, https://github.com/aiokitchen/hasql/issues
@@ -53,15 +53,15 @@
 * completely asynchronous api
 * automatic detection of the host role in the cluster
 * health-checks for each host and automatic traffic outage for
   unavailable hosts
 * autodetection of hosts role changes, in case replica
   host will be promoted to master
 * different policies for load balancing
-* support for ``asyncpg``, ``psycopg3`` and ``aiopg``
+* support for ``asyncpg``, ``psycopg3``, ``aiopg``, ``sqlalchemy`` and ``asyncpgsa``
 
 
 Usage
 =====
 
 Some useful examples
 
@@ -127,15 +127,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 Code example using ``aiopg.sa``:
 
 .. code-block:: python
 
     from hasql.aiopg_sa import PoolManager
@@ -148,15 +148,15 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 For ``asyncpg``
 ~~~~~~~~~~~~~~~
 
 **asyncpg** must be installed as a requirement
 
@@ -172,17 +172,54 @@
 
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
+For ``sqlalchemy``
+~~~~~~~~~~~~~~~~~~
+
+**sqlalchemy[asyncio] & asyncpg** must be installed as requirements
+
+.. code-block:: python
+
+    from hasql.asyncsqlalchemy import PoolManager
+
+    hosts = ",".join([
+        "master-host:5432",
+        "replica-host-1:5432",
+        "replica-host-2:5432",
+    ])
+
+    multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
+
+
+    async def create_pool(dsn) -> PoolManager:
+        pool = PoolManager(
+            multihost_dsn,
+
+            # Use master for acquire_replica, if no replicas available
+            fallback_master=True,
+
+            # You can pass pool-specific options
+            pool_factory_kwargs=dict(
+                pool_size=10,
+                max_overflow=5
+            )
+        )
+
+        # Waiting for 1 master and 1 replica will be available
+        await pool.ready(masters_count=1, replicas_count=1)
+        return pool
+
+
 For ``asyncpgsa``
 ~~~~~~~~~~~~~~~~~
 
 **asyncpgsa** must be installed as a requirement
 
 .. code-block:: python
 
@@ -197,16 +234,16 @@
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
         await asyncio.gather(
-            pool_manager.wait_masters_ready(1),
-            pool_manager.wait_replicas_ready(1)
+            pool.wait_masters_ready(1),
+            pool.wait_replicas_ready(1)
         )
         return pool
 
 
 For ``psycopg3``
 ~~~~~~~~~~~~~~~~
 
@@ -224,15 +261,15 @@
     ])
     multihost_dsn = f"postgresql://user:password@{hosts}/dbname"
 
     async def create_pool(dsn) -> PoolManager:
         pool = PoolManager(multihost_dsn)
 
         # Waiting for 1 master and 1 replica will be available
-        await pool_manager.ready(masters_count=1, replicas_count=1)
+        await pool.ready(masters_count=1, replicas_count=1)
         return pool
 
 
 Acquiring connections
 *********************
 
 Connections should be acquired with async context manager:
```

### Comparing `hasql-0.5.8/hasql.egg-info/SOURCES.txt` & `hasql-0.5.9/hasql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hasql-0.5.8/setup.py` & `hasql-0.5.9/setup.py`

 * *Files identical despite different names*

