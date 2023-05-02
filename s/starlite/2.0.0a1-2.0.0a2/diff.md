# Comparing `tmp/starlite-2.0.0a1.tar.gz` & `tmp/starlite-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlite-2.0.0a1.tar", max compression
+gzip compressed data, was "starlite-2.0.0a2.tar", max compression
```

## Comparing `starlite-2.0.0a1.tar` & `starlite-2.0.0a2.tar`

### file list

```diff
@@ -1,216 +1,259 @@
--rw-r--r--   0        0        0     1085 2023-03-04 16:58:58.355700 starlite-2.0.0a1/LICENSE
--rw-r--r--   0        0        0    45301 2023-03-04 16:58:58.355700 starlite-2.0.0a1/README.md
--rw-r--r--   0        0        0     6558 2023-03-04 16:58:58.387702 starlite-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      643 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/__init__.py
--rw-r--r--   0        0        0      128 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/__main__.py
--rw-r--r--   0        0        0    36179 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/app.py
--rw-r--r--   0        0        0       76 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/__init__.py
--rw-r--r--   0        0        0     8507 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/asgi_router.py
--rw-r--r--   0        0        0      345 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7717 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5748 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2509 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1235 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1464 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/asgi/utils.py
--rw-r--r--   0        0        0     2202 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/background_tasks.py
--rw-r--r--   0        0        0     1592 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cache.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/commands/__init__.py
--rw-r--r--   0        0        0     4247 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/commands/core.py
--rw-r--r--   0        0        0     2332 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/commands/schema.py
--rw-r--r--   0        0        0     2039 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/commands/sessions.py
--rw-r--r--   0        0        0      718 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/main.py
--rw-r--r--   0        0        0    10634 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/cli/utils.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/__init__.py
--rw-r--r--   0        0        0     1711 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/allowed_hosts.py
--rw-r--r--   0        0        0    11306 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/app.py
--rw-r--r--   0        0        0     2102 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/cache.py
--rw-r--r--   0        0        0     2703 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/compression.py
--rw-r--r--   0        0        0     5149 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/cors.py
--rw-r--r--   0        0        0     1743 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/csrf.py
--rw-r--r--   0        0        0     8455 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/logging.py
--rw-r--r--   0        0        0     5435 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/openapi.py
--rw-r--r--   0        0        0     3547 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/static_files.py
--rw-r--r--   0        0        0     1825 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/config/template.py
--rw-r--r--   0        0        0     1922 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/connection/__init__.py
--rw-r--r--   0        0        0    10991 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/connection/base.py
--rw-r--r--   0        0        0     6965 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/connection/request.py
--rw-r--r--   0        0        0     9082 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/connection/websocket.py
--rw-r--r--   0        0        0      838 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/constants.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/htmx/request.py
--rw-r--r--   0        0        0     8303 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/htmx/response.py
--rw-r--r--   0        0        0     1188 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/htmx/types.py
--rw-r--r--   0        0        0     4795 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/htmx/utils.py
--rw-r--r--   0        0        0     2590 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/jinja.py
--rw-r--r--   0        0        0      485 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28846 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     4067 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     7031 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3915 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      260 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0     4162 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2131 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      794 2023-03-04 16:58:58.387702 starlite-2.0.0a1/starlite/contrib/opentelemetry/utils.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/piccolo_orm/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/__init__.py
--rw-r--r--   0        0        0    13769 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/config.py
--rw-r--r--   0        0        0    19321 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/plugin.py
--rw-r--r--   0        0        0     1222 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/types.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/contrib/tortoise_orm/__init__.py
--rw-r--r--   0        0        0     8678 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/controller.py
--rw-r--r--   0        0        0    16461 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/data_extractors.py
--rw-r--r--   0        0        0      797 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/__init__.py
--rw-r--r--   0        0        0     3653 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/cookie.py
--rw-r--r--   0        0        0    12870 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/headers.py
--rw-r--r--   0        0        0     3167 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/multi_dicts.py
--rw-r--r--   0        0        0      938 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/response_header.py
--rw-r--r--   0        0        0     9240 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/state.py
--rw-r--r--   0        0        0     3398 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/upload_file.py
--rw-r--r--   0        0        0     7211 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/datastructures/url.py
--rw-r--r--   0        0        0     2360 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/di.py
--rw-r--r--   0        0        0    12913 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/dto.py
--rw-r--r--   0        0        0     1566 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/enums.py
--rw-r--r--   0        0        0      201 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/events/__init__.py
--rw-r--r--   0        0        0     2328 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/events/emitter.py
--rw-r--r--   0        0        0     1116 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/events/listener.py
--rw-r--r--   0        0        0     1142 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/exceptions/__init__.py
--rw-r--r--   0        0        0     1075 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4220 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1189 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5402 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/file_system.py
--rw-r--r--   0        0        0      274 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/__init__.py
--rw-r--r--   0        0        0     3778 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    10747 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/base.py
--rw-r--r--   0        0        0      263 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     8346 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    24377 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    57284 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0     1179 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/utils.py
--rw-r--r--   0        0        0     3769 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/handlers/websocket_handlers.py
--rw-r--r--   0        0        0       66 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/__init__.py
--rw-r--r--   0        0        0     3828 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/cleanup.py
--rw-r--r--   0        0        0     4130 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/dependencies.py
--rw-r--r--   0        0        0    12988 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/extractors.py
--rw-r--r--   0        0        0    19378 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2668 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/logging/__init__.py
--rw-r--r--   0        0        0     1122 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/logging/picologging.py
--rw-r--r--   0        0        0      867 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/logging/standard.py
--rw-r--r--   0        0        0      536 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/logging/utils.py
--rw-r--r--   0        0        0      385 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/__init__.py
--rw-r--r--   0        0        0     2933 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3362 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/authentication.py
--rw-r--r--   0        0        0     5248 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/base.py
--rw-r--r--   0        0        0     8284 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/compression.py
--rw-r--r--   0        0        0     2541 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/cors.py
--rw-r--r--   0        0        0     6441 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     6967 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/debug_response.py
--rw-r--r--   0        0        0     8150 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13320 2023-03-04 16:58:58.391702 starlite-2.0.0a1/starlite/middleware/logging.py
--rw-r--r--   0        0        0    10403 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/rate_limit.py
--rw-r--r--   0        0        0       69 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/session/__init__.py
--rw-r--r--   0        0        0     7908 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/session/base.py
--rw-r--r--   0        0        0    10250 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/session/client_side.py
--rw-r--r--   0        0        0     7982 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/session/server_side.py
--rw-r--r--   0        0        0     2010 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/middleware/utils.py
--rw-r--r--   0        0        0     5844 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/multipart.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/openapi/__init__.py
--rw-r--r--   0        0        0     6441 2023-03-04 16:58:58.395702 starlite-2.0.0a1/starlite/openapi/constants.py
--rw-r--r--   0        0        0    17405 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/controller.py
--rw-r--r--   0        0        0      669 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/datastructures.py
--rw-r--r--   0        0        0      924 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/enums.py
--rw-r--r--   0        0        0     9390 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/parameters.py
--rw-r--r--   0        0        0     4829 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/path_item.py
--rw-r--r--   0        0        0     1261 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/request_body.py
--rw-r--r--   0        0        0     9582 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/responses.py
--rw-r--r--   0        0        0    15959 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/schema.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10625 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5150 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7306 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     2648 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/openapi/utils.py
--rw-r--r--   0        0        0    10680 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/pagination.py
--rw-r--r--   0        0        0    16725 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/params.py
--rw-r--r--   0        0        0     2360 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/parsers.py
--rw-r--r--   0        0        0     6296 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/partial.py
--rw-r--r--   0        0        0      413 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/plugins/__init__.py
--rw-r--r--   0        0        0     7197 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/plugins/base.py
--rw-r--r--   0        0        0     4032 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/plugins/piccolo_orm.py
--rw-r--r--   0        0        0     6040 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/plugins/tortoise_orm.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/py.typed
--rw-r--r--   0        0        0      278 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/__init__.py
--rw-r--r--   0        0        0    12174 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/base.py
--rw-r--r--   0        0        0     8849 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/file.py
--rw-r--r--   0        0        0     2352 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/redirect.py
--rw-r--r--   0        0        0     4856 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/streaming.py
--rw-r--r--   0        0        0     2978 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response/template.py
--rw-r--r--   0        0        0    15121 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/response_containers.py
--rw-r--r--   0        0        0    14060 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/router.py
--rw-r--r--   0        0        0      191 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/routes/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/routes/asgi.py
--rw-r--r--   0        0        0     6308 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/routes/base.py
--rw-r--r--   0        0        0    13286 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/routes/http.py
--rw-r--r--   0        0        0     3056 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/security/__init__.py
--rw-r--r--   0        0        0     7214 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/security/base.py
--rw-r--r--   0        0        0      188 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5679 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/security/session_auth/auth.py
--rw-r--r--   0        0        0     4935 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/security/session_auth/middleware.py
--rw-r--r--   0        0        0     6493 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/serialization.py
--rw-r--r--   0        0        0      197 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/signature/__init__.py
--rw-r--r--   0        0        0    11634 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/signature/models.py
--rw-r--r--   0        0        0    10686 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/signature/parsing.py
--rw-r--r--   0        0        0     2380 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/signature/utils.py
--rw-r--r--   0        0        0       79 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/static_files/__init__.py
--rw-r--r--   0        0        0     4998 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/static_files/base.py
--rw-r--r--   0        0        0     7775 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/status_codes.py
--rw-r--r--   0        0        0        0 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/storage/__init__.py
--rw-r--r--   0        0        0     3563 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/storage/base.py
--rw-r--r--   0        0        0     4759 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/storage/file.py
--rw-r--r--   0        0        0     3619 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/storage/memory.py
--rw-r--r--   0        0        0     6173 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/storage/redis.py
--rw-r--r--   0        0        0      117 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/template/__init__.py
--rw-r--r--   0        0        0     3947 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/template/base.py
--rw-r--r--   0        0        0      402 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-03-04 16:58:58.399702 starlite-2.0.0a1/starlite/testing/client/__init__.py
--rw-r--r--   0        0        0    17706 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/client/async_client.py
--rw-r--r--   0        0        0     5329 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/client/base.py
--rw-r--r--   0        0        0    19566 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/client/sync_client.py
--rw-r--r--   0        0        0    24547 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/helpers.py
--rw-r--r--   0        0        0     2575 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/life_span_handler.py
--rw-r--r--   0        0        0    21752 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/request_factory.py
--rw-r--r--   0        0        0     8112 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/transport.py
--rw-r--r--   0        0        0     6931 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4169 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/__init__.py
--rw-r--r--   0        0        0     7539 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/asgi_types.py
--rw-r--r--   0        0        0      724 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/builtin_types.py
--rw-r--r--   0        0        0     2287 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/callable_types.py
--rw-r--r--   0        0        0     1682 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/composite_types.py
--rw-r--r--   0        0        0      113 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/empty.py
--rw-r--r--   0        0        0     2614 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/file_types.py
--rw-r--r--   0        0        0      344 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/helper_types.py
--rw-r--r--   0        0        0     1325 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/internal_types.py
--rw-r--r--   0        0        0     2344 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/types/protocols.py
--rw-r--r--   0        0        0     1623 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/__init__.py
--rw-r--r--   0        0        0     1797 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/compat.py
--rw-r--r--   0        0        0      917 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/dataclass.py
--rw-r--r--   0        0        0     3459 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/deprecation.py
--rw-r--r--   0        0        0     1408 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/helpers.py
--rw-r--r--   0        0        0      678 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/path.py
--rw-r--r--   0        0        0     6551 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/predicates.py
--rw-r--r--   0        0        0     1799 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/pydantic.py
--rw-r--r--   0        0        0     2242 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/scope.py
--rw-r--r--   0        0        0      728 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/sequence.py
--rw-r--r--   0        0        0     4133 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/sync.py
--rw-r--r--   0        0        0     1722 2023-03-04 16:58:58.403703 starlite-2.0.0a1/starlite/utils/types.py
--rw-r--r--   0        0        0    48517 1970-01-01 00:00:00.000000 starlite-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-25 14:33:49.902721 starlite-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0    46584 2023-03-25 14:33:49.906720 starlite-2.0.0a2/README.md
+-rw-r--r--   0        0        0     8464 2023-03-25 14:33:49.926721 starlite-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      739 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/__init__.py
+-rw-r--r--   0        0        0      103 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/__main__.py
+-rw-r--r--   0        0        0       77 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/__init__.py
+-rw-r--r--   0        0        0     8644 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4245 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    13507 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/extractors.py
+-rw-r--r--   0        0        0    19414 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2760 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_layers/utils.py
+-rw-r--r--   0        0        0     5935 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_multipart.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/__init__.py
+-rw-r--r--   0        0        0    10156 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/parameters.py
+-rw-r--r--   0        0        0     5490 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/path_item.py
+-rw-r--r--   0        0        0     1238 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/request_body.py
+-rw-r--r--   0        0        0    10001 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     8066 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     1756 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    28012 2023-03-25 14:33:49.926721 starlite-2.0.0a2/starlite/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5242 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1483 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_openapi/utils.py
+-rw-r--r--   0        0        0     2465 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_parsers.py
+-rw-r--r--   0        0        0      197 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_signature/__init__.py
+-rw-r--r--   0        0        0    11806 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_signature/models.py
+-rw-r--r--   0        0        0    11295 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_signature/parsing.py
+-rw-r--r--   0        0        0     2513 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/_signature/utils.py
+-rw-r--r--   0        0        0    36956 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/app.py
+-rw-r--r--   0        0        0     2200 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/background_tasks.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/__init__.py
+-rw-r--r--   0        0        0    11820 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4553 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/commands/core.py
+-rw-r--r--   0        0        0     2365 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/commands/schema.py
+-rw-r--r--   0        0        0     2224 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/commands/sessions.py
+-rw-r--r--   0        0        0      807 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11665 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/app.py
+-rw-r--r--   0        0        0     2742 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/csrf.py
+-rw-r--r--   0        0        0     1733 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/connection/__init__.py
+-rw-r--r--   0        0        0    10838 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/connection/base.py
+-rw-r--r--   0        0        0     7034 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/connection/request.py
+-rw-r--r--   0        0        0     9005 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/connection/websocket.py
+-rw-r--r--   0        0        0      797 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/constants.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/htmx/request.py
+-rw-r--r--   0        0        0     8349 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2549 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28720 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     3978 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3910 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/mako.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/msgspec/__init__.py
+-rw-r--r--   0        0        0      180 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4237 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2243 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4065 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/piccolo_orm.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0      280 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/__init__.py
+-rw-r--r--   0        0        0     9079 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/abc.py
+-rw-r--r--   0        0        0      328 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     1162 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/filters.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    12484 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3460 2023-03-25 14:33:49.930721 starlite-2.0.0a2/starlite/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0    19789 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy/repository.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/__init__.py
+-rw-r--r--   0        0        0    13787 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/config.py
+-rw-r--r--   0        0        0    19414 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/plugin.py
+-rw-r--r--   0        0        0     1319 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/types.py
+-rw-r--r--   0        0        0     6060 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/contrib/tortoise_orm.py
+-rw-r--r--   0        0        0     8888 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/controller.py
+-rw-r--r--   0        0        0    16462 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/data_extractors.py
+-rw-r--r--   0        0        0      857 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/cookie.py
+-rw-r--r--   0        0        0    12896 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/response_header.py
+-rw-r--r--   0        0        0     9302 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/state.py
+-rw-r--r--   0        0        0     3360 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/datastructures/url.py
+-rw-r--r--   0        0        0     2386 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/di.py
+-rw-r--r--   0        0        0    13204 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/dto.py
+-rw-r--r--   0        0        0     1728 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/enums.py
+-rw-r--r--   0        0        0      201 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/events/__init__.py
+-rw-r--r--   0        0        0     4597 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/events/listener.py
+-rw-r--r--   0        0        0     1142 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/exceptions/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1246 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5350 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/file_system.py
+-rw-r--r--   0        0        0      469 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/__init__.py
+-rw-r--r--   0        0        0     4155 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    11854 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     9851 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    25935 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    57739 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0     4022 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/handlers/websocket_handlers.py
+-rw-r--r--   0        0        0      147 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/logging/_utils.py
+-rw-r--r--   0        0        0    12111 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/logging/config.py
+-rw-r--r--   0        0        0     1116 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/_utils.py
+-rw-r--r--   0        0        0     2973 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3436 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/authentication.py
+-rw-r--r--   0        0        0     5302 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/base.py
+-rw-r--r--   0        0        0     8343 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/compression.py
+-rw-r--r--   0        0        0     2573 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/cors.py
+-rw-r--r--   0        0        0     6474 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7191 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9006 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13393 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/logging.py
+-rw-r--r--   0        0        0    10821 2023-03-25 14:33:49.934721 starlite-2.0.0a2/starlite/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7961 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/middleware/session/base.py
+-rw-r--r--   0        0        0    10326 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8575 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/middleware/session/server_side.py
+-rw-r--r--   0        0        0      231 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/config.py
+-rw-r--r--   0        0        0    17275 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1648 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/openapi/spec/xml.py
+-rw-r--r--   0        0        0    10984 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/pagination.py
+-rw-r--r--   0        0        0    16805 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/params.py
+-rw-r--r--   0        0        0     6337 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/partial.py
+-rw-r--r--   0        0        0     7532 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/plugins.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/py.typed
+-rw-r--r--   0        0        0      278 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/__init__.py
+-rw-r--r--   0        0        0    12185 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/base.py
+-rw-r--r--   0        0        0     8954 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/file.py
+-rw-r--r--   0        0        0     2422 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/redirect.py
+-rw-r--r--   0        0        0     4893 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/streaming.py
+-rw-r--r--   0        0        0     2994 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response/template.py
+-rw-r--r--   0        0        0    14978 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/response_containers.py
+-rw-r--r--   0        0        0    14127 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/router.py
+-rw-r--r--   0        0        0      191 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/routes/__init__.py
+-rw-r--r--   0        0        0     1763 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/routes/asgi.py
+-rw-r--r--   0        0        0     6310 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/routes/base.py
+-rw-r--r--   0        0        0    13395 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/routes/http.py
+-rw-r--r--   0        0        0     3058 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/security/base.py
+-rw-r--r--   0        0        0      188 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4941 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     6606 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/serialization.py
+-rw-r--r--   0        0        0      158 2023-03-25 14:33:49.938721 starlite-2.0.0a2/starlite/static_files/__init__.py
+-rw-r--r--   0        0        0     5019 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/static_files/base.py
+-rw-r--r--   0        0        0     3582 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/static_files/config.py
+-rw-r--r--   0        0        0     7775 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/status_codes.py
+-rw-r--r--   0        0        0        0 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/__init__.py
+-rw-r--r--   0        0        0     4377 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/template/__init__.py
+-rw-r--r--   0        0        0     4113 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/template/base.py
+-rw-r--r--   0        0        0     1894 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/template/config.py
+-rw-r--r--   0        0        0      581 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/client/__init__.py
+-rw-r--r--   0        0        0    17706 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/client/async_client.py
+-rw-r--r--   0        0        0     5360 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/client/base.py
+-rw-r--r--   0        0        0    19556 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/client/sync_client.py
+-rw-r--r--   0        0        0    24254 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/helpers.py
+-rw-r--r--   0        0        0     2534 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21819 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/request_factory.py
+-rw-r--r--   0        0        0     8094 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/transport.py
+-rw-r--r--   0        0        0     6943 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4027 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/__init__.py
+-rw-r--r--   0        0        0     8634 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/asgi_types.py
+-rw-r--r--   0        0        0      514 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/builtin_types.py
+-rw-r--r--   0        0        0     2291 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/callable_types.py
+-rw-r--r--   0        0        0     1645 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/empty.py
+-rw-r--r--   0        0        0     2662 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/helper_types.py
+-rw-r--r--   0        0        0     1496 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/internal_types.py
+-rw-r--r--   0        0        0     2407 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/types/protocols.py
+-rw-r--r--   0        0        0     1675 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/compat.py
+-rw-r--r--   0        0        0      969 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/deprecation.py
+-rw-r--r--   0        0        0     1483 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/path.py
+-rw-r--r--   0        0        0     7714 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/predicates.py
+-rw-r--r--   0        0        0     1996 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/pydantic.py
+-rw-r--r--   0        0        0     2340 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/scope.py
+-rw-r--r--   0        0        0      765 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/sequence.py
+-rw-r--r--   0        0        0     4251 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/sync.py
+-rw-r--r--   0        0        0     1796 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/types.py
+-rw-r--r--   0        0        0     1921 2023-03-25 14:33:49.942721 starlite-2.0.0a2/starlite/utils/version.py
+-rw-r--r--   0        0        0    49696 1970-01-01 00:00:00.000000 starlite-2.0.0a2/PKG-INFO
```

### Comparing `starlite-2.0.0a1/LICENSE` & `starlite-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/README.md` & `starlite-2.0.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-85-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-89-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/starlite?label=r%2FStarlite&logo=reddit)](https://reddit.com/r/starlite)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#starlitespace:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://itnext.io/introducing-starlite-3928adaa19ae)
@@ -41,14 +41,21 @@
 
 ## Installation
 
 ```shell
 pip install starlite
 ```
 
+**Starlite 2.0 is coming out soon**, bringing many new features and improvements.
+You can check out the alpha version by instead running
+
+```shell
+pip install starlite==2.0.0alpha1
+```
+
 ## Quick Start
 
 ```python
 from starlite import Starlite, get
 
 
 @get("/")
@@ -165,17 +172,14 @@
     @delete(path="/{user_id:uuid}")
     async def delete_user(self, user_id: UUID4) -> None:
         ...
 ```
 
 ### Data Parsing, Type Hints and Pydantic
 
-One key difference between Starlite and Starlette/FastAPI is in parsing of form data and query parameters- Starlite
-supports mixed form data and has faster and better query parameter parsing.
-
 Starlite is rigorously typed, and it enforces typing. For example, if you forget to type a return value for a route
 handler, an exception will be raised. The reason for this is that Starlite uses typing data to generate OpenAPI specs,
 as well as to validate and parse data. Thus typing is absolutely essential to the framework.
 
 Furthermore, Starlite allows extending its support using plugins.
 
 ### Plugin System, ORM support and DTOs
@@ -186,17 +190,16 @@
 handlers.
 
 Starlite also supports the programmatic creation of DTOs with a `DTOFactory` class, which also supports the use of
 plugins.
 
 ### OpenAPI
 
-Starlite has custom logic to generate OpenAPI 3.1.0 schema, the latest version. The schema generated by Starlite is
-significantly more complete and more correct than those generated by FastAPI, and they include optional generation of
-examples using the `pydantic-factories` library.
+Starlite has custom logic to generate OpenAPI 3.1.0 schema, include optional generation of examples using the
+`pydantic-factories` library.
 
 #### ReDoc, Swagger-UI and Stoplight Elements API Documentation
 
 Starlite serves the documentation from the generated OpenAPI schema with:
 
 - [ReDoc](https://redoc.ly/)
 - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
@@ -361,15 +364,15 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ottermata"><img src="https://avatars.githubusercontent.com/u/9451844?v=4?s=100" width="100px;" alt="Christopher Krause"/><br /><sub><b>Christopher Krause</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ottermata" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/starlite-api/starlite/commits?author=smithk86" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/starlite-api/starlite/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ste-pool" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/starlite-api/starlite/commits?author=Alc-Alc" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://asomethings.com"><img src="https://avatars.githubusercontent.com/u/16171942?v=4?s=100" width="100px;" alt="asomethings"/><br /><sub><b>asomethings</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=asomethings" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/garburator"><img src="https://avatars.githubusercontent.com/u/14207857?v=4?s=100" width="100px;" alt="Garry Bullock"/><br /><sub><b>Garry Bullock</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=garburator" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NiclasHaderer"><img src="https://avatars.githubusercontent.com/u/109728711?v=4?s=100" width="100px;" alt="Niclas Haderer"/><br /><sub><b>Niclas Haderer</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=NiclasHaderer" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dialvarezs"><img src="https://avatars.githubusercontent.com/u/13831919?v=4?s=100" width="100px;" alt="Diego Alvarez"/><br /><sub><b>Diego Alvarez</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=dialvarezs" title="Documentation">📖</a> <a href="https://github.com/starlite-api/starlite/commits?author=dialvarezs" title="Code">💻</a></td>
@@ -392,14 +395,18 @@
       <td align="center" valign="top" width="14.28%"><a href="http://wardpearce.com"><img src="https://avatars.githubusercontent.com/u/27844174?v=4?s=100" width="100px;" alt="Ward"/><br /><sub><b>Ward</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3AWardPearce" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://knowsuchagency.com"><img src="https://avatars.githubusercontent.com/u/11974795?v=4?s=100" width="100px;" alt="Stephan Fitzpatrick"/><br /><sub><b>Stephan Fitzpatrick</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Aknowsuchagency" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://codepen.io/ekeric13/"><img src="https://avatars.githubusercontent.com/u/6489651?v=4?s=100" width="100px;" alt="Eric Kennedy"/><br /><sub><b>Eric Kennedy</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ekeric13" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wassafshahzad"><img src="https://avatars.githubusercontent.com/u/25094157?v=4?s=100" width="100px;" alt="wassaf shahzad"/><br /><sub><b>wassaf shahzad</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=wassafshahzad" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://nilsso.github.io"><img src="https://avatars.githubusercontent.com/u/567181?v=4?s=100" width="100px;" alt="Nils Olsson"/><br /><sub><b>Nils Olsson</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=nilsso" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://rileychase.net"><img src="https://avatars.githubusercontent.com/u/1491530?v=4?s=100" width="100px;" alt="Riley Chase"/><br /><sub><b>Riley Chase</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Nadock" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://gh.arielle.codes"><img src="https://avatars.githubusercontent.com/u/71233171?v=4?s=100" width="100px;" alt="arl"/><br /><sub><b>arl</b></sub></a><br /><a href="#maintenance-onerandomusername" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Galdanwing" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=zoni" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `starlite-2.0.0a1/starlite/app.py` & `starlite-2.0.0a2/starlite/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 from __future__ import annotations
 
 from datetime import date, datetime, time, timedelta
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
-from pydantic_openapi_schema import construct_open_api_with_schema_class
 from typing_extensions import Self, TypedDict
 
-from starlite.asgi import ASGIRouter
-from starlite.asgi.utils import get_route_handlers, wrap_in_exception_handler
+from starlite._asgi import ASGIRouter
+from starlite._asgi.utils import get_route_handlers, wrap_in_exception_handler
+from starlite._openapi.path_item import create_path_item
+from starlite._signature import create_signature_model
 from starlite.config.allowed_hosts import AllowedHostsConfig
 from starlite.config.app import AppConfig
-from starlite.config.cache import CacheConfig
-from starlite.config.logging import LoggingConfig, get_logger_placeholder
-from starlite.config.openapi import OpenAPIConfig
+from starlite.config.response_cache import ResponseCacheConfig
 from starlite.connection import Request, WebSocket
 from starlite.datastructures.state import State
 from starlite.events.emitter import BaseEventEmitterBackend, SimpleEventEmitter
 from starlite.exceptions import (
     ImproperlyConfiguredException,
     NoRouteMatchFoundException,
 )
 from starlite.handlers.http_handlers import HTTPRouteHandler
+from starlite.logging.config import LoggingConfig, get_logger_placeholder
 from starlite.middleware.cors import CORSMiddleware
-from starlite.openapi.path_item import create_path_item
-from starlite.plugins.base import (
+from starlite.openapi.config import OpenAPIConfig
+from starlite.openapi.spec.components import Components
+from starlite.plugins import (
     InitPluginProtocol,
     OpenAPISchemaPluginProtocol,
     SerializationPluginProtocol,
 )
 from starlite.router import Router
 from starlite.routes import ASGIRoute, HTTPRoute, WebSocketRoute
-from starlite.signature import create_signature_model
 from starlite.static_files.base import StaticFiles
+from starlite.stores.registry import StoreRegistry
 from starlite.types import Empty
 from starlite.types.internal_types import PathParameterDefinition
 from starlite.utils import (
     as_async_callable_list,
     async_partial,
     is_async_callable,
     join_paths,
     unique,
 )
 from starlite.utils.dataclass import extract_dataclass_fields
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
-    from pydantic_openapi_schema.v3_1_0.open_api import OpenAPI
+__all__ = ("HandlerIndex", "Starlite")
+
 
+if TYPE_CHECKING:
     from starlite.config.compression import CompressionConfig
     from starlite.config.cors import CORSConfig
     from starlite.config.csrf import CSRFConfig
-    from starlite.config.logging import BaseLoggingConfig
-    from starlite.config.static_files import StaticFilesConfig
-    from starlite.config.template import TemplateConfig
     from starlite.datastructures import CacheControlHeader, ETag, ResponseHeader
     from starlite.events.listener import EventListener
-    from starlite.handlers.base import BaseRouteHandler  # noqa: TC004
+    from starlite.handlers.base import BaseRouteHandler
+    from starlite.logging.config import BaseLoggingConfig
+    from starlite.openapi.spec import SecurityRequirement
+    from starlite.openapi.spec.open_api import OpenAPI
     from starlite.plugins import PluginProtocol
-    from starlite.types import (  # noqa: TC004
+    from starlite.static_files.config import StaticFilesConfig
+    from starlite.stores.base import Store
+    from starlite.template.config import TemplateConfig
+    from starlite.types import (
         AfterExceptionHookHandler,
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         AnyCallable,
         ASGIApp,
         BeforeMessageSendHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
         Dependencies,
         EmptyType,
         ExceptionHandlersMap,
         GetLogger,
         Guard,
-        InitialStateType,
         LifeSpanHandler,
         LifeSpanHookHandler,
         LifeSpanReceive,
         LifeSpanScope,
         LifeSpanSend,
         Logger,
         Message,
@@ -91,20 +94,16 @@
         RouteHandlerType,
         Scope,
         Send,
         TypeEncodersMap,
     )
 
 DEFAULT_OPENAPI_CONFIG = OpenAPIConfig(title="Starlite API", version="1.0.0")
-"""The default OpenAPI config used if not configuration is explicitly passed to the :class:`Starlite
-<starlite.app.Starlite>` instance constructor.
-"""
-DEFAULT_CACHE_CONFIG = CacheConfig()
-"""The default cache config used if not configuration is explicitly passed to the :class:`Starlite
-<starlite.app.Starlite>` instance constructor.
+"""The default OpenAPI config used if not configuration is explicitly passed to the
+:class:`Starlite <.app.Starlite>` instance constructor.
 """
 
 
 class HandlerIndex(TypedDict):
     """Map route handler names to a mapping of paths + route handler.
 
     It's returned from the 'get_handler_index_by_name' utility method.
@@ -113,57 +112,57 @@
     paths: list[str]
     """Full route paths to the route handler."""
     handler: RouteHandlerType
     """Route handler instance."""
     identifier: str
     """Unique identifier of the handler.
 
-    Either equal to the 'name' attribute or the ``__str__`` value of the handler.
+    Either equal to :attr`__name__ <obj.__name__>` attribute or ``__str__`` value of the handler.
     """
 
 
 class Starlite(Router):
     """The Starlite application.
 
-    ``Starlite`` is the root level of the app - it has the base path of "/" and all root level
-    Controllers, Routers and Route Handlers should be registered on it.
-
-    Inherits from the :class:`Router <starlite.router.Router>` class
+    ``Starlite`` is the root level of the app - it has the base path of ``/`` and all root level Controllers, Routers
+    and Route Handlers should be registered on it.
     """
 
     __slots__ = (
         "_openapi_schema",
         "after_exception",
         "after_shutdown",
         "after_startup",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
         "before_shutdown",
         "before_startup",
-        "cache",
         "compression_config",
         "cors_config",
         "csrf_config",
         "debug",
         "event_emitter",
         "get_logger",
         "logger",
         "logging_config",
         "multipart_form_part_limit",
+        "signature_namespace",
         "on_shutdown",
         "on_startup",
         "openapi_config",
+        "openapi_schema_plugins",
         "request_class",
+        "response_cache_config",
         "route_map",
         "serialization_plugins",
-        "openapi_schema_plugins",
         "state",
         "static_files_config",
+        "stores",
         "template_engine",
         "websocket_class",
     )
 
     def __init__(
         self,
         route_handlers: OptionalSequence[ControllerRouterHandler] = None,
@@ -173,26 +172,25 @@
         after_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
         after_startup: OptionalSequence[LifeSpanHookHandler] = None,
         allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
         before_request: BeforeRequestHookHandler | None = None,
         before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
         before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
         before_startup: OptionalSequence[LifeSpanHookHandler] = None,
-        cache_config: CacheConfig = DEFAULT_CACHE_CONFIG,
+        response_cache_config: ResponseCacheConfig | None = None,
         cache_control: CacheControlHeader | None = None,
         compression_config: CompressionConfig | None = None,
         cors_config: CORSConfig | None = None,
         csrf_config: CSRFConfig | None = None,
         debug: bool = False,
         dependencies: Dependencies | None = None,
         etag: ETag | None = None,
         event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: OptionalSequence[Guard] = None,
-        initial_state: InitialStateType | None = None,
         listeners: OptionalSequence[EventListener] = None,
         logging_config: BaseLoggingConfig | EmptyType | None = Empty,
         middleware: OptionalSequence[Middleware] = None,
         multipart_form_part_limit: int = 1000,
         on_app_init: OptionalSequence[OnAppInitHandler] = None,
         on_shutdown: OptionalSequence[LifeSpanHandler] = None,
         on_startup: OptionalSequence[LifeSpanHandler] = None,
@@ -201,100 +199,109 @@
         parameters: ParametersMap | None = None,
         plugins: OptionalSequence[PluginProtocol] = None,
         request_class: type[Request] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: OptionalSequence[ResponseHeader] = None,
         security: OptionalSequence[SecurityRequirement] = None,
+        signature_namespace: Mapping[str, Any] | None = None,
+        state: State | None = None,
         static_files_config: OptionalSequence[StaticFilesConfig] = None,
+        stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
         type_encoders: TypeEncodersMap | None = None,
         websocket_class: type[WebSocket] | None = None,
     ) -> None:
         """Initialize a ``Starlite`` application.
 
         Args:
-            after_exception: A sequence of :class:`exception hook handlers <starlite.types.AfterExceptionHookHandler>`.
-                This hook is called after an exception occurs. In difference to exception handlers, it is not meant to
+            after_exception: A sequence of :class:`exception hook handlers <.types.AfterExceptionHookHandler>`. This
+                hook is called after an exception occurs. In difference to exception handlers, it is not meant to
                 return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
             after_request: A sync or async function executed after the route handler function returned and the response
                 object has been resolved. Receives the response object.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            after_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-                This hook is called during the ASGI shutdown, after all callables in the 'on_shutdown' list have been
-                called.
-            after_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-                This hook is called during the ASGI startup, after all callables in the 'on_startup' list have been
-                called.
-            allowed_hosts: A sequence of allowed hosts, or an :class:`allowed hosts config <starlite.config.AllowedHostsConfig>`
-                instance. Enables the builtin allowed hosts middleware.
-            before_request: A sync or async function called immediately before calling the route handler.
-                Receives the :class:`Request <starlite.connection.Request>` instance and any non-``None`` return value is
-                used for the response, bypassing the route handler.
-            before_send: A sequence of :class:`before send hook handlers <starlite.types.BeforeMessageSendHookHandler>`.
-                This hook is called when the ASGI send function is called.
-            before_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-                This hook is called during the ASGI shutdown, before any 'on_shutdown' hooks are called.
-            before_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-                This hook is called during the ASGI startup, before any 'on_startup' hooks are called.
-            cache_config: Configures caching behavior of the application.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            after_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
+                the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
+            after_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
+                the ASGI startup, after all callables in the 'on_startup' list have been called.
+            allowed_hosts: A sequence of allowed hosts, or an
+                :class:`AllowedHostsConfig <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin
+                allowed hosts middleware.
+            before_request: A sync or async function called immediately before calling the route handler. Receives the
+                :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
+                response, bypassing the route handler.
+            before_send: A sequence of :class:`before send hook handlers <.types.BeforeMessageSendHookHandler>`. Called
+                when the ASGI send function is called.
+            before_shutdown: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
+                the ASGI shutdown, before any 'on_shutdown' hooks are called.
+            before_startup: A sequence of :class:`life-span hook handlers <.types.LifeSpanHookHandler>`. Called during
+                the ASGI startup, before any 'on_startup' hooks are called.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` to add to route handlers of this app.
-                Can be overridden by route handlers.
+                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` to add to route handlers of
+                this app. Can be overridden by route handlers.
             compression_config: Configures compression behaviour of the application, this enabled a builtin or user
                 defined Compression middleware.
-            cors_config: If set this enables the builtin CORS middleware.
-            csrf_config: If set this enables the builtin CSRF middleware.
+            cors_config: If set, configures :class:`CORSMiddleware <.middleware.cors.CORSMiddleware>`.
+            csrf_config: If set, configures :class:`CSRFMiddleware <.middleware.csrf.CSRFMiddleware>`.
             debug: If ``True``, app errors rendered as HTML with a stack trace.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <datastructures.ETag>` to add to route handlers of this app.
+            dependencies: A string keyed mapping of dependency :class:`Providers <.di.Provide>`.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
                 Can be overridden by route handlers.
-            event_emitter_backend: A subclass of :class:`BaseEventEmitterBackend <starlite.events.emitter.BaseEventEmitterBackend>`.
+            event_emitter_backend: A subclass of
+                :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            initial_state: An object from which to initialize the app state.
-            listeners: A sequence of :class:`EventListener <starlite.events.listener.EventListener>`.
-            logging_config: A subclass of :class:`BaseLoggingConfig <starlite.config.logging.BaseLoggingConfig>`.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
-            multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request.
-                This limit is intended to protect from DoS attacks.
-            on_app_init: A sequence of :class:`OnAppInitHandler <starlite.types.OnAppInitHandler>` instances. Handlers
-                receive an instance of :class:`AppConfig <starlite.config.app.AppConfig>` that will have been initially
-                populated with the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an
-                instance of same. If more than one handler is registered they are called in the order they are provided.
-            on_shutdown: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
-                application shutdown.
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            listeners: A sequence of :class:`EventListener <.events.listener.EventListener>`.
+            logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
+            multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request. This limit
+                is intended to protect from DoS attacks.
+            on_app_init: A sequence of :class:`OnAppInitHandler <.types.OnAppInitHandler>` instances. Handlers receive
+                an instance of :class:`AppConfig <.config.app.AppConfig>` that will have been initially populated with
+                the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an instance of same.
+                If more than one handler is registered they are called in the order they are provided.
+            on_shutdown: A sequence of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application
+                shutdown.
             on_startup: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
                 application startup.
             openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>`
-                or wherever you have access to :class:`Request <starlite.connection.request.Request>` or
-                :class:`ASGI Scope <starlite.types.Scope>`.
-            parameters: A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all
-                application paths.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <starlite.connection.request.Request>` or
+                :class:`ASGI Scope <.types.Scope>`.
+            parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
+                paths.
             plugins: Sequence of plugins.
-            request_class: An optional subclass of :class:`Request <starlite.connection.request.Request>` to use for
-                http connections.
-            response_class: A custom subclass of [starlite.response.Response] to be used as the app's default response.
-            response_cookies: A sequence of [Cookie](starlite.datastructures.Cookie] instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
-                instances.
+            request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
+                response.
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
+            response_cache_config: Configures caching behavior of the application.
             route_handlers: A sequence of route handlers, which can include instances of
-                :class:`Router <starlite.router.Router>`, subclasses of :class:`Controller <starlite.controller.Controller>` or
-                any function decorated by the route handler decorators.
+                :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
+                callable decorated by the route handler decorators.
             security: A sequence of dicts that will be added to the schema of all route handlers in the application.
-                See :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` for details.
-            static_files_config: A sequence of :class:`StaticFilesConfig <starlite.config.StaticFilesConfig>`
-            tags: A sequence of string tags that will be appended to the schema of all route handlers under the application.
-            template_config: An instance of :class:`TemplateConfig <starlite.config.TemplateConfig>`
+                See
+                :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for details.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+            state: An optional :class:`State <.datastructures.State>` for application state.
+            static_files_config: A sequence of :class:`StaticFilesConfig <.static_files.StaticFilesConfig>`
+            stores: Central registry of :class:`Store <.stores.base.Store>` that will be available throughout the
+                application. If this is a dictionary to it will be passed to a
+                :class:`StoreRegistry <.stores.registry.StoreRegistry>`. If it is a
+                :class:`StoreRegistry <.stores.registry.StoreRegistry>`, this instance will be used directly.
+            tags: A sequence of string tags that will be appended to the schema of all route handlers under the
+                application.
+            template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-            websocket_class: An optional subclass of :class:`WebSocket <starlite.connection.websocket.WebSocket>` to use for
-                websocket connections.
+            websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket
+                connections.
         """
         self._openapi_schema: OpenAPI | None = None
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.asgi_router = ASGIRouter(app=self)
 
@@ -308,26 +315,25 @@
             after_shutdown=list(after_shutdown or []),
             after_startup=list(after_startup or []),
             allowed_hosts=allowed_hosts if isinstance(allowed_hosts, AllowedHostsConfig) else list(allowed_hosts or []),
             before_request=before_request,
             before_send=list(before_send or []),
             before_shutdown=list(before_shutdown or []),
             before_startup=list(before_startup or []),
-            cache_config=cache_config,
+            response_cache_config=response_cache_config or ResponseCacheConfig(),
             cache_control=cache_control,
             compression_config=compression_config,
             cors_config=cors_config,
             csrf_config=csrf_config,
             debug=debug,
             dependencies=dict(dependencies or {}),
             etag=etag,
             event_emitter_backend=event_emitter_backend,
             exception_handlers=exception_handlers or {},
             guards=list(guards or []),
-            initial_state=dict(initial_state or {}),
             listeners=list(listeners or []),
             logging_config=cast("BaseLoggingConfig | None", logging_config),
             middleware=list(middleware or []),
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
@@ -336,15 +342,18 @@
             plugins=list(plugins or []),
             request_class=request_class,
             response_class=response_class,
             response_cookies=response_cookies or [],
             response_headers=response_headers or [],
             route_handlers=list(route_handlers) if route_handlers is not None else [],
             security=list(security or []),
+            signature_namespace=dict(signature_namespace or {}),
+            state=state or State(),
             static_files_config=list(static_files_config or []),
+            stores=stores,
             tags=list(tags or []),
             template_config=template_config,
             type_encoders=type_encoders,
             websocket_class=websocket_class,
         )
         for handler in on_app_init or []:
             config = handler(config)
@@ -352,27 +361,27 @@
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.after_exception = as_async_callable_list(config.after_exception)
         self.after_shutdown = as_async_callable_list(config.after_shutdown)
         self.after_startup = as_async_callable_list(config.after_startup)
         self.before_send = as_async_callable_list(config.before_send)
         self.before_shutdown = as_async_callable_list(config.before_shutdown)
         self.before_startup = as_async_callable_list(config.before_startup)
-        self.cache = config.cache_config.to_cache()
+        self.response_cache_config = config.response_cache_config
         self.compression_config = config.compression_config
         self.cors_config = config.cors_config
         self.csrf_config = config.csrf_config
         self.debug = config.debug
         self.logging_config = config.logging_config
         self.on_shutdown = config.on_shutdown
         self.on_startup = config.on_startup
         self.openapi_config = config.openapi_config
         self.serialization_plugins = [p for p in config.plugins if isinstance(p, SerializationPluginProtocol)]
         self.openapi_schema_plugins = [p for p in config.plugins if isinstance(p, OpenAPISchemaPluginProtocol)]
         self.request_class = config.request_class or Request
-        self.state = State(config.initial_state, deep_copy=True)
+        self.state = config.state
         self.static_files_config = config.static_files_config
         self.template_engine = config.template_config.engine_instance if config.template_config else None
         self.websocket_class = config.websocket_class or WebSocket
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.multipart_form_part_limit = config.multipart_form_part_limit
 
         super().__init__(
@@ -390,14 +399,15 @@
             path="",
             response_class=config.response_class,
             response_cookies=config.response_cookies,
             response_headers=config.response_headers,
             # route handlers are registered below
             route_handlers=[],
             security=config.security,
+            signature_namespace=config.signature_namespace,
             tags=config.tags,
             type_encoders=config.type_encoders,
         )
 
         for plugin in (p for p in config.plugins if isinstance(p, InitPluginProtocol)):
             plugin.on_app_init(app=self)
 
@@ -415,14 +425,16 @@
             self.register(self.openapi_config.openapi_controller)
 
         for static_config in self.static_files_config:
             self.register(static_config.to_static_files_app())
 
         self.asgi_handler = self._create_asgi_handler()
 
+        self.stores = config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
+
     async def __call__(
         self,
         scope: Scope | LifeSpanScope,
         receive: Receive | LifeSpanReceive,
         send: Send | LifeSpanSend,
     ) -> None:
         """Application entry point.
@@ -444,42 +456,47 @@
         scope["state"] = {}
         await self.asgi_handler(scope, receive, self._wrap_send(send=send, scope=scope))  # type: ignore[arg-type]
 
     @property
     def openapi_schema(self) -> OpenAPI | None:
         """Access  the OpenAPI schema of the application.
 
-        :return: The :class:`OpenAPI` <pydantic_openapi_schema.open_api.OpenAPI> instance of the application's.
+        Returns:
+            The :class:`OpenAPI`
+            <pydantic_openapi_schema.open_api.OpenAPI> instance of the
+            application's.
         """
         if self.openapi_config and not self._openapi_schema:
             self._openapi_schema = self.openapi_config.to_openapi_schema()
             self.update_openapi_schema()
         return self._openapi_schema
 
     @classmethod
     def from_config(cls, config: AppConfig) -> Self:
         """Initialize a ``Starlite`` application from a configuration instance.
 
         Args:
-            config: An instance of :class:`AppConfig` <startlite.config.AppConfig>
+            config: An instance of :class:`AppConfig` <.config.AppConfig>
 
         Returns:
             An instance of ``Starlite`` application.
         """
         return cls(**dict(extract_dataclass_fields(config)))
 
     def register(self, value: ControllerRouterHandler) -> None:  # type: ignore[override]
         """Register a route handler on the app.
 
         This method can be used to dynamically add endpoints to an application.
 
-        :param value: An instance of :class:`Router <starlite.router.Router>`, a subclass of
-                :class:`Controller <starlite.controller.Controller>` or any function decorated by the route handler decorators.
+        Args:
+            value: An instance of :class:`Router <.router.Router>`, a subclass of
+                :class:`Controller <.controller.Controller>` or any function decorated by the route handler decorators.
 
-        :return: None
+        Returns:
+            None
         """
         routes = super().register(value=value)
 
         for route in routes:
             route_handlers = get_route_handlers(route)
 
             for route_handler in route_handlers:
@@ -488,15 +505,14 @@
                 route_handler.resolve_guards()
                 route_handler.resolve_middleware()
                 route_handler.resolve_opts()
 
                 if isinstance(route_handler, HTTPRouteHandler):
                     route_handler.resolve_before_request()
                     route_handler.resolve_after_response()
-                    route_handler.resolve_response_handler()
 
             if isinstance(route, HTTPRoute):
                 route.create_handler_map()
 
             elif isinstance(route, WebSocketRoute):
                 route.handler_parameter_model = route.create_handler_kwargs_model(route.route_handler)
 
@@ -510,31 +526,29 @@
         list of paths sorted lexically.
 
         Examples:
             .. code-block: python
 
                 from starlite import Starlite, get
 
-
                 @get("/", name="my-handler")
                 def handler() -> None:
                     pass
 
-
                 app = Starlite(route_handlers=[handler])
 
                 handler_index = app.get_handler_index_by_name("my-handler")
 
                 # { "paths": ["/"], "handler" ... }
 
         Args:
             name: A route handler unique name.
 
         Returns:
-            A :class:`HandlerIndex <starlite.app.HandlerIndex>` instance or None.
+            A :class:`HandlerIndex <.app.HandlerIndex>` instance or ``None``.
         """
         handler = self.asgi_router.route_handler_index.get(name)
         if not handler:
             return None
 
         identifier = handler.name or str(handler)
         routes = self.asgi_router.route_mapping[identifier]
@@ -547,20 +561,18 @@
         parameters.
 
         Examples:
             .. code-block: python
 
                 from starlite import Starlite, get
 
-
                 @get("/group/{group_id:int}/user/{user_id:int}", name="get_membership_details")
                 def get_membership_details(group_id: int, user_id: int) -> None:
                     pass
 
-
                 app = Starlite(route_handlers=[get_membership_details])
 
                 path = app.route_reverse("get_membership_details", user_id=100, group_id=10)
 
                 # /group/10/user/100
 
         Args:
@@ -627,15 +639,15 @@
                 # /static/css/main.css
 
         Args:
             name: A static handler unique name.
             file_path: a string containing path to an asset.
 
         Raises:
-            NoRouteMatchFoundException: If static files handler with 'name' does not exist.
+            NoRouteMatchFoundException: If static files handler with ``name`` does not exist.
 
         Returns:
             A url path to the asset.
         """
 
         handler_index = self.get_handler_index_by_name(name)
         if handler_index is None:
@@ -671,15 +683,15 @@
 
         return wrap_in_exception_handler(
             debug=self.debug, app=asgi_handler, exception_handlers=self.exception_handlers or {}
         )
 
     @staticmethod
     def _set_runtime_callables(route_handler: BaseRouteHandler) -> None:
-        """Optimize the 'route_handler.fn' and any 'provider.dependency' callables for runtime by doing the following:
+        """Optimize the ``route_handler.fn`` and any ``provider.dependency`` callables for runtime by doing the following:
 
         1. ensure that the ``self`` argument is preserved by binding it using partial.
         2. ensure sync functions are wrapped in AsyncCallable for sync_to_thread handlers.
 
         Args:
             route_handler: A route handler to process.
 
@@ -710,41 +722,41 @@
     def _create_handler_signature_model(self, route_handler: BaseRouteHandler) -> None:
         """Create function signature models for all route handler functions and provider dependencies."""
         if not route_handler.signature_model:
             route_handler.signature_model = create_signature_model(
                 fn=cast("AnyCallable", route_handler.fn.value),
                 plugins=self.serialization_plugins,
                 dependency_name_set=route_handler.dependency_name_set,
+                signature_namespace=route_handler.resolve_signature_namespace(),
             )
 
         for provider in route_handler.resolve_dependencies().values():
             if not getattr(provider, "signature_model", None):
                 provider.signature_model = create_signature_model(
                     fn=provider.dependency.value,
                     plugins=self.serialization_plugins,
                     dependency_name_set=route_handler.dependency_name_set,
+                    signature_namespace=route_handler.resolve_signature_namespace(),
                 )
 
     def _wrap_send(self, send: Send, scope: Scope) -> Send:
         """Wrap the ASGI send and handles any 'before send' hooks.
 
         Args:
             send: The ASGI send function.
+            scope: The ASGI scope.
 
         Returns:
             An ASGI send function.
         """
         if self.before_send:
 
             async def wrapped_send(message: "Message") -> None:
                 for hook in self.before_send:
-                    if hook.num_expected_args > 2:
-                        await hook(message, self.state, scope)
-                    else:
-                        await hook(message, self.state)
+                    await hook(message, self.state, scope)
                 await send(message)
 
             return wrapped_send
         return send
 
     def update_openapi_schema(self) -> None:
         """Update the OpenAPI schema to reflect the route handlers registered on the app.
@@ -753,43 +765,51 @@
             None
         """
         if not self.openapi_config or not self._openapi_schema or self._openapi_schema.paths is None:
             raise ImproperlyConfiguredException("Cannot generate OpenAPI schema without initializing an OpenAPIConfig")
 
         operation_ids: list[str] = []
 
+        if not self._openapi_schema.components:
+            self._openapi_schema.components = Components()
+            schemas = self._openapi_schema.components.schemas = {}
+        elif not self._openapi_schema.components.schemas:
+            schemas = self._openapi_schema.components.schemas = {}
+        else:
+            schemas = {}
+
         for route in self.routes:
             if (
                 isinstance(route, HTTPRoute)
                 and any(route_handler.include_in_schema for route_handler, _ in route.route_handler_map.values())
                 and (route.path_format or "/") not in self._openapi_schema.paths
             ):
                 path_item, created_operation_ids = create_path_item(
                     route=route,
                     create_examples=self.openapi_config.create_examples,
                     plugins=self.openapi_schema_plugins,
                     use_handler_docstrings=self.openapi_config.use_handler_docstrings,
                     operation_id_creator=self.openapi_config.operation_id_creator,
+                    schemas=schemas,
                 )
                 self._openapi_schema.paths[route.path_format or "/"] = path_item
 
                 for operation_id in created_operation_ids:
                     if operation_id in operation_ids:
                         raise ImproperlyConfiguredException(
                             f"operation_ids must be unique, "
                             f"please ensure the value of 'operation_id' is either not set or unique for {operation_id}"
                         )
                     operation_ids.append(operation_id)
 
-        self._openapi_schema = construct_open_api_with_schema_class(
-            open_api_schema=self._openapi_schema, by_alias=self.openapi_config.by_alias
-        )
-
-    async def emit(self, event_id: str, *args: Any, **kwargs: Any) -> None:
+    def emit(self, event_id: str, *args: Any, **kwargs: Any) -> None:
         """Emit an event to all attached listeners.
 
-        :param event_id: The ID of the event to emit, e.g 'my_event'.
-        :param args: args to pass to the listener(s).
-        :param kwargs: kwargs to pass to the listener(s)
-        :return: None
+        Args:
+            event_id: The ID of the event to emit, e.g ``my_event``.
+            args: args to pass to the listener(s).
+            kwargs: kwargs to pass to the listener(s)
+
+        Returns:
+            None
         """
-        await self.event_emitter.emit(event_id, *args, **kwargs)
+        self.event_emitter.emit(event_id, *args, **kwargs)
```

### Comparing `starlite-2.0.0a1/starlite/asgi/asgi_router.py` & `starlite-2.0.0a2/starlite/_asgi/asgi_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 import re
 from collections import defaultdict
 from functools import lru_cache
 from traceback import format_exc
 from typing import TYPE_CHECKING, Pattern
 
-from starlite.asgi.routing_trie import validate_node
-from starlite.asgi.routing_trie.mapping import add_route_to_trie
-from starlite.asgi.routing_trie.traversal import parse_path_to_route
-from starlite.asgi.routing_trie.types import create_node
-from starlite.asgi.utils import get_route_handlers
+from starlite._asgi.routing_trie import validate_node
+from starlite._asgi.routing_trie.mapping import add_route_to_trie
+from starlite._asgi.routing_trie.traversal import parse_path_to_route
+from starlite._asgi.routing_trie.types import create_node
+from starlite._asgi.utils import get_route_handlers
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.utils import AsyncCallable, normalize_path
 
+__all__ = ("ASGIRouter",)
+
+
 if TYPE_CHECKING:
+    from starlite._asgi.routing_trie.types import RouteTrieNode
     from starlite.app import Starlite
-    from starlite.asgi.routing_trie.types import RouteTrieNode
     from starlite.routes import ASGIRoute, HTTPRoute, WebSocketRoute
     from starlite.routes.base import BaseRoute
     from starlite.types import (
         ASGIApp,
         LifeSpanHandler,
         LifeSpanReceive,
         LifeSpanSend,
@@ -198,14 +201,16 @@
     async def startup(self) -> None:
         """Run any :class:`LifeSpanHandlers <starlite.types.LifeSpanHandler>` defined in the application's
         ``.on_startup`` list.
 
         Calls the ``before_startup`` hook and ``after_startup`` hook handlers respectively before and after calling in
         the lifespan handlers.
         """
+        await self.app.event_emitter.on_startup()
+
         for hook in self.app.before_startup:
             await hook(self.app)
 
         for handler in self.app.on_startup:
             await self._call_lifespan_handler(handler)
 
         for hook in self.app.after_startup:
@@ -214,14 +219,16 @@
     async def shutdown(self) -> None:
         """Run any :class:`LifeSpanHandlers <starlite.types.LifeSpanHandler>` defined in the application's
         ``.on_shutdown`` list.
 
         Calls the ``before_shutdown`` hook and ``after_shutdown`` hook handlers respectively before and after calling in
         the lifespan handlers.
         """
+        await self.app.event_emitter.on_shutdown()
+
         for hook in self.app.before_shutdown:
             await hook(self.app)
 
         for handler in self.app.on_shutdown:
             await self._call_lifespan_handler(handler)
 
         for hook in self.app.after_shutdown:
```

### Comparing `starlite-2.0.0a1/starlite/asgi/routing_trie/mapping.py` & `starlite-2.0.0a2/starlite/_asgi/routing_trie/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, cast
 
-from starlite.asgi.routing_trie.types import (
+from starlite._asgi.routing_trie.types import (
     ASGIHandlerTuple,
     PathParameterSentinel,
     create_node,
 )
-from starlite.asgi.utils import wrap_in_exception_handler
+from starlite._asgi.utils import wrap_in_exception_handler
 from starlite.types.internal_types import PathParameterDefinition
 
+__all__ = ("add_mount_route", "add_route_to_trie", "build_route_middleware_stack", "configure_node")
+
+
 if TYPE_CHECKING:
+    from starlite._asgi.routing_trie.types import RouteTrieNode
     from starlite.app import Starlite
-    from starlite.asgi.routing_trie.types import RouteTrieNode
     from starlite.routes import ASGIRoute, HTTPRoute, WebSocketRoute
     from starlite.types import ASGIApp, RouteHandlerType
 
 
 def add_mount_route(
     current_node: RouteTrieNode,
     mount_routes: dict[str, RouteTrieNode],
```

### Comparing `starlite-2.0.0a1/starlite/asgi/routing_trie/traversal.py` & `starlite-2.0.0a2/starlite/_asgi/routing_trie/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Pattern
 
-from starlite.asgi.routing_trie.types import PathParameterSentinel
+from starlite._asgi.routing_trie.types import PathParameterSentinel
 from starlite.exceptions import MethodNotAllowedException, NotFoundException
 from starlite.utils import normalize_path
 
+__all__ = ("parse_node_handlers", "parse_path_params", "parse_path_to_route", "traverse_route_map")
+
+
 if TYPE_CHECKING:
-    from starlite.asgi.routing_trie.types import ASGIHandlerTuple, RouteTrieNode
+    from starlite._asgi.routing_trie.types import ASGIHandlerTuple, RouteTrieNode
     from starlite.types import ASGIApp, Method, RouteHandlerType
     from starlite.types.internal_types import PathParameterDefinition
 
 
 def traverse_route_map(
     root_node: RouteTrieNode,
     path: str,
@@ -36,20 +39,24 @@
     for i, component in enumerate(path_components):
         if component in current_node.child_keys:
             current_node = current_node.children[component]
             continue
 
         if current_node.is_path_param_node:
             current_node = current_node.children[PathParameterSentinel]
+
             if current_node.is_path_type:
                 path_params.append(normalize_path("/".join(path_components[i:])))
-            else:
-                path_params.append(component)
+                break
+
+            path_params.append(component)
+            continue
 
-        continue
+        if i != len(path_components) - 1:
+            raise NotFoundException()
 
     if not current_node.asgi_handlers:
         raise NotFoundException()
 
     return current_node, path_params, path
```

### Comparing `starlite-2.0.0a1/starlite/asgi/routing_trie/types.py` & `starlite-2.0.0a2/starlite/_asgi/routing_trie/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Literal, NamedTuple
 
+__all__ = ("ASGIHandlerTuple", "PathParameterSentinel", "RouteTrieNode", "create_node")
+
+
 if TYPE_CHECKING:
     from starlite.types import ASGIApp, Method, RouteHandlerType
     from starlite.types.internal_types import PathParameterDefinition
 
 
 class PathParameterSentinel:
     """Sentinel class designating a path parameter."""
@@ -46,15 +49,15 @@
     children: dict[str | type[PathParameterSentinel], RouteTrieNode]
     """A dictionary mapping path components or using the PathParameterSentinel class to child nodes."""
     is_path_param_node: bool
     """Designates the node as having a path parameter."""
     is_path_type: bool
     """Designates the node as having a 'path' type path parameter."""
     is_asgi: bool
-    """Designate the node as having an `@asgi` type handler."""
+    """Designate the node as having an `asgi` type handler."""
     is_mount: bool
     """Designate the node as being a mount route."""
     is_static: bool
     """Designate the node as being a static mount route."""
     path_parameters: dict[Method | Literal["websocket"] | Literal["asgi"], tuple[PathParameterDefinition, ...]]
     """A list of tuples containing path parameter definitions.
```

### Comparing `starlite-2.0.0a1/starlite/asgi/routing_trie/validate.py` & `starlite-2.0.0a2/starlite/_asgi/routing_trie/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from itertools import chain
 from typing import TYPE_CHECKING
 
 from starlite.exceptions import ImproperlyConfiguredException
 
+__all__ = ("validate_node",)
+
+
 if TYPE_CHECKING:
-    from starlite.asgi.routing_trie.types import RouteTrieNode
+    from starlite._asgi.routing_trie.types import RouteTrieNode
 
 
 def validate_node(node: RouteTrieNode) -> None:
     """Recursively traverses the trie from the given node upwards.
 
     Args:
         node: A trie node.
```

### Comparing `starlite-2.0.0a1/starlite/asgi/utils.py` & `starlite-2.0.0a2/starlite/_asgi/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
+__all__ = ("get_route_handlers", "wrap_in_exception_handler")
+
+
 if TYPE_CHECKING:
     from starlite.routes import ASGIRoute, HTTPRoute, WebSocketRoute
     from starlite.routes.base import BaseRoute
     from starlite.types import ASGIApp, ExceptionHandlersMap, RouteHandlerType
 
 
 def wrap_in_exception_handler(debug: bool, app: ASGIApp, exception_handlers: ExceptionHandlersMap) -> ASGIApp:
```

### Comparing `starlite-2.0.0a1/starlite/background_tasks.py` & `starlite-2.0.0a2/starlite/background_tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Any, Callable, Iterable
 
 from anyio import create_task_group
 from typing_extensions import ParamSpec
 
 from starlite.utils.sync import AsyncCallable
 
+__all__ = ("BackgroundTask", "BackgroundTasks")
+
+
 P = ParamSpec("P")
 
 
 class BackgroundTask:
     """A container for a 'background' task function.
 
     Background tasks are called once a Response finishes.
@@ -45,18 +48,17 @@
 
     __slots__ = ("tasks", "run_in_task_group")
 
     def __init__(self, tasks: Iterable[BackgroundTask], run_in_task_group: bool = False) -> None:
         """Initialize ``BackgroundTasks``.
 
         Args:
-            tasks: An iterable of :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instances.
+            tasks: An iterable of :class:`BackgroundTask <.background_tasks.BackgroundTask>` instances.
             run_in_task_group: If you set this value to ``True`` than the tasks will run concurrently, using
-                an [anyio.task_group](https://anyio.readthedocs.io/en/stable/tasks.html). Note: this will
-                not preserve execution order.
+                a :class:`TaskGroup <anyio.abc.TaskGroup>`. Note: This will not preserve execution order.
         """
         self.tasks = tasks
         self.run_in_task_group = run_in_task_group
 
     async def __call__(self) -> None:
         """Call the wrapped background tasks.
```

### Comparing `starlite-2.0.0a1/starlite/cli/commands/core.py` & `starlite-2.0.0a2/starlite/cli/commands/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 from __future__ import annotations
 
 import inspect
 import multiprocessing
 import subprocess
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import click
 from click import command, option
 from rich.tree import Tree
 
-from starlite import Starlite
-from starlite.cli.utils import StarliteEnv, console, show_app_info
+from starlite.cli._utils import StarliteEnv, console, show_app_info
 from starlite.routes import HTTPRoute, WebSocketRoute
 from starlite.utils.helpers import unwrap_partial
 
+__all__ = ("info_command", "routes_command", "run_command")
+
+if TYPE_CHECKING:
+    from starlite import Starlite
+
 
 def _convert_uvicorn_args(args: dict[str, Any]) -> list[str]:
     process_args = []
     for arg, value in args.items():
         if isinstance(value, bool):
             if value:
                 process_args.append(f"--{arg}")
         else:
             process_args.append(f"--{arg}={value}")
 
     return process_args
 
 
+@command(name="version")
+@option("-s", "--short", help="Exclude release level and serial information", is_flag=True, default=False)
+def version_command(short: bool) -> None:
+    from starlite import __version__
+
+    click.echo(__version__.formatted(short=short))
+
+
 @command(name="info")
 def info_command(app: Starlite) -> None:
     """Show information about the detected Starlite app."""
 
     show_app_info(app)
 
 
@@ -110,15 +122,12 @@
                 if len(handler.paths) > 1:
                     for path in handler.paths:
                         branch.add(" ".join([f"[green]{path}[green]", *handler_info]))
                 else:
                     branch.add(" ".join(handler_info))
 
         else:
-            if isinstance(route, WebSocketRoute):
-                route_type = "WS"
-            else:
-                route_type = "ASGI"
+            route_type = "WS" if isinstance(route, WebSocketRoute) else "ASGI"
             branch = tree.add(f"[green]{route.path}[/green] ({route_type})")
             branch.add(f"[blue]{route.route_handler.name or route.route_handler.handler_name}[/blue]")
 
     console.print(tree)
```

### Comparing `starlite-2.0.0a1/starlite/cli/commands/schema.py` & `starlite-2.0.0a2/starlite/cli/commands/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 
 from click import Path as ClickPath
 from click import group, option
 from jsbeautifier import Beautifier
 from yaml import dump as dump_yaml
 
 from starlite import Starlite
-from starlite.cli.utils import StarliteCLIException, StarliteGroup
-from starlite.openapi.typescript_converter.converter import (
+from starlite._openapi.typescript_converter.converter import (
     convert_openapi_to_typescript,
 )
+from starlite.cli._utils import StarliteCLIException, StarliteGroup
+
+__all__ = ("generate_openapi_schema", "generate_typescript_specs", "schema_group")
+
 
 beautifier = Beautifier()
 
 
 @group(cls=StarliteGroup, name="schema")
 def schema_group() -> None:
     """Manage server-side OpenAPI schemas."""
@@ -30,17 +33,17 @@
 )
 def generate_openapi_schema(app: Starlite, output: Path) -> None:
     """Generate an OpenAPI Schema."""
     if not app.openapi_schema:  # pragma: no cover
         raise StarliteCLIException("Starlite application does not have an OpenAPI schema")
 
     if output.suffix in (".yml", ".yaml"):
-        content = dump_yaml(app.openapi_schema.dict(by_alias=True, exclude_none=True), default_flow_style=False)
+        content = dump_yaml(app.openapi_schema.to_schema(), default_flow_style=False)
     else:
-        content = dumps(app.openapi_schema.dict(by_alias=True, exclude_none=True), indent=4)
+        content = dumps(app.openapi_schema.to_schema(), indent=4)
 
     try:
         output.write_text(content)
     except OSError as e:  # pragma: no cover
         raise StarliteCLIException(f"failed to write schema to path {output}") from e
```

### Comparing `starlite-2.0.0a1/starlite/cli/commands/sessions.py` & `starlite-2.0.0a2/starlite/cli/commands/sessions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from click import argument, group
 from rich.prompt import Confirm
 
 from starlite import Starlite
-from starlite.cli.utils import StarliteCLIException, StarliteGroup, console
+from starlite.cli._utils import StarliteCLIException, StarliteGroup, console
 from starlite.middleware import DefineMiddleware
 from starlite.middleware.session import SessionMiddleware
 from starlite.middleware.session.server_side import ServerSideSessionBackend
 from starlite.utils import is_class_and_subclass
 
+__all__ = ("clear_sessions_command", "delete_session_command", "get_session_backend", "sessions_group")
+
 
 def get_session_backend(app: Starlite) -> ServerSideSessionBackend:
     """Get the session backend used by a ``Starlite`` app."""
     for middleware in app.middleware:
         if isinstance(middleware, DefineMiddleware):
             if not is_class_and_subclass(middleware.middleware, SessionMiddleware):
                 continue
@@ -30,25 +32,27 @@
 @sessions_group.command("delete")
 @argument("session-id")
 def delete_session_command(session_id: str, app: Starlite) -> None:
     """Delete a specific session."""
     import anyio
 
     backend = get_session_backend(app)
+    store = backend.config.get_store_from_app(app)
 
     if Confirm.ask(f"Delete session {session_id!r}?"):
-        anyio.run(backend.delete, session_id)
+        anyio.run(backend.delete, session_id, store)
         console.print(f"[green]Deleted session {session_id!r}")
 
 
 @sessions_group.command("clear")
 def clear_sessions_command(app: Starlite) -> None:
     """Delete all sessions."""
     import anyio
 
     backend = get_session_backend(app)
-    if not hasattr(backend.storage, "delete_all"):
-        raise StarliteCLIException(f"{type(backend.storage)} does not support clearing all sessions")
+    store = backend.config.get_store_from_app(app)
+    if not hasattr(store, "delete_all"):
+        raise StarliteCLIException(f"{type(store)} does not support clearing all sessions")
 
     if Confirm.ask("[red]Delete all sessions?"):
-        anyio.run(backend.storage.delete_all)  # pyright: ignore
+        anyio.run(store.delete_all)  # pyright: ignore
         console.print("[green]All active sessions deleted")
```

### Comparing `starlite-2.0.0a1/starlite/cli/main.py` & `starlite-2.0.0a2/starlite/cli/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 from click import Context, group, option, pass_context
 
+from ._utils import StarliteEnv, StarliteExtensionGroup
 from .commands import core, schema, sessions
-from .utils import StarliteEnv, StarliteExtensionGroup
+
+__all__ = ("starlite_group",)
 
 
 @group(cls=StarliteExtensionGroup)
 @option("--app", "app_path", help="Module path to a Starlite application")
 @pass_context
 def starlite_group(ctx: Context, app_path: str | None) -> None:
     """Starlite CLI."""
 
-    ctx.obj = StarliteEnv.from_env(app_path)
+    ctx.obj = lambda: StarliteEnv.from_env(app_path)
 
 
 # add sub commands here
 
 starlite_group.add_command(core.info_command)
 starlite_group.add_command(core.run_command)
 starlite_group.add_command(core.routes_command)
+starlite_group.add_command(core.version_command)
 starlite_group.add_command(sessions.sessions_group)
 starlite_group.add_command(schema.schema_group)
```

### Comparing `starlite-2.0.0a1/starlite/cli/utils.py` & `starlite-2.0.0a2/starlite/cli/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from __future__ import annotations
 
 import importlib
 import inspect
 import sys
 from dataclasses import dataclass
 from functools import wraps
-from importlib.metadata import version
+from itertools import chain
 from os import getenv
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Sequence, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Sequence, TypeVar, cast
 
 from click import ClickException, Command, Context, Group, pass_context, style
 from rich.console import Console
 from rich.table import Table
 from typing_extensions import Concatenate, ParamSpec
 
-from starlite import Starlite
+from starlite import Starlite, __version__
 from starlite.middleware import DefineMiddleware
 from starlite.utils import get_name
 
+__all__ = (
+    "LoadedApp",
+    "StarliteCLIException",
+    "StarliteEnv",
+    "StarliteExtensionGroup",
+    "StarliteGroup",
+    "show_app_info",
+)
+
+
 if sys.version_info >= (3, 10):
     from importlib.metadata import entry_points
 else:
     from importlib_metadata import entry_points  # pragma: no cover
 
 
 if TYPE_CHECKING:
     from starlite.types import AnyCallable
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-AUTODISCOVER_PATHS = [
-    "asgi.py",
-    "app.py",
-    "application.py",
-    "app/__init__.py",
-    "application/__init__.py",
-]
+AUTODISCOVERY_FILE_NAMES = ["app", "application"]
 
 console = Console()
 
 
 class StarliteCLIException(ClickException):
     """Base class for Starlite CLI exceptions."""
 
@@ -80,18 +84,20 @@
         try:
             import dotenv
 
             dotenv.load_dotenv()
         except ImportError:
             pass
 
-        if not app_path:
-            loaded_app = _autodiscover_app(getenv("STARLITE_APP"), cwd)
-        else:
+        app_path = app_path or getenv("STARLITE_APP")
+        if app_path:
+            console.print(f"Using Starlite app from env: [bright_blue]{app_path!r}")
             loaded_app = _load_app_from_path(app_path)
+        else:
+            loaded_app = _autodiscover_app(cwd)
 
         port = getenv("STARLITE_PORT")
         web_concurrency = getenv("WEB_CONCURRENCY")
 
         return cls(
             app_path=loaded_app.app_path,
             app=loaded_app.app,
@@ -145,15 +151,15 @@
         """Add a function as a command.
 
         If necessary, inject ``app`` and ``env`` kwargs
         """
 
         def decorator(f: AnyCallable) -> Command:
             f = _inject_args(f)
-            return cast("Command", Group.command(self, *args, **kwargs)(f))  # pylint: disable=E1102
+            return cast("Command", Group.command(self, *args, **kwargs)(f))
 
         return decorator
 
 
 class StarliteExtensionGroup(StarliteGroup):
     """``StarliteGroup`` subclass that will load Starlite-CLI extensions from the `starlite.commands` entry_point.
 
@@ -177,19 +183,26 @@
 
 def _inject_args(func: Callable[P, T]) -> Callable[Concatenate[Context, P], T]:
     """Inject the app instance into a ``Command``"""
     params = inspect.signature(func).parameters
 
     @wraps(func)
     def wrapped(ctx: Context, /, *args: P.args, **kwargs: P.kwargs) -> T:
-        env = ctx.ensure_object(StarliteEnv)
-        if "app" in params:
-            kwargs["app"] = env.app
-        if "env" in params:
-            kwargs["env"] = env
+        needs_app = "app" in params
+        needs_env = "env" in params
+        if needs_env or needs_app:
+            # only resolve this if actually requested. Commands that don't need an env or app should be able to run
+            # without
+            if not isinstance(ctx.obj, StarliteEnv):
+                ctx.obj = ctx.obj()
+            env = ctx.ensure_object(StarliteEnv)
+            if needs_app:
+                kwargs["app"] = env.app
+            if needs_env:
+                kwargs["env"] = env
         return func(*args, **kwargs)
 
     return pass_context(wrapped)
 
 
 def _wrap_commands(commands: Iterable[Command]) -> None:
     for command in commands:
@@ -220,44 +233,60 @@
 
 def _path_to_dotted_path(path: Path) -> str:
     if path.stem == "__init__":
         path = path.parent
     return ".".join(path.with_suffix("").parts)
 
 
-def _autodiscover_app(app_path: str | None, cwd: Path) -> LoadedApp:
-    if app_path:
-        console.print(f"Using Starlite app from env: [bright_blue]{app_path!r}")
-        return _load_app_from_path(app_path)
-
-    for name in AUTODISCOVER_PATHS:
-        path = cwd / name
-        if not path.exists():
+def _arbitrary_autodiscovery_paths(base_dir: Path) -> Generator[Path, None, None]:
+    yield from _autodiscovery_paths(base_dir, arbitrary=False)
+    for path in base_dir.iterdir():
+        if path.name.startswith(".") or path.name.startswith("_"):
             continue
+        if path.is_file() and path.suffix == ".py":
+            yield path
 
-        dotted_path = _path_to_dotted_path(path.relative_to(cwd))
-        module = importlib.import_module(dotted_path)
 
-        for attr, value in module.__dict__.items():
+def _autodiscovery_paths(base_dir: Path, arbitrary: bool = True) -> Generator[Path, None, None]:
+    for name in AUTODISCOVERY_FILE_NAMES:
+        path = base_dir / name
+
+        if path.exists() or path.with_suffix(".py").exists():
+            yield path
+        if arbitrary and path.is_dir():
+            yield from _arbitrary_autodiscovery_paths(path)
+
+
+def _autodiscover_app(cwd: Path) -> LoadedApp:
+    for file_path in _autodiscovery_paths(cwd):
+        import_path = _path_to_dotted_path(file_path.relative_to(cwd))
+        module = importlib.import_module(import_path)
+
+        for attr, value in chain(
+            [("app", getattr(module, "app", None)), ("application", getattr(module, "application", None))],
+            module.__dict__.items(),
+        ):
             if isinstance(value, Starlite):
-                app_string = f"{dotted_path}:{attr}"
+                app_string = f"{import_path}:{attr}"
                 console.print(f"Using Starlite app from [bright_blue]{app_string}")
                 return LoadedApp(app=value, app_path=app_string, is_factory=False)
 
         if hasattr(module, "create_app"):
-            app_string = f"{dotted_path}:create_app"
+            app_string = f"{import_path}:create_app"
             console.print(f"Using Starlite factory [bright_blue]{app_string}")
             return LoadedApp(app=module.create_app(), app_path=app_string, is_factory=True)
 
         for attr, value in module.__dict__.items():
             if not callable(value):
                 continue
-            signature = inspect.signature(value)
-            if signature.return_annotation in ("Starlite", Starlite):
-                app_string = f"{dotted_path}:{attr}"
+            return_annotation = getattr(value, "__annotations__", {}).get("return")
+            if not return_annotation:
+                continue
+            if return_annotation in ("Starlite", Starlite):
+                app_string = f"{import_path}:{attr}"
                 console.print(f"Using Starlite factory [bright_blue]{app_string}")
                 return LoadedApp(app=value(), app_path=f"{app_string}", is_factory=True)
 
     raise StarliteCLIException("Could not find a Starlite app or factory")
 
 
 def _format_is_enabled(value: Any) -> str:
@@ -270,24 +299,23 @@
 def show_app_info(app: Starlite) -> None:  # pragma: no cover
     """Display basic information about the application and its configuration."""
 
     table = Table(show_header=False)
     table.add_column("title", style="cyan")
     table.add_column("value", style="bright_blue")
 
-    table.add_row("Starlite version", version("starlite"))
+    table.add_row("Starlite version", f"{__version__.major}.{__version__.minor}.{__version__.patch}")
     table.add_row("Debug mode", _format_is_enabled(app.debug))
     table.add_row("CORS", _format_is_enabled(app.cors_config))
     table.add_row("CSRF", _format_is_enabled(app.csrf_config))
     if app.allowed_hosts:
         allowed_hosts = app.allowed_hosts
 
         table.add_row("Allowed hosts", ", ".join(allowed_hosts.allowed_hosts))
 
-    table.add_row("Request caching", _format_is_enabled(app.cache))
     openapi_enabled = _format_is_enabled(app.openapi_config)
     if app.openapi_config:
         openapi_enabled += f" path=[yellow]{app.openapi_config.openapi_controller.path}"
     table.add_row("OpenAPI", openapi_enabled)
 
     table.add_row("Compression", app.compression_config.backend if app.compression_config else "[red]Disabled")
 
@@ -306,15 +334,13 @@
 
     if app.serialization_plugins:
         plugin_names = [type(plugin).__name__ for plugin in app.serialization_plugins]
         table.add_row("Plugins", ", ".join(plugin_names))
 
     middlewares = []
     for middleware in app.middleware:
-        if isinstance(middleware, DefineMiddleware):
-            middleware = middleware.middleware
-        middlewares.append(get_name(middleware))
+        updated_middleware = middleware.middleware if isinstance(middleware, DefineMiddleware) else middleware
+        middlewares.append(get_name(updated_middleware))
     if middlewares:
         table.add_row("Middlewares", ", ".join(middlewares))
 
     console.print(table)
-    console.print(table)
```

### Comparing `starlite-2.0.0a1/starlite/config/allowed_hosts.py` & `starlite-2.0.0a2/starlite/config/allowed_hosts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 from starlite.exceptions import ImproperlyConfiguredException
 
+__all__ = ("AllowedHostsConfig",)
+
+
 if TYPE_CHECKING:
     from starlite.types import Scopes
 
 
 @dataclass
 class AllowedHostsConfig:
     """Configuration for allowed hosts protection.
```

### Comparing `starlite-2.0.0a1/starlite/config/app.py` & `starlite-2.0.0a2/starlite/config/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Sequence
 
 from starlite.config.allowed_hosts import AllowedHostsConfig
-from starlite.config.cache import CacheConfig
+from starlite.config.response_cache import ResponseCacheConfig
+from starlite.datastructures import State
 from starlite.events.emitter import SimpleEventEmitter
 
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
-
     from starlite.config.compression import CompressionConfig
     from starlite.config.cors import CORSConfig
     from starlite.config.csrf import CSRFConfig
-    from starlite.config.logging import BaseLoggingConfig
-    from starlite.config.openapi import OpenAPIConfig
-    from starlite.config.static_files import StaticFilesConfig
-    from starlite.config.template import TemplateConfig
     from starlite.connection import Request, WebSocket
     from starlite.datastructures import CacheControlHeader, ETag, ResponseHeader
     from starlite.di import Provide
     from starlite.events.emitter import BaseEventEmitterBackend
     from starlite.events.listener import EventListener
+    from starlite.logging.config import BaseLoggingConfig
+    from starlite.openapi.config import OpenAPIConfig
+    from starlite.openapi.spec import SecurityRequirement
     from starlite.plugins import PluginProtocol
+    from starlite.static_files.config import StaticFilesConfig
+    from starlite.stores.base import Store
+    from starlite.stores.registry import StoreRegistry
+    from starlite.template.config import TemplateConfig
     from starlite.types import (
         AfterExceptionHookHandler,
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeMessageSendHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
@@ -36,161 +38,166 @@
         LifeSpanHookHandler,
         Middleware,
         ParametersMap,
         ResponseCookies,
         ResponseType,
         TypeEncodersMap,
     )
-    from starlite.types.composite_types import InitialStateType
+
+__all__ = ("AppConfig",)
 
 
 @dataclass
 class AppConfig:
     """The parameters provided to the ``Starlite`` app are used to instantiate an instance, and then the instance is
     passed to any callbacks registered to ``on_app_init`` in the order they are provided.
 
     The final attribute values are used to instantiate the application object.
     """
 
     after_exception: list[AfterExceptionHookHandler] = field(default_factory=list)
-    """An application level :class:`exception hook handler <starlite.types.AfterExceptionHookHandler>` or list thereof.
+    """An application level :class:`exception hook handler <.types.AfterExceptionHookHandler>` or list thereof.
 
     This hook is called after an exception occurs. In difference to exception handlers, it is not meant to return a
     response - only to process the exception (e.g. log it, send it to Sentry etc.).
     """
     after_request: AfterRequestHookHandler | None = field(default=None)
     """A sync or async function executed after the route handler function returned and the response object has been
     resolved.
 
-    Receives the response object which may be any subclass of :class:`Response <starlite.response.Response>`.
+    Receives the response object which may be any subclass of :class:`Response <.response.Response>`.
     """
     after_response: AfterResponseHookHandler | None = field(default=None)
-    """A sync or async function called after the response has been awaited. It receives the.
-
-    :class:`Request <starlite.connection.Request>` object and should not return any values.
+    """A sync or async function called after the response has been awaited. It receives the
+    :class:`Request <.connection.Request>` object and should not return any values.
     """
     after_shutdown: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <starlite.types.LifeSpanHookHandler>` or list thereof.
+    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
 
-    This hook is called during the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
+    This hook is called during the ASGI shutdown, after all callables in the ``on_shutdown`` list have been called.
     """
     after_startup: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <starlite.types.LifeSpanHookHandler>` or list thereof.
+    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
 
-    This hook is called during the ASGI startup, after all callables in the 'on_startup' list have been called.
+    This hook is called during the ASGI startup, after all callables in the ``on_startup`` list have been called.
     """
     allowed_hosts: list[str] | AllowedHostsConfig | None = field(default=None)
     """If set enables the builtin allowed hosts middleware."""
     before_request: BeforeRequestHookHandler | None = field(default=None)
-    """A sync or async function called immediately before calling the route handler. Receives the.
-
-    :class:`Request <starlite.connection.Request>` instance and any non-``None`` return value is used for the response, bypassing
-    the route handler.
+    """A sync or async function called immediately before calling the route handler. Receives the
+    :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the response,
+    bypassing the route handler.
     """
     before_send: list[BeforeMessageSendHookHandler] = field(default_factory=list)
-    """An application level :class:`before send hook handler <starlite.types.BeforeMessageSendHookHandler>` or list thereof.
+    """An application level :class:`before send hook handler <.types.BeforeMessageSendHookHandler>` or list thereof.
 
     This hook is called when the ASGI send function is called.
     """
     before_shutdown: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <starlite.types.LifeSpanHookHandler>` or list thereof.
+    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
 
-    This hook is called during the ASGI shutdown, before any callables in the 'on_shutdown' list have been called.
+    This hook is called during the ASGI shutdown, before any callables in the ``on_shutdown`` list have been called.
     """
     before_startup: list[LifeSpanHookHandler] = field(default_factory=list)
-    """An application level :class:`life-span hook handler <starlite.types.LifeSpanHookHandler>` or list thereof.
+    """An application level :class:`life-span hook handler <.types.LifeSpanHookHandler>` or list thereof.
 
-    This hook is called during the ASGI startup, before any callables in the 'on_startup' list have been called.
+    This hook is called during the ASGI startup, before any callables in the ``on_startup`` list have been called.
     """
-    cache_config: CacheConfig = field(default_factory=CacheConfig)
-    """Configures caching behavior of the application."""
     cache_control: CacheControlHeader | None = field(default=None)
-    """A ``cache-control`` header of type :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` to add to route
-    handlers of this app.
+    """A ``cache-control`` header of type :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to
+    route handlers of this app.
 
     Can be overridden by route handlers.
     """
     compression_config: CompressionConfig | None = field(default=None)
     """Configures compression behaviour of the application, this enabled a builtin or user defined Compression
     middleware.
     """
     cors_config: CORSConfig | None = field(default=None)
     """If set this enables the builtin CORS middleware."""
     csrf_config: CSRFConfig | None = field(default=None)
     """If set this enables the builtin CSRF middleware."""
     debug: bool = field(default=False)
     """If ``True``, app errors rendered as HTML with a stack trace."""
     dependencies: dict[str, Provide] = field(default_factory=dict)
-    """A string keyed dictionary of dependency :class:`Provider <starlite.datastructures.Provide>` instances."""
+    """A string keyed dictionary of dependency :class:`Provider <.di.Provide>` instances."""
     etag: ETag | None = field(default=None)
-    """An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` to add to route handlers of this app.
+    """An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
 
     Can be overridden by route handlers.
     """
     event_emitter_backend: type[BaseEventEmitterBackend] = field(default=SimpleEventEmitter)
-    """A subclass of :class:`BaseEventEmitterBackend <starlite.events.emitter.BaseEventEmitterBackend>`."""
+    """A subclass of :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`."""
     exception_handlers: ExceptionHandlersMap = field(default_factory=dict)
     """A dictionary that maps handler functions to status codes and/or exception types."""
     guards: list[Guard] = field(default_factory=list)
-    """A list of :class:`Guard <starlite.types.Guard>` callables."""
-    initial_state: InitialStateType = field(default_factory=dict)
-    """An object from which to initialize the app state."""
+    """A list of :class:`Guard <.types.Guard>` callables."""
     listeners: list[EventListener] = field(default_factory=list)
-    """A list of :class:`EventListener <starlite.events.listener.EventListener>`."""
+    """A list of :class:`EventListener <.events.listener.EventListener>`."""
     logging_config: BaseLoggingConfig | None = field(default=None)
-    """An instance of :class:`BaseLoggingConfig <starlite.config.logging.BaseLoggingConfig>` subclass."""
+    """An instance of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>` subclass."""
     middleware: list[Middleware] = field(default_factory=list)
-    """A list of :class:`Middleware <starlite.types.Middleware>`."""
+    """A list of :class:`Middleware <.types.Middleware>`."""
     on_shutdown: list[LifeSpanHandler] = field(default_factory=list)
-    """A list of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during application shutdown."""
+    """A list of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application shutdown."""
     on_startup: list[LifeSpanHandler] = field(default_factory=list)
-    """A list of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during application startup."""
+    """A list of :class:`LifeSpanHandler <.types.LifeSpanHandler>` called during application startup."""
     openapi_config: OpenAPIConfig | None = field(default=None)
-    """Defaults to :data:`DEFAULT_OPENAPI_CONFIG <starlite.app.DEFAULT_OPENAPI_CONFIG>`"""
+    """Defaults to :data:`DEFAULT_OPENAPI_CONFIG <.app.DEFAULT_OPENAPI_CONFIG>`"""
     opt: dict[str, Any] = field(default_factory=dict)
-    """A string keyed dictionary of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-    wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
+    """A string keyed dictionary of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+    wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
 
     Can be overridden by routers and router handlers.
     """
     parameters: ParametersMap = field(default_factory=dict)
-    """A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all application paths."""
+    """A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application paths."""
     plugins: list[PluginProtocol] = field(default_factory=list)
-    """List of :class:`SerializationPluginProtocol <starlite.plugins.base.SerializationPluginProtocol>`."""
+    """List of :class:`SerializationPluginProtocol <.plugins.SerializationPluginProtocol>`."""
     request_class: type[Request] | None = field(default=None)
-    """An optional subclass of :class:`Request <starlite.connection.request.Request>` to use for http connections."""
+    """An optional subclass of :class:`Request <.connection.Request>` to use for http connections."""
     response_class: ResponseType | None = field(default=None)
-    """A custom subclass of [starlite.response.Response] to be used as the app's default response."""
+    """A custom subclass of :class:`Response <.response.Response>` to be used as the app's default response."""
     response_cookies: ResponseCookies = field(default_factory=list)  # type: ignore
-    """A list of [Cookie](starlite.datastructures.Cookie] instances."""
+    """A list of :class:`Cookie <.datastructures.Cookie>`."""
     response_headers: Sequence[ResponseHeader] = field(default_factory=list)
-    """A string keyed dictionary mapping :class:`ResponseHeader <starlite.datastructures.ResponseHeader>` instances."""
+    """A string keyed dictionary mapping :class:`ResponseHeader <.datastructures.ResponseHeader>`."""
+    response_cache_config: ResponseCacheConfig = field(default_factory=ResponseCacheConfig)
+    """Configures caching behavior of the application."""
     route_handlers: list[ControllerRouterHandler] = field(default_factory=list)
-    """A required list of route handlers, which can include instances of :class:`Router <starlite.router.Router>`, subclasses
-    of.
-
-    :class:`Controller <starlite.controller.Controller>` or any function decorated by the route handler decorators.
+    """A required list of route handlers, which can include instances of :class:`Router <.router.Router>`,
+    subclasses of :class:`Controller <.controller.Controller>` or any function decorated by the route handler
+    decorators.
     """
     security: list[SecurityRequirement] = field(default_factory=list)
-    """A list of dictionaries that will be added to the schema of all route handlers in the application. See.
-
-    :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` for details.
+    """A list of dictionaries that will be added to the schema of all route handlers in the application. See
+    :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for details.
     """
+    signature_namespace: dict[str, Any] = field(default_factory=dict)
+    """A mapping of names to types for use in forward reference resolution during signature modelling."""
+    state: State = field(default_factory=State)
+    """A :class:`State` <.datastructures.State>` instance holding application state."""
     static_files_config: list[StaticFilesConfig] = field(default_factory=list)
-    """An instance or list of :class:`StaticFilesConfig <starlite.config.StaticFilesConfig>`."""
+    """An instance or list of :class:`StaticFilesConfig <.static_files.StaticFilesConfig>`."""
+    stores: StoreRegistry | dict[str, Store] | None = None
+    """Central registry of :class:`Store <.stores.base.Store>` to be made available and be used throughout the
+    application. Can be either a dictionary mapping strings to :class:`Store <.stores.base.Store>` instances, or an
+    instance of :class:`StoreRegistry <.stores.registry.StoreRegistry>`.
+    """
     tags: list[str] = field(default_factory=list)
     """A list of string tags that will be appended to the schema of all route handlers under the application."""
     template_config: TemplateConfig | None = field(default=None)
-    """An instance of :class:`TemplateConfig <starlite.config.TemplateConfig>`."""
+    """An instance of :class:`TemplateConfig <.template.TemplateConfig>`."""
     type_encoders: TypeEncodersMap | None = field(default=None)
     """A mapping of types to callables that transform them into types supported for serialization."""
     websocket_class: type[WebSocket] | None = field(default=None)
-    """An optional subclass of :class:`WebSocket <starlite.connection.websocket.WebSocket>` to use for websocket connections."""
+    """An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket connections."""
     multipart_form_part_limit: int = field(default=1000)
-    """The maximal number of allowed parts in a multipart/formdata request. This limit is intended to protect from DoS attacks."""
+    """The maximal number of allowed parts in a multipart/formdata request. This limit is intended to protect from
+    DoS attacks."""
 
     def __post_init__(self) -> None:
         """Normalize the allowed hosts to be a config or None.
 
         Returns:
             Optional config.
         """
```

### Comparing `starlite-2.0.0a1/starlite/config/cache.py` & `starlite-2.0.0a2/starlite/config/response_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlencode
 
-from starlite.cache import Cache
-from starlite.storage.memory import MemoryStorage
+__all__ = ("ResponseCacheConfig", "default_cache_key_builder")
+
 
 if TYPE_CHECKING:
+    from starlite import Starlite
     from starlite.connection import Request
-    from starlite.storage.base import Storage
+    from starlite.stores.base import Store
     from starlite.types import CacheKeyBuilder
 
 
 def default_cache_key_builder(request: Request[Any, Any, Any]) -> str:
     """Given a request object, returns a cache key by combining the path with the sorted query params.
 
     Args:
-        request (Request): request used to generate cache key.
+        request: request used to generate cache key.
 
     Returns:
-        str: combination of url path and query parameters
+        A combination of url path and query parameters
     """
     query_params: list[tuple[str, Any]] = list(request.query_params.dict().items())
     query_params.sort(key=lambda x: x[0])
     return request.url.path + urlencode(query_params, doseq=True)
 
 
 @dataclass
-class CacheConfig:
+class ResponseCacheConfig:
     """Configuration for response caching.
 
-    To enable response caching, pass an instance of this class to the :class:`Starlite <starlite.app.Starlite>` constructor
-    using the 'cache_config' key.
+    To enable response caching, pass an instance of this class to :class:`Starlite <.app.Starlite>` using the
+    ``response_cache_config`` key.
     """
 
-    backend: Storage | None = field(default=None)
-    """Instance conforming to :class:`CacheBackendProtocol <starlite.cache.CacheBackendProtocol>`, default.
-
-    :class:`MemoryStorage() <starlite.cache.MemoryStorage>`
-    """
-    expiration: int = field(default=60)
+    default_expiration: int = field(default=60)
     """Default cache expiration in seconds."""
-    cache_key_builder: CacheKeyBuilder = field(default=default_cache_key_builder)
-    """:class:`CacheKeyBuilder <starlite.types.CacheKeyBuilder>`,
-
-    :func:`default_cache_key_builder <starlite.config.cache.default_cache_key_builder>` if not provided
-    """
-
-    def to_cache(self) -> Cache:
-        """Create a cache wrapper from the config.
-
-        Returns:
-            An instance of :class:`Cache <starlite.cache.base.Cache>`
-        """
-        return Cache(
-            backend=self.backend or MemoryStorage(),
-            default_expiration=self.expiration,
-            cache_key_builder=self.cache_key_builder,
-        )
+    key_builder: CacheKeyBuilder = field(default=default_cache_key_builder)
+    """:class:`CacheKeyBuilder <.types.CacheKeyBuilder>`. Defaults to :func:`default_cache_key_builder`."""
+    store: str = "request_cache"
+    """Name of the :class:`Store <.stores.base.Store>` to use."""
+
+    def get_store_from_app(self, app: Starlite) -> Store:
+        """Get the store defined in :attr:`store` from an :class:`Starlite <.app.Starlite>` instance."""
+        return app.stores.get(self.store)
```

### Comparing `starlite-2.0.0a1/starlite/config/compression.py` & `starlite-2.0.0a2/starlite/config/compression.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,50 +2,52 @@
 
 from dataclasses import dataclass, field
 from typing import Literal
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.middleware.compression import CompressionMiddleware
 
+__all__ = ("CompressionConfig",)
+
 
 @dataclass
 class CompressionConfig:
     """Configuration for response compression.
 
-    To enable response compression, pass an instance of this class to the :class:`Starlite <starlite.app.Starlite>` constructor
-    using the 'compression_config' key.
+    To enable response compression, pass an instance of this class to the :class:`Starlite <.app.Starlite>` constructor
+    using the ``compression_config`` key.
     """
 
     backend: Literal["gzip", "brotli"]
     """Literal of "gzip" or "brotli"."""
     minimum_size: int = field(default=500)
     """Minimum response size (bytes) to enable compression, affects all backends."""
     gzip_compress_level: int = field(default=9)
-    """Range [0-9], see [official docs](https://docs.python.org/3/library/gzip.html)."""
+    """Range ``[0-9]``, see :doc:`python:library/gzip`."""
     brotli_quality: int = field(default=5)
-    """Range [0-11], Controls the compression-speed vs compression-density tradeoff.
+    """Range ``[0-11]``, Controls the compression-speed vs compression-density tradeoff.
 
     The higher the quality, the slower the compression.
     """
     brotli_mode: Literal["generic", "text", "font"] = "text"
-    """MODE_GENERIC, MODE_TEXT (for UTF-8 format text input, default) or MODE_FONT (for WOFF 2.0)."""
+    """``MODE_GENERIC``, ``MODE_TEXT`` (for UTF-8 format text input, default) or ``MODE_FONT`` (for WOFF 2.0)."""
     brotli_lgwin: int = field(default=22)
     """Base 2 logarithm of size.
 
     Range is 10 to 24. Defaults to 22.
     """
     brotli_lgblock: Literal[0, 16, 17, 18, 19, 20, 21, 22, 23, 24] = 0
     """Base 2 logarithm of the maximum input block size.
 
-    Range is 16 to 24. If set to 0, the value will be set based on the quality. Defaults to 0.
+    Range is ``16`` to ``24``. If set to ``0``, the value will be set based on the quality. Defaults to ``0``.
     """
     brotli_gzip_fallback: bool = True
     """Use GZIP if Brotli is not supported."""
     middleware_class: type[CompressionMiddleware] = CompressionMiddleware
-    """Middleware class to use, should be a subclass of CompressionMiddleware."""
+    """Middleware class to use, should be a subclass of :class:`CompressionMiddleware`."""
     exclude: str | list[str] | None = None
     """A pattern or list of patterns to skip in the compression middleware."""
     exclude_opt_key: str | None = None
     """An identifier to use on routes to disable compression for a particular route."""
 
     def __post_init__(self) -> None:
         if self.minimum_size <= 0:
```

### Comparing `starlite-2.0.0a1/starlite/config/cors.py` & `starlite-2.0.0a2/starlite/config/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import re
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import TYPE_CHECKING, Literal, Pattern
 
 from starlite.constants import DEFAULT_ALLOWED_CORS_HEADERS
 
+__all__ = ("CORSConfig",)
+
+
 if TYPE_CHECKING:
     from starlite.types import Method
 
 
 @dataclass
 class CORSConfig:
     """Configuration for CORS (Cross-Origin Resource Sharing).
```

### Comparing `starlite-2.0.0a1/starlite/config/csrf.py` & `starlite-2.0.0a2/starlite/config/csrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Literal
 
+__all__ = ("CSRFConfig",)
+
+
 if TYPE_CHECKING:
     from starlite.types import Method
 
 
 @dataclass
 class CSRFConfig:
     """Configuration for CSRF (Cross Site Request Forgery) protection.
```

### Comparing `starlite-2.0.0a1/starlite/config/logging.py` & `starlite-2.0.0a2/starlite/logging/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,29 @@
 
 from starlite.exceptions import (
     ImproperlyConfiguredException,
     MissingDependencyException,
 )
 from starlite.serialization import encode_json
 
+__all__ = ("BaseLoggingConfig", "LoggingConfig", "StructLoggingConfig")
+
+
 if TYPE_CHECKING:
     from typing import NoReturn
 
-    from starlite.types import Logger
-    from starlite.types.callable_types import GetLogger
+    # these imports are duplicated on purpose so sphinx autodoc can find and link them
+    from structlog.types import BindableLogger, Processor, WrappedLogger
+
+    from starlite.types import Logger, Scope
+    from starlite.types.callable_types import ExceptionLoggingHandler, GetLogger
+
 
 try:
-    from structlog.types import BindableLogger, Processor, WrappedLogger
+    from structlog.types import BindableLogger, Processor, WrappedLogger  # noqa: F811
 except ImportError:
     BindableLogger = Any  # type: ignore
     Processor = Any  # type: ignore
     WrappedLogger = Any  # type: ignore
 
 
 default_handlers: dict[str, dict[str, Any]] = {
@@ -49,36 +56,77 @@
         "class": "starlite.logging.picologging.QueueListenerHandler",
         "level": "DEBUG",
         "formatter": "standard",
     },
 }
 
 
-def get_default_handlers() -> dict[str, dict[str, Any]]:
+def get_logger_placeholder(_: str) -> NoReturn:  # pragma: no cover
+    """Raise: An :class:`ImproperlyConfiguredException <.exceptions.ImproperlyConfiguredException>`"""
+    raise ImproperlyConfiguredException(
+        "cannot call '.get_logger' without passing 'logging_config' to the Starlite constructor first"
+    )
+
+
+def _get_default_handlers() -> dict[str, dict[str, Any]]:
     """Return the default logging handlers for the config.
 
     Returns:
         A dictionary of logging handlers
     """
     if find_spec("picologging"):
         return default_picologging_handlers
     return default_handlers
 
 
-def get_logger_placeholder(_: str) -> NoReturn:  # pragma: no cover
-    """Raise an `ImproperlyConfiguredException."""
-    raise ImproperlyConfiguredException(
-        "To use 'app.get_logger', 'request.get_logger' or 'socket.get_logger' pass 'logging_config' to the Starlite constructor"
-    )
+def _default_exception_logging_handler_factory(
+    is_struct_logger: bool, traceback_line_limit: int
+) -> ExceptionLoggingHandler:
+    """Create an exception logging handler function.
+
+    Args:
+        is_struct_logger: Whether the logger is a structlog instance.
+        traceback_line_limit: Maximal number of lines to log from the
+            traceback.
+
+    Returns:
+        An exception logging handler.
+    """
+
+    def _default_exception_logging_handler(logger: Logger, scope: Scope, tb: list[str]) -> None:
+        # we limit the length of the stack trace to 20 lines.
+        first_line = tb.pop(0)
+
+        if is_struct_logger:
+            logger.exception(
+                "uncaught exception",
+                connection_type=scope["type"],
+                path=scope["path"],
+                traceback="".join(tb[-traceback_line_limit:]),
+            )
+        else:
+            stack_trace = first_line + "".join(tb[-traceback_line_limit:])
+            logger.exception(
+                "exception raised on %s connection to route %s\n\n%s", scope["type"], scope["path"], stack_trace
+            )
+
+    return _default_exception_logging_handler
 
 
 class BaseLoggingConfig(ABC):  # pragma: no cover
     """Abstract class that should be extended by logging configs."""
 
-    __slots__ = ()
+    __slots__ = ("log_exceptions", "traceback_line_limit", "exception_logging_handler")
+
+    log_exceptions: Literal["always", "debug", "never"]
+    """Should exceptions be logged, defaults to log exceptions when ``app.debug == True``'"""
+    traceback_line_limit: int
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None
+    """Handler function for logging exceptions."""
 
     @abstractmethod
     def configure(self) -> GetLogger:
         """Return logger with the given configuration.
 
         Returns:
             A 'logging.getLogger' like function.
@@ -111,15 +159,15 @@
     propagate: bool = field(default=True)
     """If messages must propagate to handlers higher up the logger hierarchy from this logger."""
     formatters: dict[str, dict[str, Any]] = field(
         default_factory=lambda: {
             "standard": {"format": "%(levelname)s - %(asctime)s - %(name)s - %(module)s - %(message)s"}
         }
     )
-    handlers: dict[str, dict[str, Any]] = field(default_factory=get_default_handlers)
+    handlers: dict[str, dict[str, Any]] = field(default_factory=_get_default_handlers)
     """A dict in which each key is a handler id and each value is a dict describing how to configure the corresponding
     Handler instance.
     """
     loggers: dict[str, dict[str, Any]] = field(
         default_factory=lambda: {
             "starlite": {"level": "INFO", "handlers": ["queue_listener"], "propagate": False},
         }
@@ -133,26 +181,37 @@
             "level": "INFO",
         }
     )
     """This will be the configuration for the root logger.
 
     Processing of the configuration will be as for any logger, except that the propagate setting will not be applicable.
     """
+    log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
+    """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
+    traceback_line_limit: int = field(default=20)
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
+    """Handler function for logging exceptions."""
 
     def __post_init__(self) -> None:
         if "queue_listener" not in self.handlers:
-            self.handlers["queue_listener"] = get_default_handlers()["queue_listener"]
+            self.handlers["queue_listener"] = _get_default_handlers()["queue_listener"]
 
         if "starlite" not in self.loggers:
             self.loggers["starlite"] = {
                 "level": "INFO",
                 "handlers": ["queue_listener"],
                 "propagate": False,
             }
 
+        if self.log_exceptions != "never" and self.exception_logging_handler is None:
+            self.exception_logging_handler = _default_exception_logging_handler_factory(
+                is_struct_logger=False, traceback_line_limit=self.traceback_line_limit
+            )
+
     def configure(self) -> GetLogger:
         """Return logger with the given configuration.
 
         Returns:
             A 'logging.getLogger' like function.
         """
 
@@ -222,35 +281,59 @@
 
 
 @dataclass
 class StructLoggingConfig(BaseLoggingConfig):
     """Configuration class for structlog.
 
     Notes:
-        - requires 'structlog' to be installed.
+        - requires ``structlog`` to be installed.
     """
 
     processors: list[Processor] | None = field(default_factory=default_structlog_processors)  # pyright: ignore
     """Iterable of structlog logging processors."""
     wrapper_class: type[BindableLogger] | None = field(default_factory=default_wrapper_class)  # pyright: ignore
     """Structlog bindable logger."""
     context_class: dict[str, Any] | None = None
     """Context class (a 'contextvar' context) for the logger."""
     logger_factory: Callable[..., WrappedLogger] | None = field(default_factory=default_logger_factory)
     """Logger factory to use."""
     cache_logger_on_first_use: bool = field(default=True)
     """Whether to cache the logger configuration and reuse."""
+    log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
+    """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
+    traceback_line_limit: int = field(default=20)
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
+    """Handler function for logging exceptions."""
+
+    def __post_init__(self) -> None:
+        if self.log_exceptions != "never" and self.exception_logging_handler is None:
+            self.exception_logging_handler = _default_exception_logging_handler_factory(
+                is_struct_logger=True, traceback_line_limit=self.traceback_line_limit
+            )
 
     def configure(self) -> GetLogger:
         """Return logger with the given configuration.
 
         Returns:
             A 'logging.getLogger' like function.
         """
         try:
             from structlog import configure, get_logger
 
             # we now configure structlog
-            configure(**{k: v for k, v in asdict(self).items() if k != "standard_lib_logging_config"})
+            configure(
+                **{
+                    k: v
+                    for k, v in asdict(self).items()
+                    if k
+                    not in (
+                        "standard_lib_logging_config",
+                        "log_exceptions",
+                        "traceback_line_limit",
+                        "exception_logging_handler",
+                    )
+                }
+            )
             return get_logger
         except ImportError as e:  # pragma: no cover
             raise MissingDependencyException("structlog is not installed") from e
```

### Comparing `starlite-2.0.0a1/starlite/config/openapi.py` & `starlite-2.0.0a2/starlite/openapi/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, fields
 from typing import TYPE_CHECKING, Literal, cast
 
-from pydantic_openapi_schema.v3_1_0 import (
+from starlite._openapi.utils import default_operation_id_creator
+from starlite.openapi.controller import OpenAPIController
+from starlite.openapi.spec import (
     Components,
     Contact,
     ExternalDocumentation,
     Info,
     License,
     OpenAPI,
     PathItem,
     Reference,
     SecurityRequirement,
     Server,
     Tag,
 )
 
-from starlite.openapi.controller import OpenAPIController
-from starlite.openapi.utils import default_operation_id_creator
+__all__ = ("OpenAPIConfig",)
+
 
 if TYPE_CHECKING:
     from starlite.types.callable_types import OperationIDCreator
 
 
 @dataclass
 class OpenAPIConfig:
     """Configuration for OpenAPI.
 
     To enable OpenAPI schema generation and serving, pass an instance of this class to the
-    :class:`Starlite <starlite.app.Starlite>` constructor using the 'openapi_config' kwargs.
+    :class:`Starlite <.app.Starlite>` constructor using the ``openapi_config`` kwargs.
     """
 
     title: str
     """Title of API documentation."""
     version: str
     """API version, e.g. '1.0.0'."""
 
@@ -41,92 +43,91 @@
     """Generate examples using the pydantic-factories library."""
     openapi_controller: type[OpenAPIController] = field(default_factory=lambda: OpenAPIController)
     """Controller for generating OpenAPI routes.
 
     Must be subclass of :class:`OpenAPIController <starlite.openapi.controller.OpenAPIController>`.
     """
     contact: Contact | None = field(default=None)
-    """API contact information, should be an :class:`Contact <pydantic_openapi_schema.v3_1_0.contact.Contact>` instance."""
+    """API contact information, should be an :class:`Contact <starlite.openapi.spec.contact.Contact>` instance."""
     description: str | None = field(default=None)
     """API description."""
     external_docs: ExternalDocumentation | None = field(default=None)
     """Links to external documentation.
 
-    Should be an instance of :class:`ExternalDocumentation <pydantic_openapi_schema.v3_1_0.external_documentation.ExternalDocumentation>`.
+    Should be an instance of :class:`ExternalDocumentation <starlite.openapi.spec.external_documentation.ExternalDocumentation>`.
     """
     license: License | None = field(default=None)
     """API Licensing information.
 
-    Should be an instance of :class:`License <pydantic_openapi_schema.v3_1_0.license.License>`.
+    Should be an instance of :class:`License <starlite.openapi.spec.license.License>`.
     """
     security: list[SecurityRequirement] | None = field(default=None)
     """API Security requirements information.
 
-    Should be an instance of :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>`.
+    Should be an instance of
+        :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`.
     """
     components: Components | list[Components] | None = field(default=None)
     """API Components information.
 
-    Should be an instance of :class:`Components <pydantic_openapi_schema.v3_10_0.components.Components>` or a list thereof.
+    Should be an instance of :class:`Components <starlite.openapi.spec.components.Components>` or a list thereof.
     """
     servers: list[Server] = field(default_factory=lambda: [Server(url="/")])
-    """A list of :class:`Server <pydantic_openapi_schema.v3_1_0.server.Server>` instances."""
+    """A list of :class:`Server <starlite.openapi.spec.server.Server>` instances."""
     summary: str | None = field(default=None)
     """A summary text."""
     tags: list[Tag] | None = field(default=None)
-    """A list of :class:`Tag <pydantic_openapi_schema.v3_1_0.tag.Tag>` instances."""
+    """A list of :class:`Tag <starlite.openapi.spec.tag.Tag>` instances."""
     terms_of_service: str | None = field(default=None)
     """URL to page that contains terms of service."""
     use_handler_docstrings: bool = field(default=False)
     """Draw operation description from route handler docstring if not otherwise provided."""
     webhooks: dict[str, PathItem | Reference] | None = field(default=None)
-    """A mapping of key to either :class:`PathItem <pydantic_openapi_schema.v3_1_0.path_item.PathItem>` or.
+    """A mapping of key to either :class:`PathItem <starlite.openapi.spec.path_item.PathItem>` or.
 
-    :class:`Reference <pydantic_openapi_schema.v3_1_0.reference.Reference>` objects.
+    :class:`Reference <starlite.openapi.spec.reference.Reference>` objects.
     """
     root_schema_site: Literal["redoc", "swagger", "elements"] = "redoc"
     """The static schema generator to use for the "root" path of `/schema/`."""
     enabled_endpoints: set[str] = field(
         default_factory=lambda: {"redoc", "swagger", "elements", "openapi.json", "openapi.yaml"}
     )
     """A set of the enabled documentation sites and schema download endpoints."""
-    by_alias: bool = True
-    """Render pydantic model schema using field aliases, if defined."""
     operation_id_creator: OperationIDCreator = default_operation_id_creator
     """A callable that generates unique operation ids"""
 
     def to_openapi_schema(self) -> OpenAPI:
         """Return an ``OpenAPI`` instance from the values stored in ``self``.
 
         Returns:
-            An instance of :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.open_api.OpenAPI>`.
+            An instance of :class:`OpenAPI <starlite.openapi.spec.open_api.OpenAPI>`.
         """
 
         if isinstance(self.components, list):
             merged_components = Components()
             for components in self.components:
-                for key in components.__fields__:
-                    value = getattr(components, key, None)
-                    if value:
+                for key in (f.name for f in fields(components)):
+                    if value := getattr(components, key, None):
                         merged_value_dict = getattr(merged_components, key, {}) or {}
                         merged_value_dict.update(value)
                         setattr(merged_components, key, merged_value_dict)
+
             self.components = merged_components
 
         return OpenAPI(
-            externalDocs=self.external_docs,
+            external_docs=self.external_docs,
             security=self.security,
             components=cast("Components", self.components),
             servers=self.servers,
             tags=self.tags,
             webhooks=self.webhooks,
             info=Info(
                 title=self.title,
                 version=self.version,
                 description=self.description,
                 contact=self.contact,
                 license=self.license,
                 summary=self.summary,
-                termsOfService=self.terms_of_service,  # type: ignore
+                terms_of_service=self.terms_of_service,
             ),
             paths={},
         )
```

### Comparing `starlite-2.0.0a1/starlite/config/static_files.py` & `starlite-2.0.0a2/starlite/static_files/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.file_system import BaseLocalFileSystem
 from starlite.handlers import asgi
 from starlite.static_files.base import StaticFiles
 from starlite.utils import normalize_path
 
+__all__ = ("StaticFilesConfig",)
+
+
 if TYPE_CHECKING:
     from starlite.handlers.asgi_handlers import ASGIRouteHandler
     from starlite.types import ExceptionHandlersMap, Guard, PathType
 
 
 @dataclass
 class StaticFilesConfig:
```

### Comparing `starlite-2.0.0a1/starlite/config/template.py` & `starlite-2.0.0a2/starlite/template/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from functools import cached_property
 from inspect import isclass
-from typing import Callable, Generic, TypeVar, cast
+from typing import TYPE_CHECKING, Callable, Generic, TypeVar, cast
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.template import TemplateEngineProtocol
-from starlite.types import PathType
+
+__all__ = ("TemplateConfig",)
+
+if TYPE_CHECKING:
+    from starlite.types import PathType
 
 T = TypeVar("T", bound=TemplateEngineProtocol)
 
 
 @dataclass
 class TemplateConfig(Generic[T]):
     """Configuration for Templating.
```

### Comparing `starlite-2.0.0a1/starlite/connection/__init__.py` & `starlite-2.0.0a2/starlite/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/connection/base.py` & `starlite-2.0.0a2/starlite/connection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, cast
 
+from starlite._parsers import parse_cookie_string, parse_headers, parse_query_string
 from starlite.datastructures.headers import Headers
 from starlite.datastructures.multi_dicts import MultiDict
 from starlite.datastructures.state import State
 from starlite.datastructures.url import URL, Address, make_absolute_url
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.parsers import parse_cookie_string, parse_headers, parse_query_string
 from starlite.types.empty import Empty
 
+__all__ = ("ASGIConnection", "empty_receive", "empty_send")
+
+
 if TYPE_CHECKING:
     from typing import NoReturn
 
     from pydantic import BaseModel
 
     from starlite.app import Starlite
-    from starlite.cache import Cache
     from starlite.types import EmptyType
     from starlite.types.asgi_types import Message, Receive, Scope, Send
     from starlite.types.protocols import Logger
 
 UserT = TypeVar("UserT")
 AuthT = TypeVar("AuthT")
 HandlerT = TypeVar("HandlerT")
@@ -112,15 +114,15 @@
     def url(self) -> URL:
         """Return the URL of this connection's ``Scope``.
 
         Returns:
             A URL instance constructed from the request's scope.
         """
         if self._url is Empty:
-            self._url = self.scope["_url"] = URL.from_scope(self.scope)  # type: ignore[typeddict-item]
+            self._url = self.scope["_url"] = URL.from_scope(self.scope)  # type: ignore[typeddict-unknown-key]
 
         return cast("URL", self._url)
 
     @property
     def base_url(self) -> URL:
         """Return the base URL of this connection's ``Scope``.
 
@@ -131,28 +133,28 @@
         if self._base_url is Empty:
             scope = {
                 **self.scope,
                 "path": "/",
                 "query_string": b"",
                 "root_path": self.scope.get("app_root_path") or self.scope.get("root_path", ""),
             }
-            self._base_url = self.scope["_base_url"] = URL.from_scope(cast("Scope", scope))  # type: ignore[typeddict-item]
+            self._base_url = self.scope["_base_url"] = URL.from_scope(cast("Scope", scope))  # type: ignore[typeddict-unknown-key]
 
         return cast("URL", self._base_url)
 
     @property
     def headers(self) -> Headers:
         """Return the headers of this connection's ``Scope``.
 
         Returns:
             A Headers instance with the request's scope["headers"] value.
         """
         if self._headers is Empty:
             self.scope.setdefault("headers", [])
-            self._headers = self.scope["_headers"] = parse_headers(tuple(self.scope["headers"]))  # type: ignore[typeddict-item]
+            self._headers = self.scope["_headers"] = parse_headers(tuple(self.scope["headers"]))  # type: ignore[typeddict-unknown-key]
 
         return Headers(self._headers)
 
     @property
     def query_params(self) -> MultiDict:
         """Return the query parameters of this connection's ``Scope``.
 
@@ -183,15 +185,15 @@
         if self._cookies is Empty:
             cookies: dict[str, str] = {}
             cookie_header = self.headers.get("cookie")
 
             if cookie_header:
                 cookies = parse_cookie_string(cookie_header)
 
-            self._cookies = self.scope["_cookies"] = cookies  # type: ignore[typeddict-item]
+            self._cookies = self.scope["_cookies"] = cookies  # type: ignore[typeddict-unknown-key]
 
         return cast("dict[str, str]", self._cookies)
 
     @property
     def client(self) -> Address | None:
         """Return the ``client`` data of this connection's ``Scope``.
 
@@ -256,42 +258,33 @@
             A ``Logger`` instance.
 
         Raises:
             ImproperlyConfiguredException: if ``log_config`` has not been passed to the Starlite constructor.
         """
         return self.app.get_logger()
 
-    @property
-    def cache(self) -> Cache:
-        """Return the ``Cache`` for this connection.
-
-        Returns:
-            A ``Cache`` instance.
-        """
-        return self.app.cache
-
     def set_session(self, value: dict[str, Any] | BaseModel | EmptyType) -> None:
         """Set the session in the connection's ``Scope``.
 
-        If the :class:`Starlite SessionMiddleware <starlite.middleware.session.SessionMiddleware>` is
-        enabled, the session will be added to the response as a cookie header.
+        If the :class:`SessionMiddleware <.middleware.session.base.SessionMiddleware>` is enabled, the session will be added
+        to the response as a cookie header.
 
         Args:
             value: Dictionary or pydantic model instance for the session data.
 
         Returns:
             None.
         """
         self.scope["session"] = value
 
     def clear_session(self) -> None:
         """Remove the session from the connection's ``Scope``.
 
-        If the :class:`Starlite SessionMiddleware <starlite.middleware.session.SessionMiddleware>` is
-        enabled, this will cause the session data to be cleared.
+        If the :class:`Starlite SessionMiddleware <.middleware.session.base.SessionMiddleware>` is enabled, this will cause
+        the session data to be cleared.
 
         Returns:
             None.
         """
         self.scope["session"] = Empty
 
     def url_for(self, name: str, **path_parameters: dict[str, Any]) -> str:
```

### Comparing `starlite-2.0.0a1/starlite/connection/request.py` & `starlite-2.0.0a2/starlite/connection/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Generic, cast
 
+from starlite._multipart import parse_content_header, parse_multipart_form
+from starlite._parsers import parse_url_encoded_form_data
 from starlite.connection.base import (
     ASGIConnection,
     AuthT,
     StateT,
     UserT,
     empty_receive,
     empty_send,
 )
 from starlite.datastructures.multi_dicts import FormMultiDict
 from starlite.enums import RequestEncodingType
 from starlite.exceptions import InternalServerException
-from starlite.multipart import parse_content_header, parse_multipart_form
-from starlite.parsers import parse_url_encoded_form_data
 from starlite.serialization import decode_json, decode_msgpack
 from starlite.types import Empty
 
+__all__ = ("Request",)
+
+
 if TYPE_CHECKING:
     from starlite.handlers.http_handlers import HTTPRouteHandler  # noqa: F401
     from starlite.types.asgi_types import HTTPScope, Method, Receive, Scope, Send
 
 
 SERVER_PUSH_HEADERS = {
     "accept",
@@ -73,37 +76,37 @@
     def content_type(self) -> tuple[str, dict[str, str]]:
         """Parse the request's 'Content-Type' header, returning the header value and any options as a dictionary.
 
         Returns:
             A tuple with the parsed value and a dictionary containing any options send in it.
         """
         if self._content_type is Empty:
-            self._content_type = self.scope["_content_type"] = parse_content_header(self.headers.get("Content-Type", ""))  # type: ignore[typeddict-item]
+            self._content_type = self.scope["_content_type"] = parse_content_header(self.headers.get("Content-Type", ""))  # type: ignore[typeddict-unknown-key]
         return cast("tuple[str, dict[str, str]]", self._content_type)
 
     async def json(self) -> Any:
         """Retrieve the json request body from the request.
 
         Returns:
             An arbitrary value
         """
         if self._json is Empty:
             body = await self.body()
-            self._json = self.scope["_json"] = decode_json(body or b"null")  # type: ignore[typeddict-item]
+            self._json = self.scope["_json"] = decode_json(body or b"null")  # type: ignore[typeddict-unknown-key]
         return self._json
 
     async def msgpack(self) -> Any:
         """Retrieve the MessagePack request body from the request.
 
         Returns:
             An arbitrary value
         """
         if self._msgpack is Empty:
             body = await self.body()
-            self._msgpack = self.scope["_msgpack"] = decode_msgpack(body or b"\xc0")  # type: ignore[typeddict-item]
+            self._msgpack = self.scope["_msgpack"] = decode_msgpack(body or b"\xc0")  # type: ignore[typeddict-unknown-key]
         return self._msgpack
 
     async def stream(self) -> AsyncGenerator[bytes, None]:
         """Return an async generator that streams chunks of bytes.
 
         Returns:
             An async generator.
@@ -137,36 +140,36 @@
     async def body(self) -> bytes:
         """Return the body of the request.
 
         Returns:
             A byte-string representing the body of the request.
         """
         if self._body is Empty:
-            self._body = self.scope["_body"] = b"".join([c async for c in self.stream()])  # type: ignore[typeddict-item]
+            self._body = self.scope["_body"] = b"".join([c async for c in self.stream()])  # type: ignore[typeddict-unknown-key]
         return cast("bytes", self._body)
 
     async def form(self) -> FormMultiDict:
         """Retrieve form data from the request. If the request is either a 'multipart/form-data' or an
         'application/x-www-form- urlencoded', return a FormMultiDict instance populated with the values sent in the
         request, otherwise, an empty instance.
 
         Returns:
             A FormMultiDict instance
         """
         if self._form is Empty:
             content_type, options = self.content_type
             if content_type == RequestEncodingType.MULTI_PART:
-                self._form = self.scope["_form"] = form_values = parse_multipart_form(  # type: ignore[typeddict-item]
+                self._form = self.scope["_form"] = form_values = parse_multipart_form(  # type: ignore[typeddict-unknown-key]
                     body=await self.body(),
                     boundary=options.get("boundary", "").encode(),
                     multipart_form_part_limit=self.app.multipart_form_part_limit,
                 )
                 return FormMultiDict(form_values)
             if content_type == RequestEncodingType.URL_ENCODED:
-                self._form = self.scope["_form"] = form_values = parse_url_encoded_form_data(  # type: ignore[typeddict-item]
+                self._form = self.scope["_form"] = form_values = parse_url_encoded_form_data(  # type: ignore[typeddict-unknown-key]
                     await self.body(),
                 )
                 return FormMultiDict(form_values)
             return FormMultiDict()
         return FormMultiDict(self._form)
 
     async def send_push_promise(self, path: str) -> None:
```

### Comparing `starlite-2.0.0a1/starlite/connection/websocket.py` & `starlite-2.0.0a2/starlite/connection/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,29 @@
     empty_send,
 )
 from starlite.datastructures.headers import Headers
 from starlite.exceptions import WebSocketDisconnect, WebSocketException
 from starlite.serialization import decode_json, default_serializer, encode_json
 from starlite.status_codes import WS_1000_NORMAL_CLOSURE
 
+__all__ = ("WebSocket",)
+
+
 if TYPE_CHECKING:
     from starlite.handlers.websocket_handlers import WebsocketRouteHandler  # noqa: F401
     from starlite.types import Message, Serializer, WebSocketScope
-    from starlite.types.asgi_types import WebSocketDisconnectEvent  # nopycln: import
-    from starlite.types.asgi_types import WebSocketReceiveEvent  # nopycln: import
     from starlite.types.asgi_types import (
         Receive,
         ReceiveMessage,
         Scope,
         Send,
         WebSocketAcceptEvent,
         WebSocketCloseEvent,
+        WebSocketDisconnectEvent,
+        WebSocketReceiveEvent,
         WebSocketSendEvent,
     )
 
 DISCONNECT_MESSAGE = "connection is disconnected"
 
 
 class WebSocket(Generic[UserT, AuthT, StateT], ASGIConnection["WebsocketRouteHandler", UserT, AuthT, StateT]):
```

### Comparing `starlite-2.0.0a1/starlite/constants.py` & `starlite-2.0.0a2/starlite/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from inspect import Signature
 
-from msgspec.inspect import UNSET
 from pydantic.fields import Undefined
 
 from starlite.types import Empty
 
 DEFAULT_ALLOWED_CORS_HEADERS = {"Accept", "Accept-Language", "Content-Language", "Content-Type"}
 DEFAULT_CHUNK_SIZE = 1024 * 128  # 128KB
 HTTP_RESPONSE_BODY = "http.response.body"
 HTTP_RESPONSE_START = "http.response.start"
 ONE_MEGABYTE = 1024 * 1024
 REDIRECT_STATUS_CODES = {301, 302, 303, 307, 308}
 RESERVED_KWARGS = {"state", "headers", "cookies", "request", "socket", "data", "query", "scope", "body"}
 SCOPE_STATE_DEPENDENCY_CACHE = "dependency_cache"
 SCOPE_STATE_NAMESPACE = "__starlite__"
 SCOPE_STATE_RESPONSE_COMPRESSED = "response_compressed"
-UNDEFINED_SENTINELS = {Undefined, Signature.empty, UNSET, Empty, Ellipsis}
+UNDEFINED_SENTINELS = {Undefined, Signature.empty, Empty, Ellipsis}
 SKIP_VALIDATION_NAMES = {"request", "socket", "scope", "receive", "send"}
```

### Comparing `starlite-2.0.0a1/starlite/contrib/htmx/request.py` & `starlite-2.0.0a2/starlite/contrib/htmx/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,113 @@
-from __future__ import annotations
-
-from functools import cached_property
-from typing import TYPE_CHECKING, Any
-from urllib.parse import unquote, urlsplit, urlunsplit
-
-from starlite import Request
-from starlite.contrib.htmx.utils import HTMXHeaders
-from starlite.exceptions import SerializationException
-from starlite.serialization import decode_json
-
-if TYPE_CHECKING:
-    from starlite.types import Receive, Scope, Send
-
-
-class HTMXDetails:
-    """HTMXDetails holds all the values sent by HTMX client in headers
-    and provide convenient properties.
-    """
-
-    def __init__(self, request: Request) -> None:
-        """Initialize :class:`HTMXDetails`"""
-        self.request = request
-
-    def _get_header_value(self, name: str) -> str | None:
-        """Parse request header
-
-        Check for uri encoded header and unquotes it in readable format.
-        """
-        value = self.request.headers.get(name) or None
-        if value and self.request.headers.get(name + "-URI-AutoEncoded") == "true":
-            return unquote(value)
-        return value
-
-    def __bool__(self) -> bool:
-        """Check if request is sent by an HTMX client."""
-        return self._get_header_value(HTMXHeaders.REQUEST) == "true"
-
-    @cached_property
-    def boosted(self) -> bool:
-        """Check if request is boosted."""
-        return self._get_header_value(HTMXHeaders.BOOSTED) == "true"
-
-    @cached_property
-    def current_url(self) -> str | None:
-        """Current url value sent by HTMX client."""
-        return self._get_header_value(HTMXHeaders.CURRENT_URL)
-
-    @cached_property
-    def current_url_abs_path(self) -> str | None:
-        """Current url abs path value, to get query and path parameter sent by HTMX client."""
-        if self.current_url:
-            split = urlsplit(self.current_url)
-            if split.scheme == self.request.scope["scheme"] and split.netloc == self.request.headers.get("host"):
-                return str(urlunsplit(split._replace(scheme="", netloc="")))
-            return None
-        return self.current_url
-
-    @cached_property
-    def history_restore_request(self) -> bool:
-        """If True then, request is for history restoration after a miss in the local history cache."""
-        return self._get_header_value(HTMXHeaders.HISTORY_RESTORE_REQUEST) == "true"
-
-    @cached_property
-    def prompt(self) -> str | None:
-        """User Response to prompt.
-
-        .. code-block:: html
-
-            <button hx-delete="/account" hx-prompt="Enter your account name to confirm deletion">Delete My Account</button>
-        """
-        return self._get_header_value(HTMXHeaders.PROMPT)
-
-    @cached_property
-    def target(self) -> str | None:
-        """ID of the target element if provided on the element."""
-        return self._get_header_value(HTMXHeaders.TARGET)
-
-    @cached_property
-    def trigger(self) -> str | None:
-        """ID of the triggered element if provided on the element."""
-        return self._get_header_value(HTMXHeaders.TRIGGER_ID)
-
-    @cached_property
-    def trigger_name(self) -> str | None:
-        """Name of the triggered element if provided on the element."""
-        return self._get_header_value(HTMXHeaders.TRIGGER_NAME)
-
-    @cached_property
-    def triggering_event(self) -> Any:
-        """Name of the triggered event.
-
-        This value is added by ``event-header`` extension of HTMX to the ``Triggering-Event`` header to requests.
-        """
-        value = self._get_header_value(HTMXHeaders.TRIGGERING_EVENT)
-        if value is not None:
-            try:
-                value = decode_json(value)
-            except SerializationException:
-                value = None
-        return value
-
-
-class HTMXRequest(Request):
-    """HTMX Request class to work with HTMX client."""
-
-    __slots__ = ("htmx",)
-
-    def __init__(self, scope: Scope, receive: Receive, send: Send):
-        """Initialize :class:`HTMXRequest`"""
-        super().__init__(scope=scope, receive=receive, send=send)
-        self.htmx = HTMXDetails(self)
+from __future__ import annotations
+
+from functools import cached_property
+from typing import TYPE_CHECKING, Any
+from urllib.parse import unquote, urlsplit, urlunsplit
+
+from starlite import Request
+from starlite.contrib.htmx._utils import HTMXHeaders
+from starlite.exceptions import SerializationException
+from starlite.serialization import decode_json
+
+__all__ = ("HTMXDetails", "HTMXRequest")
+
+
+if TYPE_CHECKING:
+    from starlite.types import Receive, Scope, Send
+
+
+class HTMXDetails:
+    """HTMXDetails holds all the values sent by HTMX client in headers and provide convenient properties."""
+
+    def __init__(self, request: Request) -> None:
+        """Initialize :class:`HTMXDetails`"""
+        self.request = request
+
+    def _get_header_value(self, name: str) -> str | None:
+        """Parse request header
+
+        Check for uri encoded header and unquotes it in readable format.
+        """
+        value = self.request.headers.get(name) or None
+        if value and self.request.headers.get(name + "-URI-AutoEncoded") == "true":
+            return unquote(value)
+        return value
+
+    def __bool__(self) -> bool:
+        """Check if request is sent by an HTMX client."""
+        return self._get_header_value(HTMXHeaders.REQUEST) == "true"
+
+    @cached_property
+    def boosted(self) -> bool:
+        """Check if request is boosted."""
+        return self._get_header_value(HTMXHeaders.BOOSTED) == "true"
+
+    @cached_property
+    def current_url(self) -> str | None:
+        """Current url value sent by HTMX client."""
+        return self._get_header_value(HTMXHeaders.CURRENT_URL)
+
+    @cached_property
+    def current_url_abs_path(self) -> str | None:
+        """Current url abs path value, to get query and path parameter sent by HTMX client."""
+        if self.current_url:
+            split = urlsplit(self.current_url)
+            if split.scheme == self.request.scope["scheme"] and split.netloc == self.request.headers.get("host"):
+                return str(urlunsplit(split._replace(scheme="", netloc="")))
+            return None
+        return self.current_url
+
+    @cached_property
+    def history_restore_request(self) -> bool:
+        """If True then, request is for history restoration after a miss in the local history cache."""
+        return self._get_header_value(HTMXHeaders.HISTORY_RESTORE_REQUEST) == "true"
+
+    @cached_property
+    def prompt(self) -> str | None:
+        """User Response to prompt.
+
+        .. code-block:: html
+
+            <button hx-delete="/account" hx-prompt="Enter your account name to confirm deletion">Delete My Account</button>
+        """
+        return self._get_header_value(HTMXHeaders.PROMPT)
+
+    @cached_property
+    def target(self) -> str | None:
+        """ID of the target element if provided on the element."""
+        return self._get_header_value(HTMXHeaders.TARGET)
+
+    @cached_property
+    def trigger(self) -> str | None:
+        """ID of the triggered element if provided on the element."""
+        return self._get_header_value(HTMXHeaders.TRIGGER_ID)
+
+    @cached_property
+    def trigger_name(self) -> str | None:
+        """Name of the triggered element if provided on the element."""
+        return self._get_header_value(HTMXHeaders.TRIGGER_NAME)
+
+    @cached_property
+    def triggering_event(self) -> Any:
+        """Name of the triggered event.
+
+        This value is added by ``event-header`` extension of HTMX to the ``Triggering-Event`` header to requests.
+        """
+        value = self._get_header_value(HTMXHeaders.TRIGGERING_EVENT)
+        if value is not None:
+            try:
+                value = decode_json(value)
+            except SerializationException:
+                value = None
+        return value
+
+
+class HTMXRequest(Request):
+    """HTMX Request class to work with HTMX client."""
+
+    __slots__ = ("htmx",)
+
+    def __init__(self, scope: Scope, receive: Receive, send: Send):
+        """Initialize :class:`HTMXRequest`"""
+        super().__init__(scope=scope, receive=receive, send=send)
+        self.htmx = HTMXDetails(self)
```

### Comparing `starlite-2.0.0a1/starlite/contrib/htmx/response.py` & `starlite-2.0.0a2/starlite/contrib/htmx/response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,230 +1,241 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import Any, Generic, TypeVar
-from urllib.parse import quote
-
-from starlite import MediaType, Request, Response, Starlite
-from starlite.background_tasks import BackgroundTask, BackgroundTasks
-from starlite.contrib.htmx.types import (
-    EventAfterType,
-    HtmxHeaderType,
-    LocationType,
-    PushUrlType,
-    ReSwapMethod,
-    TriggerEventType,
-)
-from starlite.contrib.htmx.utils import HTMX_STOP_POLLING, get_headers
-from starlite.datastructures import Cookie
-from starlite.response import TemplateResponse
-from starlite.response_containers import ResponseContainer, Template
-from starlite.status_codes import HTTP_200_OK
-
-# HTMX defined HTTP status code.
-# Response carrying this status code will ask client to stop Polling.
-T = TypeVar("T")
-
-
-class HXStopPolling(Response):
-    """Stop HTMX client from Polling."""
-
-    def __init__(self) -> None:
-        """Initialize"""
-        super().__init__(content=None)
-        self.status_code = HTMX_STOP_POLLING
-
-
-class ClientRedirect(Response):
-    """HTMX Response class to support client side redirect."""
-
-    def __init__(self, redirect_to: str) -> None:
-        """Set status code to 200 (required by HTMX), and pass redirect url."""
-        super().__init__(content=None, headers=get_headers(hx_headers=HtmxHeaderType(redirect=redirect_to)))
-        del self.headers["Location"]
-
-
-class ClientRefresh(Response):
-    """Response to support HTMX client page refresh"""
-
-    def __init__(self) -> None:
-        """Set Status code to 200 and set headers."""
-        super().__init__(content=None, headers=get_headers(hx_headers=HtmxHeaderType(refresh=True)))
-
-
-class PushUrl(Generic[T], Response[T]):
-    """Response to push new url into the history stack."""
-
-    def __init__(self, content: T, push_url: PushUrlType, **kwargs: Any) -> None:
-        """Initialize PushUrl."""
-        super().__init__(
-            content=content,
-            status_code=HTTP_200_OK,
-            headers=get_headers(hx_headers=HtmxHeaderType(push_url=push_url)),
-            **kwargs,
-        )
-
-
-class ReplaceUrl(Generic[T], Response[T]):
-    """Response to replace url in the Browser Location bar."""
-
-    def __init__(self, content: T, replace_url: PushUrlType, **kwargs: Any) -> None:
-        """Initialize ReplaceUrl."""
-        super().__init__(
-            content=content,
-            status_code=HTTP_200_OK,
-            headers=get_headers(hx_headers=HtmxHeaderType(replace_url=replace_url)),
-            **kwargs,
-        )
-
-
-class Reswap(Generic[T], Response[T]):
-    """Response to specify how the response will be swapped."""
-
-    def __init__(
-        self,
-        content: T,
-        method: ReSwapMethod,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize Reswap."""
-        super().__init__(content=content, headers=get_headers(hx_headers=HtmxHeaderType(re_swap=method)), **kwargs)
-
-
-class Retarget(Generic[T], Response[T]):
-    """Response to target different element on the page."""
-
-    def __init__(self, content: T, target: str, **kwargs: Any) -> None:
-        """Initialize Retarget."""
-        super().__init__(content=content, headers=get_headers(hx_headers=HtmxHeaderType(re_target=target)), **kwargs)
-
-
-class TriggerEvent(Generic[T], Response[T]):
-    """Trigger Client side event."""
-
-    def __init__(
-        self,
-        content: T,
-        name: str,
-        after: EventAfterType,
-        params: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize TriggerEvent."""
-        event = TriggerEventType(name=name, params=params, after=after)
-        headers = get_headers(hx_headers=HtmxHeaderType(trigger_event=event))
-        super().__init__(content=content, headers=headers, **kwargs)
-
-
-class HXLocation(Response):
-    """Client side redirect without full page reload."""
-
-    def __init__(
-        self,
-        redirect_to: str,
-        source: str | None = None,
-        event: str | None = None,
-        target: str | None = None,
-        swap: ReSwapMethod = None,
-        hx_headers: dict[str, Any] | None = None,
-        values: dict[str, str] | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize HXLocation, Set status code to 200 (required by HTMX),
-        and pass redirect url.
-        """
-        super().__init__(
-            content=None,
-            headers={"Location": quote(redirect_to, safe="/#%[]=:;$&()+,!?*@'~")},
-            **kwargs,
-        )
-        spec: dict[str, Any] = get_headers(
-            hx_headers=HtmxHeaderType(
-                location=LocationType(
-                    path=str(self.headers.get("Location")),
-                    source=source,
-                    event=event,
-                    target=target,
-                    swap=swap,
-                    values=values,
-                    hx_headers=hx_headers,
-                )
-            )
-        )
-        del self.headers["Location"]
-        self.headers.update(spec)
-
-
-@dataclass
-class HTMXTemplate(ResponseContainer[TemplateResponse]):
-    """HTMX template wrapper"""
-
-    name: str
-    """Path-like name for the template to be rendered, e.g. "index.html"."""
-    context: dict[str, Any] = field(default_factory=dict)
-    """A dictionary of key/value pairs to be passed to the temple engine's render method.
-
-    Defaults to None.
-    """
-    background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
-
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
-    Defaults to None.
-    """
-    headers: dict[str, Any] = field(default_factory=dict)
-    """A string/string dictionary of response headers.
-
-    Header keys are insensitive. Defaults to None.
-    """
-    cookies: list[Cookie] = field(default_factory=list)
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
-
-    Defaults to None.
-    """
-    media_type: MediaType | str | None = field(default=None)
-    """If defined, overrides the media type configured in the route decorator."""
-    encoding: str = field(default="utf-8")
-    """The encoding to be used for the response headers."""
-    push_url: PushUrlType | None = field(default=None)
-    """Either a string value specifying a URL to push to browser history or ``False`` to
-    prevent HTMX client from pushing a url to browser history."""
-    re_swap: ReSwapMethod | None = field(default=None)
-    """Method value to instruct HTMX which swapping method to use."""
-    re_target: str | None = field(default=None)
-    """Value for 'id of target element' to apply changes to."""
-    trigger_event: str | None = field(default=None)
-    """Event name to trigger."""
-    params: dict[str, Any] | None = field(default=None)
-    """Dictionary of parameters if any required with trigger event parameter."""
-    after: EventAfterType | None = field(default=None)
-    """Changes to apply after ``receive``, ``settle`` or ``swap`` event."""
-
-    def to_response(
-        self,
-        headers: dict[str, Any],
-        media_type: MediaType | str,
-        status_code: int,
-        app: Starlite,
-        request: Request,
-    ) -> TemplateResponse:
-        """Add HTMX headers and return a :class:`.response.TemplateResponse`."""
-
-        event: TriggerEventType | None = None
-        if self.trigger_event:
-            event = TriggerEventType(name=str(self.trigger_event), params=self.params, after=self.after)
-
-        hx_headers: dict[str, Any] = get_headers(
-            hx_headers=HtmxHeaderType(
-                push_url=self.push_url, re_swap=self.re_swap, re_target=self.re_target, trigger_event=event
-            )
-        )
-
-        template = Template(
-            name=self.name,
-            background=self.background,
-            encoding=self.encoding,
-        )
-
-        return template.to_response(
-            headers=hx_headers, media_type=media_type, app=app, status_code=status_code, request=request
-        )
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from urllib.parse import quote
+
+from starlite import MediaType, Request, Response, Starlite
+from starlite.contrib.htmx._utils import HTMX_STOP_POLLING, get_headers
+from starlite.contrib.htmx.types import (
+    EventAfterType,
+    HtmxHeaderType,
+    LocationType,
+    PushUrlType,
+    ReSwapMethod,
+    TriggerEventType,
+)
+from starlite.response import TemplateResponse
+from starlite.response_containers import ResponseContainer, Template
+from starlite.status_codes import HTTP_200_OK
+
+__all__ = (
+    "ClientRedirect",
+    "ClientRefresh",
+    "HTMXTemplate",
+    "HXLocation",
+    "HXStopPolling",
+    "PushUrl",
+    "ReplaceUrl",
+    "Reswap",
+    "Retarget",
+    "TriggerEvent",
+)
+
+if TYPE_CHECKING:
+    from starlite.background_tasks import BackgroundTask, BackgroundTasks
+    from starlite.datastructures import Cookie
+
+
+# HTMX defined HTTP status code.
+# Response carrying this status code will ask client to stop Polling.
+T = TypeVar("T")
+
+
+class HXStopPolling(Response):
+    """Stop HTMX client from Polling."""
+
+    def __init__(self) -> None:
+        """Initialize"""
+        super().__init__(content=None)
+        self.status_code = HTMX_STOP_POLLING
+
+
+class ClientRedirect(Response):
+    """HTMX Response class to support client side redirect."""
+
+    def __init__(self, redirect_to: str) -> None:
+        """Set status code to 200 (required by HTMX), and pass redirect url."""
+        super().__init__(content=None, headers=get_headers(hx_headers=HtmxHeaderType(redirect=redirect_to)))
+        del self.headers["Location"]
+
+
+class ClientRefresh(Response):
+    """Response to support HTMX client page refresh"""
+
+    def __init__(self) -> None:
+        """Set Status code to 200 and set headers."""
+        super().__init__(content=None, headers=get_headers(hx_headers=HtmxHeaderType(refresh=True)))
+
+
+class PushUrl(Generic[T], Response[T]):
+    """Response to push new url into the history stack."""
+
+    def __init__(self, content: T, push_url: PushUrlType, **kwargs: Any) -> None:
+        """Initialize PushUrl."""
+        super().__init__(
+            content=content,
+            status_code=HTTP_200_OK,
+            headers=get_headers(hx_headers=HtmxHeaderType(push_url=push_url)),
+            **kwargs,
+        )
+
+
+class ReplaceUrl(Generic[T], Response[T]):
+    """Response to replace url in the Browser Location bar."""
+
+    def __init__(self, content: T, replace_url: PushUrlType, **kwargs: Any) -> None:
+        """Initialize ReplaceUrl."""
+        super().__init__(
+            content=content,
+            status_code=HTTP_200_OK,
+            headers=get_headers(hx_headers=HtmxHeaderType(replace_url=replace_url)),
+            **kwargs,
+        )
+
+
+class Reswap(Generic[T], Response[T]):
+    """Response to specify how the response will be swapped."""
+
+    def __init__(
+        self,
+        content: T,
+        method: ReSwapMethod,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize Reswap."""
+        super().__init__(content=content, headers=get_headers(hx_headers=HtmxHeaderType(re_swap=method)), **kwargs)
+
+
+class Retarget(Generic[T], Response[T]):
+    """Response to target different element on the page."""
+
+    def __init__(self, content: T, target: str, **kwargs: Any) -> None:
+        """Initialize Retarget."""
+        super().__init__(content=content, headers=get_headers(hx_headers=HtmxHeaderType(re_target=target)), **kwargs)
+
+
+class TriggerEvent(Generic[T], Response[T]):
+    """Trigger Client side event."""
+
+    def __init__(
+        self,
+        content: T,
+        name: str,
+        after: EventAfterType,
+        params: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize TriggerEvent."""
+        event = TriggerEventType(name=name, params=params, after=after)
+        headers = get_headers(hx_headers=HtmxHeaderType(trigger_event=event))
+        super().__init__(content=content, headers=headers, **kwargs)
+
+
+class HXLocation(Response):
+    """Client side redirect without full page reload."""
+
+    def __init__(
+        self,
+        redirect_to: str,
+        source: str | None = None,
+        event: str | None = None,
+        target: str | None = None,
+        swap: ReSwapMethod = None,
+        hx_headers: dict[str, Any] | None = None,
+        values: dict[str, str] | None = None,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize HXLocation, Set status code to 200 (required by HTMX),
+        and pass redirect url.
+        """
+        super().__init__(
+            content=None,
+            headers={"Location": quote(redirect_to, safe="/#%[]=:;$&()+,!?*@'~")},
+            **kwargs,
+        )
+        spec: dict[str, Any] = get_headers(
+            hx_headers=HtmxHeaderType(
+                location=LocationType(
+                    path=str(self.headers.get("Location")),
+                    source=source,
+                    event=event,
+                    target=target,
+                    swap=swap,
+                    values=values,
+                    hx_headers=hx_headers,
+                )
+            )
+        )
+        del self.headers["Location"]
+        self.headers.update(spec)
+
+
+@dataclass
+class HTMXTemplate(ResponseContainer[TemplateResponse]):
+    """HTMX template wrapper"""
+
+    name: str
+    """Path-like name for the template to be rendered, e.g. "index.html"."""
+    context: dict[str, Any] = field(default_factory=dict)
+    """A dictionary of key/value pairs to be passed to the temple engine's render method.
+
+    Defaults to None.
+    """
+    background: BackgroundTask | BackgroundTasks | None = field(default=None)
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished. Defaults to
+    ``None``.
+    """
+    headers: dict[str, Any] = field(default_factory=dict)
+    """A string/string dictionary of response headers.Header keys are insensitive. Defaults to ``None``."""
+    cookies: list[Cookie] = field(default_factory=list)
+    """A list of :class:`Cookies <.datastructures.Cookie>` to be set under the response ``Set-Cookie`` header. Defaults
+    to ``None``.
+    """
+    media_type: MediaType | str | None = field(default=None)
+    """If defined, overrides the media type configured in the route decorator."""
+    encoding: str = field(default="utf-8")
+    """The encoding to be used for the response headers."""
+    push_url: PushUrlType | None = field(default=None)
+    """Either a string value specifying a URL to push to browser history or ``False`` to prevent HTMX client from
+    pushing a url to browser history."""
+    re_swap: ReSwapMethod | None = field(default=None)
+    """Method value to instruct HTMX which swapping method to use."""
+    re_target: str | None = field(default=None)
+    """Value for 'id of target element' to apply changes to."""
+    trigger_event: str | None = field(default=None)
+    """Event name to trigger."""
+    params: dict[str, Any] | None = field(default=None)
+    """Dictionary of parameters if any required with trigger event parameter."""
+    after: EventAfterType | None = field(default=None)
+    """Changes to apply after ``receive``, ``settle`` or ``swap`` event."""
+
+    def to_response(
+        self,
+        headers: dict[str, Any],
+        media_type: MediaType | str,
+        status_code: int,
+        app: Starlite,
+        request: Request,
+    ) -> TemplateResponse:
+        """Add HTMX headers and return a :class:`TemplateResponse <.response.TemplateResponse>`."""
+
+        event: TriggerEventType | None = None
+        if self.trigger_event:
+            event = TriggerEventType(name=str(self.trigger_event), params=self.params, after=self.after)
+
+        hx_headers: dict[str, Any] = get_headers(
+            hx_headers=HtmxHeaderType(
+                push_url=self.push_url, re_swap=self.re_swap, re_target=self.re_target, trigger_event=event
+            )
+        )
+
+        template = Template(
+            name=self.name,
+            background=self.background,
+            encoding=self.encoding,
+        )
+
+        return template.to_response(
+            headers=hx_headers, media_type=media_type, app=app, status_code=status_code, request=request
+        )
```

### Comparing `starlite-2.0.0a1/starlite/contrib/htmx/utils.py` & `starlite-2.0.0a2/starlite/contrib/htmx/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,145 +1,156 @@
-from __future__ import annotations
-
-from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable
-from urllib.parse import quote
-
-from starlite.exceptions import ImproperlyConfiguredException
-from starlite.serialization import encode_json
-
-if TYPE_CHECKING:
-    from starlite.contrib.htmx.types import (
-        EventAfterType,
-        HtmxHeaderType,
-        LocationType,
-        PushUrlType,
-        ReSwapMethod,
-        TriggerEventType,
-    )
-
-HTMX_STOP_POLLING = 286
-
-
-class HTMXHeaders(str, Enum):
-    """Enum for HTMX Headers"""
-
-    REDIRECT = "HX-Redirect"
-    REFRESH = "HX-Refresh"
-    PUSH_URL = "HX-Push-Url"
-    REPLACE_URL = "HX-Replace-Url"
-    RE_SWAP = "HX-Reswap"
-    RE_TARGET = "HX-Retarget"
-    LOCATION = "HX-Location"
-
-    TRIGGER_EVENT = "HX-Trigger"
-    TRIGGER_AFTER_SETTLE = "HX-Trigger-After-Settle"
-    TRIGGER_AFTER_SWAP = "HX-Trigger-After-Swap"
-
-    REQUEST = "HX-Request"
-    BOOSTED = "HX-Boosted"
-    CURRENT_URL = "HX-Current-URL"
-    HISTORY_RESTORE_REQUEST = "HX-History-Restore-Request"
-    PROMPT = "HX-Prompt"
-    TARGET = "HX-Target"
-    TRIGGER_ID = "HX-Trigger"
-    TRIGGER_NAME = "HX-Trigger-Name"
-    TRIGGERING_EVENT = "Triggering-Event"
-
-
-def get_trigger_event_headers(trigger_event: TriggerEventType) -> dict[str, Any]:
-    """Return headers for trigger event response."""
-    params = trigger_event["params"] or {}
-    after_params: dict[EventAfterType, str] = {
-        "receive": HTMXHeaders.TRIGGER_EVENT.value,
-        "settle": HTMXHeaders.TRIGGER_AFTER_SETTLE.value,
-        "swap": HTMXHeaders.TRIGGER_AFTER_SWAP.value,
-    }
-
-    if trigger_header := after_params.get(trigger_event["after"]):
-        return {trigger_header: encode_json({trigger_event["name"]: params}).decode()}
-
-    raise ImproperlyConfiguredException(
-        "invalid value for 'after' param- allowed values are 'receive', 'settle' or 'swap'."
-    )
-
-
-def get_redirect_header(url: str) -> dict[str, Any]:
-    """Return headers for redirect response."""
-    return {HTMXHeaders.REDIRECT.value: quote(url, safe="/#%[]=:;$&()+,!?*@'~"), "Location": ""}
-
-
-def get_push_url_header(url: PushUrlType) -> dict[str, Any]:
-    """Return headers for push url to browser history response."""
-    if isinstance(url, str):
-        url = url if url != "False" else "false"
-    elif isinstance(url, bool):
-        url = "false"
-
-    return {HTMXHeaders.PUSH_URL.value: url}
-
-
-def get_replace_url_header(url: PushUrlType) -> dict[str, Any]:
-    """Return headers for replace url in browser tab response."""
-    if isinstance(url, str):
-        url = url if url != "False" else "false"
-    else:
-        url = "false"
-    return {HTMXHeaders.REPLACE_URL: url}
-
-
-def get_refresh_header(refresh: bool) -> dict[str, Any]:
-    """Return headers for client refresh response."""
-    value = ""
-    if refresh:
-        value = "true"
-    return {HTMXHeaders.REFRESH.value: value}
-
-
-def get_reswap_header(method: ReSwapMethod) -> dict[str, Any]:
-    """Return headers for change swap method response."""
-    return {HTMXHeaders.RE_SWAP.value: method}
-
-
-def get_retarget_header(target: str) -> dict[str, Any]:
-    """Return headers for change target element response."""
-    return {HTMXHeaders.RE_TARGET.value: target}
-
-
-def get_location_headers(location: LocationType) -> dict[str, Any]:
-    """Return headers for redirect without page-reload response."""
-    spec: dict[str, Any] = {}
-    for key, value in location.items():
-        if value:
-            spec[key] = value
-    if not spec:
-        raise ValueError("redirect_to is required parameter.")
-    return {HTMXHeaders.LOCATION.value: encode_json(spec).decode()}
-
-
-def get_headers(hx_headers: HtmxHeaderType) -> dict[str, Any]:
-    """Return headers for HTMX responses."""
-    if not hx_headers:
-        raise ValueError("Value for hx_headers cannot be None.")
-    htmx_headers_dict: dict[str, Callable] = {
-        "redirect": get_redirect_header,
-        "refresh": get_refresh_header,
-        "push_url": get_push_url_header,
-        "replace_url": get_replace_url_header,
-        "re_swap": get_reswap_header,
-        "re_target": get_retarget_header,
-        "trigger_event": get_trigger_event_headers,
-        "location": get_location_headers,
-    }
-
-    header: dict[str, Any] = {}
-    response: dict[str, Any]
-    key: str
-    value: Any
-    for key, value in hx_headers.items():
-        if key in ["redirect", "refresh", "location", "replace_url"]:
-            response = htmx_headers_dict[key](value)
-            return response
-        if value is not None:
-            response = htmx_headers_dict[key](value)
-            header.update(response)
-    return header
+from __future__ import annotations
+
+from enum import Enum
+from typing import TYPE_CHECKING, Any, Callable
+from urllib.parse import quote
+
+from starlite.exceptions import ImproperlyConfiguredException
+from starlite.serialization import encode_json
+
+__all__ = (
+    "HTMXHeaders",
+    "get_headers",
+    "get_location_headers",
+    "get_push_url_header",
+    "get_redirect_header",
+    "get_refresh_header",
+    "get_replace_url_header",
+    "get_reswap_header",
+    "get_retarget_header",
+    "get_trigger_event_headers",
+)
+
+
+if TYPE_CHECKING:
+    from starlite.contrib.htmx.types import (
+        EventAfterType,
+        HtmxHeaderType,
+        LocationType,
+        PushUrlType,
+        ReSwapMethod,
+        TriggerEventType,
+    )
+
+HTMX_STOP_POLLING = 286
+
+
+class HTMXHeaders(str, Enum):
+    """Enum for HTMX Headers"""
+
+    REDIRECT = "HX-Redirect"
+    REFRESH = "HX-Refresh"
+    PUSH_URL = "HX-Push-Url"
+    REPLACE_URL = "HX-Replace-Url"
+    RE_SWAP = "HX-Reswap"
+    RE_TARGET = "HX-Retarget"
+    LOCATION = "HX-Location"
+
+    TRIGGER_EVENT = "HX-Trigger"
+    TRIGGER_AFTER_SETTLE = "HX-Trigger-After-Settle"
+    TRIGGER_AFTER_SWAP = "HX-Trigger-After-Swap"
+
+    REQUEST = "HX-Request"
+    BOOSTED = "HX-Boosted"
+    CURRENT_URL = "HX-Current-URL"
+    HISTORY_RESTORE_REQUEST = "HX-History-Restore-Request"
+    PROMPT = "HX-Prompt"
+    TARGET = "HX-Target"
+    TRIGGER_ID = "HX-Trigger"  # noqa: PIE796
+    TRIGGER_NAME = "HX-Trigger-Name"
+    TRIGGERING_EVENT = "Triggering-Event"
+
+
+def get_trigger_event_headers(trigger_event: TriggerEventType) -> dict[str, Any]:
+    """Return headers for trigger event response."""
+    params = trigger_event["params"] or {}
+    after_params: dict[EventAfterType, str] = {
+        "receive": HTMXHeaders.TRIGGER_EVENT.value,
+        "settle": HTMXHeaders.TRIGGER_AFTER_SETTLE.value,
+        "swap": HTMXHeaders.TRIGGER_AFTER_SWAP.value,
+    }
+
+    if trigger_header := after_params.get(trigger_event["after"]):
+        return {trigger_header: encode_json({trigger_event["name"]: params}).decode()}
+
+    raise ImproperlyConfiguredException(
+        "invalid value for 'after' param- allowed values are 'receive', 'settle' or 'swap'."
+    )
+
+
+def get_redirect_header(url: str) -> dict[str, Any]:
+    """Return headers for redirect response."""
+    return {HTMXHeaders.REDIRECT.value: quote(url, safe="/#%[]=:;$&()+,!?*@'~"), "Location": ""}
+
+
+def get_push_url_header(url: PushUrlType) -> dict[str, Any]:
+    """Return headers for push url to browser history response."""
+    if isinstance(url, str):
+        url = url if url != "False" else "false"
+    elif isinstance(url, bool):
+        url = "false"
+
+    return {HTMXHeaders.PUSH_URL.value: url}
+
+
+def get_replace_url_header(url: PushUrlType) -> dict[str, Any]:
+    """Return headers for replace url in browser tab response."""
+    url = (url if url != "False" else "false") if isinstance(url, str) else "false"
+    return {HTMXHeaders.REPLACE_URL: url}
+
+
+def get_refresh_header(refresh: bool) -> dict[str, Any]:
+    """Return headers for client refresh response."""
+    value = ""
+    if refresh:
+        value = "true"
+    return {HTMXHeaders.REFRESH.value: value}
+
+
+def get_reswap_header(method: ReSwapMethod) -> dict[str, Any]:
+    """Return headers for change swap method response."""
+    return {HTMXHeaders.RE_SWAP.value: method}
+
+
+def get_retarget_header(target: str) -> dict[str, Any]:
+    """Return headers for change target element response."""
+    return {HTMXHeaders.RE_TARGET.value: target}
+
+
+def get_location_headers(location: LocationType) -> dict[str, Any]:
+    """Return headers for redirect without page-reload response."""
+    spec: dict[str, Any] = {}
+    for key, value in location.items():
+        if value:
+            spec[key] = value
+    if not spec:
+        raise ValueError("redirect_to is required parameter.")
+    return {HTMXHeaders.LOCATION.value: encode_json(spec).decode()}
+
+
+def get_headers(hx_headers: HtmxHeaderType) -> dict[str, Any]:
+    """Return headers for HTMX responses."""
+    if not hx_headers:
+        raise ValueError("Value for hx_headers cannot be None.")
+    htmx_headers_dict: dict[str, Callable] = {
+        "redirect": get_redirect_header,
+        "refresh": get_refresh_header,
+        "push_url": get_push_url_header,
+        "replace_url": get_replace_url_header,
+        "re_swap": get_reswap_header,
+        "re_target": get_retarget_header,
+        "trigger_event": get_trigger_event_headers,
+        "location": get_location_headers,
+    }
+
+    header: dict[str, Any] = {}
+    response: dict[str, Any]
+    key: str
+    value: Any
+    for key, value in hx_headers.items():
+        if key in ["redirect", "refresh", "location", "replace_url"]:
+            response = htmx_headers_dict[key](value)
+            return response
+        if value is not None:
+            response = htmx_headers_dict[key](value)
+            header.update(response)
+    return header
```

### Comparing `starlite-2.0.0a1/starlite/contrib/jinja.py` & `starlite-2.0.0a2/starlite/contrib/jinja.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from starlite.template.base import (
     TemplateEngineProtocol,
     csrf_token,
     url_for,
     url_for_static_asset,
 )
 
+__all__ = ("JinjaTemplateEngine",)
+
+
 try:
-    from jinja2 import Environment, FileSystemLoader
+    from jinja2 import Environment, FileSystemLoader, pass_context
     from jinja2 import TemplateNotFound as JinjaTemplateNotFound
-    from jinja2 import pass_context
 except ImportError as e:
     raise MissingDependencyException("jinja2 is not installed") from e
 
 if TYPE_CHECKING:
     from jinja2 import Template as JinjaTemplate
     from pydantic import DirectoryPath
 
@@ -36,22 +38,23 @@
         self.engine = Environment(loader=loader, autoescape=True)
         self.register_template_callable(key="url_for_static_asset", template_callable=url_for_static_asset)  # type: ignore
         self.register_template_callable(key="csrf_token", template_callable=csrf_token)  # type: ignore
         self.register_template_callable(key="url_for", template_callable=url_for)  # type: ignore
 
     def get_template(self, template_name: str) -> JinjaTemplate:
         """Retrieve a template by matching its name (dotted path) with files in the directory or directories provided.
+
         Args:
             template_name: A dotted path
 
         Returns:
             JinjaTemplate instance
 
         Raises:
-            :class:`TemplateNotFoundException <starlite.exceptions.TemplateNotFoundException>`: if no template is found.
+            TemplateNotFoundException: if no template is found.
         """
         try:
             return self.engine.get_template(name=template_name)
         except JinjaTemplateNotFound as exc:
             raise TemplateNotFoundException(template_name=template_name) from exc
 
     def register_template_callable(self, key: str, template_callable: Callable[[dict[str, Any]], Any]) -> None:
```

### Comparing `starlite-2.0.0a1/starlite/contrib/jwt/jwt_auth.py` & `starlite-2.0.0a2/starlite/contrib/jwt/jwt_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timedelta, timezone
-from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, Literal
+from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, Literal, TypeVar
 
-from pydantic_openapi_schema.v3_1_0 import (
-    Components,
-    OAuthFlow,
-    OAuthFlows,
-    SecurityRequirement,
-    SecurityScheme,
-)
-
-from starlite.connection import ASGIConnection
 from starlite.contrib.jwt.jwt_token import Token
-from starlite.contrib.jwt.middleware import (
-    JWTAuthenticationMiddleware,
-    JWTCookieAuthenticationMiddleware,
-)
+from starlite.contrib.jwt.middleware import JWTAuthenticationMiddleware, JWTCookieAuthenticationMiddleware
 from starlite.datastructures import Cookie
-from starlite.di import Provide
 from starlite.enums import MediaType
 from starlite.middleware import DefineMiddleware
-from starlite.security.base import AbstractSecurityConfig, UserType
+from starlite.openapi.spec import Components, OAuthFlow, OAuthFlows, SecurityRequirement, SecurityScheme
+from starlite.security.base import AbstractSecurityConfig
 from starlite.status_codes import HTTP_201_CREATED
-from starlite.types import (
-    ControllerRouterHandler,
-    Empty,
-    Guard,
-    Scopes,
-    SyncOrAsyncUnion,
-    TypeEncodersMap,
-)
+from starlite.types import ControllerRouterHandler, Empty, Guard, Scopes, SyncOrAsyncUnion, TypeEncodersMap
+
+__all__ = ("BaseJWTAuth", "JWTAuth", "JWTCookieAuth", "OAuth2Login", "OAuth2PasswordBearerAuth")
+
 
 if TYPE_CHECKING:
     from starlite import Response
+    from starlite.connection import ASGIConnection
+    from starlite.di import Provide
+
+
+UserType = TypeVar("UserType")
 
 
 class BaseJWTAuth(Generic[UserType], AbstractSecurityConfig[UserType, Token]):
     """Base class for JWT Auth backends"""
 
     token_secret: str
     """Key with which to generate the token hash.
@@ -57,15 +46,15 @@
 
     """
     algorithm: str
     """Algorithm to use for JWT hashing."""
     auth_header: str
     """Request header key from which to retrieve the token.
 
-    E.g. ``Authorization`` or 'X-Api-Key'.
+    E.g. ``Authorization`` or ``X-Api-Key``.
     """
     default_token_expiration: timedelta
     """The default value for token expiration."""
     openapi_security_scheme_name: str
     """The value to use for the OpenAPI security scheme and security requirements."""
     description: str
     """Description for the OpenAPI security scheme."""
@@ -76,45 +65,48 @@
     """
 
     @property
     def openapi_components(self) -> Components:
         """Create OpenAPI documentation for the JWT auth schema used.
 
         Returns:
-            An :class:`Components <pydantic_openapi_schema.v3_1_0.components.Components>` instance.
+            An :class:`Components <starlite.openapi.spec.components.Components>` instance.
         """
         return Components(
-            securitySchemes={
+            security_schemes={
                 self.openapi_security_scheme_name: SecurityScheme(
                     type="http",
                     scheme="Bearer",
                     name=self.auth_header,
-                    bearerFormat="JWT",
+                    bearer_format="JWT",
                     description=self.description,
                 )
             }
         )
 
     @property
     def security_requirement(self) -> SecurityRequirement:
         """Return OpenAPI 3.1.
 
-        :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>`
+        :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
 
         Returns:
-            An OpenAPI 3.1 :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` dictionary.
+            An OpenAPI 3.1
+            :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
+            dictionary.
         """
         return {self.openapi_security_scheme_name: []}
 
     @property
     def middleware(self) -> DefineMiddleware:
-        """Create ``JWTAuthenticationMiddleware`` wrapped in Starlite's ``DefineMiddleware``.
+        """Create :class:`JWTAuthenticationMiddleware` wrapped in
+        :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
 
         Returns:
-            An instance of :class:`DefineMiddleware <starlite.middleware.base.DefineMiddleware>`.
+            An instance of :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
         """
         return DefineMiddleware(
             self.authentication_middleware_class,
             algorithm=self.algorithm,
             auth_header=self.auth_header,
             exclude=self.exclude,
             exclude_opt_key=self.exclude_opt_key,
@@ -132,30 +124,30 @@
         response_status_code: int = HTTP_201_CREATED,
         token_expiration: timedelta | None = None,
         token_issuer: str | None = None,
         token_audience: str | None = None,
         token_unique_jwt_id: str | None = None,
         send_token_as_response_body: bool = False,
     ) -> Response[Any]:
-        """Create a response with a JWT header. Calls the 'JWTAuth.store_token_handler' to persist the token ``sub``.
+        """Create a response with a JWT header.
 
         Args:
             identifier: Unique identifier of the token subject. Usually this is a user ID or equivalent kind of value.
             response_body: An optional response body to send.
-            response_media_type: An optional 'Content-Type'. Defaults to 'application/json'.
-            response_status_code: An optional status code for the response. Defaults to '201 Created'.
+            response_media_type: An optional ``Content-Type``. Defaults to ``application/json``.
+            response_status_code: An optional status code for the response. Defaults to ``201``.
             token_expiration: An optional timedelta for the token expiration.
             token_issuer: An optional value of the token ``iss`` field.
             token_audience: An optional value for the token ``aud`` field.
             token_unique_jwt_id: An optional value for the token ``jti`` field.
             send_token_as_response_body: If ``True`` the response will be a dict including the token: ``{ "token": <token> }``
                 will be returned as the response body. Note: if a response body is passed this setting will be ignored.
 
         Returns:
-            A :class:`Response <starlite.response.Response>` instance.
+            A :class:`Response <.response.Response>` instance.
         """
         encoded_token = self.create_token(
             identifier=identifier,
             token_expiration=token_expiration,
             token_issuer=token_issuer,
             token_audience=token_audience,
             token_unique_jwt_id=token_unique_jwt_id,
@@ -209,15 +201,15 @@
 
         Args:
             encoded_token: An encoded JWT token
 
         Returns:
             The encoded token formatted for the HTTP headers
         """
-        security = self.openapi_components.securitySchemes.get(self.openapi_security_scheme_name, None)  # type: ignore
+        security = self.openapi_components.security_schemes.get(self.openapi_security_scheme_name, None)  # type: ignore
         return f"{security.scheme} {encoded_token}" if isinstance(security, SecurityScheme) else encoded_token
 
 
 @dataclass
 class JWTAuth(Generic[UserType], BaseJWTAuth[UserType]):
     """JWT Authentication Configuration.
 
@@ -259,15 +251,15 @@
     """A mapping of types to callables that transform them into types supported for serialization."""
 
     algorithm: str = field(default="HS256")
     """Algorithm to use for JWT hashing."""
     auth_header: str = field(default="Authorization")
     """Request header key from which to retrieve the token.
 
-    E.g. ``Authorization`` or 'X-Api-Key'.
+    E.g. ``Authorization`` or ``X-Api-Key``.
     """
     default_token_expiration: timedelta = field(default_factory=lambda: timedelta(days=1))
     """The default value for token expiration."""
     openapi_security_scheme_name: str = field(default="BearerToken")
     """The value to use for the OpenAPI security scheme and security requirements."""
     description: str = field(default="JWT api-key authentication and authorization.")
     """Description for the OpenAPI security scheme."""
@@ -278,16 +270,16 @@
     """
 
 
 @dataclass
 class JWTCookieAuth(Generic[UserType], BaseJWTAuth[UserType]):
     """JWT Cookie Authentication Configuration.
 
-    This class is an alternate entry point to the library, and it includes all the functionality of the ``JWTAuth`` class
-    and adds support for passing JWT tokens ``HttpOnly`` cookies.
+    This class is an alternate entry point to the library, and it includes all the functionality of the :class:`JWTAuth`
+    class and adds support for passing JWT tokens ``HttpOnly`` cookies.
     """
 
     token_secret: str
     """Key with which to generate the token hash.
 
     Notes:
         - This value should be kept as a secret and the standard practice is to inject it into the environment.
@@ -320,69 +312,68 @@
     """A mapping of types to callables that transform them into types supported for serialization."""
 
     algorithm: str = field(default="HS256")
     """Algorithm to use for JWT hashing."""
     auth_header: str = field(default="Authorization")
     """Request header key from which to retrieve the token.
 
-    E.g. ``Authorization`` or 'X-Api-Key'.
+    E.g. ``Authorization`` or ``X-Api-Key``.
     """
     default_token_expiration: timedelta = field(default_factory=lambda: timedelta(days=1))
     """The default value for token expiration."""
     openapi_security_scheme_name: str = field(default="BearerToken")
     """The value to use for the OpenAPI security scheme and security requirements."""
     key: str = field(default="token")
     """Key for the cookie."""
     path: str = field(default="/")
     """Path fragment that must exist in the request url for the cookie to be valid.
 
-    Defaults to '/'.
+    Defaults to ``/``.
     """
     domain: str | None = field(default=None)
     """Domain for which the cookie is valid."""
     secure: bool | None = field(default=None)
     """Https is required for the cookie."""
     samesite: Literal["lax", "strict", "none"] = field(default="lax")
     """Controls whether or not a cookie is sent with cross-site requests. Defaults to ``lax``. """
     description: str = field(default="JWT cookie-based authentication and authorization.")
     """Description for the OpenAPI security scheme."""
     authentication_middleware_class: type[JWTCookieAuthenticationMiddleware] = field(
         default=JWTCookieAuthenticationMiddleware
     )
-    """The authentication middleware class to use.
-
-    Must inherit from :class:`JWTCookieAuthenticationMiddleware`
+    """The authentication middleware class to use. Must inherit from :class:`JWTCookieAuthenticationMiddleware`
     """
 
     @property
     def openapi_components(self) -> Components:
         """Create OpenAPI documentation for the JWT Cookie auth scheme.
 
         Returns:
-            An :class:`Components <pydantic_openapi_schema.v3_1_0.components.Components>` instance.
+            A :class:`Components <starlite.openapi.spec.components.Components>` instance.
         """
         return Components(
-            securitySchemes={
+            security_schemes={
                 self.openapi_security_scheme_name: SecurityScheme(
                     type="http",
                     scheme="Bearer",
                     name=self.key,
                     security_scheme_in="cookie",
-                    bearerFormat="JWT",
+                    bearer_format="JWT",
                     description=self.description,
                 )
             }
         )
 
     @property
     def middleware(self) -> DefineMiddleware:
-        """Create ``JWTCookieAuthenticationMiddleware`` wrapped in Starlite's ``DefineMiddleware``.
+        """Create :class:`JWTCookieAuthenticationMiddleware` wrapped in
+            :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
 
         Returns:
-            An instance of :class:`DefineMiddleware <starlite.middleware.base.DefineMiddleware>`.
+            An instance of :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
         """
         return DefineMiddleware(
             self.authentication_middleware_class,
             algorithm=self.algorithm,
             auth_cookie_key=self.key,
             auth_header=self.auth_header,
             exclude=self.exclude,
@@ -401,30 +392,30 @@
         response_status_code: int = HTTP_201_CREATED,
         token_expiration: timedelta | None = None,
         token_issuer: str | None = None,
         token_audience: str | None = None,
         token_unique_jwt_id: str | None = None,
         send_token_as_response_body: bool = False,
     ) -> Response[Any]:
-        """Create a response with a JWT header. Calls the 'JWTAuth.store_token_handler' to persist the token ``sub``.
+        """Create a response with a JWT header.
 
         Args:
             identifier: Unique identifier of the token subject. Usually this is a user ID or equivalent kind of value.
             response_body: An optional response body to send.
             response_media_type: An optional 'Content-Type'. Defaults to 'application/json'.
             response_status_code: An optional status code for the response. Defaults to '201 Created'.
             token_expiration: An optional timedelta for the token expiration.
             token_issuer: An optional value of the token ``iss`` field.
             token_audience: An optional value for the token ``aud`` field.
             token_unique_jwt_id: An optional value for the token ``jti`` field.
             send_token_as_response_body: If ``True`` the response will be a dict including the token: ``{ "token": <token> }``
                 will be returned as the response body. Note: if a response body is passed this setting will be ignored.
 
         Returns:
-            A :class:`Response <starlite.response.Response>` instance.
+            A :class:`Response <.response.Response>` instance.
         """
 
         encoded_token = self.create_token(
             identifier=identifier,
             token_expiration=token_expiration,
             token_issuer=token_issuer,
             token_audience=token_audience,
@@ -471,17 +462,16 @@
     """Expiration time of the token in seconds. """
 
 
 @dataclass
 class OAuth2PasswordBearerAuth(Generic[UserType], BaseJWTAuth[UserType]):
     """OAUTH2 Schema for Password Bearer Authentication.
 
-    This class implements an OAUTH2 authentication flow entry point to the library, and it
-    includes all the functionality of the ``JWTAuth`` class and adds
-    support for passing JWT tokens ``HttpOnly`` cookies.
+    This class implements an OAUTH2 authentication flow entry point to the library, and it includes all the
+    functionality of the :class:`JWTAuth` class and adds support for passing JWT tokens ``HttpOnly`` cookies.
 
     ``token_url`` is the only additional argument that is required, and it should point at your login route
     """
 
     token_secret: str
     """Key with which to generate the token hash.
 
@@ -531,15 +521,15 @@
     oauth_scopes: dict[str, str] | None = field(default=None)
     """Oauth Scopes available for the token."""
     key: str = field(default="token")
     """Key for the cookie."""
     path: str = field(default="/")
     """Path fragment that must exist in the request url for the cookie to be valid.
 
-    Defaults to '/'.
+    Defaults to ``/``.
     """
     domain: str | None = field(default=None)
     """Domain for which the cookie is valid."""
     secure: bool | None = field(default=None)
     """Https is required for the cookie."""
     samesite: Literal["lax", "strict", "none"] = field(default="lax")
     """Controls whether or not a cookie is sent with cross-site requests. Defaults to ``lax``. """
@@ -551,18 +541,19 @@
     """The authentication middleware class to use.
 
     Must inherit from :class:`JWTCookieAuthenticationMiddleware`
     """
 
     @property
     def middleware(self) -> DefineMiddleware:
-        """Create ``JWTCookieAuthenticationMiddleware`` wrapped in Starlite's ``DefineMiddleware``.
+        """Create ``JWTCookieAuthenticationMiddleware`` wrapped in
+            :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
 
         Returns:
-            An instance of :class:`DefineMiddleware <starlite.middleware.base.DefineMiddleware>`.
+            An instance of :class:`DefineMiddleware <.middleware.base.DefineMiddleware>`.
         """
         return DefineMiddleware(
             self.authentication_middleware_class,
             algorithm=self.algorithm,
             auth_cookie_key=self.key,
             auth_header=self.auth_header,
             exclude=self.exclude,
@@ -573,37 +564,37 @@
         )
 
     @property
     def oauth_flow(self) -> OAuthFlow:
         """Create an OpenAPI OAuth2 flow for the password bearer authentication scheme.
 
         Returns:
-            An :class:`OAuthFlow <pydantic_openapi_schema.v3_1_0.oauth_flow.OAuthFlow>` instance.
+            An :class:`OAuthFlow <starlite.openapi.spec.oauth_flow.OAuthFlow>` instance.
         """
         return OAuthFlow(
-            tokenUrl=self.token_url,
+            token_url=self.token_url,
             scopes=self.oauth_scopes,
         )
 
     @property
     def openapi_components(self) -> Components:
         """Create OpenAPI documentation for the OAUTH2 Password bearer auth scheme.
 
         Returns:
-            An :class:`Components <pydantic_openapi_schema.v3_1_0.components.Components>` instance.
+            An :class:`Components <starlite.openapi.spec.components.Components>` instance.
         """
         return Components(
-            securitySchemes={
+            security_schemes={
                 self.openapi_security_scheme_name: SecurityScheme(
                     type="oauth2",
                     scheme="Bearer",
                     name=self.auth_header,
                     security_scheme_in="header",
                     flows=OAuthFlows(password=self.oauth_flow),  # pyright: reportGeneralTypeIssues=false
-                    bearerFormat="JWT",
+                    bearer_format="JWT",
                     description=self.description,
                 )
             }
         )
 
     def login(
         self,
@@ -614,30 +605,30 @@
         response_status_code: int = HTTP_201_CREATED,
         token_expiration: timedelta | None = None,
         token_issuer: str | None = None,
         token_audience: str | None = None,
         token_unique_jwt_id: str | None = None,
         send_token_as_response_body: bool = True,
     ) -> Response[Any]:
-        """Create a response with a JWT header. Calls the 'JWTAuth.store_token_handler' to persist the token ``sub``.
+        """Create a response with a JWT header.
 
         Args:
             identifier: Unique identifier of the token subject. Usually this is a user ID or equivalent kind of value.
             response_body: An optional response body to send.
-            response_media_type: An optional 'Content-Type'. Defaults to 'application/json'.
-            response_status_code: An optional status code for the response. Defaults to '201 Created'.
+            response_media_type: An optional ``Content-Type``. Defaults to ``application/json``.
+            response_status_code: An optional status code for the response. Defaults to ``201``.
             token_expiration: An optional timedelta for the token expiration.
             token_issuer: An optional value of the token ``iss`` field.
             token_audience: An optional value for the token ``aud`` field.
             token_unique_jwt_id: An optional value for the token ``jti`` field.
             send_token_as_response_body: If ``True`` the response will be an oAuth2 token response dict.
                 Note: if a response body is passed this setting will be ignored.
 
         Returns:
-            A :class:`Response <starlite.response.Response>` instance.
+            A :class:`Response <.response.Response>` instance.
         """
         encoded_token = self.create_token(
             identifier=identifier,
             token_expiration=token_expiration,
             token_issuer=token_issuer,
             token_audience=token_audience,
             token_unique_jwt_id=token_unique_jwt_id,
@@ -656,15 +647,15 @@
 
         if response_body is not Empty:
             body = response_body
         elif send_token_as_response_body:
             token_dto = OAuth2Login(
                 access_token=encoded_token,
                 expires_in=expires_in,
-                token_type="bearer",
+                token_type="bearer",  # noqa: S106
             )
             body = asdict(token_dto)
         else:
             body = None
 
         return self.create_response(
             content=body,
```

### Comparing `starlite-2.0.0a1/starlite/contrib/jwt/jwt_token.py` & `starlite-2.0.0a2/starlite/contrib/jwt/jwt_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from datetime import datetime, timezone
 from typing import cast
 
 from jose import JWSError, JWTError, jwt
 
 from starlite.exceptions import ImproperlyConfiguredException, NotAuthorizedException
 
+__all__ = ("Token",)
+
 
 def _normalize_datetime(value: datetime) -> datetime:
     """Convert the given value into UTC and strip microseconds.
 
     Args:
         value: A datetime instance
 
@@ -70,15 +72,15 @@
             secret: The secret with which the JWT is encoded. It may optionally be an individual JWK or JWS set dict
             algorithm: The algorithm used to encode the JWT.
 
         Returns:
             A decoded Token instance.
 
         Raises:
-            :class:`NotAuthorizedException <starlite.exceptions.NotAuthorizedException>`: If token is invalid.
+            NotAuthorizedException: If the token is invalid.
         """
         try:
             payload = jwt.decode(token=encoded_token, key=secret, algorithms=[algorithm], options={"verify_aud": False})
             exp = datetime.fromtimestamp(payload.pop("exp"), tz=timezone.utc)
             iat = datetime.fromtimestamp(payload.pop("iat"), tz=timezone.utc)
             return Token(exp=exp, iat=iat, **payload)
         except (KeyError, JWTError, ImproperlyConfiguredException) as e:
@@ -91,15 +93,15 @@
             secret: The secret with which the JWT is encoded.
             algorithm: The algorithm used to encode the JWT.
 
         Returns:
             An encoded token string.
 
         Raises:
-            :class:`ImproperlyConfiguredException <starlite.exceptions.ImproperlyConfiguredException>`: If encoding fails.
+            ImproperlyConfiguredException: If encoding fails.
         """
         try:
             return cast(
                 "str",
                 jwt.encode(
                     claims={k: v for k, v in asdict(self).items() if v is not None}, key=secret, algorithm=algorithm
                 ),
```

### Comparing `starlite-2.0.0a1/starlite/contrib/jwt/middleware.py` & `starlite-2.0.0a2/starlite/contrib/jwt/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from starlite.contrib.jwt.jwt_token import Token
 from starlite.exceptions import NotAuthorizedException
 from starlite.middleware.authentication import (
     AbstractAuthenticationMiddleware,
     AuthenticationResult,
 )
 
+__all__ = ("JWTAuthenticationMiddleware", "JWTCookieAuthenticationMiddleware")
+
+
 if TYPE_CHECKING:
     from typing import Any
 
     from starlite.connection import ASGIConnection
     from starlite.types import ASGIApp, Scopes
     from starlite.utils import AsyncCallable
 
@@ -36,19 +39,19 @@
     ):
         """Check incoming requests for an encoded token in the auth header specified, and if present retrieve the user
         from persistence using the provided function.
 
         Args:
             algorithm: JWT hashing algorithm to use.
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
-            auth_header: Request header key from which to retrieve the token. E.g. ``Authorization`` or 'X-Api-Key'.
+            auth_header: Request header key from which to retrieve the token. E.g. ``Authorization`` or ``X-Api-Key``.
             exclude: A pattern or list of patterns to skip.
             exclude_opt_key: An identifier to use on routes to disable authentication for a particular route.
-            retrieve_user_handler: A function that receives an instance of ``Token`` and returns a user, which can be
-                any arbitrary value.
+            retrieve_user_handler: A function that receives a :class:`Token <.contrib.jwt.Token>` and returns a user,
+                which can be any arbitrary value.
             scopes: ASGI scopes processed by the authentication middleware.
             token_secret: Secret for decoding the JWT token. This value should be equivalent to the secret used to
                 encode it.
         """
         super().__init__(app=app, exclude=exclude, exclude_from_auth_key=exclude_opt_key, scopes=scopes)
         self.algorithm = algorithm
         self.auth_header = auth_header
@@ -62,36 +65,36 @@
         Args:
             connection: An Starlite HTTPConnection instance.
 
         Returns:
             AuthenticationResult
 
         Raises:
-            :class:`NotAuthorizedException <starlite.exceptions.NotAuthorizedException>`: If token is invalid or user is not found.
+            NotAuthorizedException: If token is invalid or user is not found.
         """
         auth_header = connection.headers.get(self.auth_header)
         if not auth_header:
             raise NotAuthorizedException("No JWT token found in request header")
         encoded_token = auth_header.partition(" ")[-1]
         return await self.authenticate_token(encoded_token=encoded_token, connection=connection)
 
     async def authenticate_token(
         self, encoded_token: str, connection: ASGIConnection[Any, Any, Any, Any]
     ) -> AuthenticationResult:
         """Given an encoded JWT token, parse, validate and look up sub within token.
 
         Args:
-            encoded_token: _description_
+            encoded_token: Encoded JWT token.
             connection: An ASGI connection instance.
 
         Raises:
-            :class:`NotAuthorizedException <starlite.exceptions.NotAuthorizedException>`: If token is invalid or user is not found.
+            NotAuthorizedException: If token is invalid or user is not found.
 
         Returns:
-            AuthenticationResult: _description_
+            AuthenticationResult
         """
         token = Token.decode(
             encoded_token=encoded_token,
             secret=self.token_secret,
             algorithm=self.algorithm,
         )
 
@@ -121,19 +124,19 @@
         """Check incoming requests for an encoded token in the auth header or cookie name specified, and if present
         retrieves the user from persistence using the provided function.
 
         Args:
             algorithm: JWT hashing algorithm to use.
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             auth_cookie_key: Cookie name from which to retrieve the token. E.g. ``token`` or ``accessToken``.
-            auth_header: Request header key from which to retrieve the token. E.g. ``Authorization`` or 'X-Api-Key'.
+            auth_header: Request header key from which to retrieve the token. E.g. ``Authorization`` or ``X-Api-Key``.
             exclude: A pattern or list of patterns to skip.
             exclude_opt_key: An identifier to use on routes to disable authentication for a particular route.
-            retrieve_user_handler: A function that receives an instance of ``Token`` and returns a user, which can be
-                any arbitrary value.
+            retrieve_user_handler: A function that receives a :class:`Token <.contrib.jwt.Token>` and returns a user,
+                which can be any arbitrary value.
             scopes: ASGI scopes processed by the authentication middleware.
             token_secret: Secret for decoding the JWT token. This value should be equivalent to the secret used to
                 encode it.
         """
         super().__init__(
             algorithm=algorithm,
             app=app,
@@ -149,18 +152,18 @@
     async def authenticate_request(self, connection: ASGIConnection[Any, Any, Any, Any]) -> AuthenticationResult:
         """Given an HTTP Connection, parse the JWT api key stored in the header and retrieve the user correlating to the
         token from the DB.
 
         Args:
             connection: An Starlite HTTPConnection instance.
 
+        Raises:
+            NotAuthorizedException: If token is invalid or user is not found.
+
         Returns:
             AuthenticationResult
-
-        Raises:
-            :class:`NotAuthorizedException <starlite.exceptions.NotAuthorizedException>`: If token is invalid or user is not found.
         """
         auth_header = connection.headers.get(self.auth_header) or connection.cookies.get(self.auth_cookie_key)
         if not auth_header:
             raise NotAuthorizedException("No JWT token found in request header or cookies")
         encoded_token = auth_header.partition(" ")[-1]
         return await self.authenticate_token(encoded_token=encoded_token, connection=connection)
```

### Comparing `starlite-2.0.0a1/starlite/contrib/mako.py` & `starlite-2.0.0a2/starlite/contrib/mako.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     TemplateEngineProtocol,
     TemplateProtocol,
     csrf_token,
     url_for,
     url_for_static_asset,
 )
 
+__all__ = ("MakoTemplate", "MakoTemplateEngine")
+
+
 try:
     from mako.exceptions import TemplateLookupException as MakoTemplateNotFound
     from mako.lookup import TemplateLookup
 
 except ImportError as e:
     raise MissingDependencyException("mako is not installed") from e
 
@@ -69,22 +72,23 @@
         self._template_callables: list[tuple[str, Callable[[dict[str, Any]], Any]]] = []
         self.register_template_callable(key="url_for_static_asset", template_callable=url_for_static_asset)  # type: ignore
         self.register_template_callable(key="csrf_token", template_callable=csrf_token)  # type: ignore
         self.register_template_callable(key="url_for", template_callable=url_for)  # type: ignore
 
     def get_template(self, template_name: str) -> MakoTemplate:
         """Retrieve a template by matching its name (dotted path) with files in the directory or directories provided.
+
         Args:
             template_name: A dotted path
 
         Returns:
             MakoTemplate instance
 
         Raises:
-            :class:`TemplateNotFoundException <starlite.exceptions.TemplateNotFoundException>`: if no template is found.
+            TemplateNotFoundException: if no template is found.
         """
         try:
             return MakoTemplate(
                 template=self.engine.get_template(template_name), template_callables=self._template_callables
             )
         except MakoTemplateNotFound as exc:
             raise TemplateNotFoundException(template_name=template_name) from exc
```

### Comparing `starlite-2.0.0a1/starlite/contrib/opentelemetry/config.py` & `starlite-2.0.0a2/starlite/contrib/opentelemetry/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Callable
 
+from starlite.contrib.opentelemetry._utils import get_route_details_from_scope
 from starlite.contrib.opentelemetry.middleware import (
     OpenTelemetryInstrumentationMiddleware,
 )
-from starlite.contrib.opentelemetry.utils import get_route_details_from_scope
 from starlite.exceptions import MissingDependencyException
 from starlite.middleware.base import DefineMiddleware
 
+__all__ = ("OpenTelemetryConfig",)
+
+
 try:
-    from opentelemetry.trace import Span, TracerProvider  # pyright: ignore
+    import opentelemetry  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("OpenTelemetry dependencies are not installed") from e
 
+
+from opentelemetry.trace import Span, TracerProvider  # pyright: ignore
+
 if TYPE_CHECKING:
     from opentelemetry.metrics import Meter, MeterProvider
 
     from starlite.types import Scope, Scopes
 
 OpenTelemetryHookHandler = Callable[[Span, dict], None]
```

### Comparing `starlite-2.0.0a1/starlite/contrib/opentelemetry/middleware.py` & `starlite-2.0.0a2/starlite/contrib/opentelemetry/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from starlite.exceptions import MissingDependencyException
 from starlite.middleware.base import AbstractMiddleware
 
+__all__ = ("OpenTelemetryInstrumentationMiddleware",)
+
+
 try:
-    from opentelemetry.instrumentation.asgi import OpenTelemetryMiddleware
-    from opentelemetry.util.http import get_excluded_urls
+    import opentelemetry  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("OpenTelemetry dependencies are not installed") from e
 
+from opentelemetry.instrumentation.asgi import OpenTelemetryMiddleware
+from opentelemetry.util.http import get_excluded_urls
+
 if TYPE_CHECKING:
     from starlite.contrib.opentelemetry import OpenTelemetryConfig
     from starlite.types import ASGIApp, Receive, Scope, Send
 
 
 class OpenTelemetryInstrumentationMiddleware(AbstractMiddleware):
     """OpenTelemetry Middleware."""
 
     __slots__ = ("open_telemetry_middleware",)
 
-    def __init__(self, app: "ASGIApp", config: "OpenTelemetryConfig"):
+    def __init__(self, app: ASGIApp, config: OpenTelemetryConfig):
         """Middleware that adds OpenTelemetry instrumentation to the application.
 
         Args:
             app: The ``next`` ASGI app to call.
-            config: An instance of :class:`OpenTelemetryConfig <starlite.contrib.opentelemetry.OpenTelemetryConfig>`
+            config: An instance of :class:`OpenTelemetryConfig <.contrib.opentelemetry.OpenTelemetryConfig>`
         """
         super().__init__(app=app, scopes=config.scopes, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key)
         self.open_telemetry_middleware = OpenTelemetryMiddleware(
             app=app,
             client_request_hook=config.client_request_hook_handler,
             client_response_hook=config.client_response_hook_handler,
             default_span_details=config.scope_span_details_extractor,
```

### Comparing `starlite-2.0.0a1/starlite/contrib/opentelemetry/utils.py` & `starlite-2.0.0a2/starlite/contrib/opentelemetry/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from starlite.exceptions import MissingDependencyException
 
+__all__ = ("get_route_details_from_scope",)
+
+
 try:
     from opentelemetry.semconv.trace import SpanAttributes
 except ImportError as e:
     raise MissingDependencyException("OpenTelemetry dependencies are not installed") from e
 
 if TYPE_CHECKING:
     from starlite.types import Scope
```

### Comparing `starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/config.py` & `starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
-from typing import TYPE_CHECKING, Any, Callable, Literal, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Literal, cast
 
-from starlite.config.logging import BaseLoggingConfig, LoggingConfig
-from starlite.datastructures.state import State  # noqa: TC001
-from starlite.exceptions import (
-    ImproperlyConfiguredException,
-    MissingDependencyException,
-)
+from starlite.exceptions import ImproperlyConfiguredException, MissingDependencyException
+from starlite.logging.config import BaseLoggingConfig, LoggingConfig
 from starlite.serialization import decode_json, encode_json
 from starlite.utils import AsyncCallable
 
 try:
-    from sqlalchemy import create_engine
-    from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, create_async_engine
-    from sqlalchemy.orm import Query, Session, sessionmaker
+    import sqlalchemy  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("sqlalchemy is not installed") from e
 
+from sqlalchemy import create_engine
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, create_async_engine
+from sqlalchemy.orm import Query, Session, sessionmaker
+
+__all__ = ("SQLAlchemyConfig", "SQLAlchemyEngineConfig", "SQLAlchemySessionConfig")
+
+
 if TYPE_CHECKING:
     from sqlalchemy.engine import Engine
     from sqlalchemy.future import Engine as FutureEngine
     from sqlalchemy.pool import Pool
 
+    from starlite.datastructures.state import State
     from starlite.types import BeforeMessageSendHookHandler, Message, Scope
 
     from .types import SessionMakerInstanceProtocol, SessionMakerTypeProtocol
 
 IsolationLevel = Literal["AUTOCOMMIT", "READ COMMITTED", "READ UNCOMMITTED", "REPEATABLE READ", "SERIALIZABLE"]
 
 SESSION_SCOPE_KEY = "_sql_alchemy_db_session"
-SESSION_TERMINUS_ASGI_EVENTS = {
-    "http.response.start",
-    "http.disconnect",
-    "websocket.disconnect",
-    "websocket.close",
-}
+SESSION_TERMINUS_ASGI_EVENTS = {"http.response.start", "http.disconnect", "websocket.disconnect", "websocket.close"}
 
 
 def serializer(value: Any) -> str:
     """Serialize JSON field values.
 
     Args:
         value: Any json serializable value.
@@ -58,15 +55,15 @@
         message: ASGI-``Message``
         _: A ``State`` (not used)
         scope: An ASGI-``Scope``
 
     Returns:
         None
     """
-    session = cast("Optional[Union[Session, AsyncSession]]", scope.get(SESSION_SCOPE_KEY))
+    session = cast("Session | AsyncSession | None", scope.get(SESSION_SCOPE_KEY))
     if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
         if isinstance(session, AsyncSession):
             await session.close()
         else:
             session.close()
         del scope[SESSION_SCOPE_KEY]  # type: ignore
 
@@ -154,15 +151,15 @@
     """
     create_engine_callable: Callable[[str], Engine | FutureEngine] = field(default=create_engine)
     """Callable that creates an :class:`Engine <sqlalchemy.engine.Engine>` or ``FutureEngine`` instance or instance of its
     subclass."""
     dependency_key: str = field(default="db_session")
     """Key to use for the dependency injection of database sessions."""
     engine_app_state_key: str = field(default="db_engine")
-    """Key under which to store the SQLAlchemy engine in the application :class:`State <starlite.datastructures.State>`
+    """Key under which to store the SQLAlchemy engine in the application :class:`State <.datastructures.State>`
     instance.
     """
     engine_config: SQLAlchemyEngineConfig = field(default_factory=SQLAlchemyEngineConfig)
     """Configuration for the SQLAlchemy engine.
 
     The configuration options are documented in the SQLAlchemy documentation.
     """
@@ -184,16 +181,16 @@
     """Configuration options for the ``sessionmaker``.
 
     The configuration options are documented in the SQLAlchemy documentation.
     """
     session_maker_class: type[SessionMakerTypeProtocol] = field(default=sessionmaker)
     """Sessionmaker class to use."""
     session_maker_app_state_key: str = field(default="session_maker_class")
-    """Key under which to store the SQLAlchemy ``sessionmaker`` in the application :class:`State <starlite.datastructures.State>`
-    instance.
+    """Key under which to store the SQLAlchemy ``sessionmaker`` in the application
+    :class:`State <.datastructures.State>` instance.
     """
     session_maker_instance: SessionMakerInstanceProtocol | None = field(default=None)
     """Optional sessionmaker to use.
 
     If set, the plugin will use the provided instance rather than instantiate a sessionmaker.
     """
     engine_instance: Engine | FutureEngine | AsyncEngine | None = field(default=None)
@@ -243,15 +240,15 @@
         if not self.engine_instance:
             create_engine_callable = (
                 self.create_async_engine_callable if self.use_async_engine else self.create_engine_callable
             )
             self.engine_instance = create_engine_callable(
                 self.connection_string, **self.engine_config_dict  # type:ignore[arg-type]
             )
-        return cast("Union[Engine, FutureEngine, AsyncEngine]", self.engine_instance)
+        return cast("Engine | FutureEngine | AsyncEngine", self.engine_instance)
 
     @property
     def session_maker(self) -> sessionmaker:
         """Get a sessionmaker. If none exists yet, create one.
 
         Returns:
             Getter that returns the session_maker instance used by the plugin.
@@ -264,64 +261,64 @@
             }
             session_class = self.session_class or (AsyncSession if self.use_async_engine else Session)
             self.session_maker_instance = self.session_maker_class(
                 self.engine, class_=session_class, **session_maker_kwargs
             )
         return cast("sessionmaker", self.session_maker_instance)
 
-    def create_db_session_dependency(self, state: State, scope: Scope) -> Session | AsyncSession:
+    def create_db_session_dependency(self, state: State, scope: Scope) -> Union[Session, AsyncSession]:  # noqa: F821
         """Create a session instance.
 
         Args:
-            state: The 'application.state' instance.
+            state: The ``Starlite.state`` instance.
             scope: The current connection's scope.
 
         Returns:
             A session instance T.
         """
         session = scope.get(SESSION_SCOPE_KEY)
         if not session:
             session_maker = cast("sessionmaker", state[self.session_maker_app_state_key])
             session = scope[SESSION_SCOPE_KEY] = session_maker()  # type: ignore
-        return cast("Union[Session, AsyncSession]", session)
+        return cast("Session | AsyncSession", session)
 
     def update_app_state(self, state: State) -> None:
         """Create a DB engine and stores it in the application state.
 
         Args:
-            state: The 'application.state' instance.
+            state: The ``Starlite.state`` instance.
 
         Returns:
             None
         """
 
         state[self.engine_app_state_key] = self.engine
         state[self.session_maker_app_state_key] = self.session_maker
 
     async def on_shutdown(self, state: State) -> None:
         """Disposes of the SQLAlchemy engine.
 
         Args:
-            state: The 'application.state' instance.
+            state: The ``Starlite.state`` instance.
 
         Returns:
             None
         """
-        engine = cast("Union[Engine, AsyncEngine]", state[self.engine_app_state_key])
+        engine = cast("Engine | AsyncEngine", state[self.engine_app_state_key])
         if isinstance(engine, AsyncEngine):
             await engine.dispose()
         else:
             engine.dispose()
         del state[self.engine_app_state_key]
 
     def config_sql_alchemy_logging(self, logging_config: BaseLoggingConfig | None) -> None:
         """Add the SQLAlchemy loggers to the logging config.
 
         Notes:
-            - Currently only works with :class:`LoggingConfig <starlite.config.logging.LoggingConfig>`.
+            - Currently only works with :class:`LoggingConfig <.logging.config.LoggingConfig>`.
 
         Args:
             logging_config: Logging config.
 
         Returns:
             None.
         """
```

### Comparing `starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/plugin.py` & `starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,69 +13,75 @@
     Type,
     Union,
 )
 from uuid import UUID
 
 from pydantic import BaseModel, conint, constr, create_model
 from pydantic_factories import ModelFactory
-from pydantic_openapi_schema.utils.utils import OpenAPI310PydanticSchema
 
 from starlite.di import Provide
 from starlite.exceptions import (
     ImproperlyConfiguredException,
     MissingDependencyException,
 )
-from starlite.plugins.base import InitPluginProtocol, SerializationPluginProtocol
-
-from .types import SQLAlchemyBinaryType
+from starlite.openapi.spec.schema import SchemaDataContainer
+from starlite.plugins import InitPluginProtocol, SerializationPluginProtocol
 
 try:
-    from sqlalchemy import inspect
-    from sqlalchemy import types as sqlalchemy_type
-    from sqlalchemy.dialects import mssql, mysql, oracle, postgresql, sqlite
-    from sqlalchemy.exc import NoInspectionAvailable
-    from sqlalchemy.orm import DeclarativeMeta, InstanceState, Mapper
-    from sqlalchemy.sql.type_api import TypeEngine
+    import sqlalchemy  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("sqlalchemy is not installed") from e
 
 
+from sqlalchemy import inspect
+from sqlalchemy import types as sqlalchemy_type
+from sqlalchemy.dialects import mssql, mysql, oracle, postgresql, sqlite
+from sqlalchemy.exc import NoInspectionAvailable
+from sqlalchemy.orm import DeclarativeMeta, InstanceState, Mapper
+from sqlalchemy.sql.type_api import TypeEngine
+
+from .types import SQLAlchemyBinaryType
+
+__all__ = ("SQLAlchemyPlugin",)
+
+
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import Schema
     from typing_extensions import TypeGuard
 
     from starlite.app import Starlite
-    from starlite.plugins.sql_alchemy.config import SQLAlchemyConfig
+    from starlite.openapi.spec import Schema
+
+    from .config import SQLAlchemyConfig
 
 
 class SQLAlchemyPlugin(InitPluginProtocol, SerializationPluginProtocol[DeclarativeMeta, BaseModel]):
     """A Plugin for SQLAlchemy."""
 
     __slots__ = ("_model_namespace_map", "_config")
 
     def __init__(self, config: Optional["SQLAlchemyConfig"] = None) -> None:
         """Initialize ``SQLAlchemyPlugin``.
 
         Support (de)serialization and OpenAPI generation for SQLAlchemy
         ORM types.
 
         Args:
-            config: Optional :class:`SQLAlchemyConfig <starlite.plugins.sql_alchemy.SQLAlchemyConfig>` instance. If
+            config: Optional :class:`SQLAlchemyConfig <.contrib.sqlalchemy_1.config.SQLAlchemyConfig>` instance. If
                 passed, the plugin will establish a DB connection and hook handlers and dependencies.
         """
         self._model_namespace_map: Dict[str, "Type[BaseModel]"] = {}
         self._config = config
 
     def on_app_init(self, app: "Starlite") -> None:
         """If config has been passed to the plugin, it will initialize SQLAlchemy and add the dependencies as expected.
 
         Executed on the application's init process.
 
         Args:
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
 
         Returns:
             None
         """
         if self._config is not None:
             app.dependencies[self._config.dependency_key] = Provide(self._config.create_db_session_dependency)
             app.before_send.append(self._config.before_send_handler)  # type: ignore[arg-type]
@@ -168,18 +174,17 @@
         """
         return column_type.enum_class  # type:ignore[union-attr]
 
     @property
     def providers_map(self) -> Dict[Type[TypeEngine], Callable[[Union[TypeEngine, Type[TypeEngine]]], Any]]:
         """Map of SQLAlchemy column types to provider functions.
 
-        This method is separated to allow for easy overriding in
-        subclasses.
+        This method is separated to allow for easy overriding in subclasses.
 
-        Returns
+        Returns:
             A dictionary mapping SQLAlchemy types to callables.
         """
         return {
             sqlalchemy_type.ARRAY: self.handle_list_type,
             sqlalchemy_type.BIGINT: lambda x: int,
             sqlalchemy_type.BINARY: self.handle_string_type,
             sqlalchemy_type.BLOB: self.handle_string_type,
@@ -214,14 +219,16 @@
             sqlalchemy_type.TIME: lambda x: time,
             sqlalchemy_type.TIMESTAMP: lambda x: datetime,
             sqlalchemy_type.Text: self.handle_string_type,
             sqlalchemy_type.Time: lambda x: time,
             sqlalchemy_type.TupleType: self.handle_tuple_type,  # pyright: ignore
             sqlalchemy_type.Unicode: self.handle_string_type,
             sqlalchemy_type.UnicodeText: self.handle_string_type,
+            sqlalchemy_type.Uuid: lambda x: UUID,
+            sqlalchemy_type.UUID: lambda x: UUID,
             sqlalchemy_type.VARBINARY: self.handle_string_type,
             sqlalchemy_type.VARCHAR: self.handle_string_type,
             # mssql
             mssql.BIT: lambda x: bool,
             mssql.DATETIME2: lambda x: datetime,
             mssql.DATETIMEOFFSET: lambda x: datetime,
             mssql.IMAGE: self.handle_string_type,
@@ -306,15 +313,15 @@
             sqlite.DATE: lambda x: date,
             sqlite.DATETIME: lambda x: datetime,
             sqlite.JSON: lambda x: Union[dict, list],
             sqlite.TIME: lambda x: time,
         }
 
     def get_pydantic_type(self, column_type: Any) -> Any:
-        """Given a 'Column.type' value, return a type supported by pydantic.
+        """Given a ``Column.type`` value, return a type supported by pydantic.
 
         Args:
             column_type: The type of the SQLColumn.
 
         Returns:
              A pydantic supported type.
         """
@@ -441,11 +448,14 @@
             An instantiated table instance.
         """
         return model_class(**kwargs)
 
     def to_openapi_schema(self, model_class: Type[DeclarativeMeta]) -> "Schema":
         """Given a model class, transform it into an OpenAPI schema class.
 
-        :param model_class: A table class.
-        :return: An :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.schema.Schema>` instance.
+        Args:
+            model_class: A table class.
+
+        Returns:
+            An :class:`OpenAPI <starlite.openapi.spec.schema.Schema>` instance.
         """
-        return OpenAPI310PydanticSchema(schema_class=self.to_data_container_class(model_class=model_class))
+        return SchemaDataContainer(data_container=self.to_data_container_class(model_class=model_class))
```

### Comparing `starlite-2.0.0a1/starlite/contrib/sqlalchemy_1/types.py` & `starlite-2.0.0a2/starlite/contrib/sqlalchemy_1/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,17 @@
     Optional,
     Protocol,
     Type,
     Union,
     runtime_checkable,
 )
 
+__all__ = ("SessionMakerInstanceProtocol", "SessionMakerTypeProtocol", "SQLAlchemyBinaryType")
+
+
 if TYPE_CHECKING:
     from sqlalchemy.engine import Connection, Engine
     from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
     from sqlalchemy.orm import Session
     from sqlalchemy.types import BINARY, VARBINARY, LargeBinary
```

### Comparing `starlite-2.0.0a1/starlite/controller.py` & `starlite-2.0.0a2/starlite/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from copy import copy
 from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, cast
 
+from starlite._layers.utils import narrow_response_cookies, narrow_response_headers
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.handlers.base import BaseRouteHandler
 from starlite.handlers.http_handlers import HTTPRouteHandler
-from starlite.handlers.utils import narrow_response_cookies, narrow_response_headers
 from starlite.handlers.websocket_handlers import WebsocketRouteHandler
 from starlite.utils import AsyncCallable, normalize_path
 from starlite.utils.helpers import unwrap_partial
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
+__all__ = ("Controller",)
+
 
+if TYPE_CHECKING:
     from starlite.datastructures import CacheControlHeader, ETag
+    from starlite.openapi.spec import SecurityRequirement
+    from starlite.response import Response
     from starlite.router import Router
     from starlite.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
         Dependencies,
         ExceptionHandlersMap,
         Guard,
         Middleware,
         OptionalSequence,
         ParametersMap,
         ResponseCookies,
-        ResponseType,
         TypeEncodersMap,
     )
     from starlite.types.composite_types import ResponseHeaders
 
 
 class Controller:
     """The Starlite Controller class.
@@ -53,105 +55,109 @@
         "owner",
         "parameters",
         "path",
         "response_class",
         "response_cookies",
         "response_headers",
         "security",
+        "signature_namespace",
         "tags",
         "type_encoders",
     )
 
     after_request: AfterRequestHookHandler | None
-    """A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed to any route handler.
+    """A sync or async function executed before a :class:`Request <.connection.Request>` is passed to any route handler.
 
     If this function returns a value, the request will not reach the route handler, and instead this value will be used.
     """
     after_response: AfterResponseHookHandler | None
     """A sync or async function called after the response has been awaited.
 
-    It receives the :class:`Request <starlite.connection.Request>` instance and should not return any values.
+    It receives the :class:`Request <.connection.Request>` instance and should not return any values.
     """
     before_request: BeforeRequestHookHandler | None
     """A sync or async function called immediately before calling the route handler.
 
-    It receives the :class:`Request <starlite.connection.Request>` instance and any non-``None`` return value is used for the
+    It receives the :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
     response, bypassing the route handler.
     """
     cache_control: CacheControlHeader | None
-    """A :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` header to add to route handlers of this
+    """A :class:`CacheControlHeader <.datastructures.CacheControlHeader>` header to add to route handlers of this
     controller.
 
     Can be overridden by route handlers.
     """
     dependencies: Dependencies | None
-    """A string keyed dictionary of dependency :class:`Provider <starlite.datastructures.Provide>` instances."""
+    """A string keyed dictionary of dependency :class:`Provider <.di.Provide>` instances."""
     etag: ETag | None
-    """An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` to add to route handlers of this controller.
+    """An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this controller.
 
     Can be overridden by route handlers.
     """
     exception_handlers: ExceptionHandlersMap | None
     """A map of handler functions to status codes and/or exception types."""
     guards: OptionalSequence[Guard]
-    """A sequence of :class:`Guard <starlite.types.Guard>` callables."""
+    """A sequence of :class:`Guard <.types.Guard>` callables."""
     middleware: OptionalSequence[Middleware]
-    """A sequence of :class:`Middleware <starlite.types.Middleware>`."""
+    """A sequence of :class:`Middleware <.types.Middleware>`."""
     opt: Mapping[str, Any] | None
-    """A string key mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or wherever
-    you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
+    """A string key mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or wherever you
+    have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
     """
     owner: Router
-    """The :class:`Router <starlite.router.Router>` or :class:`Starlite <starlite.app.Starlite>` app that owns the controller.
+    """The :class:`Router <.router.Router>` or :class:`Starlite <.app.Starlite>` app that owns the controller.
 
     This value is set internally by Starlite and it should not be set when subclassing the controller.
     """
     parameters: ParametersMap | None
-    """A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all application paths."""
+    """A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application paths."""
     path: str
     """A path fragment for the controller.
 
-    All route handlers under the controller will have the fragment appended to them. If not set it defaults to '/'.
+    All route handlers under the controller will have the fragment appended to them. If not set it defaults to ``/``.
     """
-    response_class: ResponseType | None
-    """A custom subclass of [starlite.response.Response] to be used as the default response for all route handlers under
-    the controller.
+    response_class: type[Response] | None
+    """A custom subclass of :class:`Response <.response.Response>` to be used as the default response for all route
+    handlers under the controller.
     """
     response_cookies: ResponseCookies | None
-    """A list of [Cookie](starlite.datastructures.Cookie] instances."""
+    """A list of :class:`Cookie <.datastructures.Cookie>` instances."""
     response_headers: ResponseHeaders | None
-    """A string keyed dictionary mapping :class:`ResponseHeader <starlite.datastructures.ResponseHeader>` instances."""
+    """A string keyed dictionary mapping :class:`ResponseHeader <.datastructures.ResponseHeader>` instances."""
     tags: OptionalSequence[str]
     """A sequence of string tags that will be appended to the schema of all route handlers under the controller."""
     security: OptionalSequence[SecurityRequirement]
     """A sequence of dictionaries that to the schema of all route handlers under the controller."""
+    signature_namespace: dict[str, Any]
+    """A mapping of names to types for use in forward reference resolution during signature modelling."""
     type_encoders: TypeEncodersMap | None
     """A mapping of types to callables that transform them into types supported for serialization."""
 
     def __init__(self, owner: Router) -> None:
         """Initialize a controller.
 
         Should only be called by routers as part of controller registration.
 
         Args:
-            owner: An instance of 'Router'
+            owner: An instance of :class:`Router <.router.Router>`
         """
         # Since functions set on classes are bound, we need replace the bound instance with the class version and wrap
         # it to ensure it does not get bound.
         for key in ("after_request", "after_response", "before_request"):
             cls_value = getattr(type(self), key, None)
             if callable(cls_value):
                 setattr(self, key, AsyncCallable(cls_value))
 
         for key in self.__slots__:
             if not hasattr(self, key):
                 setattr(self, key, None)
 
         self.response_cookies = narrow_response_cookies(self.response_cookies)
         self.response_headers = narrow_response_headers(self.response_headers)
+        self.signature_namespace = self.signature_namespace or {}
 
         self.path = normalize_path(self.path or "/")
         self.owner = owner
 
     def get_route_handlers(self) -> list[BaseRouteHandler]:
         """Get a controller's route handlers and set the controller as the handlers' owner.
 
@@ -178,17 +184,22 @@
         self.validate_route_handlers(route_handlers=route_handlers)
 
         return route_handlers
 
     def validate_route_handlers(self, route_handlers: list[BaseRouteHandler]) -> None:
         """Validate that the combination of path and decorator method or type are unique on the controller.
 
-        :param route_handlers: The controller's route handlers.
-        :raises: ``ImproperlyConfiguredException``
-        :return: None.
+        Args:
+            route_handlers: The controller's route handlers.
+
+        Raises:
+            ImproperlyConfiguredException
+
+        Returns:
+            None
         """
         paths: DefaultDict[str, set[str]] = defaultdict(set)
 
         for route_handler in route_handlers:
             if isinstance(route_handler, HTTPRouteHandler):
                 methods: set[str] = cast("set[str]", route_handler.http_methods)
             elif isinstance(route_handler, WebsocketRouteHandler):
```

### Comparing `starlite-2.0.0a1/starlite/data_extractors.py` & `starlite-2.0.0a2/starlite/data_extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, Literal, cast
 
 from typing_extensions import TypedDict
 
+from starlite._parsers import parse_cookie_string
 from starlite.connection.request import Request
 from starlite.datastructures.upload_file import UploadFile
 from starlite.enums import HttpMethod, RequestEncodingType
-from starlite.parsers import parse_cookie_string
+
+__all__ = ("ConnectionDataExtractor", "ExtractedRequestData", "ExtractedResponseData", "ResponseDataExtractor")
+
 
 if TYPE_CHECKING:
     from starlite.connection import ASGIConnection
     from starlite.types import Method
     from starlite.types.asgi_types import HTTPResponseBodyEvent, HTTPResponseStartEvent
 
 
@@ -395,18 +398,13 @@
                 :class:`HTTPResponseStartEvent <starlite.types.asgi_types.HTTPResponseStartEvent>`
                 and :class:`HTTPResponseBodyEvent <starlite.types.asgi_types.HTTPResponseBodyEvent>`.
 
         Returns:
             The Response's cookies dict.
         """
         cookie_string = ";".join(
-            list(  # noqa: C417
-                map(
-                    lambda x: x[1].decode("latin-1"),
-                    filter(lambda x: x[0].lower() == b"set-cookie", messages[0]["headers"]),
-                )
-            )
+            [x[1].decode("latin-1") for x in filter(lambda x: x[0].lower() == b"set-cookie", messages[0]["headers"])]
         )
         if cookie_string:
             parsed_cookies = parse_cookie_string(cookie_string)
             return _obfuscate(parsed_cookies, self.obfuscate_cookies) if self.obfuscate_cookies else parsed_cookies
         return {}
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/__init__.py` & `starlite-2.0.0a2/starlite/datastructures/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from starlite.datastructures.cookie import Cookie
 from starlite.datastructures.headers import (
     CacheControlHeader,
     ETag,
+    Header,
     Headers,
     MutableScopeHeaders,
 )
 from starlite.datastructures.multi_dicts import (
     FormMultiDict,
     ImmutableMultiDict,
     MultiDict,
+    MultiMixin,
 )
 from starlite.datastructures.response_header import ResponseHeader
 from starlite.datastructures.state import ImmutableState, State
 from starlite.datastructures.upload_file import UploadFile
 from starlite.datastructures.url import URL, Address
 
 __all__ = (
     "Address",
     "CacheControlHeader",
     "Cookie",
     "ETag",
     "FormMultiDict",
+    "Header",
     "Headers",
     "ImmutableMultiDict",
     "ImmutableState",
     "MultiDict",
+    "MultiMixin",
     "MutableScopeHeaders",
     "ResponseHeader",
     "State",
-    "URL",
     "UploadFile",
+    "URL",
 )
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/cookie.py` & `starlite-2.0.0a2/starlite/datastructures/cookie.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
 from http.cookies import SimpleCookie
 from typing import Any, Literal
 
+__all__ = ("Cookie",)
+
 
 @dataclass
 class Cookie:
-    """Container class for defining a cookie using the 'Set-Cookie' header.
+    """Container class for defining a cookie using the ``Set-Cookie`` header.
 
     See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie for more details regarding this header.
     """
 
     key: str
     """Key for the cookie."""
     path: str = "/"
     """Path fragment that must exist in the request url for the cookie to be valid.
 
-    Defaults to '/'.
+    Defaults to ``/``.
     """
     value: str | None = field(default=None)
     """Value for the cookie, if none given defaults to empty string."""
     max_age: int | None = field(default=None)
     """Maximal age of the cookie before its invalidated."""
     expires: int | None = field(default=None)
     """Expiration date as unix MS timestamp."""
     domain: str | None = field(default=None)
     """Domain for which the cookie is valid."""
     secure: bool | None = field(default=None)
     """Https is required for the cookie."""
     httponly: bool | None = field(default=None)
-    """Forbids javascript to access the cookie via 'Document.cookie'."""
+    """Forbids javascript to access the cookie via ``document.cookie``."""
     samesite: Literal["lax", "strict", "none"] = field(default="lax")
     """Controls whether or not a cookie is sent with cross-site requests.
 
     Defaults to 'lax'.
     """
     description: str | None = field(default=None)
     """Description of the response cookie header for OpenAPI documentation."""
@@ -42,40 +44,41 @@
     """Defines the Cookie instance as for OpenAPI documentation purpose only."""
 
     @property
     def simple_cookie(self) -> SimpleCookie:
         """Get a simple cookie object from the values.
 
         Returns:
-            A SimpleCookie instance.
+            A :class:`SimpleCookie <http.cookies.SimpleCookie>`
         """
         simple_cookie: SimpleCookie = SimpleCookie()
         simple_cookie[self.key] = self.value or ""
 
         namespace = simple_cookie[self.key]
         for key, value in self.dict.items():
             if key in {"key", "value"}:
                 continue
             if value is not None:
+                updated_key = key
                 if key == "max_age":
-                    key = "max-age"
-                namespace[key] = value
+                    updated_key = "max-age"
+                namespace[updated_key] = value
 
         return simple_cookie
 
     def to_header(self, **kwargs: Any) -> str:
         """Return a string representation suitable to be sent as HTTP headers.
 
         Args:
             **kwargs: Any kwargs to pass to the simple cookie output method.
         """
         return self.simple_cookie.output(**kwargs).strip()
 
     def to_encoded_header(self) -> tuple[bytes, bytes]:
-        """Create encoded header for ASGI send.
+        """Create encoded header for ASGI ``send``.
 
         Returns:
             A two tuple of bytes.
         """
         return b"set-cookie", self.to_header(header="").strip().encode("latin-1")
 
     @property
@@ -88,15 +91,15 @@
         return {
             k: v
             for k, v in asdict(self).items()
             if k not in {"documentation_only", "description", "__pydantic_initialised__"}
         }
 
     def __hash__(self) -> int:
-        return hash((self.key, self.path, self.domain or ""))
+        return hash((self.key, self.path, self.domain))
 
     def __eq__(self, other: Any) -> bool:
         """Determine whether two cookie instances are equal according to the cookie spec, i.e. hey have a similar path,
         domain and key.
 
         Args:
             other: An arbitrary value
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/headers.py` & `starlite-2.0.0a2/starlite/datastructures/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,20 @@
     cast,
 )
 
 from multidict import CIMultiDict, CIMultiDictProxy, MultiMapping
 from pydantic import BaseModel, Extra, Field, ValidationError, validator
 from typing_extensions import Annotated
 
+from starlite._parsers import parse_headers
 from starlite.datastructures.multi_dicts import MultiMixin
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.parsers import parse_headers
+
+__all__ = ("CacheControlHeader", "ETag", "Header", "Headers", "MutableScopeHeaders")
+
 
 if TYPE_CHECKING:
     from starlite.types.asgi_types import (
         HeaderScope,
         Message,
         RawHeaders,
         RawHeadersList,
@@ -86,20 +89,20 @@
         """
         # Since ``Headers`` are immutable, this can be cached
         header_list = self._header_list
         if not header_list:
             header_list = self._header_list = _encode_headers(
                 (key, value) for key in set(self) for value in self.getall(key)
             )
-        return header_list  # noqa: R504
+        return header_list
 
 
 class MutableScopeHeaders(MutableMapping):
-    """A case-insensitive, multidict-like structure that can be used to mutate headers
-    within a :class:`Scope <starlite.types.Scope>`
+    """A case-insensitive, multidict-like structure that can be used to mutate headers within a
+    :class:`Scope <.types.Scope>`
     """
 
     def __init__(self, scope: Optional["HeaderScope"] = None) -> None:
         """Initialize ``MutableScopeHeaders`` from a ``HeaderScope``.
 
         Args:
             scope: The ASGI connection scope.
@@ -114,15 +117,15 @@
             self.headers = []
 
     @classmethod
     def from_message(cls, message: "Message") -> "MutableScopeHeaders":
         """Construct a header from a message object.
 
         Args:
-            message: :class:`Message <starlite.types.Message>`.
+            message: :class:`Message <.types.Message>`.
 
         Returns:
             MutableScopeHeaders.
 
         Raises:
             ValueError: If the message does not have a ``headers`` key.
         """
@@ -374,12 +377,12 @@
         weak, value = match.group(1, 2)
         try:
             return cls(weak=bool(weak), value=value)
         except ValidationError as exc:
             raise ImproperlyConfiguredException from exc
 
     @validator("value", always=True)
-    def validate_value(cls, value: Any, values: Dict[str, Any]) -> Any:  # pylint: disable=no-self-argument
-        """Ensure that either value is set or the instance is for documentation_only."""
+    def validate_value(cls, value: Any, values: Dict[str, Any]) -> Any:
+        """Ensure that either value is set or the instance is for ``documentation_only``."""
         if values.get("documentation_only") or value is not None:
             return value
         raise ValueError("value must be set if documentation_only is false")
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/multi_dicts.py` & `starlite-2.0.0a2/starlite/datastructures/multi_dicts.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 from typing import Any, Generator, Generic, Iterable, Mapping, TypeVar
 
 from multidict import MultiDict as BaseMultiDict
 from multidict import MultiDictProxy, MultiMapping
 
 from starlite.datastructures.upload_file import UploadFile
 
+__all__ = ("FormMultiDict", "ImmutableMultiDict", "MultiDict", "MultiMixin")
+
+
 T = TypeVar("T")
 
 
 class MultiMixin(Generic[T], MultiMapping[T], ABC):
-    """Mixin providing common methods for multi dicts, used by.
-
-    :class:`ImmutableMultiDict <starlite.datastructures.multi_dicts.ImmutableMultiDict>` and
-    :class:`MultiDict <starlite.datastructures.multi_dicts.MultiDict>`
-    """
+    """Mixin providing common methods for multi dicts, used by :class:`ImmutableMultiDict` and :class:`MultiDict`"""
 
     def dict(self) -> dict[str, list[Any]]:
         """Return the multi-dict as a dict of lists.
 
         Returns:
             A dict of lists
         """
@@ -39,54 +38,49 @@
 
 class MultiDict(BaseMultiDict[T], MultiMixin[T], Generic[T]):
     """MultiDict, using :class:`MultiDict <multidict.MultiDictProxy>`."""
 
     def __init__(self, args: MultiMapping | Mapping[str, T] | Iterable[tuple[str, T]] | None = None) -> None:
         """Initialize ``MultiDict`` from a.
 
-        :class:`MultiMapping <multidict.MultiMapping>`, ``Mapping`` or an iterable of
-        tuples.
+        ``MultiMapping``, :class:`Mapping <typing.Mapping>` or an iterable of tuples.
 
         Args:
             args: Mapping-like structure to create the ``MultiDict`` from
         """
         super().__init__(args or {})
 
     def immutable(self) -> ImmutableMultiDict[T]:
         """Create an.
 
-        :class:`ImmutableMultiDict <starlite.datastructures.multi_dicts.ImmutableMultiDict>` view.
+        :class:`ImmutableMultiDict` view.
 
         Returns:
             An immutable multi dict
         """
         return ImmutableMultiDict[T](self)
 
 
 class ImmutableMultiDict(MultiDictProxy[T], MultiMixin[T], Generic[T]):
-    """Immutable MultiDict, using.
-
-    :class:`MultiDictProxy <multidict.MultiDictProxy>`.
-    """
+    """Immutable MultiDict, using class:`MultiDictProxy <multidict.MultiDictProxy>`."""
 
     def __init__(self, args: MultiMapping | Mapping[str, Any] | Iterable[tuple[str, Any]] | None = None) -> None:
         """Initialize ``ImmutableMultiDict`` from a.
 
-        :class:`MultiMapping <multidict.MultiMapping>`, ``Mapping`` or an iterable of
-        tuples.
+        ``MultiMapping``, :class:`Mapping <typing.Mapping>` or an iterable of tuples.
 
         Args:
             args: Mapping-like structure to create the ``ImmutableMultiDict`` from
         """
         super().__init__(BaseMultiDict(args or {}))
 
     def mutable_copy(self) -> MultiDict[T]:
         """Create a mutable copy as a.
 
-        :class:`MultiDict <starlite.datastructures.multi_dicts.MultiDict>`
+        :class:`MultiDict`
 
         Returns:
             A mutable multi dict
         """
         return MultiDict(list(self.multi_items()))
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/state.py` & `starlite-2.0.0a2/starlite/datastructures/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from copy import copy, deepcopy
 from threading import RLock
 from typing import Any, Callable, Generator, Iterable, Iterator, Mapping, MutableMapping
 
+__all__ = ("ImmutableState", "State")
+
 
 class ImmutableState(Mapping[str, Any]):
     """An object meant to store arbitrary state.
 
     It can be accessed using dot notation while exposing dict like functionalities.
     """
 
@@ -17,15 +19,16 @@
 
     def __init__(
         self, state: ImmutableState | Mapping[str, Any] | Iterable[tuple[str, Any]], deep_copy: bool = True
     ) -> None:
         """Initialize an ``ImmutableState`` instance.
 
         Args:
-             state: An object to initialize the state from. Can be a dict, an instance of 'ImmutableState', or a tuple of key value paris.
+             state: An object to initialize the state from. Can be a dict, an instance of :class:`ImmutableState`, or a tuple
+                of key value paris.
              deep_copy: Whether to 'deepcopy' the passed in state.
 
         Examples:
             .. code-block: python
 
                 from starlite.datastructures import ImmutableState
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/upload_file.py` & `starlite-2.0.0a2/starlite/datastructures/upload_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 from tempfile import SpooledTemporaryFile
 from typing import TYPE_CHECKING, Any
 
 from anyio.to_thread import run_sync
 
 from starlite.constants import ONE_MEGABYTE
-from starlite.openapi.enums import OpenAPIType
+from starlite.openapi.spec.enums import OpenAPIType
+
+__all__ = ("UploadFile",)
+
 
 if TYPE_CHECKING:
     from pydantic.fields import ModelField
 
 
 class UploadFile:
-    """Representation of a file upload, modifying the pydantic schema."""
+    """Representation of a file upload"""
 
     __slots__ = ("filename", "file", "content_type", "headers")
 
     def __init__(
         self,
         content_type: str,
         filename: str,
@@ -32,15 +35,15 @@
             filename: The filename.
             file_data: File data.
             headers: Any attached headers.
             max_spool_size: The size above which the temporary file will be rolled to disk.
         """
         self.filename = filename
         self.content_type = content_type
-        self.file = SpooledTemporaryFile(max_size=max_spool_size)  # pylint: disable=consider-using-with
+        self.file = SpooledTemporaryFile(max_size=max_spool_size)
         self.headers = headers or {}
 
         if file_data:
             self.file.write(file_data)
             self.file.seek(0)
 
     @property
```

### Comparing `starlite-2.0.0a1/starlite/datastructures/url.py` & `starlite-2.0.0a2/starlite/datastructures/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, NamedTuple, cast
 from urllib.parse import SplitResult, urlencode, urlsplit, urlunsplit
 
+from starlite._parsers import parse_query_string
 from starlite.datastructures import MultiDict
-from starlite.parsers import parse_query_string
 from starlite.types import Empty
 
+__all__ = ("Address", "URL")
+
+
 if TYPE_CHECKING:
     from starlite.types import EmptyType, Scope
 
 _DEFAULT_SCHEME_PORTS = {"http": 80, "https": 443, "ftp": 21, "ws": 80, "wss": 443}
 
 
 class Address(NamedTuple):
@@ -153,15 +156,15 @@
                 fragment=fragment,
                 query=query,
             )
         )
 
     @classmethod
     def from_scope(cls, scope: Scope) -> URL:
-        """Construct a URL from a :class:`Scope <starlite.types.Scope>`
+        """Construct a URL from a :class:`Scope <.types.Scope>`
 
         Args:
             scope: A scope
 
         Returns:
             A URL
         """
@@ -219,21 +222,21 @@
             path=path or self.path,
             query=query or self.query,
             fragment=fragment or self.fragment,
         )
 
     @property
     def query_params(self) -> MultiDict:
-        """Query parameters of a URL as a :class:`MultiDict <multidict.MultiDict>`
+        """Query parameters of a URL as a :class:`MultiDict <.datastructures.multi_dicts.MultiDict>`
 
         Returns:
-            A :class:`MultiDict <multidict.MultiDict>` with query parameters
+            A :class:`MultiDict <.datastructures.multi_dicts.MultiDict>` with query parameters
 
         Notes:
-            - The returned `MultiDict` is mutable, :class:`URL` itself is *immutable*,
+            - The returned ``MultiDict`` is mutable, :class:`URL` itself is *immutable*,
                 therefore mutating the query parameters will not directly mutate the ``URL``.
                 If you want to modify query parameters, make  modifications in the
                 multidict and pass them back to :meth:`with_replacements`
         """
         if self._query_params is Empty:
             self._query_params = MultiDict(parse_query_string(query_string=self.query.encode()))
         return cast("MultiDict", self._query_params)
```

### Comparing `starlite-2.0.0a1/starlite/di.py` & `starlite-2.0.0a2/starlite/di.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from inspect import isclass
 from typing import TYPE_CHECKING, Any
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.types import Empty
 from starlite.utils import Ref, is_async_callable
 
+__all__ = ("Provide",)
+
+
 if TYPE_CHECKING:
-    from starlite.signature import SignatureModel
+    from starlite._signature import SignatureModel
     from starlite.types import AnyCallable
 
 
 class Provide:
     """Wrapper class for dependency injection"""
 
     __slots__ = (
```

### Comparing `starlite-2.0.0a1/starlite/dto.py` & `starlite-2.0.0a2/starlite/dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 
 from pydantic import BaseConfig, BaseModel, create_model
 from pydantic.fields import SHAPE_SINGLETON, ModelField, Undefined
 from pydantic.generics import GenericModel
 from pydantic_factories import ModelFactory
 
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.plugins import SerializationPluginProtocol
-from starlite.plugins.base import get_plugin_for_value
+from starlite.plugins import SerializationPluginProtocol, get_plugin_for_value
 from starlite.utils import (
     convert_dataclass_to_model,
     convert_typeddict_to_model,
     is_async_callable,
-    is_dataclass_class_or_instance,
+    is_dataclass_class,
     is_typed_dict,
 )
 
+__all__ = ("DTO", "DTOFactory")
+
+
 if TYPE_CHECKING:
     from typing import Awaitable
 
 
 def get_field_type(model_field: ModelField) -> Any:
     """Given a model field instance, return the correct type.
 
@@ -94,15 +96,15 @@
                 )
             values = cast("Dict[str, Any]", result)
         elif isinstance(model_instance, BaseModel):
             values = model_instance.dict()
         elif isinstance(model_instance, dict):
             values = dict(model_instance)  # copy required as `_from_value_mapping()`` mutates ``values`.
         else:
-            values = asdict(model_instance)  # pyright: ignore
+            values = asdict(model_instance)  # type:ignore[call-overload]
         return cls._from_value_mapping(mapping=values)
 
     @classmethod
     async def from_model_instance_async(cls, model_instance: T) -> "DTO[T]":
         """Given an instance of the source model, create an instance of the given DTO subclass asynchronously.
 
         Args:
@@ -178,37 +180,33 @@
 
         .. code-block: python
 
             class MyClass(BaseModel):
                 first: int
                 second: int
 
-
             MyClassDTO = DTOFactory()(
                 MyClass, exclude=["first"], field_mapping={"second": ("third", float)}
             )
 
-
         ``MyClassDTO`` is now equal to this:
 
         .. code-block: python
 
             class MyClassDTO(BaseModel):
                 third: float
 
-
         It can be used as a regular pydantic model:
 
         .. code-block: python
 
             @post(path="/my-path")
             def create_obj(data: MyClassDTO) -> MyClass:
                 ...
 
-
         This will affect parsing, validation and how OpenAPI schema is generated exactly like when using a pydantic model.
 
         Note: Although the value generated is a pydantic factory, because it is being generated programmatically,
         it's currently not possible to extend editor auto-complete for the DTO properties - it will be typed as a
         Pydantic BaseModel, but no attributes will be inferred in the editor.
 
         Args:
@@ -218,14 +216,15 @@
             exclude (list[str] | None): Names of attributes on ``source``. Named Attributes will not have a field
                 generated on the resultant pydantic model.
             field_mapping (dict[str, str | tuple[str, Any]] | None): Keys are names of attributes on ``source``. Values
                 are either a ``str`` to rename an attribute, or tuple `(str, Any)` to remap both name and type of the
                 attribute.
             field_definitions (dict[str, tuple[Any, Any]] | None): Add fields to the model that don't exist on ``source``.
                 These are passed as kwargs to `pydantic.create_model()`.
+            base (type[DTO] | None): Base class for the generated pydantic model.
 
         Returns:
             Type[DTO[T]]
 
         Raises:
             ImproperlyConfiguredException: If ``source`` is not a pydantic model, :class:`TypedDict <typing.TypedDict>`
                 or dataclass, and there is no plugin registered for its type.
@@ -237,17 +236,21 @@
         field_definitions = self._populate_field_definitions(exclude, field_definitions, field_mapping, fields)
         dto = cast(
             "Type[DTO[T]]", create_model(name, __base__=base, **field_definitions)  # type:ignore[call-overload]
         )
         dto.dto_source_model = source
         dto.dto_source_plugin = plugin
         dto.dto_field_mapping = {}
-        for key, value in field_mapping.items():
-            if not isinstance(value, str):
-                value = value[0]
+        for key, value_tuple in field_mapping.items():
+            if isinstance(value_tuple, tuple):
+                value = value_tuple[0]
+            elif isinstance(value_tuple, str):
+                value = value_tuple
+            else:
+                raise TypeError(f"Expected a string or tuple containing a string, but got {value_tuple!r}")
             dto.dto_field_mapping[value] = key
         return dto
 
     def _get_fields_from_source(
         self, source: Type[T]  # pyright: ignore
     ) -> Tuple[Dict[str, ModelField], Optional[SerializationPluginProtocol]]:
         """Convert a ``BaseModel`` subclass, :class:`TypedDict <typing.TypedDict>`, ``dataclass`` or any other type that
@@ -259,15 +262,15 @@
             fields = model.__fields__
 
             return fields, plugin  # type: ignore
 
         if issubclass(source, BaseModel):
             source.update_forward_refs()
             fields = source.__fields__
-        elif is_dataclass_class_or_instance(source):
+        elif is_dataclass_class(source):
             fields = convert_dataclass_to_model(source).__fields__
         elif is_typed_dict(source):
             fields = convert_typeddict_to_model(source).__fields__
 
         if fields:
             return fields, plugin
```

### Comparing `starlite-2.0.0a1/starlite/enums.py` & `starlite-2.0.0a2/starlite/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 from enum import Enum
 
+__all__ = (
+    "CompressionEncoding",
+    "HttpMethod",
+    "MediaType",
+    "OpenAPIMediaType",
+    "ParamType",
+    "RequestEncodingType",
+    "ScopeType",
+)
+
 
 class HttpMethod(str, Enum):
     """An Enum for HTTP methods."""
 
     DELETE = "DELETE"
     GET = "GET"
     HEAD = "HEAD"
```

### Comparing `starlite-2.0.0a1/starlite/events/listener.py` & `starlite-2.0.0a2/starlite/events/listener.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.utils import AsyncCallable
 
+__all__ = ("EventListener", "listener")
+
+
 if TYPE_CHECKING:
     from starlite.types import AnyCallable
 
 
 class EventListener:
     """Decorator for event listeners"""
 
     __slots__ = ("event_ids", "fn", "listener_id")
 
     fn: AsyncCallable[Any, Any]
 
     def __init__(self, *event_ids: str):
         """Create a decorator for event handlers.
 
-        :param event_id: The id of the event to listen to or a list of event ids to listen to.
+        Args:
+            *event_ids: The id of the event to listen to or a list of
+                event ids to listen to.
         """
-        self.event_ids: list[str] = list(event_ids)
+        self.event_ids: frozenset[str] = frozenset(event_ids)
 
     def __call__(self, fn: AnyCallable) -> EventListener:
         """Decorate a callable by wrapping it inside an instance of EventListener.
 
-        :param fn: Callable to decorate.
-        :return: An instance of EventListener
+        Args:
+            fn: Callable to decorate.
+
+        Returns:
+            An instance of EventListener
         """
         if not callable(fn):
             raise ImproperlyConfiguredException("EventListener instance should be called as a decorator on a callable")
 
         self.fn = AsyncCallable(fn)
 
         return self
 
+    def __hash__(self) -> int:
+        return hash(self.event_ids) + hash(self.fn)
+
 
 listener = EventListener
```

### Comparing `starlite-2.0.0a1/starlite/exceptions/__init__.py` & `starlite-2.0.0a2/starlite/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/exceptions/base_exceptions.py` & `starlite-2.0.0a2/starlite/exceptions/base_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Any
 
+__all__ = ("MissingDependencyException", "SerializationException", "StarliteException")
+
 
 class StarliteException(Exception):
     """Base exception class from which all Starlite exceptions inherit."""
 
     detail: str
 
     def __init__(self, *args: Any, detail: str = "") -> None:
         """Initialize ``StarliteException``.
 
         Args:
-            *args (Any): args are cast to ``str`` before passing to `Exception.__init__()`
-            detail (str, optional): detail of the exception.
+            *args: args are converted to :class:`str` before passing to :class:`Exception`
+            detail: detail of the exception.
         """
         self.detail = detail
         super().__init__(*(str(arg) for arg in args if arg), detail)
 
     def __repr__(self) -> str:
         if self.detail:
             return f"{self.__class__.__name__} - {self.detail}"
```

### Comparing `starlite-2.0.0a1/starlite/exceptions/websocket_exceptions.py` & `starlite-2.0.0a2/starlite/exceptions/websocket_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any
 
 from starlite.exceptions.base_exceptions import StarliteException
 from starlite.status_codes import WS_1000_NORMAL_CLOSURE
 
+__all__ = ("WebSocketDisconnect", "WebSocketException")
+
 
 class WebSocketException(StarliteException):
     """Exception class for websocket related events."""
 
     code: int
     """Exception code.
```

### Comparing `starlite-2.0.0a1/starlite/file_system.py` & `starlite-2.0.0a2/starlite/file_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,43 @@
 from anyio import AsyncFile, Path, open_file
 from anyio.to_thread import run_sync
 
 from starlite.exceptions import InternalServerException, NotAuthorizedException
 from starlite.types.file_types import FileSystemProtocol
 from starlite.utils.sync import is_async_callable
 
+__all__ = ("BaseLocalFileSystem", "FileSystemAdapter")
+
+
 if TYPE_CHECKING:
     from os import stat_result
 
     from _typeshed import OpenBinaryMode
 
     from starlite.types import PathType
     from starlite.types.file_types import FileInfo
 
 
 class BaseLocalFileSystem(FileSystemProtocol):
     """Base class for a local file system."""
 
-    async def info(self, path: "PathType", **kwargs: Any) -> "FileInfo":  # pylint: disable=W0236
+    async def info(self, path: "PathType", **kwargs: Any) -> "FileInfo":
         """Retrieve information about a given file path.
 
         Args:
             path: A file path.
             **kwargs: Any additional kwargs.
 
         Returns:
             A dictionary of file info.
         """
         result = await Path(path).stat()
         return await FileSystemAdapter.parse_stat_result(path=path, result=result)
 
-    async def open(  # pylint: disable=invalid-overridden-method
-        self,
-        file: "PathType",
-        mode: str,
-        buffering: int = -1,
-    ) -> AsyncFile[AnyStr]:
+    async def open(self, file: "PathType", mode: str, buffering: int = -1) -> AsyncFile[AnyStr]:
         """Return a file-like object from the filesystem.
 
         Notes:
             - The return value must be a context-manager
 
         Args:
             file: Path to the target file.
```

### Comparing `starlite-2.0.0a1/starlite/handlers/asgi_handlers.py` & `starlite-2.0.0a2/starlite/handlers/asgi_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 from inspect import Signature
 from typing import TYPE_CHECKING, Any, Mapping, Sequence
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.handlers.base import BaseRouteHandler
 from starlite.utils import Ref, is_async_callable
 
+__all__ = ("ASGIRouteHandler", "asgi")
+
+
 if TYPE_CHECKING:
-    from starlite.types import MaybePartial  # nopycln: import # noqa: F401
-    from starlite.types import AsyncAnyCallable, ExceptionHandlersMap, Guard
+    from starlite.types import (
+        AsyncAnyCallable,
+        ExceptionHandlersMap,
+        Guard,
+        MaybePartial,  # noqa: F401
+    )
 
 
 class ASGIRouteHandler(BaseRouteHandler["ASGIRouteHandler"]):
     """ASGI Route Handler decorator.
 
     Use this decorator to decorate ASGI applications.
     """
@@ -26,36 +33,49 @@
         *,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
         is_mount: bool = False,
         is_static: bool = False,
+        signature_namespace: Mapping[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``ASGIRouteHandler``.
 
         Args:
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
             name: A string identifying the route handler.
-            opt: A string key mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            path: A path fragment for the route handler function or a list of path fragments. If not given defaults to '/'
-            is_mount: A boolean dictating whether the handler's paths should be regarded as mount paths. Mount path accept
-                any arbitrary paths that begin with the defined prefixed path. For example, a mount with the path `/some-path/`
-                will accept requests for `/some-path/` and any sub path under this, e.g. `/some-path/sub-path/` etc.
+            opt: A string key mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or
+                :class:`ASGI Scope <.types.Scope>`.
+            path: A path fragment for the route handler function or a list of path fragments. If not given defaults to
+                ``/``
+            is_mount: A boolean dictating whether the handler's paths should be regarded as mount paths. Mount path
+                accept any arbitrary paths that begin with the defined prefixed path. For example, a mount with the path
+                ``/some-path/`` will accept requests for ``/some-path/`` and any sub path under this, e.g.
+                ``/some-path/sub-path/`` etc.
             is_static: A boolean dictating whether the handler's paths should be regarded as static paths. Static paths
                 are used to deliver static files.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         self.is_mount = is_mount or is_static
         self.is_static = is_static
-        super().__init__(path, exception_handlers=exception_handlers, guards=guards, name=name, opt=opt, **kwargs)
+        super().__init__(
+            path,
+            exception_handlers=exception_handlers,
+            guards=guards,
+            name=name,
+            opt=opt,
+            signature_namespace=signature_namespace,
+            **kwargs,
+        )
 
     def __call__(self, fn: AsyncAnyCallable) -> ASGIRouteHandler:
         """Replace a function with itself."""
         self.fn = Ref["MaybePartial[AsyncAnyCallable]"](fn)
         self.signature = Signature.from_callable(fn)
         self._validate_handler_function()
         return self
```

### Comparing `starlite-2.0.0a1/starlite/handlers/base.py` & `starlite-2.0.0a2/starlite/handlers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 from __future__ import annotations
 
 from copy import copy
 from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar, cast
 
-from starlite.di import Provide
+from starlite._signature.models import SignatureField
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.signature.models import SignatureField
-from starlite.types import (
-    Dependencies,
-    Empty,
-    EmptyType,
-    ExceptionHandlersMap,
-    Guard,
-    Middleware,
-    TypeEncodersMap,
-)
-from starlite.types.composite_types import MaybePartial
+from starlite.types import Dependencies, Empty, EmptyType, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
 from starlite.utils import AsyncCallable, Ref, get_name, normalize_path
 from starlite.utils.helpers import unwrap_partial
 
+__all__ = ("BaseRouteHandler",)
+
+
 if TYPE_CHECKING:
     from inspect import Signature
 
+    from starlite._signature.models import SignatureModel
     from starlite.connection import ASGIConnection
     from starlite.controller import Controller
+    from starlite.di import Provide
     from starlite.params import ParameterKwarg
     from starlite.router import Router
-    from starlite.signature.models import SignatureModel
     from starlite.types import AnyCallable, ExceptionHandler
+    from starlite.types.composite_types import MaybePartial
 
 T = TypeVar("T", bound="BaseRouteHandler")
 
 
 class BaseRouteHandler(Generic[T]):
     """Base route handler.
 
@@ -41,69 +36,77 @@
     fn: Ref[MaybePartial[AnyCallable]]
     signature: Signature
 
     __slots__ = (
         "_resolved_dependencies",
         "_resolved_guards",
         "_resolved_layered_parameters",
+        "_resolved_signature_namespace",
         "_resolved_type_encoders",
         "dependencies",
         "exception_handlers",
         "fn",
         "guards",
         "middleware",
         "name",
         "opt",
         "owner",
         "paths",
         "signature",
         "signature_model",
+        "signature_namespace",
         "type_encoders",
     )
 
     def __init__(
         self,
         path: str | Sequence[str] | None = None,
         *,
         dependencies: Dependencies | None = None,
         exception_handlers: ExceptionHandlersMap | None = None,
         guards: Sequence[Guard] | None = None,
         middleware: Sequence[Middleware] | None = None,
         name: str | None = None,
         opt: Mapping[str, Any] | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``HTTPRouteHandler``.
 
         Args:
-            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults to '/'
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
+            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
+                to ``/``
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or
+                :class:`ASGI Scope <.types.Scope>`.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         self._resolved_dependencies: dict[str, Provide] | EmptyType = Empty
         self._resolved_guards: list[Guard] | EmptyType = Empty
         self._resolved_layered_parameters: dict[str, SignatureField] | EmptyType = Empty
+        self._resolved_signature_namespace: dict[str, Any] | EmptyType = Empty
         self._resolved_type_encoders: TypeEncodersMap | EmptyType = Empty
 
         self.dependencies = dependencies
         self.exception_handlers = exception_handlers
         self.guards = guards
         self.middleware = middleware
         self.name = name
         self.opt = dict(opt or {})
         self.owner: Controller | Router | None = None
         self.signature_model: type[SignatureModel] | None = None
+        self.signature_namespace = signature_namespace or {}
         self.paths = (
             {normalize_path(p) for p in path}
             if path and isinstance(path, list)
             else {normalize_path(path or "/")}  # type: ignore
         )
         self.opt.update(**kwargs)
         self.type_encoders = type_encoders
@@ -123,21 +126,21 @@
             raise ImproperlyConfiguredException("cannot access handler name before setting the handler function")
         return get_name(unwrap_partial(self.fn.value))
 
     @property
     def dependency_name_set(self) -> set[str]:
         """Set of all dependency names provided in the handler's ownership layers."""
         layered_dependencies = (layer.dependencies or {} for layer in self.ownership_layers)
-        return {name for layer in layered_dependencies for name in layer.keys()}
+        return {name for layer in layered_dependencies for name in layer}
 
     @property
     def ownership_layers(self) -> list[T | Controller | Router]:
         """Return the handler layers from the app down to the route handler.
 
-        app -> ... -> route handler
+        ``app -> ... -> route handler``
         """
         layers = []
 
         cur: Any = self
         while cur:
             layers.append(cur)
             cur = cur.owner
@@ -202,15 +205,16 @@
                     self._resolved_dependencies[key] = value
 
         return cast("dict[str, Provide]", self._resolved_dependencies)
 
     def resolve_middleware(self) -> list[Middleware]:
         """Build the middleware stack for the RouteHandler and return it.
 
-        The middlewares are added from top to bottom (app -> router -> controller -> route handler) and then reversed.
+        The middlewares are added from top to bottom (``app -> router -> controller -> route handler``) and then
+        reversed.
         """
         resolved_middleware: list[Middleware] = []
         for layer in self.ownership_layers:
             resolved_middleware.extend(layer.middleware or [])
         return list(reversed(resolved_middleware))
 
     def resolve_exception_handlers(self) -> ExceptionHandlersMap:
@@ -222,24 +226,38 @@
         for layer in self.ownership_layers:
             resolved_exception_handlers.update(layer.exception_handlers or {})
         return resolved_exception_handlers
 
     def resolve_opts(self) -> None:
         """Build the route handler opt dictionary by going from top to bottom.
 
-        If multiple layers define the same key, the value from the closest layer to the response handler will take
-        precedence.
+        When merging keys from multiple layers, if the same key is defined by multiple layers, the value from the
+        layer closest to the response handler will take precedence.
         """
 
         opt: dict[str, Any] = {}
         for layer in self.ownership_layers:
             opt.update(layer.opt or {})
 
         self.opt = opt
 
+    def resolve_signature_namespace(self) -> dict[str, Any]:
+        """Build the route handler signature namespace dictionary by going from top to bottom.
+
+        When merging keys from multiple layers, if the same key is defined by multiple layers, the value from the
+        layer closest to the response handler will take precedence.
+        """
+        if self._resolved_layered_parameters is Empty:
+            ns: dict[str, Any] = {}
+            for layer in self.ownership_layers:
+                ns.update(layer.signature_namespace)
+
+            self._resolved_signature_namespace = ns
+        return cast("dict[str, Any]", self._resolved_signature_namespace)
+
     async def authorize_connection(self, connection: "ASGIConnection") -> None:
         """Ensure the connection is authorized by running all the route guards in scope."""
         for guard in self.resolve_guards():
             await guard(connection, copy(self))  # type: ignore
 
     @staticmethod
     def _validate_dependency_is_unique(dependencies: dict[str, Provide], key: str, provider: Provide) -> None:
```

### Comparing `starlite-2.0.0a1/starlite/handlers/http_handlers/_utils.py` & `starlite-2.0.0a2/starlite/handlers/http_handlers/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,84 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from inspect import isawaitable
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, Any, Sequence, cast
 
 from typing_extensions import get_args
 
-from starlite.datastructures import Cookie, ResponseHeader
 from starlite.dto import DTO
 from starlite.enums import HttpMethod
 from starlite.exceptions import ValidationException
-from starlite.plugins.base import get_plugin_for_value
+from starlite.plugins import get_plugin_for_value
 from starlite.status_codes import HTTP_200_OK, HTTP_201_CREATED, HTTP_204_NO_CONTENT
 from starlite.utils import (
     annotation_is_iterable_of_type,
     is_async_callable,
     is_class_and_subclass,
 )
 
 if TYPE_CHECKING:
-    from typing import Any, Sequence
-
     from starlite.app import Starlite
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.connection import Request
+    from starlite.datastructures import Cookie, ResponseHeader
     from starlite.plugins import SerializationPluginProtocol
     from starlite.response import Response
     from starlite.response_containers import ResponseContainer
     from starlite.types import (
         AfterRequestHookHandler,
         ASGIApp,
         AsyncAnyCallable,
         Method,
         ResponseType,
         TypeEncodersMap,
     )
 
+__all__ = (
+    "create_data_handler",
+    "create_generic_asgi_response_handler",
+    "create_response_container_handler",
+    "create_response_handler",
+    "filter_cookies",
+    "get_default_status_code",
+    "normalize_headers",
+    "normalize_http_method",
+    "normalize_response_data",
+)
+
 
 def create_data_handler(
     after_request: AfterRequestHookHandler | None,
     background: BackgroundTask | BackgroundTasks | None,
     cookies: frozenset[Cookie],
     headers: frozenset[ResponseHeader],
     media_type: str,
     response_class: ResponseType,
     return_annotation: Any,
     status_code: int,
     type_encoders: TypeEncodersMap | None,
 ) -> AsyncAnyCallable:
-    """Create a handler function for arbitrary data."""
+    """Create a handler function for arbitrary data.
+
+    Args:
+        after_request: An after request handler.
+        background: A background task or background tasks.
+        cookies: A set of pre-defined cookies.
+        headers: A set of response headers.
+        media_type: The response media type.
+        response_class: The response class to use.
+        return_annotation: The return annotation.
+        status_code: The response status code.
+        type_encoders: A mapping of types to encoder functions.
+
+    Returns:
+        A handler function.
+
+    """
     normalized_headers = [
         (name.lower().encode("latin-1"), value.encode("latin-1")) for name, value in normalize_headers(headers).items()
     ]
     cookie_headers = [cookie.to_encoded_header() for cookie in cookies if not cookie.documentation_only]
     raw_headers = [*normalized_headers, *cookie_headers]
     is_dto_annotation = is_class_and_subclass(return_annotation, DTO)
     is_dto_iterable_annotation = annotation_is_iterable_of_type(return_annotation, DTO)
@@ -89,25 +115,40 @@
             data = await normalize_response_data(data=data, plugins=plugins)
 
         return await create_response(data=data)
 
     return handler
 
 
-@lru_cache(1024)
 def filter_cookies(local_cookies: frozenset[Cookie], layered_cookies: frozenset[Cookie]) -> list[Cookie]:
-    """Given two sets of cookies, return a unique list of cookies, that are not marked as documentation_only."""
+    """Given two sets of cookies, return a unique list of cookies, that are not marked as documentation_only.
+
+    Args:
+        local_cookies: Cookies returned from the local scope.
+        layered_cookies: Cookies returned from the layers.
+
+    Returns:
+        A unified list of cookies
+    """
     return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]
 
 
 def create_generic_asgi_response_handler(
     after_request: AfterRequestHookHandler | None,
     cookies: frozenset[Cookie],
 ) -> AsyncAnyCallable:
-    """Create a handler function for Responses."""
+    """Create a handler function for Responses.
+
+    Args:
+        after_request: An after request handler.
+        cookies: A set of pre-defined cookies.
+
+    Returns:
+        A handler function.
+    """
 
     async def handler(data: "ASGIApp", **kwargs: Any) -> "ASGIApp":
         if hasattr(data, "set_cookie"):
             for cookie in cookies:
                 data.set_cookie(**cookie.dict)
         return await after_request(data) if after_request else data  # type: ignore
 
@@ -159,15 +200,26 @@
 def create_response_container_handler(
     after_request: AfterRequestHookHandler | None,
     cookies: frozenset[Cookie],
     headers: frozenset[ResponseHeader],
     media_type: str,
     status_code: int,
 ) -> AsyncAnyCallable:
-    """Create a handler function for ResponseContainers."""
+    """Create a handler function for ResponseContainers.
+
+    Args:
+        after_request: An after request handler.
+        cookies: A set of pre-defined cookies.
+        headers: A set of response headers.
+        media_type: The response media type.
+        status_code: The response status code.
+
+    Returns:
+        A handler function.
+    """
     normalized_headers = normalize_headers(headers)
 
     async def handler(data: ResponseContainer, app: "Starlite", request: "Request", **kwargs: Any) -> "ASGIApp":
         response = data.to_response(
             app=app,
             headers={**normalized_headers, **data.headers},
             status_code=status_code,
@@ -180,15 +232,23 @@
     return handler
 
 
 def create_response_handler(
     after_request: AfterRequestHookHandler | None,
     cookies: frozenset[Cookie],
 ) -> AsyncAnyCallable:
-    """Create a handler function for Starlite Responses."""
+    """Create a handler function for Starlite Responses.
+
+    Args:
+        after_request: An after request handler.
+        cookies: A set of pre-defined cookies.
+
+    Returns:
+        A handler function.
+    """
 
     async def handler(data: Response, **kwargs: Any) -> "ASGIApp":
         data.cookies = filter_cookies(frozenset(data.cookies), cookies)
         return await after_request(data) if after_request else data  # type: ignore
 
     return handler
 
@@ -204,18 +264,15 @@
     """
     output: set[str] = set()
 
     if isinstance(http_methods, str):
         http_methods = [http_methods]  # pyright: ignore
 
     for method in http_methods:
-        if isinstance(method, HttpMethod):
-            method_name = method.value.upper()
-        else:
-            method_name = method.upper()
+        method_name = method.value.upper() if isinstance(method, HttpMethod) else method.upper()
         if method_name not in HTTP_METHOD_NAMES:
             raise ValidationException(f"Invalid HTTP method: {method_name}")
         output.add(method_name)
 
     return cast("set[Method]", output)
```

### Comparing `starlite-2.0.0a1/starlite/handlers/http_handlers/base.py` & `starlite-2.0.0a2/starlite/handlers/http_handlers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 from __future__ import annotations
 
 from enum import Enum
 from inspect import Signature
 from typing import TYPE_CHECKING, AnyStr, Mapping, cast
 
+from typing_extensions import TypedDict
+
+from starlite._layers.utils import narrow_response_cookies, narrow_response_headers
+from starlite._signature.utils import get_signature_model
 from starlite.constants import REDIRECT_STATUS_CODES
-from starlite.datastructures import Cookie, ResponseHeader
+from starlite.datastructures.cookie import Cookie
+from starlite.datastructures.response_header import ResponseHeader
 from starlite.enums import HttpMethod, MediaType
 from starlite.exceptions import (
     HTTPException,
     ImproperlyConfiguredException,
     ValidationException,
 )
+from starlite.handlers.base import BaseRouteHandler
+from starlite.handlers.http_handlers._utils import (
+    create_data_handler,
+    create_generic_asgi_response_handler,
+    create_response_container_handler,
+    create_response_handler,
+    get_default_status_code,
+    normalize_http_method,
+)
 from starlite.response import FileResponse, Response
 from starlite.response_containers import File, Redirect, ResponseContainer
 from starlite.status_codes import HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED
 from starlite.types import (
     AfterRequestHookHandler,
     AfterResponseHookHandler,
     AnyCallable,
@@ -31,56 +45,46 @@
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
     TypeEncodersMap,
 )
 from starlite.utils import AsyncCallable, Ref, is_async_callable, is_class_and_subclass
 
-from ..base import BaseRouteHandler
-from ..utils import narrow_response_cookies, narrow_response_headers
-from ._utils import (
-    create_data_handler,
-    create_generic_asgi_response_handler,
-    create_response_container_handler,
-    create_response_handler,
-    get_default_status_code,
-    normalize_http_method,
-)
-
 if TYPE_CHECKING:
     from typing import Any, Awaitable, Callable, Sequence
 
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
-
     from starlite.app import Starlite
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.connection import Request
     from starlite.datastructures import CacheControlHeader, ETag
     from starlite.datastructures.headers import Header
     from starlite.di import Provide
     from starlite.openapi.datastructures import ResponseSpec
+    from starlite.openapi.spec import SecurityRequirement
     from starlite.plugins import SerializationPluginProtocol
-    from starlite.types import MaybePartial  # nopycln: import # noqa: F401
+    from starlite.types import MaybePartial  # noqa: F401
 
-__all__ = (
-    "HTTPRouteHandler",
-    "route",
-)
+__all__ = ("HTTPRouteHandler", "route")
+
+
+class ResponseHandlerMap(TypedDict):
+    default_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
+    response_type_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
 
 
 class HTTPRouteHandler(BaseRouteHandler["HTTPRouteHandler"]):
     """HTTP Route Decorator.
 
     Use this decorator to decorate an HTTP handler with multiple methods.
     """
 
     __slots__ = (
         "_resolved_after_response",
         "_resolved_before_request",
-        "_resolved_response_handler",
+        "_response_handler_mapping",
         "after_request",
         "after_response",
         "background",
         "before_request",
         "cache",
         "cache_control",
         "cache_key_builder",
@@ -141,62 +145,65 @@
         deprecated: bool = False,
         description: str | None = None,
         include_in_schema: bool = True,
         operation_id: str | None = None,
         raises: Sequence[type[HTTPException]] | None = None,
         response_description: str | None = None,
         responses: Mapping[int, ResponseSpec] | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         security: Sequence[SecurityRequirement] | None = None,
         summary: str | None = None,
         tags: Sequence[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``HTTPRouteHandler``.
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
-                bypassing the route handler.
-            cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
-                of seconds (e.g. ``120``) to cache the response.
+                the :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for the
+                response, bypassing the route handler.
+            cache: Enables response caching if configured on the application level. Valid values are ``True`` or a
+                number of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
-                :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
-                route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
-                valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
+                :class:`HttpMethod <.enums.HttpMethod>` or a list of these that correlates to the methods the route
+                handler function should handle.
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a valid IANA
+                Media-Type.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or
+                :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
             content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
             content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
@@ -223,14 +230,15 @@
             path,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
             guards=guards,
             middleware=middleware,
             name=name,
             opt=opt,
+            signature_namespace=signature_namespace,
             type_encoders=type_encoders,
             **kwargs,
         )
 
         self.after_request = AsyncCallable(after_request) if after_request else None  # type: ignore[arg-type]
         self.after_response = AsyncCallable(after_response) if after_response else None
         self.background = background
@@ -258,15 +266,15 @@
         self.summary = summary
         self.tags = tags
         self.security = security
         self.responses = responses
         # memoized attributes, defaulted to Empty
         self._resolved_after_response: AfterResponseHookHandler | None | EmptyType = Empty
         self._resolved_before_request: BeforeRequestHookHandler | None | EmptyType = Empty
-        self._resolved_response_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType = Empty
+        self._response_handler_mapping: ResponseHandlerMap = {"default_handler": Empty, "response_type_handler": Empty}
 
     def __call__(self, fn: AnyCallable) -> HTTPRouteHandler:
         """Replace a function with itself."""
         self.fn = Ref["MaybePartial[AnyCallable]"](fn)
         self.signature = Signature.from_callable(fn)
         self._validate_handler_function()
 
@@ -282,26 +290,26 @@
 
     def resolve_response_class(self) -> type[Response]:
         """Return the closest custom Response class in the owner graph or the default Response class.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
-            The default :class:`Response <starlite.response.Response>` class for the route handler.
+            The default :class:`Response <.response.Response>` class for the route handler.
         """
         for layer in list(reversed(self.ownership_layers)):
             if layer.response_class is not None:
                 return layer.response_class
         return Response
 
     def resolve_response_headers(self) -> frozenset[ResponseHeader]:
         """Return all header parameters in the scope of the handler function.
 
         Returns:
-            A dictionary mapping keys to :class:`ResponseHeader <starlite.datastructures.ResponseHeader>` instances.
+            A dictionary mapping keys to :class:`ResponseHeader <.datastructures.ResponseHeader>` instances.
         """
         resolved_response_headers: dict[str, ResponseHeader] = {}
 
         for layer in self.ownership_layers:
             if layer_response_headers := layer.response_headers:
                 if isinstance(layer_response_headers, Mapping):
                     # this can't happen unless you manually set response_headers on an instance, which would result in a
@@ -322,37 +330,37 @@
 
         return frozenset(resolved_response_headers.values())
 
     def resolve_response_cookies(self) -> frozenset[Cookie]:
         """Return a list of Cookie instances. Filters the list to ensure each cookie key is unique.
 
         Returns:
-            A list of :class:`Cookie <starlite.datastructures.Cookie>` instances.
+            A list of :class:`Cookie <.datastructures.Cookie>` instances.
         """
         response_cookies: set[Cookie] = set()
         for layer in reversed(self.ownership_layers):
             if layer_response_cookies := layer.response_cookies:
                 if isinstance(layer_response_cookies, Mapping):
                     # this can't happen unless you manually set response_cookies on an instance, which would result in a
                     # type-checking error on everything but the controller. We cover this case nevertheless
                     response_cookies.update(
                         {Cookie(key=key, value=value) for key, value in layer_response_cookies.items()}
                     )
                 else:
-                    response_cookies.update(layer_response_cookies)
+                    response_cookies.update(cast("set[Cookie]", layer_response_cookies))
         return frozenset(response_cookies)
 
     def resolve_before_request(self) -> BeforeRequestHookHandler | None:
         """Resolve the before_handler handler by starting from the route handler and moving up.
 
         If a handler is found it is returned, otherwise None is set.
         This method is memoized so the computation occurs only once.
 
         Returns:
-            An optional :class:`before request lifecycle hook handler <starlite.types.BeforeRequestHookHandler>`
+            An optional :class:`before request lifecycle hook handler <.types.BeforeRequestHookHandler>`
         """
         if self._resolved_before_request is Empty:
             before_request_handlers: list[AsyncCallable] = [
                 layer.before_request for layer in self.ownership_layers if layer.before_request  # type: ignore[misc]
             ]
             self._resolved_before_request = cast(
                 "BeforeRequestHookHandler | None",
@@ -363,102 +371,119 @@
     def resolve_after_response(self) -> AfterResponseHookHandler | None:
         """Resolve the after_response handler by starting from the route handler and moving up.
 
         If a handler is found it is returned, otherwise None is set.
         This method is memoized so the computation occurs only once.
 
         Returns:
-            An optional :class:`after response lifecycle hook handler <starlite.types.AfterResponseHookHandler>`
+            An optional :class:`after response lifecycle hook handler <.types.AfterResponseHookHandler>`
         """
         if self._resolved_after_response is Empty:
             after_response_handlers: list[AsyncCallable] = [
                 layer.after_response for layer in self.ownership_layers if layer.after_response  # type: ignore[misc]
             ]
             self._resolved_after_response = cast(
                 "AfterResponseHookHandler | None",
                 after_response_handlers[-1] if after_response_handlers else None,
             )
 
         return cast("AfterResponseHookHandler | None", self._resolved_after_response)
 
-    def resolve_response_handler(
-        self,
-    ) -> Callable[[Any], Awaitable[ASGIApp]]:
+    def get_response_handler(self, is_response_type_data: bool = False) -> Callable[[Any], Awaitable[ASGIApp]]:
         """Resolve the response_handler function for the route handler.
 
         This method is memoized so the computation occurs only once.
 
+        Args:
+            is_response_type_data: Whether to return a handler for 'Response' instances.
+
         Returns:
             Async Callable to handle an HTTP Request
         """
-        if self._resolved_response_handler is Empty:
+        if self._response_handler_mapping["default_handler"] is Empty:
             after_request_handlers: list[AsyncCallable] = [
                 layer.after_request for layer in self.ownership_layers if layer.after_request  # type: ignore[misc]
             ]
             after_request = cast(
                 "AfterRequestHookHandler | None",
                 after_request_handlers[-1] if after_request_handlers else None,
             )
 
             media_type = self.media_type.value if isinstance(self.media_type, Enum) else self.media_type
             response_class = self.resolve_response_class()
             headers = self.resolve_response_headers()
             cookies = self.resolve_response_cookies()
             type_encoders = self.resolve_type_encoders()
 
-            if is_class_and_subclass(self.signature.return_annotation, ResponseContainer):  # type: ignore
-                handler = create_response_container_handler(
+            return_annotation = get_signature_model(self).return_annotation
+
+            if before_request_handler := self.resolve_before_request():
+                before_request_handler_signature = Signature.from_callable(before_request_handler)
+                if (
+                    before_request_handler_signature.return_annotation
+                    and before_request_handler_signature.return_annotation is not Signature.empty
+                ):
+                    return_annotation = before_request_handler_signature.return_annotation
+
+            self._response_handler_mapping["response_type_handler"] = create_response_handler(
+                cookies=cookies, after_request=after_request
+            )
+
+            if is_class_and_subclass(return_annotation, Response):
+                self._response_handler_mapping["default_handler"] = self._response_handler_mapping[
+                    "response_type_handler"
+                ]
+            elif is_class_and_subclass(return_annotation, ResponseContainer):  # type: ignore
+                self._response_handler_mapping["default_handler"] = create_response_container_handler(
                     after_request=after_request,
                     cookies=cookies,
                     headers=headers,
                     media_type=media_type,
                     status_code=self.status_code,
                 )
-
-            elif is_class_and_subclass(self.signature.return_annotation, Response):
-                handler = create_response_handler(cookies=cookies, after_request=after_request)
-
-            elif is_async_callable(self.signature.return_annotation) or self.signature.return_annotation in {
-                ASGIApp,
-                "ASGIApp",
-            }:
-                handler = create_generic_asgi_response_handler(cookies=cookies, after_request=after_request)
-
+            elif is_async_callable(return_annotation) or return_annotation is ASGIApp:
+                self._response_handler_mapping["default_handler"] = create_generic_asgi_response_handler(
+                    cookies=cookies, after_request=after_request
+                )
             else:
-                handler = create_data_handler(
+                self._response_handler_mapping["default_handler"] = create_data_handler(
                     after_request=after_request,
                     background=self.background,
                     cookies=cookies,
                     headers=headers,
                     media_type=media_type,
                     response_class=response_class,
-                    return_annotation=self.signature.return_annotation,
+                    return_annotation=return_annotation,
                     status_code=self.status_code,
                     type_encoders=type_encoders,
                 )
 
-            self._resolved_response_handler = handler
-        return self._resolved_response_handler  # type:ignore[return-value]
+        return cast(
+            "Callable[[Any], Awaitable[ASGIApp]]",
+            self._response_handler_mapping["response_type_handler"]
+            if is_response_type_data
+            else self._response_handler_mapping["default_handler"],
+        )
 
     async def to_response(
         self, app: "Starlite", data: Any, plugins: list["SerializationPluginProtocol"], request: "Request"
     ) -> "ASGIApp":
-        """Return a :class:`Response <starlite.Response>` from the handler by resolving and calling it.
+        """Return a :class:`Response <.response.Response>` from the handler by resolving and calling it.
 
         Args:
-            app: The :class:`Starlite <starlite.app.Starlite>` app instance
-            data: Either an instance of a :class:`ResponseContainer <starlite.datastructures.ResponseContainer>`,
+            app: The :class:`Starlite <.app.Starlite>` app instance
+            data: Either an instance of a :class:`ResponseContainer <.response_containers.ResponseContainer>`,
                 a Response instance or an arbitrary value.
             plugins: An optional mapping of plugins
-            request: A :class:`Request <starlite.connection.request.Request>` instance
+            request: A :class:`Request <.connection.Request>` instance
 
         Returns:
             A Response instance
         """
-        response_handler = self.resolve_response_handler()
+        response_handler = self.get_response_handler(is_response_type_data=isinstance(data, Response))
         return await response_handler(app=app, data=data, plugins=plugins, request=request)  # type: ignore
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it is set by inspecting its return annotations."""
         super()._validate_handler_function()
 
         if self.signature.return_annotation is Signature.empty:
```

### Comparing `starlite-2.0.0a1/starlite/handlers/http_handlers/decorators.py` & `starlite-2.0.0a2/starlite/handlers/http_handlers/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from starlite.response import FileResponse
 from starlite.response_containers import File
 from starlite.utils import is_class_and_subclass
 
 from .base import HTTPRouteHandler
 
 if TYPE_CHECKING:
-    from typing import Any
-
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
+    from typing import Any, Mapping
 
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.datastructures import CacheControlHeader, ETag
     from starlite.di import Provide
     from starlite.openapi.datastructures import ResponseSpec
+    from starlite.openapi.spec import SecurityRequirement
     from starlite.types import (
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeRequestHookHandler,
         CacheKeyBuilder,
         ExceptionHandlersMap,
         Guard,
@@ -62,14 +61,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -84,58 +84,59 @@
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``delete``
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
-            status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
-                ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+            status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT``
+                and ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -175,14 +176,15 @@
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
             security=security,
+            signature_namespace=signature_namespace,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
         )
@@ -212,14 +214,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -234,58 +237,59 @@
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``get``.
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -326,14 +330,15 @@
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
             security=security,
+            signature_namespace=signature_namespace,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
         )
@@ -363,14 +368,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -389,58 +395,59 @@
 
         Notes:
             - A response to a head request cannot include a body.
                 See: [MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/HEAD).
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -481,14 +488,15 @@
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
             security=security,
+            signature_namespace=signature_namespace,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
         )
@@ -532,14 +540,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -554,58 +563,59 @@
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``patch``.
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -645,14 +655,15 @@
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
             security=security,
+            signature_namespace=signature_namespace,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
         )
@@ -682,14 +693,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -704,58 +716,59 @@
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``post``
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -794,14 +807,15 @@
             path=path,
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
+            signature_namespace=signature_namespace,
             security=security,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
@@ -832,14 +846,15 @@
         media_type: MediaType | str | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         status_code: int | None = None,
         sync_to_thread: bool = False,
         # OpenAPI related attributes
         content_encoding: str | None = None,
         content_media_type: str | None = None,
         deprecated: bool = False,
         description: str | None = None,
@@ -854,58 +869,59 @@
         type_encoders: TypeEncodersMap | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``put``
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments.
-                If not given defaults to ``'/'``
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is passed
+                If not given defaults to ``/``
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
                 to any route handler. If this function returns a value, the request will not reach the route handler,
                 and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                :class:`Request <.connection.Request>` object and should not return any values.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to ``None``.
             before_request: A sync or async function called immediately before calling the route handler. Receives
-                the `starlite.connection.Request`` instance and any non-``None`` return value is used for the response,
+                the :class:`.connection.Request` instance and any non-``None`` return value is used for the response,
                 bypassing the route handler.
             cache: Enables response caching if configured on the application level. Valid values are ``True`` or a number
                 of seconds (e.g. ``120``) to cache the response.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` that will be added to the response.
-            cache_key_builder: A :class:`cache-key builder function <starlite.types.CacheKeyBuilder>`. Allows for customization
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` that will be added to the response.
+            cache_key_builder: A :class:`cache-key builder function <.types.CacheKeyBuilder>`. Allows for customization
                 of the cache key if caching is configured on the application level.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <starlite.datastructures.ETag>` that will be added to the response.
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` that will be added to the response.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            http_method: An :class:`http method string <starlite.types.Method>`, a member of the enum
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            http_method: An :class:`http method string <.types.Method>`, a member of the enum
                 :class:`HttpMethod <starlite.enums.HttpMethod>` or a list of these that correlates to the methods the
                 route handler function should handle.
-            media_type: A member of the :class:`MediaType <starlite.enums.MediaType>` enum or a string with a
+            media_type: A member of the :class:`MediaType <.enums.MediaType>` enum or a string with a
                 valid IANA Media-Type.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
-            response_class: A custom subclass of :class:`Response <starlite.response.Response>` to be used as route handler's
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as route handler's
                 default response.
-            response_cookies: A sequence of :class:`Cookie <starlite.datastructures.Cookie>` instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             responses: A mapping of additional status codes and a description of their expected content.
                 This information will be included in the OpenAPI schema
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             status_code: An http status code for the response. Defaults to ``200`` for mixed method or ``GET``, ``PUT`` and
                 ``PATCH``, ``201`` for ``POST`` and ``204`` for ``DELETE``.
             sync_to_thread: A boolean dictating whether the handler function will be executed in a worker thread or the
                 main event loop. This has an effect only for sync handler functions. See using sync handler functions.
-            content_encoding: A string describing the encoding of the content, e.g. ``"base64"``.
-            content_media_type: A string designating the media-type of the content, e.g. ``"image/png"``.
+            content_encoding: A string describing the encoding of the content, e.g. ``base64``.
+            content_media_type: A string designating the media-type of the content, e.g. ``image/png``.
             deprecated:  A boolean dictating whether this route should be marked as deprecated in the OpenAPI schema.
             description: Text used for the route's schema description section.
             include_in_schema: A boolean flag dictating whether  the route handler should be documented in the OpenAPI schema.
             operation_id: An identifier used for the route's schema operationId. Defaults to the ``__name__`` of the wrapped function.
             raises:  A list of exception classes extending from starlite.HttpException that is used for the OpenAPI documentation.
                 This list should describe all exceptions raised within the route handler's function/method. The Starlite
                 ValidationException will be added automatically for the schema if any validation is involved.
@@ -945,14 +961,15 @@
             raises=raises,
             response_class=response_class,
             response_cookies=response_cookies,
             response_description=response_description,
             response_headers=response_headers,
             responses=responses,
             security=security,
+            signature_namespace=signature_namespace,
             status_code=status_code,
             summary=summary,
             sync_to_thread=sync_to_thread,
             tags=tags,
             type_encoders=type_encoders,
             **kwargs,
         )
```

### Comparing `starlite-2.0.0a1/starlite/handlers/utils.py` & `starlite-2.0.0a2/starlite/_layers/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Mapping, Sequence
 
 from starlite.datastructures.cookie import Cookie
 from starlite.datastructures.response_header import ResponseHeader
 
+__all__ = ("narrow_response_cookies", "narrow_response_headers")
+
+
 if TYPE_CHECKING:
     from starlite.types.composite_types import ResponseCookies, ResponseHeaders
 
 
 def narrow_response_headers(headers: ResponseHeaders | None) -> Sequence[ResponseHeader] | None:
     """Given :class:`.types.ResponseHeaders` as a :class:`typing.Mapping`, create a list of
     :class:`.datastructures.response_header.ResponseHeader` from it, otherwise return ``headers`` unchanged
     """
     return (
-        [ResponseHeader(name=name, value=value) for name, value in headers.items()]
+        tuple(ResponseHeader(name=name, value=value) for name, value in headers.items())
         if isinstance(headers, Mapping)
         else headers
     )
 
 
 def narrow_response_cookies(cookies: ResponseCookies | None) -> Sequence[Cookie] | None:
     """Given :class:`.types.ResponseCookies` as a :class:`typing.Mapping`, create a list of
     :class:`.datastructures.cookie.Cookie` from it, otherwise return ``cookies`` unchanged
     """
-    return [Cookie(key=key, value=value) for key, value in cookies.items()] if isinstance(cookies, Mapping) else cookies
+    return (
+        tuple(Cookie(key=key, value=value) for key, value in cookies.items())
+        if isinstance(cookies, Mapping)
+        else cookies
+    )
```

### Comparing `starlite-2.0.0a1/starlite/handlers/websocket_handlers.py` & `starlite-2.0.0a2/starlite/handlers/websocket_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
 from inspect import Signature
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.handlers.base import BaseRouteHandler
 from starlite.utils import Ref, is_async_callable
 
+__all__ = ("WebsocketRouteHandler", "websocket")
+
+
 if TYPE_CHECKING:
-    from starlite.types import MaybePartial  # nopycln: import # noqa: F401
+    from typing import Any, Mapping
+
     from starlite.types import (
         AsyncAnyCallable,
         Dependencies,
         ExceptionHandler,
         Guard,
+        MaybePartial,  # noqa: F401
         Middleware,
     )
 
 
 class WebsocketRouteHandler(BaseRouteHandler["WebsocketRouteHandler"]):
     """Websocket route handler decorator.
 
@@ -30,38 +35,43 @@
         *,
         dependencies: Dependencies | None = None,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
         middleware: list[Middleware] | None = None,
         name: str | None = None,
         opt: dict[str, Any] | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize ``WebsocketRouteHandler``
 
         Args:
-            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults to '/'
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
+            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
+                to ``/``
+            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
+            guards: A sequence of :class:`Guard <.types.Guard>` callables.
+            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>` or
-                wherever you have access to :class:`Request <starlite.connection.request.Request>` or :class:`ASGI Scope <starlite.types.Scope>`.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or
+                :class:`ASGI Scope <.types.Scope>`.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         super().__init__(
             path,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
             guards=guards,
             middleware=middleware,
             name=name,
             opt=opt,
+            signature_namespace=signature_namespace,
             **kwargs,
         )
 
     def __call__(self, fn: AsyncAnyCallable) -> WebsocketRouteHandler:
         """Replace a function with itself."""
         self.fn = Ref["MaybePartial[AsyncAnyCallable]"](fn)
         self.signature = Signature.from_callable(fn)
```

### Comparing `starlite-2.0.0a1/starlite/kwargs/cleanup.py` & `starlite-2.0.0a2/starlite/_kwargs/cleanup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Coroutine, Generator
 
 from anyio import create_task_group
 
 from starlite.utils import AsyncCallable
 from starlite.utils.compat import async_next
 
+__all__ = ("DependencyCleanupGroup",)
+
+
 if TYPE_CHECKING:
     from starlite.types import AnyGenerator
 
 
 class DependencyCleanupGroup:
     """Wrapper for generator based dependencies.
```

### Comparing `starlite-2.0.0a1/starlite/kwargs/dependencies.py` & `starlite-2.0.0a2/starlite/_kwargs/dependencies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from inspect import isasyncgen, isgenerator
 from typing import TYPE_CHECKING, Any
 
-from starlite.signature.utils import get_signature_model
+from starlite._signature.utils import get_signature_model
 from starlite.utils.compat import async_next
 
+__all__ = ("Dependency", "create_dependency_batches", "map_dependencies_recursively", "resolve_dependency")
+
+
 if TYPE_CHECKING:
+    from starlite._kwargs.cleanup import DependencyCleanupGroup
     from starlite.connection import ASGIConnection
     from starlite.di import Provide
-    from starlite.kwargs.cleanup import DependencyCleanupGroup
 
 
 class Dependency:
     """Dependency graph of a given combination of ``Route`` + ``RouteHandler``"""
 
     __slots__ = ("key", "provide", "dependencies")
 
@@ -39,21 +42,21 @@
 
 async def resolve_dependency(
     dependency: "Dependency",
     connection: "ASGIConnection",
     kwargs: dict[str, Any],
     cleanup_group: "DependencyCleanupGroup",
 ) -> None:
-    """Resolve a given instance of :class:`Dependency <starlite.kwargs.Dependency>`.
+    """Resolve a given instance of :class:`Dependency <starlite._kwargs.Dependency>`.
 
     All required sub dependencies must already
     be resolved into the kwargs. The result of the dependency will be stored in the kwargs.
 
     Args:
-        dependency: An instance of :class:`Dependency <starlite.kwargs.Dependency>`
+        dependency: An instance of :class:`Dependency <starlite._kwargs.Dependency>`
         connection: An instance of :class:`Request <starlite.connection.Request>` or
             :class:`WebSocket <starlite.connection.WebSocket>`.
         kwargs: Any kwargs to pass to the dependency, the result will be stored here as well.
         cleanup_group: DependencyCleanupGroup to which generators returned by ``dependency`` will be added
     """
     signature_model = get_signature_model(dependency.provide)
     dependency_kwargs = (
@@ -73,15 +76,15 @@
     kwargs[dependency.key] = value
 
 
 def create_dependency_batches(expected_dependencies: set[Dependency]) -> list[set[Dependency]]:
     """Calculate batches for all dependencies, recursively.
 
     Args:
-        expected_dependencies: A set of all direct :class:`Dependencies <starlite.kwargs.Dependency>`.
+        expected_dependencies: A set of all direct :class:`Dependencies <starlite._kwargs.Dependency>`.
 
     Returns:
         A list of batches.
     """
     dependencies_to: dict[Dependency, set[Dependency]] = {}
     for dependency in expected_dependencies:
         if dependency not in dependencies_to:
```

### Comparing `starlite-2.0.0a1/starlite/kwargs/extractors.py` & `starlite-2.0.0a2/starlite/_kwargs/extractors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, DefaultDict, Dict, cast
 
-from starlite.datastructures.upload_file import UploadFile
-from starlite.enums import ParamType, RequestEncodingType
-from starlite.exceptions import ValidationException
-from starlite.multipart import parse_multipart_form
-from starlite.params import BodyKwarg
-from starlite.parsers import (
+from starlite._multipart import parse_multipart_form
+from starlite._parsers import (
     parse_headers,
     parse_query_string,
     parse_url_encoded_form_data,
 )
+from starlite.datastructures.upload_file import UploadFile
+from starlite.enums import ParamType, RequestEncodingType
+from starlite.exceptions import ValidationException
+from starlite.params import BodyKwarg
 from starlite.types import Empty
 
+__all__ = (
+    "body_extractor",
+    "cookies_extractor",
+    "create_connection_value_extractor",
+    "create_data_extractor",
+    "create_multipart_extractor",
+    "create_query_default_dict",
+    "create_url_encoded_data_extractor",
+    "headers_extractor",
+    "json_extractor",
+    "msgpack_extractor",
+    "parse_connection_headers",
+    "parse_connection_query_params",
+    "query_extractor",
+    "request_extractor",
+    "scope_extractor",
+    "socket_extractor",
+    "state_extractor",
+)
+
+
 if TYPE_CHECKING:
+    from starlite._kwargs import KwargsModel
+    from starlite._kwargs.parameter_definition import ParameterDefinition
+    from starlite._signature.models import SignatureField
     from starlite.connection import ASGIConnection, Request
-    from starlite.kwargs import KwargsModel
-    from starlite.kwargs.parameter_definition import ParameterDefinition
-    from starlite.signature.models import SignatureField
 
 
 def create_connection_value_extractor(
     kwargs_model: KwargsModel,
     connection_key: str,
     expected_params: set[ParameterDefinition],
     parser: Callable[[ASGIConnection, KwargsModel], dict[str, Any]] | None = None,
@@ -287,15 +308,15 @@
         connection: "Request[Any, Any, Any]",
     ) -> Any:
         multipart_form_part_limit = (
             body_kwarg_multipart_form_part_limit
             if body_kwarg_multipart_form_part_limit is not None
             else connection.app.multipart_form_part_limit
         )
-        connection.scope["_form"] = form_values = (  # type: ignore[typeddict-item]
+        connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
             connection.scope["_form"]  # type: ignore[typeddict-item]
             if "_form" in connection.scope
             else parse_multipart_form(
                 body=await connection.body(),
                 boundary=connection.content_type[-1].get("boundary", "").encode(),
                 multipart_form_part_limit=multipart_form_part_limit,
             )
@@ -322,15 +343,15 @@
     Returns:
         An extractor function.
     """
 
     async def extract_url_encoded_extractor(
         connection: "Request[Any, Any, Any]",
     ) -> Any:
-        connection.scope["_form"] = form_values = (  # type: ignore[typeddict-item]
+        connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
             connection.scope["_form"]  # type: ignore[typeddict-item]
             if "_form" in connection.scope
             else parse_url_encoded_form_data(await connection.body())
         )
         return form_values if form_values or not is_data_optional else None
 
     return cast(
```

### Comparing `starlite-2.0.0a1/starlite/kwargs/kwargs_model.py` & `starlite-2.0.0a2/starlite/_kwargs/kwargs_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable
 
 from anyio import create_task_group
 
-from starlite.constants import RESERVED_KWARGS
-from starlite.enums import ParamType, RequestEncodingType
-from starlite.exceptions import ImproperlyConfiguredException
-from starlite.kwargs.cleanup import DependencyCleanupGroup
-from starlite.kwargs.dependencies import (
+from starlite._kwargs.cleanup import DependencyCleanupGroup
+from starlite._kwargs.dependencies import (
     Dependency,
     create_dependency_batches,
     resolve_dependency,
 )
-from starlite.kwargs.extractors import (
+from starlite._kwargs.extractors import (
     body_extractor,
     cookies_extractor,
     create_connection_value_extractor,
     create_data_extractor,
     headers_extractor,
     parse_connection_headers,
     parse_connection_query_params,
     query_extractor,
     request_extractor,
     scope_extractor,
     socket_extractor,
     state_extractor,
 )
-from starlite.kwargs.parameter_definition import (
+from starlite._kwargs.parameter_definition import (
     ParameterDefinition,
     create_parameter_definition,
     merge_parameter_sets,
 )
+from starlite._signature import SignatureModel, get_signature_model
+from starlite._signature.models import SignatureField
+from starlite.constants import RESERVED_KWARGS
+from starlite.enums import ParamType, RequestEncodingType
+from starlite.exceptions import ImproperlyConfiguredException
 from starlite.params import BodyKwarg, ParameterKwarg
-from starlite.signature import SignatureModel, get_signature_model
-from starlite.signature.models import SignatureField
+
+__all__ = ("KwargsModel",)
+
 
 if TYPE_CHECKING:
     from starlite.connection import ASGIConnection
     from starlite.di import Provide
 
 
 class KwargsModel:
@@ -251,15 +254,15 @@
         path_parameters: set[str],
         layered_parameters: dict[str, SignatureField],
     ) -> KwargsModel:
         """Pre-determine what parameters are required for a given combination of route + route handler. It is executed
         during the application bootstrap process.
 
         Args:
-            signature_model: A :class:`SignatureModel <starlite.signature.SignatureModel>` subclass.
+            signature_model: A :class:`SignatureModel <starlite._signature.SignatureModel>` subclass.
             dependencies: A string keyed dictionary mapping dependency providers.
             path_parameters: Any expected path parameters.
             layered_parameters: A string keyed dictionary of layered parameters.
 
         Returns:
             An instance of KwargsModel
         """
```

### Comparing `starlite-2.0.0a1/starlite/kwargs/parameter_definition.py` & `starlite-2.0.0a2/starlite/_kwargs/parameter_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, NamedTuple
 
 from starlite.enums import ParamType
 from starlite.params import ParameterKwarg
 
+__all__ = ("ParameterDefinition", "create_parameter_definition", "merge_parameter_sets")
+
+
 if TYPE_CHECKING:
-    from starlite.signature.models import SignatureField
+    from starlite._signature.models import SignatureField
 
 
 class ParameterDefinition(NamedTuple):
     """Tuple defining a kwarg representing a request parameter."""
 
     default_value: Any
     field_alias: str
```

### Comparing `starlite-2.0.0a1/starlite/logging/picologging.py` & `starlite-2.0.0a2/starlite/logging/picologging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import atexit
 from queue import Queue
 from typing import Any
 
 from starlite.exceptions import MissingDependencyException
-from starlite.logging.utils import resolve_handlers
+from starlite.logging._utils import resolve_handlers
+
+__all__ = ("QueueListenerHandler",)
+
 
 try:
     from picologging import StreamHandler
     from picologging.handlers import QueueHandler, QueueListener
 except ImportError as e:
     raise MissingDependencyException("picologging is not installed") from e
 
@@ -23,15 +26,12 @@
         Args:
             handlers: Optional 'ConvertingList'
 
         Notes:
             - Requires ``picologging`` to be installed.
         """
         super().__init__(Queue(-1))
-        if handlers:
-            handlers = resolve_handlers(handlers)
-        else:
-            handlers = [StreamHandler()]
+        handlers = resolve_handlers(handlers) if handlers else [StreamHandler()]
         self.listener = QueueListener(self.queue, *handlers)
         self.listener.start()
 
         atexit.register(self.listener.stop)
```

### Comparing `starlite-2.0.0a1/starlite/logging/standard.py` & `starlite-2.0.0a2/starlite/logging/standard.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 import atexit
 from logging import StreamHandler
 from logging.handlers import QueueHandler, QueueListener
 from queue import Queue
 from typing import Any
 
-from starlite.logging.utils import resolve_handlers
+from starlite.logging._utils import resolve_handlers
+
+__all__ = ("QueueListenerHandler",)
 
 
 class QueueListenerHandler(QueueHandler):
     """Configure queue listener and handler to support non-blocking logging configuration."""
 
     def __init__(self, handlers: list[Any] | None = None) -> None:
         """Initialize `?QueueListenerHandler`.
 
         Args:
             handlers: Optional 'ConvertingList'
         """
         super().__init__(Queue(-1))
-        if handlers:
-            handlers = resolve_handlers(handlers)
-        else:
-            handlers = [StreamHandler()]
+        handlers = resolve_handlers(handlers) if handlers else [StreamHandler()]
         self.listener = QueueListener(self.queue, *handlers)
         self.listener.start()
 
         atexit.register(self.listener.stop)
```

### Comparing `starlite-2.0.0a1/starlite/logging/utils.py` & `starlite-2.0.0a2/starlite/logging/_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import Any
 
+__all__ = ("resolve_handlers",)
+
 
 def resolve_handlers(handlers: list[Any]) -> list[Any]:
     """Convert list of string of handlers to the object of respective handler.
 
     Indexing the list performs the evaluation of the object.
 
     Args:
```

### Comparing `starlite-2.0.0a1/starlite/middleware/allowed_hosts.py` & `starlite-2.0.0a2/starlite/middleware/allowed_hosts.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import TYPE_CHECKING, Pattern
 
 from starlite.datastructures import URL, MutableScopeHeaders
 from starlite.middleware.base import AbstractMiddleware
 from starlite.response import RedirectResponse, Response
 from starlite.status_codes import HTTP_400_BAD_REQUEST
 
+__all__ = ("AllowedHostsMiddleware",)
+
+
 if TYPE_CHECKING:
     from starlite.config.allowed_hosts import AllowedHostsConfig
     from starlite.types import ASGIApp, Receive, Scope, Send
 
 
 class AllowedHostsMiddleware(AbstractMiddleware):
     """Middleware ensuring the host of a request originated in a trusted host."""
```

### Comparing `starlite-2.0.0a1/starlite/middleware/authentication.py` & `starlite-2.0.0a2/starlite/middleware/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
 
 from starlite.connection import ASGIConnection
 from starlite.enums import ScopeType
-from starlite.middleware.utils import (
+from starlite.middleware._utils import (
     build_exclude_path_pattern,
     should_bypass_middleware,
 )
 
+__all__ = ("AbstractAuthenticationMiddleware", "AuthenticationResult")
+
+
 if TYPE_CHECKING:
     from starlite.types import ASGIApp, Receive, Scope, Scopes, Send
 
 
 @dataclass
 class AuthenticationResult:
     """Pydantic model for authentication data."""
```

### Comparing `starlite-2.0.0a1/starlite/middleware/base.py` & `starlite-2.0.0a2/starlite/middleware/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, Callable, Protocol, runtime_checkable
 
 from starlite.enums import ScopeType
-from starlite.middleware.utils import (
+from starlite.middleware._utils import (
     build_exclude_path_pattern,
     should_bypass_middleware,
 )
 
+__all__ = ("AbstractMiddleware", "DefineMiddleware", "MiddlewareProtocol")
+
+
 if TYPE_CHECKING:
     from starlite.types import Scopes
     from starlite.types.asgi_types import ASGIApp, Receive, Scope, Send
 
 
 @runtime_checkable
 class MiddlewareProtocol(Protocol):  # pragma: no cover
@@ -39,19 +42,15 @@
             None
         """
 
 
 class DefineMiddleware:
     """Container enabling passing ``*args`` and ``**kwargs`` to Middleware class constructors and factory functions."""
 
-    __slots__ = (
-        "middleware",
-        "args",
-        "kwargs",
-    )
+    __slots__ = ("middleware", "args", "kwargs")
 
     def __init__(self, middleware: Callable[..., ASGIApp], *args: Any, **kwargs: Any) -> None:
         """Initialize ``DefineMiddleware``.
 
         Args:
             middleware: A callable that returns an ASGIApp.
             *args: Positional arguments to pass to the callable.
@@ -68,15 +67,15 @@
     def __call__(self, app: ASGIApp) -> ASGIApp:
         """Call the middleware constructor or factory.
 
         Args:
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
 
         Returns:
-            Calls :attr:`DefineMiddleware.middleware` and returns the ASGIApp created.
+            Calls :class:`DefineMiddleware.middleware <.DefineMiddleware>` and returns the ASGIApp created.
         """
 
         return self.middleware(*self.args, app=app, **self.kwargs)
 
 
 class AbstractMiddleware:
     """Abstract middleware providing base functionality common to all middlewares, for dynamically engaging/bypassing
@@ -126,15 +125,15 @@
                 exclude_opt_key=self.exclude_opt_key,
             ):
                 await self.app(scope, receive, send)
             else:
                 await original__call__(self, scope, receive, send)
 
         # https://github.com/python/mypy/issues/2427#issuecomment-384229898
-        setattr(cls, "__call__", wrapped_call)  # noqa: B010
+        setattr(cls, "__call__", wrapped_call)
 
     @abstractmethod
     async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """Execute the ASGI middleware.
 
         Called by the previous middleware in the stack if a response is not awaited prior.
```

### Comparing `starlite-2.0.0a1/starlite/middleware/compression.py` & `starlite-2.0.0a2/starlite/middleware/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from starlite.constants import SCOPE_STATE_RESPONSE_COMPRESSED
 from starlite.datastructures import Headers, MutableScopeHeaders
 from starlite.enums import CompressionEncoding, ScopeType
 from starlite.exceptions import MissingDependencyException
 from starlite.middleware.base import AbstractMiddleware
 from starlite.utils import Ref, set_starlite_scope_state
 
+__all__ = ("CompressionFacade", "CompressionMiddleware")
+
+
 if TYPE_CHECKING:
     from starlite.config.compression import CompressionConfig
     from starlite.types import (
         ASGIApp,
         HTTPResponseStartEvent,
         Message,
         Receive,
```

### Comparing `starlite-2.0.0a1/starlite/middleware/cors.py` & `starlite-2.0.0a2/starlite/middleware/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 from typing import TYPE_CHECKING
 
 from starlite.datastructures import Headers, MutableScopeHeaders
 from starlite.enums import ScopeType
 from starlite.middleware.base import AbstractMiddleware
 
+__all__ = ("CORSMiddleware",)
+
+
 if TYPE_CHECKING:
     from starlite.config.cors import CORSConfig
     from starlite.types import ASGIApp, Message, Receive, Scope, Send
 
 
 class CORSMiddleware(AbstractMiddleware):
     """CORS Middleware."""
```

### Comparing `starlite-2.0.0a1/starlite/middleware/csrf.py` & `starlite-2.0.0a2/starlite/middleware/csrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 from secrets import compare_digest
 from typing import TYPE_CHECKING, Any
 
 from starlite.datastructures import MutableScopeHeaders
 from starlite.datastructures.cookie import Cookie
 from starlite.enums import RequestEncodingType, ScopeType
 from starlite.exceptions import PermissionDeniedException
-from starlite.middleware.base import MiddlewareProtocol
-from starlite.middleware.utils import (
+from starlite.middleware._utils import (
     build_exclude_path_pattern,
     should_bypass_middleware,
 )
+from starlite.middleware.base import MiddlewareProtocol
+
+__all__ = ("CSRFMiddleware",)
+
 
 if TYPE_CHECKING:
     from starlite.config.csrf import CSRFConfig
     from starlite.connection import Request
     from starlite.types import (
         ASGIApp,
         HTTPSendMessage,
```

### Comparing `starlite-2.0.0a1/starlite/middleware/exceptions/debug_response.py` & `starlite-2.0.0a2/starlite/middleware/exceptions/_debug_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 from typing import TYPE_CHECKING
 
 from starlite.enums import MediaType
 from starlite.response import Response
 from starlite.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 from starlite.utils import get_name
 
+__all__ = (
+    "create_debug_response",
+    "create_exception_html",
+    "create_frame_html",
+    "create_html_response_content",
+    "create_line_html",
+    "create_plain_text_response_content",
+    "get_symbol_name",
+)
+
+
 if TYPE_CHECKING:
     from inspect import FrameInfo
 
     from starlite.connection import Request
 
 tpl_dir = Path(__file__).parent / "templates"
```

### Comparing `starlite-2.0.0a1/starlite/middleware/exceptions/middleware.py` & `starlite-2.0.0a2/starlite/middleware/exceptions/middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, field
 from inspect import getmro
+from sys import exc_info
+from traceback import format_exception
 from typing import TYPE_CHECKING, Any, Type, cast
 
 from starlite.connection import Request
 from starlite.datastructures import Headers
 from starlite.enums import ScopeType
 from starlite.exceptions import WebSocketException
 from starlite.middleware.cors import CORSMiddleware
-from starlite.middleware.exceptions.debug_response import create_debug_response
+from starlite.middleware.exceptions._debug_response import create_debug_response
 from starlite.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 
+__all__ = ("ExceptionHandlerMiddleware",)
+
+
 if TYPE_CHECKING:
     from starlite import Response
     from starlite.app import Starlite
+    from starlite.logging import BaseLoggingConfig
     from starlite.types import (
         ASGIApp,
         ExceptionHandler,
         ExceptionHandlersMap,
+        Logger,
         Receive,
         Scope,
         Send,
     )
     from starlite.types.asgi_types import WebSocketCloseEvent
 
 
@@ -136,20 +143,19 @@
             send: The ASGI send function.
 
         Returns:
             None
         """
         try:
             await self.app(scope, receive, send)
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:  # noqa: BLE001
             starlite_app = scope["app"]
-            if self.debug and starlite_app.logger:
-                starlite_app.logger.debug(
-                    "exception raised on %s connection request to route %s", scope["type"], scope["path"], exc_info=True
-                )
+
+            if starlite_app.logging_config and (logger := starlite_app.logger):
+                self.handle_exception_logging(logger=logger, logging_config=starlite_app.logging_config, scope=scope)
 
             for hook in starlite_app.after_exception:
                 await hook(e, scope, starlite_app.state)
 
             if scope["type"] == ScopeType.HTTP:
                 await self.handle_request_exception(
                     starlite_app=starlite_app, scope=scope, receive=receive, send=send, exc=e
@@ -158,20 +164,23 @@
                 await self.handle_websocket_exception(send=send, exc=e)
 
     async def handle_request_exception(
         self, starlite_app: "Starlite", scope: "Scope", receive: "Receive", send: "Send", exc: Exception
     ) -> None:
         """Handle exception raised inside 'http' scope routes.
 
-        :param starlite_app: The starlite app instance.
-        :param scope: The ASGI connection scope.
-        :param receive: The ASGI receive function.
-        :param send: The ASGI send function.
-        :param exc: The caught exception.
-        :return: None.
+        Args:
+            starlite_app: The starlite app instance.
+            scope: The ASGI connection scope.
+            receive: The ASGI receive function.
+            send: The ASGI send function.
+            exc: The caught exception.
+
+        Returns:
+            None.
         """
 
         headers = Headers.from_scope(scope=scope)
         if starlite_app.cors_config and (origin := headers.get("origin")):
             cors_middleware = CORSMiddleware(app=self.app, config=starlite_app.cors_config)
             send = cors_middleware.send_wrapper(send=send, origin=origin, has_cookie="cookie" in headers)
 
@@ -179,31 +188,53 @@
         response = exception_handler(Request(scope=scope, receive=receive, send=send), exc)
         await response(scope=scope, receive=receive, send=send)
 
     @staticmethod
     async def handle_websocket_exception(send: "Send", exc: Exception) -> None:
         """Handle exception raised inside 'websocket' scope routes.
 
-        :param send: The ASGI send function.
-        :param exc: The caught exception.
-        :return: None.
+        Args:
+            send: The ASGI send function.
+            exc: The caught exception.
+
+        Returns:
+            None.
         """
         if isinstance(exc, WebSocketException):
             code = exc.code
             reason = exc.detail
         else:
             code = 4000 + getattr(exc, "status_code", HTTP_500_INTERNAL_SERVER_ERROR)
             reason = getattr(exc, "detail", repr(exc))
         event: WebSocketCloseEvent = {"type": "websocket.close", "code": code, "reason": reason}
         await send(event)
 
     def default_http_exception_handler(self, request: Request, exc: Exception) -> Response[Any]:
         """Handle an HTTP exception by returning the appropriate response.
 
-        :param request: An HTTP Request instance.
-        :param exc: The caught exception.
-        :return: An HTTP response.
+        Args:
+            request: An HTTP Request instance.
+            exc: The caught exception.
+
+        Returns:
+            An HTTP response.
         """
         status_code = getattr(exc, "status_code", HTTP_500_INTERNAL_SERVER_ERROR)
         if status_code == HTTP_500_INTERNAL_SERVER_ERROR and self.debug:
             return create_debug_response(request=request, exc=exc)
         return create_exception_response(exc)
+
+    def handle_exception_logging(self, logger: Logger, logging_config: BaseLoggingConfig, scope: Scope) -> None:
+        """Handle logging - if the starlite app has a logging config in place.
+
+        Args:
+            logger: A logger instance.
+            logging_config: Logging Config instance.
+            scope: The ASGI connection scope.
+
+        Returns:
+            None
+        """
+        if (
+            logging_config.log_exceptions == "always" or (logging_config.log_exceptions == "debug" and self.debug)
+        ) and logging_config.exception_logging_handler:
+            logging_config.exception_logging_handler(logger, scope, format_exception(*exc_info()))
```

### Comparing `starlite-2.0.0a1/starlite/middleware/exceptions/templates/scripts.js` & `starlite-2.0.0a2/starlite/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/middleware/exceptions/templates/styles.css` & `starlite-2.0.0a2/starlite/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/middleware/logging.py` & `starlite-2.0.0a2/starlite/middleware/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 from starlite.serialization import default_serializer, encode_json
 from starlite.utils import (
     get_serializer_from_scope,
     get_starlite_scope_state,
     set_starlite_scope_state,
 )
 
+__all__ = ("LoggingMiddleware", "LoggingMiddlewareConfig")
+
+
 if TYPE_CHECKING:
     from starlite.connection import Request
     from starlite.types import (
         ASGIApp,
         Logger,
         Message,
         Receive,
@@ -36,18 +39,18 @@
         Send,
         Serializer,
     )
 
 try:
     from structlog.types import BindableLogger
 
-    structlog_installed = True  # pylint: disable=invalid-name
+    structlog_installed = True
 except ImportError:
     BindableLogger = object  # type: ignore
-    structlog_installed = False  # pylint: disable=invalid-name
+    structlog_installed = False
 
 
 class LoggingMiddleware(AbstractMiddleware):
     """Logging middleware."""
 
     __slots__ = ("config", "logger", "request_extractor", "response_extractor", "is_struct_logger")
 
@@ -147,15 +150,17 @@
         Returns:
             None
         """
         message = values.pop("message")
         if self.is_struct_logger:
             self.logger.info(message, **values)
         else:
-            self.logger.info(f"{message}: " + ", ".join([f"{key}={value}" for key, value in values.items()]))
+            value_strings = [f"{key}={value}" for key, value in values.items()]
+            log_message = f"{message}: {', '.join(value_strings)}"
+            self.logger.info(log_message)
 
     def _serialize_value(self, serializer: Serializer | None, value: Any) -> Any:
         if not self.is_struct_logger and isinstance(value, (dict, list, tuple, set)):
             value = encode_json(value, serializer)
         if isinstance(value, bytes):
             return value.decode("utf-8")
         return value
@@ -338,24 +343,21 @@
                 from starlite.config.logging import LoggingConfig
                 from starlite.middleware.logging import LoggingMiddlewareConfig
 
                 logging_config = LoggingConfig()
 
                 logging_middleware_config = LoggingMiddlewareConfig()
 
-
                 @get("/")
                 def my_handler(request: Request) -> None:
                     ...
 
-
                 app = Starlite(
                     route_handlers=[my_handler],
                     logging_config=logging_config,
                     middleware=[logging_middleware_config.middleware],
                 )
 
-
         Returns:
             An instance of DefineMiddleware including ``self`` as the config kwarg value.
         """
         return DefineMiddleware(self.middleware_class, config=self)
```

### Comparing `starlite-2.0.0a1/starlite/middleware/rate_limit.py` & `starlite-2.0.0a2/starlite/middleware/rate_limit.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 from starlite.datastructures import MutableScopeHeaders
 from starlite.enums import ScopeType
 from starlite.exceptions import TooManyRequestsException
 from starlite.middleware.base import AbstractMiddleware, DefineMiddleware
 from starlite.serialization import decode_json, encode_json
 from starlite.utils import AsyncCallable
 
+__all__ = ("CacheObject", "RateLimitConfig", "RateLimitMiddleware")
+
+
 if TYPE_CHECKING:
     from typing import Awaitable
 
-    from starlite.cache import Cache
+    from starlite import Starlite
     from starlite.connection import Request
+    from starlite.stores.base import Store
     from starlite.types import ASGIApp, Message, Receive, Scope, Send, SyncOrAsyncUnion
 
+
 DurationUnit = Literal["second", "minute", "hour", "day"]
 
 DURATION_VALUES: dict[DurationUnit, int] = {"second": 1, "minute": 60, "hour": 3600, "day": 86400}
 
 
 @dataclass
 class CacheObject:
@@ -32,25 +37,15 @@
     history: list[int]
     reset: int
 
 
 class RateLimitMiddleware(AbstractMiddleware):
     """Rate-limiting middleware."""
 
-    __slots__ = (
-        "app",
-        "cache",
-        "check_throttle_handler",
-        "max_requests",
-        "unit",
-        "request_quota",
-        "config",
-    )
-
-    cache: Cache
+    __slots__ = ("app", "check_throttle_handler", "max_requests", "unit", "request_quota", "config")
 
     def __init__(self, app: ASGIApp, config: RateLimitConfig) -> None:
         """Initialize ``RateLimitMiddleware``.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of RateLimitConfig.
@@ -70,32 +65,31 @@
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None
         """
-        if not hasattr(self, "cache"):
-            self.cache = scope["app"].cache
-
-        request: Request[Any, Any, Any] = scope["app"].request_class(scope)
+        app = scope["app"]
+        request: Request[Any, Any, Any] = app.request_class(scope)
+        store = self.config.get_store_from_app(app)
         if await self.should_check_request(request=request):
             key = self.cache_key_from_request(request=request)
-            cache_object = await self.retrieve_cached_history(key)
+            cache_object = await self.retrieve_cached_history(key, store)
             if len(cache_object.history) >= self.max_requests:
                 raise TooManyRequestsException(
                     headers=self.create_response_headers(cache_object=cache_object)
                     if self.config.set_rate_limit_headers
                     else None
                 )
-            await self.set_cached_history(key=key, cache_object=cache_object)
+            await self.set_cached_history(key=key, cache_object=cache_object, store=store)
             if self.config.set_rate_limit_headers:
                 send = self.create_send_wrapper(send=send, cache_object=cache_object)
 
-        await self.app(scope, receive, send)
+        await self.app(scope, receive, send)  # pyright: ignore
 
     def create_send_wrapper(self, send: Send, cache_object: CacheObject) -> Send:
         """Create a ``send`` function that wraps the original send to inject response headers.
 
         Args:
             send: The ASGI send function.
             cache_object: A StorageObject instance.
@@ -122,15 +116,15 @@
 
         return send_wrapper
 
     def cache_key_from_request(self, request: Request[Any, Any, Any]) -> str:
         """Get a cache-key from a ``Request``
 
         Args:
-            request: A :class:`Request <starlite.connection.Request>` instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A cache key.
         """
         host = request.client.host if request.client else "anonymous"
         identifier = request.headers.get("X-Forwarded-For") or request.headers.get("X-Real-IP") or host
         route_handler = request.scope["route_handler"]
@@ -138,71 +132,73 @@
             identifier += "::mount"
 
         if getattr(route_handler, "is_static", False):
             identifier += "::static"
 
         return f"{type(self).__name__}::{identifier}"
 
-    async def retrieve_cached_history(self, key: str) -> CacheObject:
+    async def retrieve_cached_history(self, key: str, store: Store) -> CacheObject:
         """Retrieve a list of time stamps for the given duration unit.
 
         Args:
             key: Cache key.
+            store: A :class:`Store <.stores.base.Store>`
 
         Returns:
-            An instance of StorageObject.
+            An :class:`CacheObject`.
         """
         duration = DURATION_VALUES[self.unit]
         now = int(time())
-        cached_string = await self.cache.get(key)
+        cached_string = await store.get(key)
         if cached_string:
             cache_object = CacheObject(**decode_json(cached_string))
             if cache_object.reset <= now:
                 return CacheObject(history=[], reset=now + duration)
 
             while cache_object.history and cache_object.history[-1] <= now - duration:
                 cache_object.history.pop()
             return cache_object
 
         return CacheObject(history=[], reset=now + duration)
 
-    async def set_cached_history(self, key: str, cache_object: CacheObject) -> None:
+    async def set_cached_history(self, key: str, cache_object: CacheObject, store: Store) -> None:
         """Store history extended with the current timestamp in cache.
 
         Args:
             key: Cache key.
-            cache_object: An instance of StorageObject.
+            cache_object: A :class:`CacheObject`.
+            store: A :class:`Store <.stores.base.Store>`
 
         Returns:
             None
         """
         cache_object.history = [int(time()), *cache_object.history]
-        await self.cache.set(key, encode_json(cache_object), expiration=DURATION_VALUES[self.unit])
+        await store.set(key, encode_json(cache_object), expires_in=DURATION_VALUES[self.unit])
 
     async def should_check_request(self, request: "Request[Any, Any, Any]") -> bool:
         """Return a boolean indicating if a request should be checked for rate limiting.
 
         Args:
-            request: A :class:`Request <starlite.connection.Request>` instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
             Boolean dictating whether the request should be checked for rate-limiting.
         """
         if self.check_throttle_handler:
             return await self.check_throttle_handler(request)
         return True
 
     def create_response_headers(self, cache_object: CacheObject) -> dict[str, str]:
         """Create ratelimit response headers.
 
         Notes:
-            * see the :func:`IETF RateLimit draft <https://datatracker.ietf.org/doc/draft-ietf-httpapi-ratelimit-headers/>`
+            * see the `IETF RateLimit draft <https://datatracker.ietf.org/doc/draft-ietf-httpapi-ratelimit-headers/>_`
 
         Args:
-            cache_object: An instance of Cache Object.
+            cache_object:A :class:`CacheObject`.
 
         Returns:
             A dict of http headers.
         """
         remaining_requests = str(
             len(cache_object.history) - self.max_requests if len(cache_object.history) <= self.max_requests else 0
         )
@@ -237,15 +233,16 @@
     """Key to use for the rate limit policy header."""
     rate_limit_remaining_header_key: str = field(default="RateLimit-Remaining")
     """Key to use for the rate limit remaining header."""
     rate_limit_reset_header_key: str = field(default="RateLimit-Reset")
     """Key to use for the rate limit reset header."""
     rate_limit_limit_header_key: str = field(default="RateLimit-Limit")
     """Key to use for the rate limit limit header."""
-    cache_key_builder: Callable[[Request], str] | None = field(default=None)
+    store: str = "rate_limit"
+    """Name of the :class:`Store <.stores.base.Store>` to use"""
 
     def __post_init__(self) -> None:
         if self.check_throttle_handler:
             self.check_throttle_handler = AsyncCallable(self.check_throttle_handler)  # type: ignore
 
     @property
     def middleware(self) -> DefineMiddleware:
@@ -256,20 +253,22 @@
 
                 from starlite import Starlite, Request, get
                 from starlite.middleware.rate_limit import RateLimitConfig
 
                 # limit to 10 requests per minute, excluding the schema path
                 throttle_config = RateLimitConfig(rate_limit=("minute", 10), exclude=["/schema"])
 
-
                 @get("/")
                 def my_handler(request: Request) -> None:
                     ...
 
-
                 app = Starlite(route_handlers=[my_handler], middleware=[throttle_config.middleware])
 
-
         Returns:
-            An instance of DefineMiddleware including ``self`` as the config kwarg value.
+            An instance of :class:`DefineMiddleware <.middleware.base.DefineMiddleware>` including ``self`` as the
+            config kwarg value.
         """
         return DefineMiddleware(self.middleware_class, config=self)
+
+    def get_store_from_app(self, app: Starlite) -> Store:
+        """Get the store defined in :attr:`store` from an :class:`Starlite <.app.Starlite>` instance."""
+        return app.stores.get(self.store)
```

### Comparing `starlite-2.0.0a1/starlite/middleware/session/base.py` & `starlite-2.0.0a2/starlite/middleware/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
     cast,
 )
 
 from starlite.connection import ASGIConnection
 from starlite.enums import ScopeType
 from starlite.middleware.base import AbstractMiddleware, DefineMiddleware
 from starlite.serialization import decode_json, encode_json
-from starlite.types import Scopes
 from starlite.utils import get_serializer_from_scope
 
+__all__ = ("BaseBackendConfig", "BaseSessionBackend", "SessionMiddleware")
+
+
 if TYPE_CHECKING:
-    from starlite.types import ASGIApp, Message, Receive, Scope, ScopeSession, Send
+    from starlite.types import ASGIApp, Message, Receive, Scope, Scopes, ScopeSession, Send
 
 ONE_DAY_IN_SECONDS = 60 * 60 * 24
 
 ConfigT = TypeVar("ConfigT", bound="BaseBackendConfig")
 BaseSessionBackendT = TypeVar("BaseSessionBackendT", bound="BaseSessionBackend")
 
 
@@ -118,16 +120,16 @@
         """Serialize data into bytes for storage in the backend.
 
         Args:
             data: Session data of the current scope.
             scope: A scope, if applicable, from which to extract a serializer.
 
         Notes:
-            - The serializer will be extracted from ``scope`` or fall back
-              to :func:`default_serializer <starlite.utils.default_serializer>`
+            - The serializer will be extracted from ``scope`` or fall back to
+                :func:`default_serializer <.serialization.default_serializer>`
 
         Returns:
             ``data`` serialized as bytes.
         """
         serializer = get_serializer_from_scope(scope) if scope else None
         return encode_json(data, serializer)
```

### Comparing `starlite-2.0.0a1/starlite/middleware/session/client_side.py` & `starlite-2.0.0a2/starlite/middleware/session/client_side.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 from base64 import b64decode, b64encode
 from dataclasses import dataclass, field
 from os import urandom
 from typing import TYPE_CHECKING, Any, Literal
 
 from starlite.datastructures import MutableScopeHeaders
 from starlite.datastructures.cookie import Cookie
+from starlite.enums import ScopeType
 from starlite.exceptions import (
     ImproperlyConfiguredException,
     MissingDependencyException,
 )
 from starlite.serialization import decode_json, encode_json
 from starlite.types import Empty, Scopes
+from starlite.utils.dataclass import extract_dataclass_fields
 
-from ...enums import ScopeType
-from ...utils.dataclass import extract_dataclass_fields
 from .base import ONE_DAY_IN_SECONDS, BaseBackendConfig, BaseSessionBackend
 
+__all__ = ("ClientSideSessionBackend", "CookieBackendConfig")
+
+
 try:
     from cryptography.exceptions import InvalidTag
     from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 except ImportError as e:
     raise MissingDependencyException("cryptography is not installed") from e
 
 if TYPE_CHECKING:
```

### Comparing `starlite-2.0.0a1/starlite/middleware/session/server_side.py` & `starlite-2.0.0a2/starlite/middleware/session/server_side.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,83 +3,83 @@
 import secrets
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Literal
 
 from starlite.datastructures import Cookie, MutableScopeHeaders
 from starlite.enums import ScopeType
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.middleware.session.base import (
-    ONE_DAY_IN_SECONDS,
-    BaseBackendConfig,
-    BaseSessionBackend,
-)
-from starlite.storage.base import Storage
+from starlite.middleware.session.base import ONE_DAY_IN_SECONDS, BaseBackendConfig, BaseSessionBackend
 from starlite.types import Empty, Message, Scopes, ScopeSession
 from starlite.utils.dataclass import extract_dataclass_fields
 
+__all__ = ("ServerSideSessionBackend", "ServerSideSessionConfig")
+
+
 if TYPE_CHECKING:
+    from starlite import Starlite
     from starlite.connection import ASGIConnection
+    from starlite.stores.base import Store
 
 
 class ServerSideSessionBackend(BaseSessionBackend["ServerSideSessionConfig"]):
     """Base class for server-side backends.
 
     Implements :class:`BaseSessionBackend` and defines and interface which subclasses can
     implement to facilitate the storage of session data.
     """
 
-    __slots__ = ("storage",)
-
     def __init__(self, config: ServerSideSessionConfig) -> None:
         """Initialize ``ServerSideSessionBackend``
 
         Args:
             config: A subclass of ``ServerSideSessionConfig``
         """
         super().__init__(config=config)
-        self.storage = config.storage
 
-    async def get(self, session_id: str) -> bytes | None:
+    async def get(self, session_id: str, store: Store) -> bytes | None:
         """Retrieve data associated with ``session_id``.
 
         Args:
             session_id: The session-ID
+            store: Store to retrieve the session data from
 
         Returns:
             The session data, if existing, otherwise ``None``.
         """
         max_age = int(self.config.max_age) if self.config.max_age is not None else None
-        return await self.storage.get(session_id, renew_for=max_age if self.config.renew_on_access else None)
+        return await store.get(session_id, renew_for=max_age if self.config.renew_on_access else None)
 
-    async def set(self, session_id: str, data: bytes) -> None:
+    async def set(self, session_id: str, data: bytes, store: Store) -> None:
         """Store ``data`` under the ``session_id`` for later retrieval.
 
         If there is already data associated with ``session_id``, replace
         it with ``data`` and reset its expiry time
 
         Args:
             session_id: The session-ID
             data: Serialized session data
+            store: Store to save the session data in
 
         Returns:
             None
         """
         expires_in = int(self.config.max_age) if self.config.max_age is not None else None
-        await self.storage.set(session_id, data, expires_in=expires_in)
+        await store.set(session_id, data, expires_in=expires_in)
 
-    async def delete(self, session_id: str) -> None:
+    async def delete(self, session_id: str, store: Store) -> None:
         """Delete the data associated with ``session_id``. Fails silently if no such session-ID exists.
 
         Args:
             session_id: The session-ID
+            store: Store to delete the session data from
 
         Returns:
             None
         """
-        await self.storage.delete(session_id)
+        await store.delete(session_id)
 
     def generate_session_id(self) -> str:
         """Generate a new session-ID, with
         n=:attr:`session_id_bytes <ServerSideSessionConfig.session_id_bytes>` random bytes.
 
         Returns:
             A session-ID
@@ -100,30 +100,31 @@
             message: Outgoing send-message
             connection: Originating ASGIConnection containing the scope
 
         Returns:
             None
         """
         scope = connection.scope
+        store = self.config.get_store_from_app(scope["app"])
         headers = MutableScopeHeaders.from_message(message)
         session_id = connection.cookies.get(self.config.key)
         if not session_id or session_id == "null":
             session_id = self.generate_session_id()
 
         cookie_params = dict(extract_dataclass_fields(self.config, exclude_none=True, include=Cookie.__dict__))
 
         if scope_session is Empty:
-            await self.delete(session_id)
+            await self.delete(session_id, store=store)
             headers.add(
                 "Set-Cookie",
                 Cookie(value="null", key=self.config.key, expires=0, **cookie_params).to_header(header=""),
             )
         else:
             serialised_data = self.serialize_data(scope_session, scope)
-            await self.set(session_id=session_id, data=serialised_data)
+            await self.set(session_id=session_id, data=serialised_data, store=store)
             headers["Set-Cookie"] = Cookie(value=session_id, key=self.config.key, **cookie_params).to_header(header="")
 
     async def load_from_connection(self, connection: "ASGIConnection") -> dict[str, Any]:
         """Load session data from a connection and return it as a dictionary to be used in the current application
         scope.
 
         The session-ID will be gathered from a cookie with the key set in
@@ -136,28 +137,27 @@
             connection: An ASGIConnection instance
 
         Returns:
             The current session data
         """
         session_id = connection.cookies.get(self.config.key)
         if session_id:
-            data = await self.get(session_id)
+            store = self.config.get_store_from_app(connection.scope["app"])
+            data = await self.get(session_id, store=store)
             if data is not None:
                 return self.deserialize_data(data)
         return {}
 
 
 @dataclass
 class ServerSideSessionConfig(BaseBackendConfig[ServerSideSessionBackend]):
     """Base configuration for server side backends."""
 
     _backend_class = ServerSideSessionBackend
 
-    storage: Storage
-    """:class:`.storage.base.Storage <Storage>` to use"""
     session_id_bytes: int = field(default=32)
     """Number of bytes used to generate a random session-ID."""
     renew_on_access: bool = field(default=False)
     """Renew expiry times of sessions when they're being accessed"""
     key: str = field(default="session")
     """Key to use for the cookie inside the header, e.g. ``session=<data>`` where ``session`` is the cookie key and
     ``<data>`` is the session data.
@@ -179,21 +179,24 @@
     domain: str | None = field(default=None)
     """Domain for which the cookie is valid."""
     secure: bool = field(default=False)
     """Https is required for the cookie."""
     httponly: bool = field(default=True)
     """Forbids javascript to access the cookie via 'Document.cookie'."""
     samesite: Literal["lax", "strict", "none"] = field(default="lax")
-    """Controls whether or not a cookie is sent with cross-site requests.
-
-    Defaults to ``lax``.
-    """
+    """Controls whether or not a cookie is sent with cross-site requests. Defaults to ``lax``."""
     exclude: str | list[str] | None = field(default=None)
     """A pattern or list of patterns to skip in the session middleware."""
     exclude_opt_key: str = field(default="skip_session")
     """An identifier to use on routes to disable the session middleware for a particular route."""
+    store: str = "sessions"
+    """Name of the :class:`Store <.stores.base.Store>` to use"""
 
     def __post_init__(self) -> None:
         if len(self.key) < 1 or len(self.key) > 256:
             raise ImproperlyConfiguredException("key must be a string with a length between 1-256")
         if self.max_age < 1:
             raise ImproperlyConfiguredException("max_age must be greater than 0")
+
+    def get_store_from_app(self, app: Starlite) -> Store:
+        """Get the store defined in :attr:`store` from an :class:`Starlite <.app.Starlite>` instance"""
+        return app.stores.get(self.store)
```

### Comparing `starlite-2.0.0a1/starlite/middleware/utils.py` & `starlite-2.0.0a2/starlite/middleware/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Pattern
 
 from starlite.exceptions import ImproperlyConfiguredException
 
+__all__ = ("build_exclude_path_pattern", "should_bypass_middleware")
+
+
 if TYPE_CHECKING:
     from starlite.types import Scope, Scopes
 
 
 def build_exclude_path_pattern(*, exclude: str | list[str] | None = None) -> Pattern | None:
     """Build single path pattern from list of patterns to opt-out from middleware processing.
```

### Comparing `starlite-2.0.0a1/starlite/multipart.py` & `starlite-2.0.0a2/starlite/_multipart.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 from typing import Any, DefaultDict
 from urllib.parse import unquote
 
 from starlite.datastructures.upload_file import UploadFile
 from starlite.exceptions import SerializationException, ValidationException
 from starlite.serialization import decode_json
 
-_token = r"([\w!#$%&'*+\-.^_`|~]+)"
+__all__ = ("parse_body", "parse_content_header", "parse_multipart_form")
+
+
+_token = r"([\w!#$%&'*+\-.^_`|~]+)"  # noqa: S105
 _quoted = r'"([^"]*)"'
 _param = re.compile(rf";\s*{_token}=(?:{_token}|{_quoted})", re.ASCII)
 _firefox_quote_escape = re.compile(r'\\"(?!; |\s*$)')
 
 
 def parse_content_header(value: str) -> tuple[str, dict[str, str]]:
     """Parse content-type and content-disposition header values.
@@ -61,18 +64,20 @@
     return value.strip().lower(), options
 
 
 def parse_body(body: bytes, boundary: bytes, multipart_form_part_limit: int) -> list[bytes]:
     """Split the body using the boundary
         and validate the number of form parts is within the allowed limit.
 
-    :param body: The form body.
-    :param boundary: The boundary used to separate form components.
-    :param multipart_form_part_limit: The limit of allowed form components
-    :return:
+    Args:
+        body: The form body.
+        boundary: The boundary used to separate form components.
+        multipart_form_part_limit: The limit of allowed form components
+
+    Returns:
         A list of form components.
     """
     if not (body and boundary):
         return []
 
     form_parts = body.split(boundary, multipart_form_part_limit + 3)[1:-1]
```

### Comparing `starlite-2.0.0a1/starlite/openapi/controller.py` & `starlite-2.0.0a2/starlite/openapi/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,46 @@
+from __future__ import annotations
+
+from copy import copy
 from functools import cached_property
-from typing import TYPE_CHECKING, Callable, Dict, Literal, cast
+from typing import TYPE_CHECKING, Callable, Literal, cast
 
 from yaml import dump as dump_yaml
 
-from starlite.connection import Request
 from starlite.controller import Controller
 from starlite.enums import MediaType, OpenAPIMediaType
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.handlers import get
 from starlite.response import Response
 from starlite.serialization import encode_json
 from starlite.status_codes import HTTP_404_NOT_FOUND
 
+__all__ = ("OpenAPIController", "OpenAPISchemaResponse")
+
+
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0.open_api import OpenAPI
+    from starlite.connection.request import Request
+    from starlite.openapi.spec.open_api import OpenAPI
 
 MSG_OPENAPI_NOT_INITIALIZED = "Starlite has not been instantiated with OpenAPIConfig"
 
 
 class OpenAPISchemaResponse(Response):
     """Response class for OpenAPI Schemas."""
 
     def render(self, content: "OpenAPI") -> bytes:
         """Handle rendering of schema into the correct format - either YAML or JSON.
 
         Args:
-            content: The :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.open_api.OpenAPI>` instance to render.
+            content: The :class:`OpenAPI <starlite.openapi.spec.open_api.OpenAPI>` instance to render.
 
         Returns:
             Rendered bytes.
         """
-        content_dict = content.dict(by_alias=True, exclude_none=True)
+        content_dict = content.to_schema()
         if self.media_type == OpenAPIMediaType.OPENAPI_YAML:
             return cast("bytes", dump_yaml(content_dict, default_flow_style=False).encode("utf-8"))
         return encode_json(content_dict)
 
 
 class OpenAPIController(Controller):
     """Controller for OpenAPI endpoints."""
@@ -84,18 +90,18 @@
     _dumped_modified_schema: str = ""
 
     @staticmethod
     def get_schema_from_request(request: Request) -> "OpenAPI":
         """Return the OpenAPI pydantic model from the request instance.
 
         Args:
-            request: A :class:`Starlite <starlite.connection.Request>` instance.
+            request: A :class:`Starlite <.connection.Request>` instance.
 
         Returns:
-            An :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.open_api.OpenAPI>` instance.
+            An :class:`OpenAPI <starlite.openapi.spec.open_api.OpenAPI>` instance.
 
         Raises:
             ImproperlyConfiguredException: If the application ``openapi_config`` attribute is ``None``.
         """
         if not request.app.openapi_schema:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
         return request.app.openapi_schema
@@ -128,23 +134,23 @@
         if request_path & config.enabled_endpoints:
             return True
 
         return False
 
     @property
     def favicon(self) -> str:
-        """Return favicon `<link>` tag, if applicable.
+        """Return favicon ``<link>`` tag, if applicable.
 
         Returns:
-            A `<link>` tag if self.favicon_url is not empty, otherwise returns a placeholder meta tag.
+            A ``<link>`` tag if ``self.favicon_url`` is not empty, otherwise returns a placeholder meta tag.
         """
         return f"<link rel='icon' type='image/x-icon' href='{self.favicon_url}'>" if self.favicon_url else "<meta/>"
 
     @cached_property
-    def render_methods_map(self) -> Dict[Literal["redoc", "swagger", "elements"], Callable[[Request], str]]:
+    def render_methods_map(self) -> dict[Literal["redoc", "swagger", "elements"], Callable[[Request], str]]:
         """Map render method names to render methods.
 
         Returns:
             A mapping of string keys to render methods.
         """
         return {
             "redoc": self.render_redoc,
@@ -154,19 +160,19 @@
 
     @get(
         path="/openapi.yaml",
         media_type=OpenAPIMediaType.OPENAPI_YAML,
         include_in_schema=False,
     )
     def retrieve_schema_yaml(self, request: Request) -> Response:
-        """Return the OpenAPI schema as YAML with an 'application/vnd.oai.openapi' Content-Type header.
+        """Return the OpenAPI schema as YAML with an ``application/vnd.oai.openapi`` Content-Type header.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response instance with the YAML object rendered into a string.
         """
         if not request.app.openapi_config:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
 
@@ -174,19 +180,19 @@
             return OpenAPISchemaResponse(
                 content=self.get_schema_from_request(request), media_type=OpenAPIMediaType.OPENAPI_YAML
             )
         return Response(content={}, status_code=HTTP_404_NOT_FOUND)
 
     @get(path="/openapi.json", media_type=OpenAPIMediaType.OPENAPI_JSON, include_in_schema=False)
     def retrieve_schema_json(self, request: Request) -> Response:
-        """Return the OpenAPI schema as JSON with an 'application/vnd.oai.openapi+json' Content-Type header.
+        """Return the OpenAPI schema as JSON with an ``application/vnd.oai.openapi+json`` Content-Type header.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response instance with the JSON object rendered into a string.
         """
         if not request.app.openapi_config:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
 
@@ -196,21 +202,20 @@
             )
         return Response(content={}, status_code=HTTP_404_NOT_FOUND)
 
     @get(path="/", media_type=MediaType.HTML, include_in_schema=False)
     def root(self, request: Request) -> Response:
         """Render a static documentation site.
 
-         The site to be rendered is based on the ``root_schema_site`` value set in the
-         application's :class:`OpenAPIConfig <starlite.config.openapi.OpenAPIConfig>`.
-         Defaults to ``redoc``.
+         The site to be rendered is based on the ``root_schema_site`` value set in the application's
+         :class:`OpenAPIConfig <.openapi.OpenAPIConfig>`. Defaults to ``redoc``.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with the rendered site defined in root_schema_site.
 
         Raises:
             ImproperlyConfiguredException: If the application ``openapi_config`` attribute is ``None``.
         """
@@ -231,18 +236,18 @@
 
     @get(path="/swagger", media_type=MediaType.HTML, include_in_schema=False)
     def swagger_ui(self, request: Request) -> Response:
         """Route handler responsible for rendering Swagger-UI.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
-            response: With a rendered swagger documentation site
+            A response with a rendered swagger documentation site
         """
         if not request.app.openapi_config:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
 
         if self.should_serve_endpoint(request):
             return Response(content=self.render_swagger_ui(request), media_type=MediaType.HTML)
         return Response(
@@ -253,15 +258,15 @@
 
     @get(path="/elements", media_type=MediaType.HTML, include_in_schema=False)
     def stoplight_elements(self, request: Request) -> Response:
         """Route handler responsible for rendering StopLight Elements.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered stoplight elements documentation site
         """
         if not request.app.openapi_config:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
 
@@ -271,15 +276,15 @@
 
     @get(path="/redoc", media_type=MediaType.HTML, include_in_schema=False)
     def redoc(self, request: Request) -> Response:  # pragma: no cover
         """Route handler responsible for rendering Redoc.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered redoc documentation site
         """
         if not request.app.openapi_config:  # pragma: no cover
             raise ImproperlyConfiguredException(MSG_OPENAPI_NOT_INITIALIZED)
 
@@ -291,28 +296,27 @@
         """Render an HTML page for Swagger-UI.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A rendered html string.
         """
         schema = self.get_schema_from_request(request)
+
         # Note: Fix for Swagger rejection OpenAPI >=3.1
         if not self._dumped_modified_schema:
-            schema_copy = schema.copy()
+            schema_copy = copy(schema)
             schema_copy.openapi = "3.0.3"
 
-            self._dumped_modified_schema = encode_json(schema_copy.json(by_alias=True, exclude_none=True)).decode(
-                "utf-8"
-            )
+            self._dumped_modified_schema = encode_json(schema_copy.to_schema()).decode("utf-8")
 
         head = f"""
           <head>
             <title>{schema.info.title}</title>
             {self.favicon}
             <meta charset="utf-8"/>
             <meta name="viewport" content="width=device-width, initial-scale=1">
@@ -324,15 +328,15 @@
         """
 
         body = f"""
           <body>
             <div id='swagger-container'/>
             <script type="text/javascript">
             const ui = SwaggerUIBundle({{
-                spec: JSON.parse({self._dumped_modified_schema}),
+                spec: {self._dumped_modified_schema},
                 dom_id: '#swagger-container',
                 deepLinking: true,
                 showExtensions: true,
                 showCommonExtensions: true,
                 presets: [
                     SwaggerUIBundle.presets.apis,
                     SwaggerUIBundle.SwaggerUIStandalonePreset
@@ -354,15 +358,15 @@
         """Render an HTML page for StopLight Elements.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A rendered html string.
         """
         schema = self.get_schema_from_request(request)
         head = f"""
           <head>
@@ -398,23 +402,23 @@
         """Render an HTML page for Redoc.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
-                A :class:`Request <starlite.connection.Request>` instance.
+                A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A rendered html string.
         """
         schema = self.get_schema_from_request(request)
 
         if not self._dumped_schema:
-            self._dumped_schema = encode_json(schema.json(by_alias=True, exclude_none=True)).decode("utf-8")
+            self._dumped_schema = encode_json(schema.to_schema()).decode("utf-8")
 
         head = f"""
           <head>
             <title>{schema.info.title}</title>
             {self.favicon}
             <meta charset="utf-8"/>
             <meta name="viewport" content="width=device-width, initial-scale=1">
@@ -434,15 +438,15 @@
         """
 
         body = f"""
           <body>
             <div id='redoc-container'/>
             <script type="text/javascript">
                 Redoc.init(
-                    JSON.parse({self._dumped_schema}),
+                    {self._dumped_schema},
                     undefined,
                     document.getElementById('redoc-container')
                 )
             </script>
           </body>
         """
```

### Comparing `starlite-2.0.0a1/starlite/openapi/enums.py` & `starlite-2.0.0a2/starlite/openapi/spec/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from enum import Enum
 
+__all__ = ("OpenAPIFormat", "OpenAPIType")
 
-class OpenAPIFormat(str, Enum):
-    """Formats extracted from:
 
-    https://datatracker.ietf.org/doc/html/draft-bhutton-json-schema-validation-00#page-13
-    """
+class OpenAPIFormat(str, Enum):
+    """Formats extracted from: https://datatracker.ietf.org/doc/html/draft-bhutton-json-schema-validation-00#page-13"""
 
     DATE = "date"
     DATE_TIME = "date-time"
     TIME = "time"
     DURATION = "duration"
     URL = "url"
     EMAIL = "email"
@@ -20,15 +19,15 @@
     IPV6 = "ipv6"
     URI = "uri"
     URI_REFERENCE = "uri-reference"
     URI_TEMPLATE = "uri-template"
     JSON_POINTER = "json-pointer"
     RELATIVE_JSON_POINTER = "relative-json-pointer"
     IRI = "iri-reference"
-    IRI_REFERENCE = "iri-reference"
+    IRI_REFERENCE = "iri-reference"  # noqa: PIE796
     UUID = "uuid"
     REGEX = "regex"
 
 
 class OpenAPIType(str, Enum):
     """An OopenAPI type."""
```

### Comparing `starlite-2.0.0a1/starlite/openapi/parameters.py` & `starlite-2.0.0a2/starlite/_openapi/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,57 @@
-from typing import TYPE_CHECKING, Dict, List, Tuple
+from __future__ import annotations
 
-from pydantic_openapi_schema.v3_1_0.parameter import Parameter
+from typing import TYPE_CHECKING
 
+from starlite._openapi.schema_generation import create_schema
+from starlite._signature.models import SignatureField
 from starlite.constants import RESERVED_KWARGS
 from starlite.enums import ParamType
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.openapi.schema import create_schema
+from starlite.openapi.spec.parameter import Parameter
+from starlite.openapi.spec.schema import Schema
 from starlite.params import DependencyKwarg, ParameterKwarg
-from starlite.signature.models import SignatureField
 from starlite.types import Empty
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0.schema import Schema
+__all__ = (
+    "ParameterCollection",
+    "create_parameter",
+    "create_parameter_for_handler",
+    "create_path_parameter_schema",
+    "get_layered_parameter",
+    "get_recursive_handler_parameters",
+)
+
 
+if TYPE_CHECKING:
     from starlite.handlers.base import BaseRouteHandler
+    from starlite.openapi.spec import Reference
     from starlite.types import Dependencies
     from starlite.types.internal_types import PathParameterDefinition
 
 
 def create_path_parameter_schema(
-    path_parameter: "PathParameterDefinition", field: "SignatureField", generate_examples: bool
-) -> "Schema":
+    path_parameter: "PathParameterDefinition",
+    field: "SignatureField",
+    generate_examples: bool,
+    schemas: dict[str, Schema],
+) -> Schema | Reference:
     """Create a path parameter from the given path_param definition."""
     return create_schema(
         field=SignatureField(
-            name=field.name,
-            field_type=path_parameter.type,
             children=None,
+            default_value=field.default_value,
             extra=field.extra,
+            field_type=path_parameter.type,
             kwarg_model=field.kwarg_model,
-            default_value=field.default_value,
+            name=field.name,
         ),
         generate_examples=generate_examples,
         plugins=[],
+        schemas=schemas,
     )
 
 
 class ParameterCollection:
     """Facilitates conditional deduplication of parameters.
 
     If multiple parameters with the same name are produced for a handler, the condition is ignored if the two
@@ -47,15 +62,15 @@
     def __init__(self, route_handler: "BaseRouteHandler") -> None:
         """Initialize ``ParameterCollection``.
 
         Args:
             route_handler: Associated route handler
         """
         self.route_handler = route_handler
-        self._parameters: Dict[str, Parameter] = {}
+        self._parameters: dict[str, Parameter] = {}
 
     def add(self, parameter: Parameter) -> None:
         """Add a ``Parameter`` to the collection.
 
         If an existing parameter with the same name and type already exists, the
         parameter is ignored.
 
@@ -71,37 +86,36 @@
             return
 
         raise ImproperlyConfiguredException(
             f"OpenAPI schema generation for handler `{self.route_handler}` detected multiple parameters named "
             f"'{parameter.name}' with different types."
         )
 
-    def list(self) -> List[Parameter]:
+    def list(self) -> list[Parameter]:
         """Return a list of all ``Parameter``'s in the collection."""
         return list(self._parameters.values())
 
 
 def create_parameter(
     signature_field: "SignatureField",
     parameter_name: str,
-    path_parameters: Tuple["PathParameterDefinition", ...],
+    path_parameters: tuple["PathParameterDefinition", ...],
     generate_examples: bool,
+    schemas: dict[str, "Schema"],
 ) -> Parameter:
     """Create an OpenAPI Parameter instance."""
-    schema = None
+    result: Schema | Reference | None = None
     kwargs_model = signature_field.kwarg_model if isinstance(signature_field.kwarg_model, ParameterKwarg) else None
 
     if any(path_param.name == parameter_name for path_param in path_parameters):
         param_in = ParamType.PATH
         is_required = True
         path_parameter = [p for p in path_parameters if parameter_name in p.name][0]
-        schema = create_path_parameter_schema(
-            path_parameter=path_parameter,
-            field=signature_field,
-            generate_examples=generate_examples,
+        result = create_path_parameter_schema(
+            field=signature_field, generate_examples=generate_examples, path_parameter=path_parameter, schemas=schemas
         )
 
     elif kwargs_model and kwargs_model.header:
         parameter_name = kwargs_model.header
         param_in = ParamType.HEADER
         is_required = signature_field.is_required
     elif kwargs_model and kwargs_model.cookie:
@@ -109,59 +123,66 @@
         param_in = ParamType.COOKIE
         is_required = signature_field.is_required
     else:
         is_required = signature_field.is_required
         param_in = ParamType.QUERY
         parameter_name = kwargs_model.query if kwargs_model and kwargs_model.query else parameter_name
 
-    if not schema:
-        schema = create_schema(field=signature_field, generate_examples=generate_examples, plugins=[])
+    if not result:
+        result = create_schema(field=signature_field, generate_examples=generate_examples, plugins=[], schemas=schemas)
+
+    schema = result if isinstance(result, Schema) else schemas[result.value]
 
     return Parameter(
+        description=schema.description,
         name=parameter_name,
         param_in=param_in,
         required=is_required,
-        param_schema=schema,
-        description=schema.description,
+        schema=result,
     )
 
 
 def get_recursive_handler_parameters(
     field_name: str,
     signature_field: "SignatureField",
     dependencies: "Dependencies",
     route_handler: "BaseRouteHandler",
-    path_parameters: Tuple["PathParameterDefinition", ...],
+    path_parameters: tuple["PathParameterDefinition", ...],
     generate_examples: bool,
-) -> List[Parameter]:
+    schemas: dict[str, "Schema"],
+) -> list[Parameter]:
     """Create and return parameters for a handler.
 
     If the provided field is not a dependency, a normal parameter is created and returned as a list, otherwise
     `create_parameter_for_handler()` is called to generate parameters for the dependency.
     """
 
     if field_name not in dependencies:
         return [
             create_parameter(
-                signature_field=signature_field,
+                generate_examples=generate_examples,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
-                generate_examples=generate_examples,
+                schemas=schemas,
+                signature_field=signature_field,
             )
         ]
     dependency_fields = dependencies[field_name].signature_model.fields
-    return create_parameter_for_handler(route_handler, dependency_fields, path_parameters, generate_examples)
+    return create_parameter_for_handler(
+        route_handler, dependency_fields, path_parameters, generate_examples, schemas=schemas
+    )
 
 
 def get_layered_parameter(
     field_name: str,
     signature_field: "SignatureField",
-    layered_parameters: Dict[str, "SignatureField"],
-    path_parameters: Tuple["PathParameterDefinition", ...],
+    layered_parameters: dict[str, "SignatureField"],
+    path_parameters: tuple["PathParameterDefinition", ...],
     generate_examples: bool,
+    schemas: dict[str, "Schema"],
 ) -> Parameter:
     """Create a layered parameter for a given signature model field.
 
     Layer info is extracted from the provided ``layered_parameters`` dict and set as the field's ``field_info`` attribute.
     """
     layer_field = layered_parameters[field_name]
 
@@ -171,33 +192,35 @@
 
     parameter_name = field_name
     if isinstance(field.kwarg_model, ParameterKwarg):
         parameter_name = field.kwarg_model.query or field.kwarg_model.header or field.kwarg_model.cookie or field_name
 
     return create_parameter(
         signature_field=SignatureField.create(
+            children=field.children,
             default_value=default_value,
+            extra=field.extra,
+            field_type=field_type,
             kwarg_model=field.kwarg_model,
             name=field_name,
-            field_type=field_type,
-            extra=field.extra,
-            children=field.children,
         ),
+        generate_examples=generate_examples,
         parameter_name=parameter_name,
         path_parameters=path_parameters,
-        generate_examples=generate_examples,
+        schemas=schemas,
     )
 
 
 def create_parameter_for_handler(
     route_handler: "BaseRouteHandler",
-    handler_fields: Dict[str, "SignatureField"],
-    path_parameters: Tuple["PathParameterDefinition", ...],
+    handler_fields: dict[str, "SignatureField"],
+    path_parameters: tuple["PathParameterDefinition", ...],
     generate_examples: bool,
-) -> List[Parameter]:
+    schemas: dict[str, "Schema"],
+) -> list[Parameter]:
     """Create a list of path/query/header Parameter models for the given PathHandler."""
     parameters = ParameterCollection(route_handler=route_handler)
     dependencies = route_handler.resolve_dependencies()
 
     layered_parameters = route_handler.resolve_layered_parameters()
 
     unique_handler_fields = tuple(
@@ -212,38 +235,41 @@
 
     for field_name, signature_field in unique_handler_fields:
         if isinstance(signature_field.kwarg_model, DependencyKwarg) and field_name not in dependencies:
             # never document explicit dependencies
             continue
 
         for parameter in get_recursive_handler_parameters(
-            field_name=field_name,
-            signature_field=signature_field,
             dependencies=dependencies,
-            route_handler=route_handler,
-            path_parameters=path_parameters,
+            field_name=field_name,
             generate_examples=generate_examples,
+            path_parameters=path_parameters,
+            route_handler=route_handler,
+            schemas=schemas,
+            signature_field=signature_field,
         ):
             parameters.add(parameter)
 
     for field_name, signature_field in unique_layered_fields:
         parameters.add(
             create_parameter(
-                signature_field=signature_field,
+                generate_examples=generate_examples,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
-                generate_examples=generate_examples,
+                schemas=schemas,
+                signature_field=signature_field,
             )
         )
 
     for field_name, signature_field in intersection_fields:
         parameters.add(
             get_layered_parameter(
                 field_name=field_name,
-                signature_field=signature_field,
+                generate_examples=generate_examples,
                 layered_parameters=layered_parameters,
                 path_parameters=path_parameters,
-                generate_examples=generate_examples,
+                schemas=schemas,
+                signature_field=signature_field,
             )
         )
 
     return parameters.list()
```

### Comparing `starlite-2.0.0a1/starlite/openapi/path_item.py` & `starlite-2.0.0a2/starlite/_openapi/path_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from inspect import cleandoc
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
+from __future__ import annotations
 
-from pydantic_openapi_schema.v3_1_0.operation import Operation
-from pydantic_openapi_schema.v3_1_0.path_item import PathItem
+from inspect import cleandoc
+from typing import TYPE_CHECKING
 
-from starlite.openapi.parameters import create_parameter_for_handler
-from starlite.openapi.request_body import create_request_body
-from starlite.openapi.responses import create_responses
-from starlite.openapi.utils import SEPARATORS_CLEANUP_PATTERN
+from starlite._openapi.parameters import create_parameter_for_handler
+from starlite._openapi.request_body import create_request_body
+from starlite._openapi.responses import create_responses
+from starlite._openapi.utils import SEPARATORS_CLEANUP_PATTERN
+from starlite.openapi.spec.operation import Operation
+from starlite.openapi.spec.path_item import PathItem
 from starlite.utils.helpers import unwrap_partial
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
+__all__ = ("create_path_item", "extract_layered_values", "get_description_for_handler")
 
+
+if TYPE_CHECKING:
     from starlite.handlers.http_handlers import HTTPRouteHandler
-    from starlite.plugins.base import OpenAPISchemaPluginProtocol
+    from starlite.openapi.spec import Schema, SecurityRequirement
+    from starlite.plugins import OpenAPISchemaPluginProtocol
     from starlite.routes import HTTPRoute
     from starlite.types.callable_types import OperationIDCreator
 
 
-def get_description_for_handler(route_handler: "HTTPRouteHandler", use_handler_docstrings: bool) -> Optional[str]:
+def get_description_for_handler(route_handler: "HTTPRouteHandler", use_handler_docstrings: bool) -> str | None:
     """Produce the operation description for a route handler, either by using the description value if provided,
 
     or the docstring - if config is enabled.
 
     Args:
         route_handler: A route handler instance.
         use_handler_docstrings: If ``True`` and `route_handler.description`` is ``None` returns docstring of wrapped
@@ -37,80 +40,100 @@
         fn = unwrap_partial(route_handler.fn.value)
         return cleandoc(fn.__doc__) if fn.__doc__ else None
     return handler_description
 
 
 def extract_layered_values(
     route_handler: "HTTPRouteHandler",
-) -> Tuple[Optional[List[str]], Optional[List[Dict[str, List[str]]]]]:
+) -> tuple[list[str] | None, list[dict[str, list[str]]] | None]:
     """Extract the tags and security values from the route handler layers.
 
     Args:
         route_handler: A Route Handler instance.
 
     Returns:
         A tuple of optional lists.
     """
-    tags: List[str] = []
-    security: List["SecurityRequirement"] = []
+    tags: list[str] = []
+    security: list["SecurityRequirement"] = []
     for layer in route_handler.ownership_layers:
         if layer.tags:
             tags.extend(layer.tags)
         if layer.security:
             security.extend(layer.security)
     return sorted(set(tags)) if tags else None, security or None
 
 
 def create_path_item(
-    route: "HTTPRoute",
     create_examples: bool,
-    plugins: List["OpenAPISchemaPluginProtocol"],
-    use_handler_docstrings: bool,
     operation_id_creator: "OperationIDCreator",
-) -> Tuple[PathItem, List[str]]:
-    """Create a PathItem model for the given route parsing all http_methods into Operation Models."""
+    plugins: list["OpenAPISchemaPluginProtocol"],
+    route: "HTTPRoute",
+    schemas: dict[str, "Schema"],
+    use_handler_docstrings: bool,
+) -> tuple[PathItem, list[str]]:
+    """Create a PathItem for the given route parsing all http_methods into Operation Models.
+
+    Args:
+        create_examples: Whether to auto-generate examples.
+        operation_id_creator: A function to generate operation ids.
+        plugins: A list of plugins.
+        route: An HTTPRoute instance.
+        schemas: A mapping of schemas.
+        use_handler_docstrings: Whether to use the handler docstring.
+
+    Returns:
+        A tuple containing the path item and a list of operation ids.
+    """
     path_item = PathItem()
-    operation_ids: List[str] = []
+    operation_ids: list[str] = []
 
     for http_method, handler_tuple in route.route_handler_map.items():
         route_handler, _ = handler_tuple
+
         if route_handler.include_in_schema:
             handler_fields = route_handler.signature_model.fields if route_handler.signature_model else {}
             parameters = (
                 create_parameter_for_handler(
                     route_handler=route_handler,
                     handler_fields=handler_fields,
                     path_parameters=route.path_parameters,
                     generate_examples=create_examples,
+                    schemas=schemas,
                 )
                 or None
             )
             raises_validation_error = bool("data" in handler_fields or path_item.parameters or parameters)
 
             request_body = None
             if "data" in handler_fields:
                 request_body = create_request_body(
-                    field=handler_fields["data"], generate_examples=create_examples, plugins=plugins
+                    field=handler_fields["data"],
+                    generate_examples=create_examples,
+                    plugins=plugins,
+                    schemas=schemas,
                 )
             operation_id = route_handler.operation_id or operation_id_creator(
                 route_handler, http_method, route.path_components
             )
             tags, security = extract_layered_values(route_handler)
             operation = Operation(
-                operationId=operation_id,
+                operation_id=operation_id,
                 tags=tags,
                 summary=route_handler.summary or SEPARATORS_CLEANUP_PATTERN.sub("", route_handler.handler_name.title()),
                 description=get_description_for_handler(route_handler, use_handler_docstrings),
                 deprecated=route_handler.deprecated,
                 responses=create_responses(
                     route_handler=route_handler,
                     raises_validation_error=raises_validation_error,
                     generate_examples=create_examples,
                     plugins=plugins,
+                    schemas=schemas,
                 ),
-                requestBody=request_body,
+                request_body=request_body,
                 parameters=parameters,  # type: ignore[arg-type]
                 security=security,
             )
             operation_ids.append(operation_id)
             setattr(path_item, http_method.lower(), operation)
+
     return path_item, operation_ids
```

### Comparing `starlite-2.0.0a1/starlite/openapi/request_body.py` & `starlite-2.0.0a2/starlite/_openapi/request_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from __future__ import annotations
 
-from pydantic_openapi_schema.v3_1_0.media_type import (
-    MediaType as OpenAPISchemaMediaType,
-)
-from pydantic_openapi_schema.v3_1_0.request_body import RequestBody
+from typing import TYPE_CHECKING
 
+from starlite._openapi.schema_generation import create_schema
 from starlite.enums import RequestEncodingType
-from starlite.openapi.schema import create_schema, update_schema_with_signature_field
+from starlite.openapi.spec.media_type import OpenAPIMediaType
+from starlite.openapi.spec.request_body import RequestBody
 from starlite.params import BodyKwarg
 
+__all__ = ("create_request_body",)
+
+
 if TYPE_CHECKING:
-    from starlite.plugins.base import OpenAPISchemaPluginProtocol
-    from starlite.signature.models import SignatureField
+    from starlite._signature.models import SignatureField
+    from starlite.openapi.spec import Schema
+    from starlite.plugins import OpenAPISchemaPluginProtocol
 
 
 def create_request_body(
-    field: "SignatureField", generate_examples: bool, plugins: List["OpenAPISchemaPluginProtocol"]
-) -> Optional[RequestBody]:
+    field: "SignatureField",
+    generate_examples: bool,
+    plugins: list["OpenAPISchemaPluginProtocol"],
+    schemas: dict[str, "Schema"],
+) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
-    media_type: Union[RequestEncodingType, str] = RequestEncodingType.JSON
+    media_type: RequestEncodingType | str = RequestEncodingType.JSON
     if isinstance(field.kwarg_model, BodyKwarg) and field.kwarg_model.media_type:
         media_type = field.kwarg_model.media_type
 
-    schema = create_schema(field=field, generate_examples=generate_examples, plugins=plugins)
-    update_schema_with_signature_field(schema=schema, signature_field=field)
-    return RequestBody(required=True, content={media_type: OpenAPISchemaMediaType(media_type_schema=schema)})
+    schema = create_schema(field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+    return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `starlite-2.0.0a1/starlite/openapi/responses.py` & `starlite-2.0.0a2/starlite/_openapi/responses.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,52 @@
+from __future__ import annotations
+
+import re
 from copy import copy
+from dataclasses import asdict
 from http import HTTPStatus
 from operator import attrgetter
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Type
+from typing import TYPE_CHECKING, Any, Iterator
 
-from pydantic_openapi_schema.v3_1_0 import Response
-from pydantic_openapi_schema.v3_1_0.header import Header
-from pydantic_openapi_schema.v3_1_0.media_type import (
-    MediaType as OpenAPISchemaMediaType,
-)
-from pydantic_openapi_schema.v3_1_0.schema import Schema
 from typing_extensions import get_args, get_origin
 
+from starlite._openapi.schema_generation import create_schema
+from starlite._signature.models import SignatureField
 from starlite.enums import MediaType
-from starlite.exceptions import (
-    HTTPException,
-    ImproperlyConfiguredException,
-    ValidationException,
-)
-from starlite.openapi.enums import OpenAPIFormat, OpenAPIType
-from starlite.openapi.schema import create_schema
-from starlite.openapi.utils import pascal_case_to_text
+from starlite.exceptions import HTTPException, ValidationException
+from starlite.openapi.spec import OpenAPIResponse
+from starlite.openapi.spec.enums import OpenAPIFormat, OpenAPIType
+from starlite.openapi.spec.header import OpenAPIHeader
+from starlite.openapi.spec.media_type import OpenAPIMediaType
+from starlite.openapi.spec.schema import Schema
 from starlite.response import Response as StarliteResponse
 from starlite.response_containers import File, Redirect, Stream, Template
-from starlite.signature.models import SignatureField
 from starlite.utils import get_enum_string_value, get_name, is_class_and_subclass
 
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0.responses import Responses
-
     from starlite.datastructures.cookie import Cookie
     from starlite.handlers.http_handlers import HTTPRouteHandler
-    from starlite.plugins.base import OpenAPISchemaPluginProtocol
+    from starlite.openapi.spec.responses import Responses
+    from starlite.plugins import OpenAPISchemaPluginProtocol
+
+
+__all__ = (
+    "create_additional_responses",
+    "create_cookie_schema",
+    "create_error_responses",
+    "create_responses",
+    "create_success_response",
+)
+
+CAPITAL_LETTERS_PATTERN = re.compile(r"(?=[A-Z])")
+
+
+def pascal_case_to_text(string: str) -> str:
+    """Given a 'PascalCased' string, return its split form- 'Pascal Cased'."""
+    return " ".join(re.split(CAPITAL_LETTERS_PATTERN, string)).strip()
 
 
 def create_cookie_schema(cookie: "Cookie") -> Schema:
     """Given a Cookie instance, return its corresponding OpenAPI schema.
 
     Args:
         cookie: Cookie
@@ -45,198 +57,207 @@
     cookie_copy = copy(cookie)
     cookie_copy.value = "<string>"
     value = cookie_copy.to_header(header="")
     return Schema(description=cookie.description or "", example=value)
 
 
 def create_success_response(
-    route_handler: "HTTPRouteHandler", generate_examples: bool, plugins: List["OpenAPISchemaPluginProtocol"]
-) -> Response:
+    route_handler: "HTTPRouteHandler",
+    generate_examples: bool,
+    plugins: list["OpenAPISchemaPluginProtocol"],
+    schemas: dict[str, "Schema"],
+) -> OpenAPIResponse:
     """Create the schema for a success response."""
     signature = route_handler.signature
-    default_descriptions: Dict[Any, str] = {
+    default_descriptions: dict[Any, str] = {
         Stream: "Stream Response",
         Redirect: "Redirect Response",
         File: "File Download",
     }
     description = (
         route_handler.response_description
         or default_descriptions.get(signature.return_annotation)
         or HTTPStatus(route_handler.status_code).description
     )
 
     if signature.return_annotation not in {signature.empty, None, Redirect, File, Stream}:
         return_annotation = signature.return_annotation
         if signature.return_annotation is Template:
-            return_annotation = str  # since templates return str
+            return_annotation = str
             route_handler.media_type = get_enum_string_value(MediaType.HTML)
         elif is_class_and_subclass(get_origin(signature.return_annotation), StarliteResponse):
             return_annotation = get_args(signature.return_annotation)[0] or Any
 
-        schema = create_schema(
+        result = create_schema(
             field=SignatureField.create(field_type=return_annotation),
             generate_examples=generate_examples,
             plugins=plugins,
+            schemas=schemas,
         )
-        schema.contentEncoding = route_handler.content_encoding
-        schema.contentMediaType = route_handler.content_media_type
-        response = Response(
+
+        schema = result if isinstance(result, Schema) else schemas[result.value]
+
+        schema.content_encoding = route_handler.content_encoding
+        schema.content_media_type = route_handler.content_media_type
+
+        response = OpenAPIResponse(
             content={
-                route_handler.media_type: OpenAPISchemaMediaType(
-                    media_type_schema=schema,
+                route_handler.media_type: OpenAPIMediaType(
+                    schema=result,
                 )
             },
             description=description,
         )
 
     elif signature.return_annotation is Redirect:
-        response = Response(
+        response = OpenAPIResponse(
             content=None,
             description=description,
             headers={
-                "location": Header(
-                    param_schema=Schema(type=OpenAPIType.STRING), description="target path for the redirect"
+                "location": OpenAPIHeader(
+                    schema=Schema(type=OpenAPIType.STRING), description="target path for the redirect"
                 )
             },
         )
 
     elif signature.return_annotation in (File, Stream):
-        response = Response(
+        response = OpenAPIResponse(
             content={
-                route_handler.media_type: OpenAPISchemaMediaType(
-                    media_type_schema=Schema(
+                route_handler.media_type: OpenAPIMediaType(
+                    schema=Schema(
                         type=OpenAPIType.STRING,
-                        contentEncoding=route_handler.content_encoding or "application/octet-stream",
-                        contentMediaType=route_handler.content_media_type,
+                        content_encoding=route_handler.content_encoding or "application/octet-stream",
+                        content_media_type=route_handler.content_media_type,
                     ),
                 )
             },
             description=description,
             headers={
-                "content-length": Header(
-                    param_schema=Schema(type=OpenAPIType.STRING), description="File size in bytes"
+                "content-length": OpenAPIHeader(
+                    schema=Schema(type=OpenAPIType.STRING), description="File size in bytes"
                 ),
-                "last-modified": Header(
-                    param_schema=Schema(type=OpenAPIType.STRING, schema_format=OpenAPIFormat.DATE_TIME),
+                "last-modified": OpenAPIHeader(
+                    schema=Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.DATE_TIME),
                     description="Last modified data-time in RFC 2822 format",
                 ),
-                "etag": Header(param_schema=Schema(type=OpenAPIType.STRING), description="Entity tag"),
+                "etag": OpenAPIHeader(schema=Schema(type=OpenAPIType.STRING), description="Entity tag"),
             },
         )
 
     else:
-        response = Response(
+        response = OpenAPIResponse(
             content=None,
             description=description,
         )
 
     if response.headers is None:
         response.headers = {}
 
     for response_header in route_handler.resolve_response_headers():
-        header = Header()
-        for attribute_name, attribute_value in response_header.dict(exclude_none=True).items():
+        header = OpenAPIHeader()
+        for attribute_name, attribute_value in ((k, v) for k, v in asdict(response_header).items() if v is not None):
             if attribute_name == "value":
-                header.param_schema = create_schema(
+                header.schema = create_schema(
                     field=SignatureField.create(field_type=type(attribute_value)),
                     generate_examples=False,
                     plugins=plugins,
+                    schemas=schemas,
                 )
 
             elif attribute_name != "documentation_only":
                 setattr(header, attribute_name, attribute_value)
+
         response.headers[response_header.name] = header
 
     if cookies := route_handler.resolve_response_cookies():
-        response.headers["Set-Cookie"] = Header(
-            param_schema=Schema(
-                allOf=[create_cookie_schema(cookie=cookie) for cookie in sorted(cookies, key=attrgetter("key"))]
+        response.headers["Set-Cookie"] = OpenAPIHeader(
+            schema=Schema(
+                all_of=[create_cookie_schema(cookie=cookie) for cookie in sorted(cookies, key=attrgetter("key"))]
             )
         )
 
     return response
 
 
-def create_error_responses(exceptions: List[Type[HTTPException]]) -> Iterator[Tuple[str, Response]]:
+def create_error_responses(exceptions: list[type[HTTPException]]) -> Iterator[tuple[str, OpenAPIResponse]]:
     """Create the schema for error responses, if any."""
-    grouped_exceptions: Dict[int, List[Type[HTTPException]]] = {}
+    grouped_exceptions: dict[int, list[type[HTTPException]]] = {}
     for exc in exceptions:
         if not grouped_exceptions.get(exc.status_code):
             grouped_exceptions[exc.status_code] = []
         grouped_exceptions[exc.status_code].append(exc)
     for status_code, exception_group in grouped_exceptions.items():
         exceptions_schemas = [
             Schema(
                 type=OpenAPIType.OBJECT,
                 required=["detail", "status_code"],
                 properties={
                     "status_code": Schema(type=OpenAPIType.INTEGER),
                     "detail": Schema(type=OpenAPIType.STRING),
                     "extra": Schema(
-                        type=[OpenAPIType.NULL, OpenAPIType.OBJECT, OpenAPIType.ARRAY], additionalProperties=Schema()
+                        type=[OpenAPIType.NULL, OpenAPIType.OBJECT, OpenAPIType.ARRAY], additional_properties=Schema()
                     ),
                 },
                 description=pascal_case_to_text(get_name(exc)),
                 examples=[{"status_code": status_code, "detail": HTTPStatus(status_code).phrase, "extra": {}}],
             )
             for exc in exception_group
         ]
-        if len(exceptions_schemas) > 1:
-            schema = Schema(oneOf=exceptions_schemas)  # type:ignore[arg-type]
+        if len(exceptions_schemas) > 1:  # noqa: SIM108
+            schema = Schema(one_of=exceptions_schemas)
         else:
             schema = exceptions_schemas[0]
-        yield str(status_code), Response(
+        yield str(status_code), OpenAPIResponse(
             description=HTTPStatus(status_code).description,
-            content={MediaType.JSON: OpenAPISchemaMediaType(media_type_schema=schema)},
+            content={MediaType.JSON: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_additional_responses(
-    route_handler: "HTTPRouteHandler", plugins: List["OpenAPISchemaPluginProtocol"]
-) -> Iterator[Tuple[str, Response]]:
+    route_handler: "HTTPRouteHandler",
+    plugins: list["OpenAPISchemaPluginProtocol"],
+    schemas: dict[str, "Schema"],
+) -> Iterator[tuple[str, OpenAPIResponse]]:
     """Create the schema for additional responses, if any."""
     if not route_handler.responses:
         return
 
     for status_code, additional_response in route_handler.responses.items():
         schema = create_schema(
-            field=SignatureField.create(field_type=additional_response.model),
+            field=SignatureField.create(field_type=additional_response.data_container),
             generate_examples=additional_response.generate_examples,
             plugins=plugins,
+            schemas=schemas,
         )
-        yield str(status_code), Response(
+        yield str(status_code), OpenAPIResponse(
             description=additional_response.description,
-            content={additional_response.media_type: OpenAPISchemaMediaType(media_type_schema=schema)},
+            content={additional_response.media_type: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_responses(
     route_handler: "HTTPRouteHandler",
     raises_validation_error: bool,
     generate_examples: bool,
-    plugins: List["OpenAPISchemaPluginProtocol"],
-) -> Optional["Responses"]:
+    plugins: list["OpenAPISchemaPluginProtocol"],
+    schemas: dict[str, "Schema"],
+) -> Responses | None:
     """Create a Response model embedded in a `Responses` dictionary for the given RouteHandler or return None."""
 
-    responses: "Responses" = {
+    responses: Responses = {
         str(route_handler.status_code): create_success_response(
-            route_handler=route_handler,
-            generate_examples=generate_examples,
-            plugins=plugins,
+            generate_examples=generate_examples, plugins=plugins, route_handler=route_handler, schemas=schemas
         ),
     }
 
     exceptions = list(route_handler.raises or [])
     if raises_validation_error and ValidationException not in exceptions:
         exceptions.append(ValidationException)
     for status_code, response in create_error_responses(exceptions=exceptions):
         responses[status_code] = response
 
-    for status_code, response in create_additional_responses(route_handler, plugins):
-        if status_code in responses:
-            raise ImproperlyConfiguredException(
-                f"Additional response for status code {status_code} already exists in success or error responses"
-            )
-
+    for status_code, response in create_additional_responses(
+        route_handler=route_handler, plugins=plugins, schemas=schemas
+    ):
         responses[status_code] = response
 
     return responses or None
```

### Comparing `starlite-2.0.0a1/starlite/openapi/typescript_converter/converter.py` & `starlite-2.0.0a2/starlite/_openapi/typescript_converter/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,73 @@
+from __future__ import annotations
+
 from copy import copy
-from typing import Any, List, Optional, Tuple, TypeVar, Union, cast
+from dataclasses import fields
+from typing import Any, TypeVar, cast
 
-from pydantic import BaseModel
-from pydantic_openapi_schema.v3_1_0 import (
+from starlite._openapi.typescript_converter.schema_parsing import (
+    normalize_typescript_namespace,
+    parse_schema,
+)
+from starlite._openapi.typescript_converter.types import (
+    TypeScriptInterface,
+    TypeScriptNamespace,
+    TypeScriptPrimitive,
+    TypeScriptProperty,
+    TypeScriptType,
+    TypeScriptUnion,
+)
+from starlite.enums import HttpMethod, ParamType
+from starlite.openapi.spec import (
     Components,
     OpenAPI,
     Operation,
     Parameter,
     Reference,
     RequestBody,
     Responses,
     Schema,
 )
 
-from starlite.enums import HttpMethod, ParamType
-from starlite.openapi.typescript_converter.schema_parsing import (
-    normalize_typescript_namespace,
-    parse_schema,
-)
-from starlite.openapi.typescript_converter.types import (
-    TypeScriptInterface,
-    TypeScriptNamespace,
-    TypeScriptPrimitive,
-    TypeScriptProperty,
-    TypeScriptType,
-    TypeScriptUnion,
+__all__ = (
+    "convert_openapi_to_typescript",
+    "deref_container",
+    "get_openapi_type",
+    "parse_params",
+    "parse_request_body",
+    "parse_responses",
+    "resolve_ref",
 )
 
-T = TypeVar("T", bound=Union[BaseModel, dict, list])
+from starlite.openapi.spec.base import BaseSchemaObject
 
+T = TypeVar("T")
 
-def _deref_model(model: BaseModel, components: Components) -> BaseModel:
-    for field in model.__fields__:
-        if value := getattr(model, field, None):
-            if isinstance(value, Reference):
-                setattr(model, field, deref_container(resolve_ref(value, components=components), components=components))
-            elif isinstance(value, (Schema, (dict, list))):
-                setattr(model, field, deref_container(value, components=components))
-    return model
 
+def _deref_schema_object(value: BaseSchemaObject, components: Components) -> BaseSchemaObject:
+    for field in fields(value):
+        if field_value := getattr(value, field.name, None):
+            if isinstance(field_value, Reference):
+                setattr(
+                    value,
+                    field.name,
+                    deref_container(resolve_ref(field_value, components=components), components=components),
+                )
+            elif isinstance(field_value, (Schema, dict, list)):
+                setattr(value, field.name, deref_container(field_value, components=components))
+    return value
 
-def _deref_dict(values: dict, components: Components) -> dict:
-    for key, value in values.items():
-        if isinstance(value, Reference):
-            values[key] = deref_container(resolve_ref(value, components=components), components=components)
-        elif isinstance(value, (Schema, (dict, list))):
-            values[key] = deref_container(value, components=components)
-    return values
+
+def _deref_dict(value: dict, components: Components) -> dict:
+    for k, v in value.items():
+        if isinstance(v, Reference):
+            value[k] = deref_container(resolve_ref(v, components=components), components=components)
+        elif isinstance(v, (Schema, dict, list)):
+            value[k] = deref_container(v, components=components)
+    return value
 
 
 def _deref_list(values: list, components: Components) -> list:
     for i, value in enumerate(values):
         if isinstance(value, Reference):
             values[i] = deref_container(resolve_ref(value, components=components), components=components)
         elif isinstance(value, (Schema, (dict, list))):
@@ -64,22 +81,23 @@
     Args:
         open_api_container: Either an OpenAPI content, a dict or a list.
         components: The OpenAPI schema Components section.
 
     Returns:
         A dereferenced object.
     """
-
-    if isinstance(open_api_container, BaseModel):
-        return cast("T", _deref_model(open_api_container.copy(), components))
+    if isinstance(open_api_container, BaseSchemaObject):
+        return cast("T", _deref_schema_object(open_api_container, components))
 
     if isinstance(open_api_container, dict):
         return cast("T", _deref_dict(copy(open_api_container), components))
 
-    return cast("T", _deref_list(copy(open_api_container), components))  # type: ignore
+    if isinstance(open_api_container, list):
+        return cast("T", _deref_list(copy(open_api_container), components))
+    raise ValueError(f"unexpected container type {type(open_api_container).__name__}")  # pragma: no cover
 
 
 def resolve_ref(ref: Reference, components: Components) -> Schema:
     """Resolve a reference object into the actual value it points at.
 
     Args:
         ref: A Reference instance.
@@ -96,64 +114,66 @@
         raise ValueError(
             f"unexpected value type, expected schema but received {type(current).__name__ if current is not None else 'None'}"
         )
 
     return current
 
 
-def get_openapi_type(value: Union[Reference, T], components: Components) -> T:
+def get_openapi_type(value: Reference | T, components: Components) -> T:
     """Extract or dereference an OpenAPI container type.
 
     Args:
         value: Either a reference or a container type.
         components: The OpenAPI schema Components section.
 
     Returns:
         The extracted container.
     """
     if isinstance(value, Reference):
-        return cast("T", deref_container(resolve_ref(value, components=components), components=components))
-    return deref_container(value, components=components)
+        resolved_ref = resolve_ref(value, components=components)
+        return cast("T", deref_container(open_api_container=resolved_ref, components=components))
+
+    return deref_container(open_api_container=value, components=components)
 
 
 def parse_params(
-    params: List[Parameter],
+    params: list[Parameter],
     components: Components,
-) -> Tuple[TypeScriptInterface, ...]:
+) -> tuple[TypeScriptInterface, ...]:
     """Parse request parameters.
 
     Args:
         params: An OpenAPI Operation parameters.
         components: The OpenAPI schema Components section.
 
     Returns:
         A tuple of resolved interfaces.
     """
-    cookie_params: List[TypeScriptProperty] = []
-    header_params: List[TypeScriptProperty] = []
-    path_params: List[TypeScriptProperty] = []
-    query_params: List[TypeScriptProperty] = []
+    cookie_params: list[TypeScriptProperty] = []
+    header_params: list[TypeScriptProperty] = []
+    path_params: list[TypeScriptProperty] = []
+    query_params: list[TypeScriptProperty] = []
 
     for param in params:
-        if param.param_schema and (schema := get_openapi_type(param.param_schema, components)):
+        if param.schema and (schema := get_openapi_type(param.schema, components)):
             ts_prop = TypeScriptProperty(
                 key=normalize_typescript_namespace(param.name, allow_quoted=True),
                 required=param.required,
                 value=parse_schema(schema),
             )
             if param.param_in == ParamType.COOKIE:
                 cookie_params.append(ts_prop)
             elif param.param_in == ParamType.HEADER:
                 header_params.append(ts_prop)
             elif param.param_in == ParamType.PATH:
                 path_params.append(ts_prop)
             else:
                 query_params.append(ts_prop)
 
-    result: List[TypeScriptInterface] = []
+    result: list[TypeScriptInterface] = []
 
     if cookie_params:
         result.append(TypeScriptInterface("CookieParameters", tuple(cookie_params)))
     if header_params:
         result.append(TypeScriptInterface("HeaderParameters", tuple(header_params)))
     if path_params:
         result.append(TypeScriptInterface("PathParameters", tuple(path_params)))
@@ -173,51 +193,43 @@
     Returns:
         A TypeScript type.
     """
     undefined = TypeScriptPrimitive("undefined")
     if not body.content:
         return TypeScriptType("RequestBody", undefined)
 
-    if (
-        content := [
-            get_openapi_type(v.media_type_schema, components) for v in body.content.values() if v.media_type_schema
-        ]
-    ) and (schema := content[0]):
+    if (content := [get_openapi_type(v.schema, components) for v in body.content.values() if v.schema]) and (
+        schema := content[0]
+    ):
         return TypeScriptType(
             "RequestBody",
             parse_schema(schema) if body.required else TypeScriptUnion((parse_schema(content[0]), undefined)),
         )
 
     return TypeScriptType("RequestBody", undefined)
 
 
-def parse_responses(responses: Responses, components: Components) -> Tuple[TypeScriptNamespace, ...]:
+def parse_responses(responses: Responses, components: Components) -> tuple[TypeScriptNamespace, ...]:
     """Parse a given Operation's Responses object.
 
     Args:
         responses: An OpenAPI Responses object.
         components: The OpenAPI schema Components section.
 
     Returns:
         A tuple of namespaces, mapping response codes to data.
     """
-    result: List[TypeScriptNamespace] = []
+    result: list[TypeScriptNamespace] = []
     for http_status, response in [
         (status, get_openapi_type(res, components=components)) for status, res in responses.items()
     ]:
         if (
             response
             and response.content
-            and (
-                content := [
-                    get_openapi_type(v.media_type_schema, components)
-                    for v in response.content.values()
-                    if v.media_type_schema
-                ]
-            )
+            and (content := [get_openapi_type(v.schema, components) for v in response.content.values() if v.schema])
         ):
             ts_type = parse_schema(content[0])
         else:
             ts_type = TypeScriptPrimitive("undefined")
 
         containers = [
             TypeScriptType("ResponseBody", ts_type),
@@ -253,47 +265,47 @@
         A string representing the generated types.
     """
     if not openapi_schema.paths:  # pragma: no cover
         raise ValueError("OpenAPI schema has no paths")
     if not openapi_schema.components:  # pragma: no cover
         raise ValueError("OpenAPI schema has no components")
 
-    operations: List[TypeScriptNamespace] = []
+    operations: list[TypeScriptNamespace] = []
 
     for path_item in openapi_schema.paths.values():
         shared_params = [
             get_openapi_type(p, components=openapi_schema.components) for p in (path_item.parameters or []) if p
         ]
         for method in HttpMethod:
             if (
-                operation := cast("Optional[Operation]", getattr(path_item, method.lower(), "None"))
-            ) and operation.operationId:
+                operation := cast("Operation | None", getattr(path_item, method.lower(), "None"))
+            ) and operation.operation_id:
                 params = parse_params(
                     [
                         *(
                             get_openapi_type(p, components=openapi_schema.components)
                             for p in (operation.parameters or [])
                             if p
                         ),
                         *shared_params,
                     ],
                     components=openapi_schema.components,
                 )
                 request_body = (
                     parse_request_body(
-                        get_openapi_type(operation.requestBody, components=openapi_schema.components),
+                        get_openapi_type(operation.request_body, components=openapi_schema.components),
                         components=openapi_schema.components,
                     )
-                    if operation.requestBody
+                    if operation.request_body
                     else None
                 )
 
                 responses = parse_responses(operation.responses or {}, components=openapi_schema.components)
 
                 operations.append(
                     TypeScriptNamespace(
-                        normalize_typescript_namespace(operation.operationId, allow_quoted=False),
+                        normalize_typescript_namespace(operation.operation_id, allow_quoted=False),
                         tuple(container for container in (*params, request_body, *responses) if container),
                     )
                 )
 
     return TypeScriptNamespace(namespace, tuple(operations))
```

### Comparing `starlite-2.0.0a1/starlite/openapi/typescript_converter/schema_parsing.py` & `starlite-2.0.0a2/starlite/_openapi/typescript_converter/schema_parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-import re
-from typing import Any, Dict, Literal, Optional, Set, Union, cast, overload
+from __future__ import annotations
 
-from pydantic_openapi_schema.v3_1_0 import Schema
-from typing_extensions import TypeGuard
+import re
+from typing import TYPE_CHECKING, Any, Literal, overload
 
-from starlite.openapi.enums import OpenAPIType
-from starlite.openapi.typescript_converter.types import (
+from starlite._openapi.typescript_converter.types import (
     TypeScriptAnonymousInterface,
     TypeScriptArray,
     TypeScriptElement,
     TypeScriptInterface,
     TypeScriptIntersection,
     TypeScriptLiteral,
     TypeScriptPrimitive,
     TypeScriptProperty,
     TypeScriptUnion,
 )
+from starlite.openapi.spec import Schema
+from starlite.openapi.spec.enums import OpenAPIType
+
+__all__ = ("create_interface", "is_schema_value", "normalize_typescript_namespace", "parse_schema", "parse_type_schema")
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeGuard
 
 openapi_typescript_equivalent_types = Literal[
     "string", "boolean", "number", "null", "Record<string, unknown>", "unknown[]"
 ]
 
-openapi_to_typescript_type_map: Dict[OpenAPIType, openapi_typescript_equivalent_types] = {
+openapi_to_typescript_type_map: dict[OpenAPIType, openapi_typescript_equivalent_types] = {
     OpenAPIType.ARRAY: "unknown[]",
     OpenAPIType.BOOLEAN: "boolean",
     OpenAPIType.INTEGER: "number",
     OpenAPIType.NULL: "null",
     OpenAPIType.NUMBER: "number",
     OpenAPIType.OBJECT: "Record<string, unknown>",
     OpenAPIType.STRING: "string",
@@ -63,26 +68,26 @@
     Returns:
         A typeguard boolean dictating whether the passed in value is a Schema.
     """
     return isinstance(value, Schema)
 
 
 @overload
-def create_interface(properties: Dict[str, Schema], required: Optional[Set[str]]) -> TypeScriptAnonymousInterface:
+def create_interface(properties: dict[str, Schema], required: set[str] | None) -> TypeScriptAnonymousInterface:
     ...
 
 
 @overload
-def create_interface(properties: Dict[str, Schema], required: Optional[Set[str]], name: str) -> TypeScriptInterface:
+def create_interface(properties: dict[str, Schema], required: set[str] | None, name: str) -> TypeScriptInterface:
     ...
 
 
 def create_interface(
-    properties: Dict[str, Schema], required: Optional[Set[str]] = None, name: Optional[str] = None
-) -> Union[TypeScriptAnonymousInterface, TypeScriptInterface]:
+    properties: dict[str, Schema], required: set[str] | None = None, name: str | None = None
+) -> TypeScriptAnonymousInterface | TypeScriptInterface:
     """Create a typescript interface from the given schema.properties values.
 
     Args:
         properties: schema.properties mapping.
         required: An optional list of required properties.
         name: An optional string representing the interface name.
 
@@ -100,52 +105,49 @@
     return (
         TypeScriptInterface(name=name, properties=parsed_properties)
         if name is not None
         else TypeScriptAnonymousInterface(properties=parsed_properties)
     )
 
 
-def parse_type_schema(schema: Schema) -> Union[TypeScriptPrimitive, TypeScriptLiteral, TypeScriptUnion]:
+def parse_type_schema(schema: Schema) -> TypeScriptPrimitive | TypeScriptLiteral | TypeScriptUnion:
     """Parse an OpenAPI schema representing a primitive type(s).
 
     Args:
         schema: An OpenAPI schema.
 
     Returns:
         A typescript type.
     """
     if schema.enum:
         return TypeScriptUnion(types=tuple(TypeScriptLiteral(value=value) for value in schema.enum))
     if schema.const:
         return TypeScriptLiteral(value=schema.const)
     if isinstance(schema.type, list):
         return TypeScriptUnion(
-            tuple(
-                TypeScriptPrimitive(openapi_to_typescript_type_map[cast("OpenAPIType", s_type)])
-                for s_type in schema.type
-            )
+            tuple(TypeScriptPrimitive(openapi_to_typescript_type_map[s_type]) for s_type in schema.type)
         )
-    if schema.type in openapi_to_typescript_type_map:
-        return TypeScriptPrimitive(openapi_to_typescript_type_map[cast("OpenAPIType", schema.type)])
+    if schema.type in openapi_to_typescript_type_map and isinstance(schema.type, OpenAPIType):
+        return TypeScriptPrimitive(openapi_to_typescript_type_map[schema.type])
     raise TypeError(f"received an unexpected openapi type: {schema.type}")  # pragma: no cover
 
 
 def parse_schema(schema: Schema) -> TypeScriptElement:
     """Parse an OpenAPI schema object recursively to create typescript types.
 
     Args:
         schema: An OpenAPI Schema object.
 
     Returns:
         A typescript type.
     """
-    if schema.allOf:
-        return TypeScriptIntersection(tuple(parse_schema(s) for s in schema.allOf if is_schema_value(s)))
-    if schema.oneOf:
-        return TypeScriptUnion(tuple(parse_schema(s) for s in schema.oneOf if is_schema_value(s)))
+    if schema.all_of:
+        return TypeScriptIntersection(tuple(parse_schema(s) for s in schema.all_of if is_schema_value(s)))
+    if schema.one_of:
+        return TypeScriptUnion(tuple(parse_schema(s) for s in schema.one_of if is_schema_value(s)))
     if is_schema_value(schema.items):
         return TypeScriptArray(parse_schema(schema.items))
     if schema.type == OpenAPIType.OBJECT:
         return create_interface(
             properties={k: v for k, v in schema.properties.items() if is_schema_value(v)} if schema.properties else {},
             required=set(schema.required) if schema.required else None,
         )
```

### Comparing `starlite-2.0.0a1/starlite/openapi/typescript_converter/types.py` & `starlite-2.0.0a2/starlite/_openapi/typescript_converter/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Literal, Tuple, Union
+from typing import Any, Literal
+
+__all__ = (
+    "TypeScriptAnonymousInterface",
+    "TypeScriptArray",
+    "TypeScriptConst",
+    "TypeScriptContainer",
+    "TypeScriptElement",
+    "TypeScriptEnum",
+    "TypeScriptInterface",
+    "TypeScriptIntersection",
+    "TypeScriptLiteral",
+    "TypeScriptNamespace",
+    "TypeScriptPrimitive",
+    "TypeScriptProperty",
+    "TypeScriptType",
+    "TypeScriptUnion",
+)
 
 
 def _as_string(value: Any) -> str:
     if isinstance(value, str):
         return '"' + value + '"'
 
     if isinstance(value, bool):
@@ -44,15 +63,15 @@
         raise NotImplementedError("")
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptIntersection(TypeScriptElement):
     """A class representing a TypeScript intersection type."""
 
-    types: Tuple[TypeScriptElement, ...]
+    types: tuple[TypeScriptElement, ...]
 
     def write(self) -> str:
         """Write a typescript intersection value.
 
         Example:
             { prop: string } & { another: number }
 
@@ -62,15 +81,15 @@
         return " & ".join(t.write() for t in self.types)
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptUnion(TypeScriptElement):
     """A class representing a TypeScript union type."""
 
-    types: Tuple[TypeScriptElement, ...]
+    types: tuple[TypeScriptElement, ...]
 
     def write(self) -> str:
         """Write a typescript union value.
 
         Example:
             string | number
 
@@ -100,15 +119,15 @@
         return self.type
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptLiteral(TypeScriptElement):
     """A class representing a TypeScript literal type."""
 
-    value: Union[str, int, float, bool, None]
+    value: str | int | float | bool | None
 
     def write(self) -> str:
         """Write a typescript literal type.
 
         Example:
             "someValue"
 
@@ -162,15 +181,15 @@
         return f"{self.key}{':' if self.required else '?:'} {self.value.write()};"
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptAnonymousInterface(TypeScriptElement):
     """A class representing a TypeScript anonymous interface."""
 
-    properties: Tuple[TypeScriptProperty, ...]
+    properties: tuple[TypeScriptProperty, ...]
 
     def write(self) -> str:
         """Write a typescript interface object, without a name.
 
         Example:
             {
                 key: string;
@@ -185,15 +204,15 @@
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptInterface(TypeScriptContainer):
     """A class representing a TypeScript interface."""
 
     name: str
-    properties: Tuple[TypeScriptProperty, ...]
+    properties: tuple[TypeScriptProperty, ...]
 
     def write(self) -> str:
         """Write a typescript interface.
 
         Example:
             export interface MyInterface {
                 key: string;
@@ -208,15 +227,15 @@
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptEnum(TypeScriptContainer):
     """A class representing a TypeScript enum."""
 
     name: str
-    values: Union[Tuple[Tuple[str, str], ...], Tuple[Tuple[str, Union[int, float]], ...]]
+    values: tuple[tuple[str, str], ...] | tuple[tuple[str, int | float], ...]
 
     def write(self) -> str:
         """Write a typescript enum.
 
         Example:
             export enum MyEnum {
                 DOG = "canine",
@@ -252,15 +271,15 @@
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptConst(TypeScriptContainer):
     """A class representing a TypeScript const."""
 
     name: str
-    value: Union[TypeScriptPrimitive, TypeScriptLiteral]
+    value: TypeScriptPrimitive | TypeScriptLiteral
 
     def write(self) -> str:
         """Write a typescript const.
 
         Example:
             export const MyConst: number;
 
@@ -271,15 +290,15 @@
 
 
 @dataclass(unsafe_hash=True)
 class TypeScriptNamespace(TypeScriptContainer):
     """A class representing a TypeScript namespace."""
 
     name: str
-    values: Tuple[TypeScriptContainer, ...]
+    values: tuple[TypeScriptContainer, ...]
 
     def write(self) -> str:
         """Write a typescript namespace.
 
         Example:
             export MyNamespace {
                 export const MyConst: number;
```

### Comparing `starlite-2.0.0a1/starlite/pagination.py` & `starlite-2.0.0a2/starlite/pagination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Generic, TypeVar
 from uuid import UUID
 
+__all__ = (
+    "AbstractAsyncClassicPaginator",
+    "AbstractAsyncCursorPaginator",
+    "AbstractAsyncOffsetPaginator",
+    "AbstractSyncClassicPaginator",
+    "AbstractSyncCursorPaginator",
+    "AbstractSyncOffsetPaginator",
+    "ClassicPagination",
+    "CursorPagination",
+    "OffsetPagination",
+)
+
+
 T = TypeVar("T")
 C = TypeVar("C", int, str, UUID)
 
 
 @dataclass
 class ClassicPagination(Generic[T]):
     """Container for data returned using limit/offset pagination."""
```

### Comparing `starlite-2.0.0a1/starlite/params.py` & `starlite-2.0.0a2/starlite/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 from dataclasses import asdict, dataclass, field
 from typing import TYPE_CHECKING, Any, Hashable
 
 from starlite.enums import RequestEncodingType
 from starlite.types import Empty
 
+__all__ = ("Body", "BodyKwarg", "Dependency", "DependencyKwarg", "Parameter", "ParameterKwarg")
+
+
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0.example import Example
-    from pydantic_openapi_schema.v3_1_0.external_documentation import (
+    from starlite.openapi.spec.example import Example
+    from starlite.openapi.spec.external_documentation import (
         ExternalDocumentation,
     )
 
 
 @dataclass(frozen=True)
 class ParameterKwarg:
     """Data container representing a parameter."""
```

### Comparing `starlite-2.0.0a1/starlite/parsers.py` & `starlite-2.0.0a2/starlite/_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from http.cookies import _unquote as unquote_cookie
 from typing import Any, Iterable
 from urllib.parse import unquote
 
 from fast_query_parsers import parse_query_string as fast_parse_query_string
 from fast_query_parsers import parse_url_encoded_dict
 
+__all__ = ("parse_cookie_string", "parse_headers", "parse_query_string", "parse_url_encoded_form_data")
+
 
 @lru_cache(1024)
 def parse_url_encoded_form_data(encoded_data: bytes) -> dict[str, Any]:
     """Parse an url encoded form data dict.
 
     Args:
         encoded_data: The encoded byte string.
```

### Comparing `starlite-2.0.0a1/starlite/partial.py` & `starlite-2.0.0a2/starlite/partial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from dataclasses import MISSING
+from dataclasses import MISSING, dataclass
 from dataclasses import Field as DataclassField
-from dataclasses import dataclass
 from inspect import getmro
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Generic,
     Optional,
@@ -23,26 +22,30 @@
 from starlite.types.builtin_types import NoneType
 from starlite.utils.predicates import (
     is_class_and_subclass,
     is_dataclass_class,
     is_typed_dict,
 )
 
+__all__ = ("Partial",)
+
+
 try:
     # python 3.9 changed these variable
     from typing import _UnionGenericAlias as GenericAlias  # type: ignore
 except ImportError:  # pragma: no cover
     from typing import _GenericAlias as GenericAlias  # type: ignore
 
 if TYPE_CHECKING:
-    from starlite.types.builtin_types import DataclassClass, TypedDictClass
+    from starlite.types import DataclassProtocol
+    from starlite.types.builtin_types import TypedDictClass
 
 T = TypeVar("T")
 
-SupportedTypes: TypeAlias = "Union[DataclassClass, Type[BaseModel], TypedDictClass]"
+SupportedTypes: TypeAlias = "Union[Type[DataclassProtocol], Type[BaseModel], TypedDictClass]"
 """Types that are supported by :class:`Partial <starlite.types.partial.Partial>`"""
 
 
 class Partial(Generic[T]):
     """Type generation for PATCH routes.
 
     Partial is a special typing helper that takes a generic T, which must be a
@@ -92,22 +95,22 @@
                 field_definitions[field_name] = (Optional[field_type], None)
             else:
                 field_definitions[field_name] = (field_type, None)
 
         cls._models[item] = create_model(cls._create_partial_type_name(item), __base__=item, **field_definitions)  # type: ignore
 
     @classmethod
-    def _create_partial_dataclass(cls, item: "DataclassClass") -> None:
+    def _create_partial_dataclass(cls, item: "Type[DataclassProtocol]") -> None:
         """Receives a dataclass class and creates an all optional subclass of it.
 
         Args:
             item: A dataclass class.
         """
         fields: Dict[str, DataclassField] = cls._create_optional_field_map(item)
-        partial_type: "DataclassClass" = dataclass(
+        partial_type: "Type[DataclassProtocol]" = dataclass(
             type(cls._create_partial_type_name(item), (item,), {"__dataclass_fields__": fields})
         )
         annotated_ancestors = [a for a in getmro(partial_type) if hasattr(a, "__annotations__")]
         for ancestor in annotated_ancestors:
             for field_name, annotation in ancestor.__annotations__.items():
                 if not isinstance(annotation, GenericAlias) or NoneType not in annotation.__args__:
                     partial_type.__annotations__[field_name] = Optional[annotation]
@@ -125,19 +128,18 @@
         """
         type_hints: Dict[str, Any] = {}
         for key_name, value_type in get_type_hints(item).items():
             if NoneType in get_args(value_type):
                 type_hints[key_name] = value_type
                 continue
             type_hints[key_name] = Optional[value_type]
-        type_name = cls._create_partial_type_name(item)
-        cls._models[item] = TypedDict(type_name, type_hints, total=False)  # type:ignore
+        cls._models[item] = TypedDict(cls._create_partial_type_name(item), type_hints, total=False)  # type:ignore
 
     @staticmethod
-    def _create_optional_field_map(item: "DataclassClass") -> Dict[str, DataclassField]:
+    def _create_optional_field_map(item: "Type[DataclassProtocol]") -> Dict[str, DataclassField]:
         """Create a map of field name to optional dataclass Fields for a given dataclass.
 
         Args:
             item: A dataclass class.
 
         Returns:
             A map of field name to optional dataclass fields.
```

### Comparing `starlite-2.0.0a1/starlite/plugins/base.py` & `starlite-2.0.0a2/starlite/plugins.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,27 @@
 )
 
 from pydantic import BaseModel
 from typing_extensions import TypeGuard, get_args
 
 from starlite.types.protocols import DataclassProtocol
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import Schema
+__all__ = (
+    "InitPluginProtocol",
+    "OpenAPISchemaPluginProtocol",
+    "PluginMapping",
+    "PluginProtocol",
+    "SerializationPluginProtocol",
+    "get_plugin_for_value",
+)
 
+
+if TYPE_CHECKING:
     from starlite.app import Starlite
+    from starlite.openapi.spec import Schema
 
 ModelT = TypeVar("ModelT")
 DataContainerT = TypeVar("DataContainerT", bound=Union[BaseModel, DataclassProtocol, TypedDict])  # type: ignore[valid-type]
 
 
 @runtime_checkable
 class InitPluginProtocol(Protocol):
@@ -127,28 +136,34 @@
             A model instance.
         """
         raise NotImplementedError()
 
     def to_data_container_class(self, model_class: Type[ModelT], **kwargs: Any) -> Type[DataContainerT]:
         """Create a data container class corresponding to the given model class.
 
-        :param model_class: The model class that serves as a basis.
-        :param kwargs: Any kwargs.
-        :return: The generated data container class.
+        Args:
+            model_class: The model class that serves as a basis.
+            **kwargs: Any kwargs.
+
+        Returns:
+            The generated data container class.
         """
         raise NotImplementedError()
 
     def from_data_container_instance(
         self, model_class: Type[ModelT], data_container_instance: DataContainerT
     ) -> ModelT:
         """Create a model instance from the given data container instance.
 
-        :param model_class: The model class to be instantiated.
-        :param data_container_instance: The data container instance.
-        :return: A model instance.
+        Args:
+            model_class: The model class to be instantiated.
+            data_container_instance: The data container instance.
+
+        Returns:
+            A model instance.
         """
         raise NotImplementedError()
 
 
 @runtime_checkable
 class OpenAPISchemaPluginProtocol(Protocol[ModelT]):
     """Plugin to extend the support of OpenAPI schema generation for non-library types."""
@@ -166,16 +181,19 @@
             A typeguard dictating whether the value is supported by the plugin.
         """
         raise NotImplementedError()
 
     def to_openapi_schema(self, model_class: Type[ModelT]) -> "Schema":
         """Given a model class, transform it into an OpenAPI schema class.
 
-        :param model_class: A model class.
-        :return: An :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.schema.Schema>` instance.
+        Args:
+            model_class: A model class.
+
+        Returns:
+            An :class:`OpenAPI <starlite.openapi.spec.schema.Schema>` instance.
         """
         raise NotImplementedError()
 
 
 def get_plugin_for_value(
     value: Any, plugins: List[SerializationPluginProtocol]
 ) -> Optional[SerializationPluginProtocol]:
@@ -217,7 +235,10 @@
 
         Returns:
             Any
         """
         if isinstance(value, (list, tuple)):
             return [self.plugin.from_data_container_instance(self.model_class, item) for item in value]
         return self.plugin.from_data_container_instance(self.model_class, value)
+
+
+PluginProtocol = Union[SerializationPluginProtocol, InitPluginProtocol, OpenAPISchemaPluginProtocol]
```

### Comparing `starlite-2.0.0a1/starlite/plugins/piccolo_orm.py` & `starlite-2.0.0a2/starlite/contrib/piccolo_orm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import TYPE_CHECKING, Any, Dict, Type
 
 from pydantic import BaseModel
-from pydantic_openapi_schema.utils.utils import OpenAPI310PydanticSchema
 
 from starlite.exceptions import MissingDependencyException
-from starlite.plugins.base import (
-    OpenAPISchemaPluginProtocol,
-    SerializationPluginProtocol,
-)
+from starlite.openapi.spec.schema import SchemaDataContainer
+from starlite.plugins import OpenAPISchemaPluginProtocol, SerializationPluginProtocol
+
+__all__ = ("PiccoloORMPlugin",)
 
 try:
-    from piccolo.table import Table, TableMetaclass
-    from piccolo.utils.pydantic import create_pydantic_model
+    import piccolo  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("piccolo orm is not installed") from e
 
+from piccolo.table import Table, TableMetaclass
+from piccolo.utils.pydantic import create_pydantic_model
+
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import Schema
     from typing_extensions import TypeGuard
 
+    from starlite.openapi.spec import Schema
+
 
 class PiccoloORMPlugin(SerializationPluginProtocol[Table, BaseModel], OpenAPISchemaPluginProtocol[Table]):
     """Support (de)serialization and OpenAPI generation for Piccolo ORM types."""
 
     _models_map: Dict[Type[Table], Type["BaseModel"]] = {}
     _data_models_map: Dict[Type[Table], Type["BaseModel"]] = {}
 
@@ -73,11 +75,14 @@
             if meta.name in kwargs:
                 setattr(instance, meta.name, kwargs[meta.name])
         return instance
 
     def to_openapi_schema(self, model_class: Type[Table]) -> "Schema":
         """Given a model class, transform it into an OpenAPI schema class.
 
-        :param model_class: A table class.
-        :return: An :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.schema.Schema>` instance.
+        Args:
+            model_class: A table class.
+
+        Returns:
+            An :class:`OpenAPI <starlite.openapi.spec.schema.Schema>` instance.
         """
-        return OpenAPI310PydanticSchema(schema_class=self.to_data_container_class(model_class=model_class))
+        return SchemaDataContainer(data_container=self.to_data_container_class(model_class=model_class))
```

### Comparing `starlite-2.0.0a1/starlite/plugins/tortoise_orm.py` & `starlite-2.0.0a2/starlite/contrib/tortoise_orm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type
 
 from pydantic import BaseModel
-from pydantic_factories.utils import is_pydantic_model
-from pydantic_openapi_schema.utils.utils import OpenAPI310PydanticSchema
-from tortoise.fields import ReverseRelation
-from tortoise.fields.relational import RelationalField
 
 from starlite.exceptions import MissingDependencyException
-from starlite.plugins.base import (
-    OpenAPISchemaPluginProtocol,
-    SerializationPluginProtocol,
-)
+from starlite.openapi.spec.schema import SchemaDataContainer
+from starlite.plugins import OpenAPISchemaPluginProtocol, SerializationPluginProtocol
+from starlite.utils import is_pydantic_model_class
+
+__all__ = ("TortoiseORMPlugin",)
+
 
 try:
-    from tortoise import Model, ModelMeta  # type: ignore[attr-defined]
-    from tortoise.contrib.pydantic import (  # type: ignore[attr-defined]
-        PydanticModel,
-        pydantic_model_creator,
-    )
+    import tortoise  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("tortoise-orm is not installed") from e
 
+
+from tortoise import Model, ModelMeta  # type: ignore[attr-defined]
+from tortoise.contrib.pydantic import (  # type: ignore[attr-defined]
+    PydanticModel,  # pyright: ignore
+    pydantic_model_creator,  # pyright: ignore
+)
+from tortoise.fields import ReverseRelation
+from tortoise.fields.relational import RelationalField
+
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import Schema
     from typing_extensions import TypeGuard
 
+    from starlite.openapi.spec import Schema
+
 
 class TortoiseORMPlugin(SerializationPluginProtocol[Model, BaseModel], OpenAPISchemaPluginProtocol[Model]):
     """Support (de)serialization and OpenAPI generation for Tortoise ORMtypes."""
 
     _models_map: Dict[Type[Model], Type[PydanticModel]] = {}
     _data_models_map: Dict[Type[Model], Type[PydanticModel]] = {}
 
@@ -41,15 +45,15 @@
         pydantic_model = pydantic_model_creator(model_class, **kwargs)
         for (
             field_name,
             tortoise_model_field,
         ) in model_class._meta.fields_map.items():
             if field_name in pydantic_model.__fields__:
                 if (
-                    is_pydantic_model(pydantic_model.__fields__[field_name].type_)
+                    is_pydantic_model_class(pydantic_model.__fields__[field_name].type_)
                     and "." in pydantic_model.__fields__[field_name].type_.__name__
                 ):
                     sub_model_name = pydantic_model.__fields__[field_name].type_.__name__.split(".")[-2]
                     pydantic_model.__fields__[field_name].type_ = pydantic_model_creator(
                         model_class, name=sub_model_name
                     )
                 if not tortoise_model_field.required:
@@ -94,24 +98,27 @@
         """Given an instance of a pydantic model created using the plugin's ``to_data_container_class``, return an
         instance of the class from which that pydantic model has been created.
 
         This class is passed in as the ``model_class`` kwarg.
         """
         return model_class().update_from_dict(data_container_instance.dict())
 
-    async def to_dict(self, model_instance: Model) -> Dict[str, Any]:  # pylint: disable=invalid-overridden-method
+    async def to_dict(self, model_instance: Model) -> Dict[str, Any]:
         """Given an instance of a model supported by the plugin, return a dictionary of serializable values."""
         pydantic_model_class = self.to_data_container_class(type(model_instance))
         data = await pydantic_model_class.from_tortoise_orm(model_instance)
         return data.dict()
 
     def from_dict(self, model_class: Type[Model], **kwargs: Any) -> Model:  # pragma: no cover
         """Given a class supported by this plugin and a dict of values, create an instance of the class."""
         return model_class().update_from_dict(**kwargs)
 
     def to_openapi_schema(self, model_class: Type[Model]) -> "Schema":
         """Given a model class, transform it into an OpenAPI schema class.
 
-        :param model_class: A table class.
-        :return: An :class:`OpenAPI <pydantic_openapi_schema.v3_1_0.schema.Schema>` instance.
+        Args:
+            model_class: A table class.
+
+        Returns:
+            An :class:`OpenAPI <starlite.openapi.spec.schema.Schema>` instance.
         """
-        return OpenAPI310PydanticSchema(schema_class=self.to_data_container_class(model_class=model_class))
+        return SchemaDataContainer(data_container=self.to_data_container_class(model_class=model_class))
```

### Comparing `starlite-2.0.0a1/starlite/response/base.py` & `starlite-2.0.0a2/starlite/response/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from __future__ import annotations
 
 from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Generic, Literal, Mapping, TypeVar, overload
 
-from starlite.datastructures import Cookie, ETag
+from starlite.datastructures.cookie import Cookie
+from starlite.datastructures.headers import ETag
 from starlite.enums import MediaType, OpenAPIMediaType
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.serialization import (
-    DEFAULT_TYPE_ENCODERS,
-    default_serializer,
-    encode_json,
-    encode_msgpack,
-)
-from starlite.status_codes import (
-    HTTP_200_OK,
-    HTTP_204_NO_CONTENT,
-    HTTP_304_NOT_MODIFIED,
-)
+from starlite.serialization import DEFAULT_TYPE_ENCODERS, default_serializer, encode_json, encode_msgpack
+from starlite.status_codes import HTTP_200_OK, HTTP_204_NO_CONTENT, HTTP_304_NOT_MODIFIED
 from starlite.utils.helpers import get_enum_string_value
 
+__all__ = ("Response",)
+
+
 if TYPE_CHECKING:
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.types import (
         HTTPResponseBodyEvent,
         HTTPResponseStartEvent,
         Receive,
         ResponseCookies,
@@ -71,21 +66,21 @@
         type_encoders: TypeEncodersMap | None = None,
     ) -> None:
         """Initialize the response.
 
         Args:
             content: A value for the response body that will be rendered into bytes string.
             status_code: An HTTP status code.
-            media_type: A value for the response 'Content-Type' header.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
-                Defaults to None.
+            media_type: A value for the response ``Content-Type`` header.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
+                Defaults to ``None``.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <starlite.datastructures.Cookie>` instances to be set under
-                the response 'Set-Cookie' header.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
             encoding: The encoding to be used for the response headers.
             is_head_response: Whether the response should send only the headers ("head" request) or also the content.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
         """
         self.background = background
         self.cookies: list[Cookie] = (
             [Cookie(key=key, value=value) for key, value in cookies.items()]
@@ -157,26 +152,26 @@
         expires: int | None = None,
         path: str = "/",
         domain: str | None = None,
         secure: bool = False,
         httponly: bool = False,
         samesite: Literal["lax", "strict", "none"] = "lax",
     ) -> None:
-        """Set a cookie on the response. If passed a :class:`Cookie <starlite.Cookie>` instance, keyword arguments will be
-        ignored.
+        """Set a cookie on the response. If passed a :class:`Cookie <.datastructures.Cookie>` instance, keyword
+        arguments will be ignored.
 
         Args:
-            key: Key for the cookie or a :class:`Cookie <starlite.Cookie>` instance.
+            key: Key for the cookie or a :class:`Cookie <.datastructures.Cookie>` instance.
             value: Value for the cookie, if none given defaults to empty string.
             max_age: Maximal age of the cookie before its invalidated.
             expires: Expiration date as unix MS timestamp.
-            path: Path fragment that must exist in the request url for the cookie to be valid. Defaults to '/'.
+            path: Path fragment that must exist in the request url for the cookie to be valid. Defaults to ``/``.
             domain: Domain for which the cookie is valid.
             secure: Https is required for the cookie.
-            httponly: Forbids javascript to access the cookie via 'Document.cookie'.
+            httponly: Forbids javascript to access the cookie via ``document.cookie``.
             samesite: Controls whether a cookie is sent with cross-site requests. Defaults to ``lax``.
 
         Returns:
             None.
         """
         if not isinstance(key, Cookie):
             key = Cookie(
@@ -232,15 +227,15 @@
             None.
         """
         cookie = Cookie(key=key, path=path, domain=domain, expires=0, max_age=0)
         self.cookies = [c for c in self.cookies if c != cookie]
         self.cookies.append(cookie)
 
     def render(self, content: Any) -> bytes:
-        """Handle the rendering of content T into a bytes string.
+        """Handle the rendering of content into a bytes string.
 
         Args:
             content: A value for the response body that will be rendered into bytes string.
 
         Returns:
             An encoded bytes string
         """
@@ -259,26 +254,26 @@
             raise ImproperlyConfiguredException("Unable to serialize response content") from e
 
     @property
     def content_length(self) -> int:
         """Content length of the response if applicable.
 
         Returns:
-            The content length of the body (e.g. for use in a "Content-Length" header).
+            The content length of the body (e.g. for use in a ``Content-Length`` header).
             If the response does not have a body, this value is ``None``
         """
         if self.status_allows_body:
             return len(self.body)
         return 0
 
     def encode_headers(self) -> list[tuple[bytes, bytes]]:
         """Encode the response headers as a list of byte tuples.
 
         Notes:
-            - A 'Content-Length' header will be added if appropriate and not provided by the user.
+            - A ``Content-Length`` header will be added if appropriate and not provided by the user.
 
         Returns:
             A list of tuples containing the headers and cookies of the request in a format ready for ASGI transmission.
         """
 
         return list(
             chain(
@@ -317,15 +312,15 @@
             "type": "http.response.start",
             "status": self.status_code,
             "headers": encoded_headers,
         }
 
         await send(event)
 
-    async def send_body(self, send: "Send", receive: "Receive") -> None:  # pylint: disable=unused-argument
+    async def send_body(self, send: "Send", receive: "Receive") -> None:
         """Emit the response body.
 
         Args:
             send: The ASGI send function.
             receive: The ASGI receive function.
 
         Notes:
```

### Comparing `starlite-2.0.0a1/starlite/response/file.py` & `starlite-2.0.0a2/starlite/response/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 from inspect import iscoroutine
 from mimetypes import guess_type
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Coroutine, Literal, cast
 from urllib.parse import quote
 from zlib import adler32
 
 from starlite.constants import ONE_MEGABYTE
-from starlite.enums import MediaType
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.file_system import BaseLocalFileSystem, FileSystemAdapter
 from starlite.response.streaming import StreamingResponse
 from starlite.status_codes import HTTP_200_OK
 
+__all__ = ("FileResponse", "async_file_iterator", "create_etag_for_file")
+
+
 if TYPE_CHECKING:
     from os import PathLike
     from os import stat_result as stat_result_type
 
     from anyio import Path
 
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.datastructures.headers import ETag
-    from starlite.types import (
-        HTTPResponseBodyEvent,
-        PathType,
-        Receive,
-        ResponseCookies,
-        Send,
-    )
+    from starlite.enums import MediaType
+    from starlite.types import HTTPResponseBodyEvent, PathType, Receive, ResponseCookies, Send
     from starlite.types.file_types import FileInfo, FileSystemProtocol
 
 
 async def async_file_iterator(
     file_path: "PathType", chunk_size: int, adapter: "FileSystemAdapter"
 ) -> AsyncGenerator[bytes, None]:
     """Return an async that asynchronously reads a file and yields its chunks.
@@ -95,39 +92,41 @@
         media_type: Literal[MediaType.TEXT] | str | None = None,
         stat_result: stat_result_type | None = None,
         status_code: int = HTTP_200_OK,
     ) -> None:
         """Initialize ``FileResponse``
 
         Notes:
-            - This class extends the :class:`StreamingResponse <starlite.response.StreamingResponse>` class.
+            - This class extends the :class:`StreamingResponse <.response.StreamingResponse>` class.
 
         Args:
             path: A file path in one of the supported formats.
             status_code: An HTTP status code.
-            media_type: A value for the response 'Content-Type' header. If not provided, the value will be either
+            media_type: A value for the response ``Content-Type`` header. If not provided, the value will be either
                 derived from the filename if provided and supported by the stdlib, or will default to
-                'application/octet-stream'.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+                ``application/octet-stream``.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to None.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <starlite.datastructures.Cookie>` instances to be set under the response 'Set-Cookie' header.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
             encoding: The encoding to be used for the response headers.
             is_head_response: Whether the response should send only the headers ("head" request) or also the content.
             filename: An optional filename to set in the header.
-            stat_result: An optional result of calling 'os.stat'. If not provided, this will be done by the response
-                constructor.
+            stat_result: An optional result of calling :func:os.stat:. If not provided, this will be done by the
+                response constructor.
             chunk_size: The chunk sizes to use when streaming the file. Defaults to 1MB.
-            content_disposition_type: The type of the 'Content-Disposition'. Either ``inline`` or ``attachment``.
-            etag: An optional :class:`ETag <starlite.datastructures.ETag>` instance.
-                If not provided, an etag will be automatically generated.
-            file_system: An implementation of the :class:`FileSystemProtocol <starlite.types.FileSystemProtocol>`. If provided
+            content_disposition_type: The type of the ``Content-Disposition``. Either ``inline`` or ``attachment``.
+            etag: An optional :class:`ETag <.datastructures.ETag>` instance. If not provided, an etag will be
+                generated.
+            file_system: An implementation of the :class:`FileSystemProtocol <.types.FileSystemProtocol>`. If provided
                 it will be used to load the file.
-            file_info: The output of calling ``file_system.info(..)``, equivalent to providing a ``stat_result``.
+            file_info: The output of calling :meth:`file_system.info <types.FileSystemProtocol.info>`, equivalent to
+                providing an :class:`os.stat_result`.
         """
         if not media_type:
             mimetype, _ = guess_type(filename) if filename else (None, None)
             media_type = mimetype or "application/octet-stream"
 
         self.chunk_size = chunk_size
         self.content_disposition_type = content_disposition_type
@@ -155,28 +154,29 @@
             self.file_info = self.adapter.info(self.file_path)
 
     @property
     def content_disposition(self) -> str:
         """Content disposition.
 
         Returns:
-            A value for the 'Content-Disposition' header.
+            A value for the ``Content-Disposition`` header.
         """
         quoted_filename = quote(self.filename)
         is_utf8 = quoted_filename == self.filename
         if is_utf8:
             return f'{self.content_disposition_type}; filename="{self.filename}"'
         return f"{self.content_disposition_type}; filename*=utf-8''{quoted_filename}"
 
     @property
     def content_length(self) -> int:
         """Content length of the response if applicable.
 
         Returns:
-            Returns the value of 'self.stat_result.st_size' to populate the 'Content-Length' header.
+            Returns the value of :attr:`stat_result.st_size <os.stat_result.st_size>` to populate the ``Content-Length``
+                header.
         """
         if isinstance(self.file_info, dict):
             return self.file_info["size"]
         return 0
 
     async def send_body(self, send: "Send", receive: "Receive") -> None:
         """Emit a stream of events correlating with the response body.
```

### Comparing `starlite-2.0.0a1/starlite/response/redirect.py` & `starlite-2.0.0a2/starlite/response/redirect.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from starlite.constants import REDIRECT_STATUS_CODES
 from starlite.enums import MediaType
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.response.base import Response
 from starlite.status_codes import HTTP_307_TEMPORARY_REDIRECT
 
+__all__ = ("RedirectResponse",)
+
+
 if TYPE_CHECKING:
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.types import ResponseCookies
 
 
 class RedirectResponse(Response[Any]):
     """A redirect response."""
@@ -28,21 +31,23 @@
         encoding: str = "utf-8",
     ) -> None:
         """Initialize the response.
 
         Args:
             url: A url to redirect to.
             status_code: An HTTP status code. The status code should be one of 301, 302, 303, 307 or 308,
-                otherwise an exception will be raised. .
+                otherwise an exception will be raised.
+            background: A background task or tasks to be run after the response is sent.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <starlite.datastructures.Cookie>` instances to be set under the response 'Set-Cookie' header.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
             encoding: The encoding to be used for the response headers.
 
         Raises:
-            :class:`ImproperlyConfiguredException <starlite.exceptions.ImproperlyConfiguredException>`: If status code is not a redirect status code.
+            ImproperlyConfiguredException: If status code is not a redirect status code.
         """
         if status_code not in REDIRECT_STATUS_CODES:
             raise ImproperlyConfiguredException(
                 f"{status_code} is not a valid for this response. "
                 f"Redirect responses should have one of "
                 f"the following status codes: {', '.join([str(s) for s in REDIRECT_STATUS_CODES])}"
             )
```

### Comparing `starlite-2.0.0a1/starlite/response/streaming.py` & `starlite-2.0.0a2/starlite/response/streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 
 from starlite.enums import MediaType
 from starlite.response.base import Response
 from starlite.status_codes import HTTP_200_OK
 from starlite.types.composite_types import StreamType
 from starlite.utils.sync import AsyncIteratorWrapper
 
+__all__ = ("StreamingResponse",)
+
+
 if TYPE_CHECKING:
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.enums import OpenAPIMediaType
     from starlite.types import HTTPResponseBodyEvent, Receive, ResponseCookies, Send
 
 
 class StreamingResponse(Response[StreamType[Union[str, bytes]]]):
-    """An HTTP response that streams the response data as a series of ASGI 'http.response.body' events."""
+    """An HTTP response that streams the response data as a series of ASGI ``http.response.body`` events."""
 
     __slots__ = ("iterator",)
 
     def __init__(
         self,
         content: StreamType[str | bytes],
         *,
@@ -42,20 +45,21 @@
         is_head_response: bool = False,
     ):
         """Initialize the response.
 
         Args:
             content: A sync or async iterator or iterable.
             status_code: An HTTP status code.
-            media_type: A value for the response 'Content-Type' header.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+            media_type: A value for the response ``Content-Type`` header.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to None.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <starlite.datastructures.Cookie>` instances to be set under the response 'Set-Cookie' header.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
             encoding: The encoding to be used for the response headers.
             is_head_response: Whether the response should send only the headers ("head" request) or also the content.
         """
         super().__init__(
             background=background,
             content=b"",  # type: ignore[arg-type]
             cookies=cookies,
```

### Comparing `starlite-2.0.0a1/starlite/response/template.py` & `starlite-2.0.0a2/starlite/response/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Any
 
 from starlite.enums import MediaType
 from starlite.response.base import Response
 from starlite.status_codes import HTTP_200_OK
 
+__all__ = ("TemplateResponse",)
+
+
 if TYPE_CHECKING:
     from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.template import TemplateEngineProtocol
     from starlite.types import ResponseCookies
 
 
 class TemplateResponse(Response[bytes]):
@@ -29,27 +32,27 @@
         cookies: ResponseCookies | None = None,
         encoding: str = "utf-8",
         media_type: MediaType | str = MediaType.HTML,
     ) -> None:
         """Handle the rendering of a given template into a bytes string.
 
         Args:
-            template_name: Path-like name for the template to be rendered, e.g. "index.html".
+            template_name: Path-like name for the template to be rendered, e.g. ``index.html``.
             template_engine: The template engine class to use to render the response.
             status_code: A value for the response HTTP status code.
             context: A dictionary of key/value pairs to be passed to the temple engine's render method.
-            background: A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or
-                :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
-                Defaults to None.
+            background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+                :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
+                Defaults to ``None``.
             headers: A string keyed dictionary of response headers. Header keys are insensitive.
-            cookies: A list of :class:`Cookie <starlite.datastructures.Cookie>` instances to be set under the response
-                'Set-Cookie' header.
+            cookies: A list of :class:`Cookie <.datastructures.Cookie>` instances to be set under the response
+                ``Set-Cookie`` header.
             encoding: Content encoding
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum. If not set, try to infer
-                the media type based on the template name. If this fails, fall back to `text/plain`.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum. If not set, try to infer
+                the media type based on the template name. If this fails, fall back to ``text/plain``.
         """
         if media_type == MediaType.JSON:  # we assume this is the default
             suffixes = PurePath(template_name).suffixes
             for suffix in suffixes:
                 if _type := guess_type("name" + suffix)[0]:
                     media_type = _type
                     break
```

### Comparing `starlite-2.0.0a1/starlite/response_containers.py` & `starlite-2.0.0a2/starlite/response_containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterable,
@@ -13,53 +12,53 @@
     Generic,
     Iterable,
     Iterator,
     Literal,
     TypeVar,
 )
 
-from starlite.background_tasks import BackgroundTask, BackgroundTasks
 from starlite.constants import DEFAULT_CHUNK_SIZE
-from starlite.datastructures.cookie import Cookie
-from starlite.datastructures.headers import ETag
-from starlite.enums import MediaType
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.file_system import BaseLocalFileSystem
-from starlite.response import (
-    FileResponse,
-    RedirectResponse,
-    StreamingResponse,
-    TemplateResponse,
-)
-from starlite.types import FileInfo
-from starlite.types.composite_types import PathType, StreamType
+from starlite.response import FileResponse, RedirectResponse, StreamingResponse, TemplateResponse
+
+__all__ = ("File", "Redirect", "ResponseContainer", "Stream", "Template")
+
 
 if TYPE_CHECKING:
+    import os
+
     from starlite.app import Starlite
+    from starlite.background_tasks import BackgroundTask, BackgroundTasks
     from starlite.connection import Request
+    from starlite.datastructures.cookie import Cookie
+    from starlite.datastructures.headers import ETag
+    from starlite.enums import MediaType
+    from starlite.types import FileInfo
+    from starlite.types.composite_types import PathType, StreamType
 
 R_co = TypeVar("R_co", covariant=True)
 
 
 class ResponseContainer(ABC, Generic[R_co]):
     """Generic response container."""
 
     background: BackgroundTask | BackgroundTasks | None
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or.
 
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
     Defaults to None.
     """
     headers: dict[str, Any]
     """A string/string dictionary of response headers.
 
     Header keys are insensitive. Defaults to None.
     """
     cookies: list[Cookie]
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
+    """A list of Cookie instances to be set under the response ``Set-Cookie`` header.
 
     Defaults to None.
     """
     media_type: MediaType | str | None
     """If defined, overrides the media type configured in the route decorator."""
     encoding: str
     """The encoding to be used for the response headers."""
@@ -73,44 +72,44 @@
         app: Starlite,
         request: Request,
     ) -> R_co:  # pragma: no cover
         """Abstract method that should be implemented by subclasses.
 
         Args:
             headers: A dictionary of headers.
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum.
             status_code: A response status code.
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response Object
         """
         raise NotImplementedError("not implemented")
 
 
 @dataclass
 class File(ResponseContainer[FileResponse]):
     """Container type for returning File responses."""
 
     path: PathType
     """Path to the file to send."""
     background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or.
 
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
     Defaults to None.
     """
     headers: dict[str, Any] = field(default_factory=dict)
     """A string/string dictionary of response headers.
 
     Header keys are insensitive. Defaults to None.
     """
     cookies: list[Cookie] = field(default_factory=list)
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
+    """A list of Cookie instances to be set under the response ``Set-Cookie`` header.
 
     Defaults to None.
     """
     media_type: MediaType | str | None = field(default=None)
     """If defined, overrides the media type configured in the route decorator."""
     encoding: str = field(default="utf-8")
     """The encoding to be used for the response headers."""
@@ -122,32 +121,32 @@
     If not provided, this will be done by the response constructor.
     """
     chunk_size: int = field(default=DEFAULT_CHUNK_SIZE)
     """The size of chunks to use when streaming the file."""
     content_disposition_type: Literal["attachment", "inline"] = field(default="attachment")
     """The type of the 'Content-Disposition'.
 
-    Either 'inline' or 'attachment'.
+    Either ``inline`` or ``attachment``.
     """
     etag: ETag | None = field(default=None)
-    """An optional :class:`ETag <starlite.datastructures.ETag>` instance.
+    """An optional :class:`ETag <.datastructures.ETag>` instance.
 
     If not provided, an etag will be automatically generated.
     """
     file_system: Any = field(default_factory=BaseLocalFileSystem)
     """The file_system spec to use loading the file.
 
     Notes:
-        - A file_system is a class that adheres to the
-            :class:`FileSystemProtocol <starlite.types.FileSystemProtocol>`.
+        - A file_system is a class that adheres to the :class:`FileSystemProtocol <.types.FileSystemProtocol>`.
         - You can use any of the file systems exported from the
-            [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) library for this purpose.
+          `fsspec <https://filesystem-spec.readthedocs.io/en/latest/>`_ library for this purpose.
     """
     file_info: FileInfo | None = field(default=None)
-    """The output of calling `file_system.info(..)`, equivalent to providing a ``stat_result``."""
+    """The output of calling :meth:`file_system.info <.types.FileSystemProtocol.info>`, equivalent to providing a
+    :class`os.stat_result`."""
 
     def __post_init__(self) -> None:
         if not (
             callable(getattr(self.file_system, "info", None)) and callable(getattr(self.file_system, "open", None))
         ):
             raise ImproperlyConfiguredException("file_system must adhere to the FileSystemProtocol type")
 
@@ -162,21 +161,21 @@
         app: Starlite,
         request: Request,
     ) -> FileResponse:
         """Create a FileResponse instance.
 
         Args:
             headers: A dictionary of headers.
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum.
             status_code: A response status code.
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
-            A FileResponse instance
+            A :class:`FileResponse <.response.FileResponse>` instance
         """
         return FileResponse(
             background=self.background,
             chunk_size=self.chunk_size,
             content_disposition_type=self.content_disposition_type,
             encoding=self.encoding,
             etag=self.etag,
@@ -194,26 +193,25 @@
 @dataclass
 class Redirect(ResponseContainer[RedirectResponse]):
     """Container type for returning Redirect responses."""
 
     path: str
     """Redirection path."""
     background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
-
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
     Defaults to None.
     """
     headers: dict[str, Any] = field(default_factory=dict)
     """A string/string dictionary of response headers.
 
     Header keys are insensitive. Defaults to None.
     """
     cookies: list[Cookie] = field(default_factory=list)
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
+    """A list of Cookie instances to be set under the response ``Set-Cookie`` header.
 
     Defaults to None.
     """
     media_type: MediaType | str | None = field(default=None)
     """If defined, overrides the media type configured in the route decorator."""
     encoding: str = field(default="utf-8")
     """The encoding to be used for the response headers."""
@@ -228,21 +226,21 @@
         app: Starlite,
         request: Request,
     ) -> RedirectResponse:
         """Create a RedirectResponse instance.
 
         Args:
             headers: A dictionary of headers.
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum.
             status_code: A response status code.
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
-            A RedirectResponse instance
+            A :class:`RedirectResponse <.response.RedirectResponse>` instance
         """
         return RedirectResponse(
             background=self.background,
             encoding=self.encoding,
             headers=headers,
             status_code=status_code,
             url=self.path,
@@ -252,40 +250,37 @@
 @dataclass
 class Stream(ResponseContainer[StreamingResponse]):
     """Container type for returning Stream responses."""
 
     iterator: StreamType[str | bytes] | Callable[[], StreamType[str | bytes]]
     """Iterator, Iterable,Generator or async Iterator, Iterable or Generator returning chunks to stream."""
     background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or.
 
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
     Defaults to None.
     """
     headers: dict[str, Any] = field(default_factory=dict)
     """A string/string dictionary of response headers.
 
     Header keys are insensitive. Defaults to None.
     """
     cookies: list[Cookie] = field(default_factory=list)
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
+    """A list of Cookie instances to be set under the response ``Set-Cookie`` header.
 
     Defaults to None.
     """
     media_type: MediaType | str | None = field(default=None)
     """If defined, overrides the media type configured in the route decorator."""
     encoding: str = field(default="utf-8")
     """The encoding to be used for the response headers."""
 
     def __post_init__(self) -> None:
         """Set the iterator value by ensuring that the return value is iterable.
 
-        Args:
-            value: An iterable or callable returning an iterable.
-
         Returns:
             A sync or async iterable.
         """
 
         if not isinstance(self.iterator, (Iterable, Iterator, AsyncIterable, AsyncIterator)) and callable(
             self.iterator
         ):
@@ -304,21 +299,21 @@
         app: Starlite,
         request: Request,
     ) -> StreamingResponse:
         """Create a StreamingResponse instance.
 
         Args:
             headers: A dictionary of headers.
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum.
             status_code: A response status code.
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
-            A StreamingResponse instance
+            A :class:`StreamingResponse <.response.StreamingResponse>` instance
         """
 
         return StreamingResponse(
             background=self.background,
             content=self.iterator if isinstance(self.iterator, (Iterable, AsyncIterable)) else self.iterator(),
             encoding=self.encoding,
             headers=headers,
@@ -335,29 +330,22 @@
     """Path-like name for the template to be rendered, e.g. "index.html"."""
     context: dict[str, Any] = field(default_factory=dict)
     """A dictionary of key/value pairs to be passed to the temple engine's render method.
 
     Defaults to None.
     """
     background: BackgroundTask | BackgroundTasks | None = field(default=None)
-    """A :class:`BackgroundTask <starlite.datastructures.BackgroundTask>` instance or.
-
-    :class:`BackgroundTasks <starlite.datastructures.BackgroundTasks>` to execute after the response is finished.
-    Defaults to None.
+    """A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
+    :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished. Defaults to
+    None.
     """
     headers: dict[str, Any] = field(default_factory=dict)
-    """A string/string dictionary of response headers.
-
-    Header keys are insensitive. Defaults to None.
-    """
+    """A string/string dictionary of response headers. Header keys are insensitive. Defaults to None."""
     cookies: list[Cookie] = field(default_factory=list)
-    """A list of Cookie instances to be set under the response 'Set-Cookie' header.
-
-    Defaults to None.
-    """
+    """A list of Cookie instances to be set under the response ``Set-Cookie`` header. Defaults to None. """
     media_type: MediaType | str | None = field(default=None)
     """If defined, overrides the media type configured in the route decorator."""
     encoding: str = field(default="utf-8")
     """The encoding to be used for the response headers."""
 
     def to_response(
         self,
@@ -367,25 +355,24 @@
         app: Starlite,
         request: Request,
     ) -> TemplateResponse:
         """Create a TemplateResponse instance.
 
         Args:
             headers: A dictionary of headers.
-            media_type: A string or member of the :class:`MediaType <starlite.enums.MediaType>` enum.
+            media_type: A string or member of the :class:`MediaType <.enums.MediaType>` enum.
             status_code: A response status code.
-            app: The :class:`Starlite <starlite.app.Starlite>` application instance.
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            app: The :class:`Starlite <.app.Starlite>` application instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Raises:
-            :class:`ImproperlyConfiguredException <starlite.exceptions.ImproperlyConfiguredException>`: if app.template_engine
-                is not configured.
+            ImproperlyConfiguredException: If ``Starlite.template_engine`` is not configured.
 
         Returns:
-            A TemplateResponse instance
+            A :class:`TemplateResponse <.response.TemplateResponse>` instance
         """
         if not app.template_engine:
             raise ImproperlyConfiguredException("Template engine is not configured")
 
         return TemplateResponse(
             background=self.background,
             context=self.create_template_context(request=request),
@@ -397,15 +384,15 @@
             media_type=media_type,
         )
 
     def create_template_context(self, request: Request) -> dict[str, Any]:
         """Create a context object for the template.
 
         Args:
-            request: A :class:`Request <starlite.connection.request.Request>` instance.
+            request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A dictionary holding the template context
         """
         csrf_token = request.scope.get("_csrf_token", "")
         return {
             **self.context,
```

### Comparing `starlite-2.0.0a1/starlite/router.py` & `starlite-2.0.0a2/starlite/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from copy import copy
 from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, Sequence, cast
 
+from starlite._layers.utils import narrow_response_cookies, narrow_response_headers
 from starlite.controller import Controller
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.handlers.asgi_handlers import ASGIRouteHandler
 from starlite.handlers.base import BaseRouteHandler
 from starlite.handlers.http_handlers import HTTPRouteHandler
-from starlite.handlers.utils import narrow_response_cookies, narrow_response_headers
 from starlite.handlers.websocket_handlers import WebsocketRouteHandler
 from starlite.routes import ASGIRoute, HTTPRoute, WebSocketRoute
-from starlite.types import (
-    AfterRequestHookHandler,
-    AfterResponseHookHandler,
-    BeforeRequestHookHandler,
-    ControllerRouterHandler,
-    ExceptionHandlersMap,
-    Guard,
-    Middleware,
-    ParametersMap,
-    ResponseCookies,
-    ResponseType,
-    RouteHandlerMapItem,
-    RouteHandlerType,
-    TypeEncodersMap,
-)
-from starlite.utils import (
-    find_index,
-    is_class_and_subclass,
-    join_paths,
-    normalize_path,
-    unique,
-)
+from starlite.utils import find_index, is_class_and_subclass, join_paths, normalize_path, unique
 from starlite.utils.sync import AsyncCallable
 
-if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import SecurityRequirement
+__all__ = ("Router",)
+
 
+if TYPE_CHECKING:
     from starlite.datastructures import CacheControlHeader, ETag
     from starlite.di import Provide
+    from starlite.openapi.spec import SecurityRequirement
     from starlite.routes import BaseRoute
+    from starlite.types import (
+        AfterRequestHookHandler,
+        AfterResponseHookHandler,
+        BeforeRequestHookHandler,
+        ControllerRouterHandler,
+        ExceptionHandlersMap,
+        Guard,
+        Middleware,
+        ParametersMap,
+        ResponseCookies,
+        ResponseType,
+        RouteHandlerMapItem,
+        RouteHandlerType,
+        TypeEncodersMap,
+    )
     from starlite.types.composite_types import ResponseHeaders
 
 
 class Router:
     """The Starlite Router class.
 
     A Router instance is used to group controller, routers and route handler functions under a shared path fragment
@@ -67,14 +63,15 @@
         "path",
         "registered_route_handler_ids",
         "response_class",
         "response_cookies",
         "response_headers",
         "routes",
         "security",
+        "signature_namespace",
         "tags",
         "type_encoders",
     )
 
     def __init__(
         self,
         path: str,
@@ -91,55 +88,58 @@
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         route_handlers: Sequence[ControllerRouterHandler],
         security: Sequence[SecurityRequirement] | None = None,
+        signature_namespace: Mapping[str, Any] | None = None,
         tags: Sequence[str] | None = None,
         type_encoders: TypeEncodersMap | None = None,
     ) -> None:
         """Initialize a ``Router``.
 
         Args:
-            after_request: A sync or async function executed before a :class:`Request <starlite.connection.Request>` is
-                passed to any route handler. If this function returns a value, the request will not reach the route
-                handler, and instead this value will be used.
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
+                to any route handler. If this function returns a value, the request will not reach the route handler,
+                and instead this value will be used.
             after_response: A sync or async function called after the response has been awaited. It receives the
-                :class:`Request <starlite.connection.Request>` object and should not return any values.
+                :class:`Request <.connection.Request>` object and should not return any values.
             before_request: A sync or async function called immediately before calling the route handler. Receives
                 the :class:`starlite.connection.Request` instance and any non-``None`` return value is used for the
                 response, bypassing the route handler.
             cache_control: A ``cache-control`` header of type
-                :class:`CacheControlHeader <starlite.datastructures.CacheControlHeader>` to add to route handlers of
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to route handlers of
                 this router. Can be overridden by route handlers.
-            dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-            etag: An ``etag`` header of type :class:`ETag <datastructures.ETag>` to add to route handlers of this app.
+            dependencies: A string keyed mapping of dependency :class:`Provide <.di.Provide>` instances.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <starlite.types.Guard>`
-                or wherever you have access to :class:`Request <starlite.connection.request.Request>` or
-                :class:`ASGI Scope <starlite.types.Scope>`.
-            parameters: A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all
-                application paths.
+            guards: A sequence of :data:`Guard <.types.Guard>` callables.
+            middleware: A sequence of :data:`Middleware <.types.Middleware>`.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :data:`Guards <.types.Guard>` or
+                wherever you have access to :class:`Request <.connection.Request>` or
+                :data:`ASGI Scope <.types.Scope>`.
+            parameters: A mapping of :func:`Parameter <.params.Parameter>` definitions available to all application
+                paths.
             path: A path fragment that is prefixed to all route handlers, controllers and other routers associated
                 with the router instance.
-            response_class: A custom subclass of [starlite.response.Response] to be used as the default for all route
-                handlers, controllers and other routers associated with the router instance.
-            response_cookies: A sequence of [Cookie](starlite.datastructures.Cookie] instances.
-            response_headers: A string keyed mapping of :class:`ResponseHeader <starlite.datastructures.ResponseHeader>`
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the default for
+                all route handlers, controllers and other routers associated with the router instance.
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
                 instances.
             route_handlers: A required sequence of route handlers, which can include instances of
-                :class:`Router <starlite.router.Router>`, subclasses of
-                :class:`Controller <starlite.controller.Controller>` or any function decorated by the route handler
-                decorators.
+                :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
+                function decorated by the route handler decorators.
             security: A sequence of dicts that will be added to the schema of all route handlers in the application.
-                See :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` for details.
-            tags: A sequence of string tags that will be appended to the schema of all route handlers under the application.
+                See :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
+                for details.
+            signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+            tags: A sequence of string tags that will be appended to the schema of all route handlers under the
+                application.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
         """
 
         self.after_request = AsyncCallable(after_request) if after_request else None  # type: ignore[arg-type]
         self.after_response = AsyncCallable(after_response) if after_response else None
         self.before_request = AsyncCallable(before_request) if before_request else None
         self.cache_control = cache_control
@@ -153,28 +153,29 @@
         self.parameters = dict(parameters or {})
         self.path = normalize_path(path)
         self.response_class = response_class
         self.response_cookies = narrow_response_cookies(response_cookies)
         self.response_headers = narrow_response_headers(response_headers)
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.security = list(security or [])
+        self.signature_namespace = signature_namespace or {}
         self.tags = list(tags or [])
         self.registered_route_handler_ids: set[int] = set()
         self.type_encoders = dict(type_encoders) if type_encoders is not None else None
 
         for route_handler in route_handlers or []:
             self.register(value=route_handler)
 
     def register(self, value: ControllerRouterHandler) -> list[BaseRoute]:
         """Register a Controller, Route instance or RouteHandler on the router.
 
         Args:
-            value: a subclass or instance of Controller, an instance of ``Router`` or a function/method that has been
-                decorated by any of the routing decorators, e.g. :class:`get <starlite.handlers.http_handlers.get>`,
-                :class:`post <starlite.handlers.http_handlers.post>`.
+            value: a subclass or instance of Controller, an instance of :class:`Router` or a function/method that has
+                been decorated by any of the routing decorators, e.g. :class:`get <.handlers.get>`,
+                :class:`post <.handlers.post>`.
 
         Returns:
             Collection of handlers added to the router.
         """
         validated_value = self._validate_registration_value(value)
 
         routes: list[BaseRoute] = []
@@ -188,17 +189,15 @@
                     [
                         handler
                         for handler in self.route_handler_method_map.get(path, {}).values()
                         if isinstance(handler, HTTPRouteHandler)
                     ]
                 ):
                     http_handlers.extend(existing_handlers)
-                    existing_route_index = find_index(
-                        self.routes, lambda x: x.path == path  # pylint: disable=cell-var-from-loop # noqa: B023
-                    )
+                    existing_route_index = find_index(self.routes, lambda x: x.path == path)  # noqa: B023
 
                     if existing_route_index == -1:  # pragma: no cover
                         raise ImproperlyConfiguredException("unable to find_index existing route index")
 
                     route: WebSocketRoute | ASGIRoute | HTTPRoute = HTTPRoute(
                         path=path,
                         route_handlers=http_handlers,
```

### Comparing `starlite-2.0.0a1/starlite/routes/asgi.py` & `starlite-2.0.0a2/starlite/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/routes/base.py` & `starlite-2.0.0a2/starlite/routes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from pydantic.datetime_parse import (
     parse_date,
     parse_datetime,
     parse_duration,
     parse_time,
 )
 
+from starlite._kwargs import KwargsModel
+from starlite._signature import get_signature_model
 from starlite.exceptions import ImproperlyConfiguredException
-from starlite.kwargs import KwargsModel
-from starlite.signature import get_signature_model
 from starlite.types.internal_types import PathParameterDefinition
 from starlite.utils import join_paths, normalize_path
 
 if TYPE_CHECKING:
     from starlite.enums import ScopeType
     from starlite.handlers.base import BaseRouteHandler
     from starlite.types import Method, Receive, Scope, Send
```

### Comparing `starlite-2.0.0a1/starlite/routes/http.py` & `starlite-2.0.0a2/starlite/routes/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 from __future__ import annotations
 
 import pickle
 from itertools import chain
 from typing import TYPE_CHECKING, Any, cast
 
-from starlite.connection import Request
 from starlite.constants import DEFAULT_ALLOWED_CORS_HEADERS
 from starlite.datastructures.headers import Headers
 from starlite.datastructures.upload_file import UploadFile
 from starlite.enums import HttpMethod, MediaType, ScopeType
-from starlite.exceptions import (
-    ClientException,
-    ImproperlyConfiguredException,
-    SerializationException,
-)
+from starlite.exceptions import ClientException, ImproperlyConfiguredException, SerializationException
 from starlite.handlers.http_handlers import HTTPRouteHandler
 from starlite.response import Response
 from starlite.routes.base import BaseRoute
 from starlite.status_codes import HTTP_204_NO_CONTENT, HTTP_400_BAD_REQUEST
 
 if TYPE_CHECKING:
-    from starlite.kwargs import KwargsModel
-    from starlite.kwargs.cleanup import DependencyCleanupGroup
+    from starlite._kwargs import KwargsModel
+    from starlite._kwargs.cleanup import DependencyCleanupGroup
+    from starlite.connection import Request
     from starlite.types import ASGIApp, HTTPScope, Method, Receive, Scope, Send
 
 
 class HTTPRoute(BaseRoute):
     """An HTTP route, capable of handling multiple ``HTTPRouteHandler``s."""
 
     __slots__ = (
@@ -159,23 +155,19 @@
             response_data = await before_request_handler(request)
 
         if not response_data:
             response_data, cleanup_group = await self._get_response_data(
                 route_handler=route_handler, parameter_model=parameter_model, request=request
             )
 
-        response: ASGIApp = (
-            response_data  # type: ignore[assignment]
-            if isinstance(response_data, Response)
-            else await route_handler.to_response(
-                app=scope["app"],
-                data=response_data,
-                plugins=request.app.serialization_plugins,
-                request=request,
-            )
+        response: ASGIApp = await route_handler.to_response(
+            app=scope["app"],
+            data=response_data,
+            plugins=request.app.serialization_plugins,
+            request=request,
         )
 
         if cleanup_group:
             await cleanup_group.cleanup()
 
         return response
 
@@ -218,61 +210,65 @@
                 data = route_handler.fn.value(**parsed_kwargs)
             else:
                 data = await route_handler.fn.value(**parsed_kwargs)
 
         return data, cleanup_group
 
     @staticmethod
-    async def _get_cached_response(request: Request, route_handler: "HTTPRouteHandler") -> "ASGIApp" | None:
+    async def _get_cached_response(request: Request, route_handler: HTTPRouteHandler) -> ASGIApp | None:
         """Retrieve and un-pickle the cached response, if existing.
 
         Args:
             request: The :class:`Request <starlite.connection.Request>` instance
             route_handler: The :class:`HTTPRouteHandler <starlite.handlers.http_handlers.HTTPRouteHandler>` instance
 
         Returns:
             A cached response instance, if existing.
         """
 
-        cache = request.app.cache
-        cache_key = cache.build_cache_key(request=request, cache_key_builder=route_handler.cache_key_builder)
-        cached_response = await cache.get(key=cache_key)
+        cache_config = request.app.response_cache_config
+        cache_key = (route_handler.cache_key_builder or cache_config.key_builder)(request)
+        store = cache_config.get_store_from_app(request.app)
+
+        cached_response = await store.get(key=cache_key)
 
         if cached_response:
-            return cast("ASGIApp", pickle.loads(cached_response))  # nosec # noqa: SCS113
+            return cast("ASGIApp", pickle.loads(cached_response))  # nosec
 
         return None
 
     @staticmethod
     async def _set_cached_response(
-        response: "Response" | "ASGIApp", request: Request, route_handler: "HTTPRouteHandler"
+        response: Response | ASGIApp, request: Request, route_handler: HTTPRouteHandler
     ) -> None:
         """Pickles and caches a response object."""
-        cache = request.app.cache
-        cache_key = cache.build_cache_key(request, route_handler.cache_key_builder)
+        cache_config = request.app.response_cache_config
+        cache_key = (route_handler.cache_key_builder or cache_config.key_builder)(request)
 
-        await cache.set(
-            key=cache_key,
-            value=pickle.dumps(response, pickle.HIGHEST_PROTOCOL),
-            expiration=route_handler.cache if isinstance(route_handler.cache, int) else None,
-        )
+        expires_in: int | None = None
+        if route_handler.cache is True:
+            expires_in = cache_config.default_expiration
+        elif route_handler.cache is not False and isinstance(route_handler.cache, int):
+            expires_in = route_handler.cache
 
-    def create_options_handler(self, path: str) -> HTTPRouteHandler:
-        """
+        store = cache_config.get_store_from_app(request.app)
 
-        Args:
+        await store.set(key=cache_key, value=pickle.dumps(response, pickle.HIGHEST_PROTOCOL), expires_in=expires_in)
+
+    def create_options_handler(self, path: str) -> HTTPRouteHandler:
+        """Args:
             path: The route path
 
         Returns:
             An HTTP route handler for OPTIONS requests.
         """
 
         def options_handler(scope: Scope) -> Response:
-            """
-            Handler function for OPTIONS requests.
+            """Handler function for OPTIONS requests.
+
             Args:
                 scope: The ASGI Scope.
 
             Returns:
                 Response
             """
             cors_config = scope["app"].cors_config
```

### Comparing `starlite-2.0.0a1/starlite/routes/websocket.py` & `starlite-2.0.0a2/starlite/routes/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import TYPE_CHECKING, Any
 
 from starlite.enums import ScopeType
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.routes.base import BaseRoute
 
 if TYPE_CHECKING:
+    from starlite._kwargs import KwargsModel
+    from starlite._kwargs.cleanup import DependencyCleanupGroup
     from starlite.connection import WebSocket
     from starlite.handlers.websocket_handlers import WebsocketRouteHandler
-    from starlite.kwargs import KwargsModel
-    from starlite.kwargs.cleanup import DependencyCleanupGroup
     from starlite.types import Receive, Send, WebSocketScope
 
 
 class WebSocketRoute(BaseRoute):
     """A websocket route, handling a single ``WebsocketRouteHandler``"""
 
     __slots__ = (
```

### Comparing `starlite-2.0.0a1/starlite/security/base.py` & `starlite-2.0.0a2/starlite/security/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import copy
 from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, TypeVar
 
 from starlite import Response
-from starlite.connection import ASGIConnection
-from starlite.di import Provide
-from starlite.middleware.authentication import AbstractAuthenticationMiddleware
-from starlite.types import (
-    ControllerRouterHandler,
-    Guard,
-    Scopes,
-    SyncOrAsyncUnion,
-    TypeEncodersMap,
-)
 from starlite.utils.sync import AsyncCallable
 
 if TYPE_CHECKING:
-    from pydantic_openapi_schema.v3_1_0 import Components, SecurityRequirement
-
     from starlite.config.app import AppConfig
+    from starlite.connection import ASGIConnection
+    from starlite.di import Provide
     from starlite.enums import MediaType, OpenAPIMediaType
+    from starlite.middleware.authentication import AbstractAuthenticationMiddleware
     from starlite.middleware.base import DefineMiddleware
-    from starlite.types import ResponseCookies
+    from starlite.openapi.spec import Components, SecurityRequirement
+    from starlite.types import (
+        ControllerRouterHandler,
+        Guard,
+        ResponseCookies,
+        Scopes,
+        SyncOrAsyncUnion,
+        TypeEncodersMap,
+    )
 
+__all__ = ("AbstractSecurityConfig",)
 
 UserType = TypeVar("UserType")
 AuthType = TypeVar("AuthType")
 
 
 class AbstractSecurityConfig(ABC, Generic[UserType, AuthType]):
     """A base class for Security Configs - this class can be used on the application level
@@ -68,18 +68,18 @@
     """A mapping of types to callables that transform them into types supported for serialization."""
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         """Handle app init by injecting middleware, guards etc. into the app. This method can be used only on the app
         level.
 
         Args:
-            app_config: An instance of :class:`AppConfig <starlite.config.AppConfig>`
+            app_config: An instance of :class:`AppConfig <.config.app.AppConfig>`
 
         Returns:
-            The :class:`AppConfig <starlite.config.AppConfig>`.
+            The :class:`AppConfig <.config.app.AppConfig>`.
         """
         app_config.middleware.insert(0, self.middleware)
 
         if app_config.openapi_config:
             app_config.openapi_config = copy(app_config.openapi_config)
             if isinstance(app_config.openapi_config.components, list):
                 app_config.openapi_config.components.append(self.openapi_components)
@@ -144,28 +144,28 @@
 
     @property
     @abstractmethod
     def openapi_components(self) -> Components:  # pragma: no cover
         """Create OpenAPI documentation for the JWT auth schema used.
 
         Returns:
-            An :class:`Components <pydantic_openapi_schema.v3_1_0.components.Components>` instance.
+            An :class:`Components <starlite.openapi.spec.components.Components>` instance.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
     def security_requirement(self) -> SecurityRequirement:  # pragma: no cover
         """Return OpenAPI 3.1.
 
-        :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` for the auth
+        :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for the auth
         backend.
 
         Returns:
-            An OpenAPI 3.1 :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` dictionary.
+            An OpenAPI 3.1 :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` dictionary.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
     def middleware(self) -> DefineMiddleware:  # pragma: no cover
         """Create an instance of the config's ``authentication_middleware_class`` attribute and any required kwargs,
```

### Comparing `starlite-2.0.0a1/starlite/security/session_auth/auth.py` & `starlite-2.0.0a2/starlite/security/session_auth/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, Generic, Iterable
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generic, Iterable
 
-from pydantic_openapi_schema.v3_1_0 import (
-    Components,
-    SecurityRequirement,
-    SecurityScheme,
-)
-
-from starlite.connection import ASGIConnection
-from starlite.di import Provide
 from starlite.middleware.base import DefineMiddleware
 from starlite.middleware.session.base import BaseBackendConfig, BaseSessionBackendT
+from starlite.openapi.spec import Components, SecurityRequirement, SecurityScheme
 from starlite.security.base import AbstractSecurityConfig, UserType
-from starlite.security.session_auth.middleware import (
-    MiddlewareWrapper,
-    SessionAuthMiddleware,
-)
-from starlite.types import (
-    ControllerRouterHandler,
-    Guard,
-    Scopes,
-    SyncOrAsyncUnion,
-    TypeEncodersMap,
-)
+from starlite.security.session_auth.middleware import MiddlewareWrapper, SessionAuthMiddleware
+
+__all__ = ("SessionAuth",)
+
+if TYPE_CHECKING:
+    from starlite.connection import ASGIConnection
+    from starlite.di import Provide
+    from starlite.types import ControllerRouterHandler, Guard, Scopes, SyncOrAsyncUnion, TypeEncodersMap
 
 
 @dataclass
 class SessionAuth(Generic[UserType, BaseSessionBackendT], AbstractSecurityConfig[UserType, Dict[str, Any]]):
     """Session Based Security Backend."""
 
     session_backend_config: BaseBackendConfig[BaseSessionBackendT]
@@ -114,31 +104,31 @@
         return self.session_backend_config._backend_class(config=self.session_backend_config)
 
     @property
     def openapi_components(self) -> Components:
         """Create OpenAPI documentation for the Session Authentication schema used.
 
         Returns:
-            An :class:`Components <pydantic_openapi_schema.v3_1_0.components.Components>` instance.
+            An :class:`Components <starlite.openapi.spec.components.Components>` instance.
         """
         return Components(
-            securitySchemes={
+            security_schemes={
                 "sessionCookie": SecurityScheme(
                     type="apiKey",
                     name=self.session_backend_config.key,
                     security_scheme_in="cookie",  # pyright: ignore
                     description="Session cookie authentication.",
                 )
             }
         )
 
     @property
     def security_requirement(self) -> SecurityRequirement:
         """Return OpenAPI 3.1.
 
-        :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` for the auth
+        :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` for the auth
         backend.
 
         Returns:
-            An OpenAPI 3.1 :class:`SecurityRequirement <pydantic_openapi_schema.v3_1_0.security_requirement.SecurityRequirement>` dictionary.
+            An OpenAPI 3.1 :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>` dictionary.
         """
         return {"sessionCookie": []}
```

### Comparing `starlite-2.0.0a1/starlite/security/session_auth/middleware.py` & `starlite-2.0.0a2/starlite/security/session_auth/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     AbstractAuthenticationMiddleware,
     AuthenticationResult,
 )
 from starlite.middleware.exceptions import ExceptionHandlerMiddleware
 from starlite.middleware.session.base import SessionMiddleware
 from starlite.types import Empty, Scopes
 
+__all__ = ("MiddlewareWrapper", "SessionAuthMiddleware")
+
+
 if TYPE_CHECKING:
     from starlite.connection import ASGIConnection
     from starlite.security.session_auth.auth import SessionAuth
     from starlite.types import ASGIApp, Receive, Scope, Send
     from starlite.utils import AsyncCallable
 
 
@@ -90,22 +93,21 @@
         super().__init__(app=app, exclude=exclude, exclude_from_auth_key=exclude_opt_key, scopes=scopes)
         self.retrieve_user_handler = retrieve_user_handler
 
     async def authenticate_request(self, connection: "ASGIConnection[Any, Any, Any, Any]") -> AuthenticationResult:
         """Authenticate an incoming connection.
 
         Args:
-            connection: A Starlette ``HTTPConnection`` instance.
+            connection: An :class:`ASGIConnection <.connection.ASGIConnection>` instance.
 
         Raises:
-            :class:`NotAuthorizedException <starlite.exceptions.NotAuthorizedException>`: if session data is empty or user
-                is not found.
+            NotAuthorizedException: if session data is empty or user is not found.
 
         Returns:
-            :class:`AuthenticationResult <starlite.middleware.authentication.AuthenticationResult>`
+            :class:`AuthenticationResult <.middleware.authentication.AuthenticationResult>`
         """
         if not connection.session or connection.session is Empty:  # type: ignore
             # the assignment of 'Empty' forces the session middleware to clear session data.
             connection.scope["session"] = Empty
             raise NotAuthorizedException("no session data found")
 
         user = await self.retrieve_user_handler(connection.session, connection)
```

### Comparing `starlite-2.0.0a1/starlite/serialization.py` & `starlite-2.0.0a2/starlite/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 )
 from pydantic.color import Color
 from pydantic.json import decimal_encoder
 
 from starlite.exceptions import SerializationException
 from starlite.types import Empty
 
+__all__ = ("dec_hook", "decode_json", "decode_msgpack", "default_serializer", "encode_json", "encode_msgpack")
+
+
 if TYPE_CHECKING:
     from starlite.types import TypeEncodersMap
 
 T = TypeVar("T")
 
 
 def _enc_base_model(model: BaseModel) -> Any:
```

### Comparing `starlite-2.0.0a1/starlite/signature/models.py` & `starlite-2.0.0a2/starlite/_signature/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, ClassVar
+from typing import TYPE_CHECKING, Any, ClassVar, Literal
 
 from pydantic import BaseConfig, BaseModel, ValidationError
-from pydantic.fields import ModelField
 from typing_extensions import get_args, get_origin
 
 from starlite.connection import ASGIConnection, Request
 from starlite.constants import UNDEFINED_SENTINELS
 from starlite.enums import ScopeType
 from starlite.exceptions import InternalServerException, ValidationException
 from starlite.params import BodyKwarg, DependencyKwarg, ParameterKwarg
-from starlite.plugins import PluginMapping
 from starlite.types import Empty
 from starlite.utils import is_any, is_optional_union, is_union, make_non_optional_union
-from starlite.utils.predicates import (
-    is_generic,
-    is_mapping,
-    is_non_string_iterable,
-    is_non_string_sequence,
-)
+from starlite.utils.predicates import is_generic, is_mapping, is_non_string_iterable, is_non_string_sequence
+
+__all__ = ("PydanticSignatureModel", "SignatureField", "SignatureModel")
+
+if TYPE_CHECKING:
+    from pydantic.fields import ModelField
+
+    from starlite.plugins import PluginMapping
 
 
 @dataclass(unsafe_hash=True, frozen=True)
 class SignatureField:
     """Abstraction representing a model field. This class is meant to replace equivalent datastructures from, other
     libraries, for example, pydantic or msgspec.
     """
@@ -137,14 +137,19 @@
     def is_required(self) -> bool:
         """Check if the field should be marked as a required parameter."""
         if isinstance(self.kwarg_model, ParameterKwarg) and self.kwarg_model.required is not None:
             return self.kwarg_model.required
 
         return not (self.is_optional or self.is_any) and (self.is_empty or self.default_value is None)
 
+    @property
+    def is_literal(self) -> bool:
+        """Check if the field type is Literal."""
+        return get_origin(self.field_type) is Literal
+
     @classmethod
     def create(
         cls,
         field_type: Any,
         name: str = "",
         default_value: Any = Empty,
         children: tuple[SignatureField, ...] | None = None,
@@ -267,27 +272,27 @@
 
         Args:
             key: A field name.
 
         Returns:
             The plugin value, if available.
         """
-        value = self.__getattribute__(key)  # pylint: disable=unnecessary-dunder-call
+        value = self.__getattribute__(key)
         mapping = self.field_plugin_mappings.get(key)
         return mapping.get_model_instance_for_value(value) if mapping else value
 
     def to_dict(self) -> dict[str, Any]:
         """Normalize access to the signature model's dictionary method, because different backends use different methods
         for this.
 
         Returns: A dictionary of string keyed values.
         """
         if self.field_plugin_mappings:
             return {key: self._resolve_field_value(key) for key in self.__fields__}
-        return {key: self.__getattribute__(key) for key in self.__fields__}  # pylint: disable=unnecessary-dunder-call
+        return {key: self.__getattribute__(key) for key in self.__fields__}
 
     @classmethod
     def signature_field_from_model_field(cls, model_field: ModelField) -> SignatureField:
         """Create a SignatureField instance from a pydantic ModelField.
 
         Args:
             model_field: A pydantic ModelField instance.
```

### Comparing `starlite-2.0.0a1/starlite/signature/parsing.py` & `starlite-2.0.0a2/starlite/_signature/parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,38 @@
 from typing import TYPE_CHECKING, Any, List, cast
 
 from pydantic import create_model
 from pydantic.fields import FieldInfo, Undefined
 from pydantic_factories import ModelFactory
 from typing_extensions import get_args
 
+from starlite._signature.models import PydanticSignatureModel, SignatureModel
+from starlite._signature.utils import get_fn_type_hints
 from starlite.constants import SKIP_VALIDATION_NAMES, UNDEFINED_SENTINELS
 from starlite.datastructures import ImmutableState
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.params import BodyKwarg, DependencyKwarg, ParameterKwarg
-from starlite.plugins.base import (
+from starlite.plugins import (
     PluginMapping,
     SerializationPluginProtocol,
     get_plugin_for_value,
 )
-from starlite.signature.models import PydanticSignatureModel, SignatureModel
-from starlite.signature.utils import get_fn_type_hints
 from starlite.types import Empty
 from starlite.utils import is_optional_union
 from starlite.utils.helpers import unwrap_partial
 
+__all__ = (
+    "ParsedSignatureParameter",
+    "create_pydantic_signature_model",
+    "create_signature_model",
+    "get_type_annotation_from_plugin",
+    "parse_fn_signature",
+)
+
+
 if TYPE_CHECKING:
     from starlite.types import AnyCallable
 
 
 @dataclass
 class ParsedSignatureParameter:
     """Represents the parameters of a callable for purpose of signature model generation."""
@@ -112,34 +121,38 @@
     type_value = type_args[0] if type_args else parameter.annotation
     field_plugin_mappings[parameter.name] = PluginMapping(plugin=plugin, model_class=type_value)
     pydantic_model = plugin.to_data_container_class(model_class=type_value, parameter_name=parameter.name)
     return List[pydantic_model] if type_args else pydantic_model  # type:ignore[valid-type]
 
 
 def parse_fn_signature(
-    fn: AnyCallable, plugins: list[SerializationPluginProtocol], dependency_name_set: set[str]
+    fn: AnyCallable,
+    plugins: list[SerializationPluginProtocol],
+    dependency_name_set: set[str],
+    signature_namespace: dict[str, Any],
 ) -> tuple[list[ParsedSignatureParameter], Any, dict[str, PluginMapping], set[str]]:
     """Parse a function signature into data used for the generation of a signature model.
 
     Args:
         fn: A callable.
         plugins: A list of plugins.
         dependency_name_set: A set of dependency names
+        signature_namespace: mapping of names to types for forward reference resolution
 
     Returns:
         A tuple containing the following values for generating a signature model: a mapping of field definitions, the
         callable's return annotation, a mapping of field names to plugins - if any, and an updated dependency name set.
     """
     signature = Signature.from_callable(fn)
     fn_name = getattr(fn, "__name__", "anonymous")
 
     field_plugin_mappings: dict[str, PluginMapping] = {}
     parsed_params: list[ParsedSignatureParameter] = []
     dependency_names: set[str] = set()
-    fn_type_hints = get_fn_type_hints(fn)
+    fn_type_hints = get_fn_type_hints(fn, namespace=signature_namespace)
 
     parameters = (
         ParsedSignatureParameter.from_parameter(
             parameter=parameter, parameter_name=name, fn_name=fn_name, fn_type_hints=fn_type_hints
         )
         for name, parameter in signature.parameters.items()
         if name not in ("self", "cls")
@@ -170,36 +183,41 @@
 
         parsed_params.append(parameter)
 
     return parsed_params, signature.return_annotation, field_plugin_mappings, dependency_names
 
 
 def create_signature_model(
-    fn: AnyCallable, plugins: list[SerializationPluginProtocol], dependency_name_set: set[str]
+    fn: AnyCallable,
+    plugins: list[SerializationPluginProtocol],
+    dependency_name_set: set[str],
+    signature_namespace: dict[str, Any],
 ) -> type[SignatureModel]:
     """Create a model for a callable's signature. The model can than be used to parse and validate before passing it to
     the callable.
 
     Args:
         fn: A callable.
         plugins: A list of plugins.
         dependency_name_set: A set of dependency names
+        signature_namespace: mapping of names to types for forward reference resolution
 
     Returns:
-        A signature model.
+        A _signature model.
     """
 
     unwrapped_fn = cast("AnyCallable", unwrap_partial(fn))
     fn_name = getattr(fn, "__name__", "anonymous")
     fn_module = getattr(fn, "__module__", None)
 
     parsed_params, return_annotation, field_plugin_mappings, dependency_names = parse_fn_signature(
         fn=unwrapped_fn,
         plugins=plugins,
         dependency_name_set=dependency_name_set,
+        signature_namespace=signature_namespace,
     )
 
     # TODO: we will implement logic here to determine what kind of SignatureModel we are creating.
     # For now this is only pydantic:
 
     return create_pydantic_signature_model(
         fn_name=fn_name,
@@ -231,34 +249,39 @@
 
     Returns:
         The created PydanticSignatureModel.
     """
     field_definitions: dict[str, tuple[Any, Any]] = {}
 
     for parameter in parsed_params:
+        if isinstance(parameter.default, (ParameterKwarg, BodyKwarg)):
+            field_info = FieldInfo(
+                **asdict(parameter.default), kwargs_model=parameter.default, parsed_parameter=parameter
+            )
+        else:
+            field_info = FieldInfo(default=..., parsed_parameter=parameter)
         if parameter.should_skip_validation:
+            field_type = Any
             if isinstance(parameter.default, DependencyKwarg):
-                field_definitions[parameter.name] = (
-                    Any,
-                    parameter.default.default if parameter.default.default is not Empty else None,
-                )
-            else:
-                field_definitions[parameter.name] = (Any, ...)
+                field_info.default = parameter.default.default if parameter.default.default is not Empty else None
         elif isinstance(parameter.default, (ParameterKwarg, BodyKwarg)):
-            field_info = FieldInfo(**asdict(parameter.default), kwargs_model=parameter.default)
+            field_type = parameter.annotation
             field_info.default = parameter.default.default if parameter.default.default is not Empty else Undefined
-            field_definitions[parameter.name] = (parameter.annotation, field_info)
         elif ModelFactory.is_constrained_field(parameter.default):
-            field_definitions[parameter.name] = (parameter.default, ...)
+            field_type = parameter.default
         elif parameter.default_defined:
-            field_definitions[parameter.name] = (parameter.annotation, parameter.default)
+            field_type = parameter.annotation
+            field_info.default = parameter.default
         elif not parameter.optional:
-            field_definitions[parameter.name] = (parameter.annotation, ...)
+            field_type = parameter.annotation
         else:
-            field_definitions[parameter.name] = (parameter.annotation, None)
+            field_type = parameter.annotation
+            field_info.default = None
+
+        field_definitions[parameter.name] = (field_type, field_info)
 
     model: type[PydanticSignatureModel] = create_model(  # type: ignore
         f"{fn_name}_signature_model",
         __base__=PydanticSignatureModel,
         __module__=fn_module or "pydantic.main",
         **field_definitions,
     )
```

### Comparing `starlite-2.0.0a1/starlite/signature/utils.py` & `starlite-2.0.0a2/starlite/_signature/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 import sys
+import typing
 from inspect import isclass, ismethod
 from typing import TYPE_CHECKING, Any, cast
 
 from typing_extensions import get_type_hints
 
 from starlite.connection import Request, WebSocket
 from starlite.datastructures import Headers, ImmutableState, State
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.types import Receive, Scope, Send, WebSocketScope
-from starlite.utils.compat import py_38_safe_annotations
+
+__all__ = ("get_fn_type_hints", "get_signature_model")
+
 
 if TYPE_CHECKING:
-    from starlite.signature.models import SignatureModel
+    from starlite._signature.models import SignatureModel
 
 
-STARLITE_GLOBAL_NAMES = {
+_GLOBAL_NAMES = {
     "Headers": Headers,
     "ImmutableState": ImmutableState,
     "Receive": Receive,
     "Request": Request,
     "Scope": Scope,
     "Send": Send,
     "State": State,
@@ -37,19 +40,20 @@
     """Retrieve and validate the signature model from a provider or handler."""
     try:
         return cast("type[SignatureModel]", value.signature_model)
     except AttributeError as e:  # pragma: no cover
         raise ImproperlyConfiguredException(f"The 'signature_model' attribute for {value} is not set") from e
 
 
-def get_fn_type_hints(fn: Any) -> dict[str, Any]:
+def get_fn_type_hints(fn: Any, namespace: dict[str, Any] | None = None) -> dict[str, Any]:
     """Resolve type hints for ``fn``.
 
     Args:
         fn: Thing that is having its signature modelled.
+        namespace: Extra names for resolution of forward references.
 
     Returns:
         Mapping of names to types.
     """
     fn_to_inspect: Any = fn
 
     if isclass(fn_to_inspect):
@@ -61,10 +65,14 @@
 
     # inspect the underlying function for methods
     if hasattr(fn_to_inspect, "__func__"):
         fn_to_inspect = fn_to_inspect.__func__
 
     # Order important. If a starlite name has been overridden in the function module, we want
     # to use that instead of the starlite one.
-    namespace = {**STARLITE_GLOBAL_NAMES, **vars(sys.modules[fn_to_inspect.__module__])}
-    with py_38_safe_annotations(fn_to_inspect):
-        return get_type_hints(fn_to_inspect, globalns=namespace)
+    namespace = {
+        **_GLOBAL_NAMES,
+        **vars(typing),
+        **vars(sys.modules[fn_to_inspect.__module__]),
+        **(namespace or {}),
+    }
+    return get_type_hints(fn_to_inspect, globalns=namespace)
```

### Comparing `starlite-2.0.0a1/starlite/static_files/base.py` & `starlite-2.0.0a2/starlite/static_files/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
-from os.path import commonpath, join
+from os.path import commonpath
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, Sequence
 
 from starlite.enums import ScopeType
 from starlite.exceptions import MethodNotAllowedException, NotFoundException
 from starlite.file_system import FileSystemAdapter
 from starlite.response import FileResponse
 from starlite.status_codes import HTTP_404_NOT_FOUND
 
+__all__ = ("StaticFiles",)
+
+
 if TYPE_CHECKING:
     from starlite.types import Receive, Scope, Send
     from starlite.types.composite_types import PathType
     from starlite.types.file_types import FileInfo, FileSystemProtocol
 
 
 class StaticFiles:
@@ -27,41 +30,41 @@
         directories: Sequence[PathType],
         file_system: FileSystemProtocol,
         send_as_attachment: bool = False,
     ) -> None:
         """Initialize the Application.
 
         Args:
-            is_html_mode: Flag dictating whether serving html. If true, the default file will be 'index.html'.
+            is_html_mode: Flag dictating whether serving html. If true, the default file will be ``index.html``.
             directories: A list of directories to serve files from.
             file_system: The file_system spec to use for serving files.
             send_as_attachment: Whether to send the file with a ``content-disposition`` header of
              ``attachment`` or ``inline``
         """
         self.adapter = FileSystemAdapter(file_system)
         self.directories = tuple(Path(p).resolve() for p in directories)
         self.is_html_mode = is_html_mode
         self.send_as_attachment = send_as_attachment
 
     async def get_fs_info(
-        self, directories: Sequence[PathType], file_path: str
-    ) -> tuple[str, FileInfo] | tuple[None, None]:
-        """Return the resolved path and a :func:`stat_result <os.stat_result>`.
+        self, directories: Sequence[PathType], file_path: PathType
+    ) -> tuple[Path, FileInfo] | tuple[None, None]:
+        """Return the resolved path and a :class:`stat_result <os.stat_result>`.
 
         Args:
             directories: A list of directory paths.
             file_path: A file path to resolve
 
         Returns:
             A tuple with an optional resolved :class:`Path <anyio.Path>` instance and an optional
-            :func:`stat_result <os.stat_result>`.
+            :class:`stat_result <os.stat_result>`.
         """
         for directory in directories:
             try:
-                joined_path = join(directory, file_path)  # noqa: PL118
+                joined_path = Path(directory, file_path)
                 file_info = await self.adapter.info(joined_path)
                 if file_info and commonpath([str(directory), file_info["name"], joined_path]) == str(directory):
                     return joined_path, file_info
             except FileNotFoundError:
                 continue
         return None, None
 
@@ -77,24 +80,25 @@
             None
         """
         if scope["type"] != ScopeType.HTTP or scope["method"] not in {"GET", "HEAD"}:
             raise MethodNotAllowedException()
 
         split_path = scope["path"].split("/")
         filename = split_path[-1]
-        joined_path = join(*split_path)  # noqa: PL118
+        joined_path = Path(*split_path)
         resolved_path, fs_info = await self.get_fs_info(directories=self.directories, file_path=joined_path)
         content_disposition_type: Literal["inline", "attachment"] = (
             "attachment" if self.send_as_attachment else "inline"
         )
 
         if self.is_html_mode and fs_info and fs_info["type"] == "directory":
             filename = "index.html"
             resolved_path, fs_info = await self.get_fs_info(
-                directories=self.directories, file_path=join(resolved_path or joined_path, filename)
+                directories=self.directories,
+                file_path=Path(resolved_path or joined_path) / filename,
             )
 
         if fs_info and fs_info["type"] == "file":
             await FileResponse(
                 path=resolved_path or joined_path,
                 file_info=fs_info,
                 file_system=self.adapter.file_system,
```

### Comparing `starlite-2.0.0a1/starlite/status_codes.py` & `starlite-2.0.0a2/starlite/status_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 WS_1011_INTERNAL_ERROR: Literal[1011] = 1011
 WS_1012_SERVICE_RESTART: Literal[1012] = 1012
 WS_1013_TRY_AGAIN_LATER: Literal[1013] = 1013
 WS_1014_BAD_GATEWAY: Literal[1014] = 1014
 WS_1015_TLS_HANDSHAKE: Literal[1015] = 1015
 
 
-__all__ = [
+__all__ = (
     "HTTP_100_CONTINUE",
     "HTTP_101_SWITCHING_PROTOCOLS",
     "HTTP_102_PROCESSING",
     "HTTP_103_EARLY_HINTS",
     "HTTP_200_OK",
     "HTTP_201_CREATED",
     "HTTP_202_ACCEPTED",
@@ -190,8 +190,8 @@
     "WS_1009_MESSAGE_TOO_BIG",
     "WS_1010_MANDATORY_EXT",
     "WS_1011_INTERNAL_ERROR",
     "WS_1012_SERVICE_RESTART",
     "WS_1013_TRY_AGAIN_LATER",
     "WS_1014_BAD_GATEWAY",
     "WS_1015_TLS_HANDSHAKE",
-]
+)
```

### Comparing `starlite-2.0.0a1/starlite/storage/base.py` & `starlite-2.0.0a2/starlite/stores/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from datetime import datetime, timedelta
-from typing import Optional
+from datetime import datetime, timedelta, timezone
+from typing import TYPE_CHECKING, Optional
 
 from msgspec import Struct
 from msgspec.msgpack import decode as msgpack_decode
 from msgspec.msgpack import encode as msgpack_encode
 
+if TYPE_CHECKING:
+    from typing_extensions import Self
 
-class Storage(ABC):  # pragma: no cover
+
+__all__ = ("Store", "NamespacedStore", "StorageObject")
+
+
+class Store(ABC):  # pragma: no cover
     """Thread and process safe asynchronous key/value store."""
 
     @abstractmethod
     async def set(self, key: str, value: str | bytes, expires_in: int | timedelta | None = None) -> None:
         """Set a value.
 
         Args:
@@ -67,45 +73,60 @@
     async def expires_in(self, key: str) -> int | None:
         """Get the time in seconds ``key`` expires in. If no such ``key`` exists or no
         expiry time was set, return ``None``.
         """
         raise NotImplementedError
 
 
+class NamespacedStore(Store):
+    """A subclass of :class:`Store`, offering hierarchical namespacing.
+
+    Bulk actions on a parent namespace should affect all child namespaces, whereas other operations on all namespaces
+    should be isolated.
+    """
+
+    @abstractmethod
+    def with_namespace(self, namespace: str) -> Self:
+        """Return a new instance of :class:`NamespacedStore`, which exists in a child namespace of the current namespace.
+        Bulk actions on the parent namespace should affect all child namespaces, whereas other operations on all
+        namespaces should be isolated.
+        """
+
+
 class StorageObject(Struct):
-    """Msgspec :class:`Struct` to store serialized data alongside with their expiry time."""
+    """:class:`msgspec.Struct` to store serialized data alongside with their expiry time."""
 
-    expires_at: Optional[datetime]
+    expires_at: Optional[datetime]  # noqa: UP007
     data: bytes
 
     @classmethod
     def new(cls, data: bytes, expires_in: int | timedelta | None) -> StorageObject:
         """Construct a new :class:`StorageObject` instance."""
         if expires_in is not None and not isinstance(expires_in, timedelta):
             expires_in = timedelta(seconds=expires_in)
         return cls(
             data=data,
-            expires_at=(datetime.now() + expires_in) if expires_in else None,
+            expires_at=(datetime.now(tz=timezone.utc) + expires_in) if expires_in else None,
         )
 
     @property
     def expired(self) -> bool:
         """Return if the :class:`StorageObject` is expired"""
-        return self.expires_at is not None and datetime.now() >= self.expires_at
+        return self.expires_at is not None and datetime.now(tz=timezone.utc) >= self.expires_at
 
     @property
     def expires_in(self) -> int:
         """Return the expiry time of this ``StorageObject`` in seconds. If no expiry time
         was set, return ``-1``.
         """
         if self.expires_at:
-            return (self.expires_at - datetime.now()).seconds
+            return (self.expires_at - datetime.now(tz=timezone.utc)).seconds
         return -1
 
     def to_bytes(self) -> bytes:
         """Encode the instance to bytes"""
         return msgpack_encode(self)
 
     @classmethod
     def from_bytes(cls, raw: bytes) -> StorageObject:
-        """Load an previously encoded with :meth:`StorageObject.to_bytes`"""
+        """Load a previously encoded with :meth:`StorageObject.to_bytes`"""
         return msgpack_decode(raw, type=cls)
```

### Comparing `starlite-2.0.0a1/starlite/storage/file.py` & `starlite-2.0.0a2/starlite/stores/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,55 @@
 from __future__ import annotations
 
 import os
 import shutil
+import unicodedata
 from tempfile import mkstemp
 from typing import TYPE_CHECKING
 
 from anyio import Path
 from anyio.to_thread import run_sync
 
-from .base import Storage, StorageObject
+from .base import NamespacedStore, StorageObject
+
+__all__ = ("FileStore",)
+
 
 if TYPE_CHECKING:
     from datetime import timedelta
     from os import PathLike
 
 
-class FileStorage(Storage):
+def _safe_file_name(name: str) -> str:
+    name = unicodedata.normalize("NFKD", name)
+    return "".join(c if c.isalnum() else str(ord(c)) for c in name)
+
+
+class FileStore(NamespacedStore):
     """File based, thread and process safe, asynchronous key/value store."""
 
-    __slots__ = ("path",)
+    __slots__ = {"path": "file path"}
 
     def __init__(self, path: PathLike) -> None:
         """Initialize ``FileStorage``.
 
         Args:
             path: Path to store data under
         """
         self.path = Path(path)
 
+    def with_namespace(self, namespace: str) -> FileStore:
+        """Return a new instance of :class:`FileStore`, using  a sub-path of the current store's path."""
+        if not namespace.isalnum():
+            raise ValueError(f"Invalid namespace: {namespace!r}")
+        return FileStore(self.path / namespace)
+
+    def _path_from_key(self, key: str) -> Path:
+        return self.path / _safe_file_name(key)
+
     @staticmethod
     async def _load_from_path(path: Path) -> StorageObject | None:
         try:
             data = await path.read_bytes()
             return StorageObject.from_bytes(data)
         except FileNotFoundError:
             return None
@@ -46,15 +64,15 @@
                 finally:
                     os.close(tmp_file_fd)
 
                 shutil.move(tmp_file_name, target_file)
                 renamed = True
             finally:
                 if not renamed:
-                    os.unlink(tmp_file_name)  # noqa: PL108
+                    os.unlink(tmp_file_name)  # noqa: PTH108
         except OSError:
             pass
 
     async def _write(self, target_file: Path, storage_obj: StorageObject) -> None:
         await run_sync(self._write_sync, target_file, storage_obj)
 
     async def set(self, key: str, value: str | bytes, expires_in: int | timedelta | None = None) -> None:
@@ -64,16 +82,17 @@
             key: Key to associate the value with
             value: Value to store
             expires_in: Time in seconds before the key is considered expired
 
         Returns:
             ``None``
         """
+
         await self.path.mkdir(exist_ok=True)
-        path = self.path / key
+        path = self._path_from_key(key)
         if isinstance(value, str):
             value = value.encode("utf-8")
         storage_obj = StorageObject.new(data=value, expires_in=expires_in)
         await self._write(path, storage_obj)
 
     async def get(self, key: str, renew_for: int | timedelta | None = None) -> bytes | None:
         """Get a value.
@@ -84,15 +103,15 @@
                 expiry time for ``renew_for`` seconds. If the value has not been set
                 with an expiry time this is a no-op
 
         Returns:
             The value associated with ``key`` if it exists and is not expired, else
             ``None``
         """
-        path = self.path / key
+        path = self._path_from_key(key)
         storage_obj = await self._load_from_path(path)
 
         if not storage_obj:
             return None
 
         if storage_obj.expired:
             await path.unlink(missing_ok=True)
@@ -107,45 +126,44 @@
         """Delete a value.
 
         If no such key exists, this is a no-op.
 
         Args:
             key: Key of the value to delete
         """
-        path = self.path / key
+        path = self._path_from_key(key)
         await path.unlink(missing_ok=True)
 
     async def delete_all(self) -> None:
         """Delete all stored values.
 
-        .. note::
-
-            This deletes and recreates :attr:`FileStorage.path`
+        Note:
+            This deletes and recreates :attr:`FileStore.path`
         """
 
         await run_sync(shutil.rmtree, self.path)
         await self.path.mkdir(exist_ok=True)
 
     async def delete_expired(self) -> None:
         """Delete expired items.
 
         Since expired items are normally only cleared on access (i.e. when calling
-        :meth:`.get` or :meth:`.set`, this method should be called in regular intervals
+        :meth:`.get`), this method should be called in regular intervals
         to free disk space.
         """
         async for file in self.path.iterdir():
             wrapper = await self._load_from_path(file)
             if wrapper and wrapper.expired:
                 await file.unlink(missing_ok=True)
 
     async def exists(self, key: str) -> bool:
         """Check if a given ``key`` exists."""
-        path = self.path / key
+        path = self._path_from_key(key)
         return await path.exists()
 
     async def expires_in(self, key: str) -> int | None:
         """Get the time in seconds ``key`` expires in. If no such ``key`` exists or no
         expiry time was set, return ``None``.
         """
-        if storage_obj := await self._load_from_path(self.path / key):
+        if storage_obj := await self._load_from_path(self._path_from_key(key)):
             return storage_obj.expires_in
         return None
```

### Comparing `starlite-2.0.0a1/starlite/storage/memory.py` & `starlite-2.0.0a2/starlite/stores/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import anyio
 from anyio import Lock
 
-from .base import Storage, StorageObject
+from .base import StorageObject, Store
+
+__all__ = ("MemoryStore",)
+
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
 
-class MemoryStorage(Storage):
+class MemoryStore(Store):
     """In memory, thread-safe, asynchronous key/value store."""
 
     __slots__ = ("_store", "_lock")
 
     def __init__(self) -> None:
-        """Initialize :class:`MemoryStorage`"""
+        """Initialize :class:`MemoryStore`"""
         self._store: dict[str, StorageObject] = {}
         self._lock = Lock()
 
     async def set(self, key: str, value: str | bytes, expires_in: int | timedelta | None = None) -> None:
         """Set a value.
 
         Args:
@@ -83,15 +86,15 @@
         async with self._lock:
             self._store.clear()
 
     async def delete_expired(self) -> None:
         """Delete expired items.
 
         Since expired items are normally only cleared on access (i.e. when calling
-        :meth:`.get` or :meth:`.set`, this method should be called in regular intervals
+        :meth:`.get`), this method should be called in regular intervals
         to free memory.
         """
         async with self._lock:
             new_store = {}
             for i, (key, storage_obj) in enumerate(self._store.items()):
                 if not storage_obj.expired:
                     new_store[key] = storage_obj
```

### Comparing `starlite-2.0.0a1/starlite/storage/redis.py` & `starlite-2.0.0a2/starlite/stores/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 from redis.asyncio import Redis
 from redis.asyncio.connection import ConnectionPool
 
 from starlite.exceptions import ImproperlyConfiguredException
 from starlite.types import Empty, EmptyType
 
-from .base import Storage
+from .base import NamespacedStore
 
+__all__ = ("RedisStore",)
 
-class RedisStorage(Storage):
+
+class RedisStore(NamespacedStore):
     """Redis based, thread and process safe asynchronous key/value store."""
 
     __slots__ = ("_redis",)
 
     def __init__(self, redis: Redis, namespace: str | None | EmptyType = Empty) -> None:
-        """Initialize :class:`RedisStorage`
+        """Initialize :class:`RedisStore`
 
         Args:
             redis: An :class:`redis.asyncio.Redis` instance
             namespace: A key prefix to simulate a namespace in redis. If not given,
                 defaults to ``STARLITE``. Namespacing can be explicitly disabled by passing
                 ``None``. This will make :meth:`.delete_all` unavailable.
         """
@@ -60,23 +62,23 @@
         until cursor == 0
         """
         )
 
     @classmethod
     def with_client(
         cls,
-        url: str,
+        url: str = "redis://localhost:6379",
         *,
         db: int | None = None,
         port: int | None = None,
         username: str | None = None,
         password: str | None = None,
         namespace: str | None | EmptyType = Empty,
-    ) -> RedisStorage:
-        """Initialize a :class:`RedisStorage` instance with a new class:`redis.asyncio.Redis` instance.
+    ) -> RedisStore:
+        """Initialize a :class:`RedisStore` instance with a new class:`redis.asyncio.Redis` instance.
 
         Args:
             url: Redis URL to connect to
             db: Redis database to use
             port: Redis port to use
             username: Redis username to use
             password: Redis password to use
@@ -88,16 +90,16 @@
             decode_responses=False,
             port=port,
             username=username,
             password=password,
         )
         return cls(redis=Redis(connection_pool=pool), namespace=namespace)
 
-    def with_namespace(self, namespace: str) -> RedisStorage:
-        """Return a new :class:`RedisStorage` with a nested virtual key namespace.
+    def with_namespace(self, namespace: str) -> RedisStore:
+        """Return a new :class:`RedisStore` with a nested virtual key namespace.
         The current instances namespace will serve as a prefix for the namespace, so it
         can be considered the parent namespace.
         """
         return type(self)(redis=self._redis, namespace=f"{self.namespace}_{namespace}" if self.namespace else namespace)
 
     def _make_key(self, key: str) -> str:
         prefix = f"{self.namespace}:" if self.namespace else ""
```

### Comparing `starlite-2.0.0a1/starlite/template/base.py` & `starlite-2.0.0a2/starlite/template/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Protocol, TypeVar, runtime_checkable
 
 from typing_extensions import TypedDict
 
+__all__ = (
+    "TemplateContext",
+    "TemplateEngineProtocol",
+    "TemplateProtocol",
+    "csrf_token",
+    "url_for",
+    "url_for_static_asset",
+)
+
+
 if TYPE_CHECKING:
     from pydantic import DirectoryPath
 
     from starlite.connection import Request
 
 
 class TemplateContext(TypedDict):
@@ -40,15 +50,14 @@
     Notes:
         - to use this function make sure to pass an instance of :ref:`CSRFConfig <starlite.config.csrf_config.CSRFConfig>` to
         the :class:`Starlite <starlite.app.Starlite>` constructor.
 
     Args:
         context: The template context.
 
-
     Returns:
         A CSRF token if the app level ``csrf_config`` is set, otherwise an empty string.
     """
     return context["request"].scope.get("_csrf_token", "")  # type: ignore
 
 
 def url_for_static_asset(context: TemplateContext, name: str, file_path: str) -> str:
@@ -74,14 +83,15 @@
     Template is a class that has a render method which renders the template into a string.
     """
 
     def render(self, *args: Any, **kwargs: Any) -> str:
         """Return the rendered template as a string.
 
         Args:
+            *args: Positional arguments passed to the TemplateEngine
             **kwargs: A string keyed mapping of values passed to the TemplateEngine
 
         Returns:
             The rendered template string
         """
         ...
 
@@ -99,22 +109,23 @@
         Args:
             directory: Direct path or list of directory paths from which to serve templates.
         """
         ...
 
     def get_template(self, template_name: str) -> T_co:
         """Retrieve a template by matching its name (dotted path) with files in the directory or directories provided.
+
         Args:
             template_name: A dotted path
 
         Returns:
             Template instance
 
         Raises:
-            :class:`TemplateNotFoundException <starlite.exceptions.TemplateNotFoundException>`: if no template is found.
+            TemplateNotFoundException: if no template is found.
         """
         ...
 
     def register_template_callable(self, key: str, template_callable: Callable[[dict[str, Any]], Any]) -> None:
         """Register a callable on the template engine.
 
         Args:
```

### Comparing `starlite-2.0.0a1/starlite/testing/client/__init__.py` & `starlite-2.0.0a2/starlite/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/testing/client/async_client.py` & `starlite-2.0.0a2/starlite/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `starlite-2.0.0a1/starlite/testing/client/base.py` & `starlite-2.0.0a2/starlite/testing/client/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-import warnings
 from contextlib import contextmanager
 from http.cookiejar import CookieJar
 from typing import TYPE_CHECKING, Any, Generator, Generic, Mapping, TypeVar, cast
+from warnings import warn
 
 from anyio.from_thread import BlockingPortal, start_blocking_portal
 
 from starlite.connection import ASGIConnection
 from starlite.datastructures import MutableScopeHeaders
 from starlite.exceptions import (
     ImproperlyConfiguredException,
@@ -79,18 +79,19 @@
         base_url: str = "http://testserver.local",
         backend: AnyIOBackend = "asyncio",
         backend_options: Mapping[str, Any] | None = None,
         session_config: BaseBackendConfig | None = None,
         cookies: CookieTypes | None = None,
     ):
         if "." not in base_url:
-            warnings.warn(
+            warn(
                 f"The base_url {base_url!r} might cause issues. Try adding a domain name such as .local: "
                 f"'{base_url}.local'",
                 UserWarning,
+                stacklevel=1,
             )
         self._session_backend: BaseSessionBackend | None = None
         if session_config:
             self._session_backend = session_config._backend_class(config=session_config)
         self.app = app
         self.base_url = base_url
         self.backend = backend
```

### Comparing `starlite-2.0.0a1/starlite/testing/client/sync_client.py` & `starlite-2.0.0a2/starlite/testing/client/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.parse import urljoin
 
 from httpx import USE_CLIENT_DEFAULT, Client, Response
 
 from starlite import HttpMethod
 from starlite.testing.client.base import BaseTestClient
 from starlite.testing.life_span_handler import LifeSpanHandler
-from starlite.testing.transport import ConnectionUpgradeException, TestClientTransport
+from starlite.testing.transport import ConnectionUpgradeExceptionError, TestClientTransport
 from starlite.types import AnyIOBackend, ASGIApp
 
 if TYPE_CHECKING:
     from httpx._client import UseClientDefault
     from httpx._types import (
         AuthTypes,
         CookieTypes,
@@ -492,15 +492,15 @@
             cookies: Request cookies.
             auth: Auth headers.
             follow_redirects: Whether to follow redirects.
             timeout: Request timeout.
             extensions: Dictionary of ASGI extensions.
 
         Returns:
-            An :class:`WebSocketTestSession <starlite.testing.test_client.WebSocketTestSession>` instance.
+            A `WebSocketTestSession <starlite.testing.WebSocketTestSession>` instance.
         """
         url = urljoin("ws://testserver", url)
         default_headers: dict[str, str] = {}
         default_headers.setdefault("connection", "upgrade")
         default_headers.setdefault("sec-websocket-key", "testserver==")
         default_headers.setdefault("sec-websocket-version", "13")
         if subprotocols is not None:
@@ -514,15 +514,15 @@
                 params=params,
                 cookies=cookies,
                 auth=auth,
                 follow_redirects=follow_redirects,
                 timeout=timeout,
                 extensions=extensions,
             )
-        except ConnectionUpgradeException as exc:
+        except ConnectionUpgradeExceptionError as exc:
             return exc.session
 
         raise RuntimeError("Expected WebSocket upgrade")  # pragma: no cover
 
     def set_session_data(self, data: dict[str, Any]) -> None:
         """Set session data.
```

### Comparing `starlite-2.0.0a1/starlite/testing/helpers.py` & `starlite-2.0.0a2/starlite/testing/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal, Mapping, Sequence
 
-from starlite.app import DEFAULT_CACHE_CONFIG, Starlite
+from starlite.app import Starlite
 from starlite.controller import Controller
 from starlite.events import SimpleEventEmitter
 from starlite.testing.client import AsyncTestClient, TestClient
 from starlite.utils.predicates import is_class_and_subclass
 
 if TYPE_CHECKING:
     from starlite import Request, WebSocket
     from starlite.config.allowed_hosts import AllowedHostsConfig
-    from starlite.config.cache import CacheConfig
     from starlite.config.compression import CompressionConfig
     from starlite.config.cors import CORSConfig
     from starlite.config.csrf import CSRFConfig
-    from starlite.config.logging import BaseLoggingConfig
-    from starlite.config.openapi import OpenAPIConfig
-    from starlite.config.static_files import StaticFilesConfig
-    from starlite.config.template import TemplateConfig
+    from starlite.config.response_cache import ResponseCacheConfig
+    from starlite.datastructures import State
     from starlite.events import BaseEventEmitterBackend, EventListener
+    from starlite.logging.config import BaseLoggingConfig
     from starlite.middleware.session.base import BaseBackendConfig
+    from starlite.openapi.config import OpenAPIConfig
     from starlite.plugins import PluginProtocol, SerializationPluginProtocol
+    from starlite.static_files.config import StaticFilesConfig
+    from starlite.template.config import TemplateConfig
     from starlite.types import (
         AfterExceptionHookHandler,
         AfterRequestHookHandler,
         AfterResponseHookHandler,
         BeforeMessageSendHookHandler,
         BeforeRequestHookHandler,
         ControllerRouterHandler,
         Dependencies,
         ExceptionHandlersMap,
         Guard,
-        InitialStateType,
         LifeSpanHandler,
         LifeSpanHookHandler,
         Middleware,
         OnAppInitHandler,
         OptionalSequence,
         ParametersMap,
         ResponseType,
@@ -54,23 +54,22 @@
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
     before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
     before_startup: OptionalSequence[LifeSpanHookHandler] = None,
-    cache_config: CacheConfig = DEFAULT_CACHE_CONFIG,
+    cache_config: ResponseCacheConfig | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     dependencies: Dependencies | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] = None,
-    initial_state: InitialStateType | None = None,
     listeners: OptionalSequence[EventListener] = None,
     logging_config: BaseLoggingConfig | None = None,
     middleware: OptionalSequence[Middleware] = None,
     multipart_form_part_limit: int = 1000,
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
     on_shutdown: OptionalSequence[LifeSpanHandler] = None,
     on_startup: OptionalSequence[LifeSpanHandler] = None,
@@ -78,14 +77,16 @@
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_class: ResponseType | None = None,
     root_path: str = "",
     session_config: BaseBackendConfig | None = None,
+    signature_namespace: Mapping[str, Any] | None = None,
+    state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] = None,
     template_config: TemplateConfig | None = None,
     websocket_class: type[WebSocket] | None = None,
 ) -> TestClient[Starlite]:
     """Create a Starlite app instance and initializes it.
 
     :class:`TestClient <starlite.testing.TestClient>` with it.
@@ -96,100 +97,96 @@
 
     Examples:
         .. code-block: python
 
             from starlite import get
             from starlite.testing import create_test_client
 
-
             @get("/some-path")
             def my_handler() -> dict[str, str]:
                 return {"hello": "world"}
 
-
             def test_my_handler() -> None:
                 with create_test_client(my_handler) as client:
                     response == client.get("/some-path")
                     assert response.json() == {"hello": "world"}
 
-
     Args:
         route_handlers: A single handler or a sequence of route handlers, which can include instances of
-            :class:`Router <starlite.router.Router>`, subclasses of :class:`Controller <starlite.controller.Controller>` or
+            :class:`Router <starlite.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or
             any function decorated by the route handler decorators.
-        after_exception: A sequence of :class:`exception hook handlers <starlite.types.AfterExceptionHookHandler>`.
-            This hook is called after an exception occurs. In difference to exception handlers, it is not meant to
-            return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
+        after_exception: A sequence of exception hook handlers. This hook is called after an exception occurs. In
+            difference to exception handlers, it is not meant to return a response - only to process the exception
+            (e.g. log it, send it to Sentry etc.).
         after_request: A sync or async function executed after the route handler function returned and the response
             object has been resolved. Receives the response object which may be any subclass of
-            :class:`Response <starlite.response.Response>`.
+            :class:`Response <.response.Response>`.
         after_response: A sync or async function called after the response has been awaited. It receives the
-            :class:`Request <starlite.connection.Request>` object and should not return any values.
-        after_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-            This hook is called during the ASGI shutdown, after all callables in the 'on_shutdown' list have been
-            called.
-        after_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-            This hook is called during the ASGI startup, after all callables in the 'on_startup' list have been
-            called.
-        allowed_hosts: A sequence of allowed hosts, or an :class:`allowed hosts config <starlite.config.AllowedHostsConfig>`
-            instance. Enables the builtin allowed hosts middleware.
+            :class:`Request <.connection.Request>` object and should not return any values.
+        after_shutdown: A sequence of life-span hook handlers. This hook is called
+            during the ASGI shutdown, after all callables in the 'on_shutdown' list have been called.
+        after_startup: A sequence of life-span hook handlers. This hook is called
+            during the ASGI startup, after all callables in the 'on_startup' list have been called.
+        allowed_hosts: A sequence of allowed hosts, or an :class:`allowed hosts config
+            <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin allowed hosts middleware.
         backend: The async backend to use, options are "asyncio" or "trio".
         backend_options: ``anyio`` options.
-        base_url: URL scheme and domain for test request paths, e.g. 'http://testserver'.
+        base_url: URL scheme and domain for test request paths, e.g. ``http://testserver``.
         before_request: A sync or async function called immediately before calling the route handler.
-            Receives the :class:`Request <starlite.connection.Request>` instance and any non-``None`` return value is
-            used for the response, bypassing the route handler.
-        before_send: A sequence of :class:`before send hook handlers <starlite.types.BeforeMessageSendHookHandler>`.
+            Receives the :class:`Request <.connection.Request>` instance and any non-``None`` return value is used for
+            the response, bypassing the route handler.
+        before_send: A sequence of before send hook handlers.
             This hook is called when the ASGI send function is called.
-        before_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-            This hook is called during the ASGI shutdown, before any 'on_shutdown' hooks are called.
-        before_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-            This hook is called during the ASGI startup, before any 'on_startup' hooks are called.
+        before_shutdown: A sequence of life-span hook handlers.
+            This hook is called during the ASGI shutdown, before any ``on_shutdown`` hooks are called.
+        before_startup: A sequence of life-span hook handlers.
+            This hook is called during the ASGI startup, before any ``on_startup`` hooks are called.
         cache_config: Configures caching behavior of the application.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set this enables the builtin CORS middleware.
         csrf_config: If set this enables the builtin CSRF middleware.
-        dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-        event_emitter_backend: A subclass of :class:`BaseEventEmitterBackend <starlite.events.emitter.BaseEventEmitterBackend>`.
+        dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+        event_emitter_backend: A subclass of :class:`BaseEventEmitterBackend <.events.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
         initial_state: An object from which to initialize the app state.
-        listeners: A sequence of :class:`EventListener <starlite.events.listener.EventListener>`.
-        logging_config: A subclass of :class:`BaseLoggingConfig <starlite.config.logging.BaseLoggingConfig>`.
+        listeners: A sequence of :class:`EventListener <.events.EventListener>`.
+        logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
         middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request.
             This limit is intended to protect from DoS attacks.
-        on_app_init:  A sequence of :class:`OnAppInitHandler <starlite.types.OnAppInitHandler>` instances. Handlers receive
-            an instance of :class:`AppConfig <starlite.config.app.AppConfig>` that will have been initially populated with
-            the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an instance of same. If more
-            than one handler is registered they are called in the order they are provided.
-        on_shutdown: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
+        on_app_init:  A sequence of :class:`OnAppInitHandler <starlite.types.OnAppInitHandler>` instances. Handlers
+            receive an instance of :class:`AppConfig <starlite.config.app.AppConfig>` that will have been initially
+            populated with the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an
+            instance of same. If more than one handler is registered they are called in the order they are provided.
+        on_shutdown: A sequence of ``LifeSpanHandler`` called during
             application shutdown.
-        on_startup: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
-            application startup.
-        openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG <starlite.app.DEFAULT_OPENAPI_CONFIG>`
-        parameters: A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all
-            application paths.
+        on_startup: A sequence of ``LifeSpanHandler`` called during application startup.
+        openapi_config: Defaults to ``DEFAULT_OPENAPI_CONFIG``
+        parameters: A mapping of :func:`Parameter <.params.Parameter>` definitions available to all application paths.
         plugins: Sequence of plugins.
-        request_class: An optional subclass of :class:`Request <starlite.connection.request.Request>` to use for
+        request_class: An optional subclass of :class:`Request <.connection.Request>` to use for
             http connections.
         raise_server_exceptions: Flag for underlying the test client to raise server exceptions instead of
             wrapping them in an HTTP response.
-        response_class: A custom subclass of [starlite.response.Response] to be used as the app's default response.
+        response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
+            response.
         root_path: Path prefix for requests.
-        static_files_config: A sequence of :class:`StaticFilesConfig <starlite.config.StaticFilesConfig>`
+        signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+        state: An optional :class:`State <.datastructures.State>` for application state.
+        static_files_config: A sequence of :class:`StaticFilesConfig <.static_files.StaticFilesConfig>`
         session_config: Configuration for Session Middleware class to create raw session cookies for request to the
             route handlers.
-        template_config: An instance of :class:`TemplateConfig <starlite.config.TemplateConfig>`
-        websocket_class: An optional subclass of :class:`WebSocket <starlite.connection.websocket.WebSocket>` to use for
+        template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
+        websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for
             websocket connections.
 
     Returns:
-        An instance of :class:`TestClient <starlite.testing.TestClient>` with a created app instance.
+        An instance of :class:`TestClient <.testing.TestClient>` with a created app instance.
     """
     route_handlers = () if route_handlers is None else route_handlers
     if is_class_and_subclass(route_handlers, Controller) or not isinstance(route_handlers, Sequence):
         route_handlers = (route_handlers,)
 
     return TestClient[Starlite](
         app=Starlite(
@@ -199,36 +196,37 @@
             after_shutdown=after_shutdown,
             after_startup=after_startup,
             allowed_hosts=allowed_hosts,
             before_request=before_request,
             before_send=before_send,
             before_shutdown=before_shutdown,
             before_startup=before_startup,
-            cache_config=cache_config,
+            response_cache_config=cache_config,
             compression_config=compression_config,
             cors_config=cors_config,
             csrf_config=csrf_config,
             dependencies=dependencies,
             event_emitter_backend=event_emitter_backend,
             exception_handlers=exception_handlers,
             guards=guards,
-            initial_state=initial_state,
             listeners=listeners,
             logging_config=logging_config,
             middleware=middleware,
             multipart_form_part_limit=multipart_form_part_limit,
             on_app_init=on_app_init,
             on_shutdown=on_shutdown,
             on_startup=on_startup,
             openapi_config=openapi_config,
             parameters=parameters,
             plugins=plugins,
             request_class=request_class,
             response_class=response_class,
             route_handlers=route_handlers,
+            signature_namespace=signature_namespace,
+            state=state,
             static_files_config=static_files_config,
             template_config=template_config,
             websocket_class=websocket_class,
         ),
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
@@ -249,23 +247,22 @@
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
     before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
     before_shutdown: OptionalSequence[LifeSpanHookHandler] = None,
     before_startup: OptionalSequence[LifeSpanHookHandler] = None,
-    cache_config: CacheConfig = DEFAULT_CACHE_CONFIG,
+    cache_config: ResponseCacheConfig | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     dependencies: Dependencies | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
     guards: OptionalSequence[Guard] = None,
-    initial_state: InitialStateType | None = None,
     listeners: OptionalSequence[EventListener] = None,
     logging_config: BaseLoggingConfig | None = None,
     middleware: OptionalSequence[Middleware] = None,
     multipart_form_part_limit: int = 1000,
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
     on_shutdown: OptionalSequence[LifeSpanHandler] = None,
     on_startup: OptionalSequence[LifeSpanHandler] = None,
@@ -273,14 +270,16 @@
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[SerializationPluginProtocol] = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_class: ResponseType | None = None,
     root_path: str = "",
     session_config: BaseBackendConfig | None = None,
+    signature_namespace: Mapping[str, Any] | None = None,
+    state: State | None = None,
     static_files_config: OptionalSequence[StaticFilesConfig] = None,
     template_config: TemplateConfig | None = None,
     websocket_class: type[WebSocket] | None = None,
 ) -> AsyncTestClient[Starlite]:
     """Create a Starlite app instance and initializes it.
 
     :class:`TestClient <starlite.testing.TestClient>` with it.
@@ -291,94 +290,91 @@
 
     Examples:
         .. code-block: python
 
             from starlite import get
             from starlite.testing import create_test_client
 
-
             @get("/some-path")
             def my_handler() -> dict[str, str]:
                 return {"hello": "world"}
 
-
             def test_my_handler() -> None:
                 with create_test_client(my_handler) as client:
                     response == client.get("/some-path")
                     assert response.json() == {"hello": "world"}
 
     Args:
         route_handlers: A single handler or a sequence of route handlers, which can include instances of
             :class:`Router <starlite.router.Router>`, subclasses of :class:`Controller <starlite.controller.Controller>` or
             any function decorated by the route handler decorators.
-        after_exception: A sequence of :class:`exception hook handlers <starlite.types.AfterExceptionHookHandler>`.
+        after_exception: A sequence of exception hook handlers.
             This hook is called after an exception occurs. In difference to exception handlers, it is not meant to
             return a response - only to process the exception (e.g. log it, send it to Sentry etc.).
         after_request: A sync or async function executed after the route handler function returned and the response
             object has been resolved. Receives the response object which may be any subclass of
             :class:`Response <starlite.response.Response>`.
         after_response: A sync or async function called after the response has been awaited. It receives the
             :class:`Request <starlite.connection.Request>` object and should not return any values.
-        after_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
+        after_shutdown: A sequence of life-span hook handlers (``LifeSpanHookHandler``).
             This hook is called during the ASGI shutdown, after all callables in the 'on_shutdown' list have been
             called.
-        after_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
-            This hook is called during the ASGI startup, after all callables in the 'on_startup' list have been
-            called.
-        allowed_hosts: A sequence of allowed hosts, or an :class:`allowed hosts config <starlite.config.AllowedHostsConfig>`
-            instance. Enables the builtin allowed hosts middleware.
+        after_startup: A sequence of life-span hook handlers (``LifeSpanHookHandler``). This hook is called during the
+            ASGI startup, after all callables in the 'on_startup' list have been called.
+        allowed_hosts: A sequence of allowed hosts, or an :class:`allowed hosts config
+            <.config.allowed_hosts.AllowedHostsConfig>` instance. Enables the builtin allowed hosts middleware.
         backend: The async backend to use, options are "asyncio" or "trio".
         backend_options: ``anyio`` options.
         base_url: URL scheme and domain for test request paths, e.g. 'http://testserver'.
         before_request: A sync or async function called immediately before calling the route handler.
             Receives the :class:`Request <starlite.connection.Request>` instance and any non-``None`` return value is
             used for the response, bypassing the route handler.
         before_send: A sequence of :class:`before send hook handlers <starlite.types.BeforeMessageSendHookHandler>`.
             This hook is called when the ASGI send function is called.
-        before_shutdown: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
+        before_shutdown: A sequence of life-span hook handlers (``LifeSpanHookHandler``).
             This hook is called during the ASGI shutdown, before any 'on_shutdown' hooks are called.
-        before_startup: A sequence of :class:`life-span hook handlers <starlite.types.LifeSpanHookHandler>`.
+        before_startup: A sequence of life-span hook handlers (``LifeSpanHookHandler``).
             This hook is called during the ASGI startup, before any 'on_startup' hooks are called.
         cache_config: Configures caching behavior of the application.
         compression_config: Configures compression behaviour of the application, this enabled a builtin or user
             defined Compression middleware.
         cors_config: If set this enables the builtin CORS middleware.
         csrf_config: If set this enables the builtin CSRF middleware.
-        dependencies: A string keyed mapping of dependency :class:`Provider <starlite.datastructures.Provide>` instances.
-        event_emitter_backend: A subclass of :class:`BaseEventEmitterBackend <starlite.events.emitter.BaseEventEmitterBackend>`.
+        dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+        event_emitter_backend: A subclass of :class:`BaseEventEmitterBackend <.events.emitter.BaseEventEmitterBackend>`.
         exception_handlers: A mapping of status codes and/or exception types to handler functions.
         guards: A sequence of :class:`Guard <starlite.types.Guard>` callables.
         initial_state: An object from which to initialize the app state.
         listeners: A sequence of :class:`EventListener <starlite.events.listener.EventListener>`.
-        logging_config: A subclass of :class:`BaseLoggingConfig <starlite.config.logging.BaseLoggingConfig>`.
+        logging_config: A subclass of :class:`BaseLoggingConfig <.logging.config.BaseLoggingConfig>`.
         middleware: A sequence of :class:`Middleware <starlite.types.Middleware>`.
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request.
             This limit is intended to protect from DoS attacks.
-        on_app_init:  A sequence of :class:`OnAppInitHandler <starlite.types.OnAppInitHandler>` instances. Handlers receive
-            an instance of :class:`AppConfig <starlite.config.app.AppConfig>` that will have been initially populated with
-            the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an instance of same. If more
-            than one handler is registered they are called in the order they are provided.
-        on_shutdown: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
-            application shutdown.
-        on_startup: A sequence of :class:`LifeSpanHandler <starlite.types.LifeSpanHandler>` called during
-            application startup.
-        openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG <starlite.app.DEFAULT_OPENAPI_CONFIG>`
+        on_app_init:  A sequence of :class:`OnAppInitHandler <starlite.types.OnAppInitHandler>` instances. Handlers
+            receive an instance of :class:`AppConfig <starlite.config.app.AppConfig>` that will have been initially
+            populated with the parameters passed to :class:`Starlite <starlite.app.Starlite>`, and must return an
+            instance of same. If more than one handler is registered they are called in the order they are provided.
+        on_shutdown: A sequence of ``LifeSpanHandler`` called during application shutdown.
+        on_startup: A sequence of ``LifeSpanHandler`` called during application startup.
+        openapi_config: Defaults to ``DEFAULT_OPENAPI_CONFIG``
         parameters: A mapping of :class:`Parameter <starlite.params.Parameter>` definitions available to all
             application paths.
         plugins: Sequence of plugins.
         request_class: An optional subclass of :class:`Request <starlite.connection.request.Request>` to use for
             http connections.
         raise_server_exceptions: Flag for underlying the test client to raise server exceptions instead of
             wrapping them in an HTTP response.
         response_class: A custom subclass of [starlite.response.Response] to be used as the app's default response.
         root_path: Path prefix for requests.
-        static_files_config: A sequence of :class:`StaticFilesConfig <starlite.config.StaticFilesConfig>`
+        state: An optional :class:`State <.datastructures.State>` for application state.
+        static_files_config: A sequence of :class:`StaticFilesConfig <.static_files.StaticFilesConfig>`
         session_config: Configuration for Session Middleware class to create raw session cookies for request to the
             route handlers.
-        template_config: An instance of :class:`TemplateConfig <starlite.config.TemplateConfig>`
+        signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+        template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
         websocket_class: An optional subclass of :class:`WebSocket <starlite.connection.websocket.WebSocket>` to use for
             websocket connections.
 
     Returns:
         An instance of :class:`AsyncTestClient <starlite.testing.AsyncTestClient>` with a created app instance.
     """
     route_handlers = () if route_handlers is None else route_handlers
@@ -393,36 +389,37 @@
             after_shutdown=after_shutdown,
             after_startup=after_startup,
             allowed_hosts=allowed_hosts,
             before_request=before_request,
             before_send=before_send,
             before_shutdown=before_shutdown,
             before_startup=before_startup,
-            cache_config=cache_config,
+            response_cache_config=cache_config,
             compression_config=compression_config,
             cors_config=cors_config,
             csrf_config=csrf_config,
             dependencies=dependencies,
             event_emitter_backend=event_emitter_backend,
             exception_handlers=exception_handlers,
             guards=guards,
-            initial_state=initial_state,
             listeners=listeners,
             logging_config=logging_config,
             middleware=middleware,
             multipart_form_part_limit=multipart_form_part_limit,
             on_app_init=on_app_init,
             on_shutdown=on_shutdown,
             on_startup=on_startup,
             openapi_config=openapi_config,
             parameters=parameters,
             plugins=plugins,
             request_class=request_class,
             response_class=response_class,
             route_handlers=route_handlers,
+            signature_namespace=signature_namespace,
+            state=state,
             static_files_config=static_files_config,
             template_config=template_config,
             websocket_class=websocket_class,
         ),
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
```

### Comparing `starlite-2.0.0a1/starlite/testing/life_span_handler.py` & `starlite-2.0.0a2/starlite/testing/life_span_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from anyio import create_memory_object_stream
 from anyio.streams.stapled import StapledObjectStream
 
 from starlite.testing.client.base import BaseTestClient
 
 if TYPE_CHECKING:
-    from starlite.types import LifeSpanReceiveMessage  # noqa: F401  # nopycln: import
     from starlite.types import (
+        LifeSpanReceiveMessage,  # noqa: F401
         LifeSpanSendMessage,
         LifeSpanShutdownEvent,
         LifeSpanStartupEvent,
     )
 
 T = TypeVar("T", bound=BaseTestClient)
```

### Comparing `starlite-2.0.0a1/starlite/testing/request_factory.py` & `starlite-2.0.0a2/starlite/testing/request_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlencode
 
 from httpx._content import encode_json as httpx_encode_json
 from httpx._content import encode_multipart_data, encode_urlencoded_data
-from httpx._types import FileTypes  # noqa: TC002
 from pydantic import BaseModel
 
 from starlite.app import Starlite
 from starlite.connection import Request
 from starlite.enums import HttpMethod, ParamType, RequestEncodingType, ScopeType
 from starlite.handlers.http_handlers import get
 from starlite.serialization import decode_json, encode_json
 from starlite.types import HTTPScope, RouteHandlerType
 from starlite.types.asgi_types import ASGIVersion
 
 if TYPE_CHECKING:
+    from httpx._types import FileTypes
+
     from starlite.datastructures.cookie import Cookie
     from starlite.handlers.http_handlers import HTTPRouteHandler
 
 
 def _create_default_route_handler() -> HTTPRouteHandler:
     @get("/")
     def _default_route_handler() -> None:
@@ -226,14 +227,15 @@
                 This value can include multiple cookies.
             session: A dictionary of session data.
             user: A value for `request.scope["user"]`
             auth: A value for `request.scope["auth"]`
             request_media_type: The 'Content-Type' header of the request.
             data: A value for the request's body. Can be either a pydantic model instance
                 or a string keyed dictionary.
+            files: A dictionary of files to be sent with the request.
             query_params: A dictionary of values from which the request's query will be generated.
             state: Arbitrary request state.
             path_params: A string keyed dictionary of path parameter values.
             http_version: HTTP version. Defaults to "1.1".
             route_handler: A route handler instance or method. If not provided a default handler is set.
 
         Returns:
@@ -262,15 +264,15 @@
                 encoding_headers, stream = encode_multipart_data(data, files=files or [], boundary=None)  # type: ignore[assignment]
             else:
                 encoding_headers, stream = encode_urlencoded_data(decode_json(encode_json(data)))
             headers.update(encoding_headers)
             body = b""
             for chunk in stream:
                 body += chunk
-            scope["_body"] = body  # type: ignore[typeddict-item]
+            scope["_body"] = body  # type: ignore[typeddict-unknown-key]
         self._create_cookie_header(headers, cookies)
         scope["headers"] = self._build_headers(headers)
         return Request(scope=scope)
 
     def get(
         self,
         path: str = "/",
```

### Comparing `starlite-2.0.0a1/starlite/testing/transport.py` & `starlite-2.0.0a2/starlite/testing/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         WebSocketScope,
     )
 
 
 T = TypeVar("T", bound=Union["AsyncTestClient", "TestClient"])
 
 
-class ConnectionUpgradeException(Exception):
+class ConnectionUpgradeExceptionError(Exception):
     def __init__(self, session: WebSocketTestSession) -> None:
         self.session = session
 
 
 class SendReceiveContext(TypedDict):
     request_complete: bool
     response_complete: Event
@@ -80,25 +80,27 @@
 
         return receive
 
     @staticmethod
     def create_send(request: Request, context: SendReceiveContext) -> Send:
         async def send(message: "Message") -> None:
             if message["type"] == "http.response.start":
-                assert not context["response_started"], 'Received multiple "http.response.start" messages.'  # noqa
+                assert not context[  # noqa: S101
+                    "response_started"
+                ], 'Received multiple "http.response.start" messages.'
                 context["raw_kwargs"]["status_code"] = message["status"]
                 context["raw_kwargs"]["headers"] = [
                     (k.decode("utf-8"), v.decode("utf-8")) for k, v in message.get("headers", [])
                 ]
                 context["response_started"] = True
             elif message["type"] == "http.response.body":
-                assert context[  # noqa
+                assert context[  # noqa: S101
                     "response_started"
                 ], 'Received "http.response.body" without "http.response.start".'
-                assert not context[  # noqa
+                assert not context[  # noqa: S101
                     "response_complete"
                 ].is_set(), 'Received "http.response.body" after response completed.'
                 body = message.get("body", b"")
                 more_body = message.get("more_body", False)
                 if request.method != "HEAD":
                     context["raw_kwargs"]["stream"].write(body)
                 if not more_body:
@@ -144,21 +146,21 @@
     def handle_request(self, request: Request) -> Response:
         scope = self.parse_request(request=request)
         if scope["type"] == "websocket":
             scope.update(
                 subprotocols=[value.strip() for value in request.headers.get("sec-websocket-protocol", "").split(",")]
             )
             session = WebSocketTestSession(client=self.client, scope=cast("WebSocketScope", scope))  # type: ignore [arg-type]
-            raise ConnectionUpgradeException(session)
+            raise ConnectionUpgradeExceptionError(session)
 
         scope.update(method=request.method, http_version="1.1", extensions={"http.response.template": {}})
 
         raw_kwargs: dict[str, Any] = {"stream": BytesIO()}
 
-        try:  # pylint: disable=no-else-return
+        try:
             with self.client.portal() as portal:
                 response_complete = portal.call(Event)
                 context: SendReceiveContext = {
                     "response_complete": response_complete,
                     "request_complete": False,
                     "raw_kwargs": raw_kwargs,
                     "response_started": False,
@@ -167,29 +169,29 @@
                 }
                 portal.call(
                     self.client.app,
                     scope,
                     self.create_receive(request=request, context=context),
                     self.create_send(request=request, context=context),
                 )
-        except BaseException as exc:  # pragma: no cover # pylint: disable=W0703
+        except BaseException as exc:  # noqa: BLE001
             if self.raise_server_exceptions:
                 raise exc
             return Response(
                 status_code=HTTP_500_INTERNAL_SERVER_ERROR, headers=[], stream=ByteStream(b""), request=request
             )
         else:
             if not context["response_started"]:  # pragma: no cover
                 if self.raise_server_exceptions:
-                    assert context["response_started"], "TestClient did not receive any response."  # noqa
+                    assert context["response_started"], "TestClient did not receive any response."  # noqa: S101
                 return Response(
                     status_code=HTTP_500_INTERNAL_SERVER_ERROR, headers=[], stream=ByteStream(b""), request=request
                 )
 
             stream = ByteStream(raw_kwargs.pop("stream", BytesIO()).read())
             response = Response(**raw_kwargs, stream=stream, request=request)
-            setattr(response, "template", context["template"])  # noqa: B010
-            setattr(response, "context", context["context"])  # noqa: B010
+            setattr(response, "template", context["template"])
+            setattr(response, "context", context["context"])
             return response
 
     async def handle_async_request(self, request: "Request") -> "Response":
         return self.handle_request(request=request)
```

### Comparing `starlite-2.0.0a1/starlite/testing/websocket_test_session.py` & `starlite-2.0.0a2/starlite/testing/websocket_test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         WebSocketDisconnectEvent,
         WebSocketReceiveMessage,
         WebSocketScope,
         WebSocketSendMessage,
     )
 
 
+__all__ = ("WebSocketTestSession",)
+
+
 class WebSocketTestSession:
     exit_stack: ExitStack
 
     def __init__(
         self,
         client: TestClient,
         scope: WebSocketScope,
@@ -160,14 +163,15 @@
         self.receive_queue.put(event)
 
     def receive(self) -> WebSocketSendMessage:
         """This is the base receive method.
 
         Notes:
             - you can use one of the other receive methods to extract the data from the message.
+
         Returns:
             A websocket message.
         """
         message = cast("WebSocketSendMessage", self.send_queue.get())
         if isinstance(message, BaseException):
             raise message
 
@@ -175,26 +179,23 @@
             raise WebSocketDisconnect(
                 detail=cast("str", message.get("reason", "")),
                 code=message.get("code", WS_1000_NORMAL_CLOSURE),
             )
         return message
 
     def receive_text(self) -> str:
-        """
-
-        Returns:
-            A string value.
+        """Returns:
+        A string value.
         """
         message = self.receive()
         return cast("str", message.get("text", ""))
 
     def receive_bytes(self) -> bytes:
-        """
-        Returns:
-            A bytes string value.
+        """Returns:
+        A bytes string value.
         """
         message = self.receive()
         return cast("bytes", message.get("bytes", b""))
 
     def receive_json(self, mode: Literal["text", "binary"] = "text") -> Any:
         """Receives JSON.
```

### Comparing `starlite-2.0.0a1/starlite/types/__init__.py` & `starlite-2.0.0a2/starlite/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     WebSocketReceiveMessage,
     WebSocketResponseBodyEvent,
     WebSocketResponseStartEvent,
     WebSocketScope,
     WebSocketSendEvent,
     WebSocketSendMessage,
 )
-from .builtin_types import DataclassClass, DataclassClassOrInstance, TypedDictClass
+from .builtin_types import TypedDictClass
 from .callable_types import (
     AfterExceptionHookHandler,
     AfterRequestHookHandler,
     AfterResponseHookHandler,
     AnyCallable,
     AnyGenerator,
     AsyncAnyCallable,
@@ -59,15 +59,14 @@
     OnAppInitHandler,
     OperationIDCreator,
     Serializer,
 )
 from .composite_types import (
     Dependencies,
     ExceptionHandlersMap,
-    InitialStateType,
     MaybePartial,
     Middleware,
     ParametersMap,
     PathType,
     ResponseCookies,
     ResponseHeaders,
     Scopes,
@@ -96,16 +95,14 @@
     "AnyIOBackend",
     "AsyncAnyCallable",
     "BaseScope",
     "BeforeMessageSendHookHandler",
     "BeforeRequestHookHandler",
     "CacheKeyBuilder",
     "ControllerRouterHandler",
-    "DataclassClass",
-    "DataclassClassOrInstance",
     "DataclassProtocol",
     "Dependencies",
     "Empty",
     "EmptyType",
     "ExceptionHandler",
     "ExceptionHandlersMap",
     "FileInfo",
@@ -116,15 +113,14 @@
     "HTTPReceiveMessage",
     "HTTPRequestEvent",
     "HTTPResponseBodyEvent",
     "HTTPResponseStartEvent",
     "HTTPScope",
     "HTTPSendMessage",
     "HTTPServerPushEvent",
-    "InitialStateType",
     "LifeSpanHandler",
     "LifeSpanHookHandler",
     "LifeSpanReceive",
     "LifeSpanReceiveMessage",
     "LifeSpanScope",
     "LifeSpanSend",
     "LifeSpanSendMessage",
```

### Comparing `starlite-2.0.0a1/starlite/types/asgi_types.py` & `starlite-2.0.0a2/starlite/types/asgi_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,20 +43,67 @@
     Union,
 )
 
 from typing_extensions import TypedDict
 
 from starlite.enums import ScopeType
 
+__all__ = (
+    "ASGIApp",
+    "ASGIVersion",
+    "BaseScope",
+    "HeaderScope",
+    "HTTPDisconnectEvent",
+    "HTTPReceiveMessage",
+    "HTTPRequestEvent",
+    "HTTPResponseBodyEvent",
+    "HTTPResponseStartEvent",
+    "HTTPScope",
+    "HTTPSendMessage",
+    "HTTPServerPushEvent",
+    "LifeSpanReceive",
+    "LifeSpanReceiveMessage",
+    "LifeSpanScope",
+    "LifeSpanSend",
+    "LifeSpanSendMessage",
+    "LifeSpanShutdownCompleteEvent",
+    "LifeSpanShutdownEvent",
+    "LifeSpanShutdownFailedEvent",
+    "LifeSpanStartupCompleteEvent",
+    "LifeSpanStartupEvent",
+    "LifeSpanStartupFailedEvent",
+    "Message",
+    "Method",
+    "RawHeaders",
+    "RawHeadersList",
+    "Receive",
+    "ReceiveMessage",
+    "Scope",
+    "ScopeSession",
+    "Send",
+    "WebSocketAcceptEvent",
+    "WebSocketCloseEvent",
+    "WebSocketConnectEvent",
+    "WebSocketDisconnectEvent",
+    "WebSocketReceiveEvent",
+    "WebSocketReceiveMessage",
+    "WebSocketResponseBodyEvent",
+    "WebSocketResponseStartEvent",
+    "WebSocketScope",
+    "WebSocketSendEvent",
+    "WebSocketSendMessage",
+)
+
+
 if TYPE_CHECKING:
     from pydantic import BaseModel
 
     from starlite.app import Starlite
+    from starlite.types.empty import EmptyType
 
-    from .empty import EmptyType
     from .internal_types import RouteHandlerType
 
 Method = Literal["GET", "POST", "DELETE", "PATCH", "PUT", "HEAD", "TRACE", "OPTIONS"]
 ScopeSession = Optional[Union["EmptyType", Dict[str, Any], "BaseModel"]]
 
 
 class ASGIVersion(TypedDict):
```

### Comparing `starlite-2.0.0a1/starlite/types/builtin_types.py` & `starlite-2.0.0a2/starlite/types/builtin_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import sys
 from typing import TYPE_CHECKING, Type, Union
 
-from typing_extensions import TypeAlias  # noqa: TC002
+from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
     from typing_extensions import _TypedDictMeta  # type: ignore
 
-    from starlite.types.protocols import DataclassProtocol
-
 
 if sys.version_info >= (3, 10):
     from types import NoneType as _NoneType
     from types import UnionType
 
     NoneType = _NoneType  # type: ignore[valid-type]
 
     UNION_TYPES = {UnionType, Union}
 else:  # pragma: no cover
     UNION_TYPES = {Union}
     NoneType = type(None)
 
-DataclassClass: TypeAlias = "Type[DataclassProtocol]"
-DataclassClassOrInstance: TypeAlias = "Union[DataclassClass, DataclassProtocol]"
 TypedDictClass: TypeAlias = "Type[_TypedDictMeta]"
```

### Comparing `starlite-2.0.0a1/starlite/types/callable_types.py` & `starlite-2.0.0a2/starlite/types/callable_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,20 +38,19 @@
 AfterRequestHookHandler = Union[
     Callable[[ASGIApp], SyncOrAsyncUnion[ASGIApp]], Callable[[Response], SyncOrAsyncUnion[Response]]
 ]
 AfterResponseHookHandler = Callable[[Request], SyncOrAsyncUnion[None]]
 AsyncAnyCallable = Callable[..., Awaitable[Any]]
 AnyCallable = Callable[..., Any]
 AnyGenerator = Union[Generator[Any, Any, Any], AsyncGenerator[Any, Any]]
-BeforeMessageSendHookHandler = Union[
-    Callable[[Message, State, Scope], SyncOrAsyncUnion[None]], Callable[[Message, State], SyncOrAsyncUnion[None]]
-]
+BeforeMessageSendHookHandler = Callable[[Message, State, Scope], SyncOrAsyncUnion[None]]
 BeforeRequestHookHandler = Callable[[Request], Union[Any, Awaitable[Any]]]
 CacheKeyBuilder = Callable[[Request], str]
 ExceptionHandler = Callable[[Request, ExceptionT], Response]
+ExceptionLoggingHandler = Callable[[Logger, Scope, List[str]], None]
+GetLogger = Callable[..., Logger]
 Guard = Callable[[ASGIConnection, BaseRouteHandler], SyncOrAsyncUnion[None]]
 LifeSpanHandler = Union[Callable[[], SyncOrAsyncUnion[Any]], Callable[[State], SyncOrAsyncUnion[Any]]]
 LifeSpanHookHandler = Callable[[StarliteType], SyncOrAsyncUnion[None]]
 OnAppInitHandler = Callable[[AppConfig], AppConfig]
-Serializer = Callable[[Any], Any]
-GetLogger = Callable[..., Logger]
 OperationIDCreator = Callable[[HTTPRouteHandler, Method, List[Union[str, PathParameterDefinition]]], str]
+Serializer = Callable[[Any], Any]
```

### Comparing `starlite-2.0.0a1/starlite/types/composite_types.py` & `starlite-2.0.0a2/starlite/types/composite_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ResponseHeader = Any
 
 T = TypeVar("T")
 
 
 Dependencies = Mapping[str, Provide]
 ExceptionHandlersMap = Mapping[Union[int, Type[Exception]], ExceptionHandler]
-InitialStateType = Mapping[str, Any]
 MaybePartial = Union[T, partial]
 Middleware = Union[
     Callable[..., ASGIApp], DefineMiddleware, Iterator[Tuple[ASGIApp, Dict[str, Any]]], Type[MiddlewareProtocol]
 ]
 ParametersMap = Mapping[str, ParameterKwarg]
 PathType = Union[Path, PathLike, str]
 ResponseCookies = Union[Sequence[Cookie], Mapping[str, str]]
```

### Comparing `starlite-2.0.0a1/starlite/types/file_types.py` & `starlite-2.0.0a2/starlite/types/file_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     Protocol,
     Union,
     overload,
 )
 
 from typing_extensions import NotRequired, TypedDict
 
+__all__ = ("FileInfo", "FileSystemProtocol")
+
+
 if TYPE_CHECKING:
     from _typeshed import OpenBinaryMode, OpenTextMode
     from anyio import AsyncFile
 
     from starlite.types.composite_types import PathType
 
 
@@ -49,15 +52,15 @@
     """User ID of owner."""
 
 
 class FileSystemProtocol(Protocol):
     """Base protocol used to interact with a file-system.
 
     This protocol is commensurable with the file systems
-    exported by the [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) library.
+    exported by the `fsspec <https://filesystem-spec.readthedocs.io/en/latest/>` library.
     """
 
     def info(self, path: "PathType", **kwargs: Any) -> Union[FileInfo, Awaitable[FileInfo]]:
         """Retrieve information about a given file path.
 
         Args:
             path: A file path.
```

### Comparing `starlite-2.0.0a1/starlite/types/internal_types.py` & `starlite-2.0.0a2/starlite/types/internal_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,24 @@
     Optional,
     Type,
     Union,
 )
 
 from starlite.types import Method
 
+__all__ = (
+    "PathParameterDefinition",
+    "ControllerRouterHandler",
+    "ReservedKwargs",
+    "ResponseType",
+    "RouteHandlerMapItem",
+    "RouteHandlerType",
+)
+
+
 if TYPE_CHECKING:
     from starlite.app import Starlite
     from starlite.controller import Controller
     from starlite.handlers.asgi_handlers import ASGIRouteHandler
     from starlite.handlers.http_handlers import HTTPRouteHandler
     from starlite.handlers.websocket_handlers import WebsocketRouteHandler
     from starlite.response import Response
```

### Comparing `starlite-2.0.0a1/starlite/types/protocols.py` & `starlite-2.0.0a2/starlite/types/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Dict, Protocol, runtime_checkable
+from typing import Any, ClassVar, Dict, Protocol, runtime_checkable
+
+__all__ = ("DataclassProtocol", "Logger")
 
 
 class Logger(Protocol):  # pragma: no cover
     """Logger protocol."""
 
     def debug(self, event: str, *args: Any, **kwargs: Any) -> Any:
         """Output a log message at 'DEBUG' level.
@@ -78,8 +80,8 @@
         """
 
 
 @runtime_checkable
 class DataclassProtocol(Protocol):
     """Protocol for instance checking dataclasses"""
 
-    __dataclass_fields__: Dict[str, Any]
+    __dataclass_fields__: ClassVar[Dict[str, Any]]
```

### Comparing `starlite-2.0.0a1/starlite/utils/__init__.py` & `starlite-2.0.0a2/starlite/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 from .helpers import Ref, get_enum_string_value, get_name
 from .path import join_paths, normalize_path
 from .predicates import (
     is_any,
     is_class_and_subclass,
     is_dataclass_class,
-    is_dataclass_class_or_instance,
     is_mapping,
     is_optional_union,
+    is_pydantic_model_class,
+    is_pydantic_model_instance,
     is_typed_dict,
     is_union,
 )
 from .pydantic import (
     convert_dataclass_to_model,
     convert_typeddict_to_model,
     create_parsed_model_field,
@@ -48,19 +49,20 @@
     "get_name",
     "get_serializer_from_scope",
     "get_starlite_scope_state",
     "is_any",
     "is_async_callable",
     "is_class_and_subclass",
     "is_dataclass_class",
-    "is_dataclass_class_or_instance",
+    "is_mapping",
     "is_optional_union",
+    "is_pydantic_model_class",
+    "is_pydantic_model_instance",
     "is_typed_dict",
     "is_union",
-    "is_mapping",
     "join_paths",
     "make_non_optional_union",
     "normalize_path",
     "set_starlite_scope_state",
     "unique",
     "warn_deprecation",
 )
```

### Comparing `starlite-2.0.0a1/starlite/utils/dataclass.py` & `starlite-2.0.0a2/starlite/utils/dataclass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Iterable, cast
 
+__all__ = ("extract_dataclass_fields",)
+
+
 if TYPE_CHECKING:
     from starlite.types import DataclassProtocol
 
 
 def extract_dataclass_fields(
     dt: Any, exclude_none: bool = False, include: Iterable[str] | None = None
 ) -> tuple[tuple[str, Any], ...]:
     """Extract dataclass fields. Unlike the 'asdict' method exports by the stlib, this function does not pickle values.
 
-    :param dt: A dataclass instance.
-    :param exclude_none: Whether to exclude None values.
-    :param include: An iterable of fields to include.
-    :return: A tuple of key/value pairs.
+    Args:
+        dt: A dataclass instance.
+        exclude_none: Whether to exclude None values.
+        include: An iterable of fields to include.
+
+    Returns:
+        A tuple of key/value pairs.
     """
     return tuple(
         (field_name, getattr(dt, field_name))
         for field_name in cast("DataclassProtocol", dt).__dataclass_fields__
         if (not exclude_none or getattr(dt, field_name) is not None)
         and ((include is not None and field_name in include) or include is None)
     )
```

### Comparing `starlite-2.0.0a1/starlite/utils/deprecation.py` & `starlite-2.0.0a2/starlite/utils/deprecation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import inspect
 from functools import wraps
 from typing import Callable, Literal, TypeVar
 from warnings import warn
 
 from typing_extensions import ParamSpec
 
+__all__ = ("deprecated", "warn_deprecation")
+
+
 T = TypeVar("T")
 P = ParamSpec("P")
 DeprecatedKind = Literal["function", "method", "classmethod", "attribute", "property", "class", "parameter", "import"]
 
 
 def warn_deprecation(
     version: str,
@@ -55,15 +58,15 @@
 
     if info:
         parts.append(info)
 
     text = ". ".join(parts)
     warning_class = PendingDeprecationWarning if pending else DeprecationWarning
 
-    warn(text, warning_class)
+    warn(text, warning_class, stacklevel=1)
 
 
 def deprecated(
     version: str,
     *,
     removal_in: str | None = None,
     alternative: str | None = None,
```

### Comparing `starlite-2.0.0a1/starlite/utils/helpers.py` & `starlite-2.0.0a2/starlite/utils/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, cast
 
+__all__ = ("Ref", "get_enum_string_value", "get_name", "unwrap_partial")
+
+
 T = TypeVar("T")
 
 if TYPE_CHECKING:
     from starlite.types import MaybePartial
 
 
 def get_name(value: Any) -> str:
```

### Comparing `starlite-2.0.0a1/starlite/utils/path.py` & `starlite-2.0.0a2/starlite/utils/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 import re
 from typing import Iterable
 
+__all__ = ("join_paths", "normalize_path")
+
+
 multi_slash_pattern = re.compile("//+")
 
 
 def normalize_path(path: str) -> str:
     """Normalize a given path by ensuring it starts with a slash and does not end with a slash.
 
     Args:
```

### Comparing `starlite-2.0.0a1/starlite/utils/predicates.py` & `starlite-2.0.0a2/starlite/utils/predicates.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,63 +15,79 @@
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
+    Type,
     TypeVar,
 )
 
 from typing_extensions import (
     Annotated,
     NotRequired,
     ParamSpec,
     Required,
     TypeGuard,
     get_args,
     get_origin,
     is_typeddict,
 )
 
+from starlite.types import DataclassProtocol, Empty
 from starlite.types.builtin_types import UNION_TYPES, NoneType
 
 if TYPE_CHECKING:
     from starlite.types.builtin_types import (
-        DataclassClass,
-        DataclassClassOrInstance,
         TypedDictClass,
     )
 
+try:
+    from pydantic import BaseModel
+except ImportError:  # pragma: no cover
+    BaseModel = Empty  # type: ignore
+
+
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def _get_origin(annotation: Any) -> Any:
-    origin = get_origin(annotation)
-    return origin if origin not in (Annotated, Required, NotRequired) else get_args(annotation)[0]
+def get_origin_or_inner_type(annotation: Any) -> Any:
+    """Get origin or unwrap it. Returns None for non-generic types.
+
+    Args:
+        annotation: A type annotation.
+
+    Returns:
+        Any type.
+    """
+
+    if origin := get_origin(annotation):
+        return origin if origin not in (Annotated, Required, NotRequired) else get_args(annotation)[0]
+    return None
 
 
-def is_class_and_subclass(value: Any, t_type: type[T]) -> TypeGuard[type[T]]:
+def is_class_and_subclass(annotation: Any, t_type: type[T]) -> TypeGuard[type[T]]:
     """Return ``True`` if ``value`` is a ``class`` and is a subtype of ``t_type``.
 
     See https://github.com/starlite-api/starlite/issues/367
 
     Args:
-        value: The value to check if is class and subclass of ``t_type``.
+        annotation: The value to check if is class and subclass of ``t_type``.
         t_type: Type used for :func:`issubclass` check of ``value``
 
     Returns:
         bool
     """
-    origin = _get_origin(value)
-    if not origin and not isclass(value):
+    origin = get_origin_or_inner_type(annotation)
+    if not origin and not isclass(annotation):
         return False
     try:
-        return issubclass(origin or value, t_type)
+        return issubclass(origin or annotation, t_type)
     except TypeError:  # pragma: no cover
         return False
 
 
 def is_generic(annotation: Any) -> bool:
     """Given a type annotation determine if the annotation is a generic class.
 
@@ -89,28 +105,28 @@
 
     Args:
     annotation: A type.
 
     Returns:
         A typeguard determining whether the type can be cast as :class:`Mapping <typing.Mapping>`.
     """
-    _type = _get_origin(annotation) or annotation
+    _type = get_origin_or_inner_type(annotation) or annotation
     return isclass(_type) and issubclass(_type, (dict, defaultdict, DefaultDict, Mapping))
 
 
 def is_non_string_iterable(annotation: Any) -> TypeGuard[Iterable[Any]]:
     """Given a type annotation determine if the annotation is an iterable.
 
     Args:
     annotation: A type.
 
     Returns:
         A typeguard determining whether the type can be cast as :class:`Iterable <typing.Iterable>` that is not a string.
     """
-    origin = _get_origin(annotation)
+    origin = get_origin_or_inner_type(annotation)
     if not origin and not isclass(annotation):
         return False
     try:
         return not issubclass(origin or annotation, (str, bytes)) and (
             issubclass(origin or annotation, (Iterable, CollectionsIterable, Dict, dict, Mapping))
             or is_non_string_sequence(annotation)
         )
@@ -123,15 +139,15 @@
 
     Args:
     annotation: A type.
 
     Returns:
         A typeguard determining whether the type can be cast as :class`Sequence <typing.Sequence>` that is not a string.
     """
-    origin = _get_origin(annotation)
+    origin = get_origin_or_inner_type(annotation)
     if not origin and not isclass(annotation):
         return False
     try:
         return not issubclass(origin or annotation, (str, bytes)) and issubclass(
             origin or annotation,
             (  # type: ignore
                 Tuple,
@@ -150,81 +166,101 @@
     except TypeError:  # pragma: no cover
         return False
 
 
 def is_any(annotation: Any) -> TypeGuard[Any]:
     """Given a type annotation determine if the annotation is Any.
 
-        Args:
+    Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is :data:`Any <typing.Any>`.
     """
     return (
         annotation is Any
         or getattr(annotation, "_name", "") == "typing.Any"
-        or (get_origin(annotation) in UNION_TYPES and Any in get_args(annotation))
+        or (get_origin_or_inner_type(annotation) in UNION_TYPES and Any in get_args(annotation))
     )
 
 
 def is_union(annotation: Any) -> bool:
     """Given a type annotation determine if the annotation infers an optional union.
 
     Args:
         annotation: A type.
 
     Returns:
         A boolean determining whether the type is :data:`Union typing.Union>`.
     """
-    return _get_origin(annotation) in UNION_TYPES
+    return get_origin_or_inner_type(annotation) in UNION_TYPES
 
 
 def is_optional_union(annotation: Any) -> TypeGuard[Any | None]:
     """Given a type annotation determine if the annotation infers an optional union.
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is :data:`Union typing.Union>` with a
             None value or :data:`Optional <typing.Optional>` which is equivalent.
     """
-    origin = _get_origin(annotation)
-    return origin is Optional or (get_origin(annotation) in UNION_TYPES and NoneType in get_args(annotation))
+    origin = get_origin_or_inner_type(annotation)
+    return origin is Optional or (
+        get_origin_or_inner_type(annotation) in UNION_TYPES and NoneType in get_args(annotation)
+    )
 
 
-def is_dataclass_class(value: Any) -> TypeGuard[DataclassClass]:
-    """Wrap :func:`is_dataclass <dataclasses.is_dataclass>` in a :data:`typing.TypeGuard`, narrowing to type only, not
-        instance.
+def is_dataclass_class(annotation: Any) -> TypeGuard[type[DataclassProtocol]]:
+    """Wrap :func:`is_dataclass <dataclasses.is_dataclass>` in a :data:`typing.TypeGuard`.
 
     Args:
-        value: tested to determine if type of :class:`dataclasses.dataclass`.
+        annotation: tested to determine if instance or type of :class:`dataclasses.dataclass`.
 
     Returns:
-        ``True`` if ``value`` is a ``dataclass`` type.
+        ``True`` if instance or type of ``dataclass``.
     """
-    return is_dataclass(value) and isinstance(value, type)
+    try:
+        return isclass(annotation) and is_dataclass(annotation)
+    except TypeError:  # pragma: no cover
+        return False
 
 
-def is_dataclass_class_or_instance(value: Any) -> TypeGuard[DataclassClassOrInstance]:
-    """Wrap :func:`is_dataclass <dataclasses.is_dataclass>` in a :data:`typing.TypeGuard`.
+def is_typed_dict(annotation: Any) -> TypeGuard[TypedDictClass]:
+    """Wrap :func:`typing.is_typeddict` in a :data:`typing.TypeGuard`.
 
     Args:
-        value: tested to determine if instance or type of :class:`dataclasses.dataclass`.
+        annotation: tested to determine if instance or type of :class:`typing.TypedDict`.
 
     Returns:
-        ``True`` if instance or type of ``dataclass``.
+        ``True`` if instance or type of ``TypedDict``.
     """
-    return is_dataclass(value)
+    return is_typeddict(annotation)
 
 
-def is_typed_dict(value: Any) -> TypeGuard[TypedDictClass]:
-    """Wrap :func:`typing.is_typeddict` in a :data:`typing.TypeGuard`.
+def is_pydantic_model_class(annotation: Any) -> "TypeGuard[Type[BaseModel]]":  # pyright: ignore
+    """Given a type annotation determine if the annotation is a subclass of pydantic's BaseModel.
 
     Args:
-        value: tested to determine if instance or type of :class:`typing.TypedDict`.
+        annotation: A type.
 
     Returns:
-        ``True`` if instance or type of ``TypedDict``.
+        A typeguard determining whether the type is :data:`BaseModel pydantic.BaseModel>`.
+    """
+    if BaseModel is not Empty:  # type: ignore[comparison-overlap]
+        return is_class_and_subclass(annotation, BaseModel)
+    return False  # pragma: no cover
+
+
+def is_pydantic_model_instance(annotation: Any) -> "TypeGuard[BaseModel]":  # pyright: ignore
+    """Given a type annotation determine if the annotation is an instance of pydantic's BaseModel.
+
+    Args:
+        annotation: A type.
+
+    Returns:
+        A typeguard determining whether the type is :data:`BaseModel pydantic.BaseModel>`.
     """
-    return is_typeddict(value)
+    if BaseModel is not Empty:  # type: ignore[comparison-overlap]
+        return isinstance(annotation, BaseModel)
+    return False  # pragma: no cover
```

### Comparing `starlite-2.0.0a1/starlite/utils/scope.py` & `starlite-2.0.0a2/starlite/utils/scope.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from starlite.constants import SCOPE_STATE_NAMESPACE
 
+__all__ = ("get_serializer_from_scope", "get_starlite_scope_state", "set_starlite_scope_state")
+
+
 if TYPE_CHECKING:
     from starlite.types import Scope, Serializer
 
 
 def get_serializer_from_scope(scope: Scope) -> Serializer | None:
     """Return a serializer given a scope object.
```

### Comparing `starlite-2.0.0a1/starlite/utils/sequence.py` & `starlite-2.0.0a2/starlite/utils/sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable, Iterable, TypeVar
 
+__all__ = ("find_index", "unique")
+
+
 T = TypeVar("T")
 
 
 def find_index(target_list: list[T], predicate: Callable[[T], bool]) -> int:
     """Find element in list given a key and value.
 
     List elements can be dicts or classes
```

### Comparing `starlite-2.0.0a1/starlite/utils/sync.py` & `starlite-2.0.0a2/starlite/utils/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 )
 
 from anyio.to_thread import run_sync
 from typing_extensions import ParamSpec, TypeGuard
 
 from starlite.utils.helpers import Ref
 
+__all__ = ("AsyncCallable", "AsyncIteratorWrapper", "as_async_callable_list", "async_partial", "is_async_callable")
+
+
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def is_async_callable(value: Callable[P, T]) -> TypeGuard[Callable[P, Awaitable[T]]]:
     """Extend :func:`asyncio.iscoroutinefunction` to additionally detect async :func:`functools.partial` objects and
     class instances with ``async def __call__()`` defined.
```

### Comparing `starlite-2.0.0a1/starlite/utils/types.py` & `starlite-2.0.0a2/starlite/utils/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 )
 
 from typing_extensions import TypeGuard, get_args
 
 from starlite.types.builtin_types import NoneType
 from starlite.utils.predicates import is_class_and_subclass
 
+__all__ = ("annotation_is_iterable_of_type", "make_non_optional_union")
+
+
 T = TypeVar("T")
 UnionT = TypeVar("UnionT", bound="Union")
 
 tuple_types_regex = re.compile(
     "^"
     + "|".join(
         [*[repr(x) for x in (List, Sequence, Iterable, Iterator, Tuple, Deque)], "tuple", "list", "collections.deque"]
```

### Comparing `starlite-2.0.0a1/PKG-INFO` & `starlite-2.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: starlite
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Performant, light and flexible ASGI API Framework
-Home-page: https://github.com/starlite-api/starlite
+Home-page: https://starliteproject.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,starlite,framework,websocket
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
 Maintainer-email: nhirschfeld@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -49,29 +49,28 @@
 Requires-Dist: cryptography ; extra == "cryptography" or extra == "jwt" or extra == "full"
 Requires-Dist: fast-query-parsers
 Requires-Dist: httpx (>=0.22)
 Requires-Dist: importlib-metadata ; python_version < "3.10"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: mako (>=1.2.4)
-Requires-Dist: msgspec (>=0.11.0)
+Requires-Dist: msgspec
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
-Requires-Dist: picologging ; extra == "picologging" or extra == "standard" or extra == "full"
+Requires-Dist: picologging ; extra == "picologging" or extra == "full"
 Requires-Dist: pydantic
 Requires-Dist: pydantic-factories
-Requires-Dist: pydantic-openapi-schema (>=1.5.0)
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
-Requires-Dist: sqlalchemy (>=2.0,<3.0) ; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy (>=2.0.4) ; extra == "sqlalchemy"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
 Requires-Dist: typing-extensions
-Project-URL: Documentation, https://starlite-api.github.io/starlite
+Project-URL: Documentation, https://docs.starliteproject.dev/
 Project-URL: Repository, https://github.com/starlite-api/starlite
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
   <img src="artwork/SVG/logo-banner-inline-light.svg#gh-light-mode-only" alt="Starlite Logo - Light" width="100%" height="auto" />
   <img src="artwork/SVG/logo-banner-inline-dark.svg#gh-dark-mode-only" alt="Starlite Logo - Dark" width="100%" height="auto" />
@@ -89,15 +88,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-85-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-89-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/starlite?label=r%2FStarlite&logo=reddit)](https://reddit.com/r/starlite)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#starlitespace:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://itnext.io/introducing-starlite-3928adaa19ae)
@@ -114,14 +113,21 @@
 
 ## Installation
 
 ```shell
 pip install starlite
 ```
 
+**Starlite 2.0 is coming out soon**, bringing many new features and improvements.
+You can check out the alpha version by instead running
+
+```shell
+pip install starlite==2.0.0alpha1
+```
+
 ## Quick Start
 
 ```python
 from starlite import Starlite, get
 
 
 @get("/")
@@ -238,17 +244,14 @@
     @delete(path="/{user_id:uuid}")
     async def delete_user(self, user_id: UUID4) -> None:
         ...
 ```
 
 ### Data Parsing, Type Hints and Pydantic
 
-One key difference between Starlite and Starlette/FastAPI is in parsing of form data and query parameters- Starlite
-supports mixed form data and has faster and better query parameter parsing.
-
 Starlite is rigorously typed, and it enforces typing. For example, if you forget to type a return value for a route
 handler, an exception will be raised. The reason for this is that Starlite uses typing data to generate OpenAPI specs,
 as well as to validate and parse data. Thus typing is absolutely essential to the framework.
 
 Furthermore, Starlite allows extending its support using plugins.
 
 ### Plugin System, ORM support and DTOs
@@ -259,17 +262,16 @@
 handlers.
 
 Starlite also supports the programmatic creation of DTOs with a `DTOFactory` class, which also supports the use of
 plugins.
 
 ### OpenAPI
 
-Starlite has custom logic to generate OpenAPI 3.1.0 schema, the latest version. The schema generated by Starlite is
-significantly more complete and more correct than those generated by FastAPI, and they include optional generation of
-examples using the `pydantic-factories` library.
+Starlite has custom logic to generate OpenAPI 3.1.0 schema, include optional generation of examples using the
+`pydantic-factories` library.
 
 #### ReDoc, Swagger-UI and Stoplight Elements API Documentation
 
 Starlite serves the documentation from the generated OpenAPI schema with:
 
 - [ReDoc](https://redoc.ly/)
 - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
@@ -434,15 +436,15 @@
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ottermata"><img src="https://avatars.githubusercontent.com/u/9451844?v=4?s=100" width="100px;" alt="Christopher Krause"/><br /><sub><b>Christopher Krause</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ottermata" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/starlite-api/starlite/commits?author=smithk86" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/starlite-api/starlite/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ste-pool" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/starlite-api/starlite/commits?author=Alc-Alc" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://asomethings.com"><img src="https://avatars.githubusercontent.com/u/16171942?v=4?s=100" width="100px;" alt="asomethings"/><br /><sub><b>asomethings</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=asomethings" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/garburator"><img src="https://avatars.githubusercontent.com/u/14207857?v=4?s=100" width="100px;" alt="Garry Bullock"/><br /><sub><b>Garry Bullock</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=garburator" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NiclasHaderer"><img src="https://avatars.githubusercontent.com/u/109728711?v=4?s=100" width="100px;" alt="Niclas Haderer"/><br /><sub><b>Niclas Haderer</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=NiclasHaderer" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dialvarezs"><img src="https://avatars.githubusercontent.com/u/13831919?v=4?s=100" width="100px;" alt="Diego Alvarez"/><br /><sub><b>Diego Alvarez</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=dialvarezs" title="Documentation">📖</a> <a href="https://github.com/starlite-api/starlite/commits?author=dialvarezs" title="Code">💻</a></td>
@@ -465,14 +467,18 @@
       <td align="center" valign="top" width="14.28%"><a href="http://wardpearce.com"><img src="https://avatars.githubusercontent.com/u/27844174?v=4?s=100" width="100px;" alt="Ward"/><br /><sub><b>Ward</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3AWardPearce" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://knowsuchagency.com"><img src="https://avatars.githubusercontent.com/u/11974795?v=4?s=100" width="100px;" alt="Stephan Fitzpatrick"/><br /><sub><b>Stephan Fitzpatrick</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/issues?q=author%3Aknowsuchagency" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://codepen.io/ekeric13/"><img src="https://avatars.githubusercontent.com/u/6489651?v=4?s=100" width="100px;" alt="Eric Kennedy"/><br /><sub><b>Eric Kennedy</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=ekeric13" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wassafshahzad"><img src="https://avatars.githubusercontent.com/u/25094157?v=4?s=100" width="100px;" alt="wassaf shahzad"/><br /><sub><b>wassaf shahzad</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=wassafshahzad" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://nilsso.github.io"><img src="https://avatars.githubusercontent.com/u/567181?v=4?s=100" width="100px;" alt="Nils Olsson"/><br /><sub><b>Nils Olsson</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=nilsso" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://rileychase.net"><img src="https://avatars.githubusercontent.com/u/1491530?v=4?s=100" width="100px;" alt="Riley Chase"/><br /><sub><b>Riley Chase</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Nadock" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://gh.arielle.codes"><img src="https://avatars.githubusercontent.com/u/71233171?v=4?s=100" width="100px;" alt="arl"/><br /><sub><b>arl</b></sub></a><br /><a href="#maintenance-onerandomusername" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=Galdanwing" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/starlite-api/starlite/commits?author=zoni" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

