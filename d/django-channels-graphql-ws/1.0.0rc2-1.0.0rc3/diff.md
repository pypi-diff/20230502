# Comparing `tmp/django_channels_graphql_ws-1.0.0rc2.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_channels_graphql_ws-1.0.0rc2.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc3.tar", max compression
```

## Comparing `django_channels_graphql_ws-1.0.0rc2.tar` & `django_channels_graphql_ws-1.0.0rc3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-04-27 20:51:46.646275 django_channels_graphql_ws-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     1433 2023-04-27 20:51:46.646802 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10111 2023-04-27 20:51:46.647155 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/client.py
--rw-r--r--   0        0        0     2637 2023-04-27 20:51:46.647317 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/dict_as_object.py
--rw-r--r--   0        0        0    58225 2023-04-27 21:28:38.470594 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     3850 2023-04-27 20:51:46.647978 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    16451 2023-04-27 20:51:46.648225 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4816 2023-04-27 20:51:46.648455 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6939 2023-04-27 20:51:46.648726 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     8478 2023-04-27 21:29:50.214108 django_channels_graphql_ws-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10111 2023-05-02 12:50:55.309876 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    56638 2023-05-02 20:35:56.015983 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16451 2023-05-02 12:50:55.311452 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4816 2023-05-02 12:50:55.311701 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8478 2023-05-02 20:43:08.691294 django_channels_graphql_ws-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc3/PKG-INFO
```

### Comparing `django_channels_graphql_ws-1.0.0rc2/LICENSE` & `django_channels_graphql_ws-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/client.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/dict_as_object.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/dict_as_object.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,16 @@
     Dict,
     Optional,
     Type,
     Union,
     cast,
 )
 
-import asgiref.sync
 import channels.db
 import channels.generic.websocket as ch_websocket
-import django.db.models.query
 import graphene
 import graphql
 import graphql.error
 import graphql.execution
 import graphql.pyutils
 import graphql.utilities
 
@@ -136,32 +134,23 @@
     # ```python
     # async def my_middleware(next_middleware, root, info, *args, **kwds):
     #     result = next_middleware(root, info, *args, **kwds)
     #     if graphql.pyutils.is_awaitable(result):
     #        result = await result
     #     return result
     # ```
+    # The first middleware in the middlewares list will be the closest
+    # to the resolver in the middlewares call stack.
     # For more information read docs:
     # - https://docs.graphene-python.org/en/latest/execution/middleware/#middleware
     # - https://graphql-core-3.readthedocs.io/en/latest/diffs.html#custom-middleware
     # Docs about async middlewares are still missing - read the
     # GraphQL-core sources to know more.
     middleware: Sequence = []
 
-    # A function to execute synchronous resolvers, middlewares, request
-    # parsing functions, etc. from asynchronous context. The default is
-    # a ASGI thread pool in `channels.db.database_sync_to_async` which
-    # cleans up the database connections so resolvers can safely work
-    # with a database.
-    # https://channels.readthedocs.io/en/latest/topics/databases.html#database-sync-to-async
-    # You can redefine this to use designated thread pool or to use
-    # `asgiref.sync.sync_to_async` if you are sure your resolvers does
-    # not work with the database.
-    sync_to_async: asgiref.sync.SyncToAsync = channels.db.database_sync_to_async
-
     # Subscription implementation shall return this to tell consumer
     # to suppress subscription notification.
     SKIP = object()
 
     async def on_connect(self, payload):
         """Client connection handler.
 
@@ -587,14 +576,16 @@
             op_name = payload.get("operationName")
             variables = payload.get("variables", {})
 
             # Prepare a context object.
             context = DictAsObject({})
             context.channels_scope = self.scope
             context.channel_name = self.channel_name
+            context.graphql_operation_name = op_name
+            context.graphql_operation_id = op_id
 
             # Process the request with Graphene and GraphQL-core.
             doc_ast, op_ast, errors = await self._on_gql_start__parse_query(
                 op_name, query
             )
             if errors:
                 await self._send_gql_data(op_id, None, errors)
@@ -611,22 +602,23 @@
                 functions as middleware.
                 """
                 return await self._on_gql_start__root_middleware(
                     op_id, op_name, *args, **kwds
                 )
 
             # NOTE: Middlewares order is important, root middleware
