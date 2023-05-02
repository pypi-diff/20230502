# Comparing `tmp/frontrunner-sdk-0.1.1.tar.gz` & `tmp/frontrunner-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontrunner-sdk-0.1.1.tar", last modified: Tue Apr 25 21:21:50 2023, max compression
+gzip compressed data, was "frontrunner-sdk-0.1.2.tar", last modified: Tue May  2 00:27:15 2023, max compression
```

## Comparing `frontrunner-sdk-0.1.1.tar` & `frontrunner-sdk-0.1.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.159138 frontrunner-sdk-0.1.1/frontrunner_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_light_client_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/openapi_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/find_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_leagues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/cancel_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_account_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_order_books.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/chained.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/frontrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/injective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/paginators.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_external_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/cancel_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.159138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.578106 frontrunner-sdk-0.1.2/frontrunner_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_light_client_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/clients/openapi_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/find_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_leagues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sport_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/cancel_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/create_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/create_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_account_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_order_books.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/chained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/config/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/facades/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/facades/frontrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/facades/injective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/frontrunner_sdk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/logging/log_external_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/logging/log_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/frontrunner_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/models/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/models/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.578106 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/frontrunner_sdk/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:27:15.582106 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 00:27:15.000000 frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:27:15.586106 frontrunner-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-02 00:27:14.000000 frontrunner-sdk-0.1.2/setup.py
```

### Comparing `frontrunner-sdk-0.1.1/PKG-INFO` & `frontrunner-sdk-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontrunner-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Frontrunner SDK
 Home-page: https://github.com/GetFrontrunner/frontrunner-sdk
 Author: Frontrunner
 Author-email: support@getfrontrunner.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -131,20 +131,22 @@
 ```sh
 pants fmt ::
 pants fix ::
 ```
 
 ### Local Testing via REPL
 
-To get a Python shell to test code, run...
+To get a Python shell to test code, [comment out the `python_distribution` target][pants-16985] in `/BUILD`. Then run...
 
 ```sh
 pants repl ::
 ```
 
+[pants-16985]: https://github.com/pantsbuild/pants/issues/16985
+
 ### Viewing Docs
 
 To view docs generated from the `docs` folder, run...
 
 ```sh
 ./scripts/slate.sh serve
 ```
```

### Comparing `frontrunner-sdk-0.1.1/backend_shim.py` & `frontrunner-sdk-0.1.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_chain.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_chain.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_faucet.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_light_client_daemon.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/clients/injective_light_client_daemon.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/openapi_client.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/base.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/find_markets.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/find_markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,39 +145,39 @@
     league_names = frozenset(self.request.league_names or [])
     event_types = frozenset(self.request.event_types or [])
     sport_entity_names = frozenset(self.request.sport_entity_names or [])
     sport_entity_abbreviations = frozenset(self.request.sport_entity_abbreviations or [])
     prop_types = frozenset(self.request.prop_types or [])
     market_statuses = frozenset(self.request.market_statuses or [])
 
-    league_ids, leagues = await self.find_leagues(deps, sports, league_names)
+    league_ids, _ = await self.find_leagues(deps, sports, league_names)
 
     if not league_ids:
       return FindMarketsResponse(
         market_ids=list([]),
         markets=[],
       )
 
     (
-      (sport_event_ids, sport_events),
-      (sport_entity_ids, sport_entities),
+      (sport_event_ids, _),
+      (sport_entity_ids, _),
     ) = await asyncio.gather(
       *[
         self.find_sport_events(deps, league_ids, event_types),
         self.find_sport_entities(deps, league_ids, sport_entity_names, sport_entity_abbreviations),
       ]
     )
 
     if not sport_event_ids or not sport_entity_ids:
       return FindMarketsResponse(
         market_ids=list([]),
         markets=[],
       )
 
