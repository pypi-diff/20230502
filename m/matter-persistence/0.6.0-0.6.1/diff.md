# Comparing `tmp/matter_persistence-0.6.0-py3-none-any.whl.zip` & `tmp/matter_persistence-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15225 bytes, number of entries: 26
+Zip file size: 15291 bytes, number of entries: 26
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_persistence/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 matter_persistence/__init__.py
 -rw-r--r--  2.0 unx      191 b- defN 20-Feb-02 00:00 matter_persistence/exceptions.py
 -rw-r--r--  2.0 unx      332 b- defN 20-Feb-02 00:00 matter_persistence/cache/__init__.py
 -rw-r--r--  2.0 unx     1349 b- defN 20-Feb-02 00:00 matter_persistence/cache/client.py
 -rw-r--r--  2.0 unx      748 b- defN 20-Feb-02 00:00 matter_persistence/cache/config.py
 -rw-r--r--  2.0 unx      138 b- defN 20-Feb-02 00:00 matter_persistence/cache/exceptions.py
@@ -14,15 +14,15 @@
 -rw-r--r--  2.0 unx     4338 b- defN 20-Feb-02 00:00 matter_persistence/database/orm.py
 -rw-r--r--  2.0 unx     1241 b- defN 20-Feb-02 00:00 matter_persistence/database/session.py
 -rw-r--r--  2.0 unx      668 b- defN 20-Feb-02 00:00 matter_persistence/database/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/__init__.py
 -rw-r--r--  2.0 unx     1907 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/command.py
 -rw-r--r--  2.0 unx      216 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/exceptions.py
 -rw-r--r--  2.0 unx     2117 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/utils.py
--rw-r--r--  2.0 unx      897 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/resources/env.py
+-rw-r--r--  2.0 unx      980 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/resources/env.py
 -rw-r--r--  2.0 unx      510 b- defN 20-Feb-02 00:00 matter_persistence/database/migrations/resources/script.py.mako
-?rw-r--r--  2.0 unx     5761 b- defN 20-Feb-02 00:00 matter_persistence-0.6.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_persistence-0.6.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 matter_persistence-0.6.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_persistence-0.6.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     2487 b- defN 20-Feb-02 00:00 matter_persistence-0.6.0.dist-info/RECORD
-26 files, 31654 bytes uncompressed, 11067 bytes compressed:  65.0%
+?rw-r--r--  2.0 unx     5828 b- defN 20-Feb-02 00:00 matter_persistence-0.6.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_persistence-0.6.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 matter_persistence-0.6.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_persistence-0.6.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     2487 b- defN 20-Feb-02 00:00 matter_persistence-0.6.1.dist-info/RECORD
+26 files, 31804 bytes uncompressed, 11133 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -57,23 +57,23 @@
 
 Filename: matter_persistence/database/migrations/resources/env.py
 Comment: 
 
 Filename: matter_persistence/database/migrations/resources/script.py.mako
 Comment: 
 
-Filename: matter_persistence-0.6.0.dist-info/METADATA
+Filename: matter_persistence-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: matter_persistence-0.6.0.dist-info/WHEEL
+Filename: matter_persistence-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: matter_persistence-0.6.0.dist-info/entry_points.txt
+Filename: matter_persistence-0.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: matter_persistence-0.6.0.dist-info/licenses/LICENSE
+Filename: matter_persistence-0.6.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_persistence-0.6.0.dist-info/RECORD
+Filename: matter_persistence-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_persistence/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

## matter_persistence/database/migrations/resources/env.py

```diff
@@ -10,16 +10,20 @@
 db_config: DatabaseConfig = config.attributes["db_config"]
 
 for i in db_config.migration.models:
     subclass = load_DatabaseBaseModel_subclass(i)
 
 target_metadata = DatabaseBaseModel.metadata
 
-context.configure(connection=config.attributes["connection"], target_metadata=target_metadata)
+has_schema_defined = bool(db_config.migration.version_schema)
+
+context.configure(
+    connection=config.attributes["connection"], target_metadata=target_metadata, include_schemas=has_schema_defined
+)
 
 with context.begin_transaction():
-    if bool(db_config.migration.version_schema):
+    if has_schema_defined:
         try:
             context.execute(f"SET search_path TO {db_config.migration.version_schema}")
         except sqlalchemy.exc.OperationalError:  # pragma: no cover
             logging.warning("Database does not support schemas changing.")
     context.run_migrations()
```

## Comparing `matter_persistence-0.6.0.dist-info/METADATA` & `matter_persistence-0.6.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-persistence
-Version: 0.6.0
+Version: 0.6.1
 Summary: Matter persistance library.
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-persistence#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-persistence/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-persistence
 Author-email: Rômulo Jales <romulo@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,17 +20,17 @@
 Requires-Dist: pydantic~=1.10
 Provides-Extra: cache
 Requires-Dist: aiocache==0.12.1; extra == 'cache'
 Provides-Extra: cache-memcached
 Requires-Dist: aiocache[memcached]==0.12.1; extra == 'cache-memcached'
 Requires-Dist: matter-persistence[cache]; extra == 'cache-memcached'
 Provides-Extra: database
-Requires-Dist: sqlalchemy[asyncio]==2.0.10; extra == 'database'
+Requires-Dist: sqlalchemy[asyncio]==2.0.12; extra == 'database'
 Provides-Extra: database-migrations