-            # should always be the closest to the real resolver (first
-            # in the middleware list).
-            middleware_manager: Optional[
-                graphql.MiddlewareManager
-            ] = graphql.MiddlewareManager(
-                unbound_root_middleware,
-                *self.middleware,
-            )
+            # should always be the farest from the real resolver (last
+            # in the middleware list). Because we want to calculate
+            # resolver execution time with middlewares included.
+            middlewares = list(self.middleware)
+            if self.warn_resolver_timeout is not None:
+                middlewares.append(unbound_root_middleware)
+            middleware_manager: Optional[graphql.MiddlewareManager] = None
+            if middlewares:
+                middleware_manager = graphql.MiddlewareManager(*middlewares)
 
             # If the operation is subscription.
             if op_ast.operation == graphql.language.ast.OperationType.SUBSCRIPTION:
                 LOG.debug(
                     "Subscription request. Operation ID: %s, operation name: %s.)",
                     op_id,
                     op_name,
@@ -637,15 +629,17 @@
                 subscr_result = await self._on_gql_start__subscribe(
                     doc_ast,
                     operation_name=op_name,
                     root_value=None,
                     variable_values=variables,
                     context_value=context,
                     subscribe_field_resolver=functools.partial(
-                        self._on_gql_start__initialize_subscription_stream, op_id
+                        self._on_gql_start__initialize_subscription_stream,
+                        op_id,
+                        op_name,
                     ),
                     middleware=middleware_manager,
                     execution_context_class=self._SubscriptionExecutionContext,
                 )
 
                 # When subscr_result is an AsyncGenerator, consume
                 # stream of notifications and send them to clients.
@@ -708,15 +702,15 @@
                 # containing error) fallback to standard handling below.
                 operation_result = cast(graphql.ExecutionResult, subscr_result)
 
             # If the operation is query or mutation.
             else:
                 LOG.debug("New query/mutation. Operation %s(%s).", op_name, op_id)
 
-                if self.warn_operation_timeout:
+                if self.warn_operation_timeout is not None:
                     start_time = time.perf_counter()
 
                 # Standard name for "IntrospectionQuery". We might also
                 # check that
                 # `doc_ast.definitions[0].selection_set.selections[0].name.value`
                 # equals to `__schema`. This is a more robust way. But
                 # it will eat up more CPU pre each query. For now lets
@@ -735,15 +729,15 @@
                     context_value=context,
                     middleware=middleware_manager,
                 )
                 if inspect.isawaitable(exec_result):
                     exec_result = await exec_result
                 operation_result = cast(graphql.ExecutionResult, exec_result)
 