-    prop_ids, props = await self.find_props(deps, league_ids, sport_event_ids, prop_types)
+    prop_ids, _ = await self.find_props(deps, league_ids, sport_event_ids, prop_types)
 
     if not prop_ids:
       return FindMarketsResponse(
         market_ids=list([]),
         markets=[],
       )
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_leagues.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_leagues.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_markets.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_props.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_props.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_entities.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sport_entities.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_events.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sport_events.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sports.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/frontrunner/get_sports.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/cancel_orders.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/cancel_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_orders.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/create_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_wallet.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/create_wallet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_account_portfolio.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_account_portfolio.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_order_books.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_order_books.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_orders.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_positions.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_positions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_trades.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/get_trades.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_markets.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_orders.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_positions.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_positions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_trades.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/commands/injective/stream_trades.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/__init__.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/base.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/chained.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/chained.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/conditional.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/conditional.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/environment_variable.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/environment_variable.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/config/static.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/config/static.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/__init__.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/base.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/facades/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/frontrunner.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/facades/frontrunner.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/injective.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/facades/injective.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,14 @@
 
   async def stream_trades(
     self,
     market_ids: Iterable[str],
     mine: bool = False,
     direction: Optional[Literal["buy", "sell"]] = None,
     side: Optional[Literal["maker", "taker"]] = None,
-    start_time: Optional[datetime] = None,
-    end_time: Optional[datetime] = None,
   ) -> StreamTradesResponse:
     kwargs = as_request_args(locals())
     request = StreamTradesRequest(**kwargs)
     return await self._run_operation(StreamTradesOperation, self.deps, request)
 
   async def stream_markets(
     self,
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/paginators.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/paginators.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/streams.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/streams.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/validation.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/helpers/validation.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/ioc.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/ioc.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_external_exceptions.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/logging/log_external_exceptions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_operation.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/logging/log_operation.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/models/order.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/models/order.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/models/wallet.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/models/wallet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/__init__.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api_client.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/api_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/configuration.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/configuration.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/error.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/error.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/market.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,40 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PropType(object):
+class SportEventType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    WINNER = "winner"
+    GAME = "game"
+    FUTURE = "future"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """PropType - a model defined in Swagger"""  # noqa: E501
+        """SportEventType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(PropType, dict):
+        if issubclass(SportEventType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PropType):
+        if not isinstance(other, SportEventType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SportEventType(object):
+class PropType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    GAME = "game"
-    FUTURE = "future"
+    WINNER = "winner"
+    OTHER = "other"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """SportEventType - a model defined in Swagger"""  # noqa: E501
+        """PropType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SportEventType, dict):
+        if issubclass(PropType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SportEventType):
+        if not isinstance(other, PropType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/rest.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/openapi/frontrunner_api/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,19 @@
             else:
                 # Cannot generate the request from given parameters
                 msg = """Cannot prepare a request message for provided
                          arguments. Please check that your arguments match
                          declared content type."""
                 raise ApiException(status=0, reason=msg)
 
-        async with self.pool_manager.request(**args) as r:
-            data = await r.text()
-            r = RESTResponse(r, data)
+        # custom code: properly open and close aiohttp connection to avoid "ERROR: Unclosed ..." logs
+        async with self.pool_manager as pm:
+            async with pm.request(**args) as r:
+                data = await r.text()
+                r = RESTResponse(r, data)
 
         # log response body
         logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk/sdk.py` & `frontrunner-sdk-0.1.2/frontrunner_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/PKG-INFO` & `frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontrunner-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Frontrunner SDK
 Home-page: https://github.com/GetFrontrunner/frontrunner-sdk
 Author: Frontrunner
 Author-email: support@getfrontrunner.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -131,20 +131,22 @@
 ```sh
 pants fmt ::
 pants fix ::
 ```
 
 ### Local Testing via REPL
 
-To get a Python shell to test code, run...
+To get a Python shell to test code, [comment out the `python_distribution` target][pants-16985] in `/BUILD`. Then run...
 
 ```sh
 pants repl ::
 ```
 
+[pants-16985]: https://github.com/pantsbuild/pants/issues/16985
+
 ### Viewing Docs
 
 To view docs generated from the `docs` folder, run...
 
 ```sh
 ./scripts/slate.sh serve
 ```
```

### Comparing `frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/SOURCES.txt` & `frontrunner-sdk-0.1.2/frontrunner_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.1/setup.py` & `frontrunner-sdk-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,22 @@
 ```sh
 pants fmt ::
 pants fix ::
 ```
 
 ### Local Testing via REPL
 
-To get a Python shell to test code, run...
+To get a Python shell to test code, [comment out the `python_distribution` target][pants-16985] in `/BUILD`. Then run...
 
 ```sh
 pants repl ::
 ```
 
+[pants-16985]: https://github.com/pantsbuild/pants/issues/16985
+
 ### Viewing Docs
 
 To view docs generated from the `docs` folder, run...
 
 ```sh
 ./scripts/slate.sh serve
 ```
@@ -213,9 +215,9 @@
         'frontrunner_sdk.models',
         'frontrunner_sdk.openapi.frontrunner_api',
         'frontrunner_sdk.openapi.frontrunner_api.api',
         'frontrunner_sdk.openapi.frontrunner_api.models',
     ),
     'python_requires': '>=3.8,<=3.10',
     'url': 'https://github.com/GetFrontrunner/frontrunner-sdk',
-    'version': '0.1.1',
+    'version': '0.1.2',
 })
```