-Requires-Dist: alembic==1.10.3; extra == 'database-migrations'
+Requires-Dist: alembic==1.10.4; extra == 'database-migrations'
 Requires-Dist: matter-persistence[database]; extra == 'database-migrations'
 Requires-Dist: python-dotenv~=1.0; extra == 'database-migrations'
 Requires-Dist: typer==0.7.0; extra == 'database-migrations'
 Provides-Extra: database-postgresql
 Requires-Dist: asyncpg==0.27.0; extra == 'database-postgresql'
 Requires-Dist: matter-persistence[database]; extra == 'database-postgresql'
 Requires-Dist: sqlalchemy[postgresql]==2.0.10; extra == 'database-postgresql'
@@ -166,20 +166,20 @@
 ```console
 migrations apply --config python.path.to.your.db_config.instance 
 ```
 ### Schema support
 
 If you need deal with schemas in your database, you can define one for you versions:
 
-
 ```python
 from matter_persistence.database import DatabaseConfig
 
 db_config = DatabaseConfig(connection_uri="sqlite:///test.db",
                            migration={"path": <a path to your migrations folder>,
                                       "models": [<a list of full qualified class path of your ORM models>]},
                                       "version_schema": "another_schema")
 ``` 
 
+However, the autogenerated migrations **must** be manually edited. 
 ### Contributing
 
 for contributions, check the [CONTRIBUTING.md](CONTRIBUTING.md) file
```

## Comparing `matter_persistence-0.6.0.dist-info/licenses/LICENSE` & `matter_persistence-0.6.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_persistence-0.6.0.dist-info/RECORD` & `matter_persistence-0.6.1.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-matter_persistence/__about__.py,sha256=5TDLdrvWXWaFMLvq-aDN7cNecCvFD4lkVf7pxJhM99s,134
+matter_persistence/__about__.py,sha256=Z3JB6C4BUXcB87qk_uVec9Wqp8Qe58L1oXE-Tf_UmiY,134
 matter_persistence/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 matter_persistence/exceptions.py,sha256=619KHHqroYNuiFeb7Baw_1yZxU8IM5HcKMbFvfzvp94,191
 matter_persistence/cache/__init__.py,sha256=Fxx6JYxthO32V6zGz-0aXBNigOuf9rmVsYVQCjlpFJw,332
 matter_persistence/cache/client.py,sha256=RF63DQvyXvS-UZ9gW2QGL3F_9H_c5h6WXNXlJpNeBuA,1349
 matter_persistence/cache/config.py,sha256=n-jZnTF2WQgBeKbEubGuqhj973WxSMJNiisRL_eS2wo,748
 matter_persistence/cache/exceptions.py,sha256=rjpR3TwBs7S5K8RH2O1jP_rHGxq4Y1nhXSvJW2SrEec,138
 matter_persistence/database/__init__.py,sha256=RDDX9X24xYgFmqY0zcUpzRhIlpZvPB8SHRf1neyp9H4,1003
@@ -13,14 +13,14 @@
 matter_persistence/database/orm.py,sha256=71giNFRuAI8t5n23OX0qi1qKxyv3XeKBduLJKxBEz1U,4338
 matter_persistence/database/session.py,sha256=MokSXLDaJAmC_vgJG_yyxNSyFXxV0dzkLL0KNMKxDDQ,1241
 matter_persistence/database/utils.py,sha256=F92v87eOETc6P-p_lfTXvBBv0lq1_m2QZX18iriJOWs,668
 matter_persistence/database/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 matter_persistence/database/migrations/command.py,sha256=6NW1Zj4wU171TcB6SSOIc5dRer2oAlEQubBTBqUeLkY,1907
 matter_persistence/database/migrations/exceptions.py,sha256=8zb4aOGHJPrIQ1kY3ZCLLgU-9SvT8iWjZ1JUZCbEZ1M,216
 matter_persistence/database/migrations/utils.py,sha256=muI6zq0Y04m33B2W80S6W_MfPZEP5unaiyWPPlAUd7o,2117
-matter_persistence/database/migrations/resources/env.py,sha256=En9fi6QAPwXBhkA5fz8hV4vx6bISthVgs5wsaw0LiNY,897
+matter_persistence/database/migrations/resources/env.py,sha256=YEbCBdW0Dg9K_4zPySb5cWzMM1VyBbt_e86t8LbckhY,980
 matter_persistence/database/migrations/resources/script.py.mako,sha256=HNlf26BI1xvQKjiUojnj15BPrVUfVVr81IOgliJf83c,510
-matter_persistence-0.6.0.dist-info/METADATA,sha256=FFgjX9jFgGtNkh-DCQlQ1UotNwMhdnGv2C6R0hDEhEQ,5761
-matter_persistence-0.6.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-matter_persistence-0.6.0.dist-info/entry_points.txt,sha256=2ZQRC328nPFzSmFv0ya4FSUFL9ZtpUD265kqZoW7c_A,82
-matter_persistence-0.6.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_persistence-0.6.0.dist-info/RECORD,,
+matter_persistence-0.6.1.dist-info/METADATA,sha256=2dpkrwckG3O5u97PmuqYCp2X0D2_FFbjj9NClgRZ6ts,5828
+matter_persistence-0.6.1.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+matter_persistence-0.6.1.dist-info/entry_points.txt,sha256=2ZQRC328nPFzSmFv0ya4FSUFL9ZtpUD265kqZoW7c_A,82
+matter_persistence-0.6.1.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_persistence-0.6.1.dist-info/RECORD,,
```