-                if self.warn_operation_timeout:
+                if self.warn_operation_timeout is not None:
                     duration = time.perf_counter() - start_time
                     if duration >= self.warn_operation_timeout:
                         LOG.warning(
                             "Operation %s(%s) took %.6f seconds. Debug"
                             " log contains full operation details.",
                             op_name,
                             op_id,
@@ -799,17 +793,17 @@
         Returns:
             Tuple with three optional fields:
                 0: AST of parsed GraphQL document.
                 1: GraphQL operation definition.
                 2: Sequence of errors.
         """
 
-        res = await self.sync_to_async(self._on_gql_start__parse_query_sync_cached)(
-            op_name, query
-        )
+        res = await channels.db.database_sync_to_async(
+            self._on_gql_start__parse_query_sync_cached
+        )(op_name, query)
 
         doc_ast: Optional[graphql.DocumentNode] = res[0]
         op_ast: Optional[graphql.OperationDefinitionNode] = res[1]
         errors: Optional[Sequence[graphql.GraphQLError]] = res[2]
 
         return (doc_ast, op_ast, errors)
 
@@ -915,22 +909,16 @@
         root,
         info: graphql.GraphQLResolveInfo,
         *args,
         **kwds,
     ):
         """Root middleware injected right before resolver invocation.
 
-        This middleware is here to do two things:
-        1. Offload sync resolvers to the thread out of main event loop.
-        2. Issue a warning if resolver execution time exceeds a limit.
-
-        It is highly probable that resolvers will invoke
-        blocking operations, e.g. database operations. To avoid
-        blocking eventloop this method offloads sync resolvers
-        to the thread pool wrapping it into sync_to_async.
+        This middleware issues a warning if resolver execution time
+        exceeds a limit.
 
         Since this middleware always comes first in the list of
         middlewares, it always receives resolver as the first
         argument instead of another middleware.
 
         This is a part of START message processing routine so the name
         prefixed with `_on_gql_start__` to make this explicit.
@@ -943,51 +931,26 @@
         Returns:
             Any value: result returned by the resolver.
             AsyncGenerator: when subscription starts.
         """
 
         # Unwrap resolver from functools.partial or other wrappers.
         real_resolver = self._on_gql_start__unwrap(next_middleware)
-        module = getattr(real_resolver, "__module__", "")
-
-        # Do not offload async resolvers and resolvers from
-        # GraphQL-core/Graphene since they are not blocking.
-        if (
-            not module.startswith("graphql.type.")
-            and not module.startswith("graphene.types.")
-            and not asyncio.iscoroutinefunction(real_resolver)
-        ):
-            # Offload synchronous resolvers.
-            @functools.wraps(next_middleware)
-            def wrapped_next_middleware(root, info, *args, **kwds):
-                result = next_middleware(root, info, *args, **kwds)
-                # Manually evaluate QuerySet, otherwise we will
-                # eventually receive SynchronousOnlyOperation error:
-                # "You cannot call this from an async context - use a
-                # thread or sync_to_async.". This happens when
-                # unevaluated QuerySet moves out of its sync context.
-                if isinstance(result, django.db.models.query.QuerySet):
-                    result = list(result)
-                return result
-
-            next_resolver = self.sync_to_async(wrapped_next_middleware)
-        else:
-            next_resolver = next_middleware
 
         # Start measuring resolver execution time.
-        if self.warn_resolver_timeout:
+        if self.warn_resolver_timeout is not None:
             start_time = time.perf_counter()
 
         # Execute resolver.
-        result = next_resolver(root, info, *args, **kwds)
+        result = next_middleware(root, info, *args, **kwds)
         if inspect.isawaitable(result):
             result = await result
 
         # Warn about long resolver execution if the time limit exceeds.
-        if self.warn_resolver_timeout:
+        if self.warn_resolver_timeout is not None:
             duration = time.perf_counter() - start_time
             if duration >= self.warn_resolver_timeout:
                 pretty_name = f"{real_resolver.__qualname__}"
                 if hasattr(real_resolver, "__self__"):
                     pretty_name = f"{real_resolver.__self__.__qualname__}.{pretty_name}"
                 LOG.warning(
                     "Resolver %s took %.3f seconds (>%.3f)!"
@@ -1011,29 +974,38 @@
         if isinstance(fn, functools.partial):
             fn = self._on_gql_start__unwrap(fn.func)
         elif hasattr(fn, "__wrapped__"):
             fn = self._on_gql_start__unwrap(fn.__wrapped__)
         return fn
 
     async def _on_gql_start__initialize_subscription_stream(
-        self, op_id: int, root: Any, info: graphql.GraphQLResolveInfo, *args, **kwds
+        self,
+        operation_id: int,
+        operation_name: str,
+        root: Any,
+        info: graphql.GraphQLResolveInfo,
+        *args,
+        **kwds,
     ):
         """Create asynchronous generator with subscription events.
 
         Called inside `_on_gql_start__subscribe` function by
         graphql-core as `subscribe_field_resolver` argument.
 
         This is a part of START message processing routine so the name
         prefixed with `_on_gql_start__` to make this explicit.
         """
         # Graphene stores original subscription class in `graphene_type`
         # field of `return_type` object. Since subscriptions are build
         # on top of `graphene` we always have graphene specific
         # `return_type` class.
-        subscription_class = info.return_type.graphene_type  # type: ignore[union-attr]
+        return_type = info.return_type
+        while graphql.is_wrapping_type(return_type):
+            return_type = return_type.of_type  # type: ignore[union-attr]
+        subscription_class = return_type.graphene_type  # type: ignore[union-attr]
 
         # It is ok to access private fields of `Subscription`
         # implementation. `Subscription` class used to create
         # subscriptions as graphene object but actually it is a part of
         # consumer implementation.
         # pylint: disable=protected-access
 
@@ -1086,19 +1058,18 @@
 
             The `cls._meta.unsubscribed` might do blocking operations,
             so offload it to the thread.
             """
 
             if unsubscribed is None:
                 return None
+            result = unsubscribed(None, info, *args, **kwds)
             # Properly handle `async def unsubscribed`.
-            if asyncio.iscoroutinefunction(unsubscribed):
-                await unsubscribed(None, info, *args, **kwds)
-            else:
-                await self.sync_to_async(unsubscribed)(None, info, *args, **kwds)
+            if inspect.isawaitable(result):
+                result = await result
 
         def enqueue_notification(payload):
             """Put notification to the queue.
 
             Called by the WebSocket consumer (instance of the
             GraphqlWsConsumer subclass) when it receives the broadcast
             message (from the Channels group) sent by the
@@ -1115,18 +1086,17 @@
                     except asyncio.QueueFull:
                         # The queue is full - issue a warning and throw
                         # away the oldest item from the queue.
                         # NOTE: Queue with the size 1 means that it is
                         # safe to drop intermediate notifications.
                         if notification_queue.maxsize != 1:
                             LOG.warning(
-                                "Subscription notification dropped!"
-                                " Operation %s(%s).",
-                                info.context.graphql_operation_name,
-                                info.context.graphql_operation_id,
+                                "Subscription notification dropped! Operation %s(%s).",
+                                operation_name,
+                                operation_id,
                             )
                         notification_queue.get_nowait()
                         notification_queue.task_done()
 
                         # Try to put the incoming item to the queue
                         # within the same lock. This is an speed
                         # optimization.
@@ -1138,23 +1108,23 @@
                             # Kind'a impossible to get here, but if we
                             # do, then we should retry until the queue
                             # have capacity to process item.
                             pass
 
         waitlist = []
         for group in groups:
-            self._sids_by_group.setdefault(group, []).append(op_id)
+            self._sids_by_group.setdefault(group, []).append(operation_id)
             waitlist.append(
                 asyncio.create_task(
                     self._channel_layer.group_add(group, self.channel_name)
                 )
             )
-        self._subscriptions[op_id] = self._SubInf(
+        self._subscriptions[operation_id] = self._SubInf(
             groups=groups,
-            sid=op_id,
+            sid=operation_id,
             unsubscribed_callback=unsubscribed_callback,
             enqueue_notification=enqueue_notification,
         )
         if waitlist:
             await asyncio.wait(waitlist)
 
         _deserialize = channels.db.database_sync_to_async(Serializer.deserialize)
```

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/serializer.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/subscription.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/testing.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/transport.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc2/pyproject.toml` & `django_channels_graphql_ws-1.0.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # --------------------------------------------------------------- POETRY
 # Python packaging and dependency management.
 # Docs: https://python-poetry.org/docs/
 [tool.poetry]
 name = "django-channels-graphql-ws"
-version = "v1.0.0rc2"
+version = "v1.0.0rc3"
 description = """Django Channels based WebSocket GraphQL server with Graphene-like subscriptions"""
 authors = ["Alexander A. Prokhorov <alexander.prokhorov@datadvance.net>"]
 homepage = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 repository = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 license = "MIT"
 packages = [
     { include = "channels_graphql_ws/" },
```

### Comparing `django_channels_graphql_ws-1.0.0rc2/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

